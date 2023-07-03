# Comparing `tmp/sac_tello-0.0.7.tar.gz` & `tmp/sac_tello-0.0.8.tar.gz`

## Comparing `sac_tello-0.0.7.tar` & `sac_tello-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/SAC-Tello.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0    13144 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/workspace.xml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/dictionaries/Michael.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/__init__.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/face_encoder.py
--rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_cmd.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_drive.py
--rw-r--r--   0        0        0    11529 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_drone.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_face_hud.py
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_hud.py
--rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_rc.py
--rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_remote.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_state.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_video.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.0.7/LICENSE
--rw-r--r--   0        0        0     7278 2020-02-02 00:00:00.000000 sac_tello-0.0.7/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sac_tello-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    48260 2020-02-02 00:00:00.000000 sac_tello-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/SAC-Tello.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0    13779 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/workspace.xml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/dictionaries/Michael.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/__init__.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/face_encoder.py
+-rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_cmd.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_drive.py
+-rw-r--r--   0        0        0    11777 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_drone.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_face_hud.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_hud.py
+-rw-r--r--   0        0        0    10953 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_rc.py
+-rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_remote.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_state.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_video.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.0.8/LICENSE
+-rw-r--r--   0        0        0     7283 2020-02-02 00:00:00.000000 sac_tello-0.0.8/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sac_tello-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    48264 2020-02-02 00:00:00.000000 sac_tello-0.0.8/PKG-INFO
```

### Comparing `sac_tello-0.0.7/.idea/workspace.xml` & `sac_tello-0.0.8/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `sac_tello-0.0.7/.idea/workspace.xml` & `sac_tello-0.0.8/.idea/workspace.xml`

```diff
@@ -1,11 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="232f03d1-54a9-425b-9ce0-d606395cbea5" name="Changes" comment="Updated readme and init file."/>
+    <list default="true" id="232f03d1-54a9-425b-9ce0-d606395cbea5" name="Changes" comment="Emergency fixes and some speed improvements">
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -13,15 +16,15 @@
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_BRANCH_BY_REPOSITORY">
       <map>
-        <entry key="$PROJECT_DIR$" value="frace_recog"/>
+        <entry key="$PROJECT_DIR$" value="main"/>
       </map>
     </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
@@ -244,30 +247,36 @@
     <task id="LOCAL-00027" summary="Updated readme and init file.">
       <created>1688069662748</created>
       <option name="number" value="00027"/>
       <option name="presentableId" value="LOCAL-00027"/>
       <option name="project" value="LOCAL"/>
       <updated>1688069662748</updated>
     </task>
-    <option name="localTasksCounter" value="28"/>
+    <task id="LOCAL-00028" summary="Emergency fixes and some speed improvements">
+      <created>1688397732767</created>
+      <option name="number" value="00028"/>
+      <option name="presentableId" value="LOCAL-00028"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688397732767</updated>
+    </task>
+    <option name="localTasksCounter" value="29"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Basic Movement commands added."/>
     <MESSAGE value="Added video controls."/>
     <MESSAGE value="Added face recognizer"/>
     <MESSAGE value="Added the ability to save known encodings."/>
     <MESSAGE value="Small change"/>
     <MESSAGE value="RC Tello in place, still needs testing"/>
     <MESSAGE value="Minor adjustments. Needs testing."/>
     <MESSAGE value="Basic updates and debugging."/>
@@ -284,10 +293,11 @@
     <MESSAGE value="Basic copy-paster setup."/>
     <MESSAGE value="Minor corrections before sleep."/>
     <MESSAGE value="RC Tello now working. Framerate not great."/>
     <MESSAGE value="README update"/>
     <MESSAGE value="Version update"/>
     <MESSAGE value="Face recognition and face hud completed."/>
     <MESSAGE value="Updated readme and init file."/>
-    <option name="LAST_COMMIT_MESSAGE" value="Updated readme and init file."/>
+    <MESSAGE value="Emergency fixes and some speed improvements"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Emergency fixes and some speed improvements"/>
   </component>
 </project>
```

