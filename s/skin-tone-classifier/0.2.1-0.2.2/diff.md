# Comparing `tmp/skin-tone-classifier-0.2.1.tar.gz` & `tmp/skin-tone-classifier-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skin-tone-classifier-0.2.1.tar", last modified: Sun Jun 18 15:39:08 2023, max compression
+gzip compressed data, was "skin-tone-classifier-0.2.2.tar", last modified: Sun Jul  2 22:06:59 2023, max compression
```

## Comparing `skin-tone-classifier-0.2.1.tar` & `skin-tone-classifier-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-18 15:39:08.461399 skin-tone-classifier-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/src/stone/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/src/stone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/src/stone/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/src/stone/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/src/stone/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.895243 skin-tone-classifier-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 22:06:46.000000 skin-tone-classifier-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18615 2023-07-02 22:06:59.895243 skin-tone-classifier-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17698 2023-07-02 22:06:46.000000 skin-tone-classifier-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 22:06:59.895243 skin-tone-classifier-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-02 22:06:46.000000 skin-tone-classifier-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.895243 skin-tone-classifier-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.895243 skin-tone-classifier-0.2.2/src/skin_tone_classifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18615 2023-07-02 22:06:59.000000 skin-tone-classifier-0.2.2/src/skin_tone_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-02 22:06:59.000000 skin-tone-classifier-0.2.2/src/skin_tone_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:06:59.000000 skin-tone-classifier-0.2.2/src/skin_tone_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 22:06:59.000000 skin-tone-classifier-0.2.2/src/skin_tone_classifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:06:59.000000 skin-tone-classifier-0.2.2/src/skin_tone_classifier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 22:06:59.000000 skin-tone-classifier-0.2.2/src/skin_tone_classifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 22:06:59.000000 skin-tone-classifier-0.2.2/src/skin_tone_classifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.895243 skin-tone-classifier-0.2.2/src/stone/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-02 22:06:46.000000 skin-tone-classifier-0.2.2/src/stone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-02 22:06:46.000000 skin-tone-classifier-0.2.2/src/stone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-07-02 22:06:46.000000 skin-tone-classifier-0.2.2/src/stone/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-02 22:06:46.000000 skin-tone-classifier-0.2.2/src/stone/utils.py
```

### Comparing `skin-tone-classifier-0.2.1/LICENSE` & `skin-tone-classifier-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skin-tone-classifier-0.2.1/PKG-INFO` & `skin-tone-classifier-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skin-tone-classifier
-Version: 0.2.1
+Version: 0.2.2
 Summary: An easy-to-use library for skin tone classification
 Home-page: https://chenglongma.com/SkinToneClassifier/
 Author: Chenglong Ma
 Author-email: chenglong.m@outlook.com
 Project-URL: Documentation, https://chenglongma.com/SkinToneClassifier/
 Project-URL: Code, https://github.com/ChenglongMa/SkinToneClassifier
 Project-URL: Issue tracker, https://github.com/ChenglongMa/SkinToneClassifier/issues
@@ -69,15 +69,15 @@
 5. 🐛 **FIX!**: We fix the bug that the app will crash when the input image has dimensionality errors.
     * Now, the app won't crash and will report the error message in `./result.csv`.
 
 # Citation
 
 If you are interested in our work, please cite:
 
