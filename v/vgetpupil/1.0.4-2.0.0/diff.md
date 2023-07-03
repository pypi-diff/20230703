# Comparing `tmp/vgetpupil-1.0.4.tar.gz` & `tmp/vgetpupil-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgetpupil-1.0.4.tar", last modified: Thu Jun 29 22:49:06 2023, max compression
+gzip compressed data, was "vgetpupil-2.0.0.tar", last modified: Mon Jul  3 00:05:34 2023, max compression
```

## Comparing `vgetpupil-1.0.4.tar` & `vgetpupil-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/
--rw-rw-rw-   0        0        0    11558 2023-03-26 20:13:24.000000 vgetpupil-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      617 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-03-26 20:13:24.000000 vgetpupil-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1026 2023-06-29 22:48:43.000000 vgetpupil-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil/
--rw-rw-rw-   0        0        0     8072 2023-06-29 22:47:04.000000 vgetpupil-1.0.4/vgetpupil/vget.py
--rw-rw-rw-   0        0        0        0 2023-03-26 20:13:24.000000 vgetpupil-1.0.4/vgetpupil/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 22:49:01.000000 vgetpupil-1.0.4/vgetpupil.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      617 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/requires.txt
--rw-rw-rw-   0        0        0      298 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-06-29 22:49:06.000000 vgetpupil-1.0.4/vgetpupil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 00:05:34.243682 vgetpupil-2.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-02 22:18:08.000000 vgetpupil-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      617 2023-07-03 00:05:34.243682 vgetpupil-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-02 22:18:08.000000 vgetpupil-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 00:05:34.243682 vgetpupil-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-07-02 23:31:59.000000 vgetpupil-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:05:34.236228 vgetpupil-2.0.0/vgetpupil/
+-rw-rw-rw-   0        0        0        0 2023-07-02 22:18:09.000000 vgetpupil-2.0.0/vgetpupil/__init__.py
+-rw-rw-rw-   0        0        0     1901 2023-07-02 22:18:09.000000 vgetpupil-2.0.0/vgetpupil/detector.py
+-rw-rw-rw-   0        0        0     9315 2023-07-03 00:02:39.000000 vgetpupil-2.0.0/vgetpupil/vget.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:05:34.242684 vgetpupil-2.0.0/vgetpupil.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-07-03 00:05:34.000000 vgetpupil-2.0.0/vgetpupil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-03 00:05:34.000000 vgetpupil-2.0.0/vgetpupil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 00:05:34.000000 vgetpupil-2.0.0/vgetpupil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-03 00:05:34.000000 vgetpupil-2.0.0/vgetpupil.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-02 22:18:09.000000 vgetpupil-2.0.0/vgetpupil.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-07-03 00:05:34.000000 vgetpupil-2.0.0/vgetpupil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 00:05:34.000000 vgetpupil-2.0.0/vgetpupil.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vgetpupil-1.0.4/LICENSE` & `vgetpupil-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vgetpupil-1.0.4/PKG-INFO` & `vgetpupil-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgetpupil
-Version: 1.0.4
+Version: 2.0.0
 Summary: pupil positions generator program
 Home-page: https://github.com/jtur044/vgetpupil.git
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: pupil positions generator program vgetpupil
 Platform: UNKNOWN