### Comparing `sac_tello-0.0.7/sac_tello/face_encoder.py` & `sac_tello-0.0.8/sac_tello/face_encoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,70 +5,74 @@
 # Created On: 29 Jun 2023
 # Purpose:
 #   A simple face recognition suite.
 # Notes:
 
 import pickle
 import numpy as np
-import face_recognition
+from face_recognition import face_encodings, face_locations, face_distance
 import cv2
 
 
 class FaceEncoder:
     # Precond:
     #   encode is a string containing a file name to load a set of encodings from.
     #
     # Postcond:
     #   Creates a new FaceEncoder object loaded with encodings from a given file.
     def __init__(self, load_file=None):
         self.encodings = {}
+        # Speed upgrades
+        self.encode_scale = 1 / 4
         if load_file is not None:
             self.load(load_file)
 
     # Precond:
     #   name is a string containing the name of the person whose face is being encoded.
     #   img_file is a string containing the name of a file containing an image of a single
     #       person's face.
     #
     # Postcond:
     #   Updates the encodings based on the image file.
     #   Returns False if no face was found.
     def encode_face(self, name, img_file):
         img = cv2.imread(img_file)
+        img = cv2.resize(img, (640*self.encode_scale, 480*self.encode_scale))
         if name not in self.encodings:
             self.encodings[name] = []
-        location = face_recognition.face_locations(img)
+        location = face_locations(img)
         if len(location) > 0:
             location = location[0]
-            encoding = face_recognition.face_encodings(img, location)[0]
+            encoding = face_encodings(img, location)[0]
             self.encodings[name].append(encoding)
             return True
         return False
     
     # Precond:
     #   img is a valid ndarray representing an image.
     #   min_dist is a floating point number indicating the minimal face distance (default: 0.6) for recognition.
     #
     # Postcond:
     #   Returns the most likely name of the faces in the image, paired with their locations.
     #   If no face matches within the specified distance, then it is labeled Unknown.
     #   Returned tuples are (name, location)
     def detect_faces(self, img, min_dist=0.6):
-        locations = face_recognition.face_locations(img)
-        encodings = face_recognition.face_encodings(img, locations)
+        img = cv2.resize(img, (640 * self.encode_scale, 480 * self.encode_scale))
+        locations = face_locations(img)
+        encodings = face_encodings(img, locations)
         names = list(self.encodings.keys())
         distances = np.ones(len(names))
         idents = []
         for encoding in encodings:
             for idx, name in enumerate(names):
-                distances[idx] = face_recognition.face_distance(self.encodings[name], encoding).min()
+                distances[idx] = face_distance(self.encodings[name], encoding).min()
             if distances.min() > min_dist:
                 idents.append("unknown")
             else:
-                idents.append(names[distances.argmax()])
+                idents.append(names[distances.argmin()])
         return zip(idents, locations)
 
     # Precond:
     #   filename is the path to a file which contains serialized face encodings.
     #
     # Postcond:
     #   Updates the recognizers encodings using the provided file.
```

### Comparing `sac_tello-0.0.7/sac_tello/tello_cmd.py` & `sac_tello-0.0.8/sac_tello/tello_cmd.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.7/sac_tello/tello_drive.py` & `sac_tello-0.0.8/sac_tello/tello_drive.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # Copyright: Dr. Michael Andrew Huelsman 2023
 # License: GNU GPLv3
 # Created On: 27 Jun 2023
 # Purpose:
 #   A program for testing flying a tello drone from a ground station computer.
 # Notes:
 
-from tello_drone import TelloDrone
-from tello_rc import TelloRC
+from .tello_drone import TelloDrone
+from .tello_rc import TelloRC
 from threading import Thread
-from tello_hud import TelloHud
+from .tello_hud import TelloHud
 from time import sleep
 
 
 def drive_tello():
     drone = TelloRC()
     if not drone.start():
         print("Problem connecting.")