-```text
+```bibtex
 @article{https://doi.org/10.1111/ssqu.13242,
 author = {Rej\'{o}n Pi\tilde{n}a, Ren\'{e} Alejandro and Ma, Chenglong},
 title = {Classification Algorithm for Skin Color (CASCo): A new tool to measure skin color in social science research},
 journal = {Social Science Quarterly},
 volume = {n/a},
 number = {n/a},
 pages = {},
```

### Comparing `skin-tone-classifier-0.2.1/README.md` & `skin-tone-classifier-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 5. 🐛 **FIX!**: We fix the bug that the app will crash when the input image has dimensionality errors.
     * Now, the app won't crash and will report the error message in `./result.csv`.
 
 # Citation
 
 If you are interested in our work, please cite:
 
-```text
+```bibtex
 @article{https://doi.org/10.1111/ssqu.13242,
 author = {Rej\'{o}n Pi\tilde{n}a, Ren\'{e} Alejandro and Ma, Chenglong},
 title = {Classification Algorithm for Skin Color (CASCo): A new tool to measure skin color in social science research},
 journal = {Social Science Quarterly},
 volume = {n/a},
 number = {n/a},
 pages = {},
@@ -342,8 +342,8 @@
 
 #### 8. Multiprocessing settings
 
 ```shell
 stone --n_workers <Any Positive Integer>
 ```
 
-Use `--n_workers` to specify the number of workers to process images in parallel, defaults to the number of CPUs in your system.
+Use `--n_workers` to specify the number of workers to process images in parallel, defaults to the number of CPUs in your system.
```

### Comparing `skin-tone-classifier-0.2.1/setup.py` & `skin-tone-classifier-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 with open('README.md') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name='skin-tone-classifier',
     version=VERSION,
```

### Comparing `skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/PKG-INFO` & `skin-tone-classifier-0.2.2/src/skin_tone_classifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skin-tone-classifier
-Version: 0.2.1
+Version: 0.2.2
 Summary: An easy-to-use library for skin tone classification
 Home-page: https://chenglongma.com/SkinToneClassifier/
 Author: Chenglong Ma
 Author-email: chenglong.m@outlook.com
 Project-URL: Documentation, https://chenglongma.com/SkinToneClassifier/
 Project-URL: Code, https://github.com/ChenglongMa/SkinToneClassifier
 Project-URL: Issue tracker, https://github.com/ChenglongMa/SkinToneClassifier/issues
@@ -69,15 +69,15 @@
 5. 🐛 **FIX!**: We fix the bug that the app will crash when the input image has dimensionality errors.
     * Now, the app won't crash and will report the error message in `./result.csv`.
 
 # Citation
 
 If you are interested in our work, please cite:
 
-```text
+```bibtex
 @article{https://doi.org/10.1111/ssqu.13242,
 author = {Rej\'{o}n Pi\tilde{n}a, Ren\'{e} Alejandro and Ma, Chenglong},
 title = {Classification Algorithm for Skin Color (CASCo): A new tool to measure skin color in social science research},
 journal = {Social Science Quarterly},
 volume = {n/a},
 number = {n/a},
 pages = {},
```

### Comparing `skin-tone-classifier-0.2.1/src/stone/__main__.py` & `skin-tone-classifier-0.2.2/src/stone/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         image_type = 'bw' if is_bw else 'color'
     if len(specified_palette) == 0:
         skin_tone_palette = default_palette['bw' if to_bw or is_bw else 'color']
     else:
         skin_tone_palette = specified_palette
 
     tone_labels = specified_tone_labels or default_tone_labels['bw' if to_bw or is_bw else 'color']
-    assert len(skin_tone_palette) == len(tone_labels), 'argument -p/--palette and -l/--labels must have the same length.'
+    if len(skin_tone_palette) != len(tone_labels):
+        raise ValueError('argument -p/--palette and -l/--labels must have the same length.')
 
     try:
         records, report_images = process(image, is_bw, to_bw, skin_tone_palette, tone_labels,
                                          new_width=new_width, n_dominant_colors=n_dominant_colors,
                                          scaleFactor=scale, minNeighbors=min_nbrs, minSize=min_size, verbose=verbose)
         return {
             'basename': basename,
```

### Comparing `skin-tone-classifier-0.2.1/src/stone/image.py` & `skin-tone-classifier-0.2.2/src/stone/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     prop_strs = ['%.2f' % p for p in dmnt_props]
     result = list(np.hstack(list(zip(hex_colors, prop_strs))))
     # Calculate skin tone
     tone_id, tone_hex, PERLA, distance = skin_tone(dmnt_colors, dmnt_props, skin_tone_palette, tone_labels)
     accuracy = round(100 - distance, 2)
     result.extend([tone_hex, PERLA, accuracy])
     if not verbose:
-        return result,
+        return result, None
 
     # 0. Create initial report image
     report_image = initial_report_image(image, report_image, skin_mask, use_face, to_bw)
     bar_width = 100
 
     # 1. Create color bar for dominant colors
     color_bars = create_dominant_color_bar(report_image, dmnt_colors, dmnt_props, bar_width)
@@ -314,14 +314,16 @@
 def show(image):
     cv2.imshow('image', image)
     cv2.waitKey(0)
     cv2.destroyAllWindows()
 
 
 def face_report_image(face, idx, image):
+    if image is None:
+        return None
     x1, y1, x2, y2 = face
     width = x2 - x1
     height = 20
     bar = np.ones((height, width, 3), dtype=np.uint8) * (255, 0, 0)
     report_image = image.copy()
     report_image[y2:y2 + height, x1:x2] = bar
     txt = f'Face {idx + 1}'
```

### Comparing `skin-tone-classifier-0.2.1/src/stone/utils.py` & `skin-tone-classifier-0.2.2/src/stone/utils.py`

 * *Files identical despite different names*