```

### Comparing `vgetpupil-1.0.4/README.md` & `vgetpupil-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vgetpupil-1.0.4/setup.py` & `vgetpupil-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to write the pupil positions data from input videos.'
 
 setup(
     name='vgetpupil',
-    version='1.0.4',
+    version='2.0.0',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/vgetpupil.git',
     description='pupil positions generator program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

### Comparing `vgetpupil-1.0.4/vgetpupil/vget.py` & `vgetpupil-2.0.0/vgetpupil/vget.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import sys
 import cv2
 import csv
 import time
 from pupil_detectors import Detector2D
+import json
 
 detector = Detector2D()
 
 
 # This function is to display progressive bar
 def print_percent_done(index_input, total, bar_len=50, title_input='Please wait'):
     percent_done = (index_input + 1) / total * 100
@@ -26,29 +27,52 @@
 def frame_to_time(frame_number, frame_rate):
     return frame_number / frame_rate
 
 
 def main():
     parser = argparse.ArgumentParser(prog='vgetpupil',
                                      description='VGETPUPIL package.')
-    parser.add_argument('--version', action='version', version='1.0.4'),
+    parser.add_argument('--version', action='version', version='2.0.0'),
     parser.add_argument("-i", dest="input_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
                         help="input mp4 file", metavar="filename.mp4")
     parser.add_argument("-o", dest="output_filename", required=True, type=argparse.FileType('w'), default=sys.stdout,
                         help="output csv file", metavar="filename.csv")
     parser.add_argument("-e", dest="eye_id_input", required=False, type=int, default=None, help="eye id input",
                         metavar="0 or 1")
+    parser.add_argument("-c", dest="config_input", required=False, help="config input",
+                        metavar="config file to adjust pupil detectors")
 
     args = parser.parse_args()
     input_file = args.input_filename.name
     output_file = args.output_filename.name
     eye_id_input_from_user = args.eye_id_input
+    config_file = args.config_input
     eye_side_input = None
     convert_able = True
 
+    if config_file:
+        detector_properties = Detector2D.get_properties(detector)
+        print("<Default Detector Properties>")
+        print(detector_properties)
+        try:
+            with open(str(config_file)) as f:
+                config_info = json.load(f)
+                print("<Config Detector Properties>")
+                print(config_info)
+                detector_properties = config_info
+            Detector2D.update_properties(detector, detector_properties)
+            updated_properties = Detector2D.get_properties(detector)
+            print("<Updated Detector Properties>")
+            print(updated_properties)
+        except Exception as error:
+            print(f"Error in retrieving info from config file:{config_file}!")
+            print(error)
+
+            return
+
     # Define conditions to decide input mp4 is left or right eye video
     left_eye_indicated_string = "left" in str(input_file).lower() or "0" in str(input_file).lower()
     right_eye_indicated_string = "right" in str(input_file).lower() or "1" in str(input_file).lower()
 
     # Handle error for type of input file
     if str(input_file).endswith(".mp4"):
         if eye_id_input_from_user == 0 or eye_id_input_from_user == 1:
@@ -104,16 +128,16 @@
         frame_rate = input_video.get(cv2.CAP_PROP_FPS)
         print("Input frame rate:", frame_rate)
         frame_count = input_video.get(cv2.CAP_PROP_FRAME_COUNT)
         print("Input frame count:", frame_count)
 
         # Open the output file to write the data
         with open(output_file, mode='w', newline="") as destination_file:
-            header_names = ["pupil_time", "eye_id", "confidence", "norm_pos_x",
-                            "norm_pos_y", "diameter", "ellipse_center_x", "ellipse_center_y",
+            header_names = ["pupil_time", "record_timestamp", "direction", "eye_id", "confidence", "x_nom",
+                            "y_nom", "diameter", "ellipse_center_x", "ellipse_center_y",
                             "ellipse_axis_a", "ellipse_axis_b", "ellipse_angle"]
             csv_writer = csv.DictWriter(destination_file, fieldnames=header_names)
             csv_writer.writeheader()
 
             w_start = time.time()
             count = 0
 
@@ -143,25 +167,29 @@
                     ellipse_center_y = ellipse["center"][1]
                     ellipse_axis_a = ellipse["axes"][0]
                     ellipse_axis_b = ellipse["axes"][0]
                     ellipse_angle = ellipse["angle"]
                     diameter = result["diameter"]
                     x_nom = ellipse_center_x / 192
                     y_nom = ellipse_center_y / 192
-                    csv_writer.writerow({"pupil_time": pupil_time,
-                                         "eye_id": eye_id,
-                                         "confidence": confidence,
-                                         "norm_pos_x": x_nom,
-                                         "norm_pos_y": y_nom,
-                                         "diameter": diameter,
-                                         "ellipse_center_x": ellipse_center_x,
-                                         "ellipse_center_y": ellipse_center_y,
-                                         "ellipse_axis_a": ellipse_axis_a,
-                                         "ellipse_axis_b": ellipse_axis_b,
-                                         "ellipse_angle": ellipse_angle, })
+                    direction_input = "unknown"
+                    data_to_write = {"pupil_time": pupil_time,
+                                     "record_timestamp": pupil_time,
+                                     "direction": direction_input,
+                                     "eye_id": eye_id,
+                                     "confidence": confidence,
+                                     "x_nom": x_nom,
+                                     "y_nom": y_nom,
+                                     "diameter": diameter,
+                                     "ellipse_center_x": ellipse_center_x,
+                                     "ellipse_center_y": ellipse_center_y,
+                                     "ellipse_axis_a": ellipse_axis_a,
+                                     "ellipse_axis_b": ellipse_axis_b,
+                                     "ellipse_angle": ellipse_angle, }
+                    csv_writer.writerow(data_to_write)
                     # print(f"process time {(time.time() - cur_time) * 1000}")
                     # print(f"one loop time {(time.time() - r_start) * 1000}")
 
                 # When there is no frame to read
                 else:
                     input_video.release()
                     cv2.destroyAllWindows()
```

### Comparing `vgetpupil-1.0.4/vgetpupil.egg-info/PKG-INFO` & `vgetpupil-2.0.0/vgetpupil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgetpupil
-Version: 1.0.4
+Version: 2.0.0
 Summary: pupil positions generator program
 Home-page: https://github.com/jtur044/vgetpupil.git
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: pupil positions generator program vgetpupil
 Platform: UNKNOWN
```