```

### Comparing `sac_tello-0.0.7/sac_tello/tello_drone.py` & `sac_tello-0.0.8/sac_tello/tello_drone.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,43 +13,49 @@
 
 import multiprocessing as mp
 import queue
 from time import sleep
 import sys
 from threading import Thread
 
-from tello_cmd import tello_command_loop
-from tello_state import tello_state_loop
-from tello_video import tello_video_loop
+from .tello_cmd import tello_command_loop
+from .tello_state import tello_state_loop
+from .tello_video import tello_video_loop
 
 
 class TelloDrone:
     # Precond:
     #   The computer creating the TelloDrone instance is connected to the Tello's Wi-Fi.
     #
     # Postcond:
     #   Sets up a connection with the Tello Drone.
     def __init__(self):
         # Setup command process
         self.cmdQ = mp.Queue()
         self.cmd_confQ = mp.Queue()
         self.cmd_process = mp.Process(target=tello_command_loop, args=(self.cmdQ, self.cmd_confQ))
+        self.cmd_process.daemon = True
         self.cmd_thread = Thread(target=self.__cmd_thread)
+        self.cmd_thread.daemon = True
         
         # Setup state process
         self.state_haltQ = mp.Queue()
         self.state_recQ = mp.Queue()
         self.state_process = mp.Process(target=tello_state_loop, args=(self.state_haltQ, self.state_recQ))
+        self.state_process.daemon = True
         self.state_thread = Thread(target=self.__state_thread)
+        self.state_thread.daemon = True
 
         # Setup video process
         self.video_haltQ = mp.Queue()
         self.video_recQ = mp.Queue()
         self.video_process = mp.Process(target=tello_video_loop, args=(self.video_haltQ, self.video_recQ))
+        self.video_process.daemon = True
         self.video_thread = Thread(target=self.__video_thread)
+        self.video_thread.daemon = True
         
         # Internal variables
         self.commandQ = []
         self.commandQ_limit = 10
         self.last_state = None
         self.last_frame = None
         self.running = False
```

### Comparing `sac_tello-0.0.7/sac_tello/tello_face_hud.py` & `sac_tello-0.0.8/sac_tello/tello_face_hud.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Author: Michael Huelsman
 # Copyright: Dr. Michael Andrew Huelsman 2023
 # License: GNU GPLv3
 # Created On: 29 Jun 2023
 # Purpose:
 # Notes:
 
-from tello_drone import TelloDrone
-from tello_rc import TelloRC
-from face_encoder import FaceEncoder
+from .tello_drone import TelloDrone
+from .tello_rc import TelloRC
+from .face_encoder import FaceEncoder
 from time import perf_counter
 import pygame as pg
 from threading import Thread
 
 
 class TelloFaceHud:
     def __init__(self, drone: TelloDrone | TelloRC, faces: FaceEncoder):
```

### Comparing `sac_tello-0.0.7/sac_tello/tello_hud.py` & `sac_tello-0.0.8/sac_tello/tello_hud.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Copyright: Dr. Michael Andrew Huelsman 2023
 # License: GNU GPLv3
 # Created On: 27 Jun 2023
 # Purpose:
 #   A simple hud program that can be run on a separate thread.
 # Notes:
 
-from tello_drone import TelloDrone
-from tello_rc import TelloRC
+from .tello_drone import TelloDrone
+from .tello_rc import TelloRC
 from time import perf_counter, sleep
 import pygame as pg
 from math import sin, cos, radians
 from threading import Thread
 
 
 class TelloHud:
@@ -20,26 +20,27 @@
         self.drone = drone
         self.running = False
         self.hud_thread = Thread(target=self.__hud_stream)
         self.hud_thread.daemon = True
         # Create base visuals for hud
         self.hud_rad = 50
         self.hud_base = pg.Surface((4*self.hud_rad, 4*self.hud_rad), pg.SRCALPHA, 32)
-        hud_center = self.BasicVec(self.hud_base.get_width() // 2, self.hud_base.get_height() // 2)
-        pg.draw.circle(self.hud_base, (0, 0, 0, 100), hud_center.to_tuple(), 2*self.hud_rad)
+        hud_center = pg.Vector2(self.hud_base.get_width() // 2, self.hud_base.get_height() // 2)
+        pg.draw.circle(self.hud_base, (0, 0, 0, 100), hud_center, 2*self.hud_rad)
         # Draw baselines
-        pg.draw.circle(self.hud_base, (0, 200, 0), hud_center.to_tuple(), self.hud_rad, self.hud_rad // 10)
+        pg.draw.circle(self.hud_base, (0, 200, 0), hud_center, self.hud_rad, self.hud_rad // 10)
         # Roll baseline
-        roll_baseline = self.BasicVec(cos(0), sin(0))
-        roll_start = roll_baseline.scale(self.hud_rad).add(hud_center)
-        roll_end = roll_baseline.scale(2 * self.hud_rad).add(hud_center)
-        pg.draw.line(self.hud_base, (0, 200, 0), roll_start.to_tuple(), roll_end.to_tuple(), 6)
-        roll_start = roll_baseline.neg().scale(self.hud_rad).add(hud_center)
-        roll_end = roll_baseline.neg().scale(2 * self.hud_rad).add(hud_center)
-        pg.draw.line(self.hud_base, (0, 200, 0), roll_start.to_tuple(), roll_end.to_tuple(), 6)
+        roll_baseline = pg.Vector2(cos(0), sin(0))
+        roll_start = (roll_baseline * self.hud_rad) + hud_center
+        roll_end = (roll_baseline * (2 * self.hud_rad)) + hud_center
+        pg.draw.line(self.hud_base, (0, 200, 0), roll_start, roll_end, 6)
+        roll_baseline - -roll_baseline
+        roll_start = (roll_baseline * self.hud_rad) + hud_center
+        roll_end = (roll_baseline * (2 * self.hud_rad)) + hud_center
+        pg.draw.line(self.hud_base, (0, 200, 0), roll_start, roll_end, 6)
     
     def activate_hud(self):
         if self.running:
             return
         self.running = True
         self.hud_thread.start()
         
@@ -58,15 +59,15 @@
         # Setup Pygame
         pg.display.init()
         screen = pg.display.set_mode((640, 480))
         pg.font.init()
         hud_font = pg.font.Font(pg.font.get_default_font(), 20)
         # Setup video loop basics
         frame_timer = perf_counter()
-        frame_delta = 1/24
+        frame_delta = 1/30
         while self.running:
             if (perf_counter() - frame_timer) > frame_delta:
                 frame_timer = perf_counter()
                 frame = self.drone.get_frame()
                 if frame is not None:
                     frame = frame[0]
                     frame = pg.image.frombuffer(frame.tobytes(), frame.shape[1::-1], "BGR")
@@ -82,33 +83,33 @@
                     horizon_pos = (screen.get_width() - horizon.get_width())//2, (screen.get_height() - horizon.get_height())//2
                     screen.blit(horizon, horizon_pos)
                 pg.display.flip()
                 for event in pg.event.get(pg.QUIT):
                     self.running = False
         pg.display.quit()
         
-    def __artificial_horizon(self, rad: int, pitch:int, roll: int):
+    def __artificial_horizon(self, rad: int, pitch: int, roll: int):
         result = pg.surface.Surface((4*rad, 4*rad), pg.SRCALPHA, 32)
         result.blit(self.hud_base, (0, 0))
-        center = self.BasicVec(result.get_width() // 2, result.get_height() // 2)
+        center = pg.Vector2(result.get_width() // 2, result.get_height() // 2)
         # Draw roll lines]
         left_ang = radians(180 + roll)
-        left_vec = self.BasicVec(cos(left_ang), sin(left_ang))
-        left_start = left_vec.scale(rad)
-        left_end = left_vec.scale(rad*2)
-        left_start = left_start.add(center)
-        left_end = left_end.add(center)
-        pg.draw.line(result, (0, 200, 0), left_start.to_tuple(), left_end.to_tuple(), 3)
+        left_vec = pg.Vector2(cos(left_ang), sin(left_ang))
+        left_start = left_vec * rad
+        left_end = left_vec * (rad*2)
+        left_start = left_start + center
+        left_end = left_end + center
+        pg.draw.line(result, (0, 200, 0), left_start, left_end, 3)
         right_ang = radians(roll)
-        right_vec = self.BasicVec(cos(right_ang), sin(right_ang))
-        right_start = right_vec.scale(rad)
-        right_end = right_vec.scale(rad * 2)
-        right_start = right_start.add(center)
-        right_end = right_end.add(center)
-        pg.draw.line(result, (0, 200, 0), right_start.to_tuple(), right_end.to_tuple(), 3)
+        right_vec = pg.Vector2(cos(right_ang), sin(right_ang))
+        right_start = right_vec * rad
+        right_end = right_vec * rad * 2
+        right_start = right_start + center
+        right_end = right_end + center
+        pg.draw.line(result, (0, 200, 0), right_start, right_end, 3)
         # Draw Pitch lines
         pitch = -pitch # Line direction adjustment
         pitch_line_deg = 10
         pitch_lines = pg.Surface((rad, rad), pg.SRCALPHA)
         pixels_per_ang = 2
         start_angle = pitch - ((pitch_lines.get_height()//2)//pixels_per_ang)
         pixel_start = pitch_line_deg - (start_angle % pitch_line_deg)
@@ -118,34 +119,15 @@
             ang = start_angle + (i // pixels_per_ang)
             angles.append(ang)
             if ang % pitch_line_deg == 0:
                 if ang != 0:
                     pg.draw.line(pitch_lines, (0, 200, 0), (0, i), (pitch_lines.get_width(), i), 3)
                 else:
                     pg.draw.line(pitch_lines, (200, 0, 0), (0, i), (pitch_lines.get_width(), i), 3)
-        center_pitch = center.add((-(pitch_lines.get_width()//2), -(pitch_lines.get_height()//2)))
+        line_adj = pg.Vector2(-(pitch_lines.get_width()//2), -(pitch_lines.get_height()//2))
+        center_pitch = center + line_adj
         # Current Pitch indicator
         indicator_height = pitch_lines.get_height()//2
         pg.draw.line(pitch_lines, (0, 0, 200), (0, indicator_height), (pitch_lines.get_width(), indicator_height), 3)
-        result.blit(pitch_lines, center_pitch.to_tuple())
+        result.blit(pitch_lines, center_pitch)
         return result
-    
-    class BasicVec:
-        def __init__(self, x, y):
-            self.x = x
-            self.y = y
-        
-        def add(self, other):
-            if type(other) == TelloHud.BasicVec:
-                return TelloHud.BasicVec(self.x+other.x, self.y+other.y)
-            elif type(other) == tuple:
-                return TelloHud.BasicVec(self.x+other[0], self.y+other[1])
-            
-        def scale(self, n):
-            return TelloHud.BasicVec(self.x*n, self.y*n)
-        
-        def neg(self):
-            return TelloHud.BasicVec(-self.x, -self.y)
-        
-        def to_tuple(self):
-            return self.x, self.y
-            
+
```

### Comparing `sac_tello-0.0.7/sac_tello/tello_rc.py` & `sac_tello-0.0.8/sac_tello/tello_rc.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,49 +12,54 @@
 import queue
 from time import perf_counter
 from math import log1p
 import pygame as pg
 import sys
 from threading import Thread
 
-from tello_remote import tello_remote_loop
-from tello_state import tello_state_loop
-from tello_video import tello_video_loop
+from .tello_remote import tello_remote_loop
+from .tello_state import tello_state_loop
+from .tello_video import tello_video_loop
 
 
 class TelloRC:
     # Precond:
     #   The computer creating the TelloDrone instance is connected to the Tello's Wi-Fi.
     #
     # Postcond:
     #   Sets up a connection with the Tello Drone.
     def __init__(self):
         # Setup command process
         self.rcQ = mp.Queue()
         self.rc_confQ = mp.Queue()
         self.rc_process = mp.Process(target=tello_remote_loop, args=(self.rcQ, self.rc_confQ))
+        self.rc_process.daemon = True
         
         # Setup state process
         self.state_haltQ = mp.Queue()
         self.state_recQ = mp.Queue()
         self.state_process = mp.Process(target=tello_state_loop, args=(self.state_haltQ, self.state_recQ))
+        self.state_process.daemon = True
         self.state_thread = Thread(target=self.__state_thread)
+        self.state_thread.daemon = True
         
         # Setup video process
         self.video_haltQ = mp.Queue()
         self.video_recQ = mp.Queue()
         self.video_process = mp.Process(target=tello_video_loop, args=(self.video_haltQ, self.video_recQ))
+        self.video_process.daemon = True
         self.video_thread = Thread(target=self.__video_thread)
+        self.video_thread.daemon = True
         
         # Internal variables
         self.current_rc = [0, 0, 0, 0]
         self.last_state = None
         self.last_frame = None
         self.running = False
-        self.vel_timing = 5
+        self.vel_timing = 10
 
     # ==========================
     #   MANAGEMENT METHODS
     # ==========================
 
     # Precond:
     #   None.
@@ -71,17 +76,17 @@
         self.state_process.start()
         self.video_thread.start()
         self.video_process.start()
         return True
     
     def control(self):
         # Setup
-        key_holds = {'w': 0, 's': 0, 'd': 0, 'a': 0, 'q': 0, 'e': 0, 'up': 0, 'down': 0}
+        key_holds = {'w': 0, 's': 0, 'd': 0, 'a': 0, 'q': 0, 'e': 0, 'r': 0, 'f': 0}
         poll_timer = perf_counter()
-        poll_delta = 1/16
+        poll_delta = 1/30
         # Main Loop
         control_running = True
         pg.init()
         while control_running:
             delta = perf_counter() - poll_timer
             if delta >= poll_delta:
                 # Check for events
@@ -97,28 +102,46 @@
                             print("Problem with landing!")
                     elif event.key == pg.K_ESCAPE:
                         command_sent = True
                         if not self.emergency():
                             print("Problem with emergency shutdown!")
                     elif event.key == pg.K_BACKSPACE:
                         control_running = False
+                    elif event.key == pg.K_DELETE:
+                        self.rcQ.put((0, 0, 0, 0))
+                    elif event.key == pg.K_UP:
+                        command_sent = True
+                        if not self.flip_forward():
+                            print("Problem with forward flip!")
+                    elif event.key == pg.K_DOWN:
+                        command_sent = True
+                        if not self.flip_backward():
+                            print("Problem with backward flip!")
+                    elif event.key == pg.K_RIGHT:
+                        command_sent = True
+                        if not self.flip_right():
+                            print("Problem with right flip!")
+                    elif event.key == pg.K_LEFT:
+                        command_sent = True
+                        if not self.flip_left():
+                            print("Problem with left flip!")
                 if command_sent:
                     poll_timer = perf_counter()
                     continue
                 # Deal with held keys
                 key_state = pg.key.get_pressed()
                 for key in key_holds:
                     if key_state[pg.key.key_code(key)]:
                         key_holds[key] += delta
                     else:
                         key_holds[key] -= delta
                     key_holds[key] = max(0, min(self.vel_timing, key_holds[key]))
                 y = self.__vel_curve(key_holds['w']) - self.__vel_curve(key_holds['s'])
                 x = self.__vel_curve(key_holds['d']) - self.__vel_curve(key_holds['a'])
-                z = self.__vel_curve(key_holds['up']) - self.__vel_curve(key_holds['down'])
+                z = self.__vel_curve(key_holds['r']) - self.__vel_curve(key_holds['f'])
                 rot = self.__vel_curve(key_holds['e']) - self.__vel_curve(key_holds['q'])
                 if self.rcQ.empty():
                     self.rcQ.put((int(x), int(y), int(z), int(rot)))
     
     # Precond:
     #   None.
     #
@@ -186,14 +209,74 @@
         try:
             conf = self.rc_confQ.get(block=True, timeout=5)
             if not conf[0]:
                 return False
         except queue.Empty:
             return False
         return True
+
+    # Precond:
+    #   None.
+    #
+    # Postcond:
+    #   Adds flip l command to the command queue.
+    def flip_left(self):
+        self.rcQ.put("flip l")
+        try:
+            conf = self.rc_confQ.get(block=True, timeout=5)
+            if not conf[0]:
+                return False
+        except queue.Empty:
+            return False
+        return True
+
+    # Precond:
+    #   None.
+    #
+    # Postcond:
+    #   Adds flip r command to the command queue.
+    def flip_right(self):
+        self.rcQ.put("flip r")
+        try:
+            conf = self.rc_confQ.get(block=True, timeout=5)
+            if not conf[0]:
+                return False
+        except queue.Empty:
+            return False
+        return True
+
+    # Precond:
+    #   None.
+    #
+    # Postcond:
+    #   Adds flip f command to the command queue.
+    def flip_forward(self):
+        self.rcQ.put("flip f")
+        try:
+            conf = self.rc_confQ.get(block=True, timeout=5)
+            if not conf[0]:
+                return False
+        except queue.Empty:
+            return False
+        return True
+
+    # Precond:
+    #   None.
+    #
+    # Postcond:
+    #   Adds flip b command to the command queue.
+    def flip_backward(self):
+        self.rcQ.put("flip b")
+        try:
+            conf = self.rc_confQ.get(block=True, timeout=5)
+            if not conf[0]:
+                return False
+        except queue.Empty:
+            return False
+        return True
 
     # ======================================
     # Info METHODS
     # ======================================
 
     # Precond:
     #   None.
```

### Comparing `sac_tello-0.0.7/sac_tello/tello_remote.py` & `sac_tello-0.0.8/sac_tello/tello_remote.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,22 @@
                 running = False
             elif current == "takeoff":
                 manager.takeoff()
             elif current == "land":
                 manager.land()
             elif current == "emergency":
                 manager.emergency()
+            elif current == "flip f":
+                manager.flip_forward()
+            elif current == "flip b":
+                manager.flip_backward()
+            elif current == "flip r":
+                manager.flip_right()
+            elif current == "flip l":
+                manager.flip_left()
         elif type(current) == tuple:
             manager.set_rc(*current)
     try:
         while not rc_q.empty():
             rc_q.get_nowait()
     except queue.Empty:
         pass
```

### Comparing `sac_tello-0.0.7/sac_tello/tello_state.py` & `sac_tello-0.0.8/sac_tello/tello_state.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.7/sac_tello/tello_video.py` & `sac_tello-0.0.8/sac_tello/tello_video.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.7/.gitignore` & `sac_tello-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.7/LICENSE` & `sac_tello-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.7/README.md` & `sac_tello-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 > opencv-python>=4.6.0.66
 > 
 > face_recognition>=1.3.0
 > 
 > pygame>=2.2.0
 
 ### Install
-SAC-Tello can be install by running the following command:
+SAC-Tello can be installed by running the following command:
 ```commandline
-python3 -m pip install SAC-Tell0
+python3 -m pip install SAC-Tello
 ```
 for MacOS/Linux
 
 Or
 ```commandline
 python -m pip install SAC-Tello
 ```
@@ -182,24 +182,25 @@
 drone.control()
 drone.close()
 ```
 
 The `control()` method begins polling loop for keyboard input. The controls
 are as follows:
 
-| Key Press  | Effect                |
-|------------|-----------------------|
-| T          | Takeoff               |
-| L          | Land                  |
-| ESCAPE     | Emergency Kill Switch | 
-| BACKSPACE  | End Remote Control    |
-
-| Key Held    | Effect                      |
-|-------------|-----------------------------|
-| W           | Increase Forward Velocity   |
-| A           | Increase Leftward Velocity  |
-| S           | Increase Backward Velocity  |
-| D           | Increase Rightward Velocity |
-| Q           | Rotate Counterclockwise     |
-| E           | Rotate Clockwise            |
-| Up Arrow    | Increase Hover Height       |
-| Down Arrow  | Decrease Hover Height       |
+| Key Press | Effect                |
+|-----------|-----------------------|
+| T         | Takeoff               |
+| L         | Land                  |
+| ESCAPE    | Emergency Kill Switch | 
+| BACKSPACE | End Remote Control    |
+| DELETE    | Zero Velocity         |
+
+| Key Held | Effect                      |
+|----------|-----------------------------|
+| W        | Increase Forward Velocity   |
+| A        | Increase Leftward Velocity  |
+| S        | Increase Backward Velocity  |
+| D        | Increase Rightward Velocity |
+| Q        | Rotate Counterclockwise     |
+| E        | Rotate Clockwise            |
+| R        | Increase Hover Height       |
+| F        | Decrease Hover Height       |
```

### Comparing `sac_tello-0.0.7/pyproject.toml` & `sac_tello-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "SAC-Tello"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Michael Huelsman", email="michael.huelsman@gmail.com" },
 ]
 description = "A Python-based DJI Tello interface which utilizes parallel processing."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

### Comparing `sac_tello-0.0.7/PKG-INFO` & `sac_tello-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAC-Tello
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python-based DJI Tello interface which utilizes parallel processing.
 Project-URL: Homepage, https://github.com/xLeachimx/SAC-Tello
 Project-URL: Bug Tracker, https://github.com/xLeachimx/SAC-Tello/issues
 Author-email: Michael Huelsman <michael.huelsman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -699,17 +699,17 @@
 > opencv-python>=4.6.0.66
 > 
 > face_recognition>=1.3.0
 > 
 > pygame>=2.2.0
 
 ### Install
-SAC-Tello can be install by running the following command:
+SAC-Tello can be installed by running the following command:
 ```commandline
-python3 -m pip install SAC-Tell0
+python3 -m pip install SAC-Tello
 ```
 for MacOS/Linux
 
 Or
 ```commandline
 python -m pip install SAC-Tello
 ```
@@ -873,24 +873,25 @@
 drone.control()
 drone.close()
 ```
 
 The `control()` method begins polling loop for keyboard input. The controls
 are as follows:
 
-| Key Press  | Effect                |
-|------------|-----------------------|
-| T          | Takeoff               |
-| L          | Land                  |
-| ESCAPE     | Emergency Kill Switch | 
-| BACKSPACE  | End Remote Control    |
-
-| Key Held    | Effect                      |
-|-------------|-----------------------------|
-| W           | Increase Forward Velocity   |
-| A           | Increase Leftward Velocity  |
-| S           | Increase Backward Velocity  |
-| D           | Increase Rightward Velocity |
-| Q           | Rotate Counterclockwise     |
-| E           | Rotate Clockwise            |
-| Up Arrow    | Increase Hover Height       |
-| Down Arrow  | Decrease Hover Height       |
+| Key Press | Effect                |
+|-----------|-----------------------|
+| T         | Takeoff               |
+| L         | Land                  |
+| ESCAPE    | Emergency Kill Switch | 
+| BACKSPACE | End Remote Control    |
+| DELETE    | Zero Velocity         |
+
+| Key Held | Effect                      |
+|----------|-----------------------------|
+| W        | Increase Forward Velocity   |
+| A        | Increase Leftward Velocity  |
+| S        | Increase Backward Velocity  |
+| D        | Increase Rightward Velocity |
+| Q        | Rotate Counterclockwise     |
+| E        | Rotate Clockwise            |
+| R        | Increase Hover Height       |
+| F        | Decrease Hover Height       |
```

