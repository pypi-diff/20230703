# Comparing `tmp/chef_recipes-1.0.1.tar.gz` & `tmp/chef_recipes-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chef_recipes-1.0.1.tar", max compression
+gzip compressed data, was "chef_recipes-1.0.2.tar", max compression
```

## Comparing `chef_recipes-1.0.1.tar` & `chef_recipes-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      771 2023-06-21 14:51:29.141089 chef_recipes-1.0.1/pyproject.toml
--rw-r--r--   0        0        0   105536 2023-06-21 13:00:13.873177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-brands-400-404c746c.woff2
--rw-r--r--   0        0        0   181852 2023-06-21 13:00:13.873177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-brands-400-e523f49c.ttf
--rw-r--r--   0        0        0    60520 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-regular-400-4e96a7e0.ttf
--rw-r--r--   0        0        0    23940 2023-06-21 13:00:13.873177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-regular-400-6a274e76.woff2
--rw-r--r--   0        0        0   388460 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-solid-900-03f2986c.ttf
--rw-r--r--   0        0        0   154228 2023-06-21 13:00:13.873177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-solid-900-d76fb4e8.woff2
--rw-r--r--   0        0        0     4960 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-v4compatibility-0db31bef.woff2
--rw-r--r--   0        0        0    10556 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-v4compatibility-86a687cf.ttf
--rw-r--r--   0        0        0     9197 2023-06-21 13:00:13.869177 chef_recipes-1.0.1/src/js/chef/dist/assets/favicon-464b3816.png
--rw-r--r--   0        0        0   314577 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/index-70f2750d.css
--rw-r--r--   0        0        0   484824 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/index-b3f57f4a.js
--rw-r--r--   0        0        0   119596 2023-06-21 13:00:13.463184 chef_recipes-1.0.1/src/js/chef/dist/favicon.ico
--rw-r--r--   0        0        0      419 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/index.html
--rw-r--r--   0        0        0        1 2023-06-21 14:51:25.825143 chef_recipes-1.0.1/src/python/chef/__init__.py
--rw-r--r--   0        0        0      645 2023-06-19 15:18:02.823243 chef_recipes-1.0.1/src/python/chef/api/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-19 17:16:18.642244 chef_recipes-1.0.1/src/python/chef/api/categories.py
--rw-r--r--   0        0        0     1172 2023-06-19 14:03:07.526945 chef_recipes-1.0.1/src/python/chef/api/common.py
--rw-r--r--   0        0        0     1777 2023-06-21 06:08:54.409100 chef_recipes-1.0.1/src/python/chef/api/images.py
--rw-r--r--   0        0        0      856 2023-06-20 07:51:43.135386 chef_recipes-1.0.1/src/python/chef/api/ingredients.py
--rw-r--r--   0        0        0     1358 2023-06-20 07:51:32.853550 chef_recipes-1.0.1/src/python/chef/api/recipes.py
--rw-r--r--   0        0        0      733 2023-06-19 17:16:18.671243 chef_recipes-1.0.1/src/python/chef/api/tags.py
--rw-r--r--   0        0        0     8049 2023-06-21 08:37:20.902732 chef_recipes-1.0.1/src/python/chef/controllers.py
--rw-r--r--   0        0        0     1907 2023-06-21 09:07:09.838201 chef_recipes-1.0.1/src/python/chef/images.py
--rw-r--r--   0        0        0     2143 2023-06-21 12:43:53.141300 chef_recipes-1.0.1/src/python/chef/main.py
--rw-r--r--   0        0        0     5868 2023-06-20 13:41:42.301568 chef_recipes-1.0.1/src/python/chef/models.py
--rw-r--r--   0        0        0     3114 2023-06-19 14:05:22.906763 chef_recipes-1.0.1/src/python/chef/schemas.py
--rw-r--r--   0        0        0      634 2023-06-20 08:50:33.632068 chef_recipes-1.0.1/src/python/chef/session.py
--rw-r--r--   0        0        0     1234 2023-06-21 12:43:05.219090 chef_recipes-1.0.1/src/python/chef/settings.py
--rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 chef_recipes-1.0.1/setup.py
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 chef_recipes-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      771 2023-07-03 14:44:01.432958 chef_recipes-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0   105536 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/fa-brands-400-404c746c.woff2
+-rw-r--r--   0        0        0   181852 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/fa-brands-400-e523f49c.ttf
+-rw-r--r--   0        0        0    60520 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/fa-regular-400-4e96a7e0.ttf
+-rw-r--r--   0        0        0    23940 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/fa-regular-400-6a274e76.woff2
+-rw-r--r--   0        0        0   388460 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/fa-solid-900-03f2986c.ttf
+-rw-r--r--   0        0        0   154228 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/fa-solid-900-d76fb4e8.woff2
+-rw-r--r--   0        0        0     4960 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/fa-v4compatibility-0db31bef.woff2
+-rw-r--r--   0        0        0    10556 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/fa-v4compatibility-86a687cf.ttf
+-rw-r--r--   0        0        0     9197 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/favicon-464b3816.png
+-rw-r--r--   0        0        0   484310 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/index-0a53cac4.js
+-rw-r--r--   0        0        0   315023 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/assets/index-7e912a5f.css
+-rw-r--r--   0        0        0   119596 2023-07-03 14:43:42.741504 chef_recipes-1.0.2/src/js/chef/dist/favicon.ico
+-rw-r--r--   0        0        0      419 2023-07-03 14:43:43.014666 chef_recipes-1.0.2/src/js/chef/dist/index.html
+-rw-r--r--   0        0        0        1 2023-06-30 12:06:29.500465 chef_recipes-1.0.2/src/python/chef/__init__.py
+-rw-r--r--   0        0        0      645 2023-06-19 15:18:02.823243 chef_recipes-1.0.2/src/python/chef/api/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-19 17:16:18.642244 chef_recipes-1.0.2/src/python/chef/api/categories.py
+-rw-r--r--   0        0        0     1172 2023-06-19 14:03:07.526945 chef_recipes-1.0.2/src/python/chef/api/common.py
+-rw-r--r--   0        0        0     1777 2023-06-21 06:08:54.409100 chef_recipes-1.0.2/src/python/chef/api/images.py
+-rw-r--r--   0        0        0      856 2023-06-20 07:51:43.135386 chef_recipes-1.0.2/src/python/chef/api/ingredients.py
+-rw-r--r--   0        0        0     1525 2023-07-03 14:26:04.776719 chef_recipes-1.0.2/src/python/chef/api/recipes.py
+-rw-r--r--   0        0        0      733 2023-06-19 17:16:18.671243 chef_recipes-1.0.2/src/python/chef/api/tags.py
+-rw-r--r--   0        0        0     8351 2023-07-03 14:42:26.862892 chef_recipes-1.0.2/src/python/chef/controllers.py
+-rw-r--r--   0        0        0     1907 2023-06-21 09:07:09.838201 chef_recipes-1.0.2/src/python/chef/images.py
+-rw-r--r--   0        0        0     2143 2023-06-21 12:43:53.141300 chef_recipes-1.0.2/src/python/chef/main.py
+-rw-r--r--   0        0        0     5997 2023-07-03 08:15:18.682450 chef_recipes-1.0.2/src/python/chef/models.py
+-rw-r--r--   0        0        0     3141 2023-07-03 09:29:57.570429 chef_recipes-1.0.2/src/python/chef/schemas.py
+-rw-r--r--   0        0        0      634 2023-06-20 08:50:33.632068 chef_recipes-1.0.2/src/python/chef/session.py
+-rw-r--r--   0        0        0     1234 2023-06-21 12:43:05.219090 chef_recipes-1.0.2/src/python/chef/settings.py
+-rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 chef_recipes-1.0.2/setup.py
+-rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 chef_recipes-1.0.2/PKG-INFO
```

### Comparing `chef_recipes-1.0.1/pyproject.toml` & `chef_recipes-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chef-recipes"
-version = "1.0.1"
+version = "1.0.2"
 description = "Home recipe management app."
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 
 packages = [
     { include = "chef", from = "src/python" }
 ]
```

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/fa-brands-400-404c746c.woff2` & `chef_recipes-1.0.2/src/js/chef/dist/assets/fa-brands-400-404c746c.woff2`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/fa-brands-400-e523f49c.ttf` & `chef_recipes-1.0.2/src/js/chef/dist/assets/fa-brands-400-e523f49c.ttf`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/fa-regular-400-4e96a7e0.ttf` & `chef_recipes-1.0.2/src/js/chef/dist/assets/fa-regular-400-4e96a7e0.ttf`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/fa-regular-400-6a274e76.woff2` & `chef_recipes-1.0.2/src/js/chef/dist/assets/fa-regular-400-6a274e76.woff2`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/fa-solid-900-03f2986c.ttf` & `chef_recipes-1.0.2/src/js/chef/dist/assets/fa-solid-900-03f2986c.ttf`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/fa-solid-900-d76fb4e8.woff2` & `chef_recipes-1.0.2/src/js/chef/dist/assets/fa-solid-900-d76fb4e8.woff2`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/fa-v4compatibility-0db31bef.woff2` & `chef_recipes-1.0.2/src/js/chef/dist/assets/fa-v4compatibility-0db31bef.woff2`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/fa-v4compatibility-86a687cf.ttf` & `chef_recipes-1.0.2/src/js/chef/dist/assets/fa-v4compatibility-86a687cf.ttf`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/favicon-464b3816.png` & `chef_recipes-1.0.2/src/js/chef/dist/assets/favicon-464b3816.png`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/index-70f2750d.css` & `chef_recipes-1.0.2/src/js/chef/dist/assets/index-7e912a5f.css`

 * *Files 1% similar despite different names*

```diff
@@ -19590,30 +19590,30 @@
 0004c850: 6e73 666f 726d 3a75 7070 6572 6361 7365  nsform:uppercase
 0004c860: 7d2e 7265 6369 7065 2d6c 6973 745b 6461  }.recipe-list[da
 0004c870: 7461 2d76 2d36 3736 3032 6161 395d 7b64  ta-v-67602aa9]{d
 0004c880: 6973 706c 6179 3a66 6c65 783b 666c 6578  isplay:flex;flex
 0004c890: 2d64 6972 6563 7469 6f6e 3a63 6f6c 756d  -direction:colum
 0004c8a0: 6e3b 6761 703a 2e33 656d 7d2e 6361 7465  n;gap:.3em}.cate
 0004c8b0: 676f 7279 2d74 696c 6573 5b64 6174 612d  gory-tiles[data-
-0004c8c0: 762d 3063 6136 6463 3263 5d7b 6469 7370  v-0ca6dc2c]{disp
+0004c8c0: 762d 3131 6464 3136 6464 5d7b 6469 7370  v-11dd16dd]{disp
 0004c8d0: 6c61 793a 6772 6964 3b67 7269 642d 7465  lay:grid;grid-te
 0004c8e0: 6d70 6c61 7465 2d63 6f6c 756d 6e73 3a31  mplate-columns:1
 0004c8f0: 6672 2031 6672 2031 6672 3b67 6170 3a2e  fr 1fr 1fr;gap:.
 0004c900: 3365 6d7d 406d 6564 6961 206f 6e6c 7920  3em}@media only 
 0004c910: 7363 7265 656e 2061 6e64 2028 6d61 782d  screen and (max-
 0004c920: 7769 6474 683a 2039 3030 7078 297b 2e63  width: 900px){.c
 0004c930: 6174 6567 6f72 792d 7469 6c65 735b 6461  ategory-tiles[da
-0004c940: 7461 2d76 2d30 6361 3664 6332 635d 7b67  ta-v-0ca6dc2c]{g
+0004c940: 7461 2d76 2d31 3164 6431 3664 645d 7b67  ta-v-11dd16dd]{g
 0004c950: 7269 642d 7465 6d70 6c61 7465 2d63 6f6c  rid-template-col
 0004c960: 756d 6e73 3a31 6672 2031 6672 7d7d 406d  umns:1fr 1fr}}@m
 0004c970: 6564 6961 206f 6e6c 7920 7363 7265 656e  edia only screen
 0004c980: 2061 6e64 2028 6d61 782d 7769 6474 683a   and (max-width:
 0004c990: 2036 3030 7078 297b 2e63 6174 6567 6f72   600px){.categor
-0004c9a0: 792d 7469 6c65 735b 6461 7461 2d76 2d30  y-tiles[data-v-0
-0004c9b0: 6361 3664 6332 635d 7b67 7269 642d 7465  ca6dc2c]{grid-te
+0004c9a0: 792d 7469 6c65 735b 6461 7461 2d76 2d31  y-tiles[data-v-1
+0004c9b0: 3164 6431 3664 645d 7b67 7269 642d 7465  1dd16dd]{grid-te
 0004c9c0: 6d70 6c61 7465 2d63 6f6c 756d 6e73 3a31  mplate-columns:1
 0004c9d0: 6672 7d7d 2e50 726f 7365 4d69 7272 6f72  fr}}.ProseMirror
 0004c9e0: 7b70 6164 6469 6e67 2d74 6f70 3a2e 3565  {padding-top:.5e
 0004c9f0: 6d3b 7061 6464 696e 672d 6c65 6674 3a2e  m;padding-left:.
 0004ca00: 3565 6d3b 7061 6464 696e 672d 7269 6768  5em;padding-righ
 0004ca10: 743a 2e35 656d 3b6d 696e 2d68 6569 6768  t:.5em;min-heigh
 0004ca20: 743a 3130 656d 3b6f 7574 6c69 6e65 2d63  t:10em;outline-c
@@ -19640,23 +19640,50 @@
 0004cb70: 726f 756e 642d 636f 6c6f 723a 2361 3961  round-color:#a9a
 0004cb80: 3961 393b 626f 7264 6572 2d72 6164 6975  9a9;border-radiu
 0004cb90: 733a 3170 787d 2e65 6469 746f 722d 7772  s:1px}.editor-wr
 0004cba0: 6170 7065 7220 6275 7474 6f6e 3a68 6f76  apper button:hov
 0004cbb0: 6572 7b62 6163 6b67 726f 756e 642d 636f  er{background-co
 0004cbc0: 6c6f 723a 2364 3364 3364 337d 2e66 756c  lor:#d3d3d3}.ful
 0004cbd0: 6c77 6964 7468 7b77 6964 7468 3a31 3030  lwidth{width:100
-0004cbe0: 257d 2e61 6e69 6d61 7465 2d69 636f 6e5b  %}.animate-icon[
-0004cbf0: 6461 7461 2d76 2d63 3834 3535 6363 375d  data-v-c8455cc7]
-0004cc00: 7b74 7261 6e73 6974 696f 6e3a 2e31 3573  {transition:.15s
-0004cc10: 7d2e 726f 7461 7465 5b64 6174 612d 762d  }.rotate[data-v-
-0004cc20: 6338 3435 3563 6337 5d7b 7472 616e 7366  c8455cc7]{transf
-0004cc30: 6f72 6d3a 726f 7461 7465 282d 3930 6465  orm:rotate(-90de
-0004cc40: 6729 7d2e 7469 746c 652d 6865 6164 6572  g)}.title-header
-0004cc50: 2068 315b 6461 7461 2d76 2d63 3834 3535   h1[data-v-c8455
-0004cc60: 6363 375d 2c2e 7469 746c 652d 6865 6164  cc7],.title-head
-0004cc70: 6572 2068 325b 6461 7461 2d76 2d63 3834  er h2[data-v-c84
-0004cc80: 3535 6363 375d 7b74 6578 742d 7472 616e  55cc7]{text-tran
-0004cc90: 7366 6f72 6d3a 7570 7065 7263 6173 657d  sform:uppercase}
-0004cca0: 2e72 6563 6970 652d 6c69 7374 5b64 6174  .recipe-list[dat
-0004ccb0: 612d 762d 3562 6332 6339 3066 5d7b 6d69  a-v-5bc2c90f]{mi
-0004ccc0: 6e2d 6865 6967 6874 3a31 3830 3070 787d  n-height:1800px}
-0004ccd0: 0a                                       .
+0004cbe0: 257d 406b 6579 6672 616d 6573 206c 6f61  %}@keyframes loa
+0004cbf0: 6469 6e67 2d34 6132 3462 3465 387b 3025  ding-4a24b4e8{0%
+0004cc00: 7b74 7261 6e73 666f 726d 3a72 6f74 6174  {transform:rotat
+0004cc10: 6528 2d31 3564 6567 297d 746f 7b74 7261  e(-15deg)}to{tra
+0004cc20: 6e73 666f 726d 3a72 6f74 6174 6528 3135  nsform:rotate(15
+0004cc30: 6465 6729 7d7d 2e73 7461 725b 6461 7461  deg)}}.star[data
+0004cc40: 2d76 2d34 6132 3462 3465 385d 7b66 6f6e  -v-4a24b4e8]{fon
+0004cc50: 742d 7369 7a65 3a78 2d6c 6172 6765 3b63  t-size:x-large;c
+0004cc60: 6f6c 6f72 3a23 6461 6135 3230 7d2e 7374  olor:#daa520}.st
+0004cc70: 6172 5b64 6174 612d 762d 3461 3234 6234  ar[data-v-4a24b4
+0004cc80: 6538 5d3a 686f 7665 727b 636f 6c6f 723a  e8]:hover{color:
+0004cc90: 676f 6c64 3b63 7572 736f 723a 706f 696e  gold;cursor:poin
+0004cca0: 7465 727d 2e73 7461 722e 6c6f 6164 696e  ter}.star.loadin
+0004ccb0: 675b 6461 7461 2d76 2d34 6132 3462 3465  g[data-v-4a24b4e
+0004ccc0: 385d 7b61 6e69 6d61 7469 6f6e 2d6e 616d  8]{animation-nam
+0004ccd0: 653a 6c6f 6164 696e 672d 3461 3234 6234  e:loading-4a24b4
+0004cce0: 6538 3b61 6e69 6d61 7469 6f6e 2d64 7572  e8;animation-dur
+0004ccf0: 6174 696f 6e3a 2e32 733b 616e 696d 6174  ation:.2s;animat
+0004cd00: 696f 6e2d 6469 7265 6374 696f 6e3a 616c  ion-direction:al
+0004cd10: 7465 726e 6174 652d 7265 7665 7273 653b  ternate-reverse;
+0004cd20: 616e 696d 6174 696f 6e2d 7469 6d69 6e67  animation-timing
+0004cd30: 2d66 756e 6374 696f 6e3a 6561 7365 2d69  -function:ease-i
+0004cd40: 6e2d 6f75 743b 616e 696d 6174 696f 6e2d  n-out;animation-
+0004cd50: 6974 6572 6174 696f 6e2d 636f 756e 743a  iteration-count:
+0004cd60: 696e 6669 6e69 7465 7d2e 616e 696d 6174  infinite}.animat
+0004cd70: 652d 6963 6f6e 5b64 6174 612d 762d 3233  e-icon[data-v-23
+0004cd80: 6336 3862 3638 5d7b 7472 616e 7369 7469  c68b68]{transiti
+0004cd90: 6f6e 3a2e 3135 737d 2e72 6f74 6174 655b  on:.15s}.rotate[
+0004cda0: 6461 7461 2d76 2d32 3363 3638 6236 385d  data-v-23c68b68]
+0004cdb0: 7b74 7261 6e73 666f 726d 3a72 6f74 6174  {transform:rotat
+0004cdc0: 6528 2d39 3064 6567 297d 2e74 6974 6c65  e(-90deg)}.title
+0004cdd0: 2d68 6561 6465 7220 6831 5b64 6174 612d  -header h1[data-
+0004cde0: 762d 3233 6336 3862 3638 5d2c 2e74 6974  v-23c68b68],.tit
+0004cdf0: 6c65 2d68 6561 6465 7220 6832 5b64 6174  le-header h2[dat
+0004ce00: 612d 762d 3233 6336 3862 3638 5d7b 7465  a-v-23c68b68]{te
+0004ce10: 7874 2d74 7261 6e73 666f 726d 3a75 7070  xt-transform:upp
+0004ce20: 6572 6361 7365 7d2e 7461 675b 6461 7461  ercase}.tag[data
+0004ce30: 2d76 2d32 3363 3638 6236 385d 7b6d 6172  -v-23c68b68]{mar
+0004ce40: 6769 6e2d 626f 7474 6f6d 3a30 253b 7061  gin-bottom:0%;pa
+0004ce50: 6464 696e 672d 746f 703a 3170 787d 2e72  dding-top:1px}.r
+0004ce60: 6563 6970 652d 6c69 7374 5b64 6174 612d  ecipe-list[data-
+0004ce70: 762d 3562 6332 6339 3066 5d7b 6d69 6e2d  v-5bc2c90f]{min-
+0004ce80: 6865 6967 6874 3a31 3830 3070 787d 0a    height:1800px}.
```

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/assets/index-b3f57f4a.js` & `chef_recipes-1.0.2/src/js/chef/dist/assets/index-0a53cac4.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -27,161 +27,161 @@
 function Ya(t, e) {
     const n = Object.create(null),
         r = t.split(",");
     for (let s = 0; s < r.length; s++) n[r[s]] = !0;
     return e ? s => !!n[s.toLowerCase()] : s => !!n[s]
 }
 
-function _o(t) {
+function Eo(t) {
     if (te(t)) {
         const e = {};
         for (let n = 0; n < t.length; n++) {
             const r = t[n],
-                s = je(r) ? vg(r) : _o(r);
+                s = Ue(r) ? xg(r) : Eo(r);
             if (s)
                 for (const i in s) e[i] = s[i]
         }
         return e
     } else {
-        if (je(t)) return t;
+        if (Ue(t)) return t;
         if (Ie(t)) return t
     }
 }
-const gg = /;(?![^(]*\))/g,
-    yg = /:([^]+)/,
-    bg = /\/\*.*?\*\//gs;
+const yg = /;(?![^(]*\))/g,
+    bg = /:([^]+)/,
+    vg = /\/\*.*?\*\//gs;
 
-function vg(t) {
+function xg(t) {
     const e = {};
-    return t.replace(bg, "").split(gg).forEach(n => {
+    return t.replace(vg, "").split(yg).forEach(n => {
         if (n) {
-            const r = n.split(yg);
+            const r = n.split(bg);
             r.length > 1 && (e[r[0].trim()] = r[1].trim())
         }
     }), e
 }
 
-function he(t) {
+function fe(t) {
     let e = "";
-    if (je(t)) e = t;
+    if (Ue(t)) e = t;
     else if (te(t))
         for (let n = 0; n < t.length; n++) {
-            const r = he(t[n]);
+            const r = fe(t[n]);
             r && (e += r + " ")
         } else if (Ie(t))
             for (const n in t) t[n] && (e += n + " ");
     return e.trim()
 }
-const xg = "itemscope,allowfullscreen,formnovalidate,ismap,nomodule,novalidate,readonly",
-    kg = Ya(xg);
+const kg = "itemscope,allowfullscreen,formnovalidate,ismap,nomodule,novalidate,readonly",
+    wg = Ya(kg);
 
 function Hf(t) {
     return !!t || t === ""
 }
 
-function wg(t, e) {
+function Sg(t, e) {
     if (t.length !== e.length) return !1;
     let n = !0;
-    for (let r = 0; n && r < t.length; r++) n = Co(t[r], e[r]);
+    for (let r = 0; n && r < t.length; r++) n = To(t[r], e[r]);
     return n
 }
 
-function Co(t, e) {
+function To(t, e) {
     if (t === e) return !0;
     let n = tu(t),
         r = tu(e);
     if (n || r) return n && r ? t.getTime() === e.getTime() : !1;
     if (n = ri(t), r = ri(e), n || r) return t === e;
-    if (n = te(t), r = te(e), n || r) return n && r ? wg(t, e) : !1;
+    if (n = te(t), r = te(e), n || r) return n && r ? Sg(t, e) : !1;
     if (n = Ie(t), r = Ie(e), n || r) {
         if (!n || !r) return !1;
         const s = Object.keys(t).length,
             i = Object.keys(e).length;
         if (s !== i) return !1;
         for (const o in t) {
             const l = t.hasOwnProperty(o),
                 a = e.hasOwnProperty(o);
-            if (l && !a || !l && a || !Co(t[o], e[o])) return !1
+            if (l && !a || !l && a || !To(t[o], e[o])) return !1
         }
     }
     return String(t) === String(e)
 }
 
 function zf(t, e) {
-    return t.findIndex(n => Co(n, e))
+    return t.findIndex(n => To(n, e))
 }
-const le = t => je(t) ? t : t == null ? "" : te(t) || Ie(t) && (t.toString === Uf || !me(t.toString)) ? JSON.stringify(t, Vf, 2) : String(t),
+const le = t => Ue(t) ? t : t == null ? "" : te(t) || Ie(t) && (t.toString === Uf || !me(t.toString)) ? JSON.stringify(t, Vf, 2) : String(t),
     Vf = (t, e) => e && e.__v_isRef ? Vf(t, e.value) : Yr(e) ? {
         [`Map(${e.size})`]: [...e.entries()].reduce((n, [r, s]) => (n[`${r} =>`] = s, n), {})
-    } : To(e) ? {
+    } : Mo(e) ? {
         [`Set(${e.size})`]: [...e.values()]
     } : Ie(e) && !te(e) && !Wf(e) ? String(e) : e,
     $e = {},
     Gr = [],
     en = () => {},
-    Sg = () => !1,
-    _g = /^on[^a-z]/,
-    Eo = t => _g.test(t),
+    _g = () => !1,
+    Cg = /^on[^a-z]/,
+    Oo = t => Cg.test(t),
     Xa = t => t.startsWith("onUpdate:"),
     lt = Object.assign,
     Qa = (t, e) => {
         const n = t.indexOf(e);
         n > -1 && t.splice(n, 1)
     },
-    Cg = Object.prototype.hasOwnProperty,
-    _e = (t, e) => Cg.call(t, e),
+    Eg = Object.prototype.hasOwnProperty,
+    _e = (t, e) => Eg.call(t, e),
     te = Array.isArray,
     Yr = t => ws(t) === "[object Map]",
-    To = t => ws(t) === "[object Set]",
+    Mo = t => ws(t) === "[object Set]",
     tu = t => ws(t) === "[object Date]",
-    Eg = t => ws(t) === "[object RegExp]",
+    Tg = t => ws(t) === "[object RegExp]",
     me = t => typeof t == "function",
-    je = t => typeof t == "string",
+    Ue = t => typeof t == "string",
     ri = t => typeof t == "symbol",
     Ie = t => t !== null && typeof t == "object",
     jf = t => Ie(t) && me(t.then) && me(t.catch),
     Uf = Object.prototype.toString,
     ws = t => Uf.call(t),
-    Tg = t => ws(t).slice(8, -1),
+    Og = t => ws(t).slice(8, -1),
     Wf = t => ws(t) === "[object Object]",
-    Za = t => je(t) && t !== "NaN" && t[0] !== "-" && "" + parseInt(t, 10) === t,
-    zi = Ya(",key,ref,ref_for,ref_key,onVnodeBeforeMount,onVnodeMounted,onVnodeBeforeUpdate,onVnodeUpdated,onVnodeBeforeUnmount,onVnodeUnmounted"),
-    Oo = t => {
+    Za = t => Ue(t) && t !== "NaN" && t[0] !== "-" && "" + parseInt(t, 10) === t,
+    ji = Ya(",key,ref,ref_for,ref_key,onVnodeBeforeMount,onVnodeMounted,onVnodeBeforeUpdate,onVnodeUpdated,onVnodeBeforeUnmount,onVnodeUnmounted"),
+    Ao = t => {
         const e = Object.create(null);
         return n => e[n] || (e[n] = t(n))
     },
-    Og = /-(\w)/g,
-    yn = Oo(t => t.replace(Og, (e, n) => n ? n.toUpperCase() : "")),
-    Mg = /\B([A-Z])/g,
-    Ss = Oo(t => t.replace(Mg, "-$1").toLowerCase()),
-    Mo = Oo(t => t.charAt(0).toUpperCase() + t.slice(1)),
-    pl = Oo(t => t ? `on${Mo(t)}` : ""),
+    Mg = /-(\w)/g,
+    yn = Ao(t => t.replace(Mg, (e, n) => n ? n.toUpperCase() : "")),
+    Ag = /\B([A-Z])/g,
+    Ss = Ao(t => t.replace(Ag, "-$1").toLowerCase()),
+    No = Ao(t => t.charAt(0).toUpperCase() + t.slice(1)),
+    pl = Ao(t => t ? `on${No(t)}` : ""),
     si = (t, e) => !Object.is(t, e),
     Xr = (t, e) => {
         for (let n = 0; n < t.length; n++) t[n](e)
     },
-    Qi = (t, e, n) => {
+    eo = (t, e, n) => {
         Object.defineProperty(t, e, {
             configurable: !0,
             enumerable: !1,
             value: n
         })
     },
     ia = t => {
         const e = parseFloat(t);
         return isNaN(e) ? t : e
     },
-    Ag = t => {
-        const e = je(t) ? Number(t) : NaN;
+    Ng = t => {
+        const e = Ue(t) ? Number(t) : NaN;
         return isNaN(e) ? t : e
     };
 let nu;
-const Ng = () => nu || (nu = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {});
+const Rg = () => nu || (nu = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {});
 let Jt;
-class Rg {
+class Dg {
     constructor(e = !1) {
         this.detached = e, this._active = !0, this.effects = [], this.cleanups = [], this.parent = Jt, !e && Jt && (this.index = (Jt.scopes || (Jt.scopes = [])).push(this) - 1)
     }
     get active() {
         return this._active
     }
     run(e) {
@@ -212,34 +212,34 @@
                 s && s !== this && (this.parent.scopes[this.index] = s, s.index = this.index)
             }
             this.parent = void 0, this._active = !1
         }
     }
 }
 
-function Dg(t, e = Jt) {
+function Ig(t, e = Jt) {
     e && e.active && e.effects.push(t)
 }
 
-function Ig() {
+function Pg() {
     return Jt
 }
 const ec = t => {
         const e = new Set(t);
         return e.w = 0, e.n = 0, e
     },
     qf = t => (t.w & rr) > 0,
     Kf = t => (t.n & rr) > 0,
-    Pg = ({
+    $g = ({
         deps: t
     }) => {
         if (t.length)
             for (let e = 0; e < t.length; e++) t[e].w |= rr
     },
-    $g = t => {
+    Lg = t => {
         const {
             deps: e
         } = t;
         if (e.length) {
             let n = 0;
             for (let r = 0; r < e.length; r++) {
                 const s = e[r];
@@ -253,28 +253,28 @@
     rr = 1;
 const la = 30;
 let Yt;
 const Tr = Symbol(""),
     aa = Symbol("");
 class tc {
     constructor(e, n = null, r) {
-        this.fn = e, this.scheduler = n, this.active = !0, this.deps = [], this.parent = void 0, Dg(this, r)
+        this.fn = e, this.scheduler = n, this.active = !0, this.deps = [], this.parent = void 0, Ig(this, r)
     }
     run() {
         if (!this.active) return this.fn();
         let e = Yt,
             n = Xn;
         for (; e;) {
             if (e === this) return;
             e = e.parent
         }
         try {
-            return this.parent = Yt, Yt = this, Xn = !0, rr = 1 << ++Fs, Fs <= la ? Pg(this) : ru(this), this.fn()
+            return this.parent = Yt, Yt = this, Xn = !0, rr = 1 << ++Fs, Fs <= la ? $g(this) : ru(this), this.fn()
         } finally {
-            Fs <= la && $g(this), rr = 1 << --Fs, Yt = this.parent, Xn = n, this.parent = void 0, this.deferStop && this.stop()
+            Fs <= la && Lg(this), rr = 1 << --Fs, Yt = this.parent, Xn = n, this.parent = void 0, this.deferStop && this.stop()
         }
     }
     stop() {
         Yt === this ? this.deferStop = !0 : this.active && (ru(this), this.onStop && this.onStop(), this.active = !1)
     }
 }
 
@@ -347,22 +347,22 @@
     for (const r of n) r.computed && su(r);
     for (const r of n) r.computed || su(r)
 }
 
 function su(t, e) {
     (t !== Yt || t.allowRecurse) && (t.scheduler ? t.scheduler() : t.run())
 }
-const Lg = Ya("__proto__,__v_isRef,__isVue"),
+const Fg = Ya("__proto__,__v_isRef,__isVue"),
     Yf = new Set(Object.getOwnPropertyNames(Symbol).filter(t => t !== "arguments" && t !== "caller").map(t => Symbol[t]).filter(ri)),
-    Fg = nc(),
-    Bg = nc(!1, !0),
-    Hg = nc(!0),
-    iu = zg();
+    Bg = nc(),
+    Hg = nc(!1, !0),
+    zg = nc(!0),
+    iu = Vg();
 
-function zg() {
+function Vg() {
     const t = {};
     return ["includes", "indexOf", "lastIndexOf"].forEach(e => {
         t[e] = function(...n) {
             const r = Me(this);
             for (let i = 0, o = this.length; i < o; i++) Tt(r, "get", i + "");
             const s = r[e](...n);
             return s === -1 || s === !1 ? r[e](...n.map(Me)) : s
@@ -372,159 +372,159 @@
             _s();
             const r = Me(this)[e].apply(this, n);
             return Cs(), r
         }
     }), t
 }
 
-function Vg(t) {
+function jg(t) {
     const e = Me(this);
     return Tt(e, "has", t), e.hasOwnProperty(t)
 }
 
 function nc(t = !1, e = !1) {
     return function(r, s, i) {
         if (s === "__v_isReactive") return !t;
         if (s === "__v_isReadonly") return t;
         if (s === "__v_isShallow") return e;
-        if (s === "__v_raw" && i === (t ? e ? sy : th : e ? eh : Zf).get(r)) return r;
+        if (s === "__v_raw" && i === (t ? e ? iy : th : e ? eh : Zf).get(r)) return r;
         const o = te(r);
         if (!t) {
             if (o && _e(iu, s)) return Reflect.get(iu, s, i);
-            if (s === "hasOwnProperty") return Vg
+            if (s === "hasOwnProperty") return jg
         }
         const l = Reflect.get(r, s, i);
-        return (ri(s) ? Yf.has(s) : Lg(s)) || (t || Tt(r, "get", s), e) ? l : ft(l) ? o && Za(s) ? l : l.value : Ie(l) ? t ? nh(l) : Es(l) : l
+        return (ri(s) ? Yf.has(s) : Fg(s)) || (t || Tt(r, "get", s), e) ? l : ft(l) ? o && Za(s) ? l : l.value : Ie(l) ? t ? nh(l) : Es(l) : l
     }
 }
-const jg = Xf(),
-    Ug = Xf(!0);
+const Ug = Xf(),
+    Wg = Xf(!0);
 
 function Xf(t = !1) {
     return function(n, r, s, i) {
         let o = n[r];
         if (ss(o) && ft(o) && !ft(s)) return !1;
-        if (!t && (!Zi(s) && !ss(s) && (o = Me(o), s = Me(s)), !te(n) && ft(o) && !ft(s))) return o.value = s, !0;
+        if (!t && (!to(s) && !ss(s) && (o = Me(o), s = Me(s)), !te(n) && ft(o) && !ft(s))) return o.value = s, !0;
         const l = te(n) && Za(r) ? Number(r) < n.length : _e(n, r),
             a = Reflect.set(n, r, s, i);
         return n === Me(i) && (l ? si(s, o) && Nn(n, "set", r, s) : Nn(n, "add", r, s)), a
     }
 }
 
-function Wg(t, e) {
+function qg(t, e) {
     const n = _e(t, e);
     t[e];
     const r = Reflect.deleteProperty(t, e);
     return r && n && Nn(t, "delete", e, void 0), r
 }
 
-function qg(t, e) {
+function Kg(t, e) {
     const n = Reflect.has(t, e);
     return (!ri(e) || !Yf.has(e)) && Tt(t, "has", e), n
 }
 
-function Kg(t) {
+function Jg(t) {
     return Tt(t, "iterate", te(t) ? "length" : Tr), Reflect.ownKeys(t)
 }
 const Qf = {
-        get: Fg,
-        set: jg,
-        deleteProperty: Wg,
-        has: qg,
-        ownKeys: Kg
+        get: Bg,
+        set: Ug,
+        deleteProperty: qg,
+        has: Kg,
+        ownKeys: Jg
     },
-    Jg = {
-        get: Hg,
+    Gg = {
+        get: zg,
         set(t, e) {
             return !0
         },
         deleteProperty(t, e) {
             return !0
         }
     },
-    Gg = lt({}, Qf, {
-        get: Bg,
-        set: Ug
+    Yg = lt({}, Qf, {
+        get: Hg,
+        set: Wg
     }),
     rc = t => t,
-    Ao = t => Reflect.getPrototypeOf(t);
+    Ro = t => Reflect.getPrototypeOf(t);
 
-function Oi(t, e, n = !1, r = !1) {
+function Ai(t, e, n = !1, r = !1) {
     t = t.__v_raw;
     const s = Me(t),
         i = Me(e);
     n || (e !== i && Tt(s, "get", e), Tt(s, "get", i));
     const {
         has: o
-    } = Ao(s), l = r ? rc : n ? lc : ii;
+    } = Ro(s), l = r ? rc : n ? lc : ii;
     if (o.call(s, e)) return l(t.get(e));
     if (o.call(s, i)) return l(t.get(i));
     t !== s && t.get(e)
 }
 
-function Mi(t, e = !1) {
+function Ni(t, e = !1) {
     const n = this.__v_raw,
         r = Me(n),
         s = Me(t);
     return e || (t !== s && Tt(r, "has", t), Tt(r, "has", s)), t === s ? n.has(t) : n.has(t) || n.has(s)
 }
 
-function Ai(t, e = !1) {
+function Ri(t, e = !1) {
     return t = t.__v_raw, !e && Tt(Me(t), "iterate", Tr), Reflect.get(t, "size", t)
 }
 
 function ou(t) {
     t = Me(t);
     const e = Me(this);
-    return Ao(e).has.call(e, t) || (e.add(t), Nn(e, "add", t, t)), this
+    return Ro(e).has.call(e, t) || (e.add(t), Nn(e, "add", t, t)), this
 }
 
 function lu(t, e) {
     e = Me(e);
     const n = Me(this),
         {
             has: r,
             get: s
-        } = Ao(n);
+        } = Ro(n);
     let i = r.call(n, t);
     i || (t = Me(t), i = r.call(n, t));
     const o = s.call(n, t);
     return n.set(t, e), i ? si(e, o) && Nn(n, "set", t, e) : Nn(n, "add", t, e), this
 }
 
 function au(t) {
     const e = Me(this),
         {
             has: n,
             get: r
-        } = Ao(e);
+        } = Ro(e);
     let s = n.call(e, t);
     s || (t = Me(t), s = n.call(e, t)), r && r.call(e, t);
     const i = e.delete(t);
     return s && Nn(e, "delete", t, void 0), i
 }
 
 function cu() {
     const t = Me(this),
         e = t.size !== 0,
         n = t.clear();
     return e && Nn(t, "clear", void 0, void 0), n
 }
 
-function Ni(t, e) {
+function Di(t, e) {
     return function(r, s) {
         const i = this,
             o = i.__v_raw,
             l = Me(o),
             a = e ? rc : t ? lc : ii;
         return !t && Tt(l, "iterate", Tr), o.forEach((c, u) => r.call(s, a(c), a(u), i))
     }
 }
 
-function Ri(t, e, n) {
+function Ii(t, e, n) {
     return function(...r) {
         const s = this.__v_raw,
             i = Me(s),
             o = Yr(i),
             l = t === "entries" || t === Symbol.iterator && o,
             a = t === "keys" && o,
             c = s[t](...r),
@@ -552,163 +552,163 @@
 
 function $n(t) {
     return function(...e) {
         return t === "delete" ? !1 : this
     }
 }
 
-function Yg() {
+function Xg() {
     const t = {
             get(i) {
-                return Oi(this, i)
+                return Ai(this, i)
             },
             get size() {
-                return Ai(this)
+                return Ri(this)
             },
-            has: Mi,
+            has: Ni,
             add: ou,
             set: lu,
             delete: au,
             clear: cu,
-            forEach: Ni(!1, !1)
+            forEach: Di(!1, !1)
         },
         e = {
             get(i) {
-                return Oi(this, i, !1, !0)
+                return Ai(this, i, !1, !0)
             },
             get size() {
-                return Ai(this)
+                return Ri(this)
             },
-            has: Mi,
+            has: Ni,
             add: ou,
             set: lu,
             delete: au,
             clear: cu,
-            forEach: Ni(!1, !0)
+            forEach: Di(!1, !0)
         },
         n = {
             get(i) {
-                return Oi(this, i, !0)
+                return Ai(this, i, !0)
             },
             get size() {
-                return Ai(this, !0)
+                return Ri(this, !0)
             },
             has(i) {
-                return Mi.call(this, i, !0)
+                return Ni.call(this, i, !0)
             },
             add: $n("add"),
             set: $n("set"),
             delete: $n("delete"),
             clear: $n("clear"),
-            forEach: Ni(!0, !1)
+            forEach: Di(!0, !1)
         },
         r = {
             get(i) {
-                return Oi(this, i, !0, !0)
+                return Ai(this, i, !0, !0)
             },
             get size() {
-                return Ai(this, !0)
+                return Ri(this, !0)
             },
             has(i) {
-                return Mi.call(this, i, !0)
+                return Ni.call(this, i, !0)
             },
             add: $n("add"),
             set: $n("set"),
             delete: $n("delete"),
             clear: $n("clear"),
-            forEach: Ni(!0, !0)
+            forEach: Di(!0, !0)
         };
     return ["keys", "values", "entries", Symbol.iterator].forEach(i => {
-        t[i] = Ri(i, !1, !1), n[i] = Ri(i, !0, !1), e[i] = Ri(i, !1, !0), r[i] = Ri(i, !0, !0)
+        t[i] = Ii(i, !1, !1), n[i] = Ii(i, !0, !1), e[i] = Ii(i, !1, !0), r[i] = Ii(i, !0, !0)
     }), [t, n, e, r]
 }
-const [Xg, Qg, Zg, ey] = Yg();
+const [Qg, Zg, ey, ty] = Xg();
 
 function sc(t, e) {
-    const n = e ? t ? ey : Zg : t ? Qg : Xg;
+    const n = e ? t ? ty : ey : t ? Zg : Qg;
     return (r, s, i) => s === "__v_isReactive" ? !t : s === "__v_isReadonly" ? t : s === "__v_raw" ? r : Reflect.get(_e(n, s) && s in r ? n : r, s, i)
 }
-const ty = {
+const ny = {
         get: sc(!1, !1)
     },
-    ny = {
+    ry = {
         get: sc(!1, !0)
     },
-    ry = {
+    sy = {
         get: sc(!0, !1)
     },
     Zf = new WeakMap,
     eh = new WeakMap,
     th = new WeakMap,
-    sy = new WeakMap;
+    iy = new WeakMap;
 
-function iy(t) {
+function oy(t) {
     switch (t) {
         case "Object":
         case "Array":
             return 1;
         case "Map":
         case "Set":
         case "WeakMap":
         case "WeakSet":
             return 2;
         default:
             return 0
     }
 }
 
-function oy(t) {
-    return t.__v_skip || !Object.isExtensible(t) ? 0 : iy(Tg(t))
+function ly(t) {
+    return t.__v_skip || !Object.isExtensible(t) ? 0 : oy(Og(t))
 }
 
 function Es(t) {
-    return ss(t) ? t : ic(t, !1, Qf, ty, Zf)
+    return ss(t) ? t : ic(t, !1, Qf, ny, Zf)
 }
 
-function ly(t) {
-    return ic(t, !1, Gg, ny, eh)
+function ay(t) {
+    return ic(t, !1, Yg, ry, eh)
 }
 
 function nh(t) {
-    return ic(t, !0, Jg, ry, th)
+    return ic(t, !0, Gg, sy, th)
 }
 
 function ic(t, e, n, r, s) {
     if (!Ie(t) || t.__v_raw && !(e && t.__v_isReactive)) return t;
     const i = s.get(t);
     if (i) return i;
-    const o = oy(t);
+    const o = ly(t);
     if (o === 0) return t;
     const l = new Proxy(t, o === 2 ? r : n);
     return s.set(t, l), l
 }
 
 function Qr(t) {
     return ss(t) ? Qr(t.__v_raw) : !!(t && t.__v_isReactive)
 }
 
 function ss(t) {
     return !!(t && t.__v_isReadonly)
 }
 
-function Zi(t) {
+function to(t) {
     return !!(t && t.__v_isShallow)
 }
 
 function rh(t) {
     return Qr(t) || ss(t)
 }
 
 function Me(t) {
     const e = t && t.__v_raw;
     return e ? Me(e) : t
 }
 
 function oc(t) {
-    return Qi(t, "__v_skip", !0), t
+    return eo(t, "__v_skip", !0), t
 }
 const ii = t => Ie(t) ? Es(t) : t,
     lc = t => Ie(t) ? nh(t) : t;
 
 function ac(t) {
     Xn && Yt && (t = Me(t), Gf(t.dep || (t.dep = ec())))
 }
@@ -719,53 +719,53 @@
     n && ca(n)
 }
 
 function ft(t) {
     return !!(t && t.__v_isRef === !0)
 }
 
-function No(t) {
+function Do(t) {
     return ih(t, !1)
 }
 
 function sh(t) {
     return ih(t, !0)
 }
 
 function ih(t, e) {
-    return ft(t) ? t : new ay(t, e)
+    return ft(t) ? t : new cy(t, e)
 }
-class ay {
+class cy {
     constructor(e, n) {
         this.__v_isShallow = n, this.dep = void 0, this.__v_isRef = !0, this._rawValue = n ? e : Me(e), this._value = n ? e : ii(e)
     }
     get value() {
         return ac(this), this._value
     }
     set value(e) {
-        const n = this.__v_isShallow || Zi(e) || ss(e);
+        const n = this.__v_isShallow || to(e) || ss(e);
         e = n ? e : Me(e), si(e, this._rawValue) && (this._rawValue = e, this._value = n ? e : ii(e), cc(this))
     }
 }
 
 function de(t) {
     return ft(t) ? t.value : t
 }
-const cy = {
+const uy = {
     get: (t, e, n) => de(Reflect.get(t, e, n)),
     set: (t, e, n, r) => {
         const s = t[e];
         return ft(s) && !ft(n) ? (s.value = n, !0) : Reflect.set(t, e, n, r)
     }
 };
 
 function oh(t) {
-    return Qr(t) ? t : new Proxy(t, cy)
+    return Qr(t) ? t : new Proxy(t, uy)
 }
-class uy {
+class dy {
     constructor(e) {
         this.dep = void 0, this.__v_isRef = !0;
         const {
             get: n,
             set: r
         } = e(() => ac(this), () => cc(this));
         this._get = n, this._set = r
@@ -774,19 +774,19 @@
         return this._get()
     }
     set value(e) {
         this._set(e)
     }
 }
 
-function dy(t) {
-    return new uy(t)
+function fy(t) {
+    return new dy(t)
 }
 var lh;
-class fy {
+class hy {
     constructor(e, n, r, s) {
         this._setter = n, this.dep = void 0, this.__v_isRef = !0, this[lh] = !1, this._dirty = !0, this.effect = new tc(e, () => {
             this._dirty || (this._dirty = !0, cc(this))
         }), this.effect.computed = this, this.effect.active = this._cacheable = !s, this.__v_isReadonly = r
     }
     get value() {
         const e = Me(this);
@@ -794,43 +794,43 @@
     }
     set value(e) {
         this._setter(e)
     }
 }
 lh = "__v_isReadonly";
 
-function hy(t, e, n = !1) {
+function py(t, e, n = !1) {
     let r, s;
     const i = me(t);
-    return i ? (r = t, s = en) : (r = t.get, s = t.set), new fy(r, s, i || !s, n)
+    return i ? (r = t, s = en) : (r = t.get, s = t.set), new hy(r, s, i || !s, n)
 }
 
 function Qn(t, e, n, r) {
     let s;
     try {
         s = r ? t(...r) : t()
     } catch (i) {
-        Ro(i, e, n)
+        Io(i, e, n)
     }
     return s
 }
 
 function Vt(t, e, n, r) {
     if (me(t)) {
         const i = Qn(t, e, n, r);
         return i && jf(i) && i.catch(o => {
-            Ro(o, e, n)
+            Io(o, e, n)
         }), i
     }
     const s = [];
     for (let i = 0; i < t.length; i++) s.push(Vt(t[i], e, n, r));
     return s
 }
 
-function Ro(t, e, n, r = !0) {
+function Io(t, e, n, r = !0) {
     const s = e ? e.vnode : null;
     if (e) {
         let i = e.parent;
         const o = e.proxy,
             l = n;
         for (; i;) {
             const c = i.ec;
@@ -842,18 +842,18 @@
         }
         const a = e.appContext.config.errorHandler;
         if (a) {
             Qn(a, null, 10, [t, o, l]);
             return
         }
     }
-    py(t, n, s, r)
+    my(t, n, s, r)
 }
 
-function py(t, e, n, r = !0) {
+function my(t, e, n, r = !0) {
     console.error(t)
 }
 let oi = !1,
     ua = !1;
 const ut = [];
 let un = 0;
 const Zr = [];
@@ -863,38 +863,38 @@
 let uc = null;
 
 function dc(t) {
     const e = uc || ah;
     return t ? e.then(this ? t.bind(this) : t) : e
 }
 
-function my(t) {
+function gy(t) {
     let e = un + 1,
         n = ut.length;
     for (; e < n;) {
         const r = e + n >>> 1;
         li(ut[r]) < t ? e = r + 1 : n = r
     }
     return e
 }
 
 function fc(t) {
-    (!ut.length || !ut.includes(t, oi && t.allowRecurse ? un + 1 : un)) && (t.id == null ? ut.push(t) : ut.splice(my(t.id), 0, t), ch())
+    (!ut.length || !ut.includes(t, oi && t.allowRecurse ? un + 1 : un)) && (t.id == null ? ut.push(t) : ut.splice(gy(t.id), 0, t), ch())
 }
 
 function ch() {
     !oi && !ua && (ua = !0, uc = ah.then(dh))
 }
 
-function gy(t) {
+function yy(t) {
     const e = ut.indexOf(t);
     e > un && ut.splice(e, 1)
 }
 
-function yy(t) {
+function by(t) {
     te(t) ? Zr.push(...t) : (!Cn || !Cn.includes(t, t.allowRecurse ? vr + 1 : vr)) && Zr.push(t), ch()
 }
 
 function uu(t, e = oi ? un + 1 : 0) {
     for (; e < ut.length; e++) {
         const n = ut[e];
         n && n.pre && (ut.splice(e, 1), e--, n())
@@ -909,49 +909,49 @@
             return
         }
         for (Cn = e, Cn.sort((n, r) => li(n) - li(r)), vr = 0; vr < Cn.length; vr++) Cn[vr]();
         Cn = null, vr = 0
     }
 }
 const li = t => t.id == null ? 1 / 0 : t.id,
-    by = (t, e) => {
+    vy = (t, e) => {
         const n = li(t) - li(e);
         if (n === 0) {
             if (t.pre && !e.pre) return -1;
             if (e.pre && !t.pre) return 1
         }
         return n
     };
 
 function dh(t) {
-    ua = !1, oi = !0, ut.sort(by);
+    ua = !1, oi = !0, ut.sort(vy);
     const e = en;
     try {
         for (un = 0; un < ut.length; un++) {
             const n = ut[un];
             n && n.active !== !1 && Qn(n, null, 14)
         }
     } finally {
         un = 0, ut.length = 0, uh(), oi = !1, uc = null, (ut.length || Zr.length) && dh()
     }
 }
 
-function vy(t, e, ...n) {
+function xy(t, e, ...n) {
     if (t.isUnmounted) return;
     const r = t.vnode.props || $e;
     let s = n;
     const i = e.startsWith("update:"),
         o = i && e.slice(7);
     if (o && o in r) {
         const u = `${o==="modelValue"?"model":o}Modifiers`,
             {
                 number: d,
                 trim: f
             } = r[u] || $e;
-        f && (s = n.map(h => je(h) ? h.trim() : h)), d && (s = n.map(ia))
+        f && (s = n.map(h => Ue(h) ? h.trim() : h)), d && (s = n.map(ia))
     }
     let l, a = r[l = pl(e)] || r[l = pl(yn(e))];
     !a && i && (a = r[l = pl(Ss(e))]), a && Vt(a, t, 6, s);
     const c = r[l + "Once"];
     if (c) {
         if (!t.emitted) t.emitted = {};
         else if (t.emitted[l]) return;
@@ -972,43 +972,43 @@
             u && (l = !0, lt(o, u))
         };
         !n && e.mixins.length && e.mixins.forEach(a), t.extends && a(t.extends), t.mixins && t.mixins.forEach(a)
     }
     return !i && !l ? (Ie(t) && r.set(t, null), null) : (te(i) ? i.forEach(a => o[a] = null) : lt(o, i), Ie(t) && r.set(t, o), o)
 }
 
-function Do(t, e) {
-    return !t || !Eo(e) ? !1 : (e = e.slice(2).replace(/Once$/, ""), _e(t, e[0].toLowerCase() + e.slice(1)) || _e(t, Ss(e)) || _e(t, e))
+function Po(t, e) {
+    return !t || !Oo(e) ? !1 : (e = e.slice(2).replace(/Once$/, ""), _e(t, e[0].toLowerCase() + e.slice(1)) || _e(t, Ss(e)) || _e(t, e))
 }
 let Rt = null,
-    Io = null;
+    $o = null;
 
-function eo(t) {
+function no(t) {
     const e = Rt;
-    return Rt = t, Io = t && t.type.__scopeId || null, e
+    return Rt = t, $o = t && t.type.__scopeId || null, e
 }
 
-function Po(t) {
-    Io = t
+function xi(t) {
+    $o = t
 }
 
-function $o() {
-    Io = null
+function ki() {
+    $o = null
 }
 
 function ht(t, e = Rt, n) {
     if (!e || t._n) return t;
     const r = (...s) => {
         r._d && ku(-1);
-        const i = eo(e);
+        const i = no(e);
         let o;
         try {
             o = t(...s)
         } finally {
-            eo(i), r._d && ku(1)
+            no(i), r._d && ku(1)
         }
         return o
     };
     return r._n = !0, r._c = !0, r._d = !0, r
 }
 
 function ml(t) {
@@ -1026,52 +1026,52 @@
         renderCache: d,
         data: f,
         setupState: h,
         ctx: p,
         inheritAttrs: g
     } = t;
     let v, x;
-    const w = eo(t);
+    const w = no(t);
     try {
         if (n.shapeFlag & 4) {
             const y = s || r;
             v = an(u.call(y, y, d, i, h, f, p)), x = a
         } else {
             const y = e;
             v = an(y.length > 1 ? y(i, {
                 attrs: a,
                 slots: l,
                 emit: c
-            }) : y(i, null)), x = e.props ? a : xy(a)
+            }) : y(i, null)), x = e.props ? a : ky(a)
         }
     } catch (y) {
-        Ks.length = 0, Ro(y, t, 1), v = ce(tn)
+        Ks.length = 0, Io(y, t, 1), v = ce(tn)
     }
     let S = v;
     if (x && g !== !1) {
         const y = Object.keys(x),
             {
                 shapeFlag: I
             } = S;
-        y.length && I & 7 && (o && y.some(Xa) && (x = ky(x, o)), S = Rn(S, x))
+        y.length && I & 7 && (o && y.some(Xa) && (x = wy(x, o)), S = Rn(S, x))
     }
-    return n.dirs && (S = Rn(S), S.dirs = S.dirs ? S.dirs.concat(n.dirs) : n.dirs), n.transition && (S.transition = n.transition), v = S, eo(w), v
+    return n.dirs && (S = Rn(S), S.dirs = S.dirs ? S.dirs.concat(n.dirs) : n.dirs), n.transition && (S.transition = n.transition), v = S, no(w), v
 }
-const xy = t => {
+const ky = t => {
         let e;
-        for (const n in t)(n === "class" || n === "style" || Eo(n)) && ((e || (e = {}))[n] = t[n]);
+        for (const n in t)(n === "class" || n === "style" || Oo(n)) && ((e || (e = {}))[n] = t[n]);
         return e
     },
-    ky = (t, e) => {
+    wy = (t, e) => {
         const n = {};
         for (const r in t)(!Xa(r) || !(r.slice(9) in e)) && (n[r] = t[r]);
         return n
     };
 
-function wy(t, e, n) {
+function Sy(t, e, n) {
     const {
         props: r,
         children: s,
         component: i
     } = t, {
         props: o,
         children: l,
@@ -1081,44 +1081,44 @@
     if (n && a >= 0) {
         if (a & 1024) return !0;
         if (a & 16) return r ? du(r, o, c) : !!o;
         if (a & 8) {
             const u = e.dynamicProps;
             for (let d = 0; d < u.length; d++) {
                 const f = u[d];
-                if (o[f] !== r[f] && !Do(c, f)) return !0
+                if (o[f] !== r[f] && !Po(c, f)) return !0
             }
         }
     } else return (s || l) && (!l || !l.$stable) ? !0 : r === o ? !1 : r ? o ? du(r, o, c) : !0 : !!o;
     return !1
 }
 
 function du(t, e, n) {
     const r = Object.keys(e);
     if (r.length !== Object.keys(t).length) return !0;
     for (let s = 0; s < r.length; s++) {
         const i = r[s];
-        if (e[i] !== t[i] && !Do(n, i)) return !0
+        if (e[i] !== t[i] && !Po(n, i)) return !0
     }
     return !1
 }
 
-function Sy({
+function _y({
     vnode: t,
     parent: e
 }, n) {
     for (; e && e.subTree === t;)(t = e.vnode).el = n, e = e.parent
 }
 const hh = t => t.__isSuspense;
 
-function _y(t, e) {
-    e && e.pendingBranch ? te(t) ? e.effects.push(...t) : e.effects.push(t) : yy(t)
+function Cy(t, e) {
+    e && e.pendingBranch ? te(t) ? e.effects.push(...t) : e.effects.push(t) : by(t)
 }
 
-function Vi(t, e) {
+function Ui(t, e) {
     if (qe) {
         let n = qe.provides;
         const r = qe.parent && qe.parent.provides;
         r === n && (n = qe.provides = Object.create(r)), n[t] = e
     }
 }
 
@@ -1127,34 +1127,34 @@
     if (r) {
         const s = r.parent == null ? r.vnode.appContext && r.vnode.appContext.provides : r.parent.provides;
         if (s && t in s) return s[t];
         if (arguments.length > 1) return n && me(e) ? e.call(r.proxy) : e
     }
 }
 
-function Cy(t, e) {
+function Ey(t, e) {
     return hc(t, null, e)
 }
-const Di = {};
+const Pi = {};
 
 function js(t, e, n) {
     return hc(t, e, n)
 }
 
 function hc(t, e, {
     immediate: n,
     deep: r,
     flush: s,
     onTrack: i,
     onTrigger: o
 } = $e) {
-    const l = Ig() === (qe == null ? void 0 : qe.scope) ? qe : null;
+    const l = Pg() === (qe == null ? void 0 : qe.scope) ? qe : null;
     let a, c = !1,
         u = !1;
-    if (ft(t) ? (a = () => t.value, c = Zi(t)) : Qr(t) ? (a = () => t, r = !0) : te(t) ? (u = !0, c = t.some(S => Qr(S) || Zi(S)), a = () => t.map(S => {
+    if (ft(t) ? (a = () => t.value, c = to(t)) : Qr(t) ? (a = () => t, r = !0) : te(t) ? (u = !0, c = t.some(S => Qr(S) || to(S)), a = () => t.map(S => {
             if (ft(S)) return S.value;
             if (Qr(S)) return _r(S);
             if (me(S)) return Qn(S, l, 2)
         })) : me(t) ? e ? a = () => Qn(t, l, 2) : a = () => {
             if (!(l && l.isUnmounted)) return d && d(), Vt(t, l, 3, [f])
         } : a = en, e && r) {
         const S = a;
@@ -1164,39 +1164,39 @@
             d = x.onStop = () => {
                 Qn(S, l, 4)
             }
         },
         h;
     if (ci)
         if (f = en, e ? n && Vt(e, l, 3, [a(), u ? [] : void 0, f]) : a(), s === "sync") {
-            const S = kb();
+            const S = wb();
             h = S.__watcherHandles || (S.__watcherHandles = [])
         } else return en;
-    let p = u ? new Array(t.length).fill(Di) : Di;
+    let p = u ? new Array(t.length).fill(Pi) : Pi;
     const g = () => {
         if (x.active)
             if (e) {
                 const S = x.run();
-                (r || c || (u ? S.some((y, I) => si(y, p[I])) : si(S, p))) && (d && d(), Vt(e, l, 3, [S, p === Di ? void 0 : u && p[0] === Di ? [] : p, f]), p = S)
+                (r || c || (u ? S.some((y, I) => si(y, p[I])) : si(S, p))) && (d && d(), Vt(e, l, 3, [S, p === Pi ? void 0 : u && p[0] === Pi ? [] : p, f]), p = S)
             } else x.run()
     };
     g.allowRecurse = !!e;
     let v;
     s === "sync" ? v = g : s === "post" ? v = () => rt(g, l && l.suspense) : (g.pre = !0, l && (g.id = l.uid), v = () => fc(g));
     const x = new tc(a, v);
     e ? n ? g() : p = x.run() : s === "post" ? rt(x.run.bind(x), l && l.suspense) : x.run();
     const w = () => {
         x.stop(), l && l.scope && Qa(l.scope.effects, x)
     };
     return h && h.push(w), w
 }
 
-function Ey(t, e, n) {
+function Ty(t, e, n) {
     const r = this.proxy,
-        s = je(t) ? t.includes(".") ? ph(r, t) : () => r[t] : t.bind(r, r);
+        s = Ue(t) ? t.includes(".") ? ph(r, t) : () => r[t] : t.bind(r, r);
     let i;
     me(e) ? i = e : (i = e.handler, n = e);
     const o = qe;
     is(this);
     const l = hc(s, i.bind(r), n);
     return o ? is(o) : Or(), l
 }
@@ -1211,37 +1211,37 @@
 }
 
 function _r(t, e) {
     if (!Ie(t) || t.__v_skip || (e = e || new Set, e.has(t))) return t;
     if (e.add(t), ft(t)) _r(t.value, e);
     else if (te(t))
         for (let n = 0; n < t.length; n++) _r(t[n], e);
-    else if (To(t) || Yr(t)) t.forEach(n => {
+    else if (Mo(t) || Yr(t)) t.forEach(n => {
         _r(n, e)
     });
     else if (Wf(t))
         for (const n in t) _r(t[n], e);
     return t
 }
 
-function Ty() {
+function Oy() {
     const t = {
         isMounted: !1,
         isLeaving: !1,
         isUnmounting: !1,
         leavingVNodes: new Map
     };
     return Ts(() => {
         t.isMounted = !0
     }), or(() => {
         t.isUnmounting = !0
     }), t
 }
 const $t = [Function, Array],
-    Oy = {
+    My = {
         name: "BaseTransition",
         props: {
             mode: String,
             appear: Boolean,
             persisted: Boolean,
             onBeforeEnter: $t,
             onEnter: $t,
@@ -1256,15 +1256,15 @@
             onAfterAppear: $t,
             onAppearCancelled: $t
         },
         setup(t, {
             slots: e
         }) {
             const n = bc(),
-                r = Ty();
+                r = Oy();
             let s;
             return () => {
                 const i = e.default && yh(e.default(), !0);
                 if (!i || !i.length) return;
                 let o = i[0];
                 if (i.length > 1) {
                     for (const g of i)
@@ -1277,42 +1277,42 @@
                     {
                         mode: a
                     } = l;
                 if (r.isLeaving) return gl(o);
                 const c = fu(o);
                 if (!c) return gl(o);
                 const u = da(c, l, r, n);
-                to(c, u);
+                ro(c, u);
                 const d = n.subTree,
                     f = d && fu(d);
                 let h = !1;
                 const {
                     getTransitionKey: p
                 } = c.type;
                 if (p) {
                     const g = p();
                     s === void 0 ? s = g : g !== s && (s = g, h = !0)
                 }
                 if (f && f.type !== tn && (!qn(c, f) || h)) {
                     const g = da(f, l, r, n);
-                    if (to(f, g), a === "out-in") return r.isLeaving = !0, g.afterLeave = () => {
+                    if (ro(f, g), a === "out-in") return r.isLeaving = !0, g.afterLeave = () => {
                         r.isLeaving = !1, n.update.active !== !1 && n.update()
                     }, gl(o);
                     a === "in-out" && c.type !== tn && (g.delayLeave = (v, x, w) => {
                         const S = gh(r, f);
                         S[String(f.key)] = f, v._leaveCb = () => {
                             x(), v._leaveCb = void 0, delete u.delayedLeave
                         }, u.delayedLeave = w
                     })
                 }
                 return o
             }
         }
     },
-    mh = Oy;
+    mh = My;
 
 function gh(t, e) {
     const {
         leavingVNodes: n
     } = t;
     let r = n.get(e.type);
     return r || (r = Object.create(null), n.set(e.type, r)), r
@@ -1386,25 +1386,25 @@
     if (Lo(t)) return t = Rn(t), t.children = null, t
 }
 
 function fu(t) {
     return Lo(t) ? t.children ? t.children[0] : void 0 : t
 }
 
-function to(t, e) {
-    t.shapeFlag & 6 && t.component ? to(t.component.subTree, e) : t.shapeFlag & 128 ? (t.ssContent.transition = e.clone(t.ssContent), t.ssFallback.transition = e.clone(t.ssFallback)) : t.transition = e
+function ro(t, e) {
+    t.shapeFlag & 6 && t.component ? ro(t.component.subTree, e) : t.shapeFlag & 128 ? (t.ssContent.transition = e.clone(t.ssContent), t.ssFallback.transition = e.clone(t.ssFallback)) : t.transition = e
 }
 
 function yh(t, e = !1, n) {
     let r = [],
         s = 0;
     for (let i = 0; i < t.length; i++) {
         let o = t[i];
         const l = n == null ? o.key : String(n) + String(o.key != null ? o.key : i);
-        o.type === Fe ? (o.patchFlag & 128 && s++, r = r.concat(yh(o.children, e, l))) : (e || o.type !== tn) && r.push(l != null ? Rn(o, {
+        o.type === Le ? (o.patchFlag & 128 && s++, r = r.concat(yh(o.children, e, l))) : (e || o.type !== tn) && r.push(l != null ? Rn(o, {
             key: l
         }) : o)
     }
     if (s > 1)
         for (let i = 0; i < r.length; i++) r[i].patchFlag = -2;
     return r
 }
@@ -1413,15 +1413,15 @@
     return me(t) ? {
         setup: t,
         name: t.name
     } : t
 }
 const Us = t => !!t.type.__asyncLoader,
     Lo = t => t.type.__isKeepAlive,
-    My = {
+    Ay = {
         name: "KeepAlive",
         __isKeepAlive: !0,
         props: {
             include: [String, RegExp, Array],
             exclude: [String, RegExp, Array],
             max: [String, Number]
         },
@@ -1505,60 +1505,60 @@
                     h(w)
                 })
             }), () => {
                 if (v = null, !e.default) return null;
                 const w = e.default(),
                     S = w[0];
                 if (w.length > 1) return o = null, w;
-                if (!ro(S) || !(S.shapeFlag & 4) && !(S.shapeFlag & 128)) return o = null, S;
+                if (!io(S) || !(S.shapeFlag & 4) && !(S.shapeFlag & 128)) return o = null, S;
                 let y = bl(S);
                 const I = y.type,
                     T = ba(Us(y) ? y.type.__asyncResolved || {} : I),
                     {
                         include: V,
                         exclude: N,
                         max: G
                     } = t;
                 if (V && (!T || !Bs(V, T)) || N && T && Bs(N, T)) return o = y, S;
                 const J = y.key == null ? I : y.key,
                     ne = s.get(J);
-                return y.el && (y = Rn(y), S.shapeFlag & 128 && (S.ssContent = y)), v = J, ne ? (y.el = ne.el, y.component = ne.component, y.transition && to(y, y.transition), y.shapeFlag |= 512, i.delete(J), i.add(J)) : (i.add(J), G && i.size > parseInt(G, 10) && g(i.values().next().value)), y.shapeFlag |= 256, o = y, hh(S.type) ? S : y
+                return y.el && (y = Rn(y), S.shapeFlag & 128 && (S.ssContent = y)), v = J, ne ? (y.el = ne.el, y.component = ne.component, y.transition && ro(y, y.transition), y.shapeFlag |= 512, i.delete(J), i.add(J)) : (i.add(J), G && i.size > parseInt(G, 10) && g(i.values().next().value)), y.shapeFlag |= 256, o = y, hh(S.type) ? S : y
             }
         }
     },
-    Ay = My;
+    Ny = Ay;
 
 function Bs(t, e) {
-    return te(t) ? t.some(n => Bs(n, e)) : je(t) ? t.split(",").includes(e) : Eg(t) ? t.test(e) : !1
+    return te(t) ? t.some(n => Bs(n, e)) : Ue(t) ? t.split(",").includes(e) : Tg(t) ? t.test(e) : !1
 }
 
-function Ny(t, e) {
+function Ry(t, e) {
     bh(t, "a", e)
 }
 
-function Ry(t, e) {
+function Dy(t, e) {
     bh(t, "da", e)
 }
 
 function bh(t, e, n = qe) {
     const r = t.__wdc || (t.__wdc = () => {
         let s = n;
         for (; s;) {
             if (s.isDeactivated) return;
             s = s.parent
         }
         return t()
     });
     if (Fo(e, r, n), n) {
         let s = n.parent;
-        for (; s && s.parent;) Lo(s.parent.vnode) && Dy(r, e, n, s), s = s.parent
+        for (; s && s.parent;) Lo(s.parent.vnode) && Iy(r, e, n, s), s = s.parent
     }
 }
 
-function Dy(t, e, n, r) {
+function Iy(t, e, n, r) {
     const s = Fo(e, t, r, !0);
     xh(() => {
         Qa(r[e], s)
     }, n)
 }
 
 function yl(t) {
@@ -1578,25 +1578,25 @@
                 const l = Vt(e, n, t, o);
                 return Or(), Cs(), l
             });
         return r ? s.unshift(i) : s.push(i), i
     }
 }
 const In = t => (e, n = qe) => (!ci || t === "sp") && Fo(t, (...r) => e(...r), n),
-    Iy = In("bm"),
+    Py = In("bm"),
     Ts = In("m"),
-    Py = In("bu"),
+    $y = In("bu"),
     vh = In("u"),
     or = In("bum"),
     xh = In("um"),
-    $y = In("sp"),
-    Ly = In("rtg"),
-    Fy = In("rtc");
+    Ly = In("sp"),
+    Fy = In("rtg"),
+    By = In("rtc");
 
-function By(t, e = qe) {
+function Hy(t, e = qe) {
     Fo("ec", t, e)
 }
 
 function We(t, e) {
     const n = Rt;
     if (n === null) return t;
     const r = zo(n) || n.proxy,
@@ -1627,39 +1627,39 @@
         let a = l.dir[r];
         a && (_s(), Vt(a, n, 8, [t.el, l, t, e]), Cs())
     }
 }
 const kh = "components";
 
 function Oe(t, e) {
-    return zy(kh, t, !0, e) || t
+    return Vy(kh, t, !0, e) || t
 }
-const Hy = Symbol();
+const zy = Symbol();
 
-function zy(t, e, n = !0, r = !1) {
+function Vy(t, e, n = !0, r = !1) {
     const s = Rt || qe;
     if (s) {
         const i = s.type;
         if (t === kh) {
             const l = ba(i, !1);
-            if (l && (l === e || l === yn(e) || l === Mo(yn(e)))) return i
+            if (l && (l === e || l === yn(e) || l === No(yn(e)))) return i
         }
         const o = hu(s[t] || i[t], e) || hu(s.appContext[t], e);
         return !o && r ? i : o
     }
 }
 
 function hu(t, e) {
-    return t && (t[e] || t[yn(e)] || t[Mo(yn(e))])
+    return t && (t[e] || t[yn(e)] || t[No(yn(e))])
 }
 
 function Dt(t, e, n, r) {
     let s;
     const i = n && n[r];
-    if (te(t) || je(t)) {
+    if (te(t) || Ue(t)) {
         s = new Array(t.length);
         for (let o = 0, l = t.length; o < l; o++) s[o] = e(t[o], o, void 0, i && i[o])
     } else if (typeof t == "number") {
         s = new Array(t);
         for (let o = 0; o < t; o++) s[o] = e(o + 1, o, void 0, i && i[o])
     } else if (Ie(t))
         if (t[Symbol.iterator]) s = Array.from(t, (o, l) => e(o, l, void 0, i && i[l]));
@@ -1685,18 +1685,18 @@
         $refs: t => t.refs,
         $parent: t => fa(t.parent),
         $root: t => fa(t.root),
         $emit: t => t.emit,
         $options: t => pc(t),
         $forceUpdate: t => t.f || (t.f = () => fc(t.update)),
         $nextTick: t => t.n || (t.n = dc.bind(t.proxy)),
-        $watch: t => Ey.bind(t)
+        $watch: t => Ty.bind(t)
     }),
     vl = (t, e) => t !== $e && !t.__isScriptSetup && _e(t, e),
-    Vy = {
+    jy = {
         get({
             _: t
         }, e) {
             const {
                 ctx: n,
                 setupState: r,
                 data: s,
@@ -1757,15 +1757,15 @@
         },
         defineProperty(t, e, n) {
             return n.get != null ? t._.accessCache[e] = 0 : _e(n, "value") && this.set(t, e, n.value, null), Reflect.defineProperty(t, e, n)
         }
     };
 let ha = !0;
 
-function jy(t) {
+function Uy(t) {
     const e = pc(t),
         n = t.proxy,
         r = t.ctx;
     ha = !1, e.beforeCreate && pu(e.beforeCreate, t, "bc");
     const {
         data: s,
         computed: i,
@@ -1791,66 +1791,66 @@
         serverPrefetch: G,
         expose: J,
         inheritAttrs: ne,
         components: H,
         directives: ie,
         filters: Ae
     } = e;
-    if (c && Uy(c, r, null, t.appContext.config.unwrapInjectedRef), o)
-        for (const fe in o) {
-            const ae = o[fe];
-            me(ae) && (r[fe] = ae.bind(n))
+    if (c && Wy(c, r, null, t.appContext.config.unwrapInjectedRef), o)
+        for (const he in o) {
+            const ae = o[he];
+            me(ae) && (r[he] = ae.bind(n))
         }
     if (s) {
-        const fe = s.call(n, n);
-        Ie(fe) && (t.data = Es(fe))
+        const he = s.call(n, n);
+        Ie(he) && (t.data = Es(he))
     }
     if (ha = !0, i)
-        for (const fe in i) {
-            const ae = i[fe],
-                He = me(ae) ? ae.bind(n, n) : me(ae.get) ? ae.get.bind(n, n) : en,
+        for (const he in i) {
+            const ae = i[he],
+                ze = me(ae) ? ae.bind(n, n) : me(ae.get) ? ae.get.bind(n, n) : en,
                 Ze = !me(ae) && me(ae.set) ? ae.set.bind(n) : en,
                 Ke = Bt({
-                    get: He,
+                    get: ze,
                     set: Ze
                 });
-            Object.defineProperty(r, fe, {
+            Object.defineProperty(r, he, {
                 enumerable: !0,
                 configurable: !0,
                 get: () => Ke.value,
                 set: Pe => Ke.value = Pe
             })
         }
     if (l)
-        for (const fe in l) wh(l[fe], r, n, fe);
+        for (const he in l) wh(l[he], r, n, he);
     if (a) {
-        const fe = me(a) ? a.call(n) : a;
-        Reflect.ownKeys(fe).forEach(ae => {
-            Vi(ae, fe[ae])
+        const he = me(a) ? a.call(n) : a;
+        Reflect.ownKeys(he).forEach(ae => {
+            Ui(ae, he[ae])
         })
     }
     u && pu(u, t, "c");
 
-    function ge(fe, ae) {
-        te(ae) ? ae.forEach(He => fe(He.bind(n))) : ae && fe(ae.bind(n))
+    function ge(he, ae) {
+        te(ae) ? ae.forEach(ze => he(ze.bind(n))) : ae && he(ae.bind(n))
     }
-    if (ge(Iy, d), ge(Ts, f), ge(Py, h), ge(vh, p), ge(Ny, g), ge(Ry, v), ge(By, N), ge(Fy, T), ge(Ly, V), ge(or, w), ge(xh, y), ge($y, G), te(J))
+    if (ge(Py, d), ge(Ts, f), ge($y, h), ge(vh, p), ge(Ry, g), ge(Dy, v), ge(Hy, N), ge(By, T), ge(Fy, V), ge(or, w), ge(xh, y), ge(Ly, G), te(J))
         if (J.length) {
-            const fe = t.exposed || (t.exposed = {});
+            const he = t.exposed || (t.exposed = {});
             J.forEach(ae => {
-                Object.defineProperty(fe, ae, {
+                Object.defineProperty(he, ae, {
                     get: () => n[ae],
-                    set: He => n[ae] = He
+                    set: ze => n[ae] = ze
                 })
             })
         } else t.exposed || (t.exposed = {});
     I && t.render === en && (t.render = I), ne != null && (t.inheritAttrs = ne), H && (t.components = H), ie && (t.directives = ie)
 }
 
-function Uy(t, e, n = en, r = !1) {
+function Wy(t, e, n = en, r = !1) {
     te(t) && (t = pa(t));
     for (const s in t) {
         const i = t[s];
         let o;
         Ie(i) ? "default" in i ? o = On(i.from || s, i.default, !0) : o = On(i.from || s) : o = On(i), ft(o) && r ? Object.defineProperty(e, s, {
             enumerable: !0,
             configurable: !0,
@@ -1862,15 +1862,15 @@
 
 function pu(t, e, n) {
     Vt(te(t) ? t.map(r => r.bind(e.proxy)) : t.bind(e.proxy), e, n)
 }
 
 function wh(t, e, n, r) {
     const s = r.includes(".") ? ph(n, r) : () => n[r];
-    if (je(t)) {
+    if (Ue(t)) {
         const i = e[t];
         me(i) && js(s, i)
     } else if (me(t)) js(s, t.bind(n));
     else if (Ie(t))
         if (te(t)) t.forEach(i => wh(i, e, n, r));
         else {
             const i = me(t.handler) ? t.handler.bind(n) : e[t.handler];
@@ -1889,30 +1889,30 @@
             optionsCache: i,
             config: {
                 optionMergeStrategies: o
             }
         } = t.appContext,
         l = i.get(e);
     let a;
-    return l ? a = l : !s.length && !n && !r ? a = e : (a = {}, s.length && s.forEach(c => no(a, c, o, !0)), no(a, e, o)), Ie(e) && i.set(e, a), a
+    return l ? a = l : !s.length && !n && !r ? a = e : (a = {}, s.length && s.forEach(c => so(a, c, o, !0)), so(a, e, o)), Ie(e) && i.set(e, a), a
 }
 
-function no(t, e, n, r = !1) {
+function so(t, e, n, r = !1) {
     const {
         mixins: s,
         extends: i
     } = e;
-    i && no(t, i, n, !0), s && s.forEach(o => no(t, o, n, !0));
+    i && so(t, i, n, !0), s && s.forEach(o => so(t, o, n, !0));
     for (const o in e)
         if (!(r && o === "expose")) {
-            const l = Wy[o] || n && n[o];
+            const l = qy[o] || n && n[o];
             t[o] = l ? l(t[o], e[o]) : e[o]
         } return t
 }
-const Wy = {
+const qy = {
     data: mu,
     props: yr,
     emits: yr,
     methods: yr,
     computed: yr,
     beforeCreate: gt,
     created: gt,
@@ -1926,26 +1926,26 @@
     unmounted: gt,
     activated: gt,
     deactivated: gt,
     errorCaptured: gt,
     serverPrefetch: gt,
     components: yr,
     directives: yr,
-    watch: Ky,
+    watch: Jy,
     provide: mu,
-    inject: qy
+    inject: Ky
 };
 
 function mu(t, e) {
     return e ? t ? function() {
         return lt(me(t) ? t.call(this, this) : t, me(e) ? e.call(this, this) : e)
     } : e : t
 }
 
-function qy(t, e) {
+function Ky(t, e) {
     return yr(pa(t), pa(e))
 }
 
 function pa(t) {
     if (te(t)) {
         const e = {};
         for (let n = 0; n < t.length; n++) e[t[n]] = t[n];
@@ -1958,45 +1958,45 @@
     return t ? [...new Set([].concat(t, e))] : e
 }
 
 function yr(t, e) {
     return t ? lt(lt(Object.create(null), t), e) : e
 }
 
-function Ky(t, e) {
+function Jy(t, e) {
     if (!t) return e;
     if (!e) return t;
     const n = lt(Object.create(null), t);
     for (const r in e) n[r] = gt(t[r], e[r]);
     return n
 }
 
-function Jy(t, e, n, r = !1) {
+function Gy(t, e, n, r = !1) {
     const s = {},
         i = {};
-    Qi(i, Ho, 1), t.propsDefaults = Object.create(null), Sh(t, e, s, i);
+    eo(i, Ho, 1), t.propsDefaults = Object.create(null), Sh(t, e, s, i);
     for (const o in t.propsOptions[0]) o in s || (s[o] = void 0);
-    n ? t.props = r ? s : ly(s) : t.type.props ? t.props = s : t.props = i, t.attrs = i
+    n ? t.props = r ? s : ay(s) : t.type.props ? t.props = s : t.props = i, t.attrs = i
 }
 
-function Gy(t, e, n, r) {
+function Yy(t, e, n, r) {
     const {
         props: s,
         attrs: i,
         vnode: {
             patchFlag: o
         }
     } = t, l = Me(s), [a] = t.propsOptions;
     let c = !1;
     if ((r || o > 0) && !(o & 16)) {
         if (o & 8) {
             const u = t.vnode.dynamicProps;
             for (let d = 0; d < u.length; d++) {
                 let f = u[d];
-                if (Do(t.emitsOptions, f)) continue;
+                if (Po(t.emitsOptions, f)) continue;
                 const h = e[f];
                 if (a)
                     if (_e(i, f)) h !== i[f] && (i[f] = h, c = !0);
                     else {
                         const p = yn(f);
                         s[p] = ma(a, l, p, h, t, !1)
                     }
@@ -2015,18 +2015,18 @@
 
 function Sh(t, e, n, r) {
     const [s, i] = t.propsOptions;
     let o = !1,
         l;
     if (e)
         for (let a in e) {
-            if (zi(a)) continue;
+            if (ji(a)) continue;
             const c = e[a];
             let u;
-            s && _e(s, u = yn(a)) ? !i || !i.includes(u) ? n[u] = c : (l || (l = {}))[u] = c : Do(t.emitsOptions, a) || (!(a in r) || c !== r[a]) && (r[a] = c, o = !0)
+            s && _e(s, u = yn(a)) ? !i || !i.includes(u) ? n[u] = c : (l || (l = {}))[u] = c : Po(t.emitsOptions, a) || (!(a in r) || c !== r[a]) && (r[a] = c, o = !0)
         }
     if (i) {
         const a = Me(n),
             c = l || $e;
         for (let u = 0; u < i.length; u++) {
             const d = i[u];
             n[d] = ma(s, a, d, c[d], t, !_e(c, d))
@@ -2107,43 +2107,43 @@
 }
 
 function vu(t, e) {
     return te(e) ? e.findIndex(n => bu(n, t)) : me(e) && bu(e, t) ? 0 : -1
 }
 const Ch = t => t[0] === "_" || t === "$stable",
     mc = t => te(t) ? t.map(an) : [an(t)],
-    Yy = (t, e, n) => {
+    Xy = (t, e, n) => {
         if (e._n) return e;
         const r = ht((...s) => mc(e(...s)), n);
         return r._c = !1, r
     },
     Eh = (t, e, n) => {
         const r = t._ctx;
         for (const s in t) {
             if (Ch(s)) continue;
             const i = t[s];
-            if (me(i)) e[s] = Yy(s, i, r);
+            if (me(i)) e[s] = Xy(s, i, r);
             else if (i != null) {
                 const o = mc(i);
                 e[s] = () => o
             }
         }
     },
     Th = (t, e) => {
         const n = mc(e);
         t.slots.default = () => n
     },
-    Xy = (t, e) => {
+    Qy = (t, e) => {
         if (t.vnode.shapeFlag & 32) {
             const n = e._;
-            n ? (t.slots = Me(e), Qi(e, "_", n)) : Eh(e, t.slots = {})
+            n ? (t.slots = Me(e), eo(e, "_", n)) : Eh(e, t.slots = {})
         } else t.slots = {}, e && Th(t, e);
-        Qi(t.slots, Ho, 1)
+        eo(t.slots, Ho, 1)
     },
-    Qy = (t, e, n) => {
+    Zy = (t, e, n) => {
         const {
             vnode: r,
             slots: s
         } = t;
         let i = !0,
             o = $e;
         if (r.shapeFlag & 32) {
@@ -2156,15 +2156,15 @@
             for (const l in s) !Ch(l) && !(l in o) && delete s[l]
     };
 
 function Oh() {
     return {
         app: null,
         config: {
-            isNativeTag: Sg,
+            isNativeTag: _g,
             performance: !1,
             globalProperties: {},
             optionMergeStrategies: {},
             errorHandler: void 0,
             warnHandler: void 0,
             compilerOptions: {}
         },
@@ -2173,30 +2173,30 @@
         directives: {},
         provides: Object.create(null),
         optionsCache: new WeakMap,
         propsCache: new WeakMap,
         emitsCache: new WeakMap
     }
 }
-let Zy = 0;
+let eb = 0;
 
-function eb(t, e) {
+function tb(t, e) {
     return function(r, s = null) {
         me(r) || (r = Object.assign({}, r)), s != null && !Ie(s) && (s = null);
         const i = Oh(),
             o = new Set;
         let l = !1;
         const a = i.app = {
-            _uid: Zy++,
+            _uid: eb++,
             _component: r,
             _props: s,
             _container: null,
             _context: i,
             _instance: null,
-            version: wb,
+            version: Sb,
             get config() {
                 return i.config
             },
             set config(c) {},
             use(c, ...u) {
                 return o.has(c) || (c && me(c.install) ? (o.add(c), c.install(a, ...u)) : me(c) && (o.add(c), c(a, ...u))), a
             },
@@ -2237,37 +2237,37 @@
         {
             i: l,
             r: a
         } = t,
         c = e && e.r,
         u = l.refs === $e ? l.refs = {} : l.refs,
         d = l.setupState;
-    if (c != null && c !== a && (je(c) ? (u[c] = null, _e(d, c) && (d[c] = null)) : ft(c) && (c.value = null)), me(a)) Qn(a, l, 12, [o, u]);
+    if (c != null && c !== a && (Ue(c) ? (u[c] = null, _e(d, c) && (d[c] = null)) : ft(c) && (c.value = null)), me(a)) Qn(a, l, 12, [o, u]);
     else {
-        const f = je(a),
+        const f = Ue(a),
             h = ft(a);
         if (f || h) {
             const p = () => {
                 if (t.f) {
                     const g = f ? _e(d, a) ? d[a] : u[a] : a.value;
                     s ? te(g) && Qa(g, i) : te(g) ? g.includes(i) || g.push(i) : f ? (u[a] = [i], _e(d, a) && (d[a] = u[a])) : (a.value = [i], t.k && (u[t.k] = a.value))
                 } else f ? (u[a] = o, _e(d, a) && (d[a] = o)) : h && (a.value = o, t.k && (u[t.k] = o))
             };
             o ? (p.id = -1, rt(p, n)) : p()
         }
     }
 }
-const rt = _y;
+const rt = Cy;
 
-function tb(t) {
-    return nb(t)
+function nb(t) {
+    return rb(t)
 }
 
-function nb(t, e) {
-    const n = Ng();
+function rb(t, e) {
+    const n = Rg();
     n.__VUE__ = !0;
     const {
         insert: r,
         remove: s,
         patchProp: i,
         createElement: o,
         createText: l,
@@ -2292,15 +2292,15 @@
                 break;
             case tn:
                 x(b, k, _, O);
                 break;
             case xl:
                 b == null && w(k, _, O, U);
                 break;
-            case Fe:
+            case Le:
                 H(b, k, _, O, D, F, U, L, B);
                 break;
             default:
                 K & 1 ? I(b, k, _, O, D, F, U, L, B) : K & 6 ? ie(b, k, _, O, D, F, U, L, B) : (K & 64 || K & 128) && P.process(b, k, _, O, D, F, U, L, B, ye)
         }
         Q != null && D && ga(Q, b && b.ref, F, k || b, !k)
     }, v = (b, k, _, O) => {
@@ -2335,15 +2335,15 @@
             type: Q,
             props: K,
             shapeFlag: Z,
             transition: oe,
             dirs: pe
         } = b;
         if (B = b.el = o(b.type, F, K && K.is, K), Z & 8 ? u(B, b.children) : Z & 16 && N(b.children, B, null, O, D, F && Q !== "foreignObject", U, L), pe && hr(b, null, O, "created"), V(B, b, b.scopeId, U, O), K) {
-            for (const we in K) we !== "value" && !zi(we) && i(B, we, null, K[we], F, b.children, O, D, j);
+            for (const we in K) we !== "value" && !ji(we) && i(B, we, null, K[we], F, b.children, O, D, j);
             "value" in K && i(B, "value", null, K.value), (P = K.onVnodeBeforeMount) && Lt(P, O, b)
         }
         pe && hr(b, null, O, "beforeMount");
         const Ne = (!D || D && !D.pendingBranch) && oe && !oe.persisted;
         Ne && oe.beforeEnter(B), r(B, k, _), ((P = K && K.onVnodeMounted) || Ne || pe) && rt(() => {
             P && Lt(P, O, b), Ne && oe.enter(B), pe && hr(b, null, O, "mounted")
         }, D)
@@ -2376,38 +2376,38 @@
         _ && pr(_, !1), (oe = Z.onVnodeBeforeUpdate) && Lt(oe, _, k, b), Q && hr(k, b, _, "beforeUpdate"), _ && pr(_, !0);
         const pe = D && k.type !== "foreignObject";
         if (P ? J(b.dynamicChildren, P, L, _, O, pe, F) : U || ae(b, k, L, null, _, O, pe, F, !1), B > 0) {
             if (B & 16) ne(L, k, K, Z, _, O, D);
             else if (B & 2 && K.class !== Z.class && i(L, "class", null, Z.class, D), B & 4 && i(L, "style", K.style, Z.style, D), B & 8) {
                 const Ne = k.dynamicProps;
                 for (let we = 0; we < Ne.length; we++) {
-                    const ze = Ne[we],
-                        At = K[ze],
-                        Pn = Z[ze];
-                    (Pn !== At || ze === "value") && i(L, ze, At, Pn, D, b.children, _, O, j)
+                    const Ve = Ne[we],
+                        At = K[Ve],
+                        Pn = Z[Ve];
+                    (Pn !== At || Ve === "value") && i(L, Ve, At, Pn, D, b.children, _, O, j)
                 }
             }
             B & 1 && b.children !== k.children && u(L, k.children)
         } else !U && P == null && ne(L, k, K, Z, _, O, D);
         ((oe = Z.onVnodeUpdated) || Q) && rt(() => {
             oe && Lt(oe, _, k, b), Q && hr(k, b, _, "updated")
         }, O)
     }, J = (b, k, _, O, D, F, U) => {
         for (let L = 0; L < k.length; L++) {
             const B = b[L],
                 P = k[L],
-                Q = B.el && (B.type === Fe || !qn(B, P) || B.shapeFlag & 70) ? d(B.el) : _;
+                Q = B.el && (B.type === Le || !qn(B, P) || B.shapeFlag & 70) ? d(B.el) : _;
             g(B, P, Q, null, O, D, F, U, !0)
         }
     }, ne = (b, k, _, O, D, F, U) => {
         if (_ !== O) {
             if (_ !== $e)
-                for (const L in _) !zi(L) && !(L in O) && i(b, L, _[L], null, U, k.children, D, F, j);
+                for (const L in _) !ji(L) && !(L in O) && i(b, L, _[L], null, U, k.children, D, F, j);
             for (const L in O) {
-                if (zi(L)) continue;
+                if (ji(L)) continue;
                 const B = O[L],
                     P = _[L];
                 B !== P && L !== "value" && i(b, L, P, B, U, k.children, D, F, j)
             }
             "value" in O && i(b, "value", _.value, O.value)
         }
     }, H = (b, k, _, O, D, F, U, L, B) => {
@@ -2416,98 +2416,98 @@
         let {
             patchFlag: K,
             dynamicChildren: Z,
             slotScopeIds: oe
         } = k;
         oe && (L = L ? L.concat(oe) : oe), b == null ? (r(P, _, O), r(Q, _, O), N(k.children, _, Q, D, F, U, L, B)) : K > 0 && K & 64 && Z && b.dynamicChildren ? (J(b.dynamicChildren, Z, _, D, F, U, L), (k.key != null || D && k === D.subTree) && gc(b, k, !0)) : ae(b, k, _, Q, D, F, U, L, B)
     }, ie = (b, k, _, O, D, F, U, L, B) => {
-        k.slotScopeIds = L, b == null ? k.shapeFlag & 512 ? D.ctx.activate(k, _, O, U, B) : Ae(k, _, O, D, F, U, B) : Be(b, k, B)
+        k.slotScopeIds = L, b == null ? k.shapeFlag & 512 ? D.ctx.activate(k, _, O, U, B) : Ae(k, _, O, D, F, U, B) : He(b, k, B)
     }, Ae = (b, k, _, O, D, F, U) => {
-        const L = b.component = pb(b, O, D);
-        if (Lo(b) && (L.ctx.renderer = ye), mb(L), L.asyncDep) {
+        const L = b.component = mb(b, O, D);
+        if (Lo(b) && (L.ctx.renderer = ye), gb(L), L.asyncDep) {
             if (D && D.registerDep(L, ge), !b.el) {
                 const B = L.subTree = ce(tn);
                 x(null, B, k, _)
             }
             return
         }
         ge(L, b, k, _, D, F, U)
-    }, Be = (b, k, _) => {
+    }, He = (b, k, _) => {
         const O = k.component = b.component;
-        if (wy(b, k, _))
+        if (Sy(b, k, _))
             if (O.asyncDep && !O.asyncResolved) {
-                fe(O, k, _);
+                he(O, k, _);
                 return
-            } else O.next = k, gy(O.update), O.update();
+            } else O.next = k, yy(O.update), O.update();
         else k.el = b.el, O.vnode = k
     }, ge = (b, k, _, O, D, F, U) => {
         const L = () => {
                 if (b.isMounted) {
                     let {
                         next: Q,
                         bu: K,
                         u: Z,
                         parent: oe,
                         vnode: pe
                     } = b, Ne = Q, we;
-                    pr(b, !1), Q ? (Q.el = pe.el, fe(b, Q, U)) : Q = pe, K && Xr(K), (we = Q.props && Q.props.onVnodeBeforeUpdate) && Lt(we, oe, Q, pe), pr(b, !0);
-                    const ze = ml(b),
+                    pr(b, !1), Q ? (Q.el = pe.el, he(b, Q, U)) : Q = pe, K && Xr(K), (we = Q.props && Q.props.onVnodeBeforeUpdate) && Lt(we, oe, Q, pe), pr(b, !0);
+                    const Ve = ml(b),
                         At = b.subTree;
-                    b.subTree = ze, g(At, ze, d(At.el), z(At), b, D, F), Q.el = ze.el, Ne === null && Sy(b, ze.el), Z && rt(Z, D), (we = Q.props && Q.props.onVnodeUpdated) && rt(() => Lt(we, oe, Q, pe), D)
+                    b.subTree = Ve, g(At, Ve, d(At.el), z(At), b, D, F), Q.el = Ve.el, Ne === null && _y(b, Ve.el), Z && rt(Z, D), (we = Q.props && Q.props.onVnodeUpdated) && rt(() => Lt(we, oe, Q, pe), D)
                 } else {
                     let Q;
                     const {
                         el: K,
                         props: Z
                     } = k, {
                         bm: oe,
                         m: pe,
                         parent: Ne
                     } = b, we = Us(k);
                     if (pr(b, !1), oe && Xr(oe), !we && (Q = Z && Z.onVnodeBeforeMount) && Lt(Q, Ne, k), pr(b, !0), K && ue) {
-                        const ze = () => {
+                        const Ve = () => {
                             b.subTree = ml(b), ue(K, b.subTree, b, D, null)
                         };
-                        we ? k.type.__asyncLoader().then(() => !b.isUnmounted && ze()) : ze()
+                        we ? k.type.__asyncLoader().then(() => !b.isUnmounted && Ve()) : Ve()
                     } else {
-                        const ze = b.subTree = ml(b);
-                        g(null, ze, _, O, b, D, F), k.el = ze.el
+                        const Ve = b.subTree = ml(b);
+                        g(null, Ve, _, O, b, D, F), k.el = Ve.el
                     }
                     if (pe && rt(pe, D), !we && (Q = Z && Z.onVnodeMounted)) {
-                        const ze = k;
-                        rt(() => Lt(Q, Ne, ze), D)
+                        const Ve = k;
+                        rt(() => Lt(Q, Ne, Ve), D)
                     }(k.shapeFlag & 256 || Ne && Us(Ne.vnode) && Ne.vnode.shapeFlag & 256) && b.a && rt(b.a, D), b.isMounted = !0, k = _ = O = null
                 }
             },
             B = b.effect = new tc(L, () => fc(P), b.scope),
             P = b.update = () => B.run();
         P.id = b.uid, pr(b, !0), P()
-    }, fe = (b, k, _) => {
+    }, he = (b, k, _) => {
         k.component = b;
         const O = b.vnode.props;
-        b.vnode = k, b.next = null, Gy(b, k.props, O, _), Qy(b, k.children, _), _s(), uu(), Cs()
+        b.vnode = k, b.next = null, Yy(b, k.props, O, _), Zy(b, k.children, _), _s(), uu(), Cs()
     }, ae = (b, k, _, O, D, F, U, L, B = !1) => {
         const P = b && b.children,
             Q = b ? b.shapeFlag : 0,
             K = k.children,
             {
                 patchFlag: Z,
                 shapeFlag: oe
             } = k;
         if (Z > 0) {
             if (Z & 128) {
                 Ze(P, K, _, O, D, F, U, L, B);
                 return
             } else if (Z & 256) {
-                He(P, K, _, O, D, F, U, L, B);
+                ze(P, K, _, O, D, F, U, L, B);
                 return
             }
         }
         oe & 8 ? (Q & 16 && j(P, D, F), K !== P && u(_, K)) : Q & 16 ? oe & 16 ? Ze(P, K, _, O, D, F, U, L, B) : j(P, D, F, !0) : (Q & 8 && u(_, ""), oe & 16 && N(K, _, O, D, F, U, L, B))
-    }, He = (b, k, _, O, D, F, U, L, B) => {
+    }, ze = (b, k, _, O, D, F, U, L, B) => {
         b = b || Gr, k = k || Gr;
         const P = b.length,
             Q = k.length,
             K = Math.min(P, Q);
         let Z;
         for (Z = 0; Z < K; Z++) {
             const oe = k[Z] = B ? jn(k[Z]) : an(k[Z]);
@@ -2545,36 +2545,36 @@
             const oe = P,
                 pe = P,
                 Ne = new Map;
             for (P = pe; P <= Z; P++) {
                 const W = k[P] = B ? jn(k[P]) : an(k[P]);
                 W.key != null && Ne.set(W.key, P)
             }
-            let we, ze = 0;
+            let we, Ve = 0;
             const At = Z - pe + 1;
             let Pn = !1,
-                Ci = 0;
+                Ti = 0;
             const dr = new Array(At);
             for (P = 0; P < At; P++) dr[P] = 0;
             for (P = oe; P <= K; P++) {
                 const W = b[P];
-                if (ze >= At) {
+                if (Ve >= At) {
                     Pe(W, D, F, !0);
                     continue
                 }
                 let ee;
                 if (W.key != null) ee = Ne.get(W.key);
                 else
                     for (we = pe; we <= Z; we++)
                         if (dr[we - pe] === 0 && qn(W, k[we])) {
                             ee = we;
                             break
-                        } ee === void 0 ? Pe(W, D, F, !0) : (dr[ee - pe] = P + 1, ee >= Ci ? Ci = ee : Pn = !0, g(W, k[ee], _, null, D, F, U, L, B), ze++)
+                        } ee === void 0 ? Pe(W, D, F, !0) : (dr[ee - pe] = P + 1, ee >= Ti ? Ti = ee : Pn = !0, g(W, k[ee], _, null, D, F, U, L, B), Ve++)
             }
-            const E = Pn ? rb(dr) : Gr;
+            const E = Pn ? sb(dr) : Gr;
             for (we = E.length - 1, P = At - 1; P >= 0; P--) {
                 const W = pe + P,
                     ee = k[W],
                     Te = W + 1 < Q ? k[W + 1].el : O;
                 dr[P] === 0 ? g(null, ee, _, Te, D, F, U, L, B) : Pn && (we < 0 || P !== E[we] ? Ke(ee, _, Te, 2) : we--)
             }
         }
@@ -2594,15 +2594,15 @@
             b.suspense.move(k, _, O);
             return
         }
         if (P & 64) {
             U.move(b, k, _, ye);
             return
         }
-        if (U === Fe) {
+        if (U === Le) {
             r(F, k, _);
             for (let K = 0; K < B.length; K++) Ke(B[K], k, _, O);
             r(b.anchor, k, _);
             return
         }
         if (U === xl) {
             S(b, k, _);
@@ -2643,26 +2643,26 @@
         let Ne;
         if (pe && (Ne = U && U.onVnodeBeforeUnmount) && Lt(Ne, k, b), Q & 6) M(b.component, _, O);
         else {
             if (Q & 128) {
                 b.suspense.unmount(_, O);
                 return
             }
-            oe && hr(b, null, k, "beforeUnmount"), Q & 64 ? b.type.remove(b, k, _, D, ye, O) : P && (F !== Fe || K > 0 && K & 64) ? j(P, k, _, !1, !0) : (F === Fe && K & 384 || !D && Q & 16) && j(B, k, _), O && wt(b)
+            oe && hr(b, null, k, "beforeUnmount"), Q & 64 ? b.type.remove(b, k, _, D, ye, O) : P && (F !== Le || K > 0 && K & 64) ? j(P, k, _, !1, !0) : (F === Le && K & 384 || !D && Q & 16) && j(B, k, _), O && wt(b)
         }(pe && (Ne = U && U.onVnodeUnmounted) || oe) && rt(() => {
             Ne && Lt(Ne, k, b), oe && hr(b, null, k, "unmounted")
         }, _)
     }, wt = b => {
         const {
             type: k,
             el: _,
             anchor: O,
             transition: D
         } = b;
-        if (k === Fe) {
+        if (k === Le) {
             St(_, O);
             return
         }
         if (k === xl) {
             y(b);
             return
         }
@@ -2707,15 +2707,15 @@
         n: z,
         o: t
     };
     let Ee, ue;
     return e && ([Ee, ue] = e(ye)), {
         render: Y,
         hydrate: Ee,
-        createApp: eb(Y, Ee)
+        createApp: tb(Y, Ee)
     }
 }
 
 function pr({
     effect: t,
     update: e
 }, n) {
@@ -2729,15 +2729,15 @@
         for (let i = 0; i < r.length; i++) {
             const o = r[i];
             let l = s[i];
             l.shapeFlag & 1 && !l.dynamicChildren && ((l.patchFlag <= 0 || l.patchFlag === 32) && (l = s[i] = jn(s[i]), l.el = o.el), n || gc(o, l)), l.type === Bo && (l.el = o.el)
         }
 }
 
-function rb(t) {
+function sb(t) {
     const e = t.slice(),
         n = [0];
     let r, s, i, o, l;
     const a = t.length;
     for (r = 0; r < a; r++) {
         const c = t[r];
         if (c !== 0) {
@@ -2748,22 +2748,22 @@
             for (i = 0, o = n.length - 1; i < o;) l = i + o >> 1, t[n[l]] < c ? i = l + 1 : o = l;
             c < t[n[i]] && (i > 0 && (e[r] = n[i - 1]), n[i] = r)
         }
     }
     for (i = n.length, o = n[i - 1]; i-- > 0;) n[i] = o, o = e[o];
     return n
 }
-const sb = t => t.__isTeleport,
+const ib = t => t.__isTeleport,
     qs = t => t && (t.disabled || t.disabled === ""),
     xu = t => typeof SVGElement < "u" && t instanceof SVGElement,
     ya = (t, e) => {
         const n = t && t.to;
-        return je(n) ? e ? e(n) : null : n
+        return Ue(n) ? e ? e(n) : null : n
     },
-    ib = {
+    ob = {
         __isTeleport: !0,
         process(t, e, n, r, s, i, o, l, a, c) {
             const {
                 mc: u,
                 pc: d,
                 pbc: f,
                 o: {
@@ -2793,19 +2793,19 @@
                 e.el = t.el;
                 const I = e.anchor = t.anchor,
                     T = e.target = t.target,
                     V = e.targetAnchor = t.targetAnchor,
                     N = qs(t.props),
                     G = N ? n : T,
                     J = N ? I : V;
-                if (o = o || xu(T), y ? (f(t.dynamicChildren, y, G, s, i, o, l), gc(t, e, !0)) : a || d(t, e, G, J, s, i, o, l, !1), x) N || Ii(e, n, I, c, 1);
+                if (o = o || xu(T), y ? (f(t.dynamicChildren, y, G, s, i, o, l), gc(t, e, !0)) : a || d(t, e, G, J, s, i, o, l, !1), x) N || $i(e, n, I, c, 1);
                 else if ((e.props && e.props.to) !== (t.props && t.props.to)) {
                     const ne = e.target = ya(e.props, p);
-                    ne && Ii(e, ne, null, c, 0)
-                } else N && Ii(e, T, V, c, 1)
+                    ne && $i(e, ne, null, c, 0)
+                } else N && $i(e, T, V, c, 1)
             }
             Mh(e)
         },
         remove(t, e, n, r, {
             um: s,
             o: {
                 remove: i
@@ -2821,19 +2821,19 @@
             } = t;
             if (d && i(u), (o || !qs(f)) && (i(c), l & 16))
                 for (let h = 0; h < a.length; h++) {
                     const p = a[h];
                     s(p, e, n, !0, !!p.dynamicChildren)
                 }
         },
-        move: Ii,
-        hydrate: ob
+        move: $i,
+        hydrate: lb
     };
 
-function Ii(t, e, n, {
+function $i(t, e, n, {
     o: {
         insert: r
     },
     m: s
 }, i = 2) {
     i === 0 && r(t.targetAnchor, e, n);
     const {
@@ -2844,15 +2844,15 @@
         props: u
     } = t, d = i === 2;
     if (d && r(o, e, n), (!d || qs(u)) && a & 16)
         for (let f = 0; f < c.length; f++) s(c[f], e, n, 2);
     d && r(l, e, n)
 }
 
-function ob(t, e, n, r, s, i, {
+function lb(t, e, n, r, s, i, {
     o: {
         nextSibling: o,
         parentNode: l,
         querySelector: a
     }
 }, c) {
     const u = e.target = ya(e.props, a);
@@ -2868,87 +2868,87 @@
                         e.targetAnchor = f, u._lpa = e.targetAnchor && o(e.targetAnchor);
                         break
                     } c(d, e, u, n, r, s, i)
             } Mh(e)
     }
     return e.anchor && o(e.anchor)
 }
-const lb = ib;
+const ab = ob;
 
 function Mh(t) {
     const e = t.ctx;
     if (e && e.ut) {
         let n = t.children[0].el;
         for (; n !== t.targetAnchor;) n.nodeType === 1 && n.setAttribute("data-v-owner", e.uid), n = n.nextSibling;
         e.ut()
     }
 }
-const Fe = Symbol(void 0),
+const Le = Symbol(void 0),
     Bo = Symbol(void 0),
     tn = Symbol(void 0),
     xl = Symbol(void 0),
     Ks = [];
 let Qt = null;
 
 function C(t = !1) {
     Ks.push(Qt = t ? null : [])
 }
 
-function ab() {
+function cb() {
     Ks.pop(), Qt = Ks[Ks.length - 1] || null
 }
 let ai = 1;
 
 function ku(t) {
     ai += t
 }
 
 function Ah(t) {
-    return t.dynamicChildren = ai > 0 ? Qt || Gr : null, ab(), ai > 0 && Qt && Qt.push(t), t
+    return t.dynamicChildren = ai > 0 ? Qt || Gr : null, cb(), ai > 0 && Qt && Qt.push(t), t
 }
 
 function R(t, e, n, r, s, i) {
     return Ah(m(t, e, n, r, s, i, !0))
 }
 
 function yt(t, e, n, r, s) {
     return Ah(ce(t, e, n, r, s, !0))
 }
 
-function ro(t) {
+function io(t) {
     return t ? t.__v_isVNode === !0 : !1
 }
 
 function qn(t, e) {
     return t.type === e.type && t.key === e.key
 }
 const Ho = "__vInternal",
     Nh = ({
         key: t
     }) => t ?? null,
-    ji = ({
+    Wi = ({
         ref: t,
         ref_key: e,
         ref_for: n
-    }) => t != null ? je(t) || ft(t) || me(t) ? {
+    }) => t != null ? Ue(t) || ft(t) || me(t) ? {
         i: Rt,
         r: t,
         k: e,
         f: !!n
     } : t : null;
 
-function m(t, e = null, n = null, r = 0, s = null, i = t === Fe ? 0 : 1, o = !1, l = !1) {
+function m(t, e = null, n = null, r = 0, s = null, i = t === Le ? 0 : 1, o = !1, l = !1) {
     const a = {
         __v_isVNode: !0,
         __v_skip: !0,
         type: t,
         props: e,
         key: e && Nh(e),
-        ref: e && ji(e),
-        scopeId: Io,
+        ref: e && Wi(e),
+        scopeId: $o,
         slotScopeIds: null,
         children: n,
         component: null,
         suspense: null,
         ssContent: null,
         ssFallback: null,
         dirs: null,
@@ -2961,61 +2961,61 @@
         shapeFlag: i,
         patchFlag: r,
         dynamicProps: s,
         dynamicChildren: null,
         appContext: null,
         ctx: Rt
     };
-    return l ? (yc(a, n), i & 128 && t.normalize(a)) : n && (a.shapeFlag |= je(n) ? 8 : 16), ai > 0 && !o && Qt && (a.patchFlag > 0 || i & 6) && a.patchFlag !== 32 && Qt.push(a), a
+    return l ? (yc(a, n), i & 128 && t.normalize(a)) : n && (a.shapeFlag |= Ue(n) ? 8 : 16), ai > 0 && !o && Qt && (a.patchFlag > 0 || i & 6) && a.patchFlag !== 32 && Qt.push(a), a
 }
-const ce = cb;
+const ce = ub;
 
-function cb(t, e = null, n = null, r = 0, s = null, i = !1) {
-    if ((!t || t === Hy) && (t = tn), ro(t)) {
+function ub(t, e = null, n = null, r = 0, s = null, i = !1) {
+    if ((!t || t === zy) && (t = tn), io(t)) {
         const l = Rn(t, e, !0);
         return n && yc(l, n), ai > 0 && !i && Qt && (l.shapeFlag & 6 ? Qt[Qt.indexOf(t)] = l : Qt.push(l)), l.patchFlag |= -2, l
     }
-    if (vb(t) && (t = t.__vccOpts), e) {
-        e = ub(e);
+    if (xb(t) && (t = t.__vccOpts), e) {
+        e = db(e);
         let {
             class: l,
             style: a
         } = e;
-        l && !je(l) && (e.class = he(l)), Ie(a) && (rh(a) && !te(a) && (a = lt({}, a)), e.style = _o(a))
+        l && !Ue(l) && (e.class = fe(l)), Ie(a) && (rh(a) && !te(a) && (a = lt({}, a)), e.style = Eo(a))
     }
-    const o = je(t) ? 1 : hh(t) ? 128 : sb(t) ? 64 : Ie(t) ? 4 : me(t) ? 2 : 0;
+    const o = Ue(t) ? 1 : hh(t) ? 128 : ib(t) ? 64 : Ie(t) ? 4 : me(t) ? 2 : 0;
     return m(t, e, n, r, s, o, i, !0)
 }
 
-function ub(t) {
+function db(t) {
     return t ? rh(t) || Ho in t ? lt({}, t) : t : null
 }
 
 function Rn(t, e, n = !1) {
     const {
         props: r,
         ref: s,
         patchFlag: i,
         children: o
-    } = t, l = e ? db(r || {}, e) : r;
+    } = t, l = e ? fb(r || {}, e) : r;
     return {
         __v_isVNode: !0,
         __v_skip: !0,
         type: t.type,
         props: l,
         key: l && Nh(l),
-        ref: e && e.ref ? n && s ? te(s) ? s.concat(ji(e)) : [s, ji(e)] : ji(e) : s,
+        ref: e && e.ref ? n && s ? te(s) ? s.concat(Wi(e)) : [s, Wi(e)] : Wi(e) : s,
         scopeId: t.scopeId,
         slotScopeIds: t.slotScopeIds,
         children: o,
         target: t.target,
         targetAnchor: t.targetAnchor,
         staticCount: t.staticCount,
         shapeFlag: t.shapeFlag,
-        patchFlag: e && t.type !== Fe ? i === -1 ? 16 : i | 16 : i,
+        patchFlag: e && t.type !== Le ? i === -1 ? 16 : i | 16 : i,
         dynamicProps: t.dynamicProps,
         dynamicChildren: t.dynamicChildren,
         appContext: t.appContext,
         dirs: t.dirs,
         transition: t.transition,
         component: t.component,
         suspense: t.suspense,
@@ -3033,15 +3033,15 @@
 }
 
 function re(t = "", e = !1) {
     return e ? (C(), yt(tn, null, t)) : ce(tn, null, t)
 }
 
 function an(t) {
-    return t == null || typeof t == "boolean" ? ce(tn) : te(t) ? ce(Fe, null, t.slice()) : typeof t == "object" ? jn(t) : ce(Bo, null, String(t))
+    return t == null || typeof t == "boolean" ? ce(tn) : te(t) ? ce(Le, null, t.slice()) : typeof t == "object" ? jn(t) : ce(Bo, null, String(t))
 }
 
 function jn(t) {
     return t.el === null && t.patchFlag !== -1 || t.memo ? t : Rn(t)
 }
 
 function yc(t, e) {
@@ -3064,51 +3064,51 @@
     else me(e) ? (e = {
         default: e,
         _ctx: Rt
     }, n = 32) : (e = String(e), r & 64 ? (n = 16, e = [Ge(e)]) : n = 8);
     t.children = e, t.shapeFlag |= n
 }
 
-function db(...t) {
+function fb(...t) {
     const e = {};
     for (let n = 0; n < t.length; n++) {
         const r = t[n];
         for (const s in r)
-            if (s === "class") e.class !== r.class && (e.class = he([e.class, r.class]));
-            else if (s === "style") e.style = _o([e.style, r.style]);
-        else if (Eo(s)) {
+            if (s === "class") e.class !== r.class && (e.class = fe([e.class, r.class]));
+            else if (s === "style") e.style = Eo([e.style, r.style]);
+        else if (Oo(s)) {
             const i = e[s],
                 o = r[s];
             o && i !== o && !(te(i) && i.includes(o)) && (e[s] = i ? [].concat(i, o) : o)
         } else s !== "" && (e[s] = r[s])
     }
     return e
 }
 
 function Lt(t, e, n, r = null) {
     Vt(t, e, 7, [n, r])
 }
-const fb = Oh();
-let hb = 0;
+const hb = Oh();
+let pb = 0;
 
-function pb(t, e, n) {
+function mb(t, e, n) {
     const r = t.type,
-        s = (e ? e.appContext : t.appContext) || fb,
+        s = (e ? e.appContext : t.appContext) || hb,
         i = {
-            uid: hb++,
+            uid: pb++,
             vnode: t,
             type: r,
             parent: e,
             appContext: s,
             root: null,
             next: null,
             subTree: null,
             effect: null,
             update: null,
-            scope: new Rg(!0),
+            scope: new Dg(!0),
             render: null,
             proxy: null,
             exposed: null,
             exposeProxy: null,
             withProxy: null,
             provides: e ? e.provides : Object.create(s.provides),
             accessCache: null,
@@ -3149,15 +3149,15 @@
             rtg: null,
             rtc: null,
             ec: null,
             sp: null
         };
     return i.ctx = {
         _: i
-    }, i.root = e ? e.root : i, i.emit = vy.bind(null, i), t.ce && t.ce(i), i
+    }, i.root = e ? e.root : i, i.emit = xy.bind(null, i), t.ce && t.ce(i), i
 }
 let qe = null;
 const bc = () => qe || Rt,
     is = t => {
         qe = t, t.scope.on()
     },
     Or = () => {
@@ -3165,40 +3165,40 @@
     };
 
 function Rh(t) {
     return t.vnode.shapeFlag & 4
 }
 let ci = !1;
 
-function mb(t, e = !1) {
+function gb(t, e = !1) {
     ci = e;
     const {
         props: n,
         children: r
     } = t.vnode, s = Rh(t);
-    Jy(t, n, s, e), Xy(t, r);
-    const i = s ? gb(t, e) : void 0;
+    Gy(t, n, s, e), Qy(t, r);
+    const i = s ? yb(t, e) : void 0;
     return ci = !1, i
 }
 
-function gb(t, e) {
+function yb(t, e) {
     const n = t.type;
-    t.accessCache = Object.create(null), t.proxy = oc(new Proxy(t.ctx, Vy));
+    t.accessCache = Object.create(null), t.proxy = oc(new Proxy(t.ctx, jy));
     const {
         setup: r
     } = n;
     if (r) {
-        const s = t.setupContext = r.length > 1 ? bb(t) : null;
+        const s = t.setupContext = r.length > 1 ? vb(t) : null;
         is(t), _s();
         const i = Qn(r, t, 0, [t.props, s]);
         if (Cs(), Or(), jf(i)) {
             if (i.then(Or, Or), e) return i.then(o => {
                 wu(t, o, e)
             }).catch(o => {
-                Ro(o, t, 0)
+                Io(o, t, 0)
             });
             t.asyncDep = i
         } else wu(t, i, e)
     } else Dh(t, e)
 }
 
 function wu(t, e, n) {
@@ -3223,33 +3223,33 @@
                     delimiters: l
                 }, o), a);
                 r.render = Su(s, c)
             }
         }
         t.render = r.render || en
     }
-    is(t), _s(), jy(t), Cs(), Or()
+    is(t), _s(), Uy(t), Cs(), Or()
 }
 
-function yb(t) {
+function bb(t) {
     return new Proxy(t.attrs, {
         get(e, n) {
             return Tt(t, "get", "$attrs"), e[n]
         }
     })
 }
 
-function bb(t) {
+function vb(t) {
     const e = r => {
         t.exposed = r || {}
     };
     let n;
     return {
         get attrs() {
-            return n || (n = yb(t))
+            return n || (n = bb(t))
         },
         slots: t.slots,
         emit: t.emit,
         expose: e
     }
 }
 
@@ -3265,39 +3265,39 @@
     }))
 }
 
 function ba(t, e = !0) {
     return me(t) ? t.displayName || t.name : t.name || e && t.__name
 }
 
-function vb(t) {
+function xb(t) {
     return me(t) && "__vccOpts" in t
 }
-const Bt = (t, e) => hy(t, e, ci);
+const Bt = (t, e) => py(t, e, ci);
 
 function mn(t, e, n) {
     const r = arguments.length;
-    return r === 2 ? Ie(e) && !te(e) ? ro(e) ? ce(t, null, [e]) : ce(t, e) : ce(t, null, e) : (r > 3 ? n = Array.prototype.slice.call(arguments, 2) : r === 3 && ro(n) && (n = [n]), ce(t, e, n))
+    return r === 2 ? Ie(e) && !te(e) ? io(e) ? ce(t, null, [e]) : ce(t, e) : ce(t, null, e) : (r > 3 ? n = Array.prototype.slice.call(arguments, 2) : r === 3 && io(n) && (n = [n]), ce(t, e, n))
 }
-const xb = Symbol(""),
-    kb = () => On(xb),
-    wb = "3.2.47",
-    Sb = "http://www.w3.org/2000/svg",
+const kb = Symbol(""),
+    wb = () => On(kb),
+    Sb = "3.2.47",
+    _b = "http://www.w3.org/2000/svg",
     xr = typeof document < "u" ? document : null,
     _u = xr && xr.createElement("template"),
-    _b = {
+    Cb = {
         insert: (t, e, n) => {
             e.insertBefore(t, n || null)
         },
         remove: t => {
             const e = t.parentNode;
             e && e.removeChild(t)
         },
         createElement: (t, e, n, r) => {
-            const s = e ? xr.createElementNS(Sb, t) : xr.createElement(t, n ? {
+            const s = e ? xr.createElementNS(_b, t) : xr.createElement(t, n ? {
                 is: n
             } : void 0);
             return t === "select" && r && r.multiple != null && s.setAttribute("multiple", r.multiple), s
         },
         createText: t => xr.createTextNode(t),
         createComment: t => xr.createComment(t),
         setText: (t, e) => {
@@ -3326,67 +3326,67 @@
                 }
                 e.insertBefore(l, n)
             }
             return [o ? o.nextSibling : e.firstChild, n ? n.previousSibling : e.lastChild]
         }
     };
 
-function Cb(t, e, n) {
+function Eb(t, e, n) {
     const r = t._vtc;
     r && (e = (e ? [e, ...r] : [...r]).join(" ")), e == null ? t.removeAttribute("class") : n ? t.setAttribute("class", e) : t.className = e
 }
 
-function Eb(t, e, n) {
+function Tb(t, e, n) {
     const r = t.style,
-        s = je(n);
+        s = Ue(n);
     if (n && !s) {
-        if (e && !je(e))
+        if (e && !Ue(e))
             for (const i in e) n[i] == null && va(r, i, "");
         for (const i in n) va(r, i, n[i])
     } else {
         const i = r.display;
         s ? e !== n && (r.cssText = n) : e && t.removeAttribute("style"), "_vod" in t && (r.display = i)
     }
 }
 const Cu = /\s*!important$/;
 
 function va(t, e, n) {
     if (te(n)) n.forEach(r => va(t, e, r));
     else if (n == null && (n = ""), e.startsWith("--")) t.setProperty(e, n);
     else {
-        const r = Tb(t, e);
+        const r = Ob(t, e);
         Cu.test(n) ? t.setProperty(Ss(r), n.replace(Cu, ""), "important") : t[r] = n
     }
 }
 const Eu = ["Webkit", "Moz", "ms"],
     kl = {};
 
-function Tb(t, e) {
+function Ob(t, e) {
     const n = kl[e];
     if (n) return n;
     let r = yn(e);
     if (r !== "filter" && r in t) return kl[e] = r;
-    r = Mo(r);
+    r = No(r);
     for (let s = 0; s < Eu.length; s++) {
         const i = Eu[s] + r;
         if (i in t) return kl[e] = i
     }
     return e
 }
 const Tu = "http://www.w3.org/1999/xlink";
 
-function Ob(t, e, n, r, s) {
+function Mb(t, e, n, r, s) {
     if (r && e.startsWith("xlink:")) n == null ? t.removeAttributeNS(Tu, e.slice(6, e.length)) : t.setAttributeNS(Tu, e, n);
     else {
-        const i = kg(e);
+        const i = wg(e);
         n == null || i && !Hf(n) ? t.removeAttribute(e) : t.setAttribute(e, i ? "" : n)
     }
 }
 
-function Mb(t, e, n, r, s, i, o) {
+function Ab(t, e, n, r, s, i, o) {
     if (e === "innerHTML" || e === "textContent") {
         r && o(r, s, i), t[e] = n ?? "";
         return
     }
     if (e === "value" && t.tagName !== "PROGRESS" && !t.tagName.includes("-")) {
         t._value = n;
         const a = n ?? "";
@@ -3404,75 +3404,75 @@
     l && t.removeAttribute(e)
 }
 
 function kr(t, e, n, r) {
     t.addEventListener(e, n, r)
 }
 
-function Ab(t, e, n, r) {
+function Nb(t, e, n, r) {
     t.removeEventListener(e, n, r)
 }
 
-function Nb(t, e, n, r, s = null) {
+function Rb(t, e, n, r, s = null) {
     const i = t._vei || (t._vei = {}),
         o = i[e];
     if (r && o) o.value = r;
     else {
-        const [l, a] = Rb(e);
+        const [l, a] = Db(e);
         if (r) {
-            const c = i[e] = Pb(r, s);
+            const c = i[e] = $b(r, s);
             kr(t, l, c, a)
-        } else o && (Ab(t, l, o, a), i[e] = void 0)
+        } else o && (Nb(t, l, o, a), i[e] = void 0)
     }
 }
 const Ou = /(?:Once|Passive|Capture)$/;
 
-function Rb(t) {
+function Db(t) {
     let e;
     if (Ou.test(t)) {
         e = {};
         let r;
         for (; r = t.match(Ou);) t = t.slice(0, t.length - r[0].length), e[r[0].toLowerCase()] = !0
     }
     return [t[2] === ":" ? t.slice(3) : Ss(t.slice(2)), e]
 }
 let wl = 0;
-const Db = Promise.resolve(),
-    Ib = () => wl || (Db.then(() => wl = 0), wl = Date.now());
+const Ib = Promise.resolve(),
+    Pb = () => wl || (Ib.then(() => wl = 0), wl = Date.now());
 
-function Pb(t, e) {
+function $b(t, e) {
     const n = r => {
         if (!r._vts) r._vts = Date.now();
         else if (r._vts <= n.attached) return;
-        Vt($b(r, n.value), e, 5, [r])
+        Vt(Lb(r, n.value), e, 5, [r])
     };
-    return n.value = t, n.attached = Ib(), n
+    return n.value = t, n.attached = Pb(), n
 }
 
-function $b(t, e) {
+function Lb(t, e) {
     if (te(e)) {
         const n = t.stopImmediatePropagation;
         return t.stopImmediatePropagation = () => {
             n.call(t), t._stopped = !0
         }, e.map(r => s => !s._stopped && r && r(s))
     } else return e
 }
 const Mu = /^on[a-z]/,
-    Lb = (t, e, n, r, s = !1, i, o, l, a) => {
-        e === "class" ? Cb(t, r, s) : e === "style" ? Eb(t, n, r) : Eo(e) ? Xa(e) || Nb(t, e, n, r, o) : (e[0] === "." ? (e = e.slice(1), !0) : e[0] === "^" ? (e = e.slice(1), !1) : Fb(t, e, r, s)) ? Mb(t, e, r, i, o, l, a) : (e === "true-value" ? t._trueValue = r : e === "false-value" && (t._falseValue = r), Ob(t, e, r, s))
+    Fb = (t, e, n, r, s = !1, i, o, l, a) => {
+        e === "class" ? Eb(t, r, s) : e === "style" ? Tb(t, n, r) : Oo(e) ? Xa(e) || Rb(t, e, n, r, o) : (e[0] === "." ? (e = e.slice(1), !0) : e[0] === "^" ? (e = e.slice(1), !1) : Bb(t, e, r, s)) ? Ab(t, e, r, i, o, l, a) : (e === "true-value" ? t._trueValue = r : e === "false-value" && (t._falseValue = r), Mb(t, e, r, s))
     };
 
-function Fb(t, e, n, r) {
-    return r ? !!(e === "innerHTML" || e === "textContent" || e in t && Mu.test(e) && me(n)) : e === "spellcheck" || e === "draggable" || e === "translate" || e === "form" || e === "list" && t.tagName === "INPUT" || e === "type" && t.tagName === "TEXTAREA" || Mu.test(e) && je(n) ? !1 : e in t
+function Bb(t, e, n, r) {
+    return r ? !!(e === "innerHTML" || e === "textContent" || e in t && Mu.test(e) && me(n)) : e === "spellcheck" || e === "draggable" || e === "translate" || e === "form" || e === "list" && t.tagName === "INPUT" || e === "type" && t.tagName === "TEXTAREA" || Mu.test(e) && Ue(n) ? !1 : e in t
 }
 const Ln = "transition",
     Ns = "animation",
     rn = (t, {
         slots: e
-    }) => mn(mh, Bb(t), e);
+    }) => mn(mh, Hb(t), e);
 rn.displayName = "Transition";
 const Ih = {
     name: String,
     type: String,
     css: {
         type: Boolean,
         default: !0
@@ -3490,15 +3490,15 @@
 };
 rn.props = lt({}, mh.props, Ih);
 const mr = (t, e = []) => {
         te(t) ? t.forEach(n => n(...e)) : t && t(...e)
     },
     Au = t => t ? te(t) ? t.some(e => e.length > 1) : t.length > 1 : !1;
 
-function Bb(t) {
+function Hb(t) {
     const e = {};
     for (const H in t) H in Ih || (e[H] = t[H]);
     if (t.css === !1) return e;
     const {
         name: n = "v",
         type: r,
         duration: s,
@@ -3507,47 +3507,47 @@
         enterToClass: l = `${n}-enter-to`,
         appearFromClass: a = i,
         appearActiveClass: c = o,
         appearToClass: u = l,
         leaveFromClass: d = `${n}-leave-from`,
         leaveActiveClass: f = `${n}-leave-active`,
         leaveToClass: h = `${n}-leave-to`
-    } = t, p = Hb(s), g = p && p[0], v = p && p[1], {
+    } = t, p = zb(s), g = p && p[0], v = p && p[1], {
         onBeforeEnter: x,
         onEnter: w,
         onEnterCancelled: S,
         onLeave: y,
         onLeaveCancelled: I,
         onBeforeAppear: T = x,
         onAppear: V = w,
         onAppearCancelled: N = S
     } = e, G = (H, ie, Ae) => {
         gr(H, ie ? u : l), gr(H, ie ? c : o), Ae && Ae()
     }, J = (H, ie) => {
         H._isLeaving = !1, gr(H, d), gr(H, h), gr(H, f), ie && ie()
     }, ne = H => (ie, Ae) => {
-        const Be = H ? V : w,
+        const He = H ? V : w,
             ge = () => G(ie, H, Ae);
-        mr(Be, [ie, ge]), Nu(() => {
-            gr(ie, H ? a : i), Fn(ie, H ? u : l), Au(Be) || Ru(ie, r, g, ge)
+        mr(He, [ie, ge]), Nu(() => {
+            gr(ie, H ? a : i), Fn(ie, H ? u : l), Au(He) || Ru(ie, r, g, ge)
         })
     };
     return lt(e, {
         onBeforeEnter(H) {
             mr(x, [H]), Fn(H, i), Fn(H, o)
         },
         onBeforeAppear(H) {
             mr(T, [H]), Fn(H, a), Fn(H, c)
         },
         onEnter: ne(!1),
         onAppear: ne(!0),
         onLeave(H, ie) {
             H._isLeaving = !0;
             const Ae = () => J(H, ie);
-            Fn(H, d), jb(), Fn(H, f), Nu(() => {
+            Fn(H, d), Ub(), Fn(H, f), Nu(() => {
                 H._isLeaving && (gr(H, d), Fn(H, h), Au(y) || Ru(H, r, v, Ae))
             }), mr(y, [H, Ae])
         },
         onEnterCancelled(H) {
             G(H, !1), mr(S, [H])
         },
         onAppearCancelled(H) {
@@ -3555,24 +3555,24 @@
         },
         onLeaveCancelled(H) {
             J(H), mr(I, [H])
         }
     })
 }
 
-function Hb(t) {
+function zb(t) {
     if (t == null) return null;
     if (Ie(t)) return [Sl(t.enter), Sl(t.leave)]; {
         const e = Sl(t);
         return [e, e]
     }
 }
 
 function Sl(t) {
-    return Ag(t)
+    return Ng(t)
 }
 
 function Fn(t, e) {
     e.split(/\s+/).forEach(n => n && t.classList.add(n)), (t._vtc || (t._vtc = new Set)).add(e)
 }
 
 function gr(t, e) {
@@ -3584,42 +3584,42 @@
 }
 
 function Nu(t) {
     requestAnimationFrame(() => {
         requestAnimationFrame(t)
     })
 }
-let zb = 0;
+let Vb = 0;
 
 function Ru(t, e, n, r) {
-    const s = t._endId = ++zb,
+    const s = t._endId = ++Vb,
         i = () => {
             s === t._endId && r()
         };
     if (n) return setTimeout(i, n);
     const {
         type: o,
         timeout: l,
         propCount: a
-    } = Vb(t, e);
+    } = jb(t, e);
     if (!o) return r();
     const c = o + "end";
     let u = 0;
     const d = () => {
             t.removeEventListener(c, f), i()
         },
         f = h => {
             h.target === t && ++u >= a && d()
         };
     setTimeout(() => {
         u < a && d()
     }, l + 1), t.addEventListener(c, f)
 }
 
-function Vb(t, e) {
+function jb(t, e) {
     const n = window.getComputedStyle(t),
         r = p => (n[p] || "").split(", "),
         s = r(`${Ln}Delay`),
         i = r(`${Ln}Duration`),
         o = Du(s, i),
         l = r(`${Ns}Delay`),
         a = r(`${Ns}Duration`),
@@ -3642,23 +3642,23 @@
     return Math.max(...e.map((n, r) => Iu(n) + Iu(t[r])))
 }
 
 function Iu(t) {
     return Number(t.slice(0, -1).replace(",", ".")) * 1e3
 }
 
-function jb() {
+function Ub() {
     return document.body.offsetHeight
 }
-const so = t => {
+const oo = t => {
     const e = t.props["onUpdate:modelValue"] || !1;
     return te(e) ? n => Xr(e, n) : e
 };
 
-function Ub(t) {
+function Wb(t) {
     t.target.composing = !0
 }
 
 function Pu(t) {
     const e = t.target;
     e.composing && (e.composing = !1, e.dispatchEvent(new Event("input")))
 }
@@ -3666,78 +3666,78 @@
         created(t, {
             modifiers: {
                 lazy: e,
                 trim: n,
                 number: r
             }
         }, s) {
-            t._assign = so(s);
+            t._assign = oo(s);
             const i = r || s.props && s.props.type === "number";
             kr(t, e ? "change" : "input", o => {
                 if (o.target.composing) return;
                 let l = t.value;
                 n && (l = l.trim()), i && (l = ia(l)), t._assign(l)
             }), n && kr(t, "change", () => {
                 t.value = t.value.trim()
-            }), e || (kr(t, "compositionstart", Ub), kr(t, "compositionend", Pu), kr(t, "change", Pu))
+            }), e || (kr(t, "compositionstart", Wb), kr(t, "compositionend", Pu), kr(t, "change", Pu))
         },
         mounted(t, {
             value: e
         }) {
             t.value = e ?? ""
         },
         beforeUpdate(t, {
             value: e,
             modifiers: {
                 lazy: n,
                 trim: r,
                 number: s
             }
         }, i) {
-            if (t._assign = so(i), t.composing || document.activeElement === t && t.type !== "range" && (n || r && t.value.trim() === e || (s || t.type === "number") && ia(t.value) === e)) return;
+            if (t._assign = oo(i), t.composing || document.activeElement === t && t.type !== "range" && (n || r && t.value.trim() === e || (s || t.type === "number") && ia(t.value) === e)) return;
             const o = e ?? "";
             t.value !== o && (t.value = o)
         }
     },
-    Wb = {
+    qb = {
         deep: !0,
         created(t, e, n) {
-            t._assign = so(n), kr(t, "change", () => {
+            t._assign = oo(n), kr(t, "change", () => {
                 const r = t._modelValue,
-                    s = qb(t),
+                    s = Kb(t),
                     i = t.checked,
                     o = t._assign;
                 if (te(r)) {
                     const l = zf(r, s),
                         a = l !== -1;
                     if (i && !a) o(r.concat(s));
                     else if (!i && a) {
                         const c = [...r];
                         c.splice(l, 1), o(c)
                     }
-                } else if (To(r)) {
+                } else if (Mo(r)) {
                     const l = new Set(r);
                     i ? l.add(s) : l.delete(s), o(l)
                 } else o(Ph(t, i))
             })
         },
         mounted: $u,
         beforeUpdate(t, e, n) {
-            t._assign = so(n), $u(t, e, n)
+            t._assign = oo(n), $u(t, e, n)
         }
     };
 
 function $u(t, {
     value: e,
     oldValue: n
 }, r) {
-    t._modelValue = e, te(e) ? t.checked = zf(e, r.props.value) > -1 : To(e) ? t.checked = e.has(r.props.value) : e !== n && (t.checked = Co(e, Ph(t, !0)))
+    t._modelValue = e, te(e) ? t.checked = zf(e, r.props.value) > -1 : Mo(e) ? t.checked = e.has(r.props.value) : e !== n && (t.checked = To(e, Ph(t, !0)))
 }
 
-function qb(t) {
+function Kb(t) {
     return "_value" in t ? t._value : t.value
 }
 
 function Ph(t, e) {
     const n = e ? "_trueValue" : "_falseValue";
     return n in t ? t[n] : e
 }
@@ -3772,225 +3772,228 @@
         Rs(t, e)
     }
 };
 
 function Rs(t, e) {
     t.style.display = e ? t._vod : "none"
 }
-const Kb = lt({
-    patchProp: Lb
-}, _b);
+const Jb = lt({
+    patchProp: Fb
+}, Cb);
 let Lu;
 
-function Jb() {
-    return Lu || (Lu = tb(Kb))
+function Gb() {
+    return Lu || (Lu = nb(Jb))
 }
-const Gb = (...t) => {
-    const e = Jb().createApp(...t),
+const Yb = (...t) => {
+    const e = Gb().createApp(...t),
         {
             mount: n
         } = e;
     return e.mount = r => {
-        const s = Yb(r);
+        const s = Xb(r);
         if (!s) return;
         const i = e._component;
         !me(i) && !i.render && !i.template && (i.template = s.innerHTML), s.innerHTML = "";
         const o = n(s, !1, s instanceof SVGElement);
         return s instanceof Element && (s.removeAttribute("v-cloak"), s.setAttribute("data-v-app", "")), o
     }, e
 };
 
-function Yb(t) {
-    return je(t) ? document.querySelector(t) : t
+function Xb(t) {
+    return Ue(t) ? document.querySelector(t) : t
 }
-const Xb = "/assets/favicon-464b3816.png",
-    Ue = (t, e) => {
+const Qb = "/assets/favicon-464b3816.png",
+    Be = (t, e) => {
         const n = t.__vccOpts || t;
         for (const [r, s] of e) n[r] = s;
         return n
     },
-    Qb = {},
-    Zb = {
+    Zb = {},
+    e0 = {
         class: "navbar is-primary",
         role: "navigation",
         "aria-label": "main navigation"
     },
-    e0 = {
+    t0 = {
+        class: "container"
+    },
+    n0 = {
         class: "navbar-brand"
     },
-    t0 = m("img", {
-        src: Xb,
+    r0 = m("img", {
+        src: Qb,
         alt: "Logo"
     }, null, -1),
-    n0 = m("span", {
+    s0 = m("span", {
         class: "ml-2"
     }, [m("strong", null, "CHEF")], -1),
-    r0 = {
+    i0 = {
         class: "navbar-end"
     },
-    s0 = {
+    o0 = {
         class: "navbar-item"
     },
-    i0 = {
+    l0 = {
         class: "buttons"
     },
-    o0 = m("span", {
+    a0 = m("span", {
         class: "icon is-small"
     }, [m("i", {
         class: "fas fa-list"
     })], -1),
-    l0 = m("strong", null, "All", -1),
-    a0 = m("strong", null, "Add Category", -1),
-    c0 = m("span", {
+    c0 = m("strong", null, "All", -1),
+    u0 = m("strong", null, "Add Category", -1),
+    d0 = m("span", {
         class: "icon is-small"
     }, [m("i", {
         class: "fas fa-plus"
     })], -1),
-    u0 = m("span", null, "Recipe", -1);
+    f0 = m("span", null, "Recipe", -1);
 
-function d0(t, e) {
+function h0(t, e) {
     const n = Oe("router-link");
-    return C(), R("div", null, [m("nav", Zb, [m("div", e0, [ce(n, {
+    return C(), R("div", null, [m("nav", e0, [m("div", t0, [m("div", n0, [ce(n, {
         to: {
             name: "home"
         },
         class: "navbar-item"
     }, {
-        default: ht(() => [t0, n0]),
+        default: ht(() => [r0, s0]),
         _: 1
-    })]), m("div", r0, [m("div", s0, [m("div", i0, [ce(n, {
+    })]), m("div", i0, [m("div", o0, [m("div", l0, [ce(n, {
         to: {
             name: "recipes"
         },
         class: "button is-primary mx-0"
     }, {
-        default: ht(() => [o0, l0]),
+        default: ht(() => [a0, c0]),
         _: 1
     }), ce(n, {
         to: {
             name: "newcategory"
         },
         class: "button is-primary mx-0 pl-0"
     }, {
-        default: ht(() => [a0]),
+        default: ht(() => [u0]),
         _: 1
     }), ce(n, {
         to: {
             name: "new"
         },
         class: "button is-light"
     }, {
-        default: ht(() => [c0, u0]),
+        default: ht(() => [d0, f0]),
         _: 1
-    })])])])])])
+    })])])])])])])
 }
-const f0 = Ue(Qb, [
-    ["render", d0]
+const p0 = Be(Zb, [
+    ["render", h0]
 ]);
-const h0 = {
+const m0 = {
         components: {
-            Navbar: f0
+            Navbar: p0
         }
     },
-    p0 = {
+    g0 = {
         id: "app"
     },
-    m0 = {
-        class: "container pb-4"
+    y0 = {
+        class: "container pb-4 px-1"
     };
 
-function g0(t, e, n, r, s, i) {
+function b0(t, e, n, r, s, i) {
     const o = Oe("Navbar"),
         l = Oe("router-view");
-    return C(), R("div", p0, [ce(o, {
+    return C(), R("div", g0, [ce(o, {
         class: "mb-2"
-    }), m("div", m0, [ce(rn, {
+    }), m("div", y0, [ce(rn, {
         mode: "out-in"
     }, {
-        default: ht(() => [(C(), yt(Ay, null, [ce(l)], 1024))]),
+        default: ht(() => [(C(), yt(Ny, null, [ce(l)], 1024))]),
         _: 1
     })])])
 }
-const y0 = Ue(h0, [
-    ["render", g0]
+const v0 = Be(m0, [
+    ["render", b0]
 ]);
 /*!
  * vue-router v4.1.6
  * (c) 2022 Eduardo San Martin Morote
  * @license MIT
  */
 const jr = typeof window < "u";
 
-function b0(t) {
+function x0(t) {
     return t.__esModule || t[Symbol.toStringTag] === "Module"
 }
 const Re = Object.assign;
 
 function Cl(t, e) {
     const n = {};
     for (const r in e) {
         const s = e[r];
         n[r] = sn(s) ? s.map(t) : t(s)
     }
     return n
 }
 const Js = () => {},
     sn = Array.isArray,
-    v0 = /\/$/,
-    x0 = t => t.replace(v0, "");
+    k0 = /\/$/,
+    w0 = t => t.replace(k0, "");
 
 function El(t, e, n = "/") {
     let r, s = {},
         i = "",
         o = "";
     const l = e.indexOf("#");
     let a = e.indexOf("?");
-    return l < a && l >= 0 && (a = -1), a > -1 && (r = e.slice(0, a), i = e.slice(a + 1, l > -1 ? l : e.length), s = t(i)), l > -1 && (r = r || e.slice(0, l), o = e.slice(l, e.length)), r = _0(r ?? e, n), {
+    return l < a && l >= 0 && (a = -1), a > -1 && (r = e.slice(0, a), i = e.slice(a + 1, l > -1 ? l : e.length), s = t(i)), l > -1 && (r = r || e.slice(0, l), o = e.slice(l, e.length)), r = E0(r ?? e, n), {
         fullPath: r + (i && "?") + i + o,
         path: r,
         query: s,
         hash: o
     }
 }
 
-function k0(t, e) {
+function S0(t, e) {
     const n = e.query ? t(e.query) : "";
     return e.path + (n && "?") + n + (e.hash || "")
 }
 
 function Fu(t, e) {
     return !e || !t.toLowerCase().startsWith(e.toLowerCase()) ? t : t.slice(e.length) || "/"
 }
 
-function w0(t, e, n) {
+function _0(t, e, n) {
     const r = e.matched.length - 1,
         s = n.matched.length - 1;
     return r > -1 && r === s && ls(e.matched[r], n.matched[s]) && $h(e.params, n.params) && t(e.query) === t(n.query) && e.hash === n.hash
 }
 
 function ls(t, e) {
     return (t.aliasOf || t) === (e.aliasOf || e)
 }
 
 function $h(t, e) {
     if (Object.keys(t).length !== Object.keys(e).length) return !1;
     for (const n in t)
-        if (!S0(t[n], e[n])) return !1;
+        if (!C0(t[n], e[n])) return !1;
     return !0
 }
 
-function S0(t, e) {
+function C0(t, e) {
     return sn(t) ? Bu(t, e) : sn(e) ? Bu(e, t) : t === e
 }
 
 function Bu(t, e) {
     return sn(e) ? t.length === e.length && t.every((n, r) => n === e[r]) : t.length === 1 && t[0] === e
 }
 
-function _0(t, e) {
+function E0(t, e) {
     if (t.startsWith("/")) return t;
     if (!t) return e;
     const n = e.split("/"),
         r = t.split("/");
     let s = n.length - 1,
         i, o;
     for (i = 0; i < r.length; i++)
@@ -4004,68 +4007,68 @@
     t.pop = "pop", t.push = "push"
 })(ui || (ui = {}));
 var Gs;
 (function(t) {
     t.back = "back", t.forward = "forward", t.unknown = ""
 })(Gs || (Gs = {}));
 
-function C0(t) {
+function T0(t) {
     if (!t)
         if (jr) {
             const e = document.querySelector("base");
             t = e && e.getAttribute("href") || "/", t = t.replace(/^\w+:\/\/[^\/]+/, "")
         } else t = "/";
-    return t[0] !== "/" && t[0] !== "#" && (t = "/" + t), x0(t)
+    return t[0] !== "/" && t[0] !== "#" && (t = "/" + t), w0(t)
 }
-const E0 = /^[^#]+#/;
+const O0 = /^[^#]+#/;
 
-function T0(t, e) {
-    return t.replace(E0, "#") + e
+function M0(t, e) {
+    return t.replace(O0, "#") + e
 }
 
-function O0(t, e) {
+function A0(t, e) {
     const n = document.documentElement.getBoundingClientRect(),
         r = t.getBoundingClientRect();
     return {
         behavior: e.behavior,
         left: r.left - n.left - (e.left || 0),
         top: r.top - n.top - (e.top || 0)
     }
 }
 const Vo = () => ({
     left: window.pageXOffset,
     top: window.pageYOffset
 });
 
-function M0(t) {
+function N0(t) {
     let e;
     if ("el" in t) {
         const n = t.el,
             r = typeof n == "string" && n.startsWith("#"),
             s = typeof n == "string" ? r ? document.getElementById(n.slice(1)) : document.querySelector(n) : n;
         if (!s) return;
-        e = O0(s, t)
+        e = A0(s, t)
     } else e = t;
     "scrollBehavior" in document.documentElement.style ? window.scrollTo(e) : window.scrollTo(e.left != null ? e.left : window.pageXOffset, e.top != null ? e.top : window.pageYOffset)
 }
 
 function Hu(t, e) {
     return (history.state ? history.state.position - e : -1) + t
 }
 const xa = new Map;
 
-function A0(t, e) {
+function R0(t, e) {
     xa.set(t, e)
 }
 
-function N0(t) {
+function D0(t) {
     const e = xa.get(t);
     return xa.delete(t), e
 }
-let R0 = () => location.protocol + "//" + location.host;
+let I0 = () => location.protocol + "//" + location.host;
 
 function Lh(t, e) {
     const {
         pathname: n,
         search: r,
         hash: s
     } = e, i = t.indexOf("#");
@@ -4073,15 +4076,15 @@
         let l = s.includes(t.slice(i)) ? t.slice(i).length : 1,
             a = s.slice(l);
         return a[0] !== "/" && (a = "/" + a), Fu(a, "")
     }
     return Fu(n, t) + r + s
 }
 
-function D0(t, e, n, r) {
+function P0(t, e, n, r) {
     let s = [],
         i = [],
         o = null;
     const l = ({
         state: f
     }) => {
         const h = Lh(t, location),
@@ -4144,15 +4147,15 @@
         forward: n,
         replaced: r,
         position: window.history.length,
         scroll: s ? Vo() : null
     }
 }
 
-function I0(t) {
+function $0(t) {
     const {
         history: e,
         location: n
     } = window, r = {
         value: Lh(t, n)
     }, s = {
         value: e.state
@@ -4164,15 +4167,15 @@
         position: e.length - 1,
         replaced: !0,
         scroll: null
     }, !0);
 
     function i(a, c, u) {
         const d = t.indexOf("#"),
-            f = d > -1 ? (n.host && document.querySelector("base") ? t : t.slice(d)) + a : R0() + t + a;
+            f = d > -1 ? (n.host && document.querySelector("base") ? t : t.slice(d)) + a : I0() + t + a;
         try {
             e[u ? "replaceState" : "pushState"](c, "", f), s.value = c
         } catch (h) {
             console.error(h), n[u ? "replace" : "assign"](f)
         }
     }
 
@@ -4198,42 +4201,42 @@
         location: r,
         state: s,
         push: l,
         replace: o
     }
 }
 
-function P0(t) {
-    t = C0(t);
-    const e = I0(t),
-        n = D0(t, e.state, e.location, e.replace);
+function L0(t) {
+    t = T0(t);
+    const e = $0(t),
+        n = P0(t, e.state, e.location, e.replace);
 
     function r(i, o = !0) {
         o || n.pauseListeners(), history.go(i)
     }
     const s = Re({
         location: "",
         base: t,
         go: r,
-        createHref: T0.bind(null, t)
+        createHref: M0.bind(null, t)
     }, e, n);
     return Object.defineProperty(s, "location", {
         enumerable: !0,
         get: () => e.location.value
     }), Object.defineProperty(s, "state", {
         enumerable: !0,
         get: () => e.state.value
     }), s
 }
 
-function $0(t) {
-    return t = location.host ? t || location.pathname + location.search : "", t.includes("#") || (t += "#"), P0(t)
+function F0(t) {
+    return t = location.host ? t || location.pathname + location.search : "", t.includes("#") || (t += "#"), L0(t)
 }
 
-function L0(t) {
+function B0(t) {
     return typeof t == "string" || t && typeof t == "object"
 }
 
 function Fh(t) {
     return typeof t == "string" || typeof t == "symbol"
 }
 const Bn = {
@@ -4260,34 +4263,34 @@
     }, e)
 }
 
 function _n(t, e) {
     return t instanceof Error && Bh in t && (e == null || !!(t.type & e))
 }
 const ju = "[^/]+?",
-    F0 = {
+    H0 = {
         sensitive: !1,
         strict: !1,
         start: !0,
         end: !0
     },
-    B0 = /[.+*?^${}()[\]/\\]/g;
+    z0 = /[.+*?^${}()[\]/\\]/g;
 
-function H0(t, e) {
-    const n = Re({}, F0, e),
+function V0(t, e) {
+    const n = Re({}, H0, e),
         r = [];
     let s = n.start ? "^" : "";
     const i = [];
     for (const c of t) {
         const u = c.length ? [] : [90];
         n.strict && !c.length && (s += "/");
         for (let d = 0; d < c.length; d++) {
             const f = c[d];
             let h = 40 + (n.sensitive ? .25 : 0);
-            if (f.type === 0) d || (s += "/"), s += f.value.replace(B0, "\\$&"), h += 40;
+            if (f.type === 0) d || (s += "/"), s += f.value.replace(z0, "\\$&"), h += 40;
             else if (f.type === 1) {
                 const {
                     value: p,
                     repeatable: g,
                     optional: v,
                     regexp: x
                 } = f;
@@ -4359,56 +4362,56 @@
         score: r,
         keys: i,
         parse: l,
         stringify: a
     }
 }
 
-function z0(t, e) {
+function j0(t, e) {
     let n = 0;
     for (; n < t.length && n < e.length;) {
         const r = e[n] - t[n];
         if (r) return r;
         n++
     }
     return t.length < e.length ? t.length === 1 && t[0] === 40 + 40 ? -1 : 1 : t.length > e.length ? e.length === 1 && e[0] === 40 + 40 ? 1 : -1 : 0
 }
 
-function V0(t, e) {
+function U0(t, e) {
     let n = 0;
     const r = t.score,
         s = e.score;
     for (; n < r.length && n < s.length;) {
-        const i = z0(r[n], s[n]);
+        const i = j0(r[n], s[n]);
         if (i) return i;
         n++
     }
     if (Math.abs(s.length - r.length) === 1) {
         if (Uu(r)) return 1;
         if (Uu(s)) return -1
     }
     return s.length - r.length
 }
 
 function Uu(t) {
     const e = t[t.length - 1];
     return t.length > 0 && e[e.length - 1] < 0
 }
-const j0 = {
+const W0 = {
         type: 0,
         value: ""
     },
-    U0 = /[a-zA-Z0-9_]/;
+    q0 = /[a-zA-Z0-9_]/;
 
-function W0(t) {
+function K0(t) {
     if (!t) return [
         []
     ];
     if (t === "/") return [
-        [j0]
+        [W0]
     ];
     if (!t.startsWith("/")) throw new Error(`Invalid path "${t}"`);
 
     function e(h) {
         throw new Error(`ERR (${n})/"${c}": ${h}`)
     }
     let n = 0,
@@ -4448,15 +4451,15 @@
             case 0:
                 a === "/" ? (c && d(), o()) : a === ":" ? (d(), n = 1) : f();
                 break;
             case 4:
                 f(), n = r;
                 break;
             case 1:
-                a === "(" ? n = 2 : U0.test(a) ? f() : (d(), n = 0, a !== "*" && a !== "?" && a !== "+" && l--);
+                a === "(" ? n = 2 : q0.test(a) ? f() : (d(), n = 0, a !== "*" && a !== "?" && a !== "+" && l--);
                 break;
             case 2:
                 a === ")" ? u[u.length - 1] == "\\" ? u = u.slice(0, -1) + a : n = 3 : u += a;
                 break;
             case 3:
                 d(), n = 0, a !== "*" && a !== "?" && a !== "+" && l--, u = "";
                 break;
@@ -4464,41 +4467,41 @@
                 e("Unknown state");
                 break
         }
     }
     return n === 2 && e(`Unfinished custom RegExp for param "${c}"`), d(), o(), s
 }
 
-function q0(t, e, n) {
-    const r = H0(W0(t.path), n),
+function J0(t, e, n) {
+    const r = V0(K0(t.path), n),
         s = Re(r, {
             record: t,
             parent: e,
             children: [],
             alias: []
         });
     return e && !s.record.aliasOf == !e.record.aliasOf && e.children.push(s), s
 }
 
-function K0(t, e) {
+function G0(t, e) {
     const n = [],
         r = new Map;
     e = Ku({
         strict: !1,
         end: !0,
         sensitive: !1
     }, e);
 
     function s(u) {
         return r.get(u)
     }
 
     function i(u, d, f) {
         const h = !f,
-            p = J0(u);
+            p = Y0(u);
         p.aliasOf = f && f.record;
         const g = Ku(e, u),
             v = [p];
         if ("alias" in u) {
             const S = typeof u.alias == "string" ? [u.alias] : u.alias;
             for (const y of S) v.push(Re({}, p, {
                 components: f ? f.record.components : p.components,
@@ -4512,15 +4515,15 @@
                 path: y
             } = S;
             if (d && y[0] !== "/") {
                 const I = d.record.path,
                     T = I[I.length - 1] === "/" ? "" : "/";
                 S.path = d.record.path + (y && T + y)
             }
-            if (x = q0(S, d, g), f ? f.alias.push(x) : (w = w || x, w !== x && w.alias.push(x), h && u.name && !qu(x) && o(u.name)), p.children) {
+            if (x = J0(S, d, g), f ? f.alias.push(x) : (w = w || x, w !== x && w.alias.push(x), h && u.name && !qu(x) && o(u.name)), p.children) {
                 const I = p.children;
                 for (let T = 0; T < I.length; T++) i(I[T], x, f && f.children[T])
             }
             f = f || x, (x.record.components && Object.keys(x.record.components).length || x.record.name || x.record.redirect) && a(x)
         }
         return w ? () => {
             o(w)
@@ -4539,15 +4542,15 @@
 
     function l() {
         return n
     }
 
     function a(u) {
         let d = 0;
-        for (; d < n.length && V0(u, n[d]) >= 0 && (u.record.path !== n[d].record.path || !Hh(u, n[d]));) d++;
+        for (; d < n.length && U0(u, n[d]) >= 0 && (u.record.path !== n[d].record.path || !Hh(u, n[d]));) d++;
         n.splice(d, 0, u), u.record.name && !qu(u) && r.set(u.record.name, u)
     }
 
     function c(u, d) {
         let f, h = {},
             p, g;
         if ("name" in u && u.name) {
@@ -4567,15 +4570,15 @@
         let x = f;
         for (; x;) v.unshift(x.record), x = x.parent;
         return {
             name: g,
             path: p,
             params: h,
             matched: v,
-            meta: Y0(v)
+            meta: Q0(v)
         }
     }
     return t.forEach(u => i(u)), {
         addRoute: i,
         resolve: c,
         removeRoute: o,
         getRoutes: l,
@@ -4585,35 +4588,35 @@
 
 function Wu(t, e) {
     const n = {};
     for (const r of e) r in t && (n[r] = t[r]);
     return n
 }
 
-function J0(t) {
+function Y0(t) {
     return {
         path: t.path,
         redirect: t.redirect,
         name: t.name,
         meta: t.meta || {},
         aliasOf: void 0,
         beforeEnter: t.beforeEnter,
-        props: G0(t),
+        props: X0(t),
         children: t.children || [],
         instances: {},
         leaveGuards: new Set,
         updateGuards: new Set,
         enterCallbacks: {},
         components: "components" in t ? t.components || null : t.component && {
             default: t.component
         }
     }
 }
 
-function G0(t) {
+function X0(t) {
     const e = {},
         n = t.props || !1;
     if ("component" in t) e.default = n;
     else
         for (const r in t.components) e[r] = typeof n == "boolean" ? n : n[r];
     return e
 }
@@ -4622,113 +4625,113 @@
     for (; t;) {
         if (t.record.aliasOf) return !0;
         t = t.parent
     }
     return !1
 }
 
-function Y0(t) {
+function Q0(t) {
     return t.reduce((e, n) => Re(e, n.meta), {})
 }
 
 function Ku(t, e) {
     const n = {};
     for (const r in t) n[r] = r in e ? e[r] : t[r];
     return n
 }
 
 function Hh(t, e) {
     return e.children.some(n => n === t || Hh(t, n))
 }
 const zh = /#/g,
-    X0 = /&/g,
-    Q0 = /\//g,
-    Z0 = /=/g,
-    ev = /\?/g,
+    Z0 = /&/g,
+    ev = /\//g,
+    tv = /=/g,
+    nv = /\?/g,
     Vh = /\+/g,
-    tv = /%5B/g,
-    nv = /%5D/g,
+    rv = /%5B/g,
+    sv = /%5D/g,
     jh = /%5E/g,
-    rv = /%60/g,
+    iv = /%60/g,
     Uh = /%7B/g,
-    sv = /%7C/g,
+    ov = /%7C/g,
     Wh = /%7D/g,
-    iv = /%20/g;
+    lv = /%20/g;
 
 function vc(t) {
-    return encodeURI("" + t).replace(sv, "|").replace(tv, "[").replace(nv, "]")
+    return encodeURI("" + t).replace(ov, "|").replace(rv, "[").replace(sv, "]")
 }
 
-function ov(t) {
+function av(t) {
     return vc(t).replace(Uh, "{").replace(Wh, "}").replace(jh, "^")
 }
 
 function ka(t) {
-    return vc(t).replace(Vh, "%2B").replace(iv, "+").replace(zh, "%23").replace(X0, "%26").replace(rv, "`").replace(Uh, "{").replace(Wh, "}").replace(jh, "^")
+    return vc(t).replace(Vh, "%2B").replace(lv, "+").replace(zh, "%23").replace(Z0, "%26").replace(iv, "`").replace(Uh, "{").replace(Wh, "}").replace(jh, "^")
 }
 
-function lv(t) {
-    return ka(t).replace(Z0, "%3D")
+function cv(t) {
+    return ka(t).replace(tv, "%3D")
 }
 
-function av(t) {
-    return vc(t).replace(zh, "%23").replace(ev, "%3F")
+function uv(t) {
+    return vc(t).replace(zh, "%23").replace(nv, "%3F")
 }
 
-function cv(t) {
-    return t == null ? "" : av(t).replace(Q0, "%2F")
+function dv(t) {
+    return t == null ? "" : uv(t).replace(ev, "%2F")
 }
 
-function io(t) {
+function lo(t) {
     try {
         return decodeURIComponent("" + t)
     } catch {}
     return "" + t
 }
 
-function uv(t) {
+function fv(t) {
     const e = {};
     if (t === "" || t === "?") return e;
     const r = (t[0] === "?" ? t.slice(1) : t).split("&");
     for (let s = 0; s < r.length; ++s) {
         const i = r[s].replace(Vh, " "),
             o = i.indexOf("="),
-            l = io(o < 0 ? i : i.slice(0, o)),
-            a = o < 0 ? null : io(i.slice(o + 1));
+            l = lo(o < 0 ? i : i.slice(0, o)),
+            a = o < 0 ? null : lo(i.slice(o + 1));
         if (l in e) {
             let c = e[l];
             sn(c) || (c = e[l] = [c]), c.push(a)
         } else e[l] = a
     }
     return e
 }
 
 function Ju(t) {
     let e = "";
     for (let n in t) {
         const r = t[n];
-        if (n = lv(n), r == null) {
+        if (n = cv(n), r == null) {
             r !== void 0 && (e += (e.length ? "&" : "") + n);
             continue
         }(sn(r) ? r.map(i => i && ka(i)) : [r && ka(r)]).forEach(i => {
             i !== void 0 && (e += (e.length ? "&" : "") + n, i != null && (e += "=" + i))
         })
     }
     return e
 }
 
-function dv(t) {
+function hv(t) {
     const e = {};
     for (const n in t) {
         const r = t[n];
         r !== void 0 && (e[n] = sn(r) ? r.map(s => s == null ? null : "" + s) : r == null ? r : "" + r)
     }
     return e
 }
-const fv = Symbol(""),
+const pv = Symbol(""),
     Gu = Symbol(""),
     xc = Symbol(""),
     qh = Symbol(""),
     wa = Symbol("");
 
 function Ds() {
     let t = [];
@@ -4753,15 +4756,15 @@
 function Un(t, e, n, r, s) {
     const i = r && (r.enterCallbacks[s] = r.enterCallbacks[s] || []);
     return () => new Promise((o, l) => {
         const a = d => {
                 d === !1 ? l(as(4, {
                     from: n,
                     to: e
-                })) : d instanceof Error ? l(d) : L0(d) ? l(as(2, {
+                })) : d instanceof Error ? l(d) : B0(d) ? l(as(2, {
                     from: e,
                     to: d
                 })) : (i && r.enterCallbacks[s] === i && typeof d == "function" && i.push(d), o())
             },
             c = t.call(r && r.instances[s], e, n, a);
         let u = Promise.resolve(c);
         t.length < 3 && (u = u.then(a)), u.catch(d => l(d))
@@ -4770,32 +4773,32 @@
 
 function Tl(t, e, n, r) {
     const s = [];
     for (const i of t)
         for (const o in i.components) {
             let l = i.components[o];
             if (!(e !== "beforeRouteEnter" && !i.instances[o]))
-                if (hv(l)) {
+                if (mv(l)) {
                     const c = (l.__vccOpts || l)[e];
                     c && s.push(Un(c, n, r, i, o))
                 } else {
                     let a = l();
                     s.push(() => a.then(c => {
                         if (!c) return Promise.reject(new Error(`Couldn't resolve component "${o}" at "${i.path}"`));
-                        const u = b0(c) ? c.default : c;
+                        const u = x0(c) ? c.default : c;
                         i.components[o] = u;
                         const f = (u.__vccOpts || u)[e];
                         return f && Un(f, n, r, i, o)()
                     }))
                 }
         }
     return s
 }
 
-function hv(t) {
+function mv(t) {
     return typeof t == "object" || "displayName" in t || "props" in t || "__vccOpts" in t
 }
 
 function Yu(t) {
     const e = On(xc),
         n = On(qh),
         r = Bt(() => e.resolve(de(t.to))),
@@ -4807,29 +4810,29 @@
             } = a, u = a[c - 1], d = n.matched;
             if (!u || !d.length) return -1;
             const f = d.findIndex(ls.bind(null, u));
             if (f > -1) return f;
             const h = Xu(a[c - 2]);
             return c > 1 && Xu(u) === h && d[d.length - 1].path !== h ? d.findIndex(ls.bind(null, a[c - 2])) : f
         }),
-        i = Bt(() => s.value > -1 && yv(n.params, r.value.params)),
+        i = Bt(() => s.value > -1 && vv(n.params, r.value.params)),
         o = Bt(() => s.value > -1 && s.value === n.matched.length - 1 && $h(n.params, r.value.params));
 
     function l(a = {}) {
-        return gv(a) ? e[de(t.replace) ? "replace" : "push"](de(t.to)).catch(Js) : Promise.resolve()
+        return bv(a) ? e[de(t.replace) ? "replace" : "push"](de(t.to)).catch(Js) : Promise.resolve()
     }
     return {
         route: r,
         href: Bt(() => r.value.href),
         isActive: i,
         isExactActive: o,
         navigate: l
     }
 }
-const pv = ir({
+const gv = ir({
         name: "RouterLink",
         compatConfig: {
             MODE: 3
         },
         props: {
             to: {
                 type: [String, Object],
@@ -4863,42 +4866,42 @@
                     href: n.href,
                     onClick: n.navigate,
                     class: s.value
                 }, i)
             }
         }
     }),
-    mv = pv;
+    yv = gv;
 
-function gv(t) {
+function bv(t) {
     if (!(t.metaKey || t.altKey || t.ctrlKey || t.shiftKey) && !t.defaultPrevented && !(t.button !== void 0 && t.button !== 0)) {
         if (t.currentTarget && t.currentTarget.getAttribute) {
             const e = t.currentTarget.getAttribute("target");
             if (/\b_blank\b/i.test(e)) return
         }
         return t.preventDefault && t.preventDefault(), !0
     }
 }
 
-function yv(t, e) {
+function vv(t, e) {
     for (const n in e) {
         const r = e[n],
             s = t[n];
         if (typeof r == "string") {
             if (r !== s) return !1
         } else if (!sn(s) || s.length !== r.length || r.some((i, o) => i !== s[o])) return !1
     }
     return !0
 }
 
 function Xu(t) {
     return t ? t.aliasOf ? t.aliasOf.path : t.path : ""
 }
 const Qu = (t, e, n) => t ?? e ?? n,
-    bv = ir({
+    xv = ir({
         name: "RouterView",
         inheritAttrs: !1,
         props: {
             name: {
                 type: String,
                 default: "default"
             },
@@ -4921,16 +4924,16 @@
                     } = s.value;
                     let d;
                     for (;
                         (d = u[c]) && !d.components;) c++;
                     return c
                 }),
                 l = Bt(() => s.value.matched[o.value]);
-            Vi(Gu, Bt(() => o.value + 1)), Vi(fv, l), Vi(wa, s);
-            const a = No();
+            Ui(Gu, Bt(() => o.value + 1)), Ui(pv, l), Ui(wa, s);
+            const a = Do();
             return js(() => [a.value, l.value, t.name], ([c, u, d], [f, h, p]) => {
                 u && (u.instances[d] = c, h && h !== u && c && c === f && (u.leaveGuards.size || (u.leaveGuards = h.leaveGuards), u.updateGuards.size || (u.updateGuards = h.updateGuards))), c && u && (!h || !ls(u, h) || !f) && (u.enterCallbacks[d] || []).forEach(g => g(c))
             }, {
                 flush: "post"
             }), () => {
                 const c = s.value,
                     u = t.name,
@@ -4957,30 +4960,30 @@
     });
 
 function Zu(t, e) {
     if (!t) return null;
     const n = t(e);
     return n.length === 1 ? n[0] : n
 }
-const vv = bv;
+const kv = xv;
 
-function xv(t) {
-    const e = K0(t.routes, t),
-        n = t.parseQuery || uv,
+function wv(t) {
+    const e = G0(t.routes, t),
+        n = t.parseQuery || fv,
         r = t.stringifyQuery || Ju,
         s = t.history,
         i = Ds(),
         o = Ds(),
         l = Ds(),
         a = sh(Bn);
     let c = Bn;
     jr && t.scrollBehavior && "scrollRestoration" in history && (history.scrollRestoration = "manual");
     const u = Cl.bind(null, M => "" + M),
-        d = Cl.bind(null, cv),
-        f = Cl.bind(null, io);
+        d = Cl.bind(null, dv),
+        f = Cl.bind(null, lo);
 
     function h(M, j) {
         let z, Y;
         return Fh(M) ? (z = e.getRecordMatcher(M), Y = j) : Y = M, e.addRoute(Y, z)
     }
 
     function p(M) {
@@ -5001,15 +5004,15 @@
             const b = El(n, M, j.path),
                 k = e.resolve({
                     path: b.path
                 }, j),
                 _ = s.createHref(b.fullPath);
             return Re(b, k, {
                 params: f(k.params),
-                hash: io(b.hash),
+                hash: lo(b.hash),
                 redirectedFrom: void 0,
                 href: _
             })
         }
         let z;
         if ("path" in M) z = Re({}, M, {
             path: El(n, M.path, j.path).path
@@ -5020,23 +5023,23 @@
             z = Re({}, M, {
                 params: d(M.params)
             }), j.params = d(j.params)
         }
         const Y = e.resolve(z, j),
             ye = M.hash || "";
         Y.params = u(f(Y.params));
-        const Ee = k0(r, Re({}, M, {
-                hash: ov(ye),
+        const Ee = S0(r, Re({}, M, {
+                hash: av(ye),
                 path: Y.path
             })),
             ue = s.createHref(Ee);
         return Re({
             fullPath: Ee,
             hash: ye,
-            query: r === Ju ? dv(M.query) : M.query || {}
+            query: r === Ju ? hv(M.query) : M.query || {}
         }, Y, {
             redirectedFrom: void 0,
             href: ue
         })
     }
 
     function w(M) {
@@ -5088,18 +5091,18 @@
             state: typeof b == "object" ? Re({}, ye, b.state) : ye,
             force: Ee,
             replace: ue
         }), j || z);
         const k = z;
         k.redirectedFrom = j;
         let _;
-        return !Ee && w0(r, Y, z) && (_ = as(16, {
+        return !Ee && _0(r, Y, z) && (_ = as(16, {
             to: k,
             from: Y
-        }), Ze(Y, Y, !0, !1)), (_ ? Promise.resolve(_) : G(k, Y)).catch(O => _n(O) ? _n(O, 2) ? O : He(O) : fe(O, k, Y)).then(O => {
+        }), Ze(Y, Y, !0, !1)), (_ ? Promise.resolve(_) : G(k, Y)).catch(O => _n(O) ? _n(O, 2) ? O : ze(O) : he(O, k, Y)).then(O => {
             if (O) {
                 if (_n(O, 2)) return V(Re({
                     replace: ue
                 }, w(O.to), {
                     state: typeof O.to == "object" ? Re({}, ye, O.to.state) : ye,
                     force: Ee
                 }), j || k)
@@ -5111,15 +5114,15 @@
     function N(M, j) {
         const z = S(M, j);
         return z ? Promise.reject(z) : Promise.resolve()
     }
 
     function G(M, j) {
         let z;
-        const [Y, ye, Ee] = kv(M, j);
+        const [Y, ye, Ee] = Sv(M, j);
         z = Tl(Y.reverse(), "beforeRouteLeave", M, j);
         for (const b of Y) b.leaveGuards.forEach(k => {
             z.push(Un(k, M, j))
         });
         const ue = N.bind(null, M, j);
         return z.push(ue), zr(z).then(() => {
             z = [];
@@ -5153,15 +5156,15 @@
     function ne(M, j, z, Y, ye) {
         const Ee = S(M, j);
         if (Ee) return Ee;
         const ue = j === Bn,
             b = jr ? history.state : {};
         z && (Y || ue ? s.replace(M.fullPath, Re({
             scroll: ue && b && b.scroll
-        }, ye)) : s.push(M.fullPath, ye)), a.value = M, Ze(M, j, z, ue), He()
+        }, ye)) : s.push(M.fullPath, ye)), a.value = M, Ze(M, j, z, ue), ze()
     }
     let H;
 
     function ie() {
         H || (H = s.listen((M, j, z) => {
             if (!St.listening) return;
             const Y = x(M),
@@ -5170,48 +5173,48 @@
                 V(Re(ye, {
                     replace: !0
                 }), Y).catch(Js);
                 return
             }
             c = Y;
             const Ee = a.value;
-            jr && A0(Hu(Ee.fullPath, z.delta), Vo()), G(Y, Ee).catch(ue => _n(ue, 12) ? ue : _n(ue, 2) ? (V(ue.to, Y).then(b => {
+            jr && R0(Hu(Ee.fullPath, z.delta), Vo()), G(Y, Ee).catch(ue => _n(ue, 12) ? ue : _n(ue, 2) ? (V(ue.to, Y).then(b => {
                 _n(b, 20) && !z.delta && z.type === ui.pop && s.go(-1, !1)
-            }).catch(Js), Promise.reject()) : (z.delta && s.go(-z.delta, !1), fe(ue, Y, Ee))).then(ue => {
+            }).catch(Js), Promise.reject()) : (z.delta && s.go(-z.delta, !1), he(ue, Y, Ee))).then(ue => {
                 ue = ue || ne(Y, Ee, !1), ue && (z.delta && !_n(ue, 8) ? s.go(-z.delta, !1) : z.type === ui.pop && _n(ue, 20) && s.go(-1, !1)), J(Y, Ee, ue)
             }).catch(Js)
         }))
     }
     let Ae = Ds(),
-        Be = Ds(),
+        He = Ds(),
         ge;
 
-    function fe(M, j, z) {
-        He(M);
-        const Y = Be.list();
+    function he(M, j, z) {
+        ze(M);
+        const Y = He.list();
         return Y.length ? Y.forEach(ye => ye(M, j, z)) : console.error(M), Promise.reject(M)
     }
 
     function ae() {
         return ge && a.value !== Bn ? Promise.resolve() : new Promise((M, j) => {
             Ae.add([M, j])
         })
     }
 
-    function He(M) {
+    function ze(M) {
         return ge || (ge = !M, ie(), Ae.list().forEach(([j, z]) => M ? z(M) : j()), Ae.reset()), M
     }
 
     function Ze(M, j, z, Y) {
         const {
             scrollBehavior: ye
         } = t;
         if (!jr || !ye) return Promise.resolve();
-        const Ee = !z && N0(Hu(M.fullPath, 0)) || (Y || !z) && history.state && history.state.scroll || null;
-        return dc().then(() => ye(M, j, Ee)).then(ue => ue && M0(ue)).catch(ue => fe(ue, M, j))
+        const Ee = !z && D0(Hu(M.fullPath, 0)) || (Y || !z) && history.state && history.state.scroll || null;
+        return dc().then(() => ye(M, j, Ee)).then(ue => ue && N0(ue)).catch(ue => he(ue, M, j))
     }
     const Ke = M => s.go(M);
     let Pe;
     const wt = new Set,
         St = {
             currentRoute: a,
             listening: !0,
@@ -5225,19 +5228,19 @@
             replace: I,
             go: Ke,
             back: () => Ke(-1),
             forward: () => Ke(1),
             beforeEach: i.add,
             beforeResolve: o.add,
             afterEach: l.add,
-            onError: Be.add,
+            onError: He.add,
             isReady: ae,
             install(M) {
                 const j = this;
-                M.component("RouterLink", mv), M.component("RouterView", vv), M.config.globalProperties.$router = j, Object.defineProperty(M.config.globalProperties, "$route", {
+                M.component("RouterLink", yv), M.component("RouterView", kv), M.config.globalProperties.$router = j, Object.defineProperty(M.config.globalProperties, "$route", {
                     enumerable: !0,
                     get: () => de(a)
                 }), jr && !Pe && a.value === Bn && (Pe = !0, y(s.location).catch(ye => {}));
                 const z = {};
                 for (const ye in Bn) z[ye] = Bt(() => a.value[ye]);
                 M.provide(xc, j), M.provide(qh, Es(z)), M.provide(wa, a);
                 const Y = M.unmount;
@@ -5249,15 +5252,15 @@
     return St
 }
 
 function zr(t) {
     return t.reduce((e, n) => e.then(() => n()), Promise.resolve())
 }
 
-function kv(t, e) {
+function Sv(t, e) {
     const n = [],
         r = [],
         s = [],
         i = Math.max(e.matched.length, t.matched.length);
     for (let o = 0; o < i; o++) {
         const l = e.matched[o];
         l && (t.matched.find(c => ls(c, l)) ? r.push(l) : n.push(l));
@@ -5269,56 +5272,56 @@
 
 function Kh(t, e) {
     return function() {
         return t.apply(e, arguments)
     }
 }
 const {
-    toString: wv
+    toString: _v
 } = Object.prototype, {
     getPrototypeOf: kc
 } = Object, jo = (t => e => {
-    const n = wv.call(e);
+    const n = _v.call(e);
     return t[n] || (t[n] = n.slice(8, -1).toLowerCase())
 })(Object.create(null)), wn = t => (t = t.toLowerCase(), e => jo(e) === t), Uo = t => e => typeof e === t, {
     isArray: Os
 } = Array, di = Uo("undefined");
 
-function Sv(t) {
+function Cv(t) {
     return t !== null && !di(t) && t.constructor !== null && !di(t.constructor) && jt(t.constructor.isBuffer) && t.constructor.isBuffer(t)
 }
 const Jh = wn("ArrayBuffer");
 
-function _v(t) {
+function Ev(t) {
     let e;
     return typeof ArrayBuffer < "u" && ArrayBuffer.isView ? e = ArrayBuffer.isView(t) : e = t && t.buffer && Jh(t.buffer), e
 }
-const Cv = Uo("string"),
+const Tv = Uo("string"),
     jt = Uo("function"),
     Gh = Uo("number"),
     Wo = t => t !== null && typeof t == "object",
-    Ev = t => t === !0 || t === !1,
-    Ui = t => {
+    Ov = t => t === !0 || t === !1,
+    qi = t => {
         if (jo(t) !== "object") return !1;
         const e = kc(t);
         return (e === null || e === Object.prototype || Object.getPrototypeOf(e) === null) && !(Symbol.toStringTag in t) && !(Symbol.iterator in t)
     },
-    Tv = wn("Date"),
-    Ov = wn("File"),
-    Mv = wn("Blob"),
-    Av = wn("FileList"),
-    Nv = t => Wo(t) && jt(t.pipe),
-    Rv = t => {
+    Mv = wn("Date"),
+    Av = wn("File"),
+    Nv = wn("Blob"),
+    Rv = wn("FileList"),
+    Dv = t => Wo(t) && jt(t.pipe),
+    Iv = t => {
         let e;
         return t && (typeof FormData == "function" && t instanceof FormData || jt(t.append) && ((e = jo(t)) === "formdata" || e === "object" && jt(t.toString) && t.toString() === "[object FormData]"))
     },
-    Dv = wn("URLSearchParams"),
-    Iv = t => t.trim ? t.trim() : t.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "");
+    Pv = wn("URLSearchParams"),
+    $v = t => t.trim ? t.trim() : t.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "");
 
-function xi(t, e, {
+function wi(t, e, {
     allOwnKeys: n = !1
 } = {}) {
     if (t === null || typeof t > "u") return;
     let r, s;
     if (typeof t != "object" && (t = [t]), Os(t))
         for (r = 0, s = t.length; r < s; r++) e.call(null, t[r], r, t);
     else {
@@ -5342,205 +5345,205 @@
     Qh = t => !di(t) && t !== Xh;
 
 function Sa() {
     const {
         caseless: t
     } = Qh(this) && this || {}, e = {}, n = (r, s) => {
         const i = t && Yh(e, s) || s;
-        Ui(e[i]) && Ui(r) ? e[i] = Sa(e[i], r) : Ui(r) ? e[i] = Sa({}, r) : Os(r) ? e[i] = r.slice() : e[i] = r
+        qi(e[i]) && qi(r) ? e[i] = Sa(e[i], r) : qi(r) ? e[i] = Sa({}, r) : Os(r) ? e[i] = r.slice() : e[i] = r
     };
-    for (let r = 0, s = arguments.length; r < s; r++) arguments[r] && xi(arguments[r], n);
+    for (let r = 0, s = arguments.length; r < s; r++) arguments[r] && wi(arguments[r], n);
     return e
 }
-const Pv = (t, e, n, {
+const Lv = (t, e, n, {
         allOwnKeys: r
-    } = {}) => (xi(e, (s, i) => {
+    } = {}) => (wi(e, (s, i) => {
         n && jt(s) ? t[i] = Kh(s, n) : t[i] = s
     }, {
         allOwnKeys: r
     }), t),
-    $v = t => (t.charCodeAt(0) === 65279 && (t = t.slice(1)), t),
-    Lv = (t, e, n, r) => {
+    Fv = t => (t.charCodeAt(0) === 65279 && (t = t.slice(1)), t),
+    Bv = (t, e, n, r) => {
         t.prototype = Object.create(e.prototype, r), t.prototype.constructor = t, Object.defineProperty(t, "super", {
             value: e.prototype
         }), n && Object.assign(t.prototype, n)
     },
-    Fv = (t, e, n, r) => {
+    Hv = (t, e, n, r) => {
         let s, i, o;
         const l = {};
         if (e = e || {}, t == null) return e;
         do {
             for (s = Object.getOwnPropertyNames(t), i = s.length; i-- > 0;) o = s[i], (!r || r(o, t, e)) && !l[o] && (e[o] = t[o], l[o] = !0);
             t = n !== !1 && kc(t)
         } while (t && (!n || n(t, e)) && t !== Object.prototype);
         return e
     },
-    Bv = (t, e, n) => {
+    zv = (t, e, n) => {
         t = String(t), (n === void 0 || n > t.length) && (n = t.length), n -= e.length;
         const r = t.indexOf(e, n);
         return r !== -1 && r === n
     },
-    Hv = t => {
+    Vv = t => {
         if (!t) return null;
         if (Os(t)) return t;
         let e = t.length;
         if (!Gh(e)) return null;
         const n = new Array(e);
         for (; e-- > 0;) n[e] = t[e];
         return n
     },
-    zv = (t => e => t && e instanceof t)(typeof Uint8Array < "u" && kc(Uint8Array)),
-    Vv = (t, e) => {
+    jv = (t => e => t && e instanceof t)(typeof Uint8Array < "u" && kc(Uint8Array)),
+    Uv = (t, e) => {
         const r = (t && t[Symbol.iterator]).call(t);
         let s;
         for (;
             (s = r.next()) && !s.done;) {
             const i = s.value;
             e.call(t, i[0], i[1])
         }
     },
-    jv = (t, e) => {
+    Wv = (t, e) => {
         let n;
         const r = [];
         for (;
             (n = t.exec(e)) !== null;) r.push(n);
         return r
     },
-    Uv = wn("HTMLFormElement"),
-    Wv = t => t.toLowerCase().replace(/[-_\s]([a-z\d])(\w*)/g, function(n, r, s) {
+    qv = wn("HTMLFormElement"),
+    Kv = t => t.toLowerCase().replace(/[-_\s]([a-z\d])(\w*)/g, function(n, r, s) {
         return r.toUpperCase() + s
     }),
     ed = (({
         hasOwnProperty: t
     }) => (e, n) => t.call(e, n))(Object.prototype),
-    qv = wn("RegExp"),
+    Jv = wn("RegExp"),
     Zh = (t, e) => {
         const n = Object.getOwnPropertyDescriptors(t),
             r = {};
-        xi(n, (s, i) => {
+        wi(n, (s, i) => {
             e(s, i, t) !== !1 && (r[i] = s)
         }), Object.defineProperties(t, r)
     },
-    Kv = t => {
+    Gv = t => {
         Zh(t, (e, n) => {
             if (jt(t) && ["arguments", "caller", "callee"].indexOf(n) !== -1) return !1;
             const r = t[n];
             if (jt(r)) {
                 if (e.enumerable = !1, "writable" in e) {
                     e.writable = !1;
                     return
                 }
                 e.set || (e.set = () => {
                     throw Error("Can not rewrite read-only method '" + n + "'")
                 })
             }
         })
     },
-    Jv = (t, e) => {
+    Yv = (t, e) => {
         const n = {},
             r = s => {
                 s.forEach(i => {
                     n[i] = !0
                 })
             };
         return Os(t) ? r(t) : r(String(t).split(e)), n
     },
-    Gv = () => {},
-    Yv = (t, e) => (t = +t, Number.isFinite(t) ? t : e),
+    Xv = () => {},
+    Qv = (t, e) => (t = +t, Number.isFinite(t) ? t : e),
     Ol = "abcdefghijklmnopqrstuvwxyz",
     td = "0123456789",
     ep = {
         DIGIT: td,
         ALPHA: Ol,
         ALPHA_DIGIT: Ol + Ol.toUpperCase() + td
     },
-    Xv = (t = 16, e = ep.ALPHA_DIGIT) => {
+    Zv = (t = 16, e = ep.ALPHA_DIGIT) => {
         let n = "";
         const {
             length: r
         } = e;
         for (; t--;) n += e[Math.random() * r | 0];
         return n
     };
 
-function Qv(t) {
+function e1(t) {
     return !!(t && jt(t.append) && t[Symbol.toStringTag] === "FormData" && t[Symbol.iterator])
 }
-const Zv = t => {
+const t1 = t => {
         const e = new Array(10),
             n = (r, s) => {
                 if (Wo(r)) {
                     if (e.indexOf(r) >= 0) return;
                     if (!("toJSON" in r)) {
                         e[s] = r;
                         const i = Os(r) ? [] : {};
-                        return xi(r, (o, l) => {
+                        return wi(r, (o, l) => {
                             const a = n(o, s + 1);
                             !di(a) && (i[l] = a)
                         }), e[s] = void 0, i
                     }
                 }
                 return r
             };
         return n(t, 0)
     },
-    e1 = wn("AsyncFunction"),
-    t1 = t => t && (Wo(t) || jt(t)) && jt(t.then) && jt(t.catch),
+    n1 = wn("AsyncFunction"),
+    r1 = t => t && (Wo(t) || jt(t)) && jt(t.then) && jt(t.catch),
     A = {
         isArray: Os,
         isArrayBuffer: Jh,
-        isBuffer: Sv,
-        isFormData: Rv,
-        isArrayBufferView: _v,
-        isString: Cv,
+        isBuffer: Cv,
+        isFormData: Iv,
+        isArrayBufferView: Ev,
+        isString: Tv,
         isNumber: Gh,
-        isBoolean: Ev,
+        isBoolean: Ov,
         isObject: Wo,
-        isPlainObject: Ui,
+        isPlainObject: qi,
         isUndefined: di,
-        isDate: Tv,
-        isFile: Ov,
-        isBlob: Mv,
-        isRegExp: qv,
+        isDate: Mv,
+        isFile: Av,
+        isBlob: Nv,
+        isRegExp: Jv,
         isFunction: jt,
-        isStream: Nv,
-        isURLSearchParams: Dv,
-        isTypedArray: zv,
-        isFileList: Av,
-        forEach: xi,
+        isStream: Dv,
+        isURLSearchParams: Pv,
+        isTypedArray: jv,
+        isFileList: Rv,
+        forEach: wi,
         merge: Sa,
-        extend: Pv,
-        trim: Iv,
-        stripBOM: $v,
-        inherits: Lv,
-        toFlatObject: Fv,
+        extend: Lv,
+        trim: $v,
+        stripBOM: Fv,
+        inherits: Bv,
+        toFlatObject: Hv,
         kindOf: jo,
         kindOfTest: wn,
-        endsWith: Bv,
-        toArray: Hv,
-        forEachEntry: Vv,
-        matchAll: jv,
-        isHTMLForm: Uv,
+        endsWith: zv,
+        toArray: Vv,
+        forEachEntry: Uv,
+        matchAll: Wv,
+        isHTMLForm: qv,
         hasOwnProperty: ed,
         hasOwnProp: ed,
         reduceDescriptors: Zh,
-        freezeMethods: Kv,
-        toObjectSet: Jv,
-        toCamelCase: Wv,
-        noop: Gv,
-        toFiniteNumber: Yv,
+        freezeMethods: Gv,
+        toObjectSet: Yv,
+        toCamelCase: Kv,
+        noop: Xv,
+        toFiniteNumber: Qv,
         findKey: Yh,
         global: Xh,
         isContextDefined: Qh,
         ALPHABET: ep,
-        generateString: Xv,
-        isSpecCompliantForm: Qv,
-        toJSONObject: Zv,
-        isAsyncFn: e1,
-        isThenable: t1
+        generateString: Zv,
+        isSpecCompliantForm: e1,
+        toJSONObject: t1,
+        isAsyncFn: n1,
+        isThenable: r1
     };
 
 function Ce(t, e, n, r, s) {
     Error.call(this), Error.captureStackTrace ? Error.captureStackTrace(this, this.constructor) : this.stack = new Error().stack, this.message = t, this.name = "AxiosError", e && (this.code = e), n && (this.config = n), r && (this.request = r), s && (this.response = s)
 }
 A.inherits(Ce, Error, {
     toJSON: function() {
@@ -5572,15 +5575,15 @@
 });
 Ce.from = (t, e, n, r, s, i) => {
     const o = Object.create(tp);
     return A.toFlatObject(t, o, function(a) {
         return a !== Error.prototype
     }, l => l !== "isAxiosError"), Ce.call(o, t.message, e, n, r, s), o.cause = t, o.name = t.name, i && Object.assign(o, i), o
 };
-const n1 = null;
+const s1 = null;
 
 function _a(t) {
     return A.isPlainObject(t) || A.isArray(t)
 }
 
 function rp(t) {
     return A.endsWith(t, "[]") ? t.slice(0, -2) : t
@@ -5588,18 +5591,18 @@
 
 function nd(t, e, n) {
     return t ? t.concat(e).map(function(s, i) {
         return s = rp(s), !n && i ? "[" + s + "]" : s
     }).join(n ? "." : "") : e
 }
 
-function r1(t) {
+function i1(t) {
     return A.isArray(t) && !t.some(_a)
 }
-const s1 = A.toFlatObject(A, {}, null, function(e) {
+const o1 = A.toFlatObject(A, {}, null, function(e) {
     return /^is[A-Z]/.test(e)
 });
 
 function qo(t, e, n) {
     if (!A.isObject(t)) throw new TypeError("target must be an object");
     e = e || new FormData, n = A.toFlatObject(n, {
         metaTokens: !0,
@@ -5622,22 +5625,22 @@
         return A.isArrayBuffer(p) || A.isTypedArray(p) ? a && typeof Blob == "function" ? new Blob([p]) : Buffer.from(p) : p
     }
 
     function u(p, g, v) {
         let x = p;
         if (p && !v && typeof p == "object") {
             if (A.endsWith(g, "{}")) g = r ? g : g.slice(0, -2), p = JSON.stringify(p);
-            else if (A.isArray(p) && r1(p) || (A.isFileList(p) || A.endsWith(g, "[]")) && (x = A.toArray(p))) return g = rp(g), x.forEach(function(S, y) {
+            else if (A.isArray(p) && i1(p) || (A.isFileList(p) || A.endsWith(g, "[]")) && (x = A.toArray(p))) return g = rp(g), x.forEach(function(S, y) {
                 !(A.isUndefined(S) || S === null) && e.append(o === !0 ? nd([g], y, i) : o === null ? g : g + "[]", c(S))
             }), !1
         }
         return _a(p) ? !0 : (e.append(nd(v, g, i), c(p)), !1)
     }
     const d = [],
-        f = Object.assign(s1, {
+        f = Object.assign(o1, {
             defaultVisitor: u,
             convertValue: c,
             isVisitable: _a
         });
 
     function h(p, g) {
         if (!A.isUndefined(p)) {
@@ -5678,30 +5681,30 @@
         return e.call(this, r, rd)
     } : rd;
     return this._pairs.map(function(s) {
         return n(s[0]) + "=" + n(s[1])
     }, "").join("&")
 };
 
-function i1(t) {
+function l1(t) {
     return encodeURIComponent(t).replace(/%3A/gi, ":").replace(/%24/g, "$").replace(/%2C/gi, ",").replace(/%20/g, "+").replace(/%5B/gi, "[").replace(/%5D/gi, "]")
 }
 
 function ip(t, e, n) {
     if (!e) return t;
-    const r = n && n.encode || i1,
+    const r = n && n.encode || l1,
         s = n && n.serialize;
     let i;
     if (s ? i = s(e, n) : i = A.isURLSearchParams(e) ? e.toString() : new wc(e, n).toString(r), i) {
         const o = t.indexOf("#");
         o !== -1 && (t = t.slice(0, o)), t += (t.indexOf("?") === -1 ? "?" : "&") + i
     }
     return t
 }
-class o1 {
+class a1 {
     constructor() {
         this.handlers = []
     }
     use(e, n, r) {
         return this.handlers.push({
             fulfilled: e,
             rejected: n,
@@ -5717,82 +5720,82 @@
     }
     forEach(e) {
         A.forEach(this.handlers, function(r) {
             r !== null && e(r)
         })
     }
 }
-const sd = o1,
+const sd = a1,
     op = {
         silentJSONParsing: !0,
         forcedJSONParsing: !0,
         clarifyTimeoutError: !1
     },
-    l1 = typeof URLSearchParams < "u" ? URLSearchParams : wc,
-    a1 = typeof FormData < "u" ? FormData : null,
-    c1 = typeof Blob < "u" ? Blob : null,
-    u1 = (() => {
+    c1 = typeof URLSearchParams < "u" ? URLSearchParams : wc,
+    u1 = typeof FormData < "u" ? FormData : null,
+    d1 = typeof Blob < "u" ? Blob : null,
+    f1 = (() => {
         let t;
         return typeof navigator < "u" && ((t = navigator.product) === "ReactNative" || t === "NativeScript" || t === "NS") ? !1 : typeof window < "u" && typeof document < "u"
     })(),
-    d1 = (() => typeof WorkerGlobalScope < "u" && self instanceof WorkerGlobalScope && typeof self.importScripts == "function")(),
+    h1 = (() => typeof WorkerGlobalScope < "u" && self instanceof WorkerGlobalScope && typeof self.importScripts == "function")(),
     fn = {
         isBrowser: !0,
         classes: {
-            URLSearchParams: l1,
-            FormData: a1,
-            Blob: c1
+            URLSearchParams: c1,
+            FormData: u1,
+            Blob: d1
         },
-        isStandardBrowserEnv: u1,
-        isStandardBrowserWebWorkerEnv: d1,
+        isStandardBrowserEnv: f1,
+        isStandardBrowserWebWorkerEnv: h1,
         protocols: ["http", "https", "file", "blob", "url", "data"]
     };
 
-function f1(t, e) {
+function p1(t, e) {
     return qo(t, new fn.classes.URLSearchParams, Object.assign({
         visitor: function(n, r, s, i) {
             return fn.isNode && A.isBuffer(n) ? (this.append(r, n.toString("base64")), !1) : i.defaultVisitor.apply(this, arguments)
         }
     }, e))
 }
 
-function h1(t) {
+function m1(t) {
     return A.matchAll(/\w+|\[(\w*)]/g, t).map(e => e[0] === "[]" ? "" : e[1] || e[0])
 }
 
-function p1(t) {
+function g1(t) {
     const e = {},
         n = Object.keys(t);
     let r;
     const s = n.length;
     let i;
     for (r = 0; r < s; r++) i = n[r], e[i] = t[i];
     return e
 }
 
 function lp(t) {
     function e(n, r, s, i) {
         let o = n[i++];
         const l = Number.isFinite(+o),
             a = i >= n.length;
-        return o = !o && A.isArray(s) ? s.length : o, a ? (A.hasOwnProp(s, o) ? s[o] = [s[o], r] : s[o] = r, !l) : ((!s[o] || !A.isObject(s[o])) && (s[o] = []), e(n, r, s[o], i) && A.isArray(s[o]) && (s[o] = p1(s[o])), !l)
+        return o = !o && A.isArray(s) ? s.length : o, a ? (A.hasOwnProp(s, o) ? s[o] = [s[o], r] : s[o] = r, !l) : ((!s[o] || !A.isObject(s[o])) && (s[o] = []), e(n, r, s[o], i) && A.isArray(s[o]) && (s[o] = g1(s[o])), !l)
     }
     if (A.isFormData(t) && A.isFunction(t.entries)) {
         const n = {};
         return A.forEachEntry(t, (r, s) => {
-            e(h1(r), s, n, 0)
+            e(m1(r), s, n, 0)
         }), n
     }
     return null
 }
-const m1 = {
+const y1 = {
     "Content-Type": void 0
 };
 
-function g1(t, e, n) {
+function b1(t, e, n) {
     if (A.isString(t)) try {
         return (e || JSON.parse)(t), A.trim(t)
     } catch (r) {
         if (r.name !== "SyntaxError") throw r
     }
     return (n || JSON.stringify)(t)
 }
@@ -5805,23 +5808,23 @@
             i = A.isObject(e);
         if (i && A.isHTMLForm(e) && (e = new FormData(e)), A.isFormData(e)) return s && s ? JSON.stringify(lp(e)) : e;
         if (A.isArrayBuffer(e) || A.isBuffer(e) || A.isStream(e) || A.isFile(e) || A.isBlob(e)) return e;
         if (A.isArrayBufferView(e)) return e.buffer;
         if (A.isURLSearchParams(e)) return n.setContentType("application/x-www-form-urlencoded;charset=utf-8", !1), e.toString();
         let l;
         if (i) {
-            if (r.indexOf("application/x-www-form-urlencoded") > -1) return f1(e, this.formSerializer).toString();
+            if (r.indexOf("application/x-www-form-urlencoded") > -1) return p1(e, this.formSerializer).toString();
             if ((l = A.isFileList(e)) || r.indexOf("multipart/form-data") > -1) {
                 const a = this.env && this.env.FormData;
                 return qo(l ? {
                     "files[]": e
                 } : e, a && new a, this.formSerializer)
             }
         }
-        return i || s ? (n.setContentType("application/json", !1), g1(e)) : e
+        return i || s ? (n.setContentType("application/json", !1), b1(e)) : e
     }],
     transformResponse: [function(e) {
         const n = this.transitional || Ko.transitional,
             r = n && n.forcedJSONParsing,
             s = this.responseType === "json";
         if (e && A.isString(e) && (r && !this.responseType || s)) {
             const o = !(n && n.silentJSONParsing) && s;
@@ -5851,58 +5854,58 @@
         }
     }
 };
 A.forEach(["delete", "get", "head"], function(e) {
     Ko.headers[e] = {}
 });
 A.forEach(["post", "put", "patch"], function(e) {
-    Ko.headers[e] = A.merge(m1)
+    Ko.headers[e] = A.merge(y1)
 });
 const Sc = Ko,
-    y1 = A.toObjectSet(["age", "authorization", "content-length", "content-type", "etag", "expires", "from", "host", "if-modified-since", "if-unmodified-since", "last-modified", "location", "max-forwards", "proxy-authorization", "referer", "retry-after", "user-agent"]),
-    b1 = t => {
+    v1 = A.toObjectSet(["age", "authorization", "content-length", "content-type", "etag", "expires", "from", "host", "if-modified-since", "if-unmodified-since", "last-modified", "location", "max-forwards", "proxy-authorization", "referer", "retry-after", "user-agent"]),
+    x1 = t => {
         const e = {};
         let n, r, s;
         return t && t.split(`
 `).forEach(function(o) {
-            s = o.indexOf(":"), n = o.substring(0, s).trim().toLowerCase(), r = o.substring(s + 1).trim(), !(!n || e[n] && y1[n]) && (n === "set-cookie" ? e[n] ? e[n].push(r) : e[n] = [r] : e[n] = e[n] ? e[n] + ", " + r : r)
+            s = o.indexOf(":"), n = o.substring(0, s).trim().toLowerCase(), r = o.substring(s + 1).trim(), !(!n || e[n] && v1[n]) && (n === "set-cookie" ? e[n] ? e[n].push(r) : e[n] = [r] : e[n] = e[n] ? e[n] + ", " + r : r)
         }), e
     },
     id = Symbol("internals");
 
 function Is(t) {
     return t && String(t).trim().toLowerCase()
 }
 
-function Wi(t) {
-    return t === !1 || t == null ? t : A.isArray(t) ? t.map(Wi) : String(t)
+function Ki(t) {
+    return t === !1 || t == null ? t : A.isArray(t) ? t.map(Ki) : String(t)
 }
 
-function v1(t) {
+function k1(t) {
     const e = Object.create(null),
         n = /([^\s,;=]+)\s*(?:=\s*([^,;]+))?/g;
     let r;
     for (; r = n.exec(t);) e[r[1]] = r[2];
     return e
 }
-const x1 = t => /^[-_a-zA-Z0-9^`|~,!#$%&'*+.]+$/.test(t.trim());
+const w1 = t => /^[-_a-zA-Z0-9^`|~,!#$%&'*+.]+$/.test(t.trim());
 
 function Ml(t, e, n, r, s) {
     if (A.isFunction(r)) return r.call(this, e, n);
     if (s && (e = n), !!A.isString(e)) {
         if (A.isString(r)) return e.indexOf(r) !== -1;
         if (A.isRegExp(r)) return r.test(e)
     }
 }
 
-function k1(t) {
+function S1(t) {
     return t.trim().toLowerCase().replace(/([a-z\d])(\w*)/g, (e, n, r) => n.toUpperCase() + r)
 }
 
-function w1(t, e) {
+function _1(t, e) {
     const n = A.toCamelCase(" " + e);
     ["get", "set", "has"].forEach(r => {
         Object.defineProperty(t, r + n, {
             value: function(s, i, o) {
                 return this[r].call(this, e, s, i, o)
             },
             configurable: !0
@@ -5916,26 +5919,26 @@
     set(e, n, r) {
         const s = this;
 
         function i(l, a, c) {
             const u = Is(a);
             if (!u) throw new Error("header name must be a non-empty string");
             const d = A.findKey(s, u);
-            (!d || s[d] === void 0 || c === !0 || c === void 0 && s[d] !== !1) && (s[d || a] = Wi(l))
+            (!d || s[d] === void 0 || c === !0 || c === void 0 && s[d] !== !1) && (s[d || a] = Ki(l))
         }
         const o = (l, a) => A.forEach(l, (c, u) => i(c, u, a));
-        return A.isPlainObject(e) || e instanceof this.constructor ? o(e, n) : A.isString(e) && (e = e.trim()) && !x1(e) ? o(b1(e), n) : e != null && i(n, e, r), this
+        return A.isPlainObject(e) || e instanceof this.constructor ? o(e, n) : A.isString(e) && (e = e.trim()) && !w1(e) ? o(x1(e), n) : e != null && i(n, e, r), this
     }
     get(e, n) {
         if (e = Is(e), e) {
             const r = A.findKey(this, e);
             if (r) {
                 const s = this[r];
                 if (!n) return s;
-                if (n === !0) return v1(s);
+                if (n === !0) return k1(s);
                 if (A.isFunction(n)) return n.call(this, s, r);
                 if (A.isRegExp(n)) return n.exec(s);
                 throw new TypeError("parser must be boolean|regexp|function")
             }
         }
     }
     has(e, n) {
@@ -5969,19 +5972,19 @@
     }
     normalize(e) {
         const n = this,
             r = {};
         return A.forEach(this, (s, i) => {
             const o = A.findKey(r, i);
             if (o) {
-                n[o] = Wi(s), delete n[i];
+                n[o] = Ki(s), delete n[i];
                 return
             }
-            const l = e ? k1(i) : String(i).trim();
-            l !== i && delete n[i], n[l] = Wi(s), r[l] = !0
+            const l = e ? S1(i) : String(i).trim();
+            l !== i && delete n[i], n[l] = Ki(s), r[l] = !0
         }), this
     }
     concat(...e) {
         return this.constructor.concat(this, ...e)
     }
     toJSON(e) {
         const n = Object.create(null);
@@ -6009,15 +6012,15 @@
         const r = (this[id] = this[id] = {
                 accessors: {}
             }).accessors,
             s = this.prototype;
 
         function i(o) {
             const l = Is(o);
-            r[l] || (w1(s, o), r[l] = !0)
+            r[l] || (_1(s, o), r[l] = !0)
         }
         return A.isArray(e) ? e.forEach(i) : i(e), this
     }
 }
 Jo.accessor(["Content-Type", "Content-Length", "Accept", "Accept-Encoding", "User-Agent", "Authorization"]);
 A.freezeMethods(Jo.prototype);
 A.freezeMethods(Jo);
@@ -6033,26 +6036,26 @@
     }), s.normalize(), i
 }
 
 function ap(t) {
     return !!(t && t.__CANCEL__)
 }
 
-function ki(t, e, n) {
+function Si(t, e, n) {
     Ce.call(this, t ?? "canceled", Ce.ERR_CANCELED, e, n), this.name = "CanceledError"
 }
-A.inherits(ki, Ce, {
+A.inherits(Si, Ce, {
     __CANCEL__: !0
 });
 
-function S1(t, e, n) {
+function C1(t, e, n) {
     const r = n.config.validateStatus;
     !n.status || !r || r(n.status) ? t(n) : e(new Ce("Request failed with status code " + n.status, [Ce.ERR_BAD_REQUEST, Ce.ERR_BAD_RESPONSE][Math.floor(n.status / 100) - 4], n.config, n.request, n))
 }
-const _1 = fn.isStandardBrowserEnv ? function() {
+const E1 = fn.isStandardBrowserEnv ? function() {
     return {
         write: function(n, r, s, i, o, l) {
             const a = [];
             a.push(n + "=" + encodeURIComponent(r)), A.isNumber(s) && a.push("expires=" + new Date(s).toGMTString()), A.isString(i) && a.push("path=" + i), A.isString(o) && a.push("domain=" + o), l === !0 && a.push("secure"), document.cookie = a.join("; ")
         },
         read: function(n) {
             const r = document.cookie.match(new RegExp("(^|;\\s*)(" + n + ")=([^;]*)"));
@@ -6068,26 +6071,26 @@
         read: function() {
             return null
         },
         remove: function() {}
     }
 }();
 
-function C1(t) {
+function T1(t) {
     return /^([a-z][a-z\d+\-.]*:)?\/\//i.test(t)
 }
 
-function E1(t, e) {
+function O1(t, e) {
     return e ? t.replace(/\/+$/, "") + "/" + e.replace(/^\/+/, "") : t
 }
 
 function cp(t, e) {
-    return t && !C1(e) ? E1(t, e) : e
+    return t && !T1(e) ? O1(t, e) : e
 }
-const T1 = fn.isStandardBrowserEnv ? function() {
+const M1 = fn.isStandardBrowserEnv ? function() {
     const e = /(msie|trident)/i.test(navigator.userAgent),
         n = document.createElement("a");
     let r;
 
     function s(i) {
         let o = i;
         return e && (n.setAttribute("href", o), o = n.href), n.setAttribute("href", o), {
@@ -6108,20 +6111,20 @@
         }
 }() : function() {
     return function() {
         return !0
     }
 }();
 
-function O1(t) {
+function A1(t) {
     const e = /^([-+\w]{1,25})(:?\/\/|:)/.exec(t);
     return e && e[1] || ""
 }
 
-function M1(t, e) {
+function N1(t, e) {
     t = t || 10;
     const n = new Array(t),
         r = new Array(t);
     let s = 0,
         i = 0,
         o;
     return e = e !== void 0 ? e : 1e3,
@@ -6136,15 +6139,15 @@
             const h = u && c - u;
             return h ? Math.round(f * 1e3 / h) : void 0
         }
 }
 
 function od(t, e) {
     let n = 0;
-    const r = M1(50, 250);
+    const r = N1(50, 250);
     return s => {
         const i = s.loaded,
             o = s.lengthComputable ? s.total : void 0,
             l = i - n,
             a = r(l),
             c = i <= o;
         n = i;
@@ -6156,16 +6159,16 @@
             rate: a || void 0,
             estimated: a && o && c ? (o - i) / a : void 0,
             event: s
         };
         u[e ? "download" : "upload"] = !0, t(u)
     }
 }
-const A1 = typeof XMLHttpRequest < "u",
-    N1 = A1 && function(t) {
+const R1 = typeof XMLHttpRequest < "u",
+    D1 = R1 && function(t) {
         return new Promise(function(n, r) {
             let s = t.data;
             const i = Mn.from(t.headers).normalize(),
                 o = t.responseType;
             let l;
 
             function a() {
@@ -6188,15 +6191,15 @@
                         data: !o || o === "text" || o === "json" ? c.responseText : c.response,
                         status: c.status,
                         statusText: c.statusText,
                         headers: h,
                         config: t,
                         request: c
                     };
-                S1(function(x) {
+                C1(function(x) {
                     n(x), a()
                 }, function(x) {
                     r(x), a()
                 }, g), c = null
             }
             if ("onloadend" in c ? c.onloadend = d : c.onreadystatechange = function() {
                     !c || c.readyState !== 4 || c.status === 0 && !(c.responseURL && c.responseURL.indexOf("file:") === 0) || setTimeout(d)
@@ -6205,67 +6208,67 @@
                 }, c.onerror = function() {
                     r(new Ce("Network Error", Ce.ERR_NETWORK, t, c)), c = null
                 }, c.ontimeout = function() {
                     let p = t.timeout ? "timeout of " + t.timeout + "ms exceeded" : "timeout exceeded";
                     const g = t.transitional || op;
                     t.timeoutErrorMessage && (p = t.timeoutErrorMessage), r(new Ce(p, g.clarifyTimeoutError ? Ce.ETIMEDOUT : Ce.ECONNABORTED, t, c)), c = null
                 }, fn.isStandardBrowserEnv) {
-                const h = (t.withCredentials || T1(u)) && t.xsrfCookieName && _1.read(t.xsrfCookieName);
+                const h = (t.withCredentials || M1(u)) && t.xsrfCookieName && E1.read(t.xsrfCookieName);
                 h && i.set(t.xsrfHeaderName, h)
             }
             s === void 0 && i.setContentType(null), "setRequestHeader" in c && A.forEach(i.toJSON(), function(p, g) {
                 c.setRequestHeader(g, p)
             }), A.isUndefined(t.withCredentials) || (c.withCredentials = !!t.withCredentials), o && o !== "json" && (c.responseType = t.responseType), typeof t.onDownloadProgress == "function" && c.addEventListener("progress", od(t.onDownloadProgress, !0)), typeof t.onUploadProgress == "function" && c.upload && c.upload.addEventListener("progress", od(t.onUploadProgress)), (t.cancelToken || t.signal) && (l = h => {
-                c && (r(!h || h.type ? new ki(null, t, c) : h), c.abort(), c = null)
+                c && (r(!h || h.type ? new Si(null, t, c) : h), c.abort(), c = null)
             }, t.cancelToken && t.cancelToken.subscribe(l), t.signal && (t.signal.aborted ? l() : t.signal.addEventListener("abort", l)));
-            const f = O1(u);
+            const f = A1(u);
             if (f && fn.protocols.indexOf(f) === -1) {
                 r(new Ce("Unsupported protocol " + f + ":", Ce.ERR_BAD_REQUEST, t));
                 return
             }
             c.send(s || null)
         })
     },
-    qi = {
-        http: n1,
-        xhr: N1
+    Ji = {
+        http: s1,
+        xhr: D1
     };
-A.forEach(qi, (t, e) => {
+A.forEach(Ji, (t, e) => {
     if (t) {
         try {
             Object.defineProperty(t, "name", {
                 value: e
             })
         } catch {}
         Object.defineProperty(t, "adapterName", {
             value: e
         })
     }
 });
-const R1 = {
+const I1 = {
     getAdapter: t => {
         t = A.isArray(t) ? t : [t];
         const {
             length: e
         } = t;
         let n, r;
-        for (let s = 0; s < e && (n = t[s], !(r = A.isString(n) ? qi[n.toLowerCase()] : n)); s++);
-        if (!r) throw r === !1 ? new Ce(`Adapter ${n} is not supported by the environment`, "ERR_NOT_SUPPORT") : new Error(A.hasOwnProp(qi, n) ? `Adapter '${n}' is not available in the build` : `Unknown adapter '${n}'`);
+        for (let s = 0; s < e && (n = t[s], !(r = A.isString(n) ? Ji[n.toLowerCase()] : n)); s++);
+        if (!r) throw r === !1 ? new Ce(`Adapter ${n} is not supported by the environment`, "ERR_NOT_SUPPORT") : new Error(A.hasOwnProp(Ji, n) ? `Adapter '${n}' is not available in the build` : `Unknown adapter '${n}'`);
         if (!A.isFunction(r)) throw new TypeError("adapter is not a function");
         return r
     },
-    adapters: qi
+    adapters: Ji
 };
 
 function Nl(t) {
-    if (t.cancelToken && t.cancelToken.throwIfRequested(), t.signal && t.signal.aborted) throw new ki(null, t)
+    if (t.cancelToken && t.cancelToken.throwIfRequested(), t.signal && t.signal.aborted) throw new Si(null, t)
 }
 
 function ld(t) {
-    return Nl(t), t.headers = Mn.from(t.headers), t.data = Al.call(t, t.transformRequest), ["post", "put", "patch"].indexOf(t.method) !== -1 && t.headers.setContentType("application/x-www-form-urlencoded", !1), R1.getAdapter(t.adapter || Sc.adapter)(t).then(function(r) {
+    return Nl(t), t.headers = Mn.from(t.headers), t.data = Al.call(t, t.transformRequest), ["post", "put", "patch"].indexOf(t.method) !== -1 && t.headers.setContentType("application/x-www-form-urlencoded", !1), I1.getAdapter(t.adapter || Sc.adapter)(t).then(function(r) {
         return Nl(t), r.data = Al.call(t, t.transformResponse, r), r.headers = Mn.from(r.headers), r
     }, function(r) {
         return ap(r) || (Nl(t), r && r.response && (r.response.data = Al.call(t, t.transformResponse, r.response), r.response.headers = Mn.from(r.response.headers))), Promise.reject(r)
     })
 }
 const ad = t => t instanceof Mn ? t.toJSON() : t;
 
@@ -6349,15 +6352,15 @@
     }
     return (i, o, l) => {
         if (e === !1) throw new Ce(s(o, " has been removed" + (n ? " in " + n : "")), Ce.ERR_DEPRECATED);
         return n && !cd[o] && (cd[o] = !0, console.warn(s(o, " has been deprecated since v" + n + " and will be removed in the near future"))), e ? e(i, o, l) : !0
     }
 };
 
-function D1(t, e, n) {
+function P1(t, e, n) {
     if (typeof t != "object") throw new Ce("options must be an object", Ce.ERR_BAD_OPTION_VALUE);
     const r = Object.keys(t);
     let s = r.length;
     for (; s-- > 0;) {
         const i = r[s],
             o = e[i];
         if (o) {
@@ -6366,19 +6369,19 @@
             if (a !== !0) throw new Ce("option " + i + " must be " + a, Ce.ERR_BAD_OPTION_VALUE);
             continue
         }
         if (n !== !0) throw new Ce("Unknown option " + i, Ce.ERR_BAD_OPTION)
     }
 }
 const Ca = {
-        assertOptions: D1,
+        assertOptions: P1,
         validators: _c
     },
     Hn = Ca.validators;
-class oo {
+class ao {
     constructor(e) {
         this.defaults = e, this.interceptors = {
             request: new sd,
             response: new sd
         }
     }
     request(e, n) {
@@ -6441,15 +6444,15 @@
     getUri(e) {
         e = cs(this.defaults, e);
         const n = cp(e.baseURL, e.url);
         return ip(n, e.params, e.paramsSerializer)
     }
 }
 A.forEach(["delete", "get", "head", "options"], function(e) {
-    oo.prototype[e] = function(n, r) {
+    ao.prototype[e] = function(n, r) {
         return this.request(cs(r || {}, {
             method: e,
             url: n,
             data: (r || {}).data
         }))
     }
 });
@@ -6462,17 +6465,17 @@
                     "Content-Type": "multipart/form-data"
                 } : {},
                 url: i,
                 data: o
             }))
         }
     }
-    oo.prototype[e] = n(), oo.prototype[e + "Form"] = n(!0)
+    ao.prototype[e] = n(), ao.prototype[e + "Form"] = n(!0)
 });
-const Ki = oo;
+const Gi = ao;
 class Cc {
     constructor(e) {
         if (typeof e != "function") throw new TypeError("executor must be a function.");
         let n;
         this.promise = new Promise(function(i) {
             n = i
         });
@@ -6487,15 +6490,15 @@
             const o = new Promise(l => {
                 r.subscribe(l), i = l
             }).then(s);
             return o.cancel = function() {
                 r.unsubscribe(i)
             }, o
         }, e(function(i, o, l) {
-            r.reason || (r.reason = new ki(i, o, l), n(r.reason))
+            r.reason || (r.reason = new Si(i, o, l), n(r.reason))
         })
     }
     throwIfRequested() {
         if (this.reason) throw this.reason
     }
     subscribe(e) {
         if (this.reason) {
@@ -6515,23 +6518,23 @@
             token: new Cc(function(s) {
                 e = s
             }),
             cancel: e
         }
     }
 }
-const I1 = Cc;
+const $1 = Cc;
 
-function P1(t) {
+function L1(t) {
     return function(n) {
         return t.apply(null, n)
     }
 }
 
-function $1(t) {
+function F1(t) {
     return A.isObject(t) && t.isAxiosError === !0
 }
 const Ea = {
     Continue: 100,
     SwitchingProtocols: 101,
     Processing: 102,
     EarlyHints: 103,
@@ -6594,222 +6597,222 @@
     LoopDetected: 508,
     NotExtended: 510,
     NetworkAuthenticationRequired: 511
 };
 Object.entries(Ea).forEach(([t, e]) => {
     Ea[e] = t
 });
-const L1 = Ea;
+const B1 = Ea;
 
 function dp(t) {
-    const e = new Ki(t),
-        n = Kh(Ki.prototype.request, e);
-    return A.extend(n, Ki.prototype, e, {
+    const e = new Gi(t),
+        n = Kh(Gi.prototype.request, e);
+    return A.extend(n, Gi.prototype, e, {
         allOwnKeys: !0
     }), A.extend(n, e, null, {
         allOwnKeys: !0
     }), n.create = function(s) {
         return dp(cs(t, s))
     }, n
 }
 const Xe = dp(Sc);
-Xe.Axios = Ki;
-Xe.CanceledError = ki;
-Xe.CancelToken = I1;
+Xe.Axios = Gi;
+Xe.CanceledError = Si;
+Xe.CancelToken = $1;
 Xe.isCancel = ap;
 Xe.VERSION = up;
 Xe.toFormData = qo;
 Xe.AxiosError = Ce;
 Xe.Cancel = Xe.CanceledError;
 Xe.all = function(e) {
     return Promise.all(e)
 };
-Xe.spread = P1;
-Xe.isAxiosError = $1;
+Xe.spread = L1;
+Xe.isAxiosError = F1;
 Xe.mergeConfig = cs;
 Xe.AxiosHeaders = Mn;
 Xe.formToJSON = t => lp(A.isHTMLForm(t) ? new FormData(t) : t);
-Xe.HttpStatusCode = L1;
+Xe.HttpStatusCode = B1;
 Xe.default = Xe;
-const Le = Xe,
+const Fe = Xe,
     ke = {
-        HOST_URL: "/api",
+        HOST_URL: "http://localhost:8000/api",
         IMAGES_URL: "/images",
         methods: {
             replaceUnicode(t) {
                 return t.replaceAll("ě", "e").replaceAll("š", "s").replaceAll("č", "c").replaceAll("ř", "r").replaceAll("ž", "z").replaceAll("ý", "y").replaceAll("á", "a").replaceAll("é", "e").replaceAll("í", "i").replaceAll("ů", "u").replaceAll("ú", "u").replaceAll("ť", "t").replaceAll("ď", "d").replaceAll("ó", "o").replaceAll("ň", "n")
             }
         }
     };
-const F1 = {
+const H1 = {
         props: ["inputCategory"],
         data() {
             return {
                 availableTags: [],
                 createTagField: null,
                 postSuccess: null,
                 postError: null,
                 category: {
                     tags: []
                 }
             }
         },
         methods: {
             toggleTag(t) {
-                console.log(this.category.tags), this.category.tags.map(n => n.name).includes(t.name) ? this.category.tags = this.category.tags.filter(n => n.name != t.name) : this.category.tags.push(t)
+                this.category.tags.map(n => n.name).includes(t.name) ? this.category.tags = this.category.tags.filter(n => n.name != t.name) : this.category.tags.push(t)
             },
             getRootData() {
-                Le.get(`${ke.HOST_URL}/tags`).then(t => {
+                Fe.get(`${ke.HOST_URL}/tags`).then(t => {
                     t.status !== "success" && (this.availableTags = t.data)
-                }).catch(t => this.error = t), Le.get(`${ke.HOST_URL}/ingredients`).then(t => {
+                }).catch(t => this.error = t), Fe.get(`${ke.HOST_URL}/ingredients`).then(t => {
                     t.status !== "success" && (this.ingredients = t.data.map(e => e.name))
                 }).catch(t => this.error = t)
             },
             updateCategory(t) {
                 const e = `${ke.HOST_URL}/categories/${t}`,
                     n = {
                         headers: {
                             "Content-Type": "application/json"
                         }
                     };
-                Le.put(e, this.category, n).then(r => {
+                Fe.put(e, this.category, n).then(r => {
                     this.postSuccess = `${r.status} ${r.statusText}`, this.$emit("categoryPosted", r.data)
                 }).catch(r => {
                     this.postError = r
                 })
             },
             postCategory() {
                 if (this.category.id) return this.updateCategory(this.category.id);
                 const t = `${ke.HOST_URL}/categories`,
                     e = {
                         headers: {
                             "Content-Type": "application/json"
                         }
                     };
-                Le.post(t, this.category, e).then(n => {
+                Fe.post(t, this.category, e).then(n => {
                     this.postSuccess = `${n.status} ${n.statusText}`, this.$emit("categoryPosted", n.data)
                 }).catch(n => {
                     this.postError = n
                 })
             }
         },
         created() {
             this.inputCategory && (this.category = {
                 ...this.inputCategory
             }), this.getRootData()
         }
     },
-    B1 = {
+    z1 = {
         class: "field"
     },
-    H1 = {
+    V1 = {
         class: "control has-icons-left has-icons-right"
     },
-    z1 = m("span", {
+    j1 = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-heading"
     })], -1),
-    V1 = {
+    U1 = {
         key: 0,
         class: "icon is-small is-right"
     },
-    j1 = m("i", {
+    W1 = m("i", {
         class: "fas fa-check"
     }, null, -1),
-    U1 = [j1],
-    W1 = {
+    q1 = [W1],
+    K1 = {
         key: 0,
         class: "help is-danger"
     },
-    q1 = {
+    J1 = {
         class: "field"
     },
-    K1 = m("label", {
+    G1 = m("label", {
         class: "label"
     }, "Tags", -1),
-    J1 = {
+    Y1 = {
         key: 0,
         class: "message is-warning p-0"
     },
-    G1 = m("small", {
+    X1 = m("small", {
         class: "message-body p-2"
     }, "no tags created yet", -1),
-    Y1 = [G1],
-    X1 = {
+    Q1 = [X1],
+    Z1 = {
         class: "control"
     },
-    Q1 = ["onClick"],
-    Z1 = {
+    ex = ["onClick"],
+    tx = {
         class: "my-5"
     },
-    ex = {
+    nx = {
         class: "field is-grouped"
     },
-    tx = {
+    rx = {
         class: "control mr-1 is-expanded"
     },
-    nx = ["disabled"],
-    rx = m("i", {
+    sx = ["disabled"],
+    ix = m("i", {
         class: "fas fa-save"
     }, null, -1),
-    sx = m("span", {
+    ox = m("span", {
         class: "ml-2"
     }, "Save", -1),
-    ix = [rx, sx],
-    ox = {
+    lx = [ix, ox],
+    ax = {
         key: 0,
         class: "message is-success"
     },
-    lx = {
+    cx = {
         class: "message-body"
     },
-    ax = {
+    ux = {
         key: 1,
         class: "message is-danger"
     },
-    cx = {
+    dx = {
         class: "message-body"
     };
 
-function ux(t, e, n, r, s, i) {
-    return C(), R("div", null, [m("div", B1, [m("div", H1, [We(m("input", {
+function fx(t, e, n, r, s, i) {
+    return C(), R("div", null, [m("div", z1, [m("div", V1, [We(m("input", {
         "onUpdate:modelValue": e[0] || (e[0] = o => s.category.name = o),
-        class: he({
+        class: fe({
             input: !0,
             "is-success": s.category.name,
             "is-danger": !s.category.name
         }),
         type: "text",
         placeholder: "Name"
     }, null, 2), [
         [st, s.category.name]
-    ]), z1, s.category.title ? (C(), R("span", V1, U1)) : re("", !0)]), s.category.name ? re("", !0) : (C(), R("p", W1, "Name is required"))]), m("div", q1, [K1, s.availableTags.length < 1 ? (C(), R("article", J1, Y1)) : re("", !0), m("div", X1, [m("div", null, [(C(!0), R(Fe, null, Dt(s.availableTags, (o, l) => (C(), R("a", {
+    ]), j1, s.category.title ? (C(), R("span", U1, q1)) : re("", !0)]), s.category.name ? re("", !0) : (C(), R("p", K1, "Name is required"))]), m("div", J1, [G1, s.availableTags.length < 1 ? (C(), R("article", Y1, Q1)) : re("", !0), m("div", Z1, [m("div", null, [(C(!0), R(Le, null, Dt(s.availableTags, (o, l) => (C(), R("a", {
         key: o + l,
         onClick: a => i.toggleTag(o)
     }, [m("span", {
-        class: he({
+        class: fe({
             tag: !0,
             "is-dark": s.category.tags && s.category.tags.map(a => a.name).includes(o.name),
             "is-rounded": !0,
             "mr-1": !0
         })
-    }, le(o.name), 3)], 8, Q1))), 128))])])]), m("div", Z1, [m("div", ex, [m("p", tx, [m("button", {
+    }, le(o.name), 3)], 8, ex))), 128))])])]), m("div", tx, [m("div", nx, [m("p", rx, [m("button", {
         class: "button is-success mr-1",
         disabled: !s.category.name,
         onClick: e[1] || (e[1] = (...o) => i.postCategory && i.postCategory(...o))
-    }, ix, 8, nx), m("button", {
+    }, lx, 8, sx), m("button", {
         class: "button",
         onClick: e[2] || (e[2] = o => t.$emit("cancel"))
-    }, "Cancel")])])]), s.postSuccess ? (C(), R("article", ox, [m("div", lx, le(s.postSuccess), 1)])) : re("", !0), s.postError ? (C(), R("article", ax, [m("div", cx, le(s.postError), 1)])) : re("", !0)])
+    }, "Cancel")])])]), s.postSuccess ? (C(), R("article", ax, [m("div", cx, le(s.postSuccess), 1)])) : re("", !0), s.postError ? (C(), R("article", ux, [m("div", dx, le(s.postError), 1)])) : re("", !0)])
 }
-const fp = Ue(F1, [
-        ["render", ux]
+const fp = Be(H1, [
+        ["render", fx]
     ]),
-    dx = {
+    hx = {
         props: ["recipe", "category", "small"],
         data() {
             return {
                 file: null,
                 error: null,
                 success: null,
                 loading: !1,
@@ -6819,166 +6822,166 @@
         methods: {
             handleFile() {
                 this.file = document.querySelector("#file").files[0]
             },
             upload() {
                 this.loading = !0;
                 var t = new FormData;
-                t.append("image", this.file), Le.post(this.url, t, {
+                t.append("image", this.file), Fe.post(this.url, t, {
                     headers: {
                         "Content-Type": "multipart/form-data"
                     }
                 }).then(e => {
                     this.success = e, this.error = null, this.$emit("uploadSuccess", e)
                 }).catch(e => {
                     this.success = null, this.error = e, this.$emit("uploadFailed", e)
                 }).finally(() => this.loading = !1)
             }
         },
         created() {
             this.category && (this.url = `${ke.HOST_URL}/images/categories/${this.category.id}`), this.recipe && (this.url = `${ke.HOST_URL}/images/recipes/${this.recipe.id}`)
         }
     },
-    fx = {
+    px = {
         key: 0
     },
-    hx = m("i", {
+    mx = m("i", {
         class: "fas fa-check"
     }, null, -1),
-    px = [hx],
-    mx = {
+    gx = [mx],
+    yx = {
         key: 1
     },
-    gx = m("i", {
+    bx = m("i", {
         class: "fas fa-upload"
     }, null, -1),
-    yx = [gx],
-    bx = m("span", null, [m("i", {
+    vx = [bx],
+    xx = m("span", null, [m("i", {
         class: "fas fa-upload"
     })], -1);
 
-function vx(t, e, n, r, s, i) {
-    return C(), R("div", null, [s.success ? (C(), R("div", fx, [m("button", {
-        class: he({
+function kx(t, e, n, r, s, i) {
+    return C(), R("div", null, [s.success ? (C(), R("div", px, [m("button", {
+        class: fe({
             button: !0,
             "is-success": !0,
             "is-small": n.small,
             "is-rounded": n.small
         }),
         disabled: ""
-    }, px, 2)])) : (C(), R("div", mx, [s.file ? (C(), R("button", {
+    }, gx, 2)])) : (C(), R("div", yx, [s.file ? (C(), R("button", {
         key: 0,
         onClick: e[0] || (e[0] = (...o) => i.upload && i.upload(...o)),
-        class: he({
+        class: fe({
             button: !0,
             "is-success": !0,
             "is-small": n.small,
             "is-rounded": n.small,
             "is-loading": s.loading
         })
-    }, yx, 2)) : (C(), R("button", {
+    }, vx, 2)) : (C(), R("button", {
         key: 1,
-        class: he({
+        class: fe({
             button: !0,
             file: !0,
             "is-info": !0,
             "is-rounded": n.small,
             "is-small": n.small
         })
-    }, [bx, m("input", {
+    }, [xx, m("input", {
         onChange: e[1] || (e[1] = (...o) => i.handleFile && i.handleFile(...o)),
         id: "file",
         class: "file-input",
         type: "file",
         name: "resume"
     }, null, 32)], 2))]))])
 }
-const hp = Ue(dx, [
-        ["render", vx]
+const hp = Be(hx, [
+        ["render", kx]
     ]),
-    xx = {
+    wx = {
         props: ["small", "rounded"],
         data() {
             return {
                 youSure: !1
             }
         }
     },
-    kx = {
+    Sx = {
         class: "ml-1"
     },
-    wx = m("i", {
+    _x = m("i", {
         class: "fas fa-trash"
     }, null, -1),
-    Sx = [wx],
-    _x = {
+    Cx = [_x],
+    Ex = {
         key: 1
     },
-    Cx = {
+    Tx = {
         class: "field has-addons"
     },
-    Ex = {
+    Ox = {
         class: "control"
     },
-    Tx = m("span", {
+    Mx = m("span", {
         class: "icon is-small"
     }, [m("i", {
         class: "fas fa-trash"
     })], -1),
-    Ox = [Tx],
-    Mx = {
+    Ax = [Mx],
+    Nx = {
         class: "control"
     },
-    Ax = m("span", {
+    Rx = m("span", {
         class: "icon is-small"
     }, [m("i", {
         class: "fas fa-times"
     })], -1),
-    Nx = [Ax];
+    Dx = [Rx];
 
-function Rx(t, e, n, r, s, i) {
-    return C(), R("div", kx, [ce(rn, {
+function Ix(t, e, n, r, s, i) {
+    return C(), R("div", Sx, [ce(rn, {
         name: "slide-up",
         mode: "out-in"
     }, {
-        default: ht(() => [s.youSure ? (C(), R("div", _x, [m("div", Cx, [m("p", Ex, [m("button", {
+        default: ht(() => [s.youSure ? (C(), R("div", Ex, [m("div", Tx, [m("p", Ox, [m("button", {
             onClick: e[1] || (e[1] = o => t.$emit("delete")),
-            class: he({
+            class: fe({
                 button: !0,
                 "is-danger": !0,
                 "is-small": n.small,
                 "is-rounded": n.rounded,
                 "clickable-link": !0
             })
-        }, Ox, 2)]), m("p", Mx, [m("button", {
+        }, Ax, 2)]), m("p", Nx, [m("button", {
             onClick: e[2] || (e[2] = o => s.youSure = !s.youSure),
-            class: he({
+            class: fe({
                 button: !0,
                 "is-small": n.small,
                 "is-rounded": n.rounded,
                 "clickable-link": !0
             })
-        }, Nx, 2)])])])) : (C(), R("button", {
+        }, Dx, 2)])])])) : (C(), R("button", {
             key: 0,
             onClick: e[0] || (e[0] = o => s.youSure = !s.youSure),
-            class: he({
+            class: fe({
                 button: !0,
                 "is-danger": !0,
                 "is-small": n.small,
                 "is-rounded": n.rounded,
                 "clickable-link": !0
             })
-        }, Sx, 2))]),
+        }, Cx, 2))]),
         _: 1
     })])
 }
-const pp = Ue(xx, [
-    ["render", Rx]
+const pp = Be(wx, [
+    ["render", Ix]
 ]);
-const Dx = {
+const Px = {
         data() {
             return {
                 edit: !1,
                 youSure: !1,
                 uploadError: null
             }
         },
@@ -6996,63 +6999,63 @@
                 this.editable || this.$emit("clicked", this.category)
             },
             edited() {
                 this.edit = !1, this.$emit("categoryEdited")
             },
             deleteCategory() {
                 const t = `${ke.HOST_URL}/categories/${this.category.id}`;
-                Le.delete(t).then(e => {
+                Fe.delete(t).then(e => {
                     this.$emit("categoryDeleted", e)
                 }).catch(e => {
                     this.postError = e
                 })
             },
             getRandomColor() {
                 for (var t = "012345html6789ABCDEF", e = "#", n = 0; n < 6; n++) e += t[Math.floor(Math.random() * 16)];
                 return e
             },
             getTileStyle() {
                 return `background-image: url('${ke.IMAGES_URL}/categories/${this.category.id}/landscape.jpeg');`
             }
         }
     },
-    Ix = t => (Po("data-v-560fa5c2"), t = t(), $o(), t),
-    Px = {
+    $x = t => (xi("data-v-560fa5c2"), t = t(), ki(), t),
+    Lx = {
         class: "title tile-title"
     },
-    $x = {
+    Fx = {
         class: "tags my-0"
     },
-    Lx = {
+    Bx = {
         class: "level is-mobile mb-2"
     },
-    Fx = {
+    Hx = {
         key: 0,
         class: "level-item level-right"
     },
-    Bx = {
+    zx = {
         class: "control mr-1"
     },
-    Hx = {
+    Vx = {
         class: "mx-0"
     },
-    zx = Ix(() => m("i", {
+    jx = $x(() => m("i", {
         class: "fas fa-pen"
     }, null, -1)),
-    Vx = [zx],
-    jx = {
+    Ux = [jx],
+    Wx = {
         key: 0,
         class: "help is-danger"
     },
-    Ux = {
+    qx = {
         key: 1,
         class: "help is-danger"
     };
 
-function Wx(t, e, n, r, s, i) {
+function Kx(t, e, n, r, s, i) {
     const o = Oe("CategoryForm"),
         l = Oe("ImageUpload"),
         a = Oe("DeleteButton");
     return C(), R("div", null, [ce(rn, {
         name: "slide",
         mode: "out-in"
     }, {
@@ -7062,59 +7065,59 @@
             inputCategory: n.category,
             onCategoryPosted: i.edited,
             onCancel: e[0] || (e[0] = c => s.edit = !s.edit)
         }, null, 8, ["inputCategory", "onCategoryPosted"])) : (C(), R("a", {
             key: 1,
             onClick: e[3] || (e[3] = (...c) => i.clicked && i.clicked(...c)),
             class: "tile box is-child image-background clickable",
-            style: _o(i.getTileStyle())
-        }, [m("p", Px, le(n.category.name), 1), m("div", $x, [(C(!0), R(Fe, null, Dt(n.category.tags, (c, u) => (C(), R("span", {
+            style: Eo(i.getTileStyle())
+        }, [m("p", Lx, le(n.category.name), 1), m("div", Fx, [(C(!0), R(Le, null, Dt(n.category.tags, (c, u) => (C(), R("span", {
             class: "mytag",
             key: "category-tag-" + u
-        }, le(c.name), 1))), 128))]), m("div", Lx, [n.editable ? (C(), R("div", Fx, [m("p", Bx, [ce(l, {
+        }, le(c.name), 1))), 128))]), m("div", Bx, [n.editable ? (C(), R("div", Hx, [m("p", zx, [ce(l, {
             category: n.category,
             small: !0,
             onUploadFailed: i.imageUploadFailed,
             onUploadSuccess: i.edited
-        }, null, 8, ["category", "onUploadFailed", "onUploadSuccess"])]), m("div", Hx, [m("button", {
+        }, null, 8, ["category", "onUploadFailed", "onUploadSuccess"])]), m("div", Vx, [m("button", {
             onClick: e[1] || (e[1] = c => s.edit = !s.edit),
             class: "button is-warning is-small is-rounded"
-        }, Vx)]), ce(a, {
+        }, Ux)]), ce(a, {
             onDelete: i.deleteCategory,
             small: !0,
             rounded: !0
-        }, null, 8, ["onDelete"])])) : re("", !0)]), s.uploadError ? (C(), R("span", jx, " Upload failed... ")) : re("", !0), s.youSure ? (C(), R("span", Ux, [Ge(" You absolutely sure you want to delete this category? "), m("a", {
+        }, null, 8, ["onDelete"])])) : re("", !0)]), s.uploadError ? (C(), R("span", Wx, " Upload failed... ")) : re("", !0), s.youSure ? (C(), R("span", qx, [Ge(" You absolutely sure you want to delete this category? "), m("a", {
             onClick: e[2] || (e[2] = (...c) => i.deleteCategory && i.deleteCategory(...c))
         }, "Yep, let's do this!")])) : re("", !0)], 4))]),
         _: 1
     })])
 }
-const mp = Ue(Dx, [
-    ["render", Wx],
+const mp = Be(Px, [
+    ["render", Kx],
     ["__scopeId", "data-v-560fa5c2"]
 ]);
-const qx = {
+const Jx = {
         props: ["loading"]
     },
-    Kx = {
+    Gx = {
         class: "section has-text-centered py-0"
     },
-    Jx = {
+    Yx = {
         key: 0,
         class: "loading-btn button is-loading p-0",
         disabled: ""
     };
 
-function Gx(t, e, n, r, s, i) {
-    return C(), R("section", Kx, [n.loading ? (C(), R("button", Jx, "X")) : re("", !0)])
+function Xx(t, e, n, r, s, i) {
+    return C(), R("section", Gx, [n.loading ? (C(), R("button", Yx, "X")) : re("", !0)])
 }
-const Go = Ue(qx, [
-    ["render", Gx]
+const Go = Be(Jx, [
+    ["render", Xx]
 ]);
-const Yx = {
+const Qx = {
         props: ["recipe"],
         data() {
             return {
                 imageFailedToLoad: !1
             }
         },
         methods: {
@@ -7128,91 +7131,91 @@
                     t.target.src = "";
                     return
                 }
                 this.imageFailedToLoad = !0, t.target.src = `${ke.IMAGES_URL}/not-found.png`
             }
         }
     },
-    Xx = t => (Po("data-v-d10c6c84"), t = t(), $o(), t),
-    Qx = {
+    Zx = t => (xi("data-v-d10c6c84"), t = t(), ki(), t),
+    ek = {
         class: "media box boxhov p-0"
     },
-    Zx = {
+    tk = {
         class: "media-left m-0"
     },
-    ek = {
+    nk = {
         class: "image is-96x96",
         style: {
             display: "flex"
         }
     },
-    tk = ["src"],
-    nk = {
+    rk = ["src"],
+    sk = {
         class: "media-content p-3"
     },
-    rk = {
+    ik = {
         class: "content"
     },
-    sk = {
+    ok = {
         class: "title is-5"
     },
-    ik = Xx(() => m("br", null, null, -1)),
-    ok = {
+    lk = Zx(() => m("br", null, null, -1)),
+    ak = {
         key: 0,
         style: {
             color: "gray"
         }
     },
-    lk = {
+    ck = {
         class: "level"
     },
-    ak = {
+    uk = {
         class: "level-left"
     },
-    ck = {
+    dk = {
         class: "tags my-0"
     };
 
-function uk(t, e, n, r, s, i) {
+function fk(t, e, n, r, s, i) {
     const o = Oe("router-link");
     return C(), R("div", null, [ce(o, {
         to: {
             name: "recipe",
             params: {
                 id: n.recipe.id
             }
         }
     }, {
-        default: ht(() => [m("article", Qx, [m("figure", Zx, [m("p", ek, [m("img", {
+        default: ht(() => [m("article", ek, [m("figure", tk, [m("p", nk, [m("img", {
             ref: "r-img",
             src: i.getImageUrl(),
             alt: "recipe image",
             class: "is-rounded p-2"
-        }, null, 8, tk)])]), m("div", nk, [m("div", rk, [m("p", sk, [Ge(le(n.recipe.title) + " ", 1), ik, n.recipe.subtitle ? (C(), R("span", ok, [m("small", null, le(n.recipe.subtitle), 1)])) : re("", !0)])]), m("nav", lk, [m("div", ak, [m("div", ck, [(C(!0), R(Fe, null, Dt(n.recipe.tags, (l, a) => (C(), R("span", {
+        }, null, 8, rk)])]), m("div", sk, [m("div", ik, [m("p", ok, [Ge(le(n.recipe.title) + " ", 1), lk, n.recipe.subtitle ? (C(), R("span", ak, [m("small", null, le(n.recipe.subtitle), 1)])) : re("", !0)])]), m("nav", ck, [m("div", uk, [m("div", dk, [(C(!0), R(Le, null, Dt(n.recipe.tags, (l, a) => (C(), R("span", {
             class: "tag is-rounded",
             key: "item-tag-" + a
         }, le(l.name), 1))), 128))])])])])])]),
         _: 1
     }, 8, ["to"])])
 }
-const dk = Ue(Yx, [
-    ["render", uk],
+const hk = Be(Qx, [
+    ["render", fk],
     ["__scopeId", "data-v-d10c6c84"]
 ]);
-const fk = {
+const pk = {
         props: ["allRecipes", "title", "hideSearch", "hideFilters"],
         data() {
             return {
                 activeTags: [],
                 search: null,
                 recipesInitiated: !1
             }
         },
         components: {
-            RecipeListItem: dk
+            RecipeListItem: hk
         },
         computed: {
             tags() {
                 return new Set(this.allRecipes.map(t => t.tags.map(e => e.name)).flat())
             },
             recipes() {
                 this.recipesInitiated = !0;
@@ -7235,190 +7238,190 @@
         },
         methods: {
             toggleFilter(t) {
                 this.activeTags.includes(t) ? this.activeTags = this.activeTags.filter(e => e != t) : this.activeTags.push(t)
             }
         }
     },
-    hk = t => (Po("data-v-67602aa9"), t = t(), $o(), t),
-    pk = {
+    mk = t => (xi("data-v-67602aa9"), t = t(), ki(), t),
+    gk = {
         class: "mb-2"
     },
-    mk = {
+    yk = {
         class: "title is-4 has-text-primary"
     },
-    gk = {
+    bk = {
         key: 0,
         class: "tags"
     },
-    yk = ["onClick"],
-    bk = {
+    vk = ["onClick"],
+    xk = {
         key: 1,
         class: "control has-icons-left mb-4"
     },
-    vk = hk(() => m("span", {
+    kk = mk(() => m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-search"
     })], -1)),
-    xk = {
+    wk = {
         class: "recipe-list"
     };
 
-function kk(t, e, n, r, s, i) {
+function Sk(t, e, n, r, s, i) {
     const o = Oe("RecipeListItem");
-    return C(), R("div", null, [m("div", pk, [m("h1", mk, le(i.recipes.length) + " " + le(n.title || "Recipes"), 1)]), n.hideFilters ? re("", !0) : (C(), R("div", gk, [(C(!0), R(Fe, null, Dt(i.tags, l => (C(), R("a", {
+    return C(), R("div", null, [m("div", gk, [m("h1", yk, le(i.recipes.length) + " " + le(n.title || "Recipes"), 1)]), n.hideFilters ? re("", !0) : (C(), R("div", bk, [(C(!0), R(Le, null, Dt(i.tags, l => (C(), R("a", {
         key: "tag_key" + l,
         onClick: a => i.toggleFilter(l),
-        class: he({
+        class: fe({
             tag: !0,
             "is-rounded": !0,
             "is-dark": s.activeTags.includes(l),
             noselect: !0
         }),
         style: {
             "text-decoration": "none"
         }
-    }, le(l), 11, yk))), 128))])), n.hideSearch ? re("", !0) : (C(), R("p", bk, [We(m("input", {
+    }, le(l), 11, vk))), 128))])), n.hideSearch ? re("", !0) : (C(), R("p", xk, [We(m("input", {
         "onUpdate:modelValue": e[0] || (e[0] = l => s.search = l),
         onInput: e[1] || (e[1] = (...l) => t.refresh && t.refresh(...l)),
         class: "input is-rounded",
         type: "text",
         placeholder: "search"
     }, null, 544), [
         [st, s.search]
-    ]), vk])), m("div", xk, [(C(!0), R(Fe, null, Dt(i.recipes, l => (C(), yt(o, {
+    ]), kk])), m("div", wk, [(C(!0), R(Le, null, Dt(i.recipes, l => (C(), yt(o, {
         key: "recipe_a_key+" + l.id,
         recipe: l
     }, null, 8, ["recipe"]))), 128))])])
 }
-const Ec = Ue(fk, [
-    ["render", kk],
+const Ec = Be(pk, [
+    ["render", Sk],
     ["__scopeId", "data-v-67602aa9"]
 ]);
-const wk = {
+const _k = {
         components: {
             CategoryTile: mp,
             LoadingSection: Go,
             RecipeList: Ec
         },
         data() {
             return {
                 error: null,
                 columns: 3,
                 categories: [],
                 newCategory: !1,
                 loading: !1,
-                current_recipes: []
+                favorites: []
             }
         },
         methods: {
             getAllCategories() {
                 this.loading = !0;
                 const t = `${ke.HOST_URL}/categories`;
-                Le.get(t).then(e => {
+                Fe.get(t).then(e => {
                     e.status !== "success" && (e.data ? (this.categories = e.data, this.$route.query.category && this.selectCategoryByName(this.$route.query.category)) : this.error = "No categories received.")
                 }).catch(e => this.error = e).finally(() => this.loading = !1)
             },
-            getCurrent() {
+            getFavoriteRecipes() {
                 this.loading = !0;
-                const t = `${ke.HOST_URL}/recipes/current`;
-                Le.get(t).then(e => this.current_recipes = e.data).catch(e => this.error = e).finally(() => this.loading = !1)
+                const t = `${ke.HOST_URL}/recipes?favorite=true`;
+                Fe.get(t).then(e => this.favorites = e.data).catch(e => this.error = e).finally(() => this.loading = !1)
             }
         },
         created() {
-            this.getAllCategories(), this.getCurrent()
+            this.getAllCategories(), this.getFavoriteRecipes()
         }
     },
-    Sk = {
+    Ck = {
         key: 1
     },
-    _k = {
+    Ek = {
         class: "category-tiles"
     };
 
-function Ck(t, e, n, r, s, i) {
+function Tk(t, e, n, r, s, i) {
     const o = Oe("LoadingSection"),
         l = Oe("RecipeList"),
         a = Oe("CategoryTile");
     return C(), R("div", null, [ce(rn, {
         name: "loading",
         mode: "out-in"
     }, {
         default: ht(() => [s.loading ? (C(), yt(o, {
             key: 0,
             loading: s.loading
-        }, null, 8, ["loading"])) : (C(), R("div", Sk, [s.current_recipes.length > 0 ? (C(), yt(l, {
+        }, null, 8, ["loading"])) : (C(), R("div", Ck, [s.favorites.length > 0 ? (C(), yt(l, {
             key: 0,
             class: "mb-4 mt-5",
-            allRecipes: s.current_recipes,
+            allRecipes: s.favorites,
             hideSearch: !0,
             hideFilters: !0,
-            title: "Planned"
-        }, null, 8, ["allRecipes"])) : re("", !0), m("div", _k, [(C(!0), R(Fe, null, Dt(s.categories, c => (C(), yt(a, {
+            title: "favorite recipes"
+        }, null, 8, ["allRecipes"])) : re("", !0), m("div", Ek, [(C(!0), R(Le, null, Dt(s.categories, c => (C(), yt(a, {
             category: c,
             onClicked: u => t.$router.push({
                 name: "category",
                 params: {
                     id: c.id
                 }
             })
         }, null, 8, ["category", "onClicked"]))), 256))])]))]),
         _: 1
     })])
 }
-const Ek = Ue(wk, [
-        ["render", Ck],
-        ["__scopeId", "data-v-0ca6dc2c"]
+const Ok = Be(_k, [
+        ["render", Tk],
+        ["__scopeId", "data-v-11dd16dd"]
     ]),
-    Tk = {
+    Mk = {
         data() {
             return {
                 recipes: [],
                 loading: !1,
                 error: null
             }
         },
         components: {
             RecipeList: Ec,
             LoadingSection: Go
         },
         created() {
             this.loading = !0;
             const t = `${ke.HOST_URL}/recipes`;
-            Le.get(t).then(e => {
+            Fe.get(t).then(e => {
                 e.status !== "success" && (e.data ? this.recipes = e.data.sort((n, r) => n.name > r.name) : this.error = "No recipes received.")
             }).catch(e => this.error = e).finally(() => this.loading = !1)
         }
     },
-    Ok = {
+    Ak = {
         class: "recipes px-3"
     };
 
-function Mk(t, e, n, r, s, i) {
+function Nk(t, e, n, r, s, i) {
     const o = Oe("LoadingSection"),
         l = Oe("RecipeList");
-    return C(), R("div", Ok, [ce(rn, {
+    return C(), R("div", Ak, [ce(rn, {
         name: "loading",
         mode: "out-in"
     }, {
         default: ht(() => [s.loading ? (C(), yt(o, {
             key: 0,
             loading: s.loading
         }, null, 8, ["loading"])) : (C(), yt(l, {
             key: 1,
             allRecipes: s.recipes
         }, null, 8, ["allRecipes"]))]),
         _: 1
     })])
 }
-const Ak = Ue(Tk, [
-        ["render", Mk]
+const Rk = Be(Mk, [
+        ["render", Nk]
     ]),
-    Nk = {
+    Dk = {
         props: ["initialValue"],
         data() {
             return {
                 counter: 4
             }
         },
         methods: {
@@ -7429,57 +7432,57 @@
                 this.counter != 0 && this.$emit("counterUpdate", --this.counter)
             }
         },
         created() {
             this.initialValue && (this.counter = this.initialValue)
         }
     },
-    Rk = {
+    Ik = {
         class: "field has-addons"
     },
-    Dk = {
+    Pk = {
         class: "control"
     },
-    Ik = m("span", {
+    $k = m("span", {
         class: "icon is-small"
     }, [m("i", {
         class: "fas fa-minus"
     })], -1),
-    Pk = [Ik],
-    $k = {
+    Lk = [$k],
+    Fk = {
         class: "control is-expanded"
     },
-    Lk = {
+    Bk = {
         class: "control"
     },
-    Fk = m("span", {
+    Hk = m("span", {
         class: "icon is-small"
     }, [m("i", {
         class: "fas fa-plus"
     })], -1),
-    Bk = [Fk];
+    zk = [Hk];
 
-function Hk(t, e, n, r, s, i) {
-    return C(), R("div", Rk, [m("p", Dk, [m("a", {
+function Vk(t, e, n, r, s, i) {
+    return C(), R("div", Ik, [m("p", Pk, [m("a", {
         class: "button is-small",
         onClick: e[0] || (e[0] = (...o) => i.decrement && i.decrement(...o))
-    }, Pk)]), m("p", $k, [We(m("input", {
+    }, Lk)]), m("p", Fk, [We(m("input", {
         class: "input has-text-centered is-small",
         type: "text",
         "onUpdate:modelValue": e[1] || (e[1] = o => s.counter = o),
         disabled: ""
     }, null, 512), [
         [st, s.counter]
-    ])]), m("p", Lk, [m("a", {
+    ])]), m("p", Bk, [m("a", {
         class: "button is-small",
         onClick: e[2] || (e[2] = (...o) => i.increment && i.increment(...o))
-    }, Bk)])])
+    }, zk)])])
 }
-const gp = Ue(Nk, [
-    ["render", Hk]
+const gp = Be(Dk, [
+    ["render", Vk]
 ]);
 
 function nt(t) {
     this.content = t
 }
 nt.prototype = {
     constructor: nt,
@@ -7701,21 +7704,21 @@
     findDiffStart(e, n = 0) {
         return yp(this, e, n)
     }
     findDiffEnd(e, n = this.size, r = e.size) {
         return bp(this, e, n, r)
     }
     findIndex(e, n = -1) {
-        if (e == 0) return Pi(0, e);
-        if (e == this.size) return Pi(this.content.length, e);
+        if (e == 0) return Li(0, e);
+        if (e == this.size) return Li(this.content.length, e);
         if (e > this.size || e < 0) throw new RangeError(`Position ${e} outside of fragment (${this})`);
         for (let r = 0, s = 0;; r++) {
             let i = this.child(r),
                 o = s + i.nodeSize;
-            if (o >= e) return o == e || n > 0 ? Pi(r + 1, o) : Pi(r, s);
+            if (o >= e) return o == e || n > 0 ? Li(r + 1, o) : Li(r, s);
             s = o
         }
     }
     toString() {
         return "<" + this.toStringInner() + ">"
     }
     toStringInner() {
@@ -7748,30 +7751,30 @@
 }
 $.empty = new $([], 0);
 const Rl = {
     index: 0,
     offset: 0
 };
 
-function Pi(t, e) {
+function Li(t, e) {
     return Rl.index = t, Rl.offset = e, Rl
 }
 
-function lo(t, e) {
+function co(t, e) {
     if (t === e) return !0;
     if (!(t && typeof t == "object") || !(e && typeof e == "object")) return !1;
     let n = Array.isArray(t);
     if (Array.isArray(e) != n) return !1;
     if (n) {
         if (t.length != e.length) return !1;
         for (let r = 0; r < t.length; r++)
-            if (!lo(t[r], e[r])) return !1
+            if (!co(t[r], e[r])) return !1
     } else {
         for (let r in t)
-            if (!(r in e) || !lo(t[r], e[r])) return !1;
+            if (!(r in e) || !co(t[r], e[r])) return !1;
         for (let r in e)
             if (!(r in t)) return !1
     }
     return !0
 }
 let De = class Ta {
     constructor(e, n) {
@@ -7797,15 +7800,15 @@
     }
     isInSet(e) {
         for (let n = 0; n < e.length; n++)
             if (this.eq(e[n])) return !0;
         return !1
     }
     eq(e) {
-        return this == e || this.type == e.type && lo(this.attrs, e.attrs)
+        return this == e || this.type == e.type && co(this.attrs, e.attrs)
     }
     toJSON() {
         let e = {
             type: this.type.name
         };
         for (let n in this.attrs) {
             e.attrs = this.attrs;
@@ -7830,15 +7833,15 @@
         if (!e || Array.isArray(e) && e.length == 0) return Ta.none;
         if (e instanceof Ta) return [e];
         let n = e.slice();
         return n.sort((r, s) => r.type.rank - s.type.rank), n
     }
 };
 De.none = [];
-class ao extends Error {}
+class uo extends Error {}
 class q {
     constructor(e, n, r) {
         this.content = e, this.openStart = n, this.openEnd = r
     }
     get size() {
         return this.content.size - this.openStart - this.openEnd
     }
@@ -7901,17 +7904,17 @@
         offset: i
     } = t.findIndex(e), o = t.maybeChild(s);
     if (i == e || o.isText) return r && !r.canReplace(s, s, n) ? null : t.cut(0, e).append(n).append(t.cut(e));
     let l = xp(o.content, e - i - 1, n);
     return l && t.replaceChild(s, o.copy(l))
 }
 
-function zk(t, e, n) {
-    if (n.openStart > t.depth) throw new ao("Inserted content deeper than insertion position");
-    if (t.depth - n.openStart != e.depth - n.openEnd) throw new ao("Inconsistent open depths");
+function jk(t, e, n) {
+    if (n.openStart > t.depth) throw new uo("Inserted content deeper than insertion position");
+    if (t.depth - n.openStart != e.depth - n.openEnd) throw new uo("Inconsistent open depths");
     return kp(t, e, n, 0)
 }
 
 function kp(t, e, n, r) {
     let s = t.index(r),
         i = t.node(r);
     if (s == e.index(r) && r < t.depth - n.openStart) {
@@ -7922,22 +7925,22 @@
             let o = t.parent,
                 l = o.content;
             return Ar(o, l.cut(0, t.parentOffset).append(n.content).append(l.cut(e.parentOffset)))
         } else {
             let {
                 start: o,
                 end: l
-            } = Vk(n, t);
+            } = Uk(n, t);
             return Ar(i, Sp(t, o, l, e, r))
         }
-    else return Ar(i, co(t, e, r))
+    else return Ar(i, fo(t, e, r))
 }
 
 function wp(t, e) {
-    if (!e.type.compatibleContent(t.type)) throw new ao("Cannot join " + e.type.name + " onto " + t.type.name)
+    if (!e.type.compatibleContent(t.type)) throw new uo("Cannot join " + e.type.name + " onto " + t.type.name)
 }
 
 function Oa(t, e, n) {
     let r = t.node(n);
     return wp(r, e.node(n)), r
 }
 
@@ -7959,27 +7962,27 @@
     return t.type.checkContent(e), t.copy(e)
 }
 
 function Sp(t, e, n, r, s) {
     let i = t.depth > s && Oa(t, e, s + 1),
         o = r.depth > s && Oa(n, r, s + 1),
         l = [];
-    return Ys(null, t, s, l), i && o && e.index(s) == n.index(s) ? (wp(i, o), Mr(Ar(i, Sp(t, e, n, r, s + 1)), l)) : (i && Mr(Ar(i, co(t, e, s + 1)), l), Ys(e, n, s, l), o && Mr(Ar(o, co(n, r, s + 1)), l)), Ys(r, null, s, l), new $(l)
+    return Ys(null, t, s, l), i && o && e.index(s) == n.index(s) ? (wp(i, o), Mr(Ar(i, Sp(t, e, n, r, s + 1)), l)) : (i && Mr(Ar(i, fo(t, e, s + 1)), l), Ys(e, n, s, l), o && Mr(Ar(o, fo(n, r, s + 1)), l)), Ys(r, null, s, l), new $(l)
 }
 
-function co(t, e, n) {
+function fo(t, e, n) {
     let r = [];
     if (Ys(null, t, n, r), t.depth > n) {
         let s = Oa(t, e, n + 1);
-        Mr(Ar(s, co(t, e, n + 1)), r)
+        Mr(Ar(s, fo(t, e, n + 1)), r)
     }
     return Ys(e, null, n, r), new $(r)
 }
 
-function Vk(t, e) {
+function Uk(t, e) {
     let n = e.depth - t.openStart,
         s = e.node(n).copy(t.content);
     for (let i = n - 1; i >= 0; i--) s = e.node(i).copy($.from(s));
     return {
         start: s.resolveNoCache(t.openStart + n),
         end: s.resolveNoCache(s.content.size - t.openEnd - n)
     }
@@ -8070,15 +8073,15 @@
         for (let n = this.depth; n > 0; n--)
             if (this.start(n) <= e && this.end(n) >= e) return n;
         return 0
     }
     blockRange(e = this, n) {
         if (e.pos < this.pos) return e.blockRange(this);
         for (let r = this.depth - (this.parent.inlineContent || this.pos == e.pos ? 1 : 0); r >= 0; r--)
-            if (e.pos <= this.end(r) && (!n || n(this.node(r)))) return new uo(this, e, r);
+            if (e.pos <= this.end(r) && (!n || n(this.node(r)))) return new ho(this, e, r);
         return null
     }
     sameParent(e) {
         return this.pos - this.parentOffset == e.pos - e.parentOffset
     }
     max(e) {
         return e.pos > this.pos ? e : this
@@ -8108,21 +8111,21 @@
     }
     static resolveCached(e, n) {
         for (let s = 0; s < Dl.length; s++) {
             let i = Dl[s];
             if (i.pos == n && i.doc == e) return i
         }
         let r = Dl[Il] = fi.resolve(e, n);
-        return Il = (Il + 1) % jk, r
+        return Il = (Il + 1) % Wk, r
     }
 }
 let Dl = [],
     Il = 0,
-    jk = 12;
-class uo {
+    Wk = 12;
+class ho {
     constructor(e, n, r) {
         this.$from = e, this.$to = n, this.depth = r
     }
     get start() {
         return this.$from.before(this.depth + 1)
     }
     get end() {
@@ -8134,15 +8137,15 @@
     get startIndex() {
         return this.$from.index(this.depth)
     }
     get endIndex() {
         return this.$to.indexAfter(this.depth)
     }
 }
-const Uk = Object.create(null);
+const qk = Object.create(null);
 let Nr = class Ma {
     constructor(e, n, r, s = De.none) {
         this.type = e, this.attrs = n, this.marks = s, this.content = r || $.empty
     }
     get nodeSize() {
         return this.isLeaf ? 1 : 2 + this.content.size
     }
@@ -8179,15 +8182,15 @@
     eq(e) {
         return this == e || this.sameMarkup(e) && this.content.eq(e.content)
     }
     sameMarkup(e) {
         return this.hasMarkup(e.type, e.attrs, e.marks)
     }
     hasMarkup(e, n, r) {
-        return this.type == e && lo(this.attrs, n || e.defaultAttrs || Uk) && De.sameSet(this.marks, r || De.none)
+        return this.type == e && co(this.attrs, n || e.defaultAttrs || qk) && De.sameSet(this.marks, r || De.none)
     }
     copy(e = null) {
         return e == this.content ? this : new Ma(this.type, this.attrs, e, this.marks)
     }
     mark(e) {
         return e == this.marks ? this : new Ma(this.type, this.attrs, this.content, e)
     }
@@ -8200,15 +8203,15 @@
             i = this.resolve(n),
             o = r ? 0 : s.sharedDepth(n),
             l = s.start(o),
             c = s.node(o).content.cut(s.pos - l, i.pos - l);
         return new q(c, s.depth - o, i.depth - o)
     }
     replace(e, n, r) {
-        return zk(this.resolve(e), this.resolve(n), r)
+        return jk(this.resolve(e), this.resolve(n), r)
     }
     nodeAt(e) {
         for (let n = this;;) {
             let {
                 index: r,
                 offset: s
             } = n.content.findIndex(e);
@@ -8337,15 +8340,15 @@
             return e.text(n.text, r)
         }
         let s = $.fromJSON(e, n.content);
         return e.nodeType(n.type).create(n.attrs, s, r)
     }
 };
 Nr.prototype.text = void 0;
-class fo extends Nr {
+class po extends Nr {
     constructor(e, n, r, s) {
         if (super(e, n, null, s), !r) throw new RangeError("Empty text nodes are not allowed");
         this.text = r
     }
     toString() {
         return this.type.spec.toDebugString ? this.type.spec.toDebugString(this) : _p(this.marks, JSON.stringify(this.text))
     }
@@ -8355,18 +8358,18 @@
     textBetween(e, n) {
         return this.text.slice(e, n)
     }
     get nodeSize() {
         return this.text.length
     }
     mark(e) {
-        return e == this.marks ? this : new fo(this.type, this.attrs, this.text, e)
+        return e == this.marks ? this : new po(this.type, this.attrs, this.text, e)
     }
     withText(e) {
-        return e == this.text ? this : new fo(this.type, this.attrs, e, this.marks)
+        return e == this.text ? this : new po(this.type, this.attrs, e, this.marks)
     }
     cut(e = 0, n = this.text.length) {
         return e == 0 && n == this.text.length ? this : this.withText(this.text.slice(e, n))
     }
     eq(e) {
         return this.sameMarkup(e) && this.text == e.text
     }
@@ -8381,20 +8384,20 @@
     return e
 }
 class Pr {
     constructor(e) {
         this.validEnd = e, this.next = [], this.wrapCache = []
     }
     static parse(e, n) {
-        let r = new Wk(e, n);
+        let r = new Kk(e, n);
         if (r.next == null) return Pr.empty;
         let s = Cp(r);
         r.next && r.err("Unexpected trailing text");
-        let i = Qk(Xk(s));
-        return Zk(i, r), i
+        let i = ew(Zk(s));
+        return tw(i, r), i
     }
     matchType(e) {
         for (let n = 0; n < this.next.length; n++)
             if (this.next[n].type == e) return this.next[n].next;
         return null
     }
     matchFragment(e, n = 0, r = e.childCount) {
@@ -8495,15 +8498,15 @@
             for (let o = 0; o < r.next.length; o++) i += (o ? ", " : "") + r.next[o].type.name + "->" + e.indexOf(r.next[o].next);
             return i
         }).join(`
 `)
     }
 }
 Pr.empty = new Pr(!0);
-class Wk {
+class Kk {
     constructor(e, n) {
         this.string = e, this.nodeTypes = n, this.inline = null, this.pos = 0, this.tokens = e.split(/\s*(?=\b|\W|$)/), this.tokens[this.tokens.length - 1] == "" && this.tokens.pop(), this.tokens[0] == "" && this.tokens.shift()
     }
     get next() {
         return this.tokens[this.pos]
     }
     eat(e) {
@@ -8512,97 +8515,97 @@
     err(e) {
         throw new SyntaxError(e + " (in content expression '" + this.string + "')")
     }
 }
 
 function Cp(t) {
     let e = [];
-    do e.push(qk(t)); while (t.eat("|"));
+    do e.push(Jk(t)); while (t.eat("|"));
     return e.length == 1 ? e[0] : {
         type: "choice",
         exprs: e
     }
 }
 
-function qk(t) {
+function Jk(t) {
     let e = [];
-    do e.push(Kk(t)); while (t.next && t.next != ")" && t.next != "|");
+    do e.push(Gk(t)); while (t.next && t.next != ")" && t.next != "|");
     return e.length == 1 ? e[0] : {
         type: "seq",
         exprs: e
     }
 }
 
-function Kk(t) {
-    let e = Yk(t);
+function Gk(t) {
+    let e = Qk(t);
     for (;;)
         if (t.eat("+")) e = {
             type: "plus",
             expr: e
         };
         else if (t.eat("*")) e = {
         type: "star",
         expr: e
     };
     else if (t.eat("?")) e = {
         type: "opt",
         expr: e
     };
-    else if (t.eat("{")) e = Jk(t, e);
+    else if (t.eat("{")) e = Yk(t, e);
     else break;
     return e
 }
 
 function ud(t) {
     /\D/.test(t.next) && t.err("Expected number, got '" + t.next + "'");
     let e = Number(t.next);
     return t.pos++, e
 }
 
-function Jk(t, e) {
+function Yk(t, e) {
     let n = ud(t),
         r = n;
     return t.eat(",") && (t.next != "}" ? r = ud(t) : r = -1), t.eat("}") || t.err("Unclosed braced range"), {
         type: "range",
         min: n,
         max: r,
         expr: e
     }
 }
 
-function Gk(t, e) {
+function Xk(t, e) {
     let n = t.nodeTypes,
         r = n[e];
     if (r) return [r];
     let s = [];
     for (let i in n) {
         let o = n[i];
         o.groups.indexOf(e) > -1 && s.push(o)
     }
     return s.length == 0 && t.err("No node type or group '" + e + "' found"), s
 }
 
-function Yk(t) {
+function Qk(t) {
     if (t.eat("(")) {
         let e = Cp(t);
         return t.eat(")") || t.err("Missing closing paren"), e
     } else if (/\W/.test(t.next)) t.err("Unexpected token '" + t.next + "'");
     else {
-        let e = Gk(t, t.next).map(n => (t.inline == null ? t.inline = n.isInline : t.inline != n.isInline && t.err("Mixing inline and block content"), {
+        let e = Xk(t, t.next).map(n => (t.inline == null ? t.inline = n.isInline : t.inline != n.isInline && t.err("Mixing inline and block content"), {
             type: "name",
             value: n
         }));
         return t.pos++, e.length == 1 ? e[0] : {
             type: "choice",
             exprs: e
         }
     }
 }
 
-function Xk(t) {
+function Zk(t) {
     let e = [
         []
     ];
     return s(i(t, 0), n()), e;
 
     function n() {
         return e.push([]) - 1
@@ -8674,15 +8677,15 @@
                 to: a
             } = i[o];
             !l && n.indexOf(a) == -1 && r(a)
         }
     }
 }
 
-function Qk(t) {
+function ew(t) {
     let e = Object.create(null);
     return n(dd(t, 0));
 
     function n(r) {
         let s = [];
         r.forEach(o => {
             t[o].forEach(({
@@ -8705,15 +8708,15 @@
                 next: e[l.join(",")] || n(l)
             })
         }
         return i
     }
 }
 
-function Zk(t, e) {
+function tw(t, e) {
     for (let n = 0, r = [t]; n < r.length; n++) {
         let s = r[n],
             i = !s.validEnd,
             o = [];
         for (let l = 0; l < s.next.length; l++) {
             let {
                 type: a,
@@ -8748,15 +8751,15 @@
     }
     return n
 }
 
 function Mp(t) {
     let e = Object.create(null);
     if (t)
-        for (let n in t) e[n] = new ew(t[n]);
+        for (let n in t) e[n] = new nw(t[n]);
     return e
 }
 let fd = class Ap {
     constructor(e, n, r) {
         this.name = e, this.schema = n, this.spec = r, this.markSet = null, this.groups = r.group ? r.group.split(" ") : [], this.attrs = Mp(r.attrs), this.defaultAttrs = Tp(this.attrs), this.contentMatch = null, this.inlineContent = null, this.isBlock = !(r.inline || e == "text"), this.isText = e == "text"
     }
     get isInline() {
@@ -8833,15 +8836,15 @@
         let s = n.spec.topNode || "doc";
         if (!r[s]) throw new RangeError("Schema is missing its top node type ('" + s + "')");
         if (!r.text) throw new RangeError("Every schema needs a 'text' type");
         for (let i in r.text.attrs) throw new RangeError("The text node type should not have attributes");
         return r
     }
 };
-class ew {
+class nw {
     constructor(e) {
         this.hasDefault = Object.prototype.hasOwnProperty.call(e, "default"), this.default = e.default
     }
     get isRequired() {
         return !this.hasDefault
     }
 }
@@ -8867,15 +8870,15 @@
         for (let n = 0; n < e.length; n++)
             if (e[n].type == this) return e[n]
     }
     excludes(e) {
         return this.excluded.indexOf(e) > -1
     }
 }
-class tw {
+class rw {
     constructor(e) {
         this.cached = Object.create(null);
         let n = this.spec = {};
         for (let s in e) n[s] = e[s];
         n.nodes = nt.from(e.nodes), n.marks = nt.from(e.marks || {}), this.nodes = fd.compile(this.spec.nodes, this), this.marks = Yo.compile(this.spec.marks, this);
         let r = Object.create(null);
         for (let s in this.nodes) {
@@ -8897,15 +8900,15 @@
         else if (e instanceof fd) {
             if (e.schema != this) throw new RangeError("Node type from different schema used (" + e.name + ")")
         } else throw new RangeError("Invalid node type: " + e);
         return e.createChecked(n, r, s)
     }
     text(e, n) {
         let r = this.nodes.text;
-        return new fo(r, r.defaultAttrs, e, De.setFrom(n))
+        return new po(r, r.defaultAttrs, e, De.setFrom(n))
     }
     mark(e, n) {
         return typeof e == "string" && (e = this.marks[e]), e.create(n)
     }
     nodeFromJSON(e) {
         return Nr.fromJSON(this, e)
     }
@@ -8952,15 +8955,15 @@
     parseSlice(e, n = {}) {
         let r = new md(this, n, !0);
         return r.addAll(e, n.from, n.to), q.maxOpen(r.finish())
     }
     matchTag(e, n, r) {
         for (let s = r ? this.tags.indexOf(r) + 1 : 0; s < this.tags.length; s++) {
             let i = this.tags[s];
-            if (sw(e, i.tag) && (i.namespace === void 0 || e.namespaceURI == i.namespace) && (!i.context || n.matchesContext(i.context))) {
+            if (ow(e, i.tag) && (i.namespace === void 0 || e.namespaceURI == i.namespace) && (!i.context || n.matchesContext(i.context))) {
                 if (i.getAttrs) {
                     let o = i.getAttrs(e);
                     if (o === !1) continue;
                     i.attrs = o || void 0
                 }
                 return i
             }
@@ -9040,34 +9043,34 @@
         p: !0,
         pre: !0,
         section: !0,
         table: !0,
         tfoot: !0,
         ul: !0
     },
-    nw = {
+    sw = {
         head: !0,
         noscript: !0,
         object: !0,
         script: !0,
         style: !0,
         title: !0
     },
     Rp = {
         ol: !0,
         ul: !0
     },
-    ho = 1,
-    po = 2,
+    mo = 1,
+    go = 2,
     Xs = 4;
 
 function pd(t, e, n) {
-    return e != null ? (e ? ho : 0) | (e === "full" ? po : 0) : t && t.whitespace == "pre" ? ho | po : n & ~Xs
+    return e != null ? (e ? mo : 0) | (e === "full" ? go : 0) : t && t.whitespace == "pre" ? mo | go : n & ~Xs
 }
-class $i {
+class Fi {
     constructor(e, n, r, s, i, o, l) {
         this.type = e, this.attrs = n, this.marks = r, this.pendingMarks = s, this.solid = i, this.options = l, this.content = [], this.activeMarks = De.none, this.stashMarks = [], this.match = o || (l & Xs ? null : e.contentMatch)
     }
     findWrapping(e) {
         if (!this.match) {
             if (!this.type) return [];
             let n = this.type.contentMatch.fillBefore($.from(e));
@@ -9077,15 +9080,15 @@
                     s;
                 return (s = r.findWrapping(e.type)) ? (this.match = r, s) : null
             }
         }
         return this.match.findWrapping(e.type)
     }
     finish(e) {
-        if (!(this.options & ho)) {
+        if (!(this.options & mo)) {
             let r = this.content[this.content.length - 1],
                 s;
             if (r && r.isText && (s = /[ \t\r\n\u000c]+$/.exec(r.text))) {
                 let i = r;
                 r.text.length == s[0].length ? this.content.pop() : this.content[this.content.length - 1] = i.withText(i.text.slice(0, i.text.length - s[0].length))
             }
         }
@@ -9095,68 +9098,68 @@
     popFromStashMark(e) {
         for (let n = this.stashMarks.length - 1; n >= 0; n--)
             if (e.eq(this.stashMarks[n])) return this.stashMarks.splice(n, 1)[0]
     }
     applyPending(e) {
         for (let n = 0, r = this.pendingMarks; n < r.length; n++) {
             let s = r[n];
-            (this.type ? this.type.allowsMarkType(s.type) : ow(s.type, e)) && !s.isInSet(this.activeMarks) && (this.activeMarks = s.addToSet(this.activeMarks), this.pendingMarks = s.removeFromSet(this.pendingMarks))
+            (this.type ? this.type.allowsMarkType(s.type) : aw(s.type, e)) && !s.isInSet(this.activeMarks) && (this.activeMarks = s.addToSet(this.activeMarks), this.pendingMarks = s.removeFromSet(this.pendingMarks))
         }
     }
     inlineContext(e) {
         return this.type ? this.type.inlineContent : this.content.length ? this.content[0].isInline : e.parentNode && !Np.hasOwnProperty(e.parentNode.nodeName.toLowerCase())
     }
 }
 class md {
     constructor(e, n, r) {
         this.parser = e, this.options = n, this.isOpen = r, this.open = 0;
         let s = n.topNode,
             i, o = pd(null, n.preserveWhitespace, 0) | (r ? Xs : 0);
-        s ? i = new $i(s.type, s.attrs, De.none, De.none, !0, n.topMatch || s.type.contentMatch, o) : r ? i = new $i(null, null, De.none, De.none, !0, null, o) : i = new $i(e.schema.topNodeType, null, De.none, De.none, !0, null, o), this.nodes = [i], this.find = n.findPositions, this.needsBlock = !1
+        s ? i = new Fi(s.type, s.attrs, De.none, De.none, !0, n.topMatch || s.type.contentMatch, o) : r ? i = new Fi(null, null, De.none, De.none, !0, null, o) : i = new Fi(e.schema.topNodeType, null, De.none, De.none, !0, null, o), this.nodes = [i], this.find = n.findPositions, this.needsBlock = !1
     }
     get top() {
         return this.nodes[this.open]
     }
     addDOM(e) {
         if (e.nodeType == 3) this.addTextNode(e);
         else if (e.nodeType == 1) {
             let n = e.getAttribute("style");
             if (!n) this.addElement(e);
             else {
-                let r = this.readStyles(iw(n));
+                let r = this.readStyles(lw(n));
                 if (!r) return;
                 let [s, i] = r, o = this.top;
                 for (let l = 0; l < i.length; l++) this.removePendingMark(i[l], o);
                 for (let l = 0; l < s.length; l++) this.addPendingMark(s[l]);
                 this.addElement(e);
                 for (let l = 0; l < s.length; l++) this.removePendingMark(s[l], o);
                 for (let l = 0; l < i.length; l++) this.addPendingMark(i[l])
             }
         }
     }
     addTextNode(e) {
         let n = e.nodeValue,
             r = this.top;
-        if (r.options & po || r.inlineContext(e) || /[^ \t\r\n\u000c]/.test(n)) {
-            if (r.options & ho) r.options & po ? n = n.replace(/\r\n?/g, `
+        if (r.options & go || r.inlineContext(e) || /[^ \t\r\n\u000c]/.test(n)) {
+            if (r.options & mo) r.options & go ? n = n.replace(/\r\n?/g, `
 `) : n = n.replace(/\r?\n|\r/g, " ");
             else if (n = n.replace(/[ \t\r\n\u000c]+/g, " "), /^[ \t\r\n\u000c]/.test(n) && this.open == this.nodes.length - 1) {
                 let s = r.content[r.content.length - 1],
                     i = e.previousSibling;
                 (!s || i && i.nodeName == "BR" || s.isText && /[ \t\r\n\u000c]$/.test(s.text)) && (n = n.slice(1))
             }
             n && this.insertNode(this.parser.schema.text(n)), this.findInText(e)
         } else this.findInside(e)
     }
     addElement(e, n) {
         let r = e.nodeName.toLowerCase(),
             s;
-        Rp.hasOwnProperty(r) && this.parser.normalizeLists && rw(e);
+        Rp.hasOwnProperty(r) && this.parser.normalizeLists && iw(e);
         let i = this.options.ruleFromNode && this.options.ruleFromNode(e) || (s = this.parser.matchTag(e, this, n));
-        if (i ? i.ignore : nw.hasOwnProperty(r)) this.findInside(e), this.ignoreFallback(e);
+        if (i ? i.ignore : sw.hasOwnProperty(r)) this.findInside(e), this.ignoreFallback(e);
         else if (!i || i.skip || i.closeParent) {
             i && i.closeParent ? this.open = Math.max(0, this.open - 1) : i && i.skip.nodeType && (e = i.skip);
             let o, l = this.top,
                 a = this.needsBlock;
             if (Np.hasOwnProperty(r)) l.content.length && l.content[0].isInline && this.open && (this.open--, l = this.top), o = !0, l.type || (this.needsBlock = !0);
             else if (!e.firstChild) {
                 this.leafFallback(e);
@@ -9237,15 +9240,15 @@
         return s && this.enterInner(e, n, !0, r), s
     }
     enterInner(e, n = null, r = !1, s) {
         this.closeExtra();
         let i = this.top;
         i.applyPending(e), i.match = i.match && i.match.matchType(e);
         let o = pd(e, s, i.options);
-        i.options & Xs && i.content.length == 0 && (o |= Xs), this.nodes.push(new $i(e, n, i.activeMarks, i.pendingMarks, r, null, o)), this.open++
+        i.options & Xs && i.content.length == 0 && (o |= Xs), this.nodes.push(new Fi(e, n, i.activeMarks, i.pendingMarks, r, null, o)), this.open++
     }
     closeExtra(e = !1) {
         let n = this.nodes.length - 1;
         if (n > this.open) {
             for (; n > this.open; n--) this.nodes[n - 1].content.push(this.nodes[n].finish(e));
             this.nodes.length = this.open + 1
         }
@@ -9317,15 +9320,15 @@
             }
         for (let n in this.parser.schema.nodes) {
             let r = this.parser.schema.nodes[n];
             if (r.isTextblock && r.defaultAttrs) return r
         }
     }
     addPendingMark(e) {
-        let n = lw(e, this.top.pendingMarks);
+        let n = cw(e, this.top.pendingMarks);
         n && this.top.stashMarks.push(n), this.top.pendingMarks = e.addToSet(this.top.pendingMarks)
     }
     removePendingMark(e, n) {
         for (let r = this.open; r >= 0; r--) {
             let s = this.nodes[r];
             if (s.pendingMarks.lastIndexOf(e) > -1) s.pendingMarks = e.removeFromSet(s.pendingMarks);
             else {
@@ -9334,39 +9337,39 @@
                 o && s.type && s.type.allowsMarkType(o.type) && (s.activeMarks = o.addToSet(s.activeMarks))
             }
             if (s == n) break
         }
     }
 }
 
-function rw(t) {
+function iw(t) {
     for (let e = t.firstChild, n = null; e; e = e.nextSibling) {
         let r = e.nodeType == 1 ? e.nodeName.toLowerCase() : null;
         r && Rp.hasOwnProperty(r) && n ? (n.appendChild(e), e = n) : r == "li" ? n = e : r && (n = null)
     }
 }
 
-function sw(t, e) {
+function ow(t, e) {
     return (t.matches || t.msMatchesSelector || t.webkitMatchesSelector || t.mozMatchesSelector).call(t, e)
 }
 
-function iw(t) {
+function lw(t) {
     let e = /\s*([\w-]+)\s*:\s*([^;]+)/g,
         n, r = [];
     for (; n = e.exec(t);) r.push(n[1], n[2].trim());
     return r
 }
 
 function gd(t) {
     let e = {};
     for (let n in t) e[n] = t[n];
     return e
 }
 
-function ow(t, e) {
+function aw(t, e) {
     let n = e.schema.nodes;
     for (let r in n) {
         let s = n[r];
         if (!s.allowsMarkType(t)) continue;
         let i = [],
             o = l => {
                 i.push(l);
@@ -9378,15 +9381,15 @@
                     if (c == e || i.indexOf(u) < 0 && o(u)) return !0
                 }
             };
         if (o(s.contentMatch)) return !0
     }
 }
 
-function lw(t, e) {
+function cw(t, e) {
     for (let n = 0; n < e.length; n++)
         if (t.eq(e[n])) return e[n]
 }
 class hn {
     constructor(e, n) {
         this.nodes = e, this.marks = n
     }
@@ -9509,56 +9512,56 @@
 
 function Pl(t) {
     return t.document || window.document
 }
 const Dp = 65535,
     Ip = Math.pow(2, 16);
 
-function aw(t, e) {
+function uw(t, e) {
     return t + e * Ip
 }
 
 function bd(t) {
     return t & Dp
 }
 
-function cw(t) {
+function dw(t) {
     return (t - (t & Dp)) / Ip
 }
 const Pp = 1,
     $p = 2,
-    Ji = 4,
+    Yi = 4,
     Lp = 8;
 class Aa {
     constructor(e, n, r) {
         this.pos = e, this.delInfo = n, this.recover = r
     }
     get deleted() {
         return (this.delInfo & Lp) > 0
     }
     get deletedBefore() {
-        return (this.delInfo & (Pp | Ji)) > 0
+        return (this.delInfo & (Pp | Yi)) > 0
     }
     get deletedAfter() {
-        return (this.delInfo & ($p | Ji)) > 0
+        return (this.delInfo & ($p | Yi)) > 0
     }
     get deletedAcross() {
-        return (this.delInfo & Ji) > 0
+        return (this.delInfo & Yi) > 0
     }
 }
 class Ht {
     constructor(e, n = !1) {
         if (this.ranges = e, this.inverted = n, !e.length && Ht.empty) return Ht.empty
     }
     recover(e) {
         let n = 0,
             r = bd(e);
         if (!this.inverted)
             for (let s = 0; s < r; s++) n += this.ranges[s * 3 + 2] - this.ranges[s * 3 + 1];
-        return this.ranges[r * 3] + n + cw(e)
+        return this.ranges[r * 3] + n + dw(e)
     }
     mapResult(e, n = 1) {
         return this._map(e, n, !1)
     }
     map(e, n = 1) {
         return this._map(e, n, !0)
     }
@@ -9572,16 +9575,16 @@
             let c = this.ranges[l + i],
                 u = this.ranges[l + o],
                 d = a + c;
             if (e <= d) {
                 let f = c ? e == a ? -1 : e == d ? 1 : n : n,
                     h = a + s + (f < 0 ? 0 : u);
                 if (r) return h;
-                let p = e == (n < 0 ? a : d) ? null : aw(l / 3, e - a),
-                    g = e == a ? $p : e == d ? Pp : Ji;
+                let p = e == (n < 0 ? a : d) ? null : uw(l / 3, e - a),
+                    g = e == a ? $p : e == d ? Pp : Yi;
                 return (n < 0 ? e != a : e != d) && (g |= Lp), new Aa(h, g, p)
             }
             s += u - c
         }
         return r ? e + s : new Aa(e + s, 0, null)
     }
     touches(e, n) {
@@ -9714,15 +9717,15 @@
     static fail(e) {
         return new Ye(null, e)
     }
     static fromReplace(e, n, r, s) {
         try {
             return Ye.ok(e.replace(n, r, s))
         } catch (i) {
-            if (i instanceof ao) return Ye.fail(i.message);
+            if (i instanceof uo) return Ye.fail(i.message);
             throw i
         }
     }
 }
 
 function Tc(t, e, n) {
     let r = [];
@@ -9968,15 +9971,15 @@
             if (!o || o.isLeaf) return !0;
             o = o.firstChild, s--
         }
     }
     return !1
 }
 
-function uw(t, e, n, r) {
+function fw(t, e, n, r) {
     let s = [],
         i = [],
         o, l;
     t.doc.nodesBetween(e, n, (a, c, u) => {
         if (!a.isInline) return;
         let d = a.marks;
         if (!r.isInSet(d) && u.type.allowsMarkType(r.type)) {
@@ -9985,15 +9988,15 @@
                 p = r.addToSet(d);
             for (let g = 0; g < d.length; g++) d[g].isInSet(p) || (o && o.to == f && o.mark.eq(d[g]) ? o.to = h : s.push(o = new pn(f, h, d[g])));
             l && l.to == f ? l.to = h : i.push(l = new Jn(f, h, r))
         }
     }), s.forEach(a => t.step(a)), i.forEach(a => t.step(a))
 }
 
-function dw(t, e, n, r) {
+function hw(t, e, n, r) {
     let s = [],
         i = 0;
     t.doc.nodesBetween(e, n, (o, l) => {
         if (!o.isInline) return;
         i++;
         let a = null;
         if (r instanceof Yo) {
@@ -10017,15 +10020,15 @@
                     step: i
                 })
             }
         }
     }), s.forEach(o => t.step(new pn(o.from, o.to, o.style)))
 }
 
-function fw(t, e, n, r = n.contentMatch) {
+function pw(t, e, n, r = n.contentMatch) {
     let s = t.doc.nodeAt(e),
         i = [],
         o = e + 1;
     for (let l = 0; l < s.childCount; l++) {
         let a = s.child(l),
             c = o + a.nodeSize,
             u = r.matchType(a.type);
@@ -10039,117 +10042,117 @@
     if (!r.validEnd) {
         let l = r.fillBefore($.empty, !0);
         t.replace(o, o, new q(l, 0, 0))
     }
     for (let l = i.length - 1; l >= 0; l--) t.step(i[l])
 }
 
-function hw(t, e, n) {
+function mw(t, e, n) {
     return (e == 0 || t.canReplace(e, t.childCount)) && (n == t.childCount || t.canReplace(0, n))
 }
 
 function Ms(t) {
     let n = t.parent.content.cutByIndex(t.startIndex, t.endIndex);
     for (let r = t.depth;; --r) {
         let s = t.$from.node(r),
             i = t.$from.index(r),
             o = t.$to.indexAfter(r);
         if (r < t.depth && s.canReplace(i, o, n)) return r;
-        if (r == 0 || s.type.spec.isolating || !hw(s, i, o)) break
+        if (r == 0 || s.type.spec.isolating || !mw(s, i, o)) break
     }
     return null
 }
 
-function pw(t, e, n) {
+function gw(t, e, n) {
     let {
         $from: r,
         $to: s,
         depth: i
     } = e, o = r.before(i + 1), l = s.after(i + 1), a = o, c = l, u = $.empty, d = 0;
     for (let p = i, g = !1; p > n; p--) g || r.index(p) > 0 ? (g = !0, u = $.from(r.node(p).copy(u)), d++) : a--;
     let f = $.empty,
         h = 0;
     for (let p = i, g = !1; p > n; p--) g || s.after(p + 1) < s.end(p) ? (g = !0, f = $.from(s.node(p).copy(f)), h++) : c++;
     t.step(new et(a, c, o, l, new q(u.append(f), d, h), u.size - d, !0))
 }
 
 function Oc(t, e, n = null, r = t) {
-    let s = mw(t, e),
-        i = s && gw(r, e);
+    let s = yw(t, e),
+        i = s && bw(r, e);
     return i ? s.map(vd).concat({
         type: e,
         attrs: n
     }).concat(i.map(vd)) : null
 }
 
 function vd(t) {
     return {
         type: t,
         attrs: null
     }
 }
 
-function mw(t, e) {
+function yw(t, e) {
     let {
         parent: n,
         startIndex: r,
         endIndex: s
     } = t, i = n.contentMatchAt(r).findWrapping(e);
     if (!i) return null;
     let o = i.length ? i[0] : e;
     return n.canReplaceWith(r, s, o) ? i : null
 }
 
-function gw(t, e) {
+function bw(t, e) {
     let {
         parent: n,
         startIndex: r,
         endIndex: s
     } = t, i = n.child(r), o = e.contentMatch.findWrapping(i.type);
     if (!o) return null;
     let a = (o.length ? o[o.length - 1] : e).contentMatch;
     for (let c = r; a && c < s; c++) a = a.matchType(n.child(c).type);
     return !a || !a.validEnd ? null : o
 }
 
-function yw(t, e, n) {
+function vw(t, e, n) {
     let r = $.empty;
     for (let o = n.length - 1; o >= 0; o--) {
         if (r.size) {
             let l = n[o].type.contentMatch.matchFragment(r);
             if (!l || !l.validEnd) throw new RangeError("Wrapper type given to Transform.wrap does not form valid content of its parent wrapper")
         }
         r = $.from(n[o].type.create(n[o].attrs, r))
     }
     let s = e.start,
         i = e.end;
     t.step(new et(s, i, s, i, new q(r, 0, 0), n.length, !0))
 }
 
-function bw(t, e, n, r, s) {
+function xw(t, e, n, r, s) {
     if (!r.isTextblock) throw new RangeError("Type given to setBlockType should be a textblock");
     let i = t.steps.length;
     t.doc.nodesBetween(e, n, (o, l) => {
-        if (o.isTextblock && !o.hasMarkup(r, s) && vw(t.doc, t.mapping.slice(i).map(l), r)) {
+        if (o.isTextblock && !o.hasMarkup(r, s) && kw(t.doc, t.mapping.slice(i).map(l), r)) {
             t.clearIncompatible(t.mapping.slice(i).map(l, 1), r);
             let a = t.mapping.slice(i),
                 c = a.map(l, 1),
                 u = a.map(l + o.nodeSize, 1);
             return t.step(new et(c, u, c + 1, u - 1, new q($.from(r.create(s, null, o.marks)), 0, 0), 1, !0)), !1
         }
     })
 }
 
-function vw(t, e, n) {
+function kw(t, e, n) {
     let r = t.resolve(e),
         s = r.index();
     return r.parent.canReplaceWith(s, s + 1, n)
 }
 
-function xw(t, e, n, r, s) {
+function ww(t, e, n, r, s) {
     let i = t.doc.nodeAt(e);
     if (!i) throw new RangeError("No node at given position");
     n || (n = i.type);
     let o = n.create(r, null, s || i.marks);
     if (i.isLeaf) return t.replaceWith(e, e + i.nodeSize, o);
     if (!n.validContent(i.content)) throw new RangeError("Invalid content for node type " + n.name);
     t.step(new et(e, e + i.nodeSize, e + 1, e + i.nodeSize - 1, new q($.from(o), 0, 0), 1, !0))
@@ -10169,15 +10172,15 @@
         if (p != d && (h = h.replaceChild(0, p.type.create(p.attrs))), !d.canReplace(f + 1, d.childCount) || !p.type.validContent(h)) return !1
     }
     let l = s.indexAfter(i),
         a = r && r[0];
     return s.node(i).canReplaceWith(l, l, a ? a.type : s.node(i + 1).type)
 }
 
-function kw(t, e, n = 1, r) {
+function Sw(t, e, n = 1, r) {
     let s = t.doc.resolve(e),
         i = $.empty,
         o = $.empty;
     for (let l = s.depth, a = s.depth - n, c = n - 1; l > a; l--, c--) {
         i = $.from(s.node(l).copy(i));
         let u = r && r[c];
         o = $.from(u ? u.type.create(u.attrs, o) : s.node(l).copy(o))
@@ -10201,20 +10204,20 @@
         let i, o, l = r.index(s);
         if (s == r.depth ? (i = r.nodeBefore, o = r.nodeAfter) : n > 0 ? (i = r.node(s + 1), l++, o = r.node(s).maybeChild(l)) : (i = r.node(s).maybeChild(l - 1), o = r.node(s + 1)), i && !i.isTextblock && Fp(i, o) && r.node(s).canReplace(l, l + 1)) return e;
         if (s == 0) break;
         e = n < 0 ? r.before(s) : r.after(s)
     }
 }
 
-function ww(t, e, n) {
+function _w(t, e, n) {
     let r = new ct(e - n, e + n, q.empty, !0);
     t.step(r)
 }
 
-function Sw(t, e, n) {
+function Cw(t, e, n) {
     let r = t.resolve(e);
     if (r.parent.canReplaceWith(r.index(), r.index(), n)) return e;
     if (r.parentOffset == 0)
         for (let s = r.depth - 1; s >= 0; s--) {
             let i = r.index(s);
             if (r.node(s).canReplaceWith(i, i, n)) return r.before(s + 1);
             if (i > 0) return null
@@ -10249,21 +10252,21 @@
     return null
 }
 
 function Mc(t, e, n = e, r = q.empty) {
     if (e == n && !r.size) return null;
     let s = t.resolve(e),
         i = t.resolve(n);
-    return zp(s, i, r) ? new ct(e, n, r) : new _w(s, i, r).fit()
+    return zp(s, i, r) ? new ct(e, n, r) : new Ew(s, i, r).fit()
 }
 
 function zp(t, e, n) {
     return !n.openStart && !n.openEnd && t.start() == e.start() && t.parent.canReplace(t.index(), e.index(), n.content)
 }
-class _w {
+class Ew {
     constructor(e, n, r) {
         this.$from = e, this.$to = n, this.unplaced = r, this.frontier = [], this.placed = $.empty;
         for (let s = 0; s <= e.depth; s++) {
             let i = e.node(s);
             this.frontier.push({
                 type: i.type,
                 match: i.contentMatchAt(e.indexAfter(s))
@@ -10465,28 +10468,28 @@
 }
 
 function Fl(t, e, n, r, s) {
     let i = t.node(e),
         o = s ? t.indexAfter(e) : t.index(e);
     if (o == i.childCount && !n.compatibleContent(i.type)) return null;
     let l = r.fillBefore(i.content, !0, o);
-    return l && !Cw(n, i.content, o) ? l : null
+    return l && !Tw(n, i.content, o) ? l : null
 }
 
-function Cw(t, e, n) {
+function Tw(t, e, n) {
     for (let r = n; r < e.childCount; r++)
         if (!t.allowsMarks(e.child(r).marks)) return !0;
     return !1
 }
 
-function Ew(t) {
+function Ow(t) {
     return t.spec.defining || t.spec.definingForContent
 }
 
-function Tw(t, e, n, r) {
+function Mw(t, e, n, r) {
     if (!r.size) return t.deleteRange(e, n);
     let s = t.doc.resolve(e),
         i = t.doc.resolve(n);
     if (zp(s, i, r)) return t.step(new ct(e, n, r));
     let o = Up(s, t.doc.resolve(n));
     o[o.length - 1] == 0 && o.pop();
     let l = -(s.depth + 1);
@@ -10502,15 +10505,15 @@
     for (let f = r.content, h = 0;; h++) {
         let p = f.firstChild;
         if (c.push(p), h == r.openStart) break;
         f = p.content
     }
     for (let f = u - 1; f >= 0; f--) {
         let h = c[f].type,
-            p = Ew(h);
+            p = Ow(h);
         if (p && s.node(a).type != h) u = f;
         else if (p || !h.isTextblock) break
     }
     for (let f = r.openStart; f >= 0; f--) {
         let h = (f + u + 1) % (r.openStart + 1),
             p = c[h];
         if (p)
@@ -10539,23 +10542,23 @@
         let i = s.contentMatchAt(0),
             o = i.fillBefore(t).append(t);
         t = o.append(i.matchFragment(o).fillBefore($.empty, !0))
     }
     return t
 }
 
-function Ow(t, e, n, r) {
+function Aw(t, e, n, r) {
     if (!r.isInline && e == n && t.doc.resolve(e).parent.content.size) {
-        let s = Sw(t.doc, e, r.type);
+        let s = Cw(t.doc, e, r.type);
         s != null && (e = n = s)
     }
     t.replaceRange(e, n, new q($.from(r), 0, 0))
 }
 
-function Mw(t, e, n) {
+function Nw(t, e, n) {
     let r = t.doc.resolve(e),
         s = t.doc.resolve(n),
         i = Up(r, s);
     for (let o = 0; o < i.length; o++) {
         let l = i[o],
             a = o == i.length - 1;
         if (a && l == 0 || r.node(l).type.contentMatch.validEnd) return t.delete(r.start(l), s.end(l));
@@ -10617,15 +10620,15 @@
 fs = function t(e) {
     let n = Error.call(this, e);
     return n.__proto__ = t.prototype, n
 };
 fs.prototype = Object.create(Error.prototype);
 fs.prototype.constructor = fs;
 fs.prototype.name = "TransformError";
-class Aw {
+class Rw {
     constructor(e) {
         this.doc = e, this.steps = [], this.docs = [], this.mapping = new es
     }
     get before() {
         return this.docs.length ? this.docs[0] : this.doc
     }
     step(e) {
@@ -10653,36 +10656,36 @@
     delete(e, n) {
         return this.replace(e, n, q.empty)
     }
     insert(e, n) {
         return this.replaceWith(e, e, n)
     }
     replaceRange(e, n, r) {
-        return Tw(this, e, n, r), this
+        return Mw(this, e, n, r), this
     }
     replaceRangeWith(e, n, r) {
-        return Ow(this, e, n, r), this
+        return Aw(this, e, n, r), this
     }
     deleteRange(e, n) {
-        return Mw(this, e, n), this
+        return Nw(this, e, n), this
     }
     lift(e, n) {
-        return pw(this, e, n), this
+        return gw(this, e, n), this
     }
     join(e, n = 1) {
-        return ww(this, e, n), this
+        return _w(this, e, n), this
     }
     wrap(e, n) {
-        return yw(this, e, n), this
+        return vw(this, e, n), this
     }
     setBlockType(e, n = e, r, s = null) {
-        return bw(this, e, n, r, s), this
+        return xw(this, e, n, r, s), this
     }
     setNodeMarkup(e, n, r = null, s) {
-        return xw(this, e, n, r, s), this
+        return ww(this, e, n, r, s), this
     }
     setNodeAttribute(e, n, r) {
         return this.step(new ns(e, n, r)), this
     }
     addNodeMark(e, n) {
         return this.step(new Gn(e, n)), this
     }
@@ -10691,30 +10694,30 @@
             let r = this.doc.nodeAt(e);
             if (!r) throw new RangeError("No node at position " + e);
             if (n = n.isInSet(r.marks), !n) return this
         }
         return this.step(new ds(e, n)), this
     }
     split(e, n = 1, r) {
-        return kw(this, e, n, r), this
+        return Sw(this, e, n, r), this
     }
     addMark(e, n, r) {
-        return uw(this, e, n, r), this
+        return fw(this, e, n, r), this
     }
     removeMark(e, n, r) {
-        return dw(this, e, n, r), this
+        return hw(this, e, n, r), this
     }
     clearIncompatible(e, n, r) {
-        return fw(this, e, n, r), this
+        return pw(this, e, n, r), this
     }
 }
 const Bl = Object.create(null);
 class ve {
     constructor(e, n, r) {
-        this.$anchor = e, this.$head = n, this.ranges = r || [new Nw(e.min(n), e.max(n))]
+        this.$anchor = e, this.$head = n, this.ranges = r || [new Dw(e.min(n), e.max(n))]
     }
     get anchor() {
         return this.$anchor.pos
     }
     get head() {
         return this.$head.pos
     }
@@ -10793,15 +10796,15 @@
         return Bl[e] = n, n.prototype.jsonID = e, n
     }
     getBookmark() {
         return xe.between(this.$anchor, this.$head).getBookmark()
     }
 }
 ve.prototype.visible = !0;
-class Nw {
+class Dw {
     constructor(e, n) {
         this.$from = e, this.$to = n
     }
 }
 let xd = !1;
 
 function kd(t) {
@@ -10949,19 +10952,19 @@
     map(e) {
         return new nn(e)
     }
     eq(e) {
         return e instanceof nn
     }
     getBookmark() {
-        return Rw
+        return Iw
     }
 }
 ve.jsonID("all", nn);
-const Rw = {
+const Iw = {
     map() {
         return this
     },
     resolve(t) {
         return new nn(t)
     }
 };
@@ -10989,47 +10992,47 @@
     let i = t.mapping.maps[r],
         o;
     i.forEach((l, a, c, u) => {
         o == null && (o = u)
     }), t.setSelection(ve.near(t.doc.resolve(o), n))
 }
 const Sd = 1,
-    Li = 2,
+    Bi = 2,
     _d = 4;
-class Dw extends Aw {
+class Pw extends Rw {
     constructor(e) {
         super(e.doc), this.curSelectionFor = 0, this.updated = 0, this.meta = Object.create(null), this.time = Date.now(), this.curSelection = e.selection, this.storedMarks = e.storedMarks
     }
     get selection() {
         return this.curSelectionFor < this.steps.length && (this.curSelection = this.curSelection.map(this.doc, this.mapping.slice(this.curSelectionFor)), this.curSelectionFor = this.steps.length), this.curSelection
     }
     setSelection(e) {
         if (e.$from.doc != this.doc) throw new RangeError("Selection passed to setSelection must point at the current document");
-        return this.curSelection = e, this.curSelectionFor = this.steps.length, this.updated = (this.updated | Sd) & ~Li, this.storedMarks = null, this
+        return this.curSelection = e, this.curSelectionFor = this.steps.length, this.updated = (this.updated | Sd) & ~Bi, this.storedMarks = null, this
     }
     get selectionSet() {
         return (this.updated & Sd) > 0
     }
     setStoredMarks(e) {
-        return this.storedMarks = e, this.updated |= Li, this
+        return this.storedMarks = e, this.updated |= Bi, this
     }
     ensureMarks(e) {
         return De.sameSet(this.storedMarks || this.selection.$from.marks(), e) || this.setStoredMarks(e), this
     }
     addStoredMark(e) {
         return this.ensureMarks(e.addToSet(this.storedMarks || this.selection.$head.marks()))
     }
     removeStoredMark(e) {
         return this.ensureMarks(e.removeFromSet(this.storedMarks || this.selection.$head.marks()))
     }
     get storedMarksSet() {
-        return (this.updated & Li) > 0
+        return (this.updated & Bi) > 0
     }
     addStep(e, n) {
-        super.addStep(e, n), this.updated = this.updated & ~Li, this.storedMarks = null
+        super.addStep(e, n), this.updated = this.updated & ~Bi, this.storedMarks = null
     }
     setTime(e) {
         return this.time = e, this
     }
     replaceSelection(e) {
         return this.selection.replace(this, e), this
     }
@@ -11074,15 +11077,15 @@
     return !e || !t ? t : t.bind(e)
 }
 class Vs {
     constructor(e, n, r) {
         this.name = e, this.init = Cd(n.init, r), this.apply = Cd(n.apply, r)
     }
 }
-const Iw = [new Vs("doc", {
+const $w = [new Vs("doc", {
     init(t) {
         return t.doc || t.schema.topNodeType.createAndFill()
     },
     apply(t) {
         return t.doc
     }
 }), new Vs("selection", {
@@ -11105,15 +11108,15 @@
     },
     apply(t, e) {
         return t.scrolledIntoView ? e + 1 : e
     }
 })];
 class Hl {
     constructor(e, n) {
-        this.schema = e, this.plugins = [], this.pluginsByKey = Object.create(null), this.fields = Iw.slice(), n && n.forEach(r => {
+        this.schema = e, this.plugins = [], this.pluginsByKey = Object.create(null), this.fields = $w.slice(), n && n.forEach(r => {
             if (this.pluginsByKey[r.key]) throw new RangeError("Adding different instances of a keyed plugin (" + r.key + ")");
             this.plugins.push(r), this.pluginsByKey[r.key] = r, r.spec.state && this.fields.push(new Vs(r.key, r.spec.state, r))
         })
     }
 }
 class Kr {
     constructor(e) {
@@ -11183,15 +11186,15 @@
         for (let s = 0; s < r.length; s++) {
             let i = r[s];
             n[i.name] = i.apply(e, this[i.name], this, n)
         }
         return n
     }
     get tr() {
-        return new Dw(this)
+        return new Pw(this)
     }
     static create(e) {
         let n = new Hl(e.doc ? e.doc.type.schema : e.schema, e.plugins),
             r = new Kr(n);
         for (let s = 0; s < n.fields.length; s++) r[n.fields[s].name] = n.fields[s].init(e, r);
         return r
     }
@@ -11287,64 +11290,64 @@
 const En = function(t, e, n) {
         let r = Ed || (Ed = document.createRange());
         return r.setEnd(t, n ?? t.nodeValue.length), r.setStart(t, e || 0), r
     },
     $r = function(t, e, n, r) {
         return n && (Td(t, e, n, r, -1) || Td(t, e, n, r, 1))
     },
-    Pw = /^(img|br|input|textarea|hr)$/i;
+    Lw = /^(img|br|input|textarea|hr)$/i;
 
 function Td(t, e, n, r, s) {
     for (;;) {
         if (t == n && e == r) return !0;
         if (e == (s < 0 ? 0 : dn(t))) {
             let i = t.parentNode;
-            if (!i || i.nodeType != 1 || Lw(t) || Pw.test(t.nodeName) || t.contentEditable == "false") return !1;
+            if (!i || i.nodeType != 1 || Bw(t) || Lw.test(t.nodeName) || t.contentEditable == "false") return !1;
             e = Nt(t) + (s < 0 ? 0 : 1), t = i
         } else if (t.nodeType == 1) {
             if (t = t.childNodes[e + (s < 0 ? -1 : 0)], t.contentEditable == "false") return !1;
             e = s < 0 ? dn(t) : 0
         } else return !1
     }
 }
 
 function dn(t) {
     return t.nodeType == 3 ? t.nodeValue.length : t.childNodes.length
 }
 
-function $w(t, e, n) {
+function Fw(t, e, n) {
     for (let r = e == 0, s = e == dn(t); r || s;) {
         if (t == n) return !0;
         let i = Nt(t);
         if (t = t.parentNode, !t) return !1;
         r = r && i == 0, s = s && i == dn(t)
     }
 }
 
-function Lw(t) {
+function Bw(t) {
     let e;
     for (let n = t; n && !(e = n.pmViewDesc); n = n.parentNode);
     return e && e.node && e.node.isBlock && (e.dom == t || e.contentDOM == t)
 }
 const Qo = function(t) {
     return t.focusNode && $r(t.focusNode, t.focusOffset, t.anchorNode, t.anchorOffset)
 };
 
 function wr(t, e) {
     let n = document.createEvent("Event");
     return n.initEvent("keydown", !0, !0), n.keyCode = t, n.key = n.code = e, n
 }
 
-function Fw(t) {
+function Hw(t) {
     let e = t.activeElement;
     for (; e && e.shadowRoot;) e = e.shadowRoot.activeElement;
     return e
 }
 
-function Bw(t, e, n) {
+function zw(t, e, n) {
     if (t.caretPositionFromPoint) try {
         let r = t.caretPositionFromPoint(e, n);
         if (r) return {
             node: r.offsetNode,
             offset: r.offset
         }
     } catch {}
@@ -11364,37 +11367,37 @@
     Da = /Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(ar),
     _t = !!(Kp || Da || Ra),
     Zn = Kp ? document.documentMode : Da ? +Da[1] : Ra ? +Ra[1] : 0,
     on = !_t && /gecko\/(\d+)/i.test(ar);
 on && +(/Firefox\/(\d+)/.exec(ar) || [0, 0])[1];
 const Ia = !_t && /Chrome\/(\d+)/.exec(ar),
     dt = !!Ia,
-    Hw = Ia ? +Ia[1] : 0,
+    Vw = Ia ? +Ia[1] : 0,
     bt = !_t && !!bn && /Apple Computer/.test(bn.vendor),
     hs = bt && (/Mobile\/\w+/.test(ar) || !!bn && bn.maxTouchPoints > 2),
     Ft = hs || (bn ? /Mac/.test(bn.platform) : !1),
-    zw = bn ? /Win/.test(bn.platform) : !1,
+    jw = bn ? /Win/.test(bn.platform) : !1,
     Gt = /Android \d/.test(ar),
     Zo = !!Od && "webkitFontSmoothing" in Od.documentElement.style,
-    Vw = Zo ? +(/\bAppleWebKit\/(\d+)/.exec(navigator.userAgent) || [0, 0])[1] : 0;
+    Uw = Zo ? +(/\bAppleWebKit\/(\d+)/.exec(navigator.userAgent) || [0, 0])[1] : 0;
 
-function jw(t) {
+function Ww(t) {
     return {
         left: 0,
         right: t.documentElement.clientWidth,
         top: 0,
         bottom: t.documentElement.clientHeight
     }
 }
 
 function zn(t, e) {
     return typeof t == "number" ? t : t[e]
 }
 
-function Uw(t) {
+function qw(t) {
     let e = t.getBoundingClientRect(),
         n = e.width / t.offsetWidth || 1,
         r = e.height / t.offsetHeight || 1;
     return {
         left: e.left,
         right: e.left + t.clientWidth * n,
         top: e.top,
@@ -11406,15 +11409,15 @@
     let r = t.someProp("scrollThreshold") || 0,
         s = t.someProp("scrollMargin") || 5,
         i = t.dom.ownerDocument;
     for (let o = n || t.dom; o; o = hi(o)) {
         if (o.nodeType != 1) continue;
         let l = o,
             a = l == i.body,
-            c = a ? jw(i) : Uw(l),
+            c = a ? Ww(i) : qw(l),
             u = 0,
             d = 0;
         if (e.top < c.top + zn(r, "top") ? d = -(c.top - e.top + zn(s, "top")) : e.bottom > c.bottom - zn(r, "bottom") && (d = e.bottom - c.bottom + zn(s, "bottom")), e.left < c.left + zn(r, "left") ? u = -(c.left - e.left + zn(s, "left")) : e.right > c.right - zn(r, "right") && (u = e.right - c.right + zn(s, "right")), u || d)
             if (a) i.defaultView.scrollBy(u, d);
             else {
                 let f = l.scrollLeft,
                     h = l.scrollTop;
@@ -11427,15 +11430,15 @@
                     right: e.right - p,
                     bottom: e.bottom - g
                 }
             } if (a) break
     }
 }
 
-function Ww(t) {
+function Kw(t) {
     let e = t.dom.getBoundingClientRect(),
         n = Math.max(0, e.top),
         r, s;
     for (let i = (e.left + e.right) / 2, o = n + 1; o < Math.min(innerHeight, e.bottom); o += 5) {
         let l = t.root.elementFromPoint(i, o);
         if (!l || l == t.dom || !t.dom.contains(l)) continue;
         let a = l.getBoundingClientRect();
@@ -11458,15 +11461,15 @@
             dom: r,
             top: r.scrollTop,
             left: r.scrollLeft
         }), t != n); r = hi(r));
     return e
 }
 
-function qw({
+function Jw({
     refDOM: t,
     refTop: e,
     stack: n
 }) {
     let r = t ? t.getBoundingClientRect().top : 0;
     Gp(n, r == 0 ? 0 : r - e)
 }
@@ -11479,15 +11482,15 @@
             left: i
         } = t[n];
         r.scrollTop != s + e && (r.scrollTop = s + e), r.scrollLeft != i && (r.scrollLeft = i)
     }
 }
 let Vr = null;
 
-function Kw(t) {
+function Gw(t) {
     if (t.setActive) return t.setActive();
     if (Vr) return t.focus(Vr);
     let e = Jp(t);
     t.focus(Vr == null ? {
         get preventScroll() {
             return Vr = {
                 preventScroll: !0
@@ -11522,21 +11525,21 @@
             } else p.top > e.top && !a && p.left <= e.left && p.right >= e.left && (a = u, c = {
                 left: Math.max(p.left, Math.min(p.right, e.left)),
                 top: p.top
             });
             !n && (e.left >= p.right && e.top >= p.top || e.left >= p.left && e.top >= p.bottom) && (i = d + 1)
         }
     }
-    return !n && a && (n = a, s = c, r = 0), n && n.nodeType == 3 ? Jw(n, s) : !n || r && n.nodeType == 1 ? {
+    return !n && a && (n = a, s = c, r = 0), n && n.nodeType == 3 ? Yw(n, s) : !n || r && n.nodeType == 1 ? {
         node: t,
         offset: i
     } : Yp(n, s)
 }
 
-function Jw(t, e) {
+function Yw(t, e) {
     let n = t.nodeValue.length,
         r = document.createRange();
     for (let s = 0; s < n; s++) {
         r.setEnd(t, s + 1), r.setStart(t, s);
         let i = Vn(r, 1);
         if (i.top != i.bottom && Nc(e, i)) return {
             node: t,
@@ -11549,32 +11552,32 @@
     }
 }
 
 function Nc(t, e) {
     return t.left >= e.left - 1 && t.left <= e.right + 1 && t.top >= e.top - 1 && t.top <= e.bottom + 1
 }
 
-function Gw(t, e) {
+function Xw(t, e) {
     let n = t.parentNode;
     return n && /^li$/i.test(n.nodeName) && e.left < t.getBoundingClientRect().left ? n : t
 }
 
-function Yw(t, e, n) {
+function Qw(t, e, n) {
     let {
         node: r,
         offset: s
     } = Yp(e, n), i = -1;
     if (r.nodeType == 1 && !r.firstChild) {
         let o = r.getBoundingClientRect();
         i = o.left != o.right && n.left > (o.left + o.right) / 2 ? 1 : -1
     }
     return t.docView.posFromDOM(r, s, i)
 }
 
-function Xw(t, e, n, r) {
+function Zw(t, e, n, r) {
     let s = -1;
     for (let i = e, o = !1; i != t.dom;) {
         let l = t.docView.nearestDesc(i, !0);
         if (!l) return null;
         if (l.dom.nodeType == 1 && (l.node.isBlock && l.parent && !o || !l.contentDOM)) {
             let a = l.dom.getBoundingClientRect();
             if (l.node.isBlock && l.parent && !o && (o = !0, a.left > r.left || a.top > r.top ? s = l.posBefore : (a.right < r.left || a.bottom < r.top) && (s = l.posAfter)), !l.contentDOM && s < 0) return (l.node.isBlock ? r.top < (a.top + a.bottom) / 2 : r.left < (a.left + a.right) / 2) ? l.posBefore : l.posAfter
@@ -11597,39 +11600,39 @@
                 }
             }
             if ((i = (i + 1) % r) == s) break
         }
     return t
 }
 
-function Qw(t, e) {
+function eS(t, e) {
     let n = t.dom.ownerDocument,
         r, s = 0,
-        i = Bw(n, e.left, e.top);
+        i = zw(n, e.left, e.top);
     i && ({
         node: r,
         offset: s
     } = i);
     let o = (t.root.elementFromPoint ? t.root : n).elementFromPoint(e.left, e.top),
         l;
     if (!o || !t.dom.contains(o.nodeType != 1 ? o.parentNode : o)) {
         let c = t.dom.getBoundingClientRect();
         if (!Nc(e, c) || (o = Xp(t.dom, e, c), !o)) return null
     }
     if (bt)
         for (let c = o; r && c; c = hi(c)) c.draggable && (r = void 0);
-    if (o = Gw(o, e), r) {
+    if (o = Xw(o, e), r) {
         if (on && r.nodeType == 1 && (s = Math.min(s, r.childNodes.length), s < r.childNodes.length)) {
             let c = r.childNodes[s],
                 u;
             c.nodeName == "IMG" && (u = c.getBoundingClientRect()).right <= e.left && u.bottom > e.top && s++
         }
-        r == t.dom && s == r.childNodes.length - 1 && r.lastChild.nodeType == 1 && e.top > r.lastChild.getBoundingClientRect().bottom ? l = t.state.doc.content.size : (s == 0 || r.nodeType != 1 || r.childNodes[s - 1].nodeName != "BR") && (l = Xw(t, r, s, e))
+        r == t.dom && s == r.childNodes.length - 1 && r.lastChild.nodeType == 1 && e.top > r.lastChild.getBoundingClientRect().bottom ? l = t.state.doc.content.size : (s == 0 || r.nodeType != 1 || r.childNodes[s - 1].nodeName != "BR") && (l = Zw(t, r, s, e))
     }
-    l == null && (l = Yw(t, o, e));
+    l == null && (l = Qw(t, o, e));
     let a = t.docView.nearestDesc(o, !0);
     return {
         pos: l,
         inside: a ? a.posAtStart - a.border : -1
     }
 }
 
@@ -11641,24 +11644,24 @@
     let n = t.getClientRects();
     if (n.length) {
         let r = n[e < 0 ? 0 : n.length - 1];
         if (Ad(r)) return r
     }
     return Array.prototype.find.call(n, Ad) || t.getBoundingClientRect()
 }
-const Zw = /[\u0590-\u05f4\u0600-\u06ff\u0700-\u08ac]/;
+const tS = /[\u0590-\u05f4\u0600-\u06ff\u0700-\u08ac]/;
 
 function Qp(t, e, n) {
     let {
         node: r,
         offset: s,
         atom: i
     } = t.docView.domFromPos(e, n < 0 ? -1 : 1), o = Zo || on;
     if (r.nodeType == 3)
-        if (o && (Zw.test(r.nodeValue) || (n < 0 ? !s : s == r.nodeValue.length))) {
+        if (o && (tS.test(r.nodeValue) || (n < 0 ? !s : s == r.nodeValue.length))) {
             let a = Vn(En(r, s, s), n);
             if (on && s && /\s/.test(r.nodeValue[s - 1]) && s < r.nodeValue.length) {
                 let c = Vn(En(r, s - 1, s - 1), -1);
                 if (c.top == a.top) {
                     let u = Vn(En(r, s, s + 1), -1);
                     if (u.top != a.top) return Ps(u, u.left < c.left)
                 }
@@ -11723,15 +11726,15 @@
     try {
         return n()
     } finally {
         r != e && t.updateState(r), s != t.dom && s && s.focus()
     }
 }
 
-function eS(t, e, n) {
+function nS(t, e, n) {
     let r = e.selection,
         s = n == "up" ? r.$from : r.$to;
     return Zp(t, e, () => {
         let {
             node: i
         } = t.docView.domFromPos(s.pos, n == "up" ? -1 : 1);
         for (;;) {
@@ -11753,26 +11756,26 @@
                 let u = a[c];
                 if (u.bottom > u.top + 1 && (n == "up" ? o.top - u.top > (u.bottom - o.top) * 2 : u.bottom - o.bottom > (o.bottom - u.top) * 2)) return !1
             }
         }
         return !0
     })
 }
-const tS = /[\u0590-\u08ac]/;
+const rS = /[\u0590-\u08ac]/;
 
-function nS(t, e, n) {
+function sS(t, e, n) {
     let {
         $head: r
     } = e.selection;
     if (!r.parent.isTextblock) return !1;
     let s = r.parentOffset,
         i = !s,
         o = s == r.parent.content.size,
         l = t.domSelection();
-    return !tS.test(r.parent.textContent) || !l.modify ? n == "left" || n == "backward" ? i : o : Zp(t, e, () => {
+    return !rS.test(r.parent.textContent) || !l.modify ? n == "left" || n == "backward" ? i : o : Zp(t, e, () => {
         let {
             focusNode: a,
             focusOffset: c,
             anchorNode: u,
             anchorOffset: d
         } = t.domSelectionRange(), f = l.caretBidiLevel;
         l.modify("move", n, "character");
@@ -11788,22 +11791,22 @@
         return f != null && (l.caretBidiLevel = f), v
     })
 }
 let Nd = null,
     Rd = null,
     Dd = !1;
 
-function rS(t, e, n) {
-    return Nd == e && Rd == n ? Dd : (Nd = e, Rd = n, Dd = n == "up" || n == "down" ? eS(t, e, n) : nS(t, e, n))
+function iS(t, e, n) {
+    return Nd == e && Rd == n ? Dd : (Nd = e, Rd = n, Dd = n == "up" || n == "down" ? nS(t, e, n) : sS(t, e, n))
 }
 const Ut = 0,
     Id = 1,
     Cr = 2,
     vn = 3;
-class wi {
+class _i {
     constructor(e, n, r, s) {
         this.parent = e, this.children = n, this.dom = r, this.contentDOM = s, this.dirty = Ut, r.pmViewDesc = this
     }
     matchesWidget(e) {
         return !1
     }
     matchesMark(e) {
@@ -12116,15 +12119,15 @@
     get domAtom() {
         return !1
     }
     get ignoreForCoords() {
         return !1
     }
 }
-class em extends wi {
+class em extends _i {
     constructor(e, n, r, s) {
         let i, o = n.type.toDOM;
         if (typeof o == "function" && (o = o(r, () => {
                 if (!i) return s;
                 if (i.parent) return i.parent.posBeforeChild(i)
             })), !n.type.spec.raw) {
             if (o.nodeType != 1) {
@@ -12156,15 +12159,15 @@
     get domAtom() {
         return !0
     }
     get side() {
         return this.widget.type.side
     }
 }
-class sS extends wi {
+class oS extends _i {
     constructor(e, n, r, s) {
         super(e, [], n, null), this.textDOM = r, this.text = s
     }
     get size() {
         return this.text.length
     }
     localPosFromDOM(e, n) {
@@ -12176,15 +12179,15 @@
             offset: e
         }
     }
     ignoreMutation(e) {
         return e.type === "characterData" && e.target.nodeValue == e.oldValue
     }
 }
-class Lr extends wi {
+class Lr extends _i {
     constructor(e, n, r, s) {
         super(e, [], r, s), this.mark = n
     }
     static create(e, n, r, s) {
         let i = s.nodeViews[n.type.name],
             o = i && i(n, s, r);
         return (!o || !o.dom) && (o = hn.renderSpec(document, n.type.spec.toDOM(n, r))), new Lr(e, n, o.dom, o.contentDOM || o.dom)
@@ -12211,15 +12214,15 @@
             i = this.children,
             o = this.size;
         n < o && (i = La(i, n, o, r)), e > 0 && (i = La(i, 0, e, r));
         for (let l = 0; l < i.length; l++) i[l].parent = s;
         return s.children = i, s
     }
 }
-class er extends wi {
+class er extends _i {
     constructor(e, n, r, s, i, o, l, a, c) {
         super(e, [], i, o), this.node = n, this.outerDeco = r, this.innerDeco = s, this.nodeDOM = l
     }
     static create(e, n, r, s, i, o) {
         let l = i.nodeViews[n.type.name],
             a, c = l && l(n, i, () => {
                 if (!a) return o;
@@ -12232,15 +12235,15 @@
             else if (u.nodeType != 3) throw new RangeError("Text must be rendered as a DOM text node")
         } else u || ({
             dom: u,
             contentDOM: d
         } = hn.renderSpec(document, n.type.spec.toDOM(n)));
         !d && !n.isText && u.nodeName != "BR" && (u.hasAttribute("contenteditable") || (u.contentEditable = "false"), n.type.spec.draggable && (u.draggable = !0));
         let f = u;
-        return u = sm(u, r, n), c ? a = new iS(e, n, r, s, u, d || null, f, c, i, o + 1) : n.isText ? new el(e, n, r, s, u, f, i) : new er(e, n, r, s, u, d || null, f, i, o + 1)
+        return u = sm(u, r, n), c ? a = new lS(e, n, r, s, u, d || null, f, c, i, o + 1) : n.isText ? new el(e, n, r, s, u, f, i) : new er(e, n, r, s, u, d || null, f, i, o + 1)
     }
     parseRule() {
         if (this.node.type.spec.reparseInView) return null;
         let e = {
             node: this.node.type.name,
             attrs: this.node.attrs
         };
@@ -12269,35 +12272,35 @@
     }
     updateChildren(e, n) {
         let r = this.node.inlineContent,
             s = n,
             i = e.composing ? this.localCompositionInfo(e, n) : null,
             o = i && i.pos > -1 ? i : null,
             l = i && i.pos < 0,
-            a = new lS(this, o && o.node, e);
-        uS(this.node, this.innerDeco, (c, u, d) => {
+            a = new cS(this, o && o.node, e);
+        fS(this.node, this.innerDeco, (c, u, d) => {
             c.spec.marks ? a.syncToMarks(c.spec.marks, r, e) : c.type.side >= 0 && !d && a.syncToMarks(u == this.node.childCount ? De.none : this.node.child(u).marks, r, e), a.placeWidget(c, e, s)
         }, (c, u, d, f) => {
             a.syncToMarks(c.marks, r, e);
             let h;
             a.findNodeMatch(c, u, d, f) || l && e.state.selection.from > s && e.state.selection.to < s + c.nodeSize && (h = a.findIndexWithChild(i.node)) > -1 && a.updateNodeAt(c, u, d, h, e) || a.updateNextNode(c, u, d, e, f, s) || a.addNode(c, u, d, e, s), s += c.nodeSize
-        }), a.syncToMarks([], r, e), this.node.isTextblock && a.addTextblockHacks(), a.destroyRest(), (a.changed || this.dirty == Cr) && (o && this.protectLocalComposition(e, o), nm(this.contentDOM, this.children, e), hs && dS(this.dom))
+        }), a.syncToMarks([], r, e), this.node.isTextblock && a.addTextblockHacks(), a.destroyRest(), (a.changed || this.dirty == Cr) && (o && this.protectLocalComposition(e, o), nm(this.contentDOM, this.children, e), hs && hS(this.dom))
     }
     localCompositionInfo(e, n) {
         let {
             from: r,
             to: s
         } = e.state.selection;
         if (!(e.state.selection instanceof xe) || r < n || s > n + this.node.content.size) return null;
         let i = e.domSelectionRange(),
-            o = fS(i.focusNode, i.focusOffset);
+            o = pS(i.focusNode, i.focusOffset);
         if (!o || !this.dom.contains(o.parentNode)) return null;
         if (this.node.inlineContent) {
             let l = o.nodeValue,
-                a = hS(this.node.content, l, r - n, s - n);
+                a = mS(this.node.content, l, r - n, s - n);
             return a < 0 ? null : {
                 node: o,
                 pos: a,
                 text: l
             }
         } else return {
             node: o,
@@ -12313,15 +12316,15 @@
         if (this.getDesc(n)) return;
         let i = n;
         for (; i.parentNode != this.contentDOM; i = i.parentNode) {
             for (; i.previousSibling;) i.parentNode.removeChild(i.previousSibling);
             for (; i.nextSibling;) i.parentNode.removeChild(i.nextSibling);
             i.pmViewDesc && (i.pmViewDesc = void 0)
         }
-        let o = new sS(this, i, n, s);
+        let o = new oS(this, i, n, s);
         e.input.compositionNodes.push(o), this.children = La(this.children, r, r + s.length, e, o)
     }
     update(e, n, r, s) {
         return this.dirty == vn || !e.sameMarkup(this.node) ? !1 : (this.updateInner(e, n, r, s), !0)
     }
     updateInner(e, n, r, s) {
         this.updateOuterDeco(n), this.node = e, this.innerDeco = r, this.contentDOM && this.updateChildren(s, this.posAtStart), this.dirty = Ut
@@ -12388,15 +12391,15 @@
     markDirty(e, n) {
         super.markDirty(e, n), this.dom != this.nodeDOM && (e == 0 || n == this.nodeDOM.nodeValue.length) && (this.dirty = vn)
     }
     get domAtom() {
         return !1
     }
 }
-class tm extends wi {
+class tm extends _i {
     parseRule() {
         return {
             ignore: !0
         }
     }
     matchesHack(e) {
         return this.dirty == Ut && this.dom.nodeName == e
@@ -12404,15 +12407,15 @@
     get domAtom() {
         return !0
     }
     get ignoreForCoords() {
         return this.dom.nodeName == "IMG"
     }
 }
-class iS extends er {
+class lS extends er {
     constructor(e, n, r, s, i, o, l, a, c, u) {
         super(e, n, r, s, i, o, l, c, u), this.spec = a
     }
     update(e, n, r, s) {
         if (this.dirty == vn) return !1;
         if (this.spec.update) {
             let i = this.spec.update(e, n, r);
@@ -12486,20 +12489,20 @@
     for (let i = 0; i < r.length; i++) {
         let o = r[i],
             l = n[i];
         if (i) {
             let a;
             l && l.nodeName == o.nodeName && s != t && (a = s.parentNode) && a.nodeName.toLowerCase() == o.nodeName || (a = document.createElement(o.nodeName), a.pmIsDeco = !0, a.appendChild(s), l = Er[0]), s = a
         }
-        oS(s, l || Er[0], o)
+        aS(s, l || Er[0], o)
     }
     return s
 }
 
-function oS(t, e, n) {
+function aS(t, e, n) {
     for (let r in e) r != "class" && r != "style" && r != "nodeName" && !(r in n) && t.removeAttribute(r);
     for (let r in n) r != "class" && r != "style" && r != "nodeName" && n[r] != e[r] && t.setAttribute(r, n[r]);
     if (e.class != n.class) {
         let r = e.class ? e.class.split(" ").filter(Boolean) : [],
             s = n.class ? n.class.split(" ").filter(Boolean) : [];
         for (let i = 0; i < r.length; i++) s.indexOf(r[i]) == -1 && t.classList.remove(r[i]);
         for (let i = 0; i < s.length; i++) r.indexOf(s[i]) == -1 && t.classList.add(s[i]);
@@ -12526,17 +12529,17 @@
     return !0
 }
 
 function $d(t) {
     let e = t.nextSibling;
     return t.parentNode.removeChild(t), e
 }
-class lS {
+class cS {
     constructor(e, n, r) {
-        this.lock = n, this.view = r, this.index = 0, this.stack = [], this.changed = !1, this.top = e, this.preMatch = aS(e.node.content, e)
+        this.lock = n, this.view = r, this.index = 0, this.stack = [], this.changed = !1, this.top = e, this.preMatch = uS(e.node.content, e)
     }
     destroyBetween(e, n) {
         if (e != n) {
             for (let r = e; r < n; r++) this.top.children[r].destroy();
             this.top.children.splice(e, n - e), this.changed = !0
         }
     }
@@ -12651,15 +12654,15 @@
         }
     }
     isLocked(e) {
         return this.lock && (e == this.lock || e.nodeType == 1 && e.contains(this.lock.parentNode))
     }
 }
 
-function aS(t, e) {
+function uS(t, e) {
     let n = e,
         r = n.children.length,
         s = t.childCount,
         i = new Map,
         o = [];
     e: for (; s > 0;) {
         let l;
@@ -12683,19 +12686,19 @@
     return {
         index: s,
         matched: i,
         matches: o.reverse()
     }
 }
 
-function cS(t, e) {
+function dS(t, e) {
     return t.type.side - e.type.side
 }
 
-function uS(t, e, n, r) {
+function fS(t, e, n, r) {
     let s = e.locals(t),
         i = 0;
     if (s.length == 0) {
         for (let c = 0; c < t.childCount; c++) {
             let u = t.child(c);
             r(u, s, e.forChild(i, u), c), i += u.nodeSize
         }
@@ -12706,15 +12709,15 @@
         a = null;
     for (let c = 0;;) {
         if (o < s.length && s[o].to == i) {
             let p = s[o++],
                 g;
             for (; o < s.length && s[o].to == i;)(g || (g = [p])).push(s[o++]);
             if (g) {
-                g.sort(cS);
+                g.sort(dS);
                 for (let v = 0; v < g.length; v++) n(g[v], c, !!a)
             } else n(p, c, !!a)
         }
         let u, d;
         if (a) d = -1, u = a, a = null;
         else if (c < t.childCount) d = c, u = t.child(c++);
         else break;
@@ -12728,33 +12731,33 @@
             p < f && (a = u.cut(p - i), u = u.cut(0, p - i), f = p, d = -1)
         }
         let h = u.isInline && !u.isLeaf ? l.filter(p => !p.inline) : l.slice();
         r(u, h, e.forChild(i, u), d), i = f
     }
 }
 
-function dS(t) {
+function hS(t) {
     if (t.nodeName == "UL" || t.nodeName == "OL") {
         let e = t.style.cssText;
         t.style.cssText = e + "; list-style: square !important", window.getComputedStyle(t).listStyle, t.style.cssText = e
     }
 }
 
-function fS(t, e) {
+function pS(t, e) {
     for (;;) {
         if (t.nodeType == 3) return t;
         if (t.nodeType == 1 && e > 0) {
             if (t.childNodes.length > e && t.childNodes[e].nodeType == 3) return t.childNodes[e];
             t = t.childNodes[e - 1], e = dn(t)
         } else if (t.nodeType == 1 && e < t.childNodes.length) t = t.childNodes[e], e = 0;
         else return null
     }
 }
 
-function hS(t, e, n, r) {
+function mS(t, e, n, r) {
     for (let s = 0, i = 0; s < t.childCount && i <= r;) {
         let o = t.child(s++),
             l = i;
         if (i += o.nodeSize, !o.isText) continue;
         let a = o.text;
         for (; s < t.childCount;) {
             let c = t.child(s++);
@@ -12790,15 +12793,15 @@
         o = t.docView.posFromDOM(n.focusNode, n.focusOffset, 1);
     if (o < 0) return null;
     let l = r.resolve(o),
         a, c;
     if (Qo(n)) {
         for (a = l; s && !s.node;) s = s.parent;
         let u = s.node;
-        if (s && u.isAtom && se.isSelectable(u) && s.parent && !(u.isInline && $w(n.focusNode, n.focusOffset, s.dom))) {
+        if (s && u.isAtom && se.isSelectable(u) && s.parent && !(u.isInline && Fw(n.focusNode, n.focusOffset, s.dom))) {
             let d = s.posBefore;
             c = new se(o == d ? l : r.resolve(d))
         }
     } else {
         let u = t.docView.posFromDOM(n.anchorNode, n.anchorOffset, 1);
         if (u < 0) return null;
         a = r.resolve(u)
@@ -12821,26 +12824,26 @@
             let r = t.domSelectionRange(),
                 s = t.domObserver.currentSelection;
             if (r.anchorNode && s.anchorNode && $r(r.anchorNode, r.anchorOffset, s.anchorNode, s.anchorOffset)) {
                 t.input.mouseDown.delayedSelectionSync = !0, t.domObserver.setCurSelection();
                 return
             }
         }
-        if (t.domObserver.disconnectSelection(), t.cursorWrapper) mS(t);
+        if (t.domObserver.disconnectSelection(), t.cursorWrapper) yS(t);
         else {
             let {
                 anchor: r,
                 head: s
             } = n, i, o;
-            Ld && !(n instanceof xe) && (n.$from.parent.inlineContent || (i = Fd(t, n.from)), !n.empty && !n.$from.parent.inlineContent && (o = Fd(t, n.to))), t.docView.setSelection(r, s, t.root, e), Ld && (i && Bd(i), o && Bd(o)), n.visible ? t.dom.classList.remove("ProseMirror-hideselection") : (t.dom.classList.add("ProseMirror-hideselection"), "onselectionchange" in document && pS(t))
+            Ld && !(n instanceof xe) && (n.$from.parent.inlineContent || (i = Fd(t, n.from)), !n.empty && !n.$from.parent.inlineContent && (o = Fd(t, n.to))), t.docView.setSelection(r, s, t.root, e), Ld && (i && Bd(i), o && Bd(o)), n.visible ? t.dom.classList.remove("ProseMirror-hideselection") : (t.dom.classList.add("ProseMirror-hideselection"), "onselectionchange" in document && gS(t))
         }
         t.domObserver.setCurSelection(), t.domObserver.connectSelection()
     }
 }
-const Ld = bt || dt && Hw < 63;
+const Ld = bt || dt && Vw < 63;
 
 function Fd(t, e) {
     let {
         node: n,
         offset: r
     } = t.docView.domFromPos(e, 0), s = r < n.childNodes.length ? n.childNodes[r] : null, i = r ? n.childNodes[r - 1] : null;
     if (bt && s && s.contentEditable == "false") return jl(s);
@@ -12854,28 +12857,28 @@
     return t.contentEditable = "true", bt && t.draggable && (t.draggable = !1, t.wasDraggable = !0), t
 }
 
 function Bd(t) {
     t.contentEditable = "false", t.wasDraggable && (t.draggable = !0, t.wasDraggable = null)
 }
 
-function pS(t) {
+function gS(t) {
     let e = t.dom.ownerDocument;
     e.removeEventListener("selectionchange", t.input.hideSelectionGuard);
     let n = t.domSelectionRange(),
         r = n.anchorNode,
         s = n.anchorOffset;
     e.addEventListener("selectionchange", t.input.hideSelectionGuard = () => {
         (n.anchorNode != r || n.anchorOffset != s) && (e.removeEventListener("selectionchange", t.input.hideSelectionGuard), setTimeout(() => {
             (!im(t) || t.state.selection.visible) && t.dom.classList.remove("ProseMirror-hideselection")
         }, 20))
     })
 }
 
-function mS(t) {
+function yS(t) {
     let e = t.domSelection(),
         n = document.createRange(),
         r = t.cursorWrapper.dom,
         s = r.nodeName == "IMG";
     s ? n.setEnd(r.parentNode, Nt(r) + 1) : n.setEnd(r, 0), n.collapse(!1), e.removeAllRanges(), e.addRange(n), !s && !t.state.selection.visible && _t && Zn <= 11 && (r.disabled = !0, r.disabled = !1)
 }
 
@@ -12904,15 +12907,15 @@
     try {
         return t.dom.contains(e.anchorNode.nodeType == 3 ? e.anchorNode.parentNode : e.anchorNode) && (t.editable || t.dom.contains(e.focusNode.nodeType == 3 ? e.focusNode.parentNode : e.focusNode))
     } catch {
         return !1
     }
 }
 
-function gS(t) {
+function bS(t) {
     let e = t.docView.domFromPos(t.state.selection.anchor, 0),
         n = t.domSelectionRange();
     return $r(e.node, e.offset, n.anchorNode, n.anchorOffset)
 }
 
 function Fa(t, e) {
     let {
@@ -12945,72 +12948,72 @@
         if (r instanceof se && r.node.isInline) return Sr(t, new xe(e > 0 ? r.$to : r.$from)); {
             let s = Fa(t.state, e);
             return s ? Sr(t, s) : !1
         }
     }
 }
 
-function mo(t) {
+function yo(t) {
     return t.nodeType == 3 ? t.nodeValue.length : t.childNodes.length
 }
 
 function Zs(t) {
     let e = t.pmViewDesc;
     return e && e.size == 0 && (t.nextSibling || t.nodeName != "BR")
 }
 
 function $s(t, e) {
-    return e < 0 ? yS(t) : am(t)
+    return e < 0 ? vS(t) : am(t)
 }
 
-function yS(t) {
+function vS(t) {
     let e = t.domSelectionRange(),
         n = e.focusNode,
         r = e.focusOffset;
     if (!n) return;
     let s, i, o = !1;
-    for (on && n.nodeType == 1 && r < mo(n) && Zs(n.childNodes[r]) && (o = !0);;)
+    for (on && n.nodeType == 1 && r < yo(n) && Zs(n.childNodes[r]) && (o = !0);;)
         if (r > 0) {
             if (n.nodeType != 1) break; {
                 let l = n.childNodes[r - 1];
                 if (Zs(l)) s = n, i = --r;
                 else if (l.nodeType == 3) n = l, r = n.nodeValue.length;
                 else break
             }
         } else {
             if (cm(n)) break; {
                 let l = n.previousSibling;
                 for (; l && Zs(l);) s = n.parentNode, i = Nt(l), l = l.previousSibling;
-                if (l) n = l, r = mo(n);
+                if (l) n = l, r = yo(n);
                 else {
                     if (n = n.parentNode, n == t.dom) break;
                     r = 0
                 }
             }
         } o ? Ba(t, n, r) : s && Ba(t, s, i)
 }
 
 function am(t) {
     let e = t.domSelectionRange(),
         n = e.focusNode,
         r = e.focusOffset;
     if (!n) return;
-    let s = mo(n),
+    let s = yo(n),
         i, o;
     for (;;)
         if (r < s) {
             if (n.nodeType != 1) break;
             let l = n.childNodes[r];
             if (Zs(l)) i = n, o = ++r;
             else break
         } else {
             if (cm(n)) break; {
                 let l = n.nextSibling;
                 for (; l && Zs(l);) i = l.parentNode, o = Nt(l) + 1, l = l.nextSibling;
-                if (l) n = l, r = 0, s = mo(n);
+                if (l) n = l, r = 0, s = yo(n);
                 else {
                     if (n = n.parentNode, n == t.dom) break;
                     r = s = 0
                 }
             }
         } i && Ba(t, i, o)
 }
@@ -13033,15 +13036,15 @@
     setTimeout(() => {
         t.state == s && An(t)
     }, 50)
 }
 
 function jd(t, e) {
     let n = t.state.doc.resolve(e);
-    if (!(dt || zw) && n.parent.inlineContent) {
+    if (!(dt || jw) && n.parent.inlineContent) {
         let s = t.coordsAtPos(e);
         if (e > n.start()) {
             let i = t.coordsAtPos(e - 1),
                 o = (i.top + i.bottom) / 2;
             if (o > s.top && o < s.bottom && Math.abs(i.left - s.left) > 1) return i.left < s.left ? "ltr" : "rtl"
         }
         if (e < n.end()) {
@@ -13090,47 +13093,47 @@
     return !1
 }
 
 function qd(t, e, n) {
     t.domObserver.stop(), e.contentEditable = n, t.domObserver.start()
 }
 
-function bS(t) {
+function xS(t) {
     if (!bt || t.state.selection.$head.parentOffset > 0) return !1;
     let {
         focusNode: e,
         focusOffset: n
     } = t.domSelectionRange();
     if (e && e.nodeType == 1 && n == 0 && e.firstChild && e.firstChild.contentEditable == "false") {
         let r = e.firstChild;
         qd(t, r, "true"), setTimeout(() => qd(t, r, "false"), 20)
     }
     return !1
 }
 
-function vS(t) {
+function kS(t) {
     let e = "";
     return t.ctrlKey && (e += "c"), t.metaKey && (e += "m"), t.altKey && (e += "a"), t.shiftKey && (e += "s"), e
 }
 
-function xS(t, e) {
+function wS(t, e) {
     let n = e.keyCode,
-        r = vS(e);
+        r = kS(e);
     if (n == 8 || Ft && n == 72 && r == "c") return Wd(t, -1) || $s(t, -1);
     if (n == 46 || Ft && n == 68 && r == "c") return Wd(t, 1) || $s(t, 1);
     if (n == 13 || n == 27) return !0;
     if (n == 37 || Ft && n == 66 && r == "c") {
         let s = n == 37 ? jd(t, t.state.selection.from) == "ltr" ? -1 : 1 : -1;
         return Vd(t, s, r) || $s(t, s)
     } else if (n == 39 || Ft && n == 70 && r == "c") {
         let s = n == 39 ? jd(t, t.state.selection.from) == "ltr" ? 1 : -1 : 1;
         return Vd(t, s, r) || $s(t, s)
     } else {
         if (n == 38 || Ft && n == 80 && r == "c") return Ud(t, -1, r) || $s(t, -1);
-        if (n == 40 || Ft && n == 78 && r == "c") return bS(t) || Ud(t, 1, r) || am(t);
+        if (n == 40 || Ft && n == 78 && r == "c") return xS(t) || Ud(t, 1, r) || am(t);
         if (r == (Ft ? "m" : "c") && (n == 66 || n == 73 || n == 89 || n == 90)) return !0
     }
     return !1
 }
 
 function um(t, e) {
     t.someProp("transformCopied", h => {
@@ -13194,47 +13197,47 @@
             o = document.createElement("div"), e.split(/(?:\r\n?|\n)+/).forEach(g => {
                 let v = o.appendChild(document.createElement("p"));
                 g && v.appendChild(p.serializeNode(h.text(g, f)))
             })
         }
     } else t.someProp("transformPastedHTML", d => {
         n = d(n, t)
-    }), o = SS(n), Zo && _S(o);
+    }), o = CS(n), Zo && ES(o);
     let c = o && o.querySelector("[data-pm-slice]"),
         u = c && /^(\d+) (\d+)(?: -(\d+))? (.*)/.exec(c.getAttribute("data-pm-slice") || "");
     if (u && u[3])
         for (let d = +u[3]; d > 0; d--) {
             let f = o.firstChild;
             for (; f && f.nodeType != 1;) f = f.nextSibling;
             if (!f) break;
             o = f
         }
     if (l || (l = (t.someProp("clipboardParser") || t.someProp("domParser") || us.fromSchema(t.state.schema)).parseSlice(o, {
             preserveWhitespace: !!(a || u),
             context: s,
             ruleFromNode(f) {
-                return f.nodeName == "BR" && !f.nextSibling && f.parentNode && !kS.test(f.parentNode.nodeName) ? {
+                return f.nodeName == "BR" && !f.nextSibling && f.parentNode && !SS.test(f.parentNode.nodeName) ? {
                     ignore: !0
                 } : null
             }
-        })), u) l = CS(Kd(l, +u[1], +u[2]), u[4]);
-    else if (l = q.maxOpen(wS(l.content, s), !0), l.openStart || l.openEnd) {
+        })), u) l = TS(Kd(l, +u[1], +u[2]), u[4]);
+    else if (l = q.maxOpen(_S(l.content, s), !0), l.openStart || l.openEnd) {
         let d = 0,
             f = 0;
         for (let h = l.content.firstChild; d < l.openStart && !h.type.spec.isolating; d++, h = h.firstChild);
         for (let h = l.content.lastChild; f < l.openEnd && !h.type.spec.isolating; f++, h = h.lastChild);
         l = Kd(l, d, f)
     }
     return t.someProp("transformPasted", d => {
         l = d(l, t)
     }), l
 }
-const kS = /^(a|abbr|acronym|b|cite|code|del|em|i|ins|kbd|label|output|q|ruby|s|samp|span|strong|sub|sup|time|u|tt|var)$/i;
+const SS = /^(a|abbr|acronym|b|cite|code|del|em|i|ins|kbd|label|output|q|ruby|s|samp|span|strong|sub|sup|time|u|tt|var)$/i;
 
-function wS(t, e) {
+function _S(t, e) {
     if (t.childCount < 2) return t;
     for (let n = e.depth; n >= 0; n--) {
         let s = e.node(n).contentMatchAt(e.index(n)),
             i, o = [];
         if (t.forEach(l => {
                 if (!o) return;
                 let a = s.findWrapping(l.type),
@@ -13293,34 +13296,34 @@
 };
 let Jd = null;
 
 function gm() {
     return Jd || (Jd = document.implementation.createHTMLDocument("title"))
 }
 
-function SS(t) {
+function CS(t) {
     let e = /^(\s*<meta [^>]*>)*/.exec(t);
     e && (t = t.slice(e[0].length));
     let n = gm().createElement("div"),
         r = /<([a-z][^>\s]+)/i.exec(t),
         s;
     if ((s = r && mm[r[1].toLowerCase()]) && (t = s.map(i => "<" + i + ">").join("") + t + s.map(i => "</" + i + ">").reverse().join("")), n.innerHTML = t, s)
         for (let i = 0; i < s.length; i++) n = n.querySelector(s[i]) || n;
     return n
 }
 
-function _S(t) {
+function ES(t) {
     let e = t.querySelectorAll(dt ? "span:not([class]):not([style])" : "span.Apple-converted-space");
     for (let n = 0; n < e.length; n++) {
         let r = e[n];
         r.childNodes.length == 1 && r.textContent == " " && r.parentNode && r.parentNode.replaceChild(t.ownerDocument.createTextNode(" "), r)
     }
 }
 
-function CS(t, e) {
+function TS(t, e) {
     if (!t.size) return t;
     let n = t.content.firstChild.type.schema,
         r;
     try {
         r = JSON.parse(e)
     } catch {
         return t
@@ -13335,46 +13338,46 @@
         if (!a || a.hasRequiredAttrs()) break;
         s = $.from(a.create(r[l + 1], s)), i++, o++
     }
     return new q(s, i, o)
 }
 const vt = {},
     xt = {},
-    ES = {
+    OS = {
         touchstart: !0,
         touchmove: !0
     };
-class TS {
+class MS {
     constructor() {
         this.shiftKey = !1, this.mouseDown = null, this.lastKeyCode = null, this.lastKeyCodeTime = 0, this.lastClick = {
             time: 0,
             x: 0,
             y: 0,
             type: ""
         }, this.lastSelectionOrigin = null, this.lastSelectionTime = 0, this.lastIOSEnter = 0, this.lastIOSEnterFallbackTimeout = -1, this.lastFocus = 0, this.lastTouch = 0, this.lastAndroidDelete = 0, this.composing = !1, this.composingTimeout = -1, this.compositionNodes = [], this.compositionEndedAt = -2e8, this.compositionID = 1, this.domChangeCount = 0, this.eventHandlers = Object.create(null), this.hideSelectionGuard = null
     }
 }
 
-function OS(t) {
+function AS(t) {
     for (let e in vt) {
         let n = vt[e];
         t.dom.addEventListener(e, t.input.eventHandlers[e] = r => {
-            AS(t, r) && !Ic(t, r) && (t.editable || !(r.type in xt)) && n(t, r)
-        }, ES[e] ? {
+            RS(t, r) && !Ic(t, r) && (t.editable || !(r.type in xt)) && n(t, r)
+        }, OS[e] ? {
             passive: !0
         } : void 0)
     }
     bt && t.dom.addEventListener("input", () => null), za(t)
 }
 
 function Yn(t, e) {
     t.input.lastSelectionOrigin = e, t.input.lastSelectionTime = Date.now()
 }
 
-function MS(t) {
+function NS(t) {
     t.domObserver.stop();
     for (let e in t.input.eventHandlers) t.dom.removeEventListener(e, t.input.eventHandlers[e]);
     clearTimeout(t.input.composingTimeout), clearTimeout(t.input.lastIOSEnterFallbackTimeout)
 }
 
 function za(t) {
     t.someProp("handleDOMEvents", e => {
@@ -13385,34 +13388,34 @@
 function Ic(t, e) {
     return t.someProp("handleDOMEvents", n => {
         let r = n[e.type];
         return r ? r(t, e) || e.defaultPrevented : !1
     })
 }
 
-function AS(t, e) {
+function RS(t, e) {
     if (!e.bubbles) return !0;
     if (e.defaultPrevented) return !1;
     for (let n = e.target; n != t.dom; n = n.parentNode)
         if (!n || n.nodeType == 11 || n.pmViewDesc && n.pmViewDesc.stopEvent(e)) return !1;
     return !0
 }
 
-function NS(t, e) {
+function DS(t, e) {
     !Ic(t, e) && vt[e.type] && (t.editable || !(e.type in xt)) && vt[e.type](t, e)
 }
 xt.keydown = (t, e) => {
     let n = e;
     if (t.input.shiftKey = n.keyCode == 16 || n.shiftKey, !bm(t, n) && (t.input.lastKeyCode = n.keyCode, t.input.lastKeyCodeTime = Date.now(), !(Gt && dt && n.keyCode == 13)))
         if (n.keyCode != 229 && t.domObserver.forceFlush(), hs && n.keyCode == 13 && !n.ctrlKey && !n.altKey && !n.metaKey) {
             let r = Date.now();
             t.input.lastIOSEnter = r, t.input.lastIOSEnterFallbackTimeout = setTimeout(() => {
                 t.input.lastIOSEnter == r && (t.someProp("handleKeyDown", s => s(t, wr(13, "Enter"))), t.input.lastIOSEnter = 0)
             }, 200)
-        } else t.someProp("handleKeyDown", r => r(t, n)) || xS(t, n) ? n.preventDefault() : Yn(t, "key")
+        } else t.someProp("handleKeyDown", r => r(t, n)) || wS(t, n) ? n.preventDefault() : Yn(t, "key")
 };
 xt.keyup = (t, e) => {
     e.keyCode == 16 && (t.input.shiftKey = !1)
 };
 xt.keypress = (t, e) => {
     let n = e;
     if (bm(t, n) || !n.charCode || n.ctrlKey && !n.altKey || Ft && n.metaKey) return;
@@ -13430,15 +13433,15 @@
 function tl(t) {
     return {
         left: t.clientX,
         top: t.clientY
     }
 }
 
-function RS(t, e) {
+function IS(t, e) {
     let n = e.x - t.clientX,
         r = e.y - t.clientY;
     return n * n + r * r < 100
 }
 
 function Pc(t, e, n, r, s) {
     if (r == -1) return !1;
@@ -13450,22 +13453,22 @@
 
 function rs(t, e, n) {
     t.focused || t.focus();
     let r = t.state.tr.setSelection(e);
     n == "pointer" && r.setMeta("pointer", !0), t.dispatch(r)
 }
 
-function DS(t, e) {
+function PS(t, e) {
     if (e == -1) return !1;
     let n = t.state.doc.resolve(e),
         r = n.nodeAfter;
     return r && r.isAtom && se.isSelectable(r) ? (rs(t, new se(n), "pointer"), !0) : !1
 }
 
-function IS(t, e) {
+function $S(t, e) {
     if (e == -1) return !1;
     let n = t.state.selection,
         r, s;
     n instanceof se && (r = n.node);
     let i = t.state.doc.resolve(e);
     for (let o = i.depth + 1; o > 0; o--) {
         let l = o > i.depth ? i.nodeAfter : i.node(o);
@@ -13473,27 +13476,27 @@
             r && n.$from.depth > 0 && o >= n.$from.depth && i.before(n.$from.depth + 1) == n.$from.pos ? s = i.before(n.$from.depth) : s = i.before(o);
             break
         }
     }
     return s != null ? (rs(t, se.create(t.state.doc, s), "pointer"), !0) : !1
 }
 
-function PS(t, e, n, r, s) {
-    return Pc(t, "handleClickOn", e, n, r) || t.someProp("handleClick", i => i(t, e, r)) || (s ? IS(t, n) : DS(t, n))
+function LS(t, e, n, r, s) {
+    return Pc(t, "handleClickOn", e, n, r) || t.someProp("handleClick", i => i(t, e, r)) || (s ? $S(t, n) : PS(t, n))
 }
 
-function $S(t, e, n, r) {
+function FS(t, e, n, r) {
     return Pc(t, "handleDoubleClickOn", e, n, r) || t.someProp("handleDoubleClick", s => s(t, e, r))
 }
 
-function LS(t, e, n, r) {
-    return Pc(t, "handleTripleClickOn", e, n, r) || t.someProp("handleTripleClick", s => s(t, e, r)) || FS(t, n, r)
+function BS(t, e, n, r) {
+    return Pc(t, "handleTripleClickOn", e, n, r) || t.someProp("handleTripleClick", s => s(t, e, r)) || HS(t, n, r)
 }
 
-function FS(t, e, n) {
+function HS(t, e, n) {
     if (n.button != 0) return !1;
     let r = t.state.doc;
     if (e == -1) return r.inlineContent ? (rs(t, xe.create(r, 0, r.content.size), "pointer"), !0) : !1;
     let s = r.resolve(e);
     for (let i = s.depth + 1; i > 0; i--) {
         let o = i > s.depth ? s.nodeAfter : s.node(i),
             l = s.before(i);
@@ -13501,33 +13504,33 @@
         else if (se.isSelectable(o)) rs(t, se.create(r, l), "pointer");
         else continue;
         return !0
     }
 }
 
 function $c(t) {
-    return go(t)
+    return bo(t)
 }
 const ym = Ft ? "metaKey" : "ctrlKey";
 vt.mousedown = (t, e) => {
     let n = e;
     t.input.shiftKey = n.shiftKey;
     let r = $c(t),
         s = Date.now(),
         i = "singleClick";
-    s - t.input.lastClick.time < 500 && RS(n, t.input.lastClick) && !n[ym] && (t.input.lastClick.type == "singleClick" ? i = "doubleClick" : t.input.lastClick.type == "doubleClick" && (i = "tripleClick")), t.input.lastClick = {
+    s - t.input.lastClick.time < 500 && IS(n, t.input.lastClick) && !n[ym] && (t.input.lastClick.type == "singleClick" ? i = "doubleClick" : t.input.lastClick.type == "doubleClick" && (i = "tripleClick")), t.input.lastClick = {
         time: s,
         x: n.clientX,
         y: n.clientY,
         type: i
     };
     let o = t.posAtCoords(tl(n));
-    o && (i == "singleClick" ? (t.input.mouseDown && t.input.mouseDown.done(), t.input.mouseDown = new BS(t, o, n, !!r)) : (i == "doubleClick" ? $S : LS)(t, o.pos, o.inside, n) ? n.preventDefault() : Yn(t, "pointer"))
+    o && (i == "singleClick" ? (t.input.mouseDown && t.input.mouseDown.done(), t.input.mouseDown = new zS(t, o, n, !!r)) : (i == "doubleClick" ? FS : BS)(t, o.pos, o.inside, n) ? n.preventDefault() : Yn(t, "pointer"))
 };
-class BS {
+class zS {
     constructor(e, n, r, s) {
         this.view = e, this.pos = n, this.event = r, this.flushed = s, this.delayedSelectionSync = !1, this.mightDrag = null, this.startDoc = e.state.doc, this.selectNode = !!r[ym], this.allowDefault = r.shiftKey;
         let i, o;
         if (n.inside > -1) i = e.state.doc.nodeAt(n.inside), o = n.inside;
         else {
             let u = e.state.doc.resolve(n.pos);
             i = u.parent, o = u.depth ? u.before() : 0
@@ -13549,15 +13552,15 @@
     }
     done() {
         this.view.root.removeEventListener("mouseup", this.up), this.view.root.removeEventListener("mousemove", this.move), this.mightDrag && this.target && (this.view.domObserver.stop(), this.mightDrag.addAttr && this.target.removeAttribute("draggable"), this.mightDrag.setUneditable && this.target.removeAttribute("contentEditable"), this.view.domObserver.start()), this.delayedSelectionSync && setTimeout(() => An(this.view)), this.view.input.mouseDown = null
     }
     up(e) {
         if (this.done(), !this.view.dom.contains(e.target)) return;
         let n = this.pos;
-        this.view.state.doc != this.startDoc && (n = this.view.posAtCoords(tl(e))), this.updateAllowDefault(e), this.allowDefault || !n ? Yn(this.view, "pointer") : PS(this.view, n.pos, n.inside, e, this.selectNode) ? e.preventDefault() : e.button == 0 && (this.flushed || bt && this.mightDrag && !this.mightDrag.node.isAtom || dt && !this.view.state.selection.visible && Math.min(Math.abs(n.pos - this.view.state.selection.from), Math.abs(n.pos - this.view.state.selection.to)) <= 2) ? (rs(this.view, ve.near(this.view.state.doc.resolve(n.pos)), "pointer"), e.preventDefault()) : Yn(this.view, "pointer")
+        this.view.state.doc != this.startDoc && (n = this.view.posAtCoords(tl(e))), this.updateAllowDefault(e), this.allowDefault || !n ? Yn(this.view, "pointer") : LS(this.view, n.pos, n.inside, e, this.selectNode) ? e.preventDefault() : e.button == 0 && (this.flushed || bt && this.mightDrag && !this.mightDrag.node.isAtom || dt && !this.view.state.selection.visible && Math.min(Math.abs(n.pos - this.view.state.selection.from), Math.abs(n.pos - this.view.state.selection.to)) <= 2) ? (rs(this.view, ve.near(this.view.state.doc.resolve(n.pos)), "pointer"), e.preventDefault()) : Yn(this.view, "pointer")
     }
     move(e) {
         this.updateAllowDefault(e), Yn(this.view, "pointer"), e.buttons == 0 && this.done()
     }
     updateAllowDefault(e) {
         !this.allowDefault && (Math.abs(this.event.x - e.clientX) > 4 || Math.abs(this.event.y - e.clientY) > 4) && (this.allowDefault = !0)
     }
@@ -13569,117 +13572,117 @@
     t.input.lastTouch = Date.now(), Yn(t, "pointer")
 };
 vt.contextmenu = t => $c(t);
 
 function bm(t, e) {
     return t.composing ? !0 : bt && Math.abs(e.timeStamp - t.input.compositionEndedAt) < 500 ? (t.input.compositionEndedAt = -2e8, !0) : !1
 }
-const HS = Gt ? 5e3 : -1;
+const VS = Gt ? 5e3 : -1;
 xt.compositionstart = xt.compositionupdate = t => {
     if (!t.composing) {
         t.domObserver.flush();
         let {
             state: e
         } = t, n = e.selection.$from;
-        if (e.selection.empty && (e.storedMarks || !n.textOffset && n.parentOffset && n.nodeBefore.marks.some(r => r.type.spec.inclusive === !1))) t.markCursor = t.state.storedMarks || n.marks(), go(t, !0), t.markCursor = null;
-        else if (go(t), on && e.selection.empty && n.parentOffset && !n.textOffset && n.nodeBefore.marks.length) {
+        if (e.selection.empty && (e.storedMarks || !n.textOffset && n.parentOffset && n.nodeBefore.marks.some(r => r.type.spec.inclusive === !1))) t.markCursor = t.state.storedMarks || n.marks(), bo(t, !0), t.markCursor = null;
+        else if (bo(t), on && e.selection.empty && n.parentOffset && !n.textOffset && n.nodeBefore.marks.length) {
             let r = t.domSelectionRange();
             for (let s = r.focusNode, i = r.focusOffset; s && s.nodeType == 1 && i != 0;) {
                 let o = i < 0 ? s.lastChild : s.childNodes[i - 1];
                 if (!o) break;
                 if (o.nodeType == 3) {
                     t.domSelection().collapse(o, o.nodeValue.length);
                     break
                 } else s = o, i = -1
             }
         }
         t.input.composing = !0
     }
-    vm(t, HS)
+    vm(t, VS)
 };
 xt.compositionend = (t, e) => {
     t.composing && (t.input.composing = !1, t.input.compositionEndedAt = e.timeStamp, t.input.compositionID++, vm(t, 20))
 };
 
 function vm(t, e) {
-    clearTimeout(t.input.composingTimeout), e > -1 && (t.input.composingTimeout = setTimeout(() => go(t), e))
+    clearTimeout(t.input.composingTimeout), e > -1 && (t.input.composingTimeout = setTimeout(() => bo(t), e))
 }
 
 function xm(t) {
-    for (t.composing && (t.input.composing = !1, t.input.compositionEndedAt = zS()); t.input.compositionNodes.length > 0;) t.input.compositionNodes.pop().markParentsDirty()
+    for (t.composing && (t.input.composing = !1, t.input.compositionEndedAt = jS()); t.input.compositionNodes.length > 0;) t.input.compositionNodes.pop().markParentsDirty()
 }
 
-function zS() {
+function jS() {
     let t = document.createEvent("Event");
     return t.initEvent("event", !0, !0), t.timeStamp
 }
 
-function go(t, e = !1) {
+function bo(t, e = !1) {
     if (!(Gt && t.domObserver.flushingSoon >= 0)) {
         if (t.domObserver.forceFlush(), xm(t), e || t.docView && t.docView.dirty) {
             let n = Rc(t);
             return n && !n.eq(t.state.selection) ? t.dispatch(t.state.tr.setSelection(n)) : t.updateState(t.state), !0
         }
         return !1
     }
 }
 
-function VS(t, e) {
+function US(t, e) {
     if (!t.dom.parentNode) return;
     let n = t.dom.parentNode.appendChild(document.createElement("div"));
     n.appendChild(e), n.style.cssText = "position: fixed; left: -10000px; top: 10px";
     let r = getSelection(),
         s = document.createRange();
     s.selectNodeContents(e), t.dom.blur(), r.removeAllRanges(), r.addRange(s), setTimeout(() => {
         n.parentNode && n.parentNode.removeChild(n), t.focus()
     }, 50)
 }
-const ps = _t && Zn < 15 || hs && Vw < 604;
+const ps = _t && Zn < 15 || hs && Uw < 604;
 vt.copy = xt.cut = (t, e) => {
     let n = e,
         r = t.state.selection,
         s = n.type == "cut";
     if (r.empty) return;
     let i = ps ? null : n.clipboardData,
         o = r.content(),
         {
             dom: l,
             text: a
         } = um(t, o);
-    i ? (n.preventDefault(), i.clearData(), i.setData("text/html", l.innerHTML), i.setData("text/plain", a)) : VS(t, l), s && t.dispatch(t.state.tr.deleteSelection().scrollIntoView().setMeta("uiEvent", "cut"))
+    i ? (n.preventDefault(), i.clearData(), i.setData("text/html", l.innerHTML), i.setData("text/plain", a)) : US(t, l), s && t.dispatch(t.state.tr.deleteSelection().scrollIntoView().setMeta("uiEvent", "cut"))
 };
 
-function jS(t) {
+function WS(t) {
     return t.openStart == 0 && t.openEnd == 0 && t.content.childCount == 1 ? t.content.firstChild : null
 }
 
-function US(t, e) {
+function qS(t, e) {
     if (!t.dom.parentNode) return;
     let n = t.input.shiftKey || t.state.selection.$from.parent.type.spec.code,
         r = t.dom.parentNode.appendChild(document.createElement(n ? "textarea" : "div"));
     n || (r.contentEditable = "true"), r.style.cssText = "position: fixed; left: -10000px; top: 10px", r.focus(), setTimeout(() => {
         t.focus(), r.parentNode && r.parentNode.removeChild(r), n ? pi(t, r.value, null, t.input.shiftKey, e) : pi(t, r.textContent, r.innerHTML, t.input.shiftKey, e)
     }, 50)
 }
 
 function pi(t, e, n, r, s) {
     let i = dm(t, e, n, r, t.state.selection.$from);
     if (t.someProp("handlePaste", a => a(t, s, i || q.empty))) return !0;
     if (!i) return !1;
-    let o = jS(i),
+    let o = WS(i),
         l = o ? t.state.tr.replaceSelectionWith(o, t.input.shiftKey) : t.state.tr.replaceSelection(i);
     return t.dispatch(l.scrollIntoView().setMeta("paste", !0).setMeta("uiEvent", "paste")), !0
 }
 xt.paste = (t, e) => {
     let n = e;
     if (t.composing && !Gt) return;
     let r = ps ? null : n.clipboardData;
-    r && pi(t, r.getData("text/plain"), r.getData("text/html"), t.input.shiftKey, n) ? n.preventDefault() : US(t, n)
+    r && pi(t, r.getData("text/plain"), r.getData("text/html"), t.input.shiftKey, n) ? n.preventDefault() : qS(t, n)
 };
-class WS {
+class KS {
     constructor(e, n) {
         this.slice = e, this.move = n
     }
 }
 const km = Ft ? "altKey" : "ctrlKey";
 vt.dragstart = (t, e) => {
     let n = e,
@@ -13695,15 +13698,15 @@
         }
     }
     let o = t.state.selection.content(),
         {
             dom: l,
             text: a
         } = um(t, o);
-    n.dataTransfer.clearData(), n.dataTransfer.setData(ps ? "Text" : "text/html", l.innerHTML), n.dataTransfer.effectAllowed = "copyMove", ps || n.dataTransfer.setData("text/plain", a), t.dragging = new WS(o, !n[km])
+    n.dataTransfer.clearData(), n.dataTransfer.setData(ps ? "Text" : "text/html", l.innerHTML), n.dataTransfer.effectAllowed = "copyMove", ps || n.dataTransfer.setData("text/plain", a), t.dragging = new KS(o, !n[km])
 };
 vt.dragend = t => {
     let e = t.dragging;
     window.setTimeout(() => {
         t.dragging == e && (t.dragging = null)
     }, 50)
 };
@@ -13871,15 +13874,15 @@
 const Wr = [],
     Rr = {};
 class Je {
     constructor(e, n) {
         this.local = e.length ? e : Wr, this.children = n.length ? n : Wr
     }
     static create(e, n) {
-        return n.length ? yo(n, e, 0, Rr) : at
+        return n.length ? vo(n, e, 0, Rr) : at
     }
     find(e, n, r) {
         let s = [];
         return this.findInner(e ?? 0, n ?? 1e9, s, 0, r), s
     }
     findInner(e, n, r, s, i) {
         for (let o = 0; o < this.local.length; o++) {
@@ -13897,27 +13900,27 @@
     }
     mapInner(e, n, r, s, i) {
         let o;
         for (let l = 0; l < this.local.length; l++) {
             let a = this.local[l].map(e, r, s);
             a && a.type.valid(n, a) ? (o || (o = [])).push(a) : i.onRemove && i.onRemove(this.local[l].spec)
         }
-        return this.children.length ? qS(this.children, o || [], e, n, r, s, i) : o ? new Je(o.sort(Dr), Wr) : at
+        return this.children.length ? JS(this.children, o || [], e, n, r, s, i) : o ? new Je(o.sort(Dr), Wr) : at
     }
     add(e, n) {
         return n.length ? this == at ? Je.create(e, n) : this.addInner(e, n, 0) : this
     }
     addInner(e, n, r) {
         let s, i = 0;
         e.forEach((l, a) => {
             let c = a + r,
                 u;
             if (u = Sm(n, l, c)) {
                 for (s || (s = this.children.slice()); i < s.length && s[i] < a;) i += 3;
-                s[i] == a ? s[i + 2] = s[i + 2].addInner(l, u, c + 1) : s.splice(i, 0, a, a + l.nodeSize, yo(u, l, c + 1, Rr)), i += 3
+                s[i] == a ? s[i + 2] = s[i + 2].addInner(l, u, c + 1) : s.splice(i, 0, a, a + l.nodeSize, vo(u, l, c + 1, Rr)), i += 3
             }
         });
         let o = wm(i ? _m(n) : n, -r);
         for (let l = 0; l < o.length; l++) o[l].type.valid(e, o[l]) || o.splice(l--, 1);
         return new Je(o.length ? this.local.concat(o).sort(Dr) : this.local, s || this.children)
     }
     remove(e) {
@@ -14033,15 +14036,15 @@
                 return e[0];
             default:
                 return new Kn(e.every(n => n instanceof Je) ? e : e.reduce((n, r) => n.concat(r instanceof Je ? r : r.members), []))
         }
     }
 }
 
-function qS(t, e, n, r, s, i, o) {
+function JS(t, e, n, r, s, i, o) {
     let l = t.slice();
     for (let c = 0, u = i; c < n.maps.length; c++) {
         let d = 0;
         n.maps[c].forEach((f, h, p, g) => {
             let v = g - p - (h - f);
             for (let x = 0; x < l.length; x += 3) {
                 let w = l[x + 1];
@@ -14073,16 +14076,16 @@
                 } = r.content.findIndex(d),
                 v = r.maybeChild(p);
             if (v && g == d && g + v.nodeSize == h) {
                 let x = l[c + 2].mapInner(n, v, u + 1, t[c] + i + 1, o);
                 x != at ? (l[c] = d, l[c + 1] = h, l[c + 2] = x) : (l[c + 1] = -2, a = !0)
             } else a = !0
         } if (a) {
-        let c = KS(l, t, e, n, s, i, o),
-            u = yo(c, r, 0, o);
+        let c = GS(l, t, e, n, s, i, o),
+            u = vo(c, r, 0, o);
         e = u.local;
         for (let d = 0; d < l.length; d += 3) l[d + 1] < 0 && (l.splice(d, 3), d -= 3);
         for (let d = 0, f = 0; d < u.children.length; d += 3) {
             let h = u.children[d];
             for (; f < l.length && l[f] < h;) f += 3;
             l.splice(f, 0, u.children[d], u.children[d + 1], u.children[d + 2])
         }
@@ -14096,15 +14099,15 @@
     for (let r = 0; r < t.length; r++) {
         let s = t[r];
         n.push(new zt(s.from + e, s.to + e, s.type))
     }
     return n
 }
 
-function KS(t, e, n, r, s, i, o) {
+function GS(t, e, n, r, s, i, o) {
     function l(a, c) {
         for (let u = 0; u < a.local.length; u++) {
             let d = a.local[u].map(r, s, c);
             d ? n.push(d) : o.onRemove && o.onRemove(a.local[u].spec)
         }
         for (let u = 0; u < a.children.length; u += 3) l(a.children[u + 2], a.children[u] + c + 1)
     }
@@ -14122,22 +14125,22 @@
 
 function _m(t) {
     let e = [];
     for (let n = 0; n < t.length; n++) t[n] != null && e.push(t[n]);
     return e
 }
 
-function yo(t, e, n, r) {
+function vo(t, e, n, r) {
     let s = [],
         i = !1;
     e.forEach((l, a) => {
         let c = Sm(t, l, a + n);
         if (c) {
             i = !0;
-            let u = yo(c, l, n + a + 1, r);
+            let u = vo(c, l, n + a + 1, r);
             u != at && s.push(a, a + l.nodeSize, u)
         }
     });
     let o = wm(i ? _m(t) : t, -n).sort(Dr);
     for (let l = 0; l < o.length; l++) o[l].type.valid(e, o[l]) || (r.onRemove && r.onRemove(o[l].spec), o.splice(l--, 1));
     return o.length || s.length ? new Je(o, s) : at
 }
@@ -14173,43 +14176,43 @@
 function Ul(t) {
     let e = [];
     return t.someProp("decorations", n => {
         let r = n(t.state);
         r && r != at && e.push(r)
     }), t.cursorWrapper && e.push(Je.create(t.state.doc, [t.cursorWrapper.deco])), Kn.from(e)
 }
-const JS = {
+const YS = {
         childList: !0,
         characterData: !0,
         characterDataOldValue: !0,
         attributes: !0,
         attributeOldValue: !0,
         subtree: !0
     },
-    GS = _t && Zn <= 11;
-class YS {
+    XS = _t && Zn <= 11;
+class QS {
     constructor() {
         this.anchorNode = null, this.anchorOffset = 0, this.focusNode = null, this.focusOffset = 0
     }
     set(e) {
         this.anchorNode = e.anchorNode, this.anchorOffset = e.anchorOffset, this.focusNode = e.focusNode, this.focusOffset = e.focusOffset
     }
     clear() {
         this.anchorNode = this.focusNode = null
     }
     eq(e) {
         return e.anchorNode == this.anchorNode && e.anchorOffset == this.anchorOffset && e.focusNode == this.focusNode && e.focusOffset == this.focusOffset
     }
 }
-class XS {
+class ZS {
     constructor(e, n) {
-        this.view = e, this.handleDOMChange = n, this.queue = [], this.flushingSoon = -1, this.observer = null, this.currentSelection = new YS, this.onCharData = null, this.suppressingSelectionUpdates = !1, this.observer = window.MutationObserver && new window.MutationObserver(r => {
+        this.view = e, this.handleDOMChange = n, this.queue = [], this.flushingSoon = -1, this.observer = null, this.currentSelection = new QS, this.onCharData = null, this.suppressingSelectionUpdates = !1, this.observer = window.MutationObserver && new window.MutationObserver(r => {
             for (let s = 0; s < r.length; s++) this.queue.push(r[s]);
             _t && Zn <= 11 && r.some(s => s.type == "childList" && s.removedNodes.length || s.type == "characterData" && s.oldValue.length > s.target.nodeValue.length) ? this.flushSoon() : this.flush()
-        }), GS && (this.onCharData = r => {
+        }), XS && (this.onCharData = r => {
             this.queue.push({
                 target: r.target,
                 type: "characterData",
                 oldValue: r.prevValue
             }), this.flushSoon()
         }), this.onSelectionChange = this.onSelectionChange.bind(this)
     }
@@ -14218,15 +14221,15 @@
             this.flushingSoon = -1, this.flush()
         }, 20))
     }
     forceFlush() {
         this.flushingSoon > -1 && (window.clearTimeout(this.flushingSoon), this.flushingSoon = -1, this.flush())
     }
     start() {
-        this.observer && (this.observer.takeRecords(), this.observer.observe(this.view.dom, JS)), this.onCharData && this.view.dom.addEventListener("DOMCharacterDataModified", this.onCharData), this.connectSelection()
+        this.observer && (this.observer.takeRecords(), this.observer.observe(this.view.dom, YS)), this.onCharData && this.view.dom.addEventListener("DOMCharacterDataModified", this.onCharData), this.connectSelection()
     }
     stop() {
         if (this.observer) {
             let e = this.observer.takeRecords();
             if (e.length) {
                 for (let n = 0; n < e.length; n++) this.queue.push(e[n]);
                 window.setTimeout(() => this.flush(), 20)
@@ -14295,15 +14298,15 @@
             if (u.length == 2) {
                 let d = u[0],
                     f = u[1];
                 d.parentNode && d.parentNode.parentNode == f.parentNode ? f.remove() : d.remove()
             }
         }
         let c = null;
-        i < 0 && s && e.input.lastFocus > Date.now() - 200 && Math.max(e.input.lastTouch, e.input.lastClick.time) < Date.now() - 300 && Qo(r) && (c = Rc(e)) && c.eq(ve.near(e.state.doc.resolve(0), 1)) ? (e.input.lastFocus = 0, An(e), this.currentSelection.set(r), e.scrollToSelection()) : (i > -1 || s) && (i > -1 && (e.docView.markDirty(i, o), QS(e)), this.handleDOMChange(i, o, l, a), e.docView && e.docView.dirty ? e.updateState(e.state) : this.currentSelection.eq(r) || An(e), this.currentSelection.set(r))
+        i < 0 && s && e.input.lastFocus > Date.now() - 200 && Math.max(e.input.lastTouch, e.input.lastClick.time) < Date.now() - 300 && Qo(r) && (c = Rc(e)) && c.eq(ve.near(e.state.doc.resolve(0), 1)) ? (e.input.lastFocus = 0, An(e), this.currentSelection.set(r), e.scrollToSelection()) : (i > -1 || s) && (i > -1 && (e.docView.markDirty(i, o), e_(e)), this.handleDOMChange(i, o, l, a), e.docView && e.docView.dirty ? e.updateState(e.state) : this.currentSelection.eq(r) || An(e), this.currentSelection.set(r))
     }
     registerMutation(e, n) {
         if (n.indexOf(e.target) > -1) return null;
         let r = this.view.docView.nearestDesc(e.target);
         if (e.type == "attributes" && (r == this.view.docView || e.attributeName == "contenteditable" || e.attributeName == "style" && !e.oldValue && !e.target.getAttribute("style")) || !r || r.ignoreMutation(e)) return null;
         if (e.type == "childList") {
             for (let u = 0; u < e.addedNodes.length; u++) n.push(e.addedNodes[u]);
@@ -14338,22 +14341,22 @@
             typeOver: e.target.nodeValue == e.oldValue
         }
     }
 }
 let Yd = new WeakMap,
     Xd = !1;
 
-function QS(t) {
+function e_(t) {
     if (!Yd.has(t) && (Yd.set(t, null), ["normal", "nowrap", "pre-line"].indexOf(getComputedStyle(t.dom).whiteSpace) !== -1)) {
         if (t.requiresGeckoHackNode = on, Xd) return;
         console.warn("ProseMirror expects the CSS white-space property to be set, preferably to 'pre-wrap'. It is recommended to load style/prosemirror.css from the prosemirror-view package."), Xd = !0
     }
 }
 
-function ZS(t) {
+function t_(t) {
     let e;
 
     function n(a) {
         a.preventDefault(), a.stopImmediatePropagation(), e = a.getTargetRanges()[0]
     }
     t.dom.addEventListener("beforeinput", n, !0), document.execCommand("indent"), t.dom.removeEventListener("beforeinput", n, !0);
     let r = e.startContainer,
@@ -14365,15 +14368,15 @@
         anchorNode: r,
         anchorOffset: s,
         focusNode: i,
         focusOffset: o
     }
 }
 
-function e_(t, e, n) {
+function n_(t, e, n) {
     let {
         node: r,
         fromOffset: s,
         toOffset: i,
         from: o,
         to: l
     } = t.docView.parseRange(e, n), a = t.domSelectionRange(), c, u = a.anchorNode;
@@ -14401,15 +14404,15 @@
             topNode: h.parent,
             topMatch: h.parent.contentMatchAt(h.index()),
             topOpen: !0,
             from: s,
             to: i,
             preserveWhitespace: h.parent.type.whitespace == "pre" ? "full" : !0,
             findPositions: c,
-            ruleFromNode: t_,
+            ruleFromNode: r_,
             context: h
         });
     if (c && c[0].pos != null) {
         let v = c[0].pos,
             x = c[1] && c[1].pos;
         x == null && (x = v), p = {
             anchor: v + o,
@@ -14420,15 +14423,15 @@
         doc: g,
         sel: p,
         from: o,
         to: l
     }
 }
 
-function t_(t) {
+function r_(t) {
     let e = t.pmViewDesc;
     if (e) return e.parseRule();
     if (t.nodeName == "BR" && t.parentNode) {
         if (bt && /^(ul|ol)$/i.test(t.parentNode.nodeName)) {
             let n = document.createElement("div");
             return n.appendChild(document.createElement("li")), {
                 skip: n
@@ -14437,38 +14440,38 @@
             ignore: !0
         }
     } else if (t.nodeName == "IMG" && t.getAttribute("mark-placeholder")) return {
         ignore: !0
     };
     return null
 }
-const n_ = /^(a|abbr|acronym|b|bd[io]|big|br|button|cite|code|data(list)?|del|dfn|em|i|ins|kbd|label|map|mark|meter|output|q|ruby|s|samp|small|span|strong|su[bp]|time|u|tt|var)$/i;
+const s_ = /^(a|abbr|acronym|b|bd[io]|big|br|button|cite|code|data(list)?|del|dfn|em|i|ins|kbd|label|map|mark|meter|output|q|ruby|s|samp|small|span|strong|su[bp]|time|u|tt|var)$/i;
 
-function r_(t, e, n, r, s) {
+function i_(t, e, n, r, s) {
     if (e < 0) {
         let N = t.input.lastSelectionTime > Date.now() - 50 ? t.input.lastSelectionOrigin : null,
             G = Rc(t, N);
         if (G && !t.state.selection.eq(G)) {
             if (dt && Gt && t.input.lastKeyCode === 13 && Date.now() - 100 < t.input.lastKeyCodeTime && t.someProp("handleKeyDown", ne => ne(t, wr(13, "Enter")))) return;
             let J = t.state.tr.setSelection(G);
             N == "pointer" ? J.setMeta("pointer", !0) : N == "key" && J.scrollIntoView(), t.composing && J.setMeta("composition", t.input.compositionID), t.dispatch(J)
         }
         return
     }
     let i = t.state.doc.resolve(e),
         o = i.sharedDepth(n);
     e = i.before(o + 1), n = t.state.doc.resolve(n).after(o + 1);
     let l = t.state.selection,
-        a = e_(t, e, n),
+        a = n_(t, e, n),
         c = t.state.doc,
         u = c.slice(a.from, a.to),
         d, f;
     t.input.lastKeyCode === 8 && Date.now() - 100 < t.input.lastKeyCodeTime ? (d = t.state.selection.to, f = "end") : (d = t.state.selection.from, f = "start"), t.input.lastKeyCode = null;
-    let h = o_(u.content, a.doc.content, a.from, d, f);
-    if ((hs && t.input.lastIOSEnter > Date.now() - 225 || Gt) && s.some(N => N.nodeType == 1 && !n_.test(N.nodeName)) && (!h || h.endA >= h.endB) && t.someProp("handleKeyDown", N => N(t, wr(13, "Enter")))) {
+    let h = a_(u.content, a.doc.content, a.from, d, f);
+    if ((hs && t.input.lastIOSEnter > Date.now() - 225 || Gt) && s.some(N => N.nodeType == 1 && !s_.test(N.nodeName)) && (!h || h.endA >= h.endB) && t.someProp("handleKeyDown", N => N(t, wr(13, "Enter")))) {
         t.input.lastIOSEnter = 0;
         return
     }
     if (!h)
         if (r && l instanceof xe && !l.empty && l.$head.sameParent(l.$anchor) && !t.composing && !(a.sel && a.sel.anchor != a.sel.head)) h = {
             start: l.from,
             endA: l.to,
@@ -14496,29 +14499,29 @@
         v = c.resolve(h.start),
         x = p.sameParent(g) && p.parent.inlineContent && v.end() >= h.endA,
         w;
     if ((hs && t.input.lastIOSEnter > Date.now() - 225 && (!x || s.some(N => N.nodeName == "DIV" || N.nodeName == "P")) || !x && p.pos < a.doc.content.size && (w = ve.findFrom(a.doc.resolve(p.pos + 1), 1, !0)) && w.head == g.pos) && t.someProp("handleKeyDown", N => N(t, wr(13, "Enter")))) {
         t.input.lastIOSEnter = 0;
         return
     }
-    if (t.state.selection.anchor > h.start && i_(c, h.start, h.endA, p, g) && t.someProp("handleKeyDown", N => N(t, wr(8, "Backspace")))) {
+    if (t.state.selection.anchor > h.start && l_(c, h.start, h.endA, p, g) && t.someProp("handleKeyDown", N => N(t, wr(8, "Backspace")))) {
         Gt && dt && t.domObserver.suppressSelectionUpdates();
         return
     }
     dt && Gt && h.endB == h.start && (t.input.lastAndroidDelete = Date.now()), Gt && !x && p.start() != g.start() && g.parentOffset == 0 && p.depth == g.depth && a.sel && a.sel.anchor == a.sel.head && a.sel.head == h.endA && (h.endB -= 2, g = a.doc.resolveNoCache(h.endB - a.from), setTimeout(() => {
         t.someProp("handleKeyDown", function(N) {
             return N(t, wr(13, "Enter"))
         })
     }, 20));
     let S = h.start,
         y = h.endA,
         I, T, V;
     if (x) {
         if (p.pos == g.pos) _t && Zn <= 11 && p.parentOffset == 0 && (t.domObserver.suppressSelectionUpdates(), setTimeout(() => An(t), 20)), I = t.state.tr.delete(S, y), T = c.resolve(h.start).marksAcross(c.resolve(h.endA));
-        else if (h.endA == h.endB && (V = s_(p.parent.content.cut(p.parentOffset, g.parentOffset), v.parent.content.cut(v.parentOffset, h.endA - v.start())))) I = t.state.tr, V.type == "add" ? I.addMark(S, y, V.mark) : I.removeMark(S, y, V.mark);
+        else if (h.endA == h.endB && (V = o_(p.parent.content.cut(p.parentOffset, g.parentOffset), v.parent.content.cut(v.parentOffset, h.endA - v.start())))) I = t.state.tr, V.type == "add" ? I.addMark(S, y, V.mark) : I.removeMark(S, y, V.mark);
         else if (p.parent.child(p.index()).isText && p.index() == g.index() - (g.textOffset ? 0 : 1)) {
             let N = p.parent.textBetween(p.parentOffset, g.parentOffset);
             if (t.someProp("handleTextInput", G => G(t, S, y, N))) return;
             I = t.state.tr.insertText(N, S, y)
         }
     }
     if (I || (I = t.state.tr.replace(S, y, a.doc.slice(h.start - a.from, h.endB - a.from))), a.sel) {
@@ -14528,15 +14531,15 @@
     T && I.ensureMarks(T), t.composing && I.setMeta("composition", t.input.compositionID), t.dispatch(I.scrollIntoView())
 }
 
 function Qd(t, e, n) {
     return Math.max(n.anchor, n.head) > e.content.size ? null : Dc(t, e.resolve(n.anchor), e.resolve(n.head))
 }
 
-function s_(t, e) {
+function o_(t, e) {
     let n = t.firstChild.marks,
         r = e.firstChild.marks,
         s = n,
         i = r,
         o, l, a;
     for (let u = 0; u < r.length; u++) s = r[u].removeFromSet(s);
     for (let u = 0; u < n.length; u++) i = n[u].removeFromSet(i);
@@ -14547,15 +14550,15 @@
     for (let u = 0; u < e.childCount; u++) c.push(a(e.child(u)));
     if ($.from(c).eq(t)) return {
         mark: l,
         type: o
     }
 }
 
-function i_(t, e, n, r, s) {
+function l_(t, e, n, r, s) {
     if (!r.parent.isTextblock || n - e <= s.pos - r.pos || Wl(r, !0, !1) < s.pos) return !1;
     let i = t.resolve(e);
     if (i.parentOffset < i.parent.content.size || !i.parent.isTextblock) return !1;
     let o = t.resolve(Wl(i, !0, !0));
     return !o.parent.isTextblock || o.pos > n || Wl(o, !0, !1) < n ? !1 : r.parent.content.cut(r.parentOffset).eq(o.parent.content)
 }
 
@@ -14566,15 +14569,15 @@
     if (n) {
         let i = t.node(r).maybeChild(t.indexAfter(r));
         for (; i && !i.isLeaf;) i = i.firstChild, s++
     }
     return s
 }
 
-function o_(t, e, n, r, s) {
+function a_(t, e, n, r, s) {
     let i = t.findDiffStart(e, n);
     if (i == null) return null;
     let {
         a: o,
         b: l
     } = t.findDiffEnd(e, n + t.size, n + e.size);
     if (s == "end") {
@@ -14590,17 +14593,17 @@
     }
     return {
         start: i,
         endA: o,
         endB: l
     }
 }
-class l_ {
+class c_ {
     constructor(e, n) {
-        this._root = null, this.focused = !1, this.trackWrites = null, this.mounted = !1, this.markCursor = null, this.cursorWrapper = null, this.lastSelectedViewDesc = void 0, this.input = new TS, this.prevDirectPlugins = [], this.pluginViews = [], this.requiresGeckoHackNode = !1, this.dragging = null, this._props = n, this.state = n.state, this.directPlugins = n.plugins || [], this.directPlugins.forEach(rf), this.dispatch = this.dispatch.bind(this), this.dom = e && e.mount || document.createElement("div"), e && (e.appendChild ? e.appendChild(this.dom) : typeof e == "function" ? e(this.dom) : e.mount && (this.mounted = !0)), this.editable = tf(this), ef(this), this.nodeViews = nf(this), this.docView = Pd(this.state.doc, Zd(this), Ul(this), this.dom, this), this.domObserver = new XS(this, (r, s, i, o) => r_(this, r, s, i, o)), this.domObserver.start(), OS(this), this.updatePluginViews()
+        this._root = null, this.focused = !1, this.trackWrites = null, this.mounted = !1, this.markCursor = null, this.cursorWrapper = null, this.lastSelectedViewDesc = void 0, this.input = new MS, this.prevDirectPlugins = [], this.pluginViews = [], this.requiresGeckoHackNode = !1, this.dragging = null, this._props = n, this.state = n.state, this.directPlugins = n.plugins || [], this.directPlugins.forEach(rf), this.dispatch = this.dispatch.bind(this), this.dom = e && e.mount || document.createElement("div"), e && (e.appendChild ? e.appendChild(this.dom) : typeof e == "function" ? e(this.dom) : e.mount && (this.mounted = !0)), this.editable = tf(this), ef(this), this.nodeViews = nf(this), this.docView = Pd(this.state.doc, Zd(this), Ul(this), this.dom, this), this.domObserver = new ZS(this, (r, s, i, o) => i_(this, r, s, i, o)), this.domObserver.start(), AS(this), this.updatePluginViews()
     }
     get composing() {
         return this.input.composing
     }
     get props() {
         if (this._props.state != this.state) {
             let e = this._props;
@@ -14629,32 +14632,32 @@
         let r = this.state,
             s = !1,
             i = !1;
         e.storedMarks && this.composing && (xm(this), i = !0), this.state = e;
         let o = r.plugins != e.plugins || this._props.plugins != n.plugins;
         if (o || this._props.plugins != n.plugins || this._props.nodeViews != n.nodeViews) {
             let f = nf(this);
-            c_(f, this.nodeViews) && (this.nodeViews = f, s = !0)
+            d_(f, this.nodeViews) && (this.nodeViews = f, s = !0)
         }(o || n.handleDOMEvents != this._props.handleDOMEvents) && za(this), this.editable = tf(this), ef(this);
         let l = Ul(this),
             a = Zd(this),
             c = r.plugins != e.plugins && !r.doc.eq(e.doc) ? "reset" : e.scrollToSelection > r.scrollToSelection ? "to selection" : "preserve",
             u = s || !this.docView.matchesNode(e.doc, a, l);
         (u || !e.selection.eq(r.selection)) && (i = !0);
-        let d = c == "preserve" && i && this.dom.style.overflowAnchor == null && Ww(this);
+        let d = c == "preserve" && i && this.dom.style.overflowAnchor == null && Kw(this);
         if (i) {
             this.domObserver.stop();
-            let f = u && (_t || dt) && !this.composing && !r.selection.empty && !e.selection.empty && a_(r.selection, e.selection);
+            let f = u && (_t || dt) && !this.composing && !r.selection.empty && !e.selection.empty && u_(r.selection, e.selection);
             if (u) {
                 let h = dt ? this.trackWrites = this.domSelectionRange().focusNode : null;
                 (s || !this.docView.update(e.doc, a, l, this)) && (this.docView.updateOuterDeco([]), this.docView.destroy(), this.docView = Pd(e.doc, a, l, this.dom, this)), h && !this.trackWrites && (f = !0)
             }
-            f || !(this.input.mouseDown && this.domObserver.currentSelection.eq(this.domSelectionRange()) && gS(this)) ? An(this, f) : (om(this, e.selection), this.domObserver.setCurSelection()), this.domObserver.start()
+            f || !(this.input.mouseDown && this.domObserver.currentSelection.eq(this.domSelectionRange()) && bS(this)) ? An(this, f) : (om(this, e.selection), this.domObserver.setCurSelection()), this.domObserver.start()
         }
-        this.updatePluginViews(r), c == "reset" ? this.dom.scrollTop = 0 : c == "to selection" ? this.scrollToSelection() : d && qw(d)
+        this.updatePluginViews(r), c == "reset" ? this.dom.scrollTop = 0 : c == "to selection" ? this.scrollToSelection() : d && Jw(d)
     }
     scrollToSelection() {
         let e = this.domSelectionRange().focusNode;
         if (!this.someProp("handleScrollToSelection", n => n(this)))
             if (this.state.selection instanceof se) {
                 let n = this.docView.domAfterPos(this.state.selection.from);
                 n.nodeType == 1 && Md(this, n.getBoundingClientRect(), e)
@@ -14706,26 +14709,26 @@
                 e = e.parentElement
             }
             return !0
         }
         return this.root.activeElement == this.dom
     }
     focus() {
-        this.domObserver.stop(), this.editable && Kw(this.dom), An(this), this.domObserver.start()
+        this.domObserver.stop(), this.editable && Gw(this.dom), An(this), this.domObserver.start()
     }
     get root() {
         let e = this._root;
         if (e == null) {
             for (let n = this.dom.parentNode; n; n = n.parentNode)
                 if (n.nodeType == 9 || n.nodeType == 11 && n.host) return n.getSelection || (Object.getPrototypeOf(n).getSelection = () => n.ownerDocument.getSelection()), this._root = n
         }
         return e || document
     }
     posAtCoords(e) {
-        return Qw(this, e)
+        return eS(this, e)
     }
     coordsAtPos(e, n = 1) {
         return Qp(this, e, n)
     }
     domAtPos(e, n = 0) {
         return this.docView.domFromPos(e, n)
     }
@@ -14735,37 +14738,37 @@
     }
     posAtDOM(e, n, r = -1) {
         let s = this.docView.posFromDOM(e, n, r);
         if (s == null) throw new RangeError("DOM position not inside the editor");
         return s
     }
     endOfTextblock(e, n) {
-        return rS(this, n || this.state, e)
+        return iS(this, n || this.state, e)
     }
     pasteHTML(e, n) {
         return pi(this, "", e, !1, n || new ClipboardEvent("paste"))
     }
     pasteText(e, n) {
         return pi(this, e, null, !0, n || new ClipboardEvent("paste"))
     }
     destroy() {
-        this.docView && (MS(this), this.destroyPluginViews(), this.mounted ? (this.docView.update(this.state.doc, [], Ul(this), this), this.dom.textContent = "") : this.dom.parentNode && this.dom.parentNode.removeChild(this.dom), this.docView.destroy(), this.docView = null)
+        this.docView && (NS(this), this.destroyPluginViews(), this.mounted ? (this.docView.update(this.state.doc, [], Ul(this), this), this.dom.textContent = "") : this.dom.parentNode && this.dom.parentNode.removeChild(this.dom), this.docView.destroy(), this.docView = null)
     }
     get isDestroyed() {
         return this.docView == null
     }
     dispatchEvent(e) {
-        return NS(this, e)
+        return DS(this, e)
     }
     dispatch(e) {
         let n = this._props.dispatchTransaction;
         n ? n.call(this, e) : this.updateState(this.state.apply(e))
     }
     domSelectionRange() {
-        return bt && this.root.nodeType === 11 && Fw(this.dom.ownerDocument) == this.dom ? ZS(this) : this.domSelection()
+        return bt && this.root.nodeType === 11 && Hw(this.dom.ownerDocument) == this.dom ? t_(this) : this.domSelection()
     }
     domSelection() {
         return this.root.getSelection()
     }
 }
 
 function Zd(t) {
@@ -14789,29 +14792,29 @@
     } else t.cursorWrapper = null
 }
 
 function tf(t) {
     return !t.someProp("editable", e => e(t.state) === !1)
 }
 
-function a_(t, e) {
+function u_(t, e) {
     let n = Math.min(t.$anchor.sharedDepth(t.head), e.$anchor.sharedDepth(e.head));
     return t.$anchor.start(n) != e.$anchor.start(n)
 }
 
 function nf(t) {
     let e = Object.create(null);
 
     function n(r) {
         for (let s in r) Object.prototype.hasOwnProperty.call(e, s) || (e[s] = r[s])
     }
     return t.someProp("nodeViews", n), t.someProp("markViews", n), e
 }
 
-function c_(t, e) {
+function d_(t, e) {
     let n = 0,
         r = 0;
     for (let s in t) {
         if (t[s] != e[s]) return !0;
         n++
     }
     for (let s in e) r++;
@@ -14871,15 +14874,15 @@
         191: "/",
         192: "`",
         219: "[",
         220: "\\",
         221: "]",
         222: "'"
     },
-    bo = {
+    xo = {
         48: ")",
         49: "!",
         50: "@",
         51: "#",
         52: "$",
         53: "%",
         54: "^",
@@ -14898,68 +14901,68 @@
         192: "~",
         219: "{",
         220: "|",
         221: "}",
         222: '"'
     },
     sf = typeof navigator < "u" && /Chrome\/(\d+)/.exec(navigator.userAgent),
-    u_ = typeof navigator < "u" && /Mac/.test(navigator.platform),
-    d_ = typeof navigator < "u" && /MSIE \d|Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(navigator.userAgent),
-    f_ = u_ || sf && +sf[1] < 57;
+    f_ = typeof navigator < "u" && /Mac/.test(navigator.platform),
+    h_ = typeof navigator < "u" && /MSIE \d|Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(navigator.userAgent),
+    p_ = f_ || sf && +sf[1] < 57;
 for (var it = 0; it < 10; it++) sr[48 + it] = sr[96 + it] = String(it);
 for (var it = 1; it <= 24; it++) sr[it + 111] = "F" + it;
-for (var it = 65; it <= 90; it++) sr[it] = String.fromCharCode(it + 32), bo[it] = String.fromCharCode(it);
-for (var ql in sr) bo.hasOwnProperty(ql) || (bo[ql] = sr[ql]);
+for (var it = 65; it <= 90; it++) sr[it] = String.fromCharCode(it + 32), xo[it] = String.fromCharCode(it);
+for (var ql in sr) xo.hasOwnProperty(ql) || (xo[ql] = sr[ql]);
 
-function h_(t) {
-    var e = f_ && (t.ctrlKey || t.altKey || t.metaKey) || d_ && t.shiftKey && t.key && t.key.length == 1 || t.key == "Unidentified",
-        n = !e && t.key || (t.shiftKey ? bo : sr)[t.keyCode] || t.key || "Unidentified";
+function m_(t) {
+    var e = p_ && (t.ctrlKey || t.altKey || t.metaKey) || h_ && t.shiftKey && t.key && t.key.length == 1 || t.key == "Unidentified",
+        n = !e && t.key || (t.shiftKey ? xo : sr)[t.keyCode] || t.key || "Unidentified";
     return n == "Esc" && (n = "Escape"), n == "Del" && (n = "Delete"), n == "Left" && (n = "ArrowLeft"), n == "Up" && (n = "ArrowUp"), n == "Right" && (n = "ArrowRight"), n == "Down" && (n = "ArrowDown"), n
 }
-const p_ = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : !1;
+const g_ = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : !1;
 
-function m_(t) {
+function y_(t) {
     let e = t.split(/-(?!$)/),
         n = e[e.length - 1];
     n == "Space" && (n = " ");
     let r, s, i, o;
     for (let l = 0; l < e.length - 1; l++) {
         let a = e[l];
         if (/^(cmd|meta|m)$/i.test(a)) o = !0;
         else if (/^a(lt)?$/i.test(a)) r = !0;
         else if (/^(c|ctrl|control)$/i.test(a)) s = !0;
         else if (/^s(hift)?$/i.test(a)) i = !0;
-        else if (/^mod$/i.test(a)) p_ ? o = !0 : s = !0;
+        else if (/^mod$/i.test(a)) g_ ? o = !0 : s = !0;
         else throw new Error("Unrecognized modifier name: " + a)
     }
     return r && (n = "Alt-" + n), s && (n = "Ctrl-" + n), o && (n = "Meta-" + n), i && (n = "Shift-" + n), n
 }
 
-function g_(t) {
+function b_(t) {
     let e = Object.create(null);
-    for (let n in t) e[m_(n)] = t[n];
+    for (let n in t) e[y_(n)] = t[n];
     return e
 }
 
 function Kl(t, e, n = !0) {
     return e.altKey && (t = "Alt-" + t), e.ctrlKey && (t = "Ctrl-" + t), e.metaKey && (t = "Meta-" + t), n && e.shiftKey && (t = "Shift-" + t), t
 }
 
-function y_(t) {
+function v_(t) {
     return new Mt({
         props: {
             handleKeyDown: Cm(t)
         }
     })
 }
 
 function Cm(t) {
-    let e = g_(t);
+    let e = b_(t);
     return function(n, r) {
-        let s = h_(r),
+        let s = m_(r),
             i, o = e[Kl(s, r)];
         if (o && o(n.state, n.dispatch, n)) return !0;
         if (s.length == 1 && s != " ") {
             if (r.shiftKey) {
                 let l = e[Kl(s, r, !1)];
                 if (l && l(n.state, n.dispatch, n)) return !0
             }
@@ -14967,24 +14970,24 @@
                 let l = e[Kl(i, r)];
                 if (l && l(n.state, n.dispatch, n)) return !0
             }
         }
         return !1
     }
 }
-const b_ = (t, e) => t.selection.empty ? !1 : (e && e(t.tr.deleteSelection().scrollIntoView()), !0);
+const x_ = (t, e) => t.selection.empty ? !1 : (e && e(t.tr.deleteSelection().scrollIntoView()), !0);
 
-function v_(t, e) {
+function k_(t, e) {
     let {
         $cursor: n
     } = t.selection;
     return !n || (e ? !e.endOfTextblock("backward", t) : n.parentOffset > 0) ? null : n
 }
-const x_ = (t, e, n) => {
-    let r = v_(t, n);
+const w_ = (t, e, n) => {
+    let r = k_(t, n);
     if (!r) return !1;
     let s = Em(r);
     if (!s) {
         let o = r.blockRange(),
             l = o && Ms(o);
         return l == null ? !1 : (e && e(t.tr.lift(o, l).scrollIntoView()), !0)
     }
@@ -15006,15 +15009,15 @@
 function ms(t, e, n = !1) {
     for (let r = t; r; r = e == "start" ? r.firstChild : r.lastChild) {
         if (r.isTextblock) return !0;
         if (n && r.childCount != 1) return !1
     }
     return !1
 }
-const k_ = (t, e, n) => {
+const S_ = (t, e, n) => {
     let {
         $head: r,
         empty: s
     } = t.selection, i = r;
     if (!s) return !1;
     if (r.parent.isTextblock) {
         if (n ? !n.endOfTextblock("backward", t) : r.parentOffset > 0) return !1;
@@ -15029,22 +15032,22 @@
         for (let e = t.depth - 1; e >= 0; e--) {
             if (t.index(e) > 0) return t.doc.resolve(t.before(e + 1));
             if (t.node(e).type.spec.isolating) break
         }
     return null
 }
 
-function w_(t, e) {
+function __(t, e) {
     let {
         $cursor: n
     } = t.selection;
     return !n || (e ? !e.endOfTextblock("forward", t) : n.parentOffset < n.parent.content.size) ? null : n
 }
-const S_ = (t, e, n) => {
-        let r = w_(t, n);
+const C_ = (t, e, n) => {
+        let r = __(t, n);
         if (!r) return !1;
         let s = Tm(r);
         if (!s) return !1;
         let i = s.nodeAfter;
         if (Mm(t, s, e)) return !0;
         if (r.parent.content.size == 0 && (ms(i, "start") || se.isSelectable(i))) {
             let o = Mc(t.doc, r.before(), r.after(), q.empty);
@@ -15054,15 +15057,15 @@
                     l.setSelection(ms(i, "start") ? ve.findFrom(l.doc.resolve(l.mapping.map(s.pos)), 1) : se.create(l.doc, l.mapping.map(s.pos))), e(l.scrollIntoView())
                 }
                 return !0
             }
         }
         return i.isAtom && s.depth == r.depth - 1 ? (e && e(t.tr.delete(s.pos, s.pos + i.nodeSize).scrollIntoView()), !0) : !1
     },
-    __ = (t, e, n) => {
+    E_ = (t, e, n) => {
         let {
             $head: r,
             empty: s
         } = t.selection, i = r;
         if (!s) return !1;
         if (r.parent.isTextblock) {
             if (n ? !n.endOfTextblock("forward", t) : r.parentOffset < r.parent.content.size) return !1;
@@ -15077,45 +15080,45 @@
         for (let e = t.depth - 1; e >= 0; e--) {
             let n = t.node(e);
             if (t.index(e) + 1 < n.childCount) return t.doc.resolve(t.after(e + 1));
             if (n.type.spec.isolating) break
         }
     return null
 }
-const C_ = (t, e) => {
+const T_ = (t, e) => {
         let n = t.selection,
             r = n instanceof se,
             s;
         if (r) {
             if (n.node.isTextblock || !lr(t.doc, n.from)) return !1;
             s = n.from
         } else if (s = Bp(t.doc, n.from, -1), s == null) return !1;
         if (e) {
             let i = t.tr.join(s);
             r && i.setSelection(se.create(i.doc, s - t.doc.resolve(s).nodeBefore.nodeSize)), e(i.scrollIntoView())
         }
         return !0
     },
-    E_ = (t, e) => {
+    O_ = (t, e) => {
         let n = t.selection,
             r;
         if (n instanceof se) {
             if (n.node.isTextblock || !lr(t.doc, n.to)) return !1;
             r = n.to
         } else if (r = Bp(t.doc, n.to, 1), r == null) return !1;
         return e && e(t.tr.join(r).scrollIntoView()), !0
     },
-    T_ = (t, e) => {
+    M_ = (t, e) => {
         let {
             $from: n,
             $to: r
         } = t.selection, s = n.blockRange(r), i = s && Ms(s);
         return i == null ? !1 : (e && e(t.tr.lift(s, i).scrollIntoView()), !0)
     },
-    O_ = (t, e) => {
+    A_ = (t, e) => {
         let {
             $head: n,
             $anchor: r
         } = t.selection;
         return !n.parent.type.spec.code || !n.sameParent(r) ? !1 : (e && e(t.tr.insertText(`
 `).scrollIntoView()), !0)
     };
@@ -15125,15 +15128,15 @@
         let {
             type: n
         } = t.edge(e);
         if (n.isTextblock && !n.hasRequiredAttrs()) return n
     }
     return null
 }
-const M_ = (t, e) => {
+const N_ = (t, e) => {
         let {
             $head: n,
             $anchor: r
         } = t.selection;
         if (!n.parent.type.spec.code || !n.sameParent(r)) return !1;
         let s = n.node(-1),
             i = n.indexAfter(-1),
@@ -15142,15 +15145,15 @@
         if (e) {
             let l = n.after(),
                 a = t.tr.replaceWith(l, l, o.createAndFill());
             a.setSelection(ve.near(a.doc.resolve(l), 1)), e(a.scrollIntoView())
         }
         return !0
     },
-    A_ = (t, e) => {
+    R_ = (t, e) => {
         let n = t.selection,
             {
                 $from: r,
                 $to: s
             } = n;
         if (n instanceof nn || r.parent.inlineContent || s.parent.inlineContent) return !1;
         let i = Om(s.parent.contentMatchAt(s.indexAfter()));
@@ -15158,48 +15161,48 @@
         if (e) {
             let o = (!r.parentOffset && s.index() < s.parent.childCount ? r : s).pos,
                 l = t.tr.insert(o, i.createAndFill());
             l.setSelection(xe.create(l.doc, o + 1)), e(l.scrollIntoView())
         }
         return !0
     },
-    N_ = (t, e) => {
+    D_ = (t, e) => {
         let {
             $cursor: n
         } = t.selection;
         if (!n || n.parent.content.size) return !1;
         if (n.depth > 1 && n.after() != n.end(-1)) {
             let i = n.before();
             if (ts(t.doc, i)) return e && e(t.tr.split(i).scrollIntoView()), !0
         }
         let r = n.blockRange(),
             s = r && Ms(r);
         return s == null ? !1 : (e && e(t.tr.lift(r, s).scrollIntoView()), !0)
     },
-    R_ = (t, e) => {
+    I_ = (t, e) => {
         let {
             $from: n,
             to: r
         } = t.selection, s, i = n.sharedDepth(r);
         return i == 0 ? !1 : (s = n.before(i), e && e(t.tr.setSelection(se.create(t.doc, s))), !0)
     };
 
-function D_(t, e, n) {
+function P_(t, e, n) {
     let r = e.nodeBefore,
         s = e.nodeAfter,
         i = e.index();
     return !r || !s || !r.type.compatibleContent(s.type) ? !1 : !r.content.size && e.parent.canReplace(i - 1, i) ? (n && n(t.tr.delete(e.pos - r.nodeSize, e.pos).scrollIntoView()), !0) : !e.parent.canReplace(i, i + 1) || !(s.isTextblock || lr(t.doc, e.pos)) ? !1 : (n && n(t.tr.clearIncompatible(e.pos, r.type, r.contentMatchAt(r.childCount)).join(e.pos).scrollIntoView()), !0)
 }
 
 function Mm(t, e, n) {
     let r = e.nodeBefore,
         s = e.nodeAfter,
         i, o;
     if (r.type.spec.isolating || s.type.spec.isolating) return !1;
-    if (D_(t, e, n)) return !0;
+    if (P_(t, e, n)) return !0;
     let l = e.parent.canReplace(e.index(), e.index() + 1);
     if (l && (i = (o = r.contentMatchAt(r.childCount)).findWrapping(s.type)) && o.matchType(i[0] || s.type).validEnd) {
         if (n) {
             let d = e.pos + s.nodeSize,
                 f = $.empty;
             for (let g = i.length - 1; g >= 0; g--) f = $.from(i[g].create(null, f));
             f = $.from(r.copy(f));
@@ -15241,18 +15244,18 @@
         for (; s.node(i).isInline;) {
             if (!i) return !1;
             i--
         }
         return s.node(i).isTextblock ? (n && n(e.tr.setSelection(xe.create(e.doc, t < 0 ? s.start(i) : s.end(i)))), !0) : !1
     }
 }
-const I_ = Am(-1),
-    P_ = Am(1);
+const $_ = Am(-1),
+    L_ = Am(1);
 
-function $_(t, e = null) {
+function F_(t, e = null) {
     return function(n, r) {
         let {
             $from: s,
             $to: i
         } = n.selection, o = s.blockRange(i), l = o && Oc(o, t, e);
         return l ? (r && r(n.tr.wrap(o, l).scrollIntoView()), !0) : !1
     }
@@ -15298,67 +15301,67 @@
             r(i.scrollIntoView())
         }
         return !0
     }
 }
 typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : typeof os < "u" && os.platform && os.platform() == "darwin";
 
-function L_(t, e = null) {
+function B_(t, e = null) {
     return function(n, r) {
         let {
             $from: s,
             $to: i
         } = n.selection, o = s.blockRange(i), l = !1, a = o;
         if (!o) return !1;
         if (o.depth >= 2 && s.node(o.depth - 1).type.compatibleContent(t) && o.startIndex == 0) {
             if (s.index(o.depth - 1) == 0) return !1;
             let u = n.doc.resolve(o.start - 2);
-            a = new uo(u, u, o.depth), o.endIndex < o.parent.childCount && (o = new uo(s, n.doc.resolve(i.end(o.depth)), o.depth)), l = !0
+            a = new ho(u, u, o.depth), o.endIndex < o.parent.childCount && (o = new ho(s, n.doc.resolve(i.end(o.depth)), o.depth)), l = !0
         }
         let c = Oc(a, t, e, o);
-        return c ? (r && r(F_(n.tr, o, c, l, t).scrollIntoView()), !0) : !1
+        return c ? (r && r(H_(n.tr, o, c, l, t).scrollIntoView()), !0) : !1
     }
 }
 
-function F_(t, e, n, r, s) {
+function H_(t, e, n, r, s) {
     let i = $.empty;
     for (let u = n.length - 1; u >= 0; u--) i = $.from(n[u].type.create(n[u].attrs, i));
     t.step(new et(e.start - (r ? 2 : 0), e.end, e.start, e.end, new q(i, 0, 0), n.length, !0));
     let o = 0;
     for (let u = 0; u < n.length; u++) n[u].type == s && (o = u + 1);
     let l = n.length - o,
         a = e.start + n.length - (r ? 2 : 0),
         c = e.parent;
     for (let u = e.startIndex, d = e.endIndex, f = !0; u < d; u++, f = !1) !f && ts(t.doc, a, l) && (t.split(a, l), a += 2 * l), a += c.child(u).nodeSize;
     return t
 }
 
-function B_(t) {
+function z_(t) {
     return function(e, n) {
         let {
             $from: r,
             $to: s
         } = e.selection, i = r.blockRange(s, o => o.childCount > 0 && o.firstChild.type == t);
-        return i ? n ? r.node(i.depth - 1).type == t ? H_(e, n, t, i) : z_(e, n, i) : !0 : !1
+        return i ? n ? r.node(i.depth - 1).type == t ? V_(e, n, t, i) : j_(e, n, i) : !0 : !1
     }
 }
 
-function H_(t, e, n, r) {
+function V_(t, e, n, r) {
     let s = t.tr,
         i = r.end,
         o = r.$to.end(r.depth);
-    i < o && (s.step(new et(i - 1, o, i, o, new q($.from(n.create(null, r.parent.copy())), 1, 0), 1, !0)), r = new uo(s.doc.resolve(r.$from.pos), s.doc.resolve(o), r.depth));
+    i < o && (s.step(new et(i - 1, o, i, o, new q($.from(n.create(null, r.parent.copy())), 1, 0), 1, !0)), r = new ho(s.doc.resolve(r.$from.pos), s.doc.resolve(o), r.depth));
     const l = Ms(r);
     if (l == null) return !1;
     s.lift(r, l);
     let a = s.mapping.map(i, -1) - 1;
     return lr(s.doc, a) && s.join(a), e(s.scrollIntoView()), !0
 }
 
-function z_(t, e, n) {
+function j_(t, e, n) {
     let r = t.tr,
         s = n.parent;
     for (let h = n.end, p = n.endIndex - 1, g = n.startIndex; p > g; p--) h -= s.child(p).nodeSize, r.delete(h - 1, h + 1);
     let i = r.doc.resolve(n.start),
         o = i.nodeAfter;
     if (r.mapping.map(n.end) != n.start + i.nodeAfter.nodeSize) return !1;
     let l = n.startIndex == 0,
@@ -15367,15 +15370,15 @@
         u = i.index(-1);
     if (!c.canReplace(u + (l ? 0 : 1), u + 1, o.content.append(a ? $.empty : $.from(s)))) return !1;
     let d = i.pos,
         f = d + o.nodeSize;
     return r.step(new et(d - (l ? 1 : 0), f + (a ? 1 : 0), d + 1, f - 1, new q((l ? $.empty : $.from(s.copy($.empty))).append(a ? $.empty : $.from(s.copy($.empty))), l ? 0 : 1, a ? 0 : 1), l ? 0 : 1)), e(r.scrollIntoView()), !0
 }
 
-function V_(t) {
+function U_(t) {
     return function(e, n) {
         let {
             $from: r,
             $to: s
         } = e.selection, i = r.blockRange(s, c => c.childCount > 0 && c.firstChild.type == t);
         if (!i) return !1;
         let o = i.startIndex;
@@ -15514,15 +15517,15 @@
             get commands() {
                 return Object.fromEntries(Object.entries(r).map(([a, c]) => [a, (...u) => c(...u)(l)]))
             }
         };
         return l
     }
 }
-class j_ {
+class W_ {
     constructor() {
         this.callbacks = {}
     }
     on(e, n) {
         return this.callbacks[e] || (this.callbacks[e] = []), this.callbacks[e].push(n), this
     }
     emit(e, ...n) {
@@ -15649,48 +15652,48 @@
     return typeof t == "function"
 }
 
 function be(t, e = void 0, ...n) {
     return Rm(t) ? e ? t.bind(e)(...n) : t(...n) : t
 }
 
-function U_(t = {}) {
+function q_(t = {}) {
     return Object.keys(t).length === 0 && t.constructor === Object
 }
 
-function W_(t) {
+function K_(t) {
     return typeof t != "string" ? t : t.match(/^[+-]?(?:\d*\.)?\d+$/) ? Number(t) : t === "true" ? !0 : t === "false" ? !1 : t
 }
 
 function lf(t, e) {
     return t.style ? t : {
         ...t,
         getAttrs: n => {
             const r = t.getAttrs ? t.getAttrs(n) : t.attrs;
             if (r === !1) return !1;
             const s = e.reduce((i, o) => {
-                const l = o.attribute.parseHTML ? o.attribute.parseHTML(n) : W_(n.getAttribute(o.name));
+                const l = o.attribute.parseHTML ? o.attribute.parseHTML(n) : K_(n.getAttribute(o.name));
                 return l == null ? i : {
                     ...i,
                     [o.name]: l
                 }
             }, {});
             return {
                 ...r,
                 ...s
             }
         }
     }
 }
 
 function af(t) {
-    return Object.fromEntries(Object.entries(t).filter(([e, n]) => e === "attrs" && U_(n) ? !1 : n != null))
+    return Object.fromEntries(Object.entries(t).filter(([e, n]) => e === "attrs" && q_(n) ? !1 : n != null))
 }
 
-function q_(t, e) {
+function J_(t, e) {
     var n;
     const r = Nm(t),
         {
             nodeExtensions: s,
             markExtensions: i
         } = sl(t),
         o = (n = s.find(c => X(c, "topNode"))) === null || n === void 0 ? void 0 : n.name,
@@ -15771,29 +15774,29 @@
             p && (h.parseDOM = p.map(v => lf(v, u)));
             const g = X(c, "renderHTML", d);
             return g && (h.toDOM = v => g({
                 mark: v,
                 HTMLAttributes: Va(v, u)
             })), [c.name, h]
         }));
-    return new tw({
+    return new rw({
         topNode: o,
         nodes: l,
         marks: a
     })
 }
 
 function Jl(t, e) {
     return e.nodes[t] || e.marks[t] || null
 }
 
 function cf(t, e) {
     return Array.isArray(e) ? e.some(n => (typeof n == "string" ? n : n.name) === t.name) : e
 }
-const K_ = (t, e = 500) => {
+const G_ = (t, e = 500) => {
     let n = "";
     const r = t.parentOffset;
     return t.parent.nodesBetween(Math.max(0, r - e), r, (s, i, o, l) => {
         var a, c;
         const u = ((c = (a = s.type.spec).toText) === null || c === void 0 ? void 0 : c.call(a, {
             node: s,
             pos: i,
@@ -15808,15 +15811,15 @@
     return Object.prototype.toString.call(t) === "[object RegExp]"
 }
 class il {
     constructor(e) {
         this.find = e.find, this.handler = e.handler
     }
 }
-const J_ = (t, e) => {
+const Y_ = (t, e) => {
     if (Hc(e)) return e.exec(t);
     const n = e(t);
     if (!n) return null;
     const r = [n.text];
     return r.index = n.index, r.input = t, r.data = n.data, n.replaceWith && (n.text.includes(n.replaceWith) || console.warn('[tiptap warn]: "inputRuleMatch.replaceWith" must be part of "inputRuleMatch.text".'), r.push(n.replaceWith)), r
 };
 
@@ -15832,18 +15835,18 @@
     } = t, {
         view: a
     } = n;
     if (a.composing) return !1;
     const c = a.state.doc.resolve(r);
     if (c.parent.type.spec.code || !((e = c.nodeBefore || c.nodeAfter) === null || e === void 0) && e.marks.find(f => f.type.spec.code)) return !1;
     let u = !1;
-    const d = K_(c) + i;
+    const d = G_(c) + i;
     return o.forEach(f => {
         if (u) return;
-        const h = J_(d, f.find);
+        const h = Y_(d, f.find);
         if (!h) return;
         const p = a.state.tr,
             g = nl({
                 state: a.state,
                 transaction: p
             }),
             v = {
@@ -15870,15 +15873,15 @@
             from: r,
             to: s,
             text: i
         }), a.dispatch(p), u = !0)
     }), u
 }
 
-function G_(t) {
+function X_(t) {
     const {
         editor: e,
         rules: n
     } = t, r = new Mt({
         state: {
             init() {
                 return null
@@ -15931,32 +15934,32 @@
             }
         },
         isInputRules: !0
     });
     return r
 }
 
-function Y_(t) {
+function Q_(t) {
     return typeof t == "number"
 }
-class X_ {
+class Z_ {
     constructor(e) {
         this.find = e.find, this.handler = e.handler
     }
 }
-const Q_ = (t, e) => {
+const eC = (t, e) => {
     if (Hc(e)) return [...t.matchAll(e)];
     const n = e(t);
     return n ? n.map(r => {
         const s = [r.text];
         return s.index = r.index, s.input = t, s.data = r.data, r.replaceWith && (r.text.includes(r.replaceWith) || console.warn('[tiptap warn]: "pasteRuleMatch.replaceWith" must be part of "pasteRuleMatch.text".'), s.push(r.replaceWith)), s
     }) : []
 };
 
-function Z_(t) {
+function tC(t) {
     const {
         editor: e,
         state: n,
         from: r,
         to: s,
         rule: i
     } = t, {
@@ -15968,15 +15971,15 @@
         state: n
     }), c = [];
     return n.doc.nodesBetween(r, s, (d, f) => {
         if (!d.isTextblock || d.type.spec.code) return;
         const h = Math.max(r, f),
             p = Math.min(s, f + d.content.size),
             g = d.textBetween(h - f, p - f, void 0, "￼");
-        Q_(g, i.find).forEach(x => {
+        eC(g, i.find).forEach(x => {
             if (x.index === void 0) return;
             const w = h + x.index + 1,
                 S = w + x[0].length,
                 y = {
                     from: n.tr.mapping.map(w),
                     to: n.tr.mapping.map(S)
                 },
@@ -15989,15 +15992,15 @@
                     can: a
                 });
             c.push(I)
         })
     }), c.every(d => d !== null)
 }
 
-function eC(t) {
+function nC(t) {
     const {
         editor: e,
         rules: n
     } = t;
     let r = null,
         s = !1,
         i = !1;
@@ -16026,38 +16029,38 @@
         appendTransaction: (a, c, u) => {
             const d = a[0],
                 f = d.getMeta("uiEvent") === "paste" && !s,
                 h = d.getMeta("uiEvent") === "drop" && !i;
             if (!f && !h) return;
             const p = c.doc.content.findDiffStart(u.doc.content),
                 g = c.doc.content.findDiffEnd(u.doc.content);
-            if (!Y_(p) || !g || p === g.b) return;
+            if (!Q_(p) || !g || p === g.b) return;
             const v = u.tr,
                 x = nl({
                     state: u,
                     transaction: v
                 });
-            if (!(!Z_({
+            if (!(!tC({
                     editor: e,
                     state: x,
                     from: Math.max(p - 1, 0),
                     to: g.b - 1,
                     rule: l
                 }) || !v.steps.length)) return v
         }
     }))
 }
 
-function tC(t) {
+function rC(t) {
     const e = t.filter((n, r) => t.indexOf(n) !== r);
     return [...new Set(e)]
 }
 class Jr {
     constructor(e, n) {
-        this.splittableMarks = [], this.editor = n, this.extensions = Jr.resolve(e), this.schema = q_(this.extensions, n), this.extensions.forEach(r => {
+        this.splittableMarks = [], this.editor = n, this.extensions = Jr.resolve(e), this.schema = J_(this.extensions, n), this.extensions.forEach(r => {
             var s;
             this.editor.extensionStorage[r.name] = r.storage;
             const i = {
                 name: r.name,
                 options: r.options,
                 storage: r.storage,
                 editor: this.editor,
@@ -16080,15 +16083,15 @@
             f && this.editor.on("blur", f);
             const h = X(r, "onDestroy", i);
             h && this.editor.on("destroy", h)
         })
     }
     static resolve(e) {
         const n = Jr.sort(Jr.flatten(e)),
-            r = tC(n.map(s => s.name));
+            r = rC(n.map(s => s.name));
         return r.length && console.warn(`[tiptap warn]: Duplicate extension names found: [${r.map(s=>`'${s}'`).join(", ")}]. This can lead to issues.`), n
     }
     static flatten(e) {
         return e.map(n => {
             const r = {
                     name: n.name,
                     options: n.options,
@@ -16143,31 +16146,31 @@
                     editor: e
                 })]));
                 u = {
                     ...u,
                     ...g
                 }
             }
-            const d = y_(u);
+            const d = v_(u);
             a.push(d);
             const f = X(o, "addInputRules", l);
             cf(o, e.options.enableInputRules) && f && r.push(...f());
             const h = X(o, "addPasteRules", l);
             cf(o, e.options.enablePasteRules) && h && s.push(...h());
             const p = X(o, "addProseMirrorPlugins", l);
             if (p) {
                 const g = p();
                 a.push(...g)
             }
             return a
         }).flat();
-        return [G_({
+        return [X_({
             editor: e,
             rules: r
-        }), ...eC({
+        }), ...nC({
             editor: e,
             rules: s
         }), ...i]
     }
     get attributes() {
         return Nm(this.extensions)
     }
@@ -16200,20 +16203,20 @@
                 })
             };
             return [r.name, l]
         }))
     }
 }
 
-function nC(t) {
+function sC(t) {
     return Object.prototype.toString.call(t).slice(8, -1)
 }
 
 function Yl(t) {
-    return nC(t) !== "Object" ? !1 : t.constructor === Object && Object.getPrototypeOf(t) === Object.prototype
+    return sC(t) !== "Object" ? !1 : t.constructor === Object && Object.getPrototypeOf(t) === Object.prototype
 }
 
 function ol(t, e) {
     const n = {
         ...t
     };
     return Yl(t) && Yl(e) && Object.keys(e).forEach(r => {
@@ -16284,15 +16287,15 @@
         }))) : c.isText ? (l += (h = c == null ? void 0 : c.text) === null || h === void 0 ? void 0 : h.slice(Math.max(r, u) - u, s - u), a = !1) : c.isBlock && !a && (l += i, a = !0)
     }), l
 }
 
 function Im(t) {
     return Object.fromEntries(Object.entries(t.nodes).filter(([, e]) => e.spec.toText).map(([e, n]) => [e, n.spec.toText]))
 }
-const rC = kt.create({
+const iC = kt.create({
         name: "clipboardTextSerializer",
         addProseMirrorPlugins() {
             return [new Mt({
                 key: new Sn("clipboardTextSerializer"),
                 props: {
                     clipboardTextSerializer: () => {
                         const {
@@ -16313,25 +16316,25 @@
                             textSerializers: a
                         })
                     }
                 }
             })]
         }
     }),
-    sC = () => ({
+    oC = () => ({
         editor: t,
         view: e
     }) => (requestAnimationFrame(() => {
         var n;
         t.isDestroyed || (e.dom.blur(), (n = window == null ? void 0 : window.getSelection()) === null || n === void 0 || n.removeAllRanges())
     }), !0),
-    iC = (t = !1) => ({
+    lC = (t = !1) => ({
         commands: e
     }) => e.setContent("", t),
-    oC = () => ({
+    aC = () => ({
         state: t,
         tr: e,
         dispatch: n
     }) => {
         const {
             selection: r
         } = e, {
@@ -16354,20 +16357,20 @@
                         defaultType: g
                     } = d.parent.contentMatchAt(d.index());
                     e.setNodeMarkup(h.start, g)
                 }(p || p === 0) && e.lift(h, p)
             })
         }), !0
     },
-    lC = t => e => t(e),
-    aC = () => ({
+    cC = t => e => t(e),
+    uC = () => ({
         state: t,
         dispatch: e
-    }) => A_(t, e),
-    cC = () => ({
+    }) => R_(t, e),
+    dC = () => ({
         tr: t,
         dispatch: e
     }) => {
         const {
             selection: n
         } = t, r = n.$anchor.node();
         if (r.content.size > 0) return !1;
@@ -16378,15 +16381,15 @@
                     const l = s.before(i),
                         a = s.after(i);
                     t.delete(l, a).scrollIntoView()
                 }
                 return !0
             } return !1
     },
-    uC = t => ({
+    fC = t => ({
         tr: e,
         state: n,
         dispatch: r
     }) => {
         const s = tt(t, n.schema),
             i = e.selection.$anchor;
         for (let o = i.depth; o > 0; o -= 1)
@@ -16395,77 +16398,77 @@
                     const a = i.before(o),
                         c = i.after(o);
                     e.delete(a, c).scrollIntoView()
                 }
                 return !0
             } return !1
     },
-    dC = t => ({
+    hC = t => ({
         tr: e,
         dispatch: n
     }) => {
         const {
             from: r,
             to: s
         } = t;
         return n && e.delete(r, s), !0
     },
-    fC = () => ({
+    pC = () => ({
         state: t,
         dispatch: e
-    }) => b_(t, e),
-    hC = () => ({
+    }) => x_(t, e),
+    mC = () => ({
         commands: t
     }) => t.keyboardShortcut("Enter"),
-    pC = () => ({
+    gC = () => ({
         state: t,
         dispatch: e
-    }) => M_(t, e);
+    }) => N_(t, e);
 
-function vo(t, e, n = {
+function ko(t, e, n = {
     strict: !0
 }) {
     const r = Object.keys(e);
     return r.length ? r.every(s => n.strict ? e[s] === t[s] : Hc(e[s]) ? e[s].test(t[s]) : e[s] === t[s]) : !0
 }
 
 function ja(t, e, n = {}) {
-    return t.find(r => r.type === e && vo(r.attrs, n))
+    return t.find(r => r.type === e && ko(r.attrs, n))
 }
 
-function mC(t, e, n = {}) {
+function yC(t, e, n = {}) {
     return !!ja(t, e, n)
 }
 
 function zc(t, e, n = {}) {
     if (!t || !e) return;
     let r = t.parent.childAfter(t.parentOffset);
     if (t.parentOffset === r.offset && r.offset !== 0 && (r = t.parent.childBefore(t.parentOffset)), !r.node) return;
     const s = ja([...r.node.marks], e, n);
     if (!s) return;
     let i = r.index,
         o = t.start() + r.offset,
         l = i + 1,
         a = o + r.node.nodeSize;
     for (ja([...r.node.marks], e, n); i > 0 && s.isInSet(t.parent.child(i - 1).marks);) i -= 1, o -= t.parent.child(i).nodeSize;
-    for (; l < t.parent.childCount && mC([...t.parent.child(l).marks], e, n);) a += t.parent.child(l).nodeSize, l += 1;
+    for (; l < t.parent.childCount && yC([...t.parent.child(l).marks], e, n);) a += t.parent.child(l).nodeSize, l += 1;
     return {
         from: o,
         to: a
     }
 }
 
 function cr(t, e) {
     if (typeof t == "string") {
         if (!e.marks[t]) throw Error(`There is no mark type named '${t}'. Maybe you forgot to add the extension?`);
         return e.marks[t]
     }
     return t
 }
-const gC = (t, e = {}) => ({
+const bC = (t, e = {}) => ({
         tr: n,
         state: r,
         dispatch: s
     }) => {
         const i = cr(t, r.schema),
             {
                 doc: o,
@@ -16481,15 +16484,15 @@
             if (d && d.from <= c && d.to >= u) {
                 const f = xe.create(o, d.from, d.to);
                 n.setSelection(f)
             }
         }
         return !0
     },
-    yC = t => e => {
+    vC = t => e => {
         const n = typeof t == "function" ? t(e) : t;
         for (let r = 0; r < n.length; r += 1)
             if (n[r](e)) return !0;
         return !1
     };
 
 function Vc(t) {
@@ -16510,15 +16513,15 @@
         i = r.to;
     return e === "all" ? xe.create(t, Tn(0, s, i), Tn(t.content.size, s, i)) : xe.create(t, Tn(e, s, i), Tn(e, s, i))
 }
 
 function jc() {
     return ["iPad Simulator", "iPhone Simulator", "iPod Simulator", "iPad", "iPhone", "iPod"].includes(navigator.platform) || navigator.userAgent.includes("Mac") && "ontouchend" in document
 }
-const bC = (t = null, e = {}) => ({
+const xC = (t = null, e = {}) => ({
         editor: n,
         view: r,
         tr: s,
         dispatch: i
     }) => {
         e = {
             scrollIntoView: !0,
@@ -16531,119 +16534,119 @@
         };
         if (r.hasFocus() && t === null || t === !1) return !0;
         if (i && t === null && !Vc(n.state.selection)) return o(), !0;
         const l = Pm(s.doc, t) || n.state.selection,
             a = n.state.selection.eq(l);
         return i && (a || s.setSelection(l), a && s.storedMarks && s.setStoredMarks(s.storedMarks), o()), !0
     },
-    vC = (t, e) => n => t.every((r, s) => e(r, {
+    kC = (t, e) => n => t.every((r, s) => e(r, {
         ...n,
         index: s
     })),
-    xC = (t, e) => ({
+    wC = (t, e) => ({
         tr: n,
         commands: r
     }) => r.insertContentAt({
         from: n.selection.from,
         to: n.selection.to
     }, t, e);
 
 function uf(t) {
     const e = `<body>${t}</body>`;
     return new window.DOMParser().parseFromString(e, "text/html").body
 }
 
-function xo(t, e, n) {
+function wo(t, e, n) {
     if (n = {
             slice: !0,
             parseOptions: {},
             ...n
         }, typeof t == "object" && t !== null) try {
         return Array.isArray(t) && t.length > 0 ? $.fromArray(t.map(r => e.nodeFromJSON(r))) : e.nodeFromJSON(t)
     } catch (r) {
-        return console.warn("[tiptap warn]: Invalid content.", "Passed value:", t, "Error:", r), xo("", e, n)
+        return console.warn("[tiptap warn]: Invalid content.", "Passed value:", t, "Error:", r), wo("", e, n)
     }
     if (typeof t == "string") {
         const r = us.fromSchema(e);
         return n.slice ? r.parseSlice(uf(t), n.parseOptions).content : r.parse(uf(t), n.parseOptions)
     }
-    return xo("", e, n)
+    return wo("", e, n)
 }
 
-function kC(t, e, n) {
+function SC(t, e, n) {
     const r = t.steps.length - 1;
     if (r < e) return;
     const s = t.steps[r];
     if (!(s instanceof ct || s instanceof et)) return;
     const i = t.mapping.maps[r];
     let o = 0;
     i.forEach((l, a, c, u) => {
         o === 0 && (o = u)
     }), t.setSelection(ve.near(t.doc.resolve(o), n))
 }
-const wC = t => t.toString().startsWith("<"),
-    SC = (t, e, n) => ({
+const _C = t => t.toString().startsWith("<"),
+    CC = (t, e, n) => ({
         tr: r,
         dispatch: s,
         editor: i
     }) => {
         if (s) {
             n = {
                 parseOptions: {},
                 updateSelection: !0,
                 ...n
             };
-            const o = xo(e, i.schema, {
+            const o = wo(e, i.schema, {
                 parseOptions: {
                     preserveWhitespace: "full",
                     ...n.parseOptions
                 }
             });
             if (o.toString() === "<>") return !0;
             let {
                 from: l,
                 to: a
             } = typeof t == "number" ? {
                 from: t,
                 to: t
             } : t, c = !0, u = !0;
-            if ((wC(o) ? o : [o]).forEach(f => {
+            if ((_C(o) ? o : [o]).forEach(f => {
                     f.check(), c = c ? f.isText && f.marks.length === 0 : !1, u = u ? f.isBlock : !1
                 }), l === a && u) {
                 const {
                     parent: f
                 } = r.doc.resolve(l);
                 f.isTextblock && !f.type.spec.code && !f.childCount && (l -= 1, a += 1)
             }
-            c ? Array.isArray(e) ? r.insertText(e.map(f => f.text || "").join(""), l, a) : typeof e == "object" && e && e.text ? r.insertText(e.text, l, a) : r.insertText(e, l, a) : r.replaceWith(l, a, o), n.updateSelection && kC(r, r.steps.length - 1, -1)
+            c ? Array.isArray(e) ? r.insertText(e.map(f => f.text || "").join(""), l, a) : typeof e == "object" && e && e.text ? r.insertText(e.text, l, a) : r.insertText(e, l, a) : r.replaceWith(l, a, o), n.updateSelection && SC(r, r.steps.length - 1, -1)
         }
         return !0
     },
-    _C = () => ({
+    EC = () => ({
         state: t,
         dispatch: e
-    }) => C_(t, e),
-    CC = () => ({
+    }) => T_(t, e),
+    TC = () => ({
         state: t,
         dispatch: e
-    }) => E_(t, e),
-    EC = () => ({
+    }) => O_(t, e),
+    OC = () => ({
         state: t,
         dispatch: e
-    }) => x_(t, e),
-    TC = () => ({
+    }) => w_(t, e),
+    MC = () => ({
         state: t,
         dispatch: e
-    }) => S_(t, e);
+    }) => C_(t, e);
 
 function $m() {
     return typeof navigator < "u" ? /Mac/.test(navigator.platform) : !1
 }
 
-function OC(t) {
+function AC(t) {
     const e = t.split(/-(?!$)/);
     let n = e[e.length - 1];
     n === "Space" && (n = " ");
     let r, s, i, o;
     for (let l = 0; l < e.length - 1; l += 1) {
         const a = e[l];
         if (/^(cmd|meta|m)$/i.test(a)) o = !0;
@@ -16651,21 +16654,21 @@
         else if (/^(c|ctrl|control)$/i.test(a)) s = !0;
         else if (/^s(hift)?$/i.test(a)) i = !0;
         else if (/^mod$/i.test(a)) jc() || $m() ? o = !0 : s = !0;
         else throw new Error(`Unrecognized modifier name: ${a}`)
     }
     return r && (n = `Alt-${n}`), s && (n = `Ctrl-${n}`), o && (n = `Meta-${n}`), i && (n = `Shift-${n}`), n
 }
-const MC = t => ({
+const NC = t => ({
     editor: e,
     view: n,
     tr: r,
     dispatch: s
 }) => {
-    const i = OC(t).split(/-(?!$)/),
+    const i = AC(t).split(/-(?!$)/),
         o = i.find(c => !["Alt", "Ctrl", "Meta", "Shift"].includes(c)),
         l = new KeyboardEvent("keydown", {
             key: o === "Space" ? " " : o,
             altKey: i.includes("Alt"),
             ctrlKey: i.includes("Ctrl"),
             metaKey: i.includes("Meta"),
             shiftKey: i.includes("Shift"),
@@ -16694,51 +16697,51 @@
         l.push({
             node: d,
             from: h,
             to: p
         })
     });
     const a = s - r,
-        c = l.filter(d => o ? o.name === d.node.type.name : !0).filter(d => vo(d.node.attrs, n, {
+        c = l.filter(d => o ? o.name === d.node.type.name : !0).filter(d => ko(d.node.attrs, n, {
             strict: !1
         }));
     return i ? !!c.length : c.reduce((d, f) => d + f.to - f.from, 0) >= a
 }
-const AC = (t, e = {}) => ({
+const RC = (t, e = {}) => ({
         state: n,
         dispatch: r
     }) => {
         const s = tt(t, n.schema);
-        return gi(n, s, e) ? T_(n, r) : !1
+        return gi(n, s, e) ? M_(n, r) : !1
     },
-    NC = () => ({
+    DC = () => ({
         state: t,
         dispatch: e
-    }) => N_(t, e),
-    RC = t => ({
+    }) => D_(t, e),
+    IC = t => ({
         state: e,
         dispatch: n
     }) => {
         const r = tt(t, e.schema);
-        return B_(r)(e, n)
+        return z_(r)(e, n)
     },
-    DC = () => ({
+    PC = () => ({
         state: t,
         dispatch: e
-    }) => O_(t, e);
+    }) => A_(t, e);
 
 function ll(t, e) {
     return e.nodes[t] ? "node" : e.marks[t] ? "mark" : null
 }
 
 function df(t, e) {
     const n = typeof e == "string" ? [e] : e;
     return Object.keys(t).reduce((r, s) => (n.includes(s) || (r[s] = t[s]), r), {})
 }
-const IC = (t, e) => ({
+const $C = (t, e) => ({
         tr: n,
         state: r,
         dispatch: s
     }) => {
         let i = null,
             o = null;
         const l = ll(typeof t == "string" ? t : t.name, r.schema);
@@ -16746,96 +16749,96 @@
             r.doc.nodesBetween(a.$from.pos, a.$to.pos, (c, u) => {
                 i && i === c.type && n.setNodeMarkup(u, void 0, df(c.attrs, e)), o && c.marks.length && c.marks.forEach(d => {
                     o === d.type && n.addMark(u, u + c.nodeSize, o.create(df(d.attrs, e)))
                 })
             })
         }), !0) : !1
     },
-    PC = () => ({
+    LC = () => ({
         tr: t,
         dispatch: e
     }) => (e && t.scrollIntoView(), !0),
-    $C = () => ({
+    FC = () => ({
         tr: t,
         commands: e
     }) => e.setTextSelection({
         from: 0,
         to: t.doc.content.size
     }),
-    LC = () => ({
+    BC = () => ({
         state: t,
         dispatch: e
-    }) => k_(t, e),
-    FC = () => ({
+    }) => S_(t, e),
+    HC = () => ({
         state: t,
         dispatch: e
-    }) => __(t, e),
-    BC = () => ({
+    }) => E_(t, e),
+    zC = () => ({
         state: t,
         dispatch: e
-    }) => R_(t, e),
-    HC = () => ({
+    }) => I_(t, e),
+    VC = () => ({
         state: t,
         dispatch: e
-    }) => P_(t, e),
-    zC = () => ({
+    }) => L_(t, e),
+    jC = () => ({
         state: t,
         dispatch: e
-    }) => I_(t, e);
+    }) => $_(t, e);
 
 function Lm(t, e, n = {}) {
-    return xo(t, e, {
+    return wo(t, e, {
         slice: !1,
         parseOptions: n
     })
 }
-const VC = (t, e = !1, n = {}) => ({
+const UC = (t, e = !1, n = {}) => ({
     tr: r,
     editor: s,
     dispatch: i
 }) => {
     const {
         doc: o
     } = r, l = Lm(t, s.schema, n);
     return i && r.replaceWith(0, o.content.size, l).setMeta("preventUpdate", !e), !0
 };
 
-function jC(t) {
+function WC(t) {
     for (let e = 0; e < t.edgeCount; e += 1) {
         const {
             type: n
         } = t.edge(e);
         if (n.isTextblock && !n.hasRequiredAttrs()) return n
     }
     return null
 }
 
-function UC(t, e) {
+function qC(t, e) {
     for (let n = t.depth; n > 0; n -= 1) {
         const r = t.node(n);
         if (e(r)) return {
             pos: n > 0 ? t.before(n) : 0,
             start: t.start(n),
             depth: n,
             node: r
         }
     }
 }
 
 function Uc(t) {
-    return e => UC(e.$from, t)
+    return e => qC(e.$from, t)
 }
 
-function WC(t, e) {
+function KC(t, e) {
     const n = hn.fromSchema(e).serializeFragment(t),
         s = document.implementation.createHTMLDocument().createElement("div");
     return s.appendChild(n), s.innerHTML
 }
 
-function qC(t, e) {
+function JC(t, e) {
     const n = {
         from: 0,
         to: t.content.size
     };
     return Dm(t, n, e)
 }
 
@@ -16852,15 +16855,15 @@
     });
     const l = o.find(a => a.type.name === n.name);
     return l ? {
         ...l.attrs
     } : {}
 }
 
-function KC(t, e) {
+function GC(t, e) {
     const n = tt(e, t.schema),
         {
             from: r,
             to: s
         } = t.selection,
         i = [];
     t.doc.nodesBetween(r, s, l => {
@@ -16868,17 +16871,17 @@
     });
     const o = i.reverse().find(l => l.type.name === n.name);
     return o ? {
         ...o.attrs
     } : {}
 }
 
-function JC(t, e) {
+function YC(t, e) {
     const n = ll(typeof e == "string" ? e : e.name, t.schema);
-    return n === "node" ? KC(t, e) : n === "mark" ? al(t, e) : {}
+    return n === "node" ? GC(t, e) : n === "mark" ? al(t, e) : {}
 }
 
 function Fm(t, e, n) {
     const r = [];
     return t === e ? n.resolve(t).marks().forEach(s => {
         const i = n.resolve(t - 1),
             o = zc(i, s.type);
@@ -16891,27 +16894,27 @@
             from: i,
             to: i + s.nodeSize,
             mark: o
         })))
     }), r
 }
 
-function Gi(t, e, n) {
+function Xi(t, e, n) {
     return Object.fromEntries(Object.entries(n).filter(([r]) => {
         const s = t.find(i => i.type === e && i.name === r);
         return s ? s.attribute.keepOnSplit : !1
     }))
 }
 
 function Ua(t, e, n = {}) {
     const {
         empty: r,
         ranges: s
     } = t.selection, i = e ? cr(e, t.schema) : null;
-    if (r) return !!(t.storedMarks || t.selection.$from.marks()).filter(d => i ? i.name === d.type.name : !0).find(d => vo(d.attrs, n, {
+    if (r) return !!(t.storedMarks || t.selection.$from.marks()).filter(d => i ? i.name === d.type.name : !0).find(d => ko(d.attrs, n, {
         strict: !1
     }));
     let o = 0;
     const l = [];
     if (s.forEach(({
             $from: d,
             $to: f
@@ -16926,22 +16929,22 @@
                 o += S, l.push(...g.marks.map(y => ({
                     mark: y,
                     from: x,
                     to: w
                 })))
             })
         }), o === 0) return !1;
-    const a = l.filter(d => i ? i.name === d.mark.type.name : !0).filter(d => vo(d.mark.attrs, n, {
+    const a = l.filter(d => i ? i.name === d.mark.type.name : !0).filter(d => ko(d.mark.attrs, n, {
             strict: !1
         })).reduce((d, f) => d + f.to - f.from, 0),
         c = l.filter(d => i ? d.mark.type !== i && d.mark.type.excludes(i) : !0).reduce((d, f) => d + f.to - f.from, 0);
     return (a > 0 ? a + c : a) >= o
 }
 
-function GC(t, e, n = {}) {
+function XC(t, e, n = {}) {
     if (!e) return gi(t, null, n) || Ua(t, null, n);
     const r = ll(e, t.schema);
     return r === "node" ? gi(t, e, n) : r === "mark" ? Ua(t, e, n) : !1
 }
 
 function ff(t, e) {
     const {
@@ -16953,22 +16956,22 @@
             options: r.options,
             storage: r.storage
         },
         i = be(X(r, "group", s));
     return typeof i != "string" ? !1 : i.split(" ").includes("list")
 }
 
-function YC(t) {
+function QC(t) {
     var e;
     const n = (e = t.type.createAndFill()) === null || e === void 0 ? void 0 : e.toJSON(),
         r = t.toJSON();
     return JSON.stringify(n) === JSON.stringify(r)
 }
 
-function XC(t) {
+function ZC(t) {
     return t instanceof se
 }
 
 function Bm(t, e, n) {
     const s = t.state.doc.content.size,
         i = Tn(e, 0, s),
         o = Tn(n, 0, s),
@@ -16992,15 +16995,15 @@
         };
     return {
         ...x,
         toJSON: () => x
     }
 }
 
-function QC(t, e, n) {
+function eE(t, e, n) {
     var r;
     const {
         selection: s
     } = e;
     let i = null;
     if (Vc(s) && (i = s.$cursor), i) {
         const l = (r = t.storedMarks) !== null && r !== void 0 ? r : i.marks();
@@ -17021,15 +17024,15 @@
                     p = !!n.isInSet(u.marks) || !u.marks.some(g => g.type.excludes(n));
                 c = h && p
             }
             return !c
         }), c
     })
 }
-const ZC = (t, e = {}) => ({
+const tE = (t, e = {}) => ({
         tr: n,
         state: r,
         dispatch: s
     }) => {
         const {
             selection: i
         } = n, {
@@ -17053,44 +17056,44 @@
                         a === x.type && n.addMark(p, g, a.create({
                             ...x.attrs,
                             ...e
                         }))
                     }) : n.addMark(p, g, a.create(e))
                 })
             });
-        return QC(r, n, a)
+        return eE(r, n, a)
     },
-    eE = (t, e) => ({
+    nE = (t, e) => ({
         tr: n
     }) => (n.setMeta(t, e), !0),
-    tE = (t, e = {}) => ({
+    rE = (t, e = {}) => ({
         state: n,
         dispatch: r,
         chain: s
     }) => {
         const i = tt(t, n.schema);
         return i.isTextblock ? s().command(({
             commands: o
         }) => of(i, e)(n) ? !0 : o.clearNodes()).command(({
             state: o
         }) => of(i, e)(o, r)).run() : (console.warn('[tiptap warn]: Currently "setNode()" only supports text block nodes.'), !1)
     },
-    nE = t => ({
+    sE = t => ({
         tr: e,
         dispatch: n
     }) => {
         if (n) {
             const {
                 doc: r
             } = e, s = Tn(t, 0, r.content.size), i = se.create(r, s);
             e.setSelection(i)
         }
         return !0
     },
-    rE = t => ({
+    iE = t => ({
         tr: e,
         dispatch: n
     }) => {
         if (n) {
             const {
                 doc: r
             } = e, {
@@ -17100,50 +17103,50 @@
                 from: t,
                 to: t
             } : t, o = xe.atStart(r).from, l = xe.atEnd(r).to, a = Tn(s, o, l), c = Tn(i, o, l), u = xe.create(r, a, c);
             e.setSelection(u)
         }
         return !0
     },
-    sE = t => ({
+    oE = t => ({
         state: e,
         dispatch: n
     }) => {
         const r = tt(t, e.schema);
-        return V_(r)(e, n)
+        return U_(r)(e, n)
     };
 
 function hf(t, e) {
     const n = t.storedMarks || t.selection.$to.parentOffset && t.selection.$from.marks();
     if (n) {
         const r = n.filter(s => e == null ? void 0 : e.includes(s.type.name));
         t.tr.ensureMarks(r)
     }
 }
-const iE = ({
+const lE = ({
         keepMarks: t = !0
     } = {}) => ({
         tr: e,
         state: n,
         dispatch: r,
         editor: s
     }) => {
         const {
             selection: i,
             doc: o
         } = e, {
             $from: l,
             $to: a
-        } = i, c = s.extensionManager.attributes, u = Gi(c, l.node().type.name, l.node().attrs);
+        } = i, c = s.extensionManager.attributes, u = Xi(c, l.node().type.name, l.node().attrs);
         if (i instanceof se && i.node.isBlock) return !l.parentOffset || !ts(o, l.pos) ? !1 : (r && (t && hf(n, s.extensionManager.splittableMarks), e.split(l.pos).scrollIntoView()), !0);
         if (!l.parent.isBlock) return !1;
         if (r) {
             const d = a.parentOffset === a.parent.content.size;
             i instanceof xe && e.deleteSelection();
-            const f = l.depth === 0 ? void 0 : jC(l.node(-1).contentMatchAt(l.indexAfter(-1)));
+            const f = l.depth === 0 ? void 0 : WC(l.node(-1).contentMatchAt(l.indexAfter(-1)));
             let h = d && f ? [{
                     type: f,
                     attrs: u
                 }] : void 0,
                 p = ts(e.doc, e.mapping.map(l.pos), 1, h);
             if (!h && !p && ts(e.doc, e.mapping.map(l.pos), 1, f ? [{
                     type: f
@@ -17155,15 +17158,15 @@
                     v = e.doc.resolve(g);
                 l.node(-1).canReplaceWith(v.index(), v.index() + 1, f) && e.setNodeMarkup(e.mapping.map(l.before()), f)
             }
             t && hf(n, s.extensionManager.splittableMarks), e.scrollIntoView()
         }
         return !0
     },
-    oE = t => ({
+    aE = t => ({
         tr: e,
         state: n,
         dispatch: r,
         editor: s
     }) => {
         var i;
         const o = tt(t, n.schema),
@@ -17179,30 +17182,30 @@
         if (l.parent.content.size === 0 && l.node(-1).childCount === l.indexAfter(-1)) {
             if (l.depth === 2 || l.node(-3).type !== o || l.index(-2) !== l.node(-2).childCount - 1) return !1;
             if (r) {
                 let v = $.empty;
                 const x = l.index(-1) ? 1 : l.index(-2) ? 2 : 3;
                 for (let V = l.depth - x; V >= l.depth - 3; V -= 1) v = $.from(l.node(V).copy(v));
                 const w = l.indexAfter(-1) < l.node(-2).childCount ? 1 : l.indexAfter(-2) < l.node(-3).childCount ? 2 : 3,
-                    S = Gi(d, l.node().type.name, l.node().attrs),
+                    S = Xi(d, l.node().type.name, l.node().attrs),
                     y = ((i = o.contentMatch.defaultType) === null || i === void 0 ? void 0 : i.createAndFill(S)) || void 0;
                 v = v.append($.from(o.createAndFill(null, y) || void 0));
                 const I = l.before(l.depth - (x - 1));
                 e.replace(I, l.after(-w), new q(v, 4 - x, 0));
                 let T = -1;
                 e.doc.nodesBetween(I, e.doc.content.size, (V, N) => {
                     if (T > -1) return !1;
                     V.isTextblock && V.content.size === 0 && (T = N + 1)
                 }), T > -1 && e.setSelection(xe.near(e.doc.resolve(T))), e.scrollIntoView()
             }
             return !0
         }
         const f = a.pos === l.end() ? u.contentMatchAt(0).defaultType : null,
-            h = Gi(d, u.type.name, u.attrs),
-            p = Gi(d, l.node().type.name, l.node().attrs);
+            h = Xi(d, u.type.name, u.attrs),
+            p = Xi(d, l.node().type.name, l.node().attrs);
         e.delete(l.pos, a.pos);
         const g = f ? [{
             type: o,
             attrs: h
         }, {
             type: f,
             attrs: p
@@ -17236,15 +17239,15 @@
         const n = Uc(o => o.type === e)(t.selection);
         if (!n) return !0;
         const r = t.doc.resolve(n.start).after(n.depth);
         if (r === void 0) return !0;
         const s = t.doc.nodeAt(r);
         return n.node.type === (s == null ? void 0 : s.type) && lr(t.doc, r) && t.join(r), !0
     },
-    lE = (t, e, n, r = {}) => ({
+    cE = (t, e, n, r = {}) => ({
         editor: s,
         tr: i,
         state: o,
         dispatch: l,
         chain: a,
         commands: c,
         can: u
@@ -17267,41 +17270,41 @@
         }
         return !n || !y || !l ? a().command(() => u().wrapInList(h, r) ? !0 : c.clearNodes()).wrapInList(h, r).command(() => Xl(i, h)).command(() => Ql(i, h)).run() : a().command(() => {
             const T = u().wrapInList(h, r),
                 V = y.filter(N => f.includes(N.type.name));
             return i.ensureMarks(V), T ? !0 : c.clearNodes()
         }).wrapInList(h, r).command(() => Xl(i, h)).command(() => Ql(i, h)).run()
     },
-    aE = (t, e = {}, n = {}) => ({
+    uE = (t, e = {}, n = {}) => ({
         state: r,
         commands: s
     }) => {
         const {
             extendEmptyMarkRange: i = !1
         } = n, o = cr(t, r.schema);
         return Ua(r, o, e) ? s.unsetMark(o, {
             extendEmptyMarkRange: i
         }) : s.setMark(o, e)
     },
-    cE = (t, e, n = {}) => ({
+    dE = (t, e, n = {}) => ({
         state: r,
         commands: s
     }) => {
         const i = tt(t, r.schema),
             o = tt(e, r.schema);
         return gi(r, i, n) ? s.setNode(o) : s.setNode(i, n)
     },
-    uE = (t, e = {}) => ({
+    fE = (t, e = {}) => ({
         state: n,
         commands: r
     }) => {
         const s = tt(t, n.schema);
         return gi(n, s, e) ? r.lift(s) : r.wrapIn(s, e)
     },
-    dE = () => ({
+    hE = () => ({
         state: t,
         dispatch: e
     }) => {
         const n = t.plugins;
         for (let r = 0; r < n.length; r += 1) {
             const s = n[r];
             let i;
@@ -17316,29 +17319,29 @@
                     } else o.delete(i.from, i.to)
                 }
                 return !0
             }
         }
         return !1
     },
-    fE = () => ({
+    pE = () => ({
         tr: t,
         dispatch: e
     }) => {
         const {
             selection: n
         } = t, {
             empty: r,
             ranges: s
         } = n;
         return r || e && s.forEach(i => {
             t.removeMark(i.$from.pos, i.$to.pos)
         }), !0
     },
-    hE = (t, e = {}) => ({
+    mE = (t, e = {}) => ({
         tr: n,
         state: r,
         dispatch: s
     }) => {
         var i;
         const {
             extendEmptyMarkRange: o = !1
@@ -17359,15 +17362,15 @@
                 g = zc(c, a, p);
             g && (f = g.from, h = g.to), n.removeMark(f, h, a)
         } else d.forEach(f => {
             n.removeMark(f.$from.pos, f.$to.pos, a)
         });
         return n.removeStoredMark(a), !0
     },
-    pE = (t, e = {}) => ({
+    gE = (t, e = {}) => ({
         tr: n,
         state: r,
         dispatch: s
     }) => {
         let i = null,
             o = null;
         const l = ll(typeof t == "string" ? t : t.name, r.schema);
@@ -17387,104 +17390,104 @@
                             ...e
                         }))
                     }
                 })
             })
         }), !0) : !1
     },
-    mE = (t, e = {}) => ({
+    yE = (t, e = {}) => ({
         state: n,
         dispatch: r
     }) => {
         const s = tt(t, n.schema);
-        return $_(s, e)(n, r)
+        return F_(s, e)(n, r)
     },
-    gE = (t, e = {}) => ({
+    bE = (t, e = {}) => ({
         state: n,
         dispatch: r
     }) => {
         const s = tt(t, n.schema);
-        return L_(s, e)(n, r)
+        return B_(s, e)(n, r)
     };
-var yE = Object.freeze({
+var vE = Object.freeze({
     __proto__: null,
-    blur: sC,
-    clearContent: iC,
-    clearNodes: oC,
-    command: lC,
-    createParagraphNear: aC,
-    deleteCurrentNode: cC,
-    deleteNode: uC,
-    deleteRange: dC,
-    deleteSelection: fC,
-    enter: hC,
-    exitCode: pC,
-    extendMarkRange: gC,
-    first: yC,
-    focus: bC,
-    forEach: vC,
-    insertContent: xC,
-    insertContentAt: SC,
-    joinUp: _C,
-    joinDown: CC,
-    joinBackward: EC,
-    joinForward: TC,
-    keyboardShortcut: MC,
-    lift: AC,
-    liftEmptyBlock: NC,
-    liftListItem: RC,
-    newlineInCode: DC,
-    resetAttributes: IC,
-    scrollIntoView: PC,
-    selectAll: $C,
-    selectNodeBackward: LC,
-    selectNodeForward: FC,
-    selectParentNode: BC,
-    selectTextblockEnd: HC,
-    selectTextblockStart: zC,
-    setContent: VC,
-    setMark: ZC,
-    setMeta: eE,
-    setNode: tE,
-    setNodeSelection: nE,
-    setTextSelection: rE,
-    sinkListItem: sE,
-    splitBlock: iE,
-    splitListItem: oE,
-    toggleList: lE,
-    toggleMark: aE,
-    toggleNode: cE,
-    toggleWrap: uE,
-    undoInputRule: dE,
-    unsetAllMarks: fE,
-    unsetMark: hE,
-    updateAttributes: pE,
-    wrapIn: mE,
-    wrapInList: gE
+    blur: oC,
+    clearContent: lC,
+    clearNodes: aC,
+    command: cC,
+    createParagraphNear: uC,
+    deleteCurrentNode: dC,
+    deleteNode: fC,
+    deleteRange: hC,
+    deleteSelection: pC,
+    enter: mC,
+    exitCode: gC,
+    extendMarkRange: bC,
+    first: vC,
+    focus: xC,
+    forEach: kC,
+    insertContent: wC,
+    insertContentAt: CC,
+    joinUp: EC,
+    joinDown: TC,
+    joinBackward: OC,
+    joinForward: MC,
+    keyboardShortcut: NC,
+    lift: RC,
+    liftEmptyBlock: DC,
+    liftListItem: IC,
+    newlineInCode: PC,
+    resetAttributes: $C,
+    scrollIntoView: LC,
+    selectAll: FC,
+    selectNodeBackward: BC,
+    selectNodeForward: HC,
+    selectParentNode: zC,
+    selectTextblockEnd: VC,
+    selectTextblockStart: jC,
+    setContent: UC,
+    setMark: tE,
+    setMeta: nE,
+    setNode: rE,
+    setNodeSelection: sE,
+    setTextSelection: iE,
+    sinkListItem: oE,
+    splitBlock: lE,
+    splitListItem: aE,
+    toggleList: cE,
+    toggleMark: uE,
+    toggleNode: dE,
+    toggleWrap: fE,
+    undoInputRule: hE,
+    unsetAllMarks: pE,
+    unsetMark: mE,
+    updateAttributes: gE,
+    wrapIn: yE,
+    wrapInList: bE
 });
-const bE = kt.create({
+const xE = kt.create({
         name: "commands",
         addCommands() {
             return {
-                ...yE
+                ...vE
             }
         }
     }),
-    vE = kt.create({
+    kE = kt.create({
         name: "editable",
         addProseMirrorPlugins() {
             return [new Mt({
                 key: new Sn("editable"),
                 props: {
                     editable: () => this.editor.options.editable
                 }
             })]
         }
     }),
-    xE = kt.create({
+    wE = kt.create({
         name: "focusEvents",
         addProseMirrorPlugins() {
             const {
                 editor: t
             } = this;
             return [new Mt({
                 key: new Sn("focusEvents"),
@@ -17505,15 +17508,15 @@
                             return e.dispatch(r), !1
                         }
                     }
                 }
             })]
         }
     }),
-    kE = kt.create({
+    SE = kt.create({
         name: "keymap",
         addKeyboardShortcuts() {
             const t = () => this.editor.commands.first(({
                     commands: o
                 }) => [() => o.undoInputRule(), () => o.command(({
                     tr: l
                 }) => {
@@ -17583,37 +17586,37 @@
                             state: f
                         });
                     if (h.clearNodes(), !!d.steps.length) return d
                 }
             })]
         }
     }),
-    wE = kt.create({
+    _E = kt.create({
         name: "tabindex",
         addProseMirrorPlugins() {
             return [new Mt({
                 key: new Sn("tabindex"),
                 props: {
                     attributes: this.editor.isEditable ? {
                         tabindex: "0"
                     } : {}
                 }
             })]
         }
     });
-var SE = Object.freeze({
+var CE = Object.freeze({
     __proto__: null,
-    ClipboardTextSerializer: rC,
-    Commands: bE,
-    Editable: vE,
-    FocusEvents: xE,
-    Keymap: kE,
-    Tabindex: wE
+    ClipboardTextSerializer: iC,
+    Commands: xE,
+    Editable: kE,
+    FocusEvents: wE,
+    Keymap: SE,
+    Tabindex: _E
 });
-const _E = `.ProseMirror {
+const EE = `.ProseMirror {
   position: relative;
 }
 
 .ProseMirror {
   word-wrap: break-word;
   white-space: pre-wrap;
   white-space: break-spaces;
@@ -17681,21 +17684,21 @@
   display: block;
 }
 
 .tippy-box[data-animation=fade][data-state=hidden] {
   opacity: 0
 }`;
 
-function CE(t, e) {
+function TE(t, e) {
     const n = document.querySelector("style[data-tiptap-style]");
     if (n !== null) return n;
     const r = document.createElement("style");
     return e && r.setAttribute("nonce", e), r.setAttribute("data-tiptap-style", ""), r.innerHTML = t, document.getElementsByTagName("head")[0].appendChild(r), r
 }
-let EE = class extends j_ {
+let OE = class extends W_ {
     constructor(e = {}) {
         super(), this.isFocused = !1, this.extensionStorage = {}, this.options = {
             element: document.createElement("div"),
             content: "",
             injectCSS: !0,
             injectNonce: void 0,
             extensions: [],
@@ -17731,15 +17734,15 @@
     chain() {
         return this.commandManager.chain()
     }
     can() {
         return this.commandManager.can()
     }
     injectCSS() {
-        this.options.injectCSS && document && (this.css = CE(_E, this.options.injectNonce))
+        this.options.injectCSS && document && (this.css = TE(EE, this.options.injectNonce))
     }
     setOptions(e = {}) {
         this.options = {
             ...this.options,
             ...e
         }, !(!this.view || !this.state || this.isDestroyed) && (this.options.editorProps && this.view.setProps(this.options.editorProps), this.view.updateState(this.state))
     }
@@ -17769,29 +17772,29 @@
         const n = typeof e == "string" ? `${e}$` : e.key,
             r = this.state.reconfigure({
                 plugins: this.state.plugins.filter(s => !s.key.startsWith(n))
             });
         this.view.updateState(r)
     }
     createExtensionManager() {
-        const n = [...this.options.enableCoreExtensions ? Object.values(SE) : [], ...this.options.extensions].filter(r => ["extension", "node", "mark"].includes(r == null ? void 0 : r.type));
+        const n = [...this.options.enableCoreExtensions ? Object.values(CE) : [], ...this.options.extensions].filter(r => ["extension", "node", "mark"].includes(r == null ? void 0 : r.type));
         this.extensionManager = new Jr(n, this)
     }
     createCommandManager() {
         this.commandManager = new rl({
             editor: this
         })
     }
     createSchema() {
         this.schema = this.extensionManager.schema
     }
     createView() {
         const e = Lm(this.options.content, this.schema, this.options.parseOptions),
             n = Pm(e, this.options.autofocus);
-        this.view = new l_(this.options.element, {
+        this.view = new c_(this.options.element, {
             ...this.options.editorProps,
             dispatchTransaction: this.dispatchTransaction.bind(this),
             state: Kr.create({
                 doc: e,
                 selection: n || void 0
             })
         });
@@ -17846,44 +17849,44 @@
             transaction: e
         }), !(!e.docChanged || e.getMeta("preventUpdate")) && this.emit("update", {
             editor: this,
             transaction: e
         })
     }
     getAttributes(e) {
-        return JC(this.state, e)
+        return YC(this.state, e)
     }
     isActive(e, n) {
         const r = typeof e == "string" ? e : null,
             s = typeof e == "string" ? n : e;
-        return GC(this.state, r, s)
+        return XC(this.state, r, s)
     }
     getJSON() {
         return this.state.doc.toJSON()
     }
     getHTML() {
-        return WC(this.state.doc.content, this.schema)
+        return KC(this.state.doc.content, this.schema)
     }
     getText(e) {
         const {
             blockSeparator: n = `
 
 `,
             textSerializers: r = {}
         } = e || {};
-        return qC(this.state.doc, {
+        return JC(this.state.doc, {
             blockSeparator: n,
             textSerializers: {
                 ...Im(this.schema),
                 ...r
             }
         })
     }
     get isEmpty() {
-        return YC(this.state.doc)
+        return QC(this.state.doc)
     }
     getCharacterCount() {
         return console.warn('[tiptap warn]: "editor.getCharacterCount()" is deprecated. Please use "editor.storage.characterCount.characters()" instead.'), this.state.doc.content.size - 2
     }
     destroy() {
         this.emit("destroy"), this.view && this.view.destroy(), this.removeAllListeners()
     }
@@ -17914,15 +17917,15 @@
                 if (Fm(n.from, n.to, e.doc).filter(h => h.mark.type.excluded.find(g => g === t.type && g !== h.mark.type)).filter(h => h.to > u).length) return null;
                 d < n.to && i.delete(d, n.to), u > n.from && i.delete(n.from + c, u), a = n.from + c + o.length, i.addMark(n.from + c, a, t.type.create(s || {})), i.removeStoredMark(t.type)
             }
         }
     })
 }
 
-function TE(t) {
+function ME(t) {
     return new il({
         find: t.find,
         handler: ({
             state: e,
             range: n,
             match: r
         }) => {
@@ -18077,15 +18080,15 @@
             name: n.name,
             options: n.options
         })), n
     }
 }
 
 function ys(t) {
-    return new X_({
+    return new Z_({
         find: t.find,
         handler: ({
             state: e,
             range: n,
             match: r
         }) => {
             const s = be(t.getAttributes, void 0, r);
@@ -18105,37 +18108,37 @@
     })
 }
 var Ct = "top",
     qt = "bottom",
     Kt = "right",
     Et = "left",
     Wc = "auto",
-    Si = [Ct, qt, Kt, Et],
+    Ci = [Ct, qt, Kt, Et],
     bs = "start",
     bi = "end",
-    OE = "clippingParents",
+    AE = "clippingParents",
     Hm = "viewport",
     Ls = "popper",
-    ME = "reference",
-    pf = Si.reduce(function(t, e) {
+    NE = "reference",
+    pf = Ci.reduce(function(t, e) {
         return t.concat([e + "-" + bs, e + "-" + bi])
     }, []),
-    zm = [].concat(Si, [Wc]).reduce(function(t, e) {
+    zm = [].concat(Ci, [Wc]).reduce(function(t, e) {
         return t.concat([e, e + "-" + bs, e + "-" + bi])
     }, []),
-    AE = "beforeRead",
-    NE = "read",
-    RE = "afterRead",
-    DE = "beforeMain",
-    IE = "main",
-    PE = "afterMain",
-    $E = "beforeWrite",
-    LE = "write",
-    FE = "afterWrite",
-    BE = [AE, NE, RE, DE, IE, PE, $E, LE, FE];
+    RE = "beforeRead",
+    DE = "read",
+    IE = "afterRead",
+    PE = "beforeMain",
+    $E = "main",
+    LE = "afterMain",
+    FE = "beforeWrite",
+    BE = "write",
+    HE = "afterWrite",
+    zE = [RE, DE, IE, PE, $E, LE, FE, BE, HE];
 
 function kn(t) {
     return t ? (t.nodeName || "").toLowerCase() : null
 }
 
 function It(t) {
     if (t == null) return window;
@@ -18158,28 +18161,28 @@
 
 function qc(t) {
     if (typeof ShadowRoot > "u") return !1;
     var e = It(t).ShadowRoot;
     return t instanceof e || t instanceof ShadowRoot
 }
 
-function HE(t) {
+function VE(t) {
     var e = t.state;
     Object.keys(e.elements).forEach(function(n) {
         var r = e.styles[n] || {},
             s = e.attributes[n] || {},
             i = e.elements[n];
         !Wt(i) || !kn(i) || (Object.assign(i.style, r), Object.keys(s).forEach(function(o) {
             var l = s[o];
             l === !1 ? i.removeAttribute(o) : i.setAttribute(o, l === !0 ? "" : l)
         }))
     })
 }
 
-function zE(t) {
+function jE(t) {
     var e = t.state,
         n = {
             popper: {
                 position: e.options.strategy,
                 left: "0",
                 top: "0",
                 margin: "0"
@@ -18204,24 +18207,24 @@
             })
         }
 }
 const Vm = {
     name: "applyStyles",
     enabled: !0,
     phase: "write",
-    fn: HE,
-    effect: zE,
+    fn: VE,
+    effect: jE,
     requires: ["computeStyles"]
 };
 
 function gn(t) {
     return t.split("-")[0]
 }
 var Ir = Math.max,
-    ko = Math.min,
+    So = Math.min,
     vs = Math.round;
 
 function qa() {
     var t = navigator.userAgentData;
     return t != null && t.brands && Array.isArray(t.brands) ? t.brands.map(function(e) {
         return e.brand + "/" + e.version
     }).join(" ") : navigator.userAgent
@@ -18281,15 +18284,15 @@
     return !1
 }
 
 function Dn(t) {
     return It(t).getComputedStyle(t)
 }
 
-function VE(t) {
+function UE(t) {
     return ["table", "td", "th"].indexOf(kn(t)) >= 0
 }
 
 function ur(t) {
     return ((Fr(t) ? t.ownerDocument : t.document) || window.document).documentElement
 }
 
@@ -18297,15 +18300,15 @@
     return kn(t) === "html" ? t : t.assignedSlot || t.parentNode || (qc(t) ? t.host : null) || ur(t)
 }
 
 function mf(t) {
     return !Wt(t) || Dn(t).position === "fixed" ? null : t.offsetParent
 }
 
-function jE(t) {
+function WE(t) {
     var e = /firefox/i.test(qa()),
         n = /Trident/i.test(qa());
     if (n && Wt(t)) {
         var r = Dn(t);
         if (r.position === "fixed") return null
     }
     var s = cl(t);
@@ -18313,28 +18316,28 @@
         var i = Dn(s);
         if (i.transform !== "none" || i.perspective !== "none" || i.contain === "paint" || ["transform", "perspective"].indexOf(i.willChange) !== -1 || e && i.willChange === "filter" || e && i.filter && i.filter !== "none") return s;
         s = s.parentNode
     }
     return null
 }
 
-function _i(t) {
-    for (var e = It(t), n = mf(t); n && VE(n) && Dn(n).position === "static";) n = mf(n);
-    return n && (kn(n) === "html" || kn(n) === "body" && Dn(n).position === "static") ? e : n || jE(t) || e
+function Ei(t) {
+    for (var e = It(t), n = mf(t); n && UE(n) && Dn(n).position === "static";) n = mf(n);
+    return n && (kn(n) === "html" || kn(n) === "body" && Dn(n).position === "static") ? e : n || WE(t) || e
 }
 
 function Jc(t) {
     return ["top", "bottom"].indexOf(t) >= 0 ? "x" : "y"
 }
 
 function ei(t, e, n) {
-    return Ir(t, ko(e, n))
+    return Ir(t, So(e, n))
 }
 
-function UE(t, e, n) {
+function qE(t, e, n) {
     var r = ei(t, e, n);
     return r > n ? n : r
 }
 
 function Wm() {
     return {
         top: 0,
@@ -18349,77 +18352,77 @@
 }
 
 function Km(t, e) {
     return e.reduce(function(n, r) {
         return n[r] = t, n
     }, {})
 }
-var WE = function(e, n) {
+var KE = function(e, n) {
     return e = typeof e == "function" ? e(Object.assign({}, n.rects, {
         placement: n.placement
-    })) : e, qm(typeof e != "number" ? e : Km(e, Si))
+    })) : e, qm(typeof e != "number" ? e : Km(e, Ci))
 };
 
-function qE(t) {
+function JE(t) {
     var e, n = t.state,
         r = t.name,
         s = t.options,
         i = n.elements.arrow,
         o = n.modifiersData.popperOffsets,
         l = gn(n.placement),
         a = Jc(l),
         c = [Et, Kt].indexOf(l) >= 0,
         u = c ? "height" : "width";
     if (!(!i || !o)) {
-        var d = WE(s.padding, n),
+        var d = KE(s.padding, n),
             f = Kc(i),
             h = a === "y" ? Ct : Et,
             p = a === "y" ? qt : Kt,
             g = n.rects.reference[u] + n.rects.reference[a] - o[a] - n.rects.popper[u],
             v = o[a] - n.rects.reference[a],
-            x = _i(i),
+            x = Ei(i),
             w = x ? a === "y" ? x.clientHeight || 0 : x.clientWidth || 0 : 0,
             S = g / 2 - v / 2,
             y = d[h],
             I = w - f[u] - d[p],
             T = w / 2 - f[u] / 2 + S,
             V = ei(y, T, I),
             N = a;
         n.modifiersData[r] = (e = {}, e[N] = V, e.centerOffset = V - T, e)
     }
 }
 
-function KE(t) {
+function GE(t) {
     var e = t.state,
         n = t.options,
         r = n.element,
         s = r === void 0 ? "[data-popper-arrow]" : r;
     s != null && (typeof s == "string" && (s = e.elements.popper.querySelector(s), !s) || Um(e.elements.popper, s) && (e.elements.arrow = s))
 }
-const JE = {
+const YE = {
     name: "arrow",
     enabled: !0,
     phase: "main",
-    fn: qE,
-    effect: KE,
+    fn: JE,
+    effect: GE,
     requires: ["popperOffsets"],
     requiresIfExists: ["preventOverflow"]
 };
 
 function ks(t) {
     return t.split("-")[1]
 }
-var GE = {
+var XE = {
     top: "auto",
     right: "auto",
     bottom: "auto",
     left: "auto"
 };
 
-function YE(t, e) {
+function QE(t, e) {
     var n = t.x,
         r = t.y,
         s = e.devicePixelRatio || 1;
     return {
         x: vs(n * s) / s || 0,
         y: vs(r * s) / s || 0
     }
@@ -18450,15 +18453,15 @@
     h = v.x, g = v.y;
     var x = o.hasOwnProperty("x"),
         w = o.hasOwnProperty("y"),
         S = Et,
         y = Ct,
         I = window;
     if (c) {
-        var T = _i(n),
+        var T = Ei(n),
             V = "clientHeight",
             N = "clientWidth";
         if (T === It(n) && (T = ur(n), Dn(T).position !== "static" && l === "absolute" && (V = "scrollHeight", N = "scrollWidth")), T = T, s === Ct || (s === Et || s === Kt) && i === bi) {
             y = qt;
             var G = d && T === I && I.visualViewport ? I.visualViewport.height : T[V];
             g -= G - r.height, g *= a ? 1 : -1
         }
@@ -18466,30 +18469,30 @@
             S = Kt;
             var J = d && T === I && I.visualViewport ? I.visualViewport.width : T[N];
             h -= J - r.width, h *= a ? 1 : -1
         }
     }
     var ne = Object.assign({
             position: l
-        }, c && GE),
-        H = u === !0 ? YE({
+        }, c && XE),
+        H = u === !0 ? QE({
             x: h,
             y: g
         }, It(n)) : {
             x: h,
             y: g
         };
     if (h = H.x, g = H.y, a) {
         var ie;
         return Object.assign({}, ne, (ie = {}, ie[y] = w ? "0" : "", ie[S] = x ? "0" : "", ie.transform = (I.devicePixelRatio || 1) <= 1 ? "translate(" + h + "px, " + g + "px)" : "translate3d(" + h + "px, " + g + "px, 0)", ie))
     }
     return Object.assign({}, ne, (e = {}, e[y] = w ? g + "px" : "", e[S] = x ? h + "px" : "", e.transform = "", e))
 }
 
-function XE(t) {
+function ZE(t) {
     var e = t.state,
         n = t.options,
         r = n.gpuAcceleration,
         s = r === void 0 ? !0 : r,
         i = n.adaptive,
         o = i === void 0 ? !0 : i,
         l = n.roundOffsets,
@@ -18512,72 +18515,72 @@
         position: "absolute",
         adaptive: !1,
         roundOffsets: a
     })))), e.attributes.popper = Object.assign({}, e.attributes.popper, {
         "data-popper-placement": e.placement
     })
 }
-const QE = {
+const eT = {
     name: "computeStyles",
     enabled: !0,
     phase: "beforeWrite",
-    fn: XE,
+    fn: ZE,
     data: {}
 };
-var Fi = {
+var Hi = {
     passive: !0
 };
 
-function ZE(t) {
+function tT(t) {
     var e = t.state,
         n = t.instance,
         r = t.options,
         s = r.scroll,
         i = s === void 0 ? !0 : s,
         o = r.resize,
         l = o === void 0 ? !0 : o,
         a = It(e.elements.popper),
         c = [].concat(e.scrollParents.reference, e.scrollParents.popper);
     return i && c.forEach(function(u) {
-            u.addEventListener("scroll", n.update, Fi)
-        }), l && a.addEventListener("resize", n.update, Fi),
+            u.addEventListener("scroll", n.update, Hi)
+        }), l && a.addEventListener("resize", n.update, Hi),
         function() {
             i && c.forEach(function(u) {
-                u.removeEventListener("scroll", n.update, Fi)
-            }), l && a.removeEventListener("resize", n.update, Fi)
+                u.removeEventListener("scroll", n.update, Hi)
+            }), l && a.removeEventListener("resize", n.update, Hi)
         }
 }
-const eT = {
+const nT = {
     name: "eventListeners",
     enabled: !0,
     phase: "write",
     fn: function() {},
-    effect: ZE,
+    effect: tT,
     data: {}
 };
-var tT = {
+var rT = {
     left: "right",
     right: "left",
     bottom: "top",
     top: "bottom"
 };
 
-function Yi(t) {
+function Qi(t) {
     return t.replace(/left|right|bottom|top/g, function(e) {
-        return tT[e]
+        return rT[e]
     })
 }
-var nT = {
+var sT = {
     start: "end",
     end: "start"
 };
 
 function yf(t) {
     return t.replace(/start|end/g, function(e) {
-        return nT[e]
+        return sT[e]
     })
 }
 
 function Gc(t) {
     var e = It(t),
         n = e.pageXOffset,
         r = e.pageYOffset;
@@ -18587,15 +18590,15 @@
     }
 }
 
 function Yc(t) {
     return xs(ur(t)).left + Gc(t).scrollLeft
 }
 
-function rT(t, e) {
+function iT(t, e) {
     var n = It(t),
         r = ur(t),
         s = n.visualViewport,
         i = r.clientWidth,
         o = r.clientHeight,
         l = 0,
         a = 0;
@@ -18608,15 +18611,15 @@
         width: i,
         height: o,
         x: l + Yc(t),
         y: a
     }
 }
 
-function sT(t) {
+function oT(t) {
     var e, n = ur(t),
         r = Gc(t),
         s = (e = t.ownerDocument) == null ? void 0 : e.body,
         i = Ir(n.scrollWidth, n.clientWidth, s ? s.scrollWidth : 0, s ? s.clientWidth : 0),
         o = Ir(n.scrollHeight, n.clientHeight, s ? s.scrollHeight : 0, s ? s.clientHeight : 0),
         l = -r.scrollLeft + Yc(t),
         a = -r.scrollTop;
@@ -18656,39 +18659,39 @@
         left: t.x,
         top: t.y,
         right: t.x + t.width,
         bottom: t.y + t.height
     })
 }
 
-function iT(t, e) {
+function lT(t, e) {
     var n = xs(t, !1, e === "fixed");
     return n.top = n.top + t.clientTop, n.left = n.left + t.clientLeft, n.bottom = n.top + t.clientHeight, n.right = n.left + t.clientWidth, n.width = t.clientWidth, n.height = t.clientHeight, n.x = n.left, n.y = n.top, n
 }
 
 function bf(t, e, n) {
-    return e === Hm ? Ka(rT(t, n)) : Fr(e) ? iT(e, n) : Ka(sT(ur(t)))
+    return e === Hm ? Ka(iT(t, n)) : Fr(e) ? lT(e, n) : Ka(oT(ur(t)))
 }
 
-function oT(t) {
+function aT(t) {
     var e = ti(cl(t)),
         n = ["absolute", "fixed"].indexOf(Dn(t).position) >= 0,
-        r = n && Wt(t) ? _i(t) : t;
+        r = n && Wt(t) ? Ei(t) : t;
     return Fr(r) ? e.filter(function(s) {
         return Fr(s) && Um(s, r) && kn(s) !== "body"
     }) : []
 }
 
-function lT(t, e, n, r) {
-    var s = e === "clippingParents" ? oT(t) : [].concat(e),
+function cT(t, e, n, r) {
+    var s = e === "clippingParents" ? aT(t) : [].concat(e),
         i = [].concat(s, [n]),
         o = i[0],
         l = i.reduce(function(a, c) {
             var u = bf(t, c, r);
-            return a.top = Ir(u.top, a.top), a.right = ko(u.right, a.right), a.bottom = ko(u.bottom, a.bottom), a.left = Ir(u.left, a.left), a
+            return a.top = Ir(u.top, a.top), a.right = So(u.right, a.right), a.bottom = So(u.bottom, a.bottom), a.left = Ir(u.left, a.left), a
         }, bf(t, o, r));
     return l.width = l.right - l.left, l.height = l.bottom - l.top, l.x = l.left, l.y = l.top, l
 }
 
 function Gm(t) {
     var e = t.reference,
         n = t.element,
@@ -18748,28 +18751,28 @@
     e === void 0 && (e = {});
     var n = e,
         r = n.placement,
         s = r === void 0 ? t.placement : r,
         i = n.strategy,
         o = i === void 0 ? t.strategy : i,
         l = n.boundary,
-        a = l === void 0 ? OE : l,
+        a = l === void 0 ? AE : l,
         c = n.rootBoundary,
         u = c === void 0 ? Hm : c,
         d = n.elementContext,
         f = d === void 0 ? Ls : d,
         h = n.altBoundary,
         p = h === void 0 ? !1 : h,
         g = n.padding,
         v = g === void 0 ? 0 : g,
-        x = qm(typeof v != "number" ? v : Km(v, Si)),
-        w = f === Ls ? ME : Ls,
+        x = qm(typeof v != "number" ? v : Km(v, Ci)),
+        w = f === Ls ? NE : Ls,
         S = t.rects.popper,
         y = t.elements[p ? w : f],
-        I = lT(Fr(y) ? y : y.contextElement || ur(t.elements.popper), a, u, o),
+        I = cT(Fr(y) ? y : y.contextElement || ur(t.elements.popper), a, u, o),
         T = xs(t.elements.reference),
         V = Gm({
             reference: T,
             element: S,
             strategy: "absolute",
             placement: s
         }),
@@ -18782,35 +18785,35 @@
             right: G.right - I.right + x.right
         },
         ne = t.modifiersData.offset;
     if (f === Ls && ne) {
         var H = ne[s];
         Object.keys(J).forEach(function(ie) {
             var Ae = [Kt, qt].indexOf(ie) >= 0 ? 1 : -1,
-                Be = [Ct, qt].indexOf(ie) >= 0 ? "y" : "x";
-            J[ie] += H[Be] * Ae
+                He = [Ct, qt].indexOf(ie) >= 0 ? "y" : "x";
+            J[ie] += H[He] * Ae
         })
     }
     return J
 }
 
-function aT(t, e) {
+function uT(t, e) {
     e === void 0 && (e = {});
     var n = e,
         r = n.placement,
         s = n.boundary,
         i = n.rootBoundary,
         o = n.padding,
         l = n.flipVariations,
         a = n.allowedAutoPlacements,
         c = a === void 0 ? zm : a,
         u = ks(r),
         d = u ? l ? pf : pf.filter(function(p) {
             return ks(p) === u
-        }) : Si,
+        }) : Ci,
         f = d.filter(function(p) {
             return c.indexOf(p) >= 0
         });
     f.length === 0 && (f = d);
     var h = f.reduce(function(p, g) {
         return p[g] = vi(t, {
             placement: g,
@@ -18820,58 +18823,58 @@
         })[gn(g)], p
     }, {});
     return Object.keys(h).sort(function(p, g) {
         return h[p] - h[g]
     })
 }
 
-function cT(t) {
+function dT(t) {
     if (gn(t) === Wc) return [];
-    var e = Yi(t);
+    var e = Qi(t);
     return [yf(t), e, yf(e)]
 }
 
-function uT(t) {
+function fT(t) {
     var e = t.state,
         n = t.options,
         r = t.name;
     if (!e.modifiersData[r]._skip) {
-        for (var s = n.mainAxis, i = s === void 0 ? !0 : s, o = n.altAxis, l = o === void 0 ? !0 : o, a = n.fallbackPlacements, c = n.padding, u = n.boundary, d = n.rootBoundary, f = n.altBoundary, h = n.flipVariations, p = h === void 0 ? !0 : h, g = n.allowedAutoPlacements, v = e.options.placement, x = gn(v), w = x === v, S = a || (w || !p ? [Yi(v)] : cT(v)), y = [v].concat(S).reduce(function(St, M) {
-                return St.concat(gn(M) === Wc ? aT(e, {
+        for (var s = n.mainAxis, i = s === void 0 ? !0 : s, o = n.altAxis, l = o === void 0 ? !0 : o, a = n.fallbackPlacements, c = n.padding, u = n.boundary, d = n.rootBoundary, f = n.altBoundary, h = n.flipVariations, p = h === void 0 ? !0 : h, g = n.allowedAutoPlacements, v = e.options.placement, x = gn(v), w = x === v, S = a || (w || !p ? [Qi(v)] : dT(v)), y = [v].concat(S).reduce(function(St, M) {
+                return St.concat(gn(M) === Wc ? uT(e, {
                     placement: M,
                     boundary: u,
                     rootBoundary: d,
                     padding: c,
                     flipVariations: p,
                     allowedAutoPlacements: g
                 }) : M)
             }, []), I = e.rects.reference, T = e.rects.popper, V = new Map, N = !0, G = y[0], J = 0; J < y.length; J++) {
             var ne = y[J],
                 H = gn(ne),
                 ie = ks(ne) === bs,
                 Ae = [Ct, qt].indexOf(H) >= 0,
-                Be = Ae ? "width" : "height",
+                He = Ae ? "width" : "height",
                 ge = vi(e, {
                     placement: ne,
                     boundary: u,
                     rootBoundary: d,
                     altBoundary: f,
                     padding: c
                 }),
-                fe = Ae ? ie ? Kt : Et : ie ? qt : Ct;
-            I[Be] > T[Be] && (fe = Yi(fe));
-            var ae = Yi(fe),
-                He = [];
-            if (i && He.push(ge[H] <= 0), l && He.push(ge[fe] <= 0, ge[ae] <= 0), He.every(function(St) {
+                he = Ae ? ie ? Kt : Et : ie ? qt : Ct;
+            I[He] > T[He] && (he = Qi(he));
+            var ae = Qi(he),
+                ze = [];
+            if (i && ze.push(ge[H] <= 0), l && ze.push(ge[he] <= 0, ge[ae] <= 0), ze.every(function(St) {
                     return St
                 })) {
                 G = ne, N = !1;
                 break
             }
-            V.set(ne, He)
+            V.set(ne, ze)
         }
         if (N)
             for (var Ze = p ? 3 : 1, Ke = function(M) {
                     var j = y.find(function(z) {
                         var Y = V.get(z);
                         if (Y) return Y.slice(0, M).every(function(ye) {
                             return ye
@@ -18881,19 +18884,19 @@
                 }, Pe = Ze; Pe > 0; Pe--) {
                 var wt = Ke(Pe);
                 if (wt === "break") break
             }
         e.placement !== G && (e.modifiersData[r]._skip = !0, e.placement = G, e.reset = !0)
     }
 }
-const dT = {
+const hT = {
     name: "flip",
     enabled: !0,
     phase: "main",
-    fn: uT,
+    fn: fT,
     requiresIfExists: ["offset"],
     data: {
         _skip: !1
     }
 };
 
 function vf(t, e, n) {
@@ -18910,15 +18913,15 @@
 
 function xf(t) {
     return [Ct, Kt, qt, Et].some(function(e) {
         return t[e] >= 0
     })
 }
 
-function fT(t) {
+function pT(t) {
     var e = t.state,
         n = t.name,
         r = e.rects.reference,
         s = e.rects.popper,
         i = e.modifiersData.preventOverflow,
         o = vi(e, {
             elementContext: "reference"
@@ -18936,23 +18939,23 @@
         isReferenceHidden: u,
         hasPopperEscaped: d
     }, e.attributes.popper = Object.assign({}, e.attributes.popper, {
         "data-popper-reference-hidden": u,
         "data-popper-escaped": d
     })
 }
-const hT = {
+const mT = {
     name: "hide",
     enabled: !0,
     phase: "main",
     requiresIfExists: ["preventOverflow"],
-    fn: fT
+    fn: pT
 };
 
-function pT(t, e, n) {
+function gT(t, e, n) {
     var r = gn(t),
         s = [Et, Ct].indexOf(r) >= 0 ? -1 : 1,
         i = typeof n == "function" ? n(Object.assign({}, e, {
             placement: t
         })) : n,
         o = i[0],
         l = i[1];
@@ -18961,59 +18964,59 @@
         y: o
     } : {
         x: o,
         y: l
     }
 }
 
-function mT(t) {
+function yT(t) {
     var e = t.state,
         n = t.options,
         r = t.name,
         s = n.offset,
         i = s === void 0 ? [0, 0] : s,
         o = zm.reduce(function(u, d) {
-            return u[d] = pT(d, e.rects, i), u
+            return u[d] = gT(d, e.rects, i), u
         }, {}),
         l = o[e.placement],
         a = l.x,
         c = l.y;
     e.modifiersData.popperOffsets != null && (e.modifiersData.popperOffsets.x += a, e.modifiersData.popperOffsets.y += c), e.modifiersData[r] = o
 }
-const gT = {
+const bT = {
     name: "offset",
     enabled: !0,
     phase: "main",
     requires: ["popperOffsets"],
-    fn: mT
+    fn: yT
 };
 
-function yT(t) {
+function vT(t) {
     var e = t.state,
         n = t.name;
     e.modifiersData[n] = Gm({
         reference: e.rects.reference,
         element: e.rects.popper,
         strategy: "absolute",
         placement: e.placement
     })
 }
-const bT = {
+const xT = {
     name: "popperOffsets",
     enabled: !0,
     phase: "read",
-    fn: yT,
+    fn: vT,
     data: {}
 };
 
-function vT(t) {
+function kT(t) {
     return t === "x" ? "y" : "x"
 }
 
-function xT(t) {
+function wT(t) {
     var e = t.state,
         n = t.options,
         r = t.name,
         s = n.mainAxis,
         i = s === void 0 ? !0 : s,
         o = n.altAxis,
         l = o === void 0 ? !1 : o,
@@ -19031,15 +19034,15 @@
             padding: d,
             altBoundary: u
         }),
         x = gn(e.placement),
         w = ks(e.placement),
         S = !w,
         y = Jc(x),
-        I = vT(y),
+        I = kT(y),
         T = e.modifiersData.popperOffsets,
         V = e.rects.reference,
         N = e.rects.popper,
         G = typeof g == "function" ? g(Object.assign({}, e.rects, {
             placement: e.placement
         })) : g,
         J = typeof G == "number" ? {
@@ -19053,107 +19056,107 @@
         H = {
             x: 0,
             y: 0
         };
     if (T) {
         if (i) {
             var ie, Ae = y === "y" ? Ct : Et,
-                Be = y === "y" ? qt : Kt,
+                He = y === "y" ? qt : Kt,
                 ge = y === "y" ? "height" : "width",
-                fe = T[y],
-                ae = fe + v[Ae],
-                He = fe - v[Be],
+                he = T[y],
+                ae = he + v[Ae],
+                ze = he - v[He],
                 Ze = h ? -N[ge] / 2 : 0,
                 Ke = w === bs ? V[ge] : N[ge],
                 Pe = w === bs ? -N[ge] : -V[ge],
                 wt = e.elements.arrow,
                 St = h && wt ? Kc(wt) : {
                     width: 0,
                     height: 0
                 },
                 M = e.modifiersData["arrow#persistent"] ? e.modifiersData["arrow#persistent"].padding : Wm(),
                 j = M[Ae],
-                z = M[Be],
+                z = M[He],
                 Y = ei(0, V[ge], St[ge]),
                 ye = S ? V[ge] / 2 - Ze - Y - j - J.mainAxis : Ke - Y - j - J.mainAxis,
                 Ee = S ? -V[ge] / 2 + Ze + Y + z + J.mainAxis : Pe + Y + z + J.mainAxis,
-                ue = e.elements.arrow && _i(e.elements.arrow),
+                ue = e.elements.arrow && Ei(e.elements.arrow),
                 b = ue ? y === "y" ? ue.clientTop || 0 : ue.clientLeft || 0 : 0,
                 k = (ie = ne == null ? void 0 : ne[y]) != null ? ie : 0,
-                _ = fe + ye - k - b,
-                O = fe + Ee - k,
-                D = ei(h ? ko(ae, _) : ae, fe, h ? Ir(He, O) : He);
-            T[y] = D, H[y] = D - fe
+                _ = he + ye - k - b,
+                O = he + Ee - k,
+                D = ei(h ? So(ae, _) : ae, he, h ? Ir(ze, O) : ze);
+            T[y] = D, H[y] = D - he
         }
         if (l) {
             var F, U = y === "x" ? Ct : Et,
                 L = y === "x" ? qt : Kt,
                 B = T[I],
                 P = I === "y" ? "height" : "width",
                 Q = B + v[U],
                 K = B - v[L],
                 Z = [Ct, Et].indexOf(x) !== -1,
                 oe = (F = ne == null ? void 0 : ne[I]) != null ? F : 0,
                 pe = Z ? Q : B - V[P] - N[P] - oe + J.altAxis,
                 Ne = Z ? B + V[P] + N[P] - oe - J.altAxis : K,
-                we = h && Z ? UE(pe, B, Ne) : ei(h ? pe : Q, B, h ? Ne : K);
+                we = h && Z ? qE(pe, B, Ne) : ei(h ? pe : Q, B, h ? Ne : K);
             T[I] = we, H[I] = we - B
         }
         e.modifiersData[r] = H
     }
 }
-const kT = {
+const ST = {
     name: "preventOverflow",
     enabled: !0,
     phase: "main",
-    fn: xT,
+    fn: wT,
     requiresIfExists: ["offset"]
 };
 
-function wT(t) {
+function _T(t) {
     return {
         scrollLeft: t.scrollLeft,
         scrollTop: t.scrollTop
     }
 }
 
-function ST(t) {
-    return t === It(t) || !Wt(t) ? Gc(t) : wT(t)
+function CT(t) {
+    return t === It(t) || !Wt(t) ? Gc(t) : _T(t)
 }
 
-function _T(t) {
+function ET(t) {
     var e = t.getBoundingClientRect(),
         n = vs(e.width) / t.offsetWidth || 1,
         r = vs(e.height) / t.offsetHeight || 1;
     return n !== 1 || r !== 1
 }
 
-function CT(t, e, n) {
+function TT(t, e, n) {
     n === void 0 && (n = !1);
     var r = Wt(e),
-        s = Wt(e) && _T(e),
+        s = Wt(e) && ET(e),
         i = ur(e),
         o = xs(t, s, n),
         l = {
             scrollLeft: 0,
             scrollTop: 0
         },
         a = {
             x: 0,
             y: 0
         };
-    return (r || !r && !n) && ((kn(e) !== "body" || Xc(i)) && (l = ST(e)), Wt(e) ? (a = xs(e, !0), a.x += e.clientLeft, a.y += e.clientTop) : i && (a.x = Yc(i))), {
+    return (r || !r && !n) && ((kn(e) !== "body" || Xc(i)) && (l = CT(e)), Wt(e) ? (a = xs(e, !0), a.x += e.clientLeft, a.y += e.clientTop) : i && (a.x = Yc(i))), {
         x: o.left + l.scrollLeft - a.x,
         y: o.top + l.scrollTop - a.y,
         width: o.width,
         height: o.height
     }
 }
 
-function ET(t) {
+function OT(t) {
     var e = new Map,
         n = new Set,
         r = [];
     t.forEach(function(i) {
         e.set(i.name, i)
     });
 
@@ -19168,35 +19171,35 @@
         }), r.push(i)
     }
     return t.forEach(function(i) {
         n.has(i.name) || s(i)
     }), r
 }
 
-function TT(t) {
-    var e = ET(t);
-    return BE.reduce(function(n, r) {
+function MT(t) {
+    var e = OT(t);
+    return zE.reduce(function(n, r) {
         return n.concat(e.filter(function(s) {
             return s.phase === r
         }))
     }, [])
 }
 
-function OT(t) {
+function AT(t) {
     var e;
     return function() {
         return e || (e = new Promise(function(n) {
             Promise.resolve().then(function() {
                 e = void 0, n(t())
             })
         })), e
     }
 }
 
-function MT(t) {
+function NT(t) {
     var e = t.reduce(function(n, r) {
         var s = n[r.name];
         return n[r.name] = s ? Object.assign({}, s, r, {
             options: Object.assign({}, s.options, r.options),
             data: Object.assign({}, s.data, r.data)
         }) : r, n
     }, {});
@@ -19213,15 +19216,15 @@
 function wf() {
     for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
     return !e.some(function(r) {
         return !(r && typeof r.getBoundingClientRect == "function")
     })
 }
 
-function AT(t) {
+function RT(t) {
     t === void 0 && (t = {});
     var e = t,
         n = e.defaultModifiers,
         r = n === void 0 ? [] : n,
         s = e.defaultOptions,
         i = s === void 0 ? kf : s;
     return function(l, a, c) {
@@ -19244,27 +19247,27 @@
                 state: u,
                 setOptions: function(x) {
                     var w = typeof x == "function" ? x(u.options) : x;
                     g(), u.options = Object.assign({}, i, u.options, w), u.scrollParents = {
                         reference: Fr(l) ? ti(l) : l.contextElement ? ti(l.contextElement) : [],
                         popper: ti(a)
                     };
-                    var S = TT(MT([].concat(r, u.options.modifiers)));
+                    var S = MT(NT([].concat(r, u.options.modifiers)));
                     return u.orderedModifiers = S.filter(function(y) {
                         return y.enabled
                     }), p(), h.update()
                 },
                 forceUpdate: function() {
                     if (!f) {
                         var x = u.elements,
                             w = x.reference,
                             S = x.popper;
                         if (wf(w, S)) {
                             u.rects = {
-                                reference: CT(w, _i(S), u.options.strategy === "fixed"),
+                                reference: TT(w, Ei(S), u.options.strategy === "fixed"),
                                 popper: Kc(S)
                             }, u.reset = !1, u.placement = u.options.placement, u.orderedModifiers.forEach(function(J) {
                                 return u.modifiersData[J.name] = Object.assign({}, J.data)
                             });
                             for (var y = 0; y < u.orderedModifiers.length; y++) {
                                 if (u.reset === !0) {
                                     u.reset = !1, y = -1;
@@ -19281,15 +19284,15 @@
                                     name: G,
                                     instance: h
                                 }) || u)
                             }
                         }
                     }
                 },
-                update: OT(function() {
+                update: AT(function() {
                     return new Promise(function(v) {
                         h.forceUpdate(), v(u)
                     })
                 }),
                 destroy: function() {
                     g(), f = !0
                 }
@@ -19322,21 +19325,21 @@
             d.forEach(function(v) {
                 return v()
             }), d = []
         }
         return h
     }
 }
-var NT = [eT, bT, QE, Vm, gT, dT, kT, JE, hT],
-    RT = AT({
-        defaultModifiers: NT
+var DT = [nT, xT, eT, Vm, bT, hT, ST, YE, mT],
+    IT = RT({
+        defaultModifiers: DT
     }),
-    DT = "tippy-box",
+    PT = "tippy-box",
     Ym = "tippy-content",
-    IT = "tippy-backdrop",
+    $T = "tippy-backdrop",
     Xm = "tippy-arrow",
     Qm = "tippy-svg-arrow",
     br = {
         passive: !0,
         capture: !0
     },
     Zm = function() {
@@ -19366,37 +19369,37 @@
     return function(r) {
         clearTimeout(n), n = setTimeout(function() {
             t(r)
         }, e)
     }
 }
 
-function PT(t) {
+function LT(t) {
     return t.split(/\s+/).filter(Boolean)
 }
 
 function qr(t) {
     return [].concat(t)
 }
 
 function _f(t, e) {
     t.indexOf(e) === -1 && t.push(e)
 }
 
-function $T(t) {
+function FT(t) {
     return t.filter(function(e, n) {
         return t.indexOf(e) === n
     })
 }
 
-function LT(t) {
+function BT(t) {
     return t.split("-")[0]
 }
 
-function wo(t) {
+function _o(t) {
     return [].slice.call(t)
 }
 
 function Cf(t) {
     return Object.keys(t).reduce(function(e, n) {
         return t[n] !== void 0 && (e[n] = t[n]), e
     }, {})
@@ -19408,57 +19411,57 @@
 
 function ul(t) {
     return ["Element", "Fragment"].some(function(e) {
         return Qc(t, e)
     })
 }
 
-function FT(t) {
+function HT(t) {
     return Qc(t, "NodeList")
 }
 
-function BT(t) {
+function zT(t) {
     return Qc(t, "MouseEvent")
 }
 
-function HT(t) {
+function VT(t) {
     return !!(t && t._tippy && t._tippy.reference === t)
 }
 
-function zT(t) {
-    return ul(t) ? [t] : FT(t) ? wo(t) : Array.isArray(t) ? t : wo(document.querySelectorAll(t))
+function jT(t) {
+    return ul(t) ? [t] : HT(t) ? _o(t) : Array.isArray(t) ? t : _o(document.querySelectorAll(t))
 }
 
 function ea(t, e) {
     t.forEach(function(n) {
         n && (n.style.transitionDuration = e + "ms")
     })
 }
 
 function Ef(t, e) {
     t.forEach(function(n) {
         n && n.setAttribute("data-state", e)
     })
 }
 
-function VT(t) {
+function UT(t) {
     var e, n = qr(t),
         r = n[0];
     return r != null && (e = r.ownerDocument) != null && e.body ? r.ownerDocument : document
 }
 
-function jT(t, e) {
+function WT(t, e) {
     var n = e.clientX,
         r = e.clientY;
     return t.every(function(s) {
         var i = s.popperRect,
             o = s.popperState,
             l = s.props,
             a = l.interactiveBorder,
-            c = LT(o.placement),
+            c = BT(o.placement),
             u = o.modifiersData.offset;
         if (!u) return !0;
         var d = c === "bottom" ? u.top.y : 0,
             f = c === "top" ? u.bottom.y : 0,
             h = c === "right" ? u.left.x : 0,
             p = c === "left" ? u.right.x : 0,
             g = i.top - r + d > a,
@@ -19485,43 +19488,43 @@
     return !1
 }
 var cn = {
         isTouch: !1
     },
     Of = 0;
 
-function UT() {
+function qT() {
     cn.isTouch || (cn.isTouch = !0, window.performance && document.addEventListener("mousemove", tg))
 }
 
 function tg() {
     var t = performance.now();
     t - Of < 20 && (cn.isTouch = !1, document.removeEventListener("mousemove", tg)), Of = t
 }
 
-function WT() {
+function KT() {
     var t = document.activeElement;
-    if (HT(t)) {
+    if (VT(t)) {
         var e = t._tippy;
         t.blur && !e.state.isVisible && t.blur()
     }
 }
 
-function qT() {
-    document.addEventListener("touchstart", UT, br), window.addEventListener("blur", WT)
+function JT() {
+    document.addEventListener("touchstart", qT, br), window.addEventListener("blur", KT)
 }
-var KT = typeof window < "u" && typeof document < "u",
-    JT = KT ? !!window.msCrypto : !1,
-    GT = {
+var GT = typeof window < "u" && typeof document < "u",
+    YT = GT ? !!window.msCrypto : !1,
+    XT = {
         animateFill: !1,
         followCursor: !1,
         inlinePositioning: !1,
         sticky: !1
     },
-    YT = {
+    QT = {
         allowHTML: !1,
         animation: "fade",
         arrow: !0,
         content: "",
         inertia: !1,
         maxWidth: 350,
         role: "tooltip",
@@ -19560,17 +19563,17 @@
         plugins: [],
         popperOptions: {},
         render: null,
         showOnCreate: !1,
         touch: !0,
         trigger: "mouseenter focus",
         triggerTarget: null
-    }, GT, YT),
-    XT = Object.keys(Zt),
-    QT = function(e) {
+    }, XT, QT),
+    ZT = Object.keys(Zt),
+    eO = function(e) {
         var n = Object.keys(e);
         n.forEach(function(r) {
             Zt[r] = e[r]
         })
     };
 
 function ng(t) {
@@ -19583,18 +19586,18 @@
                 r[i] = t[i] !== void 0 ? t[i] : (l = Zt[i]) != null ? l : o
             }
             return r
         }, {});
     return Object.assign({}, t, n)
 }
 
-function ZT(t, e) {
+function tO(t, e) {
     var n = e ? Object.keys(ng(Object.assign({}, Zt, {
             plugins: e
-        }))) : XT,
+        }))) : ZT,
         r = n.reduce(function(s, i) {
             var o = (t.getAttribute("data-tippy-" + i) || "").trim();
             if (!o) return s;
             if (i === "content") s[i] = o;
             else try {
                 s[i] = JSON.parse(o)
             } catch {
@@ -19604,58 +19607,58 @@
         }, {});
     return r
 }
 
 function Mf(t, e) {
     var n = Object.assign({}, e, {
         content: eg(e.content, [t])
-    }, e.ignoreAttributes ? {} : ZT(t, e.plugins));
+    }, e.ignoreAttributes ? {} : tO(t, e.plugins));
     return n.aria = Object.assign({}, Zt.aria, n.aria), n.aria = {
         expanded: n.aria.expanded === "auto" ? e.interactive : n.aria.expanded,
         content: n.aria.content === "auto" ? e.interactive ? null : "describedby" : n.aria.content
     }, n
 }
-var eO = function() {
+var nO = function() {
     return "innerHTML"
 };
 
 function Ja(t, e) {
-    t[eO()] = e
+    t[nO()] = e
 }
 
 function Af(t) {
     var e = ni();
     return t === !0 ? e.className = Xm : (e.className = Qm, ul(t) ? e.appendChild(t) : Ja(e, t)), e
 }
 
 function Nf(t, e) {
     ul(e.content) ? (Ja(t, ""), t.appendChild(e.content)) : typeof e.content != "function" && (e.allowHTML ? Ja(t, e.content) : t.textContent = e.content)
 }
 
 function Ga(t) {
     var e = t.firstElementChild,
-        n = wo(e.children);
+        n = _o(e.children);
     return {
         box: e,
         content: n.find(function(r) {
             return r.classList.contains(Ym)
         }),
         arrow: n.find(function(r) {
             return r.classList.contains(Xm) || r.classList.contains(Qm)
         }),
         backdrop: n.find(function(r) {
-            return r.classList.contains(IT)
+            return r.classList.contains($T)
         })
     }
 }
 
 function rg(t) {
     var e = ni(),
         n = ni();
-    n.className = DT, n.setAttribute("data-state", "hidden"), n.setAttribute("tabindex", "-1");
+    n.className = PT, n.setAttribute("data-state", "hidden"), n.setAttribute("tabindex", "-1");
     var r = ni();
     r.className = Ym, r.setAttribute("data-state", "hidden"), Nf(r, t.props), e.appendChild(n), n.appendChild(r), s(t.props, t.props);
 
     function s(i, o) {
         var l = Ga(e),
             a = l.box,
             c = l.content,
@@ -19664,29 +19667,29 @@
     }
     return {
         popper: e,
         onUpdate: s
     }
 }
 rg.$$tippy = !0;
-var tO = 1,
-    Bi = [],
+var rO = 1,
+    zi = [],
     na = [];
 
-function nO(t, e) {
+function sO(t, e) {
     var n = Mf(t, Object.assign({}, Zt, ng(Cf(e)))),
         r, s, i, o = !1,
         l = !1,
         a = !1,
         c = !1,
         u, d, f, h = [],
         p = Sf(_, n.interactiveDebounce),
-        g, v = tO++,
+        g, v = rO++,
         x = null,
-        w = $T(n.plugins),
+        w = FT(n.plugins),
         S = {
             isEnabled: !0,
             isVisible: !1,
             isDestroyed: !1,
             isMounted: !1,
             isShown: !1
         },
@@ -19697,32 +19700,32 @@
             popperInstance: x,
             props: n,
             state: S,
             plugins: w,
             clearDelayTimeouts: pe,
             setProps: Ne,
             setContent: we,
-            show: ze,
+            show: Ve,
             hide: At,
             hideWithInteractivity: Pn,
             enable: Z,
             disable: oe,
-            unmount: Ci,
+            unmount: Ti,
             destroy: dr
         };
     if (!n.render) return y;
     var I = n.render(y),
         T = I.popper,
         V = I.onUpdate;
     T.setAttribute("data-tippy-root", ""), T.id = "tippy-" + y.id, y.popper = T, t._tippy = y, T._tippy = y;
     var N = w.map(function(E) {
             return E.fn(y)
         }),
         G = t.hasAttribute("aria-expanded");
-    return ue(), Ze(), fe(), ae("onCreate", [y]), n.showOnCreate && Q(), T.addEventListener("mouseenter", function() {
+    return ue(), Ze(), he(), ae("onCreate", [y]), n.showOnCreate && Q(), T.addEventListener("mouseenter", function() {
         y.props.interactive && y.state.isVisible && y.clearDelayTimeouts()
     }), T.addEventListener("mouseleave", function() {
         y.props.interactive && y.props.trigger.indexOf("mouseenter") >= 0 && Ae().addEventListener("mousemove", p)
     }), y;
 
     function J() {
         var E = y.props.touch;
@@ -19740,39 +19743,39 @@
 
     function ie() {
         return g || t
     }
 
     function Ae() {
         var E = ie().parentNode;
-        return E ? VT(E) : document
+        return E ? UT(E) : document
     }
 
-    function Be() {
+    function He() {
         return Ga(T)
     }
 
     function ge(E) {
         return y.state.isMounted && !y.state.isVisible || cn.isTouch || u && u.type === "focus" ? 0 : Zl(y.props.delay, E ? 0 : 1, Zt.delay)
     }
 
-    function fe(E) {
+    function he(E) {
         E === void 0 && (E = !1), T.style.pointerEvents = y.props.interactive && !E ? "" : "none", T.style.zIndex = "" + y.props.zIndex
     }
 
     function ae(E, W, ee) {
         if (ee === void 0 && (ee = !0), N.forEach(function(Se) {
                 Se[E] && Se[E].apply(Se, W)
             }), ee) {
             var Te;
             (Te = y.props)[E].apply(Te, W)
         }
     }
 
-    function He() {
+    function ze() {
         var E = y.props.aria;
         if (E.content) {
             var W = "aria-" + E.content,
                 ee = T.id,
                 Te = qr(y.props.triggerTarget || t);
             Te.forEach(function(Se) {
                 var mt = Se.getAttribute(W);
@@ -19791,15 +19794,15 @@
             E.forEach(function(W) {
                 y.props.interactive ? W.setAttribute("aria-expanded", y.state.isVisible && W === ie() ? "true" : "false") : W.removeAttribute("aria-expanded")
             })
         }
     }
 
     function Ke() {
-        Ae().removeEventListener("mousemove", p), Bi = Bi.filter(function(E) {
+        Ae().removeEventListener("mousemove", p), zi = zi.filter(function(E) {
             return E !== p
         })
     }
 
     function Pe(E) {
         if (!(cn.isTouch && (a || E.type === "mousedown"))) {
             var W = E.composedPath && E.composedPath()[0] || E.target;
@@ -19841,15 +19844,15 @@
     }
 
     function Y(E, W) {
         ye(E, W)
     }
 
     function ye(E, W) {
-        var ee = Be().box;
+        var ee = He().box;
 
         function Te(Se) {
             Se.target === ee && (ta(ee, "remove", Te), W())
         }
         if (E === 0) return W();
         ta(ee, "remove", d), ta(ee, "add", Te), d = Te
     }
@@ -19868,21 +19871,21 @@
     }
 
     function ue() {
         ne() && (Ee("touchstart", k, {
             passive: !0
         }), Ee("touchend", O, {
             passive: !0
-        })), PT(y.props.trigger).forEach(function(E) {
+        })), LT(y.props.trigger).forEach(function(E) {
             if (E !== "manual") switch (Ee(E, k), E) {
                 case "mouseenter":
                     Ee("mouseleave", O);
                     break;
                 case "focus":
-                    Ee(JT ? "focusout" : "blur", D);
+                    Ee(YT ? "focusout" : "blur", D);
                     break;
                 case "focusin":
                     Ee("focusout", D);
                     break
             }
         })
     }
@@ -19897,15 +19900,15 @@
         }), h = []
     }
 
     function k(E) {
         var W, ee = !1;
         if (!(!y.state.isEnabled || F(E) || l)) {
             var Te = ((W = u) == null ? void 0 : W.type) === "focus";
-            u = E, g = E.currentTarget, Ze(), !y.state.isVisible && BT(E) && Bi.forEach(function(Se) {
+            u = E, g = E.currentTarget, Ze(), !y.state.isVisible && zT(E) && zi.forEach(function(Se) {
                 return Se(E)
             }), E.type === "click" && (y.props.trigger.indexOf("mouseenter") < 0 || o) && y.props.hideOnClick !== !1 && y.state.isVisible ? ee = !0 : Q(E), E.type === "click" && (o = !ee), ee && !Te && K(E)
         }
     }
 
     function _(E) {
         var W = E.target,
@@ -19916,15 +19919,15 @@
                     Br = (mt = Pt.popperInstance) == null ? void 0 : mt.state;
                 return Br ? {
                     popperRect: Se.getBoundingClientRect(),
                     popperState: Br,
                     props: n
                 } : null
             }).filter(Boolean);
-            jT(Te, E) && (Ke(), K(E))
+            WT(Te, E) && (Ke(), K(E))
         }
     }
 
     function O(E) {
         var W = F(E) || y.props.trigger.indexOf("click") >= 0 && o;
         if (!W) {
             if (y.props.interactive) {
@@ -19957,21 +19960,21 @@
                 contextElement: Se.contextElement || ie()
             } : t,
             eu = {
                 name: "$$tippy",
                 enabled: !0,
                 phase: "beforeWrite",
                 requires: ["computeStyles"],
-                fn: function(Ei) {
-                    var Hr = Ei.state;
+                fn: function(Oi) {
+                    var Hr = Oi.state;
                     if (H()) {
-                        var mg = Be(),
-                            hl = mg.box;
-                        ["placement", "reference-hidden", "escaped"].forEach(function(Ti) {
-                            Ti === "placement" ? hl.setAttribute("data-placement", Hr.placement) : Hr.attributes.popper["data-popper-" + Ti] ? hl.setAttribute("data-" + Ti, "") : hl.removeAttribute("data-" + Ti)
+                        var gg = He(),
+                            hl = gg.box;
+                        ["placement", "reference-hidden", "escaped"].forEach(function(Mi) {
+                            Mi === "placement" ? hl.setAttribute("data-placement", Hr.placement) : Hr.attributes.popper["data-popper-" + Mi] ? hl.setAttribute("data-" + Mi, "") : hl.removeAttribute("data-" + Mi)
                         }), Hr.attributes.popper = {}
                     }
                 }
             },
             fr = [{
                 name: "offset",
                 options: {
@@ -20000,15 +20003,15 @@
             }, eu];
         H() && Pt && fr.push({
             name: "arrow",
             options: {
                 element: Pt,
                 padding: 3
             }
-        }), fr.push.apply(fr, (W == null ? void 0 : W.modifiers) || []), y.popperInstance = RT(Br, T, Object.assign({}, W, {
+        }), fr.push.apply(fr, (W == null ? void 0 : W.modifiers) || []), y.popperInstance = IT(Br, T, Object.assign({}, W, {
             placement: ee,
             onFirstUpdate: f,
             modifiers: fr
         }))
     }
 
     function L() {
@@ -20018,15 +20021,15 @@
     function B() {
         var E = y.props.appendTo,
             W, ee = ie();
         y.props.interactive && E === Zm || E === "parent" ? W = ee.parentNode : W = eg(E, [ee]), W.contains(T) || W.appendChild(T), y.state.isMounted = !0, U()
     }
 
     function P() {
-        return wo(T.querySelectorAll("[data-tippy-root]"))
+        return _o(T.querySelectorAll("[data-tippy-root]"))
     }
 
     function Q(E) {
         y.clearDelayTimeouts(), E && ae("onTrigger", [y, E]), M();
         var W = ge(!0),
             ee = J(),
             Te = ee[0],
@@ -20068,77 +20071,77 @@
             ae("onBeforeUpdate", [y, E]), b();
             var W = y.props,
                 ee = Mf(t, Object.assign({}, W, Cf(E), {
                     ignoreAttributes: !0
                 }));
             y.props = ee, ue(), W.interactiveDebounce !== ee.interactiveDebounce && (Ke(), p = Sf(_, ee.interactiveDebounce)), W.triggerTarget && !ee.triggerTarget ? qr(W.triggerTarget).forEach(function(Te) {
                 Te.removeAttribute("aria-expanded")
-            }) : ee.triggerTarget && t.removeAttribute("aria-expanded"), Ze(), fe(), V && V(W, ee), y.popperInstance && (U(), P().forEach(function(Te) {
+            }) : ee.triggerTarget && t.removeAttribute("aria-expanded"), Ze(), he(), V && V(W, ee), y.popperInstance && (U(), P().forEach(function(Te) {
                 requestAnimationFrame(Te._tippy.popperInstance.forceUpdate)
             })), ae("onAfterUpdate", [y, E])
         }
     }
 
     function we(E) {
         y.setProps({
             content: E
         })
     }
 
-    function ze() {
+    function Ve() {
         var E = y.state.isVisible,
             W = y.state.isDestroyed,
             ee = !y.state.isEnabled,
             Te = cn.isTouch && !y.props.touch,
             Se = Zl(y.props.duration, 0, Zt.duration);
         if (!(E || W || ee || Te) && !ie().hasAttribute("disabled") && (ae("onShow", [y], !1), y.props.onShow(y) !== !1)) {
-            if (y.state.isVisible = !0, H() && (T.style.visibility = "visible"), fe(), M(), y.state.isMounted || (T.style.transition = "none"), H()) {
-                var mt = Be(),
+            if (y.state.isVisible = !0, H() && (T.style.visibility = "visible"), he(), M(), y.state.isMounted || (T.style.transition = "none"), H()) {
+                var mt = He(),
                     Pt = mt.box,
                     Br = mt.content;
                 ea([Pt, Br], 0)
             }
             f = function() {
                 var fr;
                 if (!(!y.state.isVisible || c)) {
                     if (c = !0, T.offsetHeight, T.style.transition = y.props.moveTransition, H() && y.props.animation) {
-                        var fl = Be(),
-                            Ei = fl.box,
+                        var fl = He(),
+                            Oi = fl.box,
                             Hr = fl.content;
-                        ea([Ei, Hr], Se), Ef([Ei, Hr], "visible")
+                        ea([Oi, Hr], Se), Ef([Oi, Hr], "visible")
                     }
-                    He(), Ze(), _f(na, y), (fr = y.popperInstance) == null || fr.forceUpdate(), ae("onMount", [y]), y.props.animation && H() && Y(Se, function() {
+                    ze(), Ze(), _f(na, y), (fr = y.popperInstance) == null || fr.forceUpdate(), ae("onMount", [y]), y.props.animation && H() && Y(Se, function() {
                         y.state.isShown = !0, ae("onShown", [y])
                     })
                 }
             }, B()
         }
     }
 
     function At() {
         var E = !y.state.isVisible,
             W = y.state.isDestroyed,
             ee = !y.state.isEnabled,
             Te = Zl(y.props.duration, 1, Zt.duration);
         if (!(E || W || ee) && (ae("onHide", [y], !1), y.props.onHide(y) !== !1)) {
-            if (y.state.isVisible = !1, y.state.isShown = !1, c = !1, o = !1, H() && (T.style.visibility = "hidden"), Ke(), j(), fe(!0), H()) {
-                var Se = Be(),
+            if (y.state.isVisible = !1, y.state.isShown = !1, c = !1, o = !1, H() && (T.style.visibility = "hidden"), Ke(), j(), he(!0), H()) {
+                var Se = He(),
                     mt = Se.box,
                     Pt = Se.content;
                 y.props.animation && (ea([mt, Pt], Te), Ef([mt, Pt], "hidden"))
             }
-            He(), Ze(), y.props.animation ? H() && z(Te, y.unmount) : y.unmount()
+            ze(), Ze(), y.props.animation ? H() && z(Te, y.unmount) : y.unmount()
         }
     }
 
     function Pn(E) {
-        Ae().addEventListener("mousemove", p), _f(Bi, p), p(E)
+        Ae().addEventListener("mousemove", p), _f(zi, p), p(E)
     }
 
-    function Ci() {
+    function Ti() {
         y.state.isVisible && y.hide(), y.state.isMounted && (L(), P().forEach(function(E) {
             E._tippy.unmount()
         }), T.parentNode && T.parentNode.removeChild(T), na = na.filter(function(E) {
             return E !== y
         }), y.state.isMounted = !1, ae("onHidden", [y]))
     }
 
@@ -20146,27 +20149,27 @@
         y.state.isDestroyed || (y.clearDelayTimeouts(), y.unmount(), b(), delete t._tippy, y.state.isDestroyed = !0, ae("onDestroy", [y]))
     }
 }
 
 function As(t, e) {
     e === void 0 && (e = {});
     var n = Zt.plugins.concat(e.plugins || []);
-    qT();
+    JT();
     var r = Object.assign({}, e, {
             plugins: n
         }),
-        s = zT(t),
+        s = jT(t),
         i = s.reduce(function(o, l) {
-            var a = l && nO(l, r);
+            var a = l && sO(l, r);
             return a && o.push(a), o
         }, []);
     return ul(t) ? i[0] : i
 }
 As.defaultProps = Zt;
-As.setDefaultProps = QT;
+As.setDefaultProps = eO;
 As.currentInput = cn;
 Object.assign({}, Vm, {
     effect: function(e) {
         var n = e.state,
             r = {
                 popper: {
                     position: n.options.strategy,
@@ -20181,15 +20184,15 @@
             };
         Object.assign(n.elements.popper.style, r.popper), n.styles = r, n.elements.arrow && Object.assign(n.elements.arrow.style, r.arrow)
     }
 });
 As.setDefaultProps({
     render: rg
 });
-class rO {
+class iO {
     constructor({
         editor: e,
         element: n,
         view: r,
         tippyOptions: s = {},
         updateDelay: i = 250,
         shouldShow: o
@@ -20253,15 +20256,15 @@
                     from: S,
                     to: y
                 }))) {
                 this.hide();
                 return
             }(f = this.tippy) === null || f === void 0 || f.setProps({
                 getReferenceClientRect: ((h = this.tippyOptions) === null || h === void 0 ? void 0 : h.getReferenceClientRect) || (() => {
-                    if (XC(p.selection)) {
+                    if (ZC(p.selection)) {
                         let T = l.nodeDOM(S);
                         const V = T.dataset.nodeViewWrapper ? T : T.querySelector("[data-node-view-wrapper]");
                         if (V && (T = V.firstChild), T) return T.getBoundingClientRect()
                     }
                     return Bm(l, S, y)
                 })
             }), this.show()
@@ -20309,15 +20312,15 @@
         !((e = this.tippy) === null || e === void 0) && e.popper.firstChild && this.tippy.popper.firstChild.removeEventListener("blur", this.tippyBlurHandler), (n = this.tippy) === null || n === void 0 || n.destroy(), this.element.removeEventListener("mousedown", this.mousedownHandler, {
             capture: !0
         }), this.view.dom.removeEventListener("dragstart", this.dragstartHandler), this.editor.off("focus", this.focusHandler), this.editor.off("blur", this.blurHandler)
     }
 }
 const sg = t => new Mt({
     key: typeof t.pluginKey == "string" ? new Sn(t.pluginKey) : t.pluginKey,
-    view: e => new rO({
+    view: e => new iO({
         view: e,
         ...t
     })
 });
 kt.create({
     name: "bubbleMenu",
     addOptions() {
@@ -20336,15 +20339,15 @@
             element: this.options.element,
             tippyOptions: this.options.tippyOptions,
             updateDelay: this.options.updateDelay,
             shouldShow: this.options.shouldShow
         })] : []
     }
 });
-class sO {
+class oO {
     constructor({
         editor: e,
         element: n,
         view: r,
         tippyOptions: s = {},
         shouldShow: i
     }) {
@@ -20432,15 +20435,15 @@
         !((e = this.tippy) === null || e === void 0) && e.popper.firstChild && this.tippy.popper.firstChild.removeEventListener("blur", this.tippyBlurHandler), (n = this.tippy) === null || n === void 0 || n.destroy(), this.element.removeEventListener("mousedown", this.mousedownHandler, {
             capture: !0
         }), this.editor.off("focus", this.focusHandler), this.editor.off("blur", this.blurHandler)
     }
 }
 const ig = t => new Mt({
     key: typeof t.pluginKey == "string" ? new Sn(t.pluginKey) : t.pluginKey,
-    view: e => new sO({
+    view: e => new oO({
         view: e,
         ...t
     })
 });
 kt.create({
     name: "floatingMenu",
     addOptions() {
@@ -20484,15 +20487,15 @@
             type: Function,
             default: null
         }
     },
     setup(t, {
         slots: e
     }) {
-        const n = No(null);
+        const n = Do(null);
         return Ts(() => {
             const {
                 updateDelay: r,
                 editor: s,
                 pluginKey: i,
                 shouldShow: o,
                 tippyOptions: l
@@ -20517,28 +20520,28 @@
                 ref: n
             }, (r = e.default) === null || r === void 0 ? void 0 : r.call(e))
         }
     }
 });
 
 function Rf(t) {
-    return dy((e, n) => ({
+    return fy((e, n) => ({
         get() {
             return e(), t
         },
         set(r) {
             t = r, requestAnimationFrame(() => {
                 requestAnimationFrame(() => {
                     n()
                 })
             })
         }
     }))
 }
-class iO extends EE {
+class lO extends OE {
     constructor(e = {}) {
         return super(e), this.vueRenderers = Es(new Map), this.contentComponent = null, this.reactiveState = Rf(this.view.state), this.reactiveExtensionStorage = Rf(this.extensionStorage), this.on("transaction", () => {
             this.reactiveState.value = this.view.state, this.reactiveExtensionStorage.value = this.extensionStorage
         }), oc(this)
     }
     get state() {
         return this.reactiveState ? this.reactiveState.value : this.view.state
@@ -20549,26 +20552,26 @@
     registerPlugin(e, n) {
         super.registerPlugin(e, n), this.reactiveState.value = this.view.state
     }
     unregisterPlugin(e) {
         super.unregisterPlugin(e), this.reactiveState.value = this.view.state
     }
 }
-const oO = ir({
+const aO = ir({
     name: "EditorContent",
     props: {
         editor: {
             default: null,
             type: Object
         }
     },
     setup(t) {
-        const e = No(),
+        const e = Do(),
             n = bc();
-        return Cy(() => {
+        return Ey(() => {
             const r = t.editor;
             r && r.options.element && e.value && dc(() => {
                 if (!e.value || !r.options.element.firstChild) return;
                 const s = de(e.value);
                 e.value.append(...r.options.element.childNodes), r.contentComponent = n.ctx._, r.setOptions({
                     element: s
                 }), r.createNodeViews()
@@ -20585,15 +20588,15 @@
         }), {
             rootEl: e
         }
     },
     render() {
         const t = [];
         return this.editor && this.editor.vueRenderers.forEach(e => {
-            const n = mn(lb, {
+            const n = mn(ab, {
                 to: e.teleportElement,
                 key: e.id
             }, mn(e.component, {
                 ref: e.id,
                 ...e.props
             }));
             t.push(n)
@@ -20623,15 +20626,15 @@
             type: Function,
             default: null
         }
     },
     setup(t, {
         slots: e
     }) {
-        const n = No(null);
+        const n = Do(null);
         return Ts(() => {
             const {
                 pluginKey: r,
                 editor: s,
                 tippyOptions: i,
                 shouldShow: o
             } = t;
@@ -20688,25 +20691,25 @@
                 whiteSpace: "normal"
             },
             "data-node-view-wrapper": "",
             onDragstart: this.onDragStart
         }, (e = (t = this.$slots).default) === null || e === void 0 ? void 0 : e.call(t))
     }
 });
-const lO = (t = {}) => {
+const cO = (t = {}) => {
         const e = sh();
         return Ts(() => {
-            e.value = new iO(t)
+            e.value = new lO(t)
         }), or(() => {
             var n;
             (n = e.value) === null || n === void 0 || n.destroy()
         }), e
     },
-    aO = /^\s*>\s$/,
-    cO = pt.create({
+    uO = /^\s*>\s$/,
+    dO = pt.create({
         name: "blockquote",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         content: "block+",
@@ -20738,24 +20741,24 @@
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-b": () => this.editor.commands.toggleBlockquote()
             }
         },
         addInputRules() {
             return [yi({
-                find: aO,
+                find: uO,
                 type: this.type
             })]
         }
     }),
-    uO = /(?:^|\s)((?:\*\*)((?:[^*]+))(?:\*\*))$/,
-    dO = /(?:^|\s)((?:\*\*)((?:[^*]+))(?:\*\*))/g,
-    fO = /(?:^|\s)((?:__)((?:[^__]+))(?:__))$/,
-    hO = /(?:^|\s)((?:__)((?:[^__]+))(?:__))/g,
-    pO = xn.create({
+    fO = /(?:^|\s)((?:\*\*)((?:[^*]+))(?:\*\*))$/,
+    hO = /(?:^|\s)((?:\*\*)((?:[^*]+))(?:\*\*))/g,
+    pO = /(?:^|\s)((?:__)((?:[^__]+))(?:__))$/,
+    mO = /(?:^|\s)((?:__)((?:[^__]+))(?:__))/g,
+    gO = xn.create({
         name: "bold",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -20791,32 +20794,32 @@
             return {
                 "Mod-b": () => this.editor.commands.toggleBold(),
                 "Mod-B": () => this.editor.commands.toggleBold()
             }
         },
         addInputRules() {
             return [gs({
-                find: uO,
+                find: fO,
                 type: this.type
             }), gs({
-                find: fO,
+                find: pO,
                 type: this.type
             })]
         },
         addPasteRules() {
             return [ys({
-                find: dO,
+                find: hO,
                 type: this.type
             }), ys({
-                find: hO,
+                find: mO,
                 type: this.type
             })]
         }
     }),
-    mO = pt.create({
+    yO = pt.create({
         name: "listItem",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         content: "paragraph block*",
@@ -20866,15 +20869,15 @@
                     const n = al(t, this.type);
                     return Object.entries(n).some(([, s]) => !!s) ? !0 : e.unsetMark(this.name)
                 }
             }
         }
     }),
     If = /^\s*([-+*])\s$/,
-    gO = pt.create({
+    bO = pt.create({
         name: "bulletList",
         addOptions() {
             return {
                 itemTypeName: "listItem",
                 HTMLAttributes: {},
                 keepMarks: !1,
                 keepAttributes: !1
@@ -20895,15 +20898,15 @@
             return ["ul", Qe(this.options.HTMLAttributes, t), 0]
         },
         addCommands() {
             return {
                 toggleBulletList: () => ({
                     commands: t,
                     chain: e
-                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(mO.name, this.editor.getAttributes(Df.name)).run() : t.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
+                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(yO.name, this.editor.getAttributes(Df.name)).run() : t.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
             }
         },
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-8": () => this.editor.commands.toggleBulletList()
             }
         },
@@ -20918,17 +20921,17 @@
                 keepMarks: this.options.keepMarks,
                 keepAttributes: this.options.keepAttributes,
                 getAttributes: () => this.editor.getAttributes(Df.name),
                 editor: this.editor
             })), [t]
         }
     }),
-    yO = /(?:^|\s)((?:`)((?:[^`]+))(?:`))$/,
-    bO = /(?:^|\s)((?:`)((?:[^`]+))(?:`))/g,
-    vO = xn.create({
+    vO = /(?:^|\s)((?:`)((?:[^`]+))(?:`))$/,
+    xO = /(?:^|\s)((?:`)((?:[^`]+))(?:`))/g,
+    kO = xn.create({
         name: "code",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         excludes: "_",
@@ -20960,28 +20963,28 @@
         addKeyboardShortcuts() {
             return {
                 "Mod-e": () => this.editor.commands.toggleCode()
             }
         },
         addInputRules() {
             return [gs({
-                find: yO,
+                find: vO,
                 type: this.type
             })]
         },
         addPasteRules() {
             return [ys({
-                find: bO,
+                find: xO,
                 type: this.type
             })]
         }
     }),
-    xO = /^```([a-z]+)?[\s\n]$/,
-    kO = /^~~~([a-z]+)?[\s\n]$/,
-    wO = pt.create({
+    wO = /^```([a-z]+)?[\s\n]$/,
+    SO = /^~~~([a-z]+)?[\s\n]$/,
+    _O = pt.create({
         name: "codeBlock",
         addOptions() {
             return {
                 languageClassPrefix: "language-",
                 exitOnTripleEnter: !0,
                 exitOnArrowDown: !0,
                 HTMLAttributes: {}
@@ -21079,21 +21082,21 @@
                     const l = s.after();
                     return l === void 0 || r.nodeAt(l) ? !1 : t.commands.exitCode()
                 }
             }
         },
         addInputRules() {
             return [Wa({
-                find: xO,
+                find: wO,
                 type: this.type,
                 getAttributes: t => ({
                     language: t[1]
                 })
             }), Wa({
-                find: kO,
+                find: SO,
                 type: this.type,
                 getAttributes: t => ({
                     language: t[1]
                 })
             })]
         },
         addProseMirrorPlugins() {
@@ -21115,28 +21118,28 @@
                         })), o.setSelection(xe.near(o.doc.resolve(Math.max(0, o.selection.from - 2)))), o.insertText(n.replace(/\r\n?/g, `
 `)), o.setMeta("paste", !0), t.dispatch(o), !0
                     }
                 }
             })]
         }
     }),
-    SO = pt.create({
+    CO = pt.create({
         name: "doc",
         topNode: !0,
         content: "block+"
     });
 
-function _O(t = {}) {
+function EO(t = {}) {
     return new Mt({
         view(e) {
-            return new CO(e, t)
+            return new TO(e, t)
         }
     })
 }
-class CO {
+class TO {
     constructor(e, n) {
         var r;
         this.editorView = e, this.cursorPos = null, this.element = null, this.timeout = -1, this.width = (r = n.width) !== null && r !== void 0 ? r : 1, this.color = n.color === !1 ? void 0 : n.color || "black", this.class = n.class, this.handlers = ["dragover", "dragend", "drop", "dragleave"].map(s => {
             let i = o => {
                 this[s](o)
             };
             return e.dom.addEventListener(s, i), {
@@ -21224,111 +21227,111 @@
     drop() {
         this.scheduleRemoval(20)
     }
     dragleave(e) {
         (e.target == this.editorView.dom || !this.editorView.dom.contains(e.relatedTarget)) && this.setCursor(null)
     }
 }
-const EO = kt.create({
+const OO = kt.create({
     name: "dropCursor",
     addOptions() {
         return {
             color: "currentColor",
             width: 1,
             class: void 0
         }
     },
     addProseMirrorPlugins() {
-        return [_O(this.options)]
+        return [EO(this.options)]
     }
 });
-class Ve extends ve {
+class je extends ve {
     constructor(e) {
         super(e, e)
     }
     map(e, n) {
         let r = e.resolve(n.map(this.head));
-        return Ve.valid(r) ? new Ve(r) : ve.near(r)
+        return je.valid(r) ? new je(r) : ve.near(r)
     }
     content() {
         return q.empty
     }
     eq(e) {
-        return e instanceof Ve && e.head == this.head
+        return e instanceof je && e.head == this.head
     }
     toJSON() {
         return {
             type: "gapcursor",
             pos: this.head
         }
     }
     static fromJSON(e, n) {
         if (typeof n.pos != "number") throw new RangeError("Invalid input for GapCursor.fromJSON");
-        return new Ve(e.resolve(n.pos))
+        return new je(e.resolve(n.pos))
     }
     getBookmark() {
         return new Zc(this.anchor)
     }
     static valid(e) {
         let n = e.parent;
-        if (n.isTextblock || !TO(e) || !OO(e)) return !1;
+        if (n.isTextblock || !MO(e) || !AO(e)) return !1;
         let r = n.type.spec.allowGapCursor;
         if (r != null) return r;
         let s = n.contentMatchAt(e.index()).defaultType;
         return s && s.isTextblock
     }
     static findGapCursorFrom(e, n, r = !1) {
         e: for (;;) {
-            if (!r && Ve.valid(e)) return e;
+            if (!r && je.valid(e)) return e;
             let s = e.pos,
                 i = null;
             for (let o = e.depth;; o--) {
                 let l = e.node(o);
                 if (n > 0 ? e.indexAfter(o) < l.childCount : e.index(o) > 0) {
                     i = l.child(n > 0 ? e.indexAfter(o) : e.index(o) - 1);
                     break
                 } else if (o == 0) return null;
                 s += n;
                 let a = e.doc.resolve(s);
-                if (Ve.valid(a)) return a
+                if (je.valid(a)) return a
             }
             for (;;) {
                 let o = n > 0 ? i.firstChild : i.lastChild;
                 if (!o) {
                     if (i.isAtom && !i.isText && !se.isSelectable(i)) {
                         e = e.doc.resolve(s + i.nodeSize * n), r = !1;
                         continue e
                     }
                     break
                 }
                 i = o, s += n;
                 let l = e.doc.resolve(s);
-                if (Ve.valid(l)) return l
+                if (je.valid(l)) return l
             }
             return null
         }
     }
 }
-Ve.prototype.visible = !1;
-Ve.findFrom = Ve.findGapCursorFrom;
-ve.jsonID("gapcursor", Ve);
+je.prototype.visible = !1;
+je.findFrom = je.findGapCursorFrom;
+ve.jsonID("gapcursor", je);
 class Zc {
     constructor(e) {
         this.pos = e
     }
     map(e) {
         return new Zc(e.map(this.pos))
     }
     resolve(e) {
         let n = e.resolve(this.pos);
-        return Ve.valid(n) ? new Ve(n) : ve.near(n)
+        return je.valid(n) ? new je(n) : ve.near(n)
     }
 }
 
-function TO(t) {
+function MO(t) {
     for (let e = t.depth; e >= 0; e--) {
         let n = t.index(e),
             r = t.node(e);
         if (n == 0) {
             if (r.type.spec.isolating) return !0;
             continue
         }
@@ -21336,15 +21339,15 @@
             if (s.childCount == 0 && !s.inlineContent || s.isAtom || s.type.spec.isolating) return !0;
             if (s.inlineContent) return !1
         }
     }
     return !0
 }
 
-function OO(t) {
+function AO(t) {
     for (let e = t.depth; e >= 0; e--) {
         let n = t.indexAfter(e),
             r = t.node(e);
         if (n == r.childCount) {
             if (r.type.spec.isolating) return !0;
             continue
         }
@@ -21352,99 +21355,99 @@
             if (s.childCount == 0 && !s.inlineContent || s.isAtom || s.type.spec.isolating) return !0;
             if (s.inlineContent) return !1
         }
     }
     return !0
 }
 
-function MO() {
+function NO() {
     return new Mt({
         props: {
-            decorations: DO,
+            decorations: PO,
             createSelectionBetween(t, e, n) {
-                return e.pos == n.pos && Ve.valid(n) ? new Ve(n) : null
+                return e.pos == n.pos && je.valid(n) ? new je(n) : null
             },
-            handleClick: NO,
-            handleKeyDown: AO,
+            handleClick: DO,
+            handleKeyDown: RO,
             handleDOMEvents: {
-                beforeinput: RO
+                beforeinput: IO
             }
         }
     })
 }
-const AO = Cm({
-    ArrowLeft: Hi("horiz", -1),
-    ArrowRight: Hi("horiz", 1),
-    ArrowUp: Hi("vert", -1),
-    ArrowDown: Hi("vert", 1)
+const RO = Cm({
+    ArrowLeft: Vi("horiz", -1),
+    ArrowRight: Vi("horiz", 1),
+    ArrowUp: Vi("vert", -1),
+    ArrowDown: Vi("vert", 1)
 });
 
-function Hi(t, e) {
+function Vi(t, e) {
     const n = t == "vert" ? e > 0 ? "down" : "up" : e > 0 ? "right" : "left";
     return function(r, s, i) {
         let o = r.selection,
             l = e > 0 ? o.$to : o.$from,
             a = o.empty;
         if (o instanceof xe) {
             if (!i.endOfTextblock(n) || l.depth == 0) return !1;
             a = !1, l = r.doc.resolve(e > 0 ? l.after() : l.before())
         }
-        let c = Ve.findGapCursorFrom(l, e, a);
-        return c ? (s && s(r.tr.setSelection(new Ve(c))), !0) : !1
+        let c = je.findGapCursorFrom(l, e, a);
+        return c ? (s && s(r.tr.setSelection(new je(c))), !0) : !1
     }
 }
 
-function NO(t, e, n) {
+function DO(t, e, n) {
     if (!t || !t.editable) return !1;
     let r = t.state.doc.resolve(e);
-    if (!Ve.valid(r)) return !1;
+    if (!je.valid(r)) return !1;
     let s = t.posAtCoords({
         left: n.clientX,
         top: n.clientY
     });
-    return s && s.inside > -1 && se.isSelectable(t.state.doc.nodeAt(s.inside)) ? !1 : (t.dispatch(t.state.tr.setSelection(new Ve(r))), !0)
+    return s && s.inside > -1 && se.isSelectable(t.state.doc.nodeAt(s.inside)) ? !1 : (t.dispatch(t.state.tr.setSelection(new je(r))), !0)
 }
 
-function RO(t, e) {
-    if (e.inputType != "insertCompositionText" || !(t.state.selection instanceof Ve)) return !1;
+function IO(t, e) {
+    if (e.inputType != "insertCompositionText" || !(t.state.selection instanceof je)) return !1;
     let {
         $from: n
     } = t.state.selection, r = n.parent.contentMatchAt(n.index()).findWrapping(t.state.schema.nodes.text);
     if (!r) return !1;
     let s = $.empty;
     for (let o = r.length - 1; o >= 0; o--) s = $.from(r[o].createAndFill(null, s));
     let i = t.state.tr.replace(n.pos, n.pos, new q(s, 0, 0));
     return i.setSelection(xe.near(i.doc.resolve(n.pos + 1))), t.dispatch(i), !1
 }
 
-function DO(t) {
-    if (!(t.selection instanceof Ve)) return null;
+function PO(t) {
+    if (!(t.selection instanceof je)) return null;
     let e = document.createElement("div");
     return e.className = "ProseMirror-gapcursor", Je.create(t.doc, [zt.widget(t.selection.head, e, {
         key: "gapcursor"
     })])
 }
-const IO = kt.create({
+const $O = kt.create({
         name: "gapCursor",
         addProseMirrorPlugins() {
-            return [MO()]
+            return [NO()]
         },
         extendNodeSchema(t) {
             var e;
             const n = {
                 name: t.name,
                 options: t.options,
                 storage: t.storage
             };
             return {
                 allowGapCursor: (e = be(X(t, "allowGapCursor", n))) !== null && e !== void 0 ? e : null
             }
         }
     }),
-    PO = pt.create({
+    LO = pt.create({
         name: "hardBreak",
         addOptions() {
             return {
                 keepMarks: !0,
                 HTMLAttributes: {}
             }
         },
@@ -21501,15 +21504,15 @@
         addKeyboardShortcuts() {
             return {
                 "Mod-Enter": () => this.editor.commands.setHardBreak(),
                 "Shift-Enter": () => this.editor.commands.setHardBreak()
             }
         }
     }),
-    $O = pt.create({
+    FO = pt.create({
         name: "heading",
         addOptions() {
             return {
                 levels: [1, 2, 3, 4, 5, 6],
                 HTMLAttributes: {}
             }
         },
@@ -21562,24 +21565,24 @@
                 type: this.type,
                 getAttributes: {
                     level: t
                 }
             }))
         }
     });
-var So = 200,
+var Co = 200,
     ot = function() {};
 ot.prototype.append = function(e) {
-    return e.length ? (e = ot.from(e), !this.length && e || e.length < So && this.leafAppend(e) || this.length < So && e.leafPrepend(this) || this.appendInner(e)) : this
+    return e.length ? (e = ot.from(e), !this.length && e || e.length < Co && this.leafAppend(e) || this.length < Co && e.leafPrepend(this) || this.appendInner(e)) : this
 };
 ot.prototype.prepend = function(e) {
     return e.length ? ot.from(e).append(this) : this
 };
 ot.prototype.appendInner = function(e) {
-    return new LO(this, e)
+    return new BO(this, e)
 };
 ot.prototype.slice = function(e, n) {
     return e === void 0 && (e = 0), n === void 0 && (n = this.length), e >= n ? ot.empty : this.sliceInner(Math.max(0, e), Math.min(this.length, n))
 };
 ot.prototype.get = function(e) {
     if (!(e < 0 || e >= this.length)) return this.getInner(e)
 };
@@ -21618,25 +21621,25 @@
     }, e.prototype.forEachInner = function(s, i, o, l) {
         for (var a = i; a < o; a++)
             if (s(this.values[a], l + a) === !1) return !1
     }, e.prototype.forEachInvertedInner = function(s, i, o, l) {
         for (var a = i - 1; a >= o; a--)
             if (s(this.values[a], l + a) === !1) return !1
     }, e.prototype.leafAppend = function(s) {
-        if (this.length + s.length <= So) return new e(this.values.concat(s.flatten()))
+        if (this.length + s.length <= Co) return new e(this.values.concat(s.flatten()))
     }, e.prototype.leafPrepend = function(s) {
-        if (this.length + s.length <= So) return new e(s.flatten().concat(this.values))
+        if (this.length + s.length <= Co) return new e(s.flatten().concat(this.values))
     }, n.length.get = function() {
         return this.values.length
     }, n.depth.get = function() {
         return 0
     }, Object.defineProperties(e.prototype, n), e
 }(ot);
 ot.empty = new og([]);
-var LO = function(t) {
+var BO = function(t) {
         function e(n, r) {
             t.call(this), this.left = n, this.right = r, this.length = n.length + r.length, this.depth = Math.max(n.depth, r.depth) + 1
         }
         return t && (e.__proto__ = t), e.prototype = Object.create(t && t.prototype), e.prototype.constructor = e, e.prototype.flatten = function() {
             return this.left.flatten().concat(this.right.flatten())
         }, e.prototype.getInner = function(r) {
             return r < this.left.length ? this.left.get(r) : this.right.get(r - this.left.length)
@@ -21657,15 +21660,15 @@
             var s = this.left.leafPrepend(r);
             if (s) return new e(s, this.right)
         }, e.prototype.appendInner = function(r) {
             return this.left.depth >= Math.max(this.right.depth, r.depth) + 1 ? new e(this.left, new e(this.right, r)) : new e(this, r)
         }, e
     }(ot),
     lg = ot;
-const FO = 500;
+const HO = 500;
 class Xt {
     constructor(e, n) {
         this.items = e, this.eventCount = n
     }
     popEvent(e, n) {
         if (this.eventCount == 0) return null;
         let r = this.items.length;
@@ -21704,15 +21707,15 @@
         for (let u = 0; u < e.steps.length; u++) {
             let d = e.steps[u].invert(e.docs[u]),
                 f = new ln(e.mapping.maps[u], d, n),
                 h;
             (h = a && a.merge(f)) && (f = h, u ? i.pop() : l = l.slice(0, l.length - 1)), i.push(f), n && (o++, n = void 0), s || (a = f)
         }
         let c = o - r.depth;
-        return c > HO && (l = BO(l, c), o -= c), new Xt(l.append(i), o)
+        return c > VO && (l = zO(l, c), o -= c), new Xt(l.append(i), o)
     }
     remapping(e, n) {
         let r = new es;
         return this.items.forEach((s, i) => {
             let o = s.mirrorOffset != null && i - s.mirrorOffset >= e ? r.maps.length - s.mirrorOffset : void 0;
             r.appendMap(s.map, o)
         }, e, n), r
@@ -21742,15 +21745,15 @@
                 v && l++, r.push(new ln(p, g, v))
             } else r.push(new ln(p))
         }, s);
         let c = [];
         for (let f = n; f < o; f++) c.push(new ln(i.maps[f]));
         let u = this.items.slice(0, s).append(c).append(r),
             d = new Xt(u, l);
-        return d.emptyItemCount() > FO && (d = d.compress(this.items.length - r.length)), d
+        return d.emptyItemCount() > HO && (d = d.compress(this.items.length - r.length)), d
     }
     emptyItemCount() {
         let e = 0;
         return this.items.forEach(n => {
             n.step || e++
         }), e
     }
@@ -21773,15 +21776,15 @@
                 }
             } else o.map && r--
         }, this.items.length, 0), new Xt(lg.from(s.reverse()), i)
     }
 }
 Xt.empty = new Xt(lg.empty, 0);
 
-function BO(t, e) {
+function zO(t, e) {
     let n;
     return t.forEach((r, s) => {
         if (r.selection && e-- == 0) return n = s, !1
     }), t.slice(n)
 }
 class ln {
     constructor(e, n, r, s) {
@@ -21795,33 +21798,33 @@
     }
 }
 class Wn {
     constructor(e, n, r, s, i) {
         this.done = e, this.undone = n, this.prevRanges = r, this.prevTime = s, this.prevComposition = i
     }
 }
-const HO = 20;
+const VO = 20;
 
-function zO(t, e, n, r) {
+function jO(t, e, n, r) {
     let s = n.getMeta(nr),
         i;
     if (s) return s.historyState;
-    n.getMeta(jO) && (t = new Wn(t.done, t.undone, null, 0, -1));
+    n.getMeta(WO) && (t = new Wn(t.done, t.undone, null, 0, -1));
     let o = n.getMeta("appendedTransaction");
     if (n.steps.length == 0) return t;
-    if (o && o.getMeta(nr)) return o.getMeta(nr).redo ? new Wn(t.done.addTransform(n, void 0, r, Xi(e)), t.undone, Pf(n.mapping.maps[n.steps.length - 1]), t.prevTime, t.prevComposition) : new Wn(t.done, t.undone.addTransform(n, void 0, r, Xi(e)), null, t.prevTime, t.prevComposition);
+    if (o && o.getMeta(nr)) return o.getMeta(nr).redo ? new Wn(t.done.addTransform(n, void 0, r, Zi(e)), t.undone, Pf(n.mapping.maps[n.steps.length - 1]), t.prevTime, t.prevComposition) : new Wn(t.done, t.undone.addTransform(n, void 0, r, Zi(e)), null, t.prevTime, t.prevComposition);
     if (n.getMeta("addToHistory") !== !1 && !(o && o.getMeta("addToHistory") === !1)) {
         let l = n.getMeta("composition"),
-            a = t.prevTime == 0 || !o && t.prevComposition != l && (t.prevTime < (n.time || 0) - r.newGroupDelay || !VO(n, t.prevRanges)),
+            a = t.prevTime == 0 || !o && t.prevComposition != l && (t.prevTime < (n.time || 0) - r.newGroupDelay || !UO(n, t.prevRanges)),
             c = o ? ra(t.prevRanges, n.mapping) : Pf(n.mapping.maps[n.steps.length - 1]);
-        return new Wn(t.done.addTransform(n, a ? e.selection.getBookmark() : void 0, r, Xi(e)), Xt.empty, c, n.time, l ?? t.prevComposition)
+        return new Wn(t.done.addTransform(n, a ? e.selection.getBookmark() : void 0, r, Zi(e)), Xt.empty, c, n.time, l ?? t.prevComposition)
     } else return (i = n.getMeta("rebased")) ? new Wn(t.done.rebased(n, i), t.undone.rebased(n, i), ra(t.prevRanges, n.mapping), t.prevTime, t.prevComposition) : new Wn(t.done.addMaps(n.mapping.maps), t.undone.addMaps(n.mapping.maps), ra(t.prevRanges, n.mapping), t.prevTime, t.prevComposition)
 }
 
-function VO(t, e) {
+function UO(t, e) {
     if (!e) return !1;
     if (!t.docChanged) return !0;
     let n = !1;
     return t.mapping.maps[0].forEach((r, s) => {
         for (let i = 0; i < e.length; i += 2) r <= e[i + 1] && s >= e[i] && (n = !0)
     }), n
 }
@@ -21839,56 +21842,56 @@
             i = e.map(t[r + 1], -1);
         s <= i && n.push(s, i)
     }
     return n
 }
 
 function ag(t, e, n, r) {
-    let s = Xi(e),
+    let s = Zi(e),
         i = nr.get(e).spec.config,
         o = (r ? t.undone : t.done).popEvent(e, s);
     if (!o) return;
     let l = o.selection.resolve(o.transform.doc),
         a = (r ? t.done : t.undone).addTransform(o.transform, e.selection.getBookmark(), i, s),
         c = new Wn(r ? a : o.remaining, r ? o.remaining : a, null, 0, -1);
     n(o.transform.setSelection(l).setMeta(nr, {
         redo: r,
         historyState: c
     }).scrollIntoView())
 }
 let sa = !1,
     $f = null;
 
-function Xi(t) {
+function Zi(t) {
     let e = t.plugins;
     if ($f != e) {
         sa = !1, $f = e;
         for (let n = 0; n < e.length; n++)
             if (e[n].spec.historyPreserveItems) {
                 sa = !0;
                 break
             }
     }
     return sa
 }
 const nr = new Sn("history"),
-    jO = new Sn("closeHistory");
+    WO = new Sn("closeHistory");
 
-function UO(t = {}) {
+function qO(t = {}) {
     return t = {
         depth: t.depth || 100,
         newGroupDelay: t.newGroupDelay || 500
     }, new Mt({
         key: nr,
         state: {
             init() {
                 return new Wn(Xt.empty, Xt.empty, null, 0, -1)
             },
             apply(e, n, r) {
-                return zO(n, r, e, t)
+                return jO(n, r, e, t)
             }
         },
         config: t,
         props: {
             handleDOMEvents: {
                 beforeinput(e, n) {
                     let r = n.inputType,
@@ -21903,15 +21906,15 @@
         let n = nr.getState(t);
         return !n || n.done.eventCount == 0 ? !1 : (e && ag(n, t, e, !1), !0)
     },
     ug = (t, e) => {
         let n = nr.getState(t);
         return !n || n.undone.eventCount == 0 ? !1 : (e && ag(n, t, e, !0), !0)
     },
-    WO = kt.create({
+    KO = kt.create({
         name: "history",
         addOptions() {
             return {
                 depth: 100,
                 newGroupDelay: 500
             }
         },
@@ -21924,27 +21927,27 @@
                 redo: () => ({
                     state: t,
                     dispatch: e
                 }) => ug(t, e)
             }
         },
         addProseMirrorPlugins() {
-            return [UO(this.options)]
+            return [qO(this.options)]
         },
         addKeyboardShortcuts() {
             return {
                 "Mod-z": () => this.editor.commands.undo(),
                 "Mod-y": () => this.editor.commands.redo(),
                 "Shift-Mod-z": () => this.editor.commands.redo(),
                 "Mod-я": () => this.editor.commands.undo(),
                 "Shift-Mod-я": () => this.editor.commands.redo()
             }
         }
     }),
-    qO = pt.create({
+    JO = pt.create({
         name: "horizontalRule",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         group: "block",
@@ -21981,25 +21984,25 @@
                         e.scrollIntoView()
                     }
                     return !0
                 }).run()
             }
         },
         addInputRules() {
-            return [TE({
+            return [ME({
                 find: /^(?:---|—-|___\s|\*\*\*\s)$/,
                 type: this.type
             })]
         }
     }),
-    KO = /(?:^|\s)((?:\*)((?:[^*]+))(?:\*))$/,
-    JO = /(?:^|\s)((?:\*)((?:[^*]+))(?:\*))/g,
-    GO = /(?:^|\s)((?:_)((?:[^_]+))(?:_))$/,
-    YO = /(?:^|\s)((?:_)((?:[^_]+))(?:_))/g,
-    XO = xn.create({
+    GO = /(?:^|\s)((?:\*)((?:[^*]+))(?:\*))$/,
+    YO = /(?:^|\s)((?:\*)((?:[^*]+))(?:\*))/g,
+    XO = /(?:^|\s)((?:_)((?:[^_]+))(?:_))$/,
+    QO = /(?:^|\s)((?:_)((?:[^_]+))(?:_))/g,
+    ZO = xn.create({
         name: "italic",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -22034,32 +22037,32 @@
             return {
                 "Mod-i": () => this.editor.commands.toggleItalic(),
                 "Mod-I": () => this.editor.commands.toggleItalic()
             }
         },
         addInputRules() {
             return [gs({
-                find: KO,
+                find: GO,
                 type: this.type
             }), gs({
-                find: GO,
+                find: XO,
                 type: this.type
             })]
         },
         addPasteRules() {
             return [ys({
-                find: JO,
+                find: YO,
                 type: this.type
             }), ys({
-                find: YO,
+                find: QO,
                 type: this.type
             })]
         }
     }),
-    QO = pt.create({
+    eM = pt.create({
         name: "listItem",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         content: "paragraph block*",
@@ -22078,15 +22081,15 @@
             return {
                 Enter: () => this.editor.commands.splitListItem(this.name),
                 Tab: () => this.editor.commands.sinkListItem(this.name),
                 "Shift-Tab": () => this.editor.commands.liftListItem(this.name)
             }
         }
     }),
-    ZO = pt.create({
+    tM = pt.create({
         name: "listItem",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         content: "paragraph block*",
@@ -22136,15 +22139,15 @@
                     const n = al(t, this.type);
                     return Object.entries(n).some(([, s]) => !!s) ? !0 : e.unsetMark(this.name)
                 }
             }
         }
     }),
     Ff = /^(\d+)\.\s$/,
-    eM = pt.create({
+    nM = pt.create({
         name: "orderedList",
         addOptions() {
             return {
                 itemTypeName: "listItem",
                 HTMLAttributes: {},
                 keepMarks: !1,
                 keepAttributes: !1
@@ -22177,15 +22180,15 @@
             return e === 1 ? ["ol", Qe(this.options.HTMLAttributes, n), 0] : ["ol", Qe(this.options.HTMLAttributes, t), 0]
         },
         addCommands() {
             return {
                 toggleOrderedList: () => ({
                     commands: t,
                     chain: e
-                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(ZO.name, this.editor.getAttributes(Lf.name)).run() : t.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
+                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(tM.name, this.editor.getAttributes(Lf.name)).run() : t.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
             }
         },
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-7": () => this.editor.commands.toggleOrderedList()
             }
         },
@@ -22208,15 +22211,15 @@
                     ...this.editor.getAttributes(Lf.name)
                 }),
                 joinPredicate: (e, n) => n.childCount + n.attrs.start === +e[1],
                 editor: this.editor
             })), [t]
         }
     }),
-    tM = pt.create({
+    rM = pt.create({
         name: "paragraph",
         priority: 1e3,
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
@@ -22241,17 +22244,17 @@
         },
         addKeyboardShortcuts() {
             return {
                 "Mod-Alt-0": () => this.editor.commands.setParagraph()
             }
         }
     }),
-    nM = /(?:^|\s)((?:~~)((?:[^~]+))(?:~~))$/,
-    rM = /(?:^|\s)((?:~~)((?:[^~]+))(?:~~))/g,
-    sM = xn.create({
+    sM = /(?:^|\s)((?:~~)((?:[^~]+))(?:~~))$/,
+    iM = /(?:^|\s)((?:~~)((?:[^~]+))(?:~~))/g,
+    oM = xn.create({
         name: "strike",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -22288,246 +22291,246 @@
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-x": () => this.editor.commands.toggleStrike()
             }
         },
         addInputRules() {
             return [gs({
-                find: nM,
+                find: sM,
                 type: this.type
             })]
         },
         addPasteRules() {
             return [ys({
-                find: rM,
+                find: iM,
                 type: this.type
             })]
         }
     }),
-    iM = pt.create({
+    lM = pt.create({
         name: "text",
         group: "inline"
     }),
-    oM = kt.create({
+    aM = kt.create({
         name: "starterKit",
         addExtensions() {
             var t, e, n, r, s, i, o, l, a, c, u, d, f, h, p, g, v, x;
             const w = [];
-            return this.options.blockquote !== !1 && w.push(cO.configure((t = this.options) === null || t === void 0 ? void 0 : t.blockquote)), this.options.bold !== !1 && w.push(pO.configure((e = this.options) === null || e === void 0 ? void 0 : e.bold)), this.options.bulletList !== !1 && w.push(gO.configure((n = this.options) === null || n === void 0 ? void 0 : n.bulletList)), this.options.code !== !1 && w.push(vO.configure((r = this.options) === null || r === void 0 ? void 0 : r.code)), this.options.codeBlock !== !1 && w.push(wO.configure((s = this.options) === null || s === void 0 ? void 0 : s.codeBlock)), this.options.document !== !1 && w.push(SO.configure((i = this.options) === null || i === void 0 ? void 0 : i.document)), this.options.dropcursor !== !1 && w.push(EO.configure((o = this.options) === null || o === void 0 ? void 0 : o.dropcursor)), this.options.gapcursor !== !1 && w.push(IO.configure((l = this.options) === null || l === void 0 ? void 0 : l.gapcursor)), this.options.hardBreak !== !1 && w.push(PO.configure((a = this.options) === null || a === void 0 ? void 0 : a.hardBreak)), this.options.heading !== !1 && w.push($O.configure((c = this.options) === null || c === void 0 ? void 0 : c.heading)), this.options.history !== !1 && w.push(WO.configure((u = this.options) === null || u === void 0 ? void 0 : u.history)), this.options.horizontalRule !== !1 && w.push(qO.configure((d = this.options) === null || d === void 0 ? void 0 : d.horizontalRule)), this.options.italic !== !1 && w.push(XO.configure((f = this.options) === null || f === void 0 ? void 0 : f.italic)), this.options.listItem !== !1 && w.push(QO.configure((h = this.options) === null || h === void 0 ? void 0 : h.listItem)), this.options.orderedList !== !1 && w.push(eM.configure((p = this.options) === null || p === void 0 ? void 0 : p.orderedList)), this.options.paragraph !== !1 && w.push(tM.configure((g = this.options) === null || g === void 0 ? void 0 : g.paragraph)), this.options.strike !== !1 && w.push(sM.configure((v = this.options) === null || v === void 0 ? void 0 : v.strike)), this.options.text !== !1 && w.push(iM.configure((x = this.options) === null || x === void 0 ? void 0 : x.text)), w
+            return this.options.blockquote !== !1 && w.push(dO.configure((t = this.options) === null || t === void 0 ? void 0 : t.blockquote)), this.options.bold !== !1 && w.push(gO.configure((e = this.options) === null || e === void 0 ? void 0 : e.bold)), this.options.bulletList !== !1 && w.push(bO.configure((n = this.options) === null || n === void 0 ? void 0 : n.bulletList)), this.options.code !== !1 && w.push(kO.configure((r = this.options) === null || r === void 0 ? void 0 : r.code)), this.options.codeBlock !== !1 && w.push(_O.configure((s = this.options) === null || s === void 0 ? void 0 : s.codeBlock)), this.options.document !== !1 && w.push(CO.configure((i = this.options) === null || i === void 0 ? void 0 : i.document)), this.options.dropcursor !== !1 && w.push(OO.configure((o = this.options) === null || o === void 0 ? void 0 : o.dropcursor)), this.options.gapcursor !== !1 && w.push($O.configure((l = this.options) === null || l === void 0 ? void 0 : l.gapcursor)), this.options.hardBreak !== !1 && w.push(LO.configure((a = this.options) === null || a === void 0 ? void 0 : a.hardBreak)), this.options.heading !== !1 && w.push(FO.configure((c = this.options) === null || c === void 0 ? void 0 : c.heading)), this.options.history !== !1 && w.push(KO.configure((u = this.options) === null || u === void 0 ? void 0 : u.history)), this.options.horizontalRule !== !1 && w.push(JO.configure((d = this.options) === null || d === void 0 ? void 0 : d.horizontalRule)), this.options.italic !== !1 && w.push(ZO.configure((f = this.options) === null || f === void 0 ? void 0 : f.italic)), this.options.listItem !== !1 && w.push(eM.configure((h = this.options) === null || h === void 0 ? void 0 : h.listItem)), this.options.orderedList !== !1 && w.push(nM.configure((p = this.options) === null || p === void 0 ? void 0 : p.orderedList)), this.options.paragraph !== !1 && w.push(rM.configure((g = this.options) === null || g === void 0 ? void 0 : g.paragraph)), this.options.strike !== !1 && w.push(oM.configure((v = this.options) === null || v === void 0 ? void 0 : v.strike)), this.options.text !== !1 && w.push(lM.configure((x = this.options) === null || x === void 0 ? void 0 : x.text)), w
         }
     }),
-    lM = {
+    cM = {
         class: "editor-wrapper content"
     },
-    aM = {
+    uM = {
         key: 0,
         class: "buttons"
     },
-    cM = m("i", {
+    dM = m("i", {
         class: "fa fa-paragraph",
         "aria-hidden": "true"
     }, null, -1),
-    uM = [cM],
-    dM = ["disabled"],
-    fM = m("i", {
+    fM = [dM],
+    hM = ["disabled"],
+    pM = m("i", {
         class: "fa fa-bold",
         "aria-hidden": "true"
     }, null, -1),
-    hM = [fM],
-    pM = ["disabled"],
-    mM = m("i", {
+    mM = [pM],
+    gM = ["disabled"],
+    yM = m("i", {
         class: "fa fa-italic",
         "aria-hidden": "true"
     }, null, -1),
-    gM = [mM],
-    yM = ["disabled"],
-    bM = m("i", {
-        class: "fa fa-strikethrough",
-        "aria-hidden": "true"
-    }, null, -1),
-    vM = [bM],
+    bM = [yM],
+    vM = ["disabled"],
     xM = m("i", {
-        class: "fa fa-heading",
+        class: "fa fa-strikethrough",
         "aria-hidden": "true"
     }, null, -1),
     kM = [xM],
     wM = m("i", {
         class: "fa fa-heading",
         "aria-hidden": "true"
     }, null, -1),
-    SM = m("i", {
-        class: "fa fa-heading",
-        "aria-hidden": "true"
-    }, null, -1),
+    SM = [wM],
     _M = m("i", {
         class: "fa fa-heading",
         "aria-hidden": "true"
     }, null, -1),
     CM = m("i", {
         class: "fa fa-heading",
         "aria-hidden": "true"
     }, null, -1),
     EM = m("i", {
-        class: "fa fa-list-ul",
+        class: "fa fa-heading",
+        "aria-hidden": "true"
+    }, null, -1),
+    TM = m("i", {
+        class: "fa fa-heading",
         "aria-hidden": "true"
     }, null, -1),
-    TM = [EM],
     OM = m("i", {
-        class: "fa fa-list-ol",
+        class: "fa fa-list-ul",
         "aria-hidden": "true"
     }, null, -1),
     MM = [OM],
     AM = m("i", {
-        class: "fa fa-code",
+        class: "fa fa-list-ol",
         "aria-hidden": "true"
     }, null, -1),
     NM = [AM],
     RM = m("i", {
-        class: "fa-solid fa-comment-dots"
+        class: "fa fa-code",
+        "aria-hidden": "true"
     }, null, -1),
     DM = [RM],
     IM = m("i", {
-        class: "fa-solid fa-ruler-horizontal"
+        class: "fa-solid fa-comment-dots"
     }, null, -1),
     PM = [IM],
-    $M = ["disabled"],
-    LM = m("i", {
+    $M = m("i", {
+        class: "fa-solid fa-ruler-horizontal"
+    }, null, -1),
+    LM = [$M],
+    FM = ["disabled"],
+    BM = m("i", {
         class: "fa-solid fa-rotate-left"
     }, null, -1),
-    FM = [LM],
-    BM = ["disabled"],
-    HM = m("i", {
+    HM = [BM],
+    zM = ["disabled"],
+    VM = m("i", {
         class: "fa-solid fa-rotate-right"
     }, null, -1),
-    zM = [HM],
-    VM = ir({
+    jM = [VM],
+    UM = ir({
         __name: "TextEditor",
         props: ["text"],
         emits: ["editorUpdate"],
         setup(t, {
             emit: e
         }) {
-            const r = lO({
+            const r = cO({
                 content: t.text,
                 onUpdate: ({
                     editor: s
                 }) => {
                     e("editorUpdate", s.getHTML())
                 },
-                extensions: [oM]
+                extensions: [aM]
             });
             return or(() => {
                 var s;
                 return (s = r.value) == null ? void 0 : s.destroy()
-            }), (s, i) => (C(), R("div", null, [m("div", lM, [de(r) ? (C(), R("div", aM, [m("button", {
+            }), (s, i) => (C(), R("div", null, [m("div", cM, [de(r) ? (C(), R("div", uM, [m("button", {
                 onClick: i[0] || (i[0] = o => de(r).chain().focus().setParagraph().run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("paragraph")
                 })
-            }, uM, 2), m("button", {
+            }, fM, 2), m("button", {
                 onClick: i[1] || (i[1] = o => de(r).chain().focus().toggleBold().run()),
                 disabled: !de(r).can().chain().focus().toggleBold().run(),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("bold")
                 })
-            }, hM, 10, dM), m("button", {
+            }, mM, 10, hM), m("button", {
                 onClick: i[2] || (i[2] = o => de(r).chain().focus().toggleItalic().run()),
                 disabled: !de(r).can().chain().focus().toggleItalic().run(),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("italic")
                 })
-            }, gM, 10, pM), m("button", {
+            }, bM, 10, gM), m("button", {
                 onClick: i[3] || (i[3] = o => de(r).chain().focus().toggleStrike().run()),
                 disabled: !de(r).can().chain().focus().toggleStrike().run(),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("strike")
                 })
-            }, vM, 10, yM), m("button", {
+            }, kM, 10, vM), m("button", {
                 onClick: i[4] || (i[4] = o => de(r).chain().focus().toggleHeading({
                     level: 1
                 }).run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("heading", {
                         level: 1
                     })
                 })
-            }, kM, 2), m("button", {
+            }, SM, 2), m("button", {
                 onClick: i[5] || (i[5] = o => de(r).chain().focus().toggleHeading({
                     level: 2
                 }).run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("heading", {
                         level: 2
                     })
                 })
-            }, [wM, Ge("2 ")], 2), m("button", {
+            }, [_M, Ge("2 ")], 2), m("button", {
                 onClick: i[6] || (i[6] = o => de(r).chain().focus().toggleHeading({
                     level: 3
                 }).run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("heading", {
                         level: 3
                     })
                 })
-            }, [SM, Ge("3 ")], 2), m("button", {
+            }, [CM, Ge("3 ")], 2), m("button", {
                 onClick: i[7] || (i[7] = o => de(r).chain().focus().toggleHeading({
                     level: 4
                 }).run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("heading", {
                         level: 4
                     })
                 })
-            }, [_M, Ge("4 ")], 2), m("button", {
+            }, [EM, Ge("4 ")], 2), m("button", {
                 onClick: i[8] || (i[8] = o => de(r).chain().focus().toggleHeading({
                     level: 5
                 }).run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("heading", {
                         level: 5
                     })
                 })
-            }, [CM, Ge("5 ")], 2), m("button", {
+            }, [TM, Ge("5 ")], 2), m("button", {
                 onClick: i[9] || (i[9] = o => de(r).chain().focus().toggleBulletList().run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("bulletList")
                 })
-            }, TM, 2), m("button", {
+            }, MM, 2), m("button", {
                 onClick: i[10] || (i[10] = o => de(r).chain().focus().toggleOrderedList().run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("orderedList")
                 })
-            }, MM, 2), m("button", {
+            }, NM, 2), m("button", {
                 onClick: i[11] || (i[11] = o => de(r).chain().focus().toggleCodeBlock().run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("codeBlock")
                 })
-            }, NM, 2), m("button", {
+            }, DM, 2), m("button", {
                 onClick: i[12] || (i[12] = o => de(r).chain().focus().toggleBlockquote().run()),
-                class: he({
+                class: fe({
                     "is-active": de(r).isActive("blockquote")
                 })
-            }, DM, 2), m("button", {
+            }, PM, 2), m("button", {
                 onClick: i[13] || (i[13] = o => de(r).chain().focus().setHorizontalRule().run())
-            }, PM), m("button", {
+            }, LM), m("button", {
                 onClick: i[14] || (i[14] = o => de(r).chain().focus().undo().run()),
                 disabled: !de(r).can().chain().focus().undo().run()
-            }, FM, 8, $M), m("button", {
+            }, HM, 8, FM), m("button", {
                 onClick: i[15] || (i[15] = o => de(r).chain().focus().redo().run()),
                 disabled: !de(r).can().chain().focus().redo().run()
-            }, zM, 8, BM)])) : re("", !0), ce(de(oO), {
+            }, jM, 8, zM)])) : re("", !0), ce(de(aO), {
                 editor: de(r)
             }, null, 8, ["editor"])])]))
         }
     });
 const Bf = (t, e) => t || e,
-    jM = {
+    WM = {
         props: ["recipe"],
         components: {
-            TextEditor: VM,
+            TextEditor: UM,
             Counter: gp
         },
         data() {
             return {
                 addIngredientSmartField: null,
                 smartFieldError: null,
                 smartFieldAutocomplete: [],
@@ -22603,453 +22606,441 @@
                     ingredient: {
                         name: s
                     },
                     note: i
                 }
             },
             getRootData() {
-                var t = `${ke.HOST_URL}/`;
-                Le.get(t).then(e => {
-                    e.status !== "success" && e.data && (this.availableTags = e.data.tags)
-                }).catch(e => this.error = e), t = `${ke.HOST_URL}/ingredients`, Le.get(t).then(e => {
+                var t = `${ke.HOST_URL}/tags`;
+                Fe.get(t).then(e => this.availableTags = e.data).catch(e => this.error = e), t = `${ke.HOST_URL}/ingredients`, Fe.get(t).then(e => {
                     e.status !== "success" && e.data && (this.ingredients = e.data.map(n => n.name))
                 }).catch(e => this.error = e)
             },
             postRecipe() {
                 if (this.recipe.id) {
                     const t = `${ke.HOST_URL}/recipes/${this.recipe.id}`,
                         e = {
                             headers: {
                                 "Content-Type": "application/json"
                             }
                         };
-                    Le.put(t, this.recipe, e).then(n => {
+                    Fe.put(t, this.recipe, e).then(n => {
                         this.postSuccess = `${n.status} ${n.statusText}`, this.$emit("recipePosted", n.data)
                     }).catch(n => {
                         this.postError = n.response.data
                     })
                 } else {
                     const t = `${ke.HOST_URL}/recipes`,
                         e = {
                             headers: {
                                 "Content-Type": "application/json"
                             }
                         };
-                    Le.post(t, this.recipe, e).then(n => {
+                    Fe.post(t, this.recipe, e).then(n => {
                         this.postSuccess = `${n.status} ${n.statusText}`, this.$emit("recipePosted", n.data)
                     }).catch(n => {
                         this.postError = n.response.data
                     })
                 }
             }
         },
         created() {
             this.getRootData(), this.counter = this.recipe.portions
         }
     },
-    UM = {
+    qM = {
         key: 0
     },
-    WM = {
+    KM = {
         class: "field"
     },
-    qM = {
+    JM = {
         class: "control has-icons-left has-icons-right"
     },
-    KM = m("span", {
+    GM = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-heading"
     })], -1),
-    JM = {
+    YM = {
         key: 0,
         class: "icon is-small is-right"
     },
-    GM = m("i", {
+    XM = m("i", {
         class: "fas fa-check"
     }, null, -1),
-    YM = [GM],
-    XM = {
+    QM = [XM],
+    ZM = {
         key: 0,
         class: "help is-danger"
     },
-    QM = {
+    eA = {
         class: "field"
     },
-    ZM = {
+    tA = {
         class: "control has-icons-left has-icons-right"
     },
-    eA = m("span", {
+    nA = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-font"
     })], -1),
-    tA = {
+    rA = {
         class: "field"
     },
-    nA = {
+    sA = {
         class: "control has-icons-left has-icons-right"
     },
-    rA = m("span", {
+    iA = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-link"
     })], -1),
-    sA = {
+    oA = {
         key: 0,
         class: "field"
     },
-    iA = {
+    lA = {
         class: "control has-icons-left has-icons-right"
     },
-    oA = m("span", {
+    aA = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-link"
     })], -1),
-    lA = {
+    cA = {
         class: "checkbox my-2"
     },
-    aA = m("i", {
+    uA = m("i", {
         class: "far fa-lightbulb"
     }, null, -1),
-    cA = {
+    dA = {
         key: 1
     },
-    uA = m("label", {
+    fA = m("label", {
         class: "label"
     }, "Ingredients", -1),
-    dA = {
+    hA = {
         class: "field"
     },
-    fA = {
+    pA = {
         class: "control"
     },
-    hA = {
+    mA = {
         class: "tags"
     },
-    pA = {
+    gA = {
         key: 0
     },
-    mA = ["onClick"],
-    gA = {
+    yA = ["onClick"],
+    bA = {
         class: "field has-addons my-0"
     },
-    yA = m("span", {
+    vA = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-drumstick-bite"
     })], -1),
-    bA = {
+    xA = {
         class: "dropdown-menu fullwidth",
         id: "dropdown-menu",
         role: "menu"
     },
-    vA = {
+    kA = {
         class: "dropdown-content"
     },
-    xA = ["onClick"],
-    kA = {
+    wA = ["onClick"],
+    SA = {
         class: "control"
     },
-    wA = ["disabled"],
-    SA = m("span", {
+    _A = ["disabled"],
+    CA = m("span", {
         class: "icon is-small"
     }, [m("i", {
         class: "fas fa-plus"
     })], -1),
-    _A = [SA],
-    CA = {
+    EA = [CA],
+    TA = {
         key: 0,
         class: "help is-danger"
     },
-    EA = {
+    OA = {
         key: 1,
         class: "help is-info"
     },
-    TA = {
+    MA = {
         class: "mt-4"
     },
-    OA = m("label", {
+    AA = m("label", {
         class: "label has-text-centered"
     }, "(1 batch)", -1),
-    MA = m("hr", null, null, -1),
-    AA = {
+    NA = m("hr", null, null, -1),
+    RA = {
         key: 2,
         class: "field my-2"
     },
-    NA = {
+    DA = {
         class: "control"
     },
-    RA = {
+    IA = {
         class: "field"
     },
-    DA = m("label", {
+    PA = m("label", {
         class: "label"
     }, "Tags", -1),
-    IA = {
+    $A = {
         key: 0,
         class: "message is-warning p-0"
     },
-    PA = m("small", {
+    LA = m("small", {
         class: "message-body p-2"
     }, "no tags created yet", -1),
-    $A = [PA],
-    LA = {
+    FA = [LA],
+    BA = {
         class: "control"
     },
-    FA = ["onClick"],
-    BA = {
+    HA = ["onClick"],
+    zA = {
         class: "mb-5"
     },
-    HA = {
+    VA = {
         class: "field has-addons"
     },
-    zA = {
+    jA = {
         class: "control is-expanded"
     },
-    VA = {
+    UA = {
         class: "control"
     },
-    jA = m("i", {
+    WA = m("i", {
         class: "fas fa-plus"
     }, null, -1),
-    UA = [jA],
-    WA = {
+    qA = [WA],
+    KA = {
         class: "my-1"
     },
-    qA = ["disabled"],
-    KA = {
+    JA = ["disabled"],
+    GA = {
         class: "my-1"
     },
-    JA = {
+    YA = {
         key: 3,
         class: "message is-success"
     },
-    GA = {
+    XA = {
         class: "message-body"
     },
-    YA = {
+    QA = {
         key: 4,
         class: "message is-danger"
     },
-    XA = {
+    ZA = {
         class: "message-body"
     };
 
-function QA(t, e, n, r, s, i) {
+function eN(t, e, n, r, s, i) {
     const o = Oe("Counter"),
         l = Oe("TextEditor");
-    return n.recipe ? (C(), R("div", UM, [m("div", WM, [m("div", qM, [We(m("input", {
+    return n.recipe ? (C(), R("div", qM, [m("div", KM, [m("div", JM, [We(m("input", {
         "onUpdate:modelValue": e[0] || (e[0] = a => n.recipe.title = a),
-        class: he({
+        class: fe({
             input: !0,
             "is-success": n.recipe.title,
             "is-danger": !n.recipe.title
         }),
         type: "text",
         placeholder: "Title"
     }, null, 2), [
         [st, n.recipe.title]
-    ]), KM, n.recipe.title ? (C(), R("span", JM, YM)) : re("", !0)]), n.recipe.title ? re("", !0) : (C(), R("p", XM, " Title is required "))]), m("div", QM, [m("div", ZM, [We(m("input", {
+    ]), GM, n.recipe.title ? (C(), R("span", YM, QM)) : re("", !0)]), n.recipe.title ? re("", !0) : (C(), R("p", ZM, " Title is required "))]), m("div", eA, [m("div", tA, [We(m("input", {
         "onUpdate:modelValue": e[1] || (e[1] = a => n.recipe.subtitle = a),
         class: "input",
         type: "text",
         placeholder: "Subtitle"
     }, null, 512), [
         [st, n.recipe.subtitle]
-    ]), eA])]), m("div", tA, [m("div", nA, [We(m("input", {
+    ]), nA])]), m("div", rA, [m("div", sA, [We(m("input", {
         "onUpdate:modelValue": e[2] || (e[2] = a => n.recipe.source = a),
         class: "input",
         type: "text",
         placeholder: "Source link"
     }, null, 512), [
         [st, n.recipe.source]
-    ]), rA])]), n.recipe.source ? (C(), R("div", sA, [m("div", iA, [We(m("input", {
+    ]), iA])]), n.recipe.source ? (C(), R("div", oA, [m("div", lA, [We(m("input", {
         "onUpdate:modelValue": e[3] || (e[3] = a => n.recipe.source_name = a),
         class: "input",
         type: "text",
         placeholder: "Source name"
     }, null, 512), [
         [st, n.recipe.source_name]
-    ]), oA])])) : re("", !0), m("label", lA, [We(m("input", {
+    ]), aA])])) : re("", !0), m("label", cA, [We(m("input", {
         type: "checkbox",
         "onUpdate:modelValue": e[4] || (e[4] = a => n.recipe.draft = a)
     }, null, 512), [
-        [Wb, n.recipe.draft]
-    ]), Ge(" Recipe idea "), aA]), n.recipe.draft ? re("", !0) : (C(), R("div", cA, [uA, m("div", dA, [m("div", fA, [m("div", hA, [(C(!0), R(Fe, null, Dt(n.recipe.ingredients, (a, c) => (C(), R("span", {
+        [qb, n.recipe.draft]
+    ]), Ge(" Recipe idea "), uA]), n.recipe.draft ? re("", !0) : (C(), R("div", dA, [fA, m("div", hA, [m("div", pA, [m("div", mA, [(C(!0), R(Le, null, Dt(n.recipe.ingredients, (a, c) => (C(), R("span", {
         key: a + c,
         class: "tag"
-    }, [m("p", null, [Ge(le(a.amount), 1), m("strong", null, le(a.unit.name), 1), Ge(" " + le(a.ingredient.name) + " ", 1), a.note ? (C(), R("span", pA, "(" + le(a.note) + ")", 1)) : re("", !0)]), m("button", {
+    }, [m("p", null, [Ge(le(a.amount), 1), m("strong", null, le(a.unit.name), 1), Ge(" " + le(a.ingredient.name) + " ", 1), a.note ? (C(), R("span", gA, "(" + le(a.note) + ")", 1)) : re("", !0)]), m("button", {
         onClick: u => i.removeIngredient(a),
         class: "delete is-small"
-    }, null, 8, mA)]))), 128))])])]), m("div", gA, [m("div", {
-        class: he({
+    }, null, 8, yA)]))), 128))])])]), m("div", bA, [m("div", {
+        class: fe({
             dropdown: !0,
             "is-active": s.smartFieldAutocomplete.length > 0,
             control: !0,
             "is-expanded": !0,
             "is-right": !0,
             "has-icons-left": !0
         })
     }, [We(m("input", {
-        class: he([{
+        class: fe([{
             "is-danger": s.smartFieldError,
             "is-success": s.parsedSmartField && !s.smartFieldNewIngredient,
             "is-info": s.smartFieldNewIngredient
         }, "input"]),
         "onUpdate:modelValue": e[5] || (e[5] = a => s.addIngredientSmartField = a),
         onInput: e[6] || (e[6] = (...a) => i.parseSmartField && i.parseSmartField(...a)),
         onKeyup: e[7] || (e[7] = (...a) => i.ingredientEnterPressed && i.ingredientEnterPressed(...a)),
         type: "text",
         placeholder: "100g <ingredient>"
     }, null, 34), [
         [st, s.addIngredientSmartField]
-    ]), yA, m("div", bA, [m("div", vA, [(C(!0), R(Fe, null, Dt(s.smartFieldAutocomplete, (a, c) => (C(), R("a", {
+    ]), vA, m("div", xA, [m("div", kA, [(C(!0), R(Le, null, Dt(s.smartFieldAutocomplete, (a, c) => (C(), R("a", {
         key: c,
         onClick: u => i.autocomplete(a),
         class: "dropdown-item"
-    }, le(a), 9, xA))), 128))])])], 2), m("p", kA, [m("button", {
-        class: he({
+    }, le(a), 9, wA))), 128))])])], 2), m("p", SA, [m("button", {
+        class: fe({
             button: !0,
             "is-success": !s.smartFieldError,
             "is-danger": s.smartFieldError,
             "is-outlined": !0
         }),
         disabled: s.smartFieldError || !s.addIngredientSmartField,
         onClick: e[8] || (e[8] = (...a) => i.confirmIngredient && i.confirmIngredient(...a))
-    }, _A, 10, wA)])]), s.smartFieldError ? (C(), R("p", CA, le(s.smartFieldError), 1)) : re("", !0), s.smartFieldNewIngredient ? (C(), R("p", EA, [Ge(" New ingredient will be added "), m("strong", null, le(s.smartFieldNewIngredient), 1)])) : re("", !0)])), m("div", TA, [ce(o, {
+    }, EA, 10, _A)])]), s.smartFieldError ? (C(), R("p", TA, le(s.smartFieldError), 1)) : re("", !0), s.smartFieldNewIngredient ? (C(), R("p", OA, [Ge(" New ingredient will be added "), m("strong", null, le(s.smartFieldNewIngredient), 1)])) : re("", !0)])), m("div", MA, [ce(o, {
         initialValue: n.recipe.portions,
         onCounterUpdate: i.updateCounter
-    }, null, 8, ["initialValue", "onCounterUpdate"])]), OA, MA, n.recipe.draft ? re("", !0) : (C(), R("div", AA, [m("div", NA, [ce(l, {
+    }, null, 8, ["initialValue", "onCounterUpdate"])]), AA, NA, n.recipe.draft ? re("", !0) : (C(), R("div", RA, [m("div", DA, [ce(l, {
         onEditorUpdate: i.updateText,
         text: n.recipe.body
-    }, null, 8, ["onEditorUpdate", "text"])])])), m("div", RA, [DA, s.availableTags.length < 1 ? (C(), R("article", IA, $A)) : re("", !0), m("div", LA, [m("div", null, [(C(!0), R(Fe, null, Dt(s.availableTags, (a, c) => (C(), R("a", {
+    }, null, 8, ["onEditorUpdate", "text"])])])), m("div", IA, [PA, s.availableTags.length < 1 ? (C(), R("article", $A, FA)) : re("", !0), m("div", BA, [m("div", null, [(C(!0), R(Le, null, Dt(s.availableTags, (a, c) => (C(), R("a", {
         key: a + c,
         onClick: u => i.toggleTag(a)
     }, [m("span", {
-        class: he({
+        class: fe({
             tag: !0,
             "is-dark": n.recipe.tags && n.recipe.tags.map(u => u.name).includes(a.name),
             "is-rounded": !0,
             "mr-1": !0
         })
-    }, le(a.name), 3)], 8, FA))), 128))])])]), m("div", BA, [m("div", HA, [m("div", zA, [We(m("input", {
+    }, le(a.name), 3)], 8, HA))), 128))])])]), m("div", zA, [m("div", VA, [m("div", jA, [We(m("input", {
         "onUpdate:modelValue": e[9] || (e[9] = a => s.createTagField = a),
         class: "input is-small is-rounded",
         type: "text",
         placeholder: "new tag"
     }, null, 512), [
         [st, s.createTagField]
-    ])]), m("div", VA, [m("button", {
+    ])]), m("div", UA, [m("button", {
         onClick: e[10] || (e[10] = (...a) => i.createTag && i.createTag(...a)),
         class: "button is-success is-small is-rounded"
-    }, UA)])])]), m("div", WA, [m("button", {
+    }, qA)])])]), m("div", KA, [m("button", {
         onClick: e[11] || (e[11] = (...a) => i.postRecipe && i.postRecipe(...a)),
         class: "button is-fullwidth is-success",
         disabled: !n.recipe.title
-    }, "Save", 8, qA)]), m("div", KA, [m("button", {
+    }, "Save", 8, JA)]), m("div", GA, [m("button", {
         onClick: e[12] || (e[12] = a => t.$emit("cancel")),
         class: "button is-fullwidth"
-    }, "Cancel")]), s.postSuccess ? (C(), R("article", JA, [m("div", GA, le(s.postSuccess), 1)])) : re("", !0), s.postError ? (C(), R("article", YA, [m("div", XA, le(s.postError), 1)])) : re("", !0)])) : re("", !0)
+    }, "Cancel")]), s.postSuccess ? (C(), R("article", YA, [m("div", XA, le(s.postSuccess), 1)])) : re("", !0), s.postError ? (C(), R("article", QA, [m("div", ZA, le(s.postError), 1)])) : re("", !0)])) : re("", !0)
 }
-const dg = Ue(jM, [
-        ["render", QA]
+const dg = Be(WM, [
+        ["render", eN]
     ]),
-    ZA = {
+    tN = {
         props: ["name", "message"],
         data() {
             return {
                 msg: "404 not found"
             }
         },
         created() {
             this.name && (this.msg = `404 ${this.name} not found.`), this.message && (this.msg = this.message)
         }
     },
-    eN = {
+    nN = {
         class: "section is-medium has-text-centered"
     },
-    tN = m("h1", {
+    rN = m("h1", {
         class: "title"
     }, "Oooops...", -1),
-    nN = {
+    sN = {
         class: "subtitle"
     },
-    rN = m("span", {
+    iN = m("span", {
         class: "icon is-large"
     }, [m("i", {
         class: "fas fa-2x fa-dizzy"
     })], -1);
 
-function sN(t, e, n, r, s, i) {
-    return C(), R("section", eN, [tN, m("h2", nN, le(s.msg), 1), rN])
+function oN(t, e, n, r, s, i) {
+    return C(), R("section", nN, [rN, m("h2", sN, le(s.msg), 1), iN])
 }
-const fg = Ue(ZA, [
-        ["render", sN]
-    ]),
-    iN = {
-        class: "mt-5"
-    },
-    oN = {
-        key: 0,
-        class: "field is-grouped"
+const fg = Be(tN, [
+    ["render", oN]
+]);
+const hg = t => (xi("data-v-4a24b4e8"), t = t(), ki(), t),
+    lN = {
+        key: 0
     },
-    lN = m("button", {
-        class: "button is-small mr-1 is-success is-rounded"
-    }, [m("i", {
-        class: "fa-solid fa-check"
-    }), m("span", {
-        class: "ml-2"
-    }, "planned")], -1),
-    aN = m("i", {
-        class: "fa-solid fa-ban"
-    }, null, -1),
+    aN = hg(() => m("i", {
+        class: "fa-solid fa-star"
+    }, null, -1)),
     cN = [aN],
-    uN = m("i", {
-        class: "fa-regular fa-calendar"
-    }, null, -1),
-    dN = m("span", {
-        class: "ml-2"
-    }, "plan", -1),
-    fN = [uN, dN],
+    uN = {
+        key: 1
+    },
+    dN = hg(() => m("i", {
+        class: "fa-regular fa-star"
+    }, null, -1)),
+    fN = [dN],
     hN = {
         __name: "MakeCurrentButton",
         props: ["recipe", "loading"],
         setup(t) {
-            return (e, n) => (C(), R("div", iN, [t.recipe.current ? (C(), R("div", oN, [lN, m("button", {
-                class: "button is-small is-rounded is-danger is-outlined",
-                onClick: n[0] || (n[0] = r => e.$emit("cancel"))
-            }, cN)])) : (C(), R("button", {
-                key: 1,
-                class: "button is-small is-rounded",
-                onClick: n[1] || (n[1] = r => e.$emit("plan"))
-            }, fN))]))
+            return (e, n) => (C(), R("span", {
+                class: fe(`star ${t.loading?"loading":""}`),
+                onClick: n[0] || (n[0] = r => e.$emit("favorite"))
+            }, [t.recipe.favorite ? (C(), R("span", lN, cN)) : (C(), R("span", uN, fN))], 2))
         }
-    };
-const pN = {
+    },
+    pN = Be(hN, [
+        ["__scopeId", "data-v-4a24b4e8"]
+    ]);
+const mN = {
         components: {
             Counter: gp,
             RecipeForm: dg,
             ImageUpload: hp,
             LoadingSection: Go,
             NotFound: fg,
             DeleteButton: pp,
-            MakeCurrentButton: hN
+            MakeCurrentButton: pN
         },
         data() {
             return {
                 recipe: null,
                 error: null,
                 portions: 4,
                 editMode: !1,
                 deletePrompt: !1,
                 loading: !1,
                 missingImage: !1,
-                ingredientsCollapsed: !1
+                ingredientsCollapsed: !1,
+                favoriteLoading: !1
             }
         },
         computed: {
             url() {
                 return `${ke.IMAGES_URL}/${this.recipe.id}/medium.jpeg`
             }
         },
@@ -23061,278 +23052,270 @@
                 this.editMode = !this.editMode, this.$refs["look-here"].scrollIntoView(), this.fetchRecipe()
             },
             youSurePrompt() {
                 this.deletePrompt = !this.deletePrompt, this.$refs.yousure.scrollIntoView()
             },
             deleteRecipe() {
                 const t = `${ke.HOST_URL}/recipes/${this.$route.params.id}`;
-                console.info(`Deleting: ${t}`), Le.delete(t).then(() => {
-                    this.$router.push("/recipes")
-                })
+                Fe.delete(t).then(() => this.$router.push("/recipes")).catch(e => console.error(e))
             },
             fetchRecipe() {
                 this.loading = !0;
                 const t = `${ke.HOST_URL}/recipes/${this.$route.params.id}`;
-                console.info(`Getting: ${t}`), Le.get(t).then(e => {
+                Fe.get(t).then(e => {
                     this.recipe = e.data, this.portions = this.recipe.portions
-                }).catch(e => this.error = e).finally(() => this.loading = !1)
-            },
-            makeCurrent() {
-                this.currentLoading = !0;
-                const t = `${ke.HOST_URL}/recipes/current`,
-                    e = {
-                        headers: {
-                            "Content-Type": "application/json"
-                        }
-                    };
-                Le.post(t, {
-                    id: this.recipe.id
-                }, e).then(() => this.recipe.current = !0).catch(n => this.error = n).finally(() => this.currentLoading = !1)
+                }).catch(e => {
+                    this.error = e, console.error(e)
+                }).finally(() => this.loading = !1)
             },
-            cancelCurrent() {
-                this.currentLoading = !0;
-                const t = `${ke.HOST_URL}/recipes/current/${this.recipe.id}`,
+            makeFavorite() {
+                this.favoriteLoading = !0;
+                const t = `${ke.HOST_URL}/recipes/${this.recipe.id}`,
                     e = {
                         headers: {
                             "Content-Type": "application/json"
                         }
+                    },
+                    n = {
+                        ...this.recipe
                     };
-                Le.delete(t, e).then(() => this.recipe.current = !1).catch(n => this.error = n).finally(() => this.currentLoading = !1)
+                n.favorite = !n.favorite, Fe.put(t, n, e).then(r => this.recipe = r.data).catch(r => this.error = r).finally(() => this.favoriteLoading = !1)
             }
         },
         created() {
             this.fetchRecipe()
         }
     },
-    dl = t => (Po("data-v-c8455cc7"), t = t(), $o(), t),
-    mN = {
+    dl = t => (xi("data-v-23c68b68"), t = t(), ki(), t),
+    gN = {
         class: "mx-3 mb-3"
     },
-    gN = {
+    yN = {
         ref: "look-here"
     },
-    yN = {
+    bN = {
         key: 0,
         ref: "recipeTitle"
     },
-    bN = {
+    vN = {
         key: 0
     },
-    vN = {
+    xN = {
         class: "level"
     },
-    xN = {
+    kN = {
         class: "level-left"
     },
-    kN = {
+    wN = {
         class: "level-item"
     },
-    wN = {
+    SN = {
         class: "image",
         style: {
             width: "256px",
             height: "256px"
         }
     },
-    SN = ["src"],
-    _N = {
+    _N = ["src"],
+    CN = {
         class: "level-item"
     },
-    CN = {
+    EN = {
         class: "has-text-centered-mobile title-header"
     },
-    EN = {
+    TN = {
         key: 0,
         class: "title is-4"
     },
-    TN = {
+    ON = {
         key: 1
     },
-    ON = {
+    MN = {
         key: 2
     },
-    MN = ["href"],
-    AN = {
+    AN = ["href"],
+    NN = {
         key: 0
     },
-    NN = {
+    RN = {
         key: 1
     },
-    RN = {
+    DN = {
         class: "tags mt-5"
     },
-    DN = {
+    IN = {
         ref: "chevron",
         class: "tabs is-right is-boxed"
     },
-    IN = {
+    PN = {
         class: "is-active"
     },
-    PN = dl(() => m("i", {
+    $N = dl(() => m("i", {
         class: "fas fa-chevron-down",
         "aria-hidden": "true"
     }, null, -1)),
-    $N = [PN],
-    LN = {
+    LN = [$N],
+    FN = {
         key: 0,
         class: "title is-5"
     },
-    FN = {
+    BN = {
         key: 1,
         class: "px-5"
     },
-    BN = {
+    HN = {
         class: "level-left"
     },
-    HN = {
+    zN = {
         class: "level-item"
     },
-    zN = {
+    VN = {
         key: 0
     },
-    VN = {
+    jN = {
         class: "level-right"
     },
-    jN = {
+    UN = {
         class: "level-item"
     },
-    UN = {
+    WN = {
         class: "my-5"
     },
-    WN = {
+    qN = {
         class: "label"
     },
-    qN = dl(() => m("hr", null, null, -1)),
-    KN = {
+    KN = dl(() => m("hr", null, null, -1)),
+    JN = {
         class: "title is-5"
     },
-    JN = ["innerHTML"],
-    GN = {
+    GN = ["innerHTML"],
+    YN = {
         key: 1,
         class: "my-5"
     },
-    YN = {
-        class: "field is-grouped"
-    },
     XN = {
-        class: "control mx-1"
+        class: "field is-grouped"
     },
     QN = {
         class: "control mx-1"
     },
     ZN = {
+        class: "control mx-1"
+    },
+    eR = {
         class: "control mx-1 is-expanded"
     },
-    eR = dl(() => m("i", {
+    tR = dl(() => m("i", {
         class: "fas fa-pen"
     }, null, -1)),
-    tR = dl(() => m("span", {
+    nR = dl(() => m("span", {
         class: "ml-2"
     }, "Edit", -1)),
-    nR = [eR, tR],
-    rR = {
+    rR = [tR, nR],
+    sR = {
         key: 2
     };
 
-function sR(t, e, n, r, s, i) {
+function iR(t, e, n, r, s, i) {
     const o = Oe("MakeCurrentButton"),
         l = Oe("router-link"),
         a = Oe("Counter"),
         c = Oe("DeleteButton"),
         u = Oe("ImageUpload"),
         d = Oe("RecipeForm"),
         f = Oe("LoadingSection"),
         h = Oe("NotFound");
-    return C(), R("div", mN, [m("div", gN, null, 512), ce(rn, {
+    return C(), R("div", gN, [m("div", yN, null, 512), ce(rn, {
         name: "loading",
         mode: "out-in"
     }, {
-        default: ht(() => [s.recipe ? (C(), R("div", yN, [s.editMode ? re("", !0) : (C(), R("div", bN, [m("div", vN, [m("div", xN, [We(m("div", kN, [m("p", wN, [m("img", {
+        default: ht(() => [s.recipe ? (C(), R("div", bN, [s.editMode ? re("", !0) : (C(), R("div", vN, [m("div", xN, [m("div", kN, [We(m("div", wN, [m("p", SN, [m("img", {
             ref: "r-img",
             src: i.url,
             onError: e[0] || (e[0] = p => s.missingImage = !0),
             alt: "recipe image",
             class: "is-rounded p-2"
-        }, null, 40, SN)])], 512), [
+        }, null, 40, _N)])], 512), [
             [_l, !s.missingImage]
-        ]), m("div", _N, [m("div", CN, [s.recipe ? (C(), R("h1", EN, le(s.recipe.title), 1)) : re("", !0), s.recipe && s.recipe.subtitle ? (C(), R("h2", TN, le(s.recipe.subtitle), 1)) : re("", !0), s.recipe && s.recipe.source ? (C(), R("p", ON, [m("a", {
+        ]), m("div", CN, [m("div", EN, [s.recipe ? (C(), R("h1", TN, le(s.recipe.title), 1)) : re("", !0), s.recipe && s.recipe.subtitle ? (C(), R("h2", ON, le(s.recipe.subtitle), 1)) : re("", !0), s.recipe && s.recipe.source ? (C(), R("p", MN, [m("a", {
             href: s.recipe.source
-        }, [s.recipe.source_name ? (C(), R("span", AN, le(s.recipe.source_name), 1)) : (C(), R("span", NN, le(s.recipe.source), 1))], 8, MN)])) : re("", !0)])])])]), m("div", RN, [(C(!0), R(Fe, null, Dt(s.recipe.tags, (p, g) => (C(), R("span", {
+        }, [s.recipe.source_name ? (C(), R("span", NN, le(s.recipe.source_name), 1)) : (C(), R("span", RN, le(s.recipe.source), 1))], 8, AN)])) : re("", !0)])])])]), m("div", DN, [ce(o, {
+            recipe: s.recipe,
+            loading: s.favoriteLoading,
+            onFavorite: i.makeFavorite,
+            onCancel: t.cancelCurrent,
+            class: "mr-2"
+        }, null, 8, ["recipe", "loading", "onFavorite", "onCancel"]), (C(!0), R(Le, null, Dt(s.recipe.tags, (p, g) => (C(), R("span", {
             class: "tag",
             key: "item-tag-" + g
-        }, le(p.name), 1))), 128))]), ce(o, {
-            recipe: s.recipe,
-            onPlan: i.makeCurrent,
-            onCancel: i.cancelCurrent,
-            loading: t.currentLoading
-        }, null, 8, ["recipe", "onPlan", "onCancel", "loading"]), m("div", DN, [m("ul", null, [m("li", IN, [m("a", {
+        }, le(p.name), 1))), 128))]), m("div", IN, [m("ul", null, [m("li", PN, [m("a", {
             onClick: e[1] || (e[1] = p => s.ingredientsCollapsed = !s.ingredientsCollapsed)
         }, [m("span", {
-            class: he({
+            class: fe({
                 icon: !0,
                 "is-small": !0,
                 rotate: s.ingredientsCollapsed,
                 "animate-icon": !0
             })
-        }, $N, 2)])])])], 512), ce(rn, {
+        }, LN, 2)])])])], 512), ce(rn, {
             name: "slide-up"
         }, {
-            default: ht(() => [We(m("div", null, [s.recipe ? (C(), R("h1", LN, "Ingredients")) : re("", !0), s.recipe && s.recipe.ingredients ? (C(), R("div", FN, [(C(!0), R(Fe, null, Dt(s.recipe.ingredients, (p, g) => (C(), R("div", {
+            default: ht(() => [We(m("div", null, [s.recipe ? (C(), R("h1", FN, "Ingredients")) : re("", !0), s.recipe && s.recipe.ingredients ? (C(), R("div", BN, [(C(!0), R(Le, null, Dt(s.recipe.ingredients, (p, g) => (C(), R("div", {
                 key: p + g + "recipe-detail",
                 class: "level is-mobile"
-            }, [m("div", BN, [m("div", HN, [ce(l, {
+            }, [m("div", HN, [m("div", zN, [ce(l, {
                 to: {
                     name: "Ingredient",
                     params: {
                         id: p.ingredient.id
                     }
                 }
             }, {
-                default: ht(() => [Ge(le(p.ingredient.name) + " ", 1), p.note ? (C(), R("span", zN, "(" + le(p.note) + ")", 1)) : re("", !0)]),
+                default: ht(() => [Ge(le(p.ingredient.name) + " ", 1), p.note ? (C(), R("span", VN, "(" + le(p.note) + ")", 1)) : re("", !0)]),
                 _: 2
-            }, 1032, ["to"])])]), m("div", VN, [m("div", jN, [m("p", null, [m("strong", null, le(Math.round(p.amount * s.portions / s.recipe.portions * 10) / 10), 1), Ge(" " + le(p.unit.name), 1)])])])]))), 128))])) : re("", !0), m("div", UN, [ce(a, {
+            }, 1032, ["to"])])]), m("div", jN, [m("div", UN, [m("p", null, [m("strong", null, le(Math.round(p.amount * s.portions / s.recipe.portions * 10) / 10), 1), Ge(" " + le(p.unit.name), 1)])])])]))), 128))])) : re("", !0), m("div", WN, [ce(a, {
                 initialValue: s.recipe.portions,
                 onCounterUpdate: i.updatePortions
-            }, null, 8, ["initialValue", "onCounterUpdate"]), m("label", WN, "Enough for " + le(Math.round(s.portions / s.recipe.portions * 10) / 10) + " batch(es).", 1)]), qN], 512), [
+            }, null, 8, ["initialValue", "onCounterUpdate"]), m("label", qN, "Enough for " + le(Math.round(s.portions / s.recipe.portions * 10) / 10) + " batch(es).", 1)]), KN], 512), [
                 [_l, !s.ingredientsCollapsed]
             ])]),
             _: 1
-        }), We(m("h1", KN, "Steps", 512), [
+        }), We(m("h1", JN, "Steps", 512), [
             [_l, s.recipe]
         ]), m("div", {
             innerHTML: s.recipe.body,
             class: "content section pt-1"
-        }, null, 8, JN)])), s.editMode ? re("", !0) : (C(), R("div", GN, [m("div", YN, [m("p", XN, [ce(c, {
+        }, null, 8, GN)])), s.editMode ? re("", !0) : (C(), R("div", YN, [m("div", XN, [m("p", QN, [ce(c, {
             onDelete: i.deleteRecipe
-        }, null, 8, ["onDelete"])]), m("p", QN, [ce(u, {
+        }, null, 8, ["onDelete"])]), m("p", ZN, [ce(u, {
             recipe: s.recipe,
             onUploadSuccess: e[2] || (e[2] = p => t.$router.go(t.$router.currentRoute))
-        }, null, 8, ["recipe"])]), m("p", ZN, [m("button", {
+        }, null, 8, ["recipe"])]), m("p", eR, [m("button", {
             onClick: e[3] || (e[3] = (...p) => i.updateRecipe && i.updateRecipe(...p)),
             class: "button is-fullwidth is-warning mb-1"
-        }, nR)])])])), s.editMode ? (C(), R("div", rR, [ce(d, {
+        }, rR)])])])), s.editMode ? (C(), R("div", sR, [ce(d, {
             recipe: s.recipe,
             onRecipePosted: i.updateRecipe,
             onCancel: e[4] || (e[4] = p => s.editMode = !1)
         }, null, 8, ["recipe", "onRecipePosted"])])) : re("", !0)], 512)) : s.loading ? (C(), yt(f, {
             key: 1,
             class: "p-5",
             loading: s.loading
         }, null, 8, ["loading"])) : (C(), yt(h, {
             key: 2,
             message: "Recipe not found"
         }))]),
         _: 1
     })])
 }
-const iR = Ue(pN, [
-    ["render", sR],
-    ["__scopeId", "data-v-c8455cc7"]
+const oR = Be(mN, [
+    ["render", iR],
+    ["__scopeId", "data-v-23c68b68"]
 ]);
-const oR = {
+const lR = {
         components: {
             CategoryTile: mp,
             RecipeList: Ec,
             LoadingSection: Go
         },
         data() {
             return {
@@ -23346,52 +23329,52 @@
         },
         methods: {
             edited() {
                 this.getCategory(), this.getRecipes()
             },
             getCategory() {
                 const t = `${ke.HOST_URL}/categories/${this.$route.params.id}`;
-                this.loadingCategory = !0, Le.get(t).then(e => this.category = e.data).catch(() => this.errorCategory = "Category NOT found").finally(() => this.loadingCategory = !1)
+                this.loadingCategory = !0, Fe.get(t).then(e => this.category = e.data).catch(() => this.errorCategory = "Category NOT found").finally(() => this.loadingCategory = !1)
             },
             getRecipes() {
                 const t = `${ke.HOST_URL}/recipes?category=${this.$route.params.id}`;
-                this.loadingRecipes = !0, Le.get(t).then(e => this.recipes = e.data).catch(() => this.errorRecipes = "Error occured while fetching recipes.").finally(() => this.loadingRecipes = !1)
+                this.loadingRecipes = !0, Fe.get(t).then(e => this.recipes = e.data).catch(() => this.errorRecipes = "Error occured while fetching recipes.").finally(() => this.loadingRecipes = !1)
             }
         },
         created() {
             this.getCategory(), this.getRecipes()
         }
     },
-    lR = {
-        key: 0
-    },
     aR = {
-        class: "message is-danger my-5"
+        key: 0
     },
     cR = {
-        class: "message-body"
+        class: "message is-danger my-5"
     },
     uR = {
-        key: 1
+        class: "message-body"
     },
     dR = {
         key: 1
     },
     fR = {
-        class: "message is-danger my-5"
+        key: 1
     },
     hR = {
-        class: "message-body"
+        class: "message is-danger my-5"
     },
     pR = {
+        class: "message-body"
+    },
+    mR = {
         key: 2,
         class: "px-2 pt-3 recipe-list"
     };
 
-function mR(t, e, n, r, s, i) {
+function gR(t, e, n, r, s, i) {
     const o = Oe("LoadingSection"),
         l = Oe("CategoryTile"),
         a = Oe("RecipeList");
     return C(), R("div", null, [ce(rn, {
         name: "loading",
         mode: "out-in"
     }, {
@@ -23404,61 +23387,61 @@
             editable: !0,
             onCategoryDeleted: e[0] || (e[0] = c => t.$router.push({
                 name: "home"
             })),
             onCategoryEdited: i.edited
         }, null, 8, ["category", "onCategoryEdited"]))]),
         _: 1
-    }), s.errorCategory ? (C(), R("div", lR, [m("article", aR, [m("div", cR, le(s.errorCategory), 1)])])) : (C(), R("div", uR, [ce(rn, {
+    }), s.errorCategory ? (C(), R("div", aR, [m("article", cR, [m("div", uR, le(s.errorCategory), 1)])])) : (C(), R("div", dR, [ce(rn, {
         name: "loading",
         mode: "out-in"
     }, {
         default: ht(() => [s.loadingRecipes ? (C(), yt(o, {
             key: 0,
             loading: s.loadingRecipes
-        }, null, 8, ["loading"])) : s.errorRecipes ? (C(), R("div", dR, [m("article", fR, [m("div", hR, le(s.errorRecipes), 1)])])) : (C(), R("div", pR, [ce(a, {
+        }, null, 8, ["loading"])) : s.errorRecipes ? (C(), R("div", fR, [m("article", hR, [m("div", pR, le(s.errorRecipes), 1)])])) : (C(), R("div", mR, [ce(a, {
             allRecipes: s.recipes
         }, null, 8, ["allRecipes"])]))]),
         _: 1
     })]))])
 }
-const gR = Ue(oR, [
-        ["render", mR],
+const yR = Be(lR, [
+        ["render", gR],
         ["__scopeId", "data-v-5bc2c90f"]
     ]),
-    yR = {
+    bR = {
         components: {
             CategoryForm: fp
         }
     },
-    bR = {
+    vR = {
         class: "px-3"
     },
-    vR = m("h1", {
+    xR = m("h1", {
         class: "title is-3"
     }, "Add", -1),
-    xR = m("h2", {
+    kR = m("h2", {
         class: "subtitle is-5"
     }, "a new category", -1);
 
-function kR(t, e, n, r, s, i) {
+function wR(t, e, n, r, s, i) {
     const o = Oe("CategoryForm");
-    return C(), R("div", bR, [vR, xR, ce(o, {
+    return C(), R("div", vR, [xR, kR, ce(o, {
         onCategoryPosted: e[0] || (e[0] = l => t.$router.push({
             name: "home"
         })),
         onCancel: e[1] || (e[1] = l => t.$router.push({
             name: "home"
         }))
     })])
 }
-const wR = Ue(yR, [
-        ["render", kR]
+const SR = Be(bR, [
+        ["render", wR]
     ]),
-    SR = {
+    _R = {
         components: {
             RecipeForm: dg
         },
         data() {
             return {
                 recipe: {
                     portions: 4,
@@ -23475,38 +23458,38 @@
                     params: {
                         id: t.id
                     }
                 })
             }
         }
     },
-    _R = {
+    CR = {
         class: "px-3"
     },
-    CR = m("h1", {
+    ER = m("h1", {
         class: "title is-3"
     }, "Add", -1),
-    ER = m("h2", {
+    TR = m("h2", {
         class: "subtitle is-5"
     }, "a new recipe", -1);
 
-function TR(t, e, n, r, s, i) {
+function OR(t, e, n, r, s, i) {
     const o = Oe("RecipeForm");
-    return C(), R("div", _R, [CR, ER, ce(o, {
+    return C(), R("div", CR, [ER, TR, ce(o, {
         recipe: s.recipe,
         onRecipePosted: i.routeToNewRecipe,
         onCancel: e[0] || (e[0] = l => t.$router.push({
             name: "home"
         }))
     }, null, 8, ["recipe", "onRecipePosted"])])
 }
-const OR = Ue(SR, [
-        ["render", TR]
+const MR = Be(_R, [
+        ["render", OR]
     ]),
-    MR = {
+    AR = {
         props: ["ingredientProp"],
         data() {
             return {
                 postError: null,
                 ingredient: {}
             }
         },
@@ -23520,357 +23503,354 @@
             post() {
                 const t = `${ke.HOST_URL}/ingredients/${this.ingredient.id}`,
                     e = {
                         headers: {
                             "Content-Type": "application/json"
                         }
                     };
-                Le.post(t, this.ingredient, e).then(n => {
+                Fe.post(t, this.ingredient, e).then(n => {
                     this.postSuccess = `${n.status} ${n.statusText}`, this.$emit("posted", this.ingredient)
                 }).catch(n => {
                     this.postError = n.response.data
                 })
             }
         },
         mounted() {
             this.ingredientProp && (this.ingredient = {
                 ...this.ingredientProp
             })
         }
     },
-    AR = {
+    NR = {
         class: "field"
     },
-    NR = {
+    RR = {
         class: "control has-icons-left has-icons-right"
     },
-    RR = m("span", {
+    DR = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-font"
     })], -1),
-    DR = {
+    IR = {
         class: "control has-icons-left is-expanded"
     },
-    IR = m("span", {
+    PR = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-charging-station"
     })], -1),
-    PR = m("p", {
+    $R = m("p", {
         class: "control"
     }, [m("a", {
         class: "button is-static"
     }, "kcal / 100g")], -1),
-    $R = {
+    LR = {
         key: 0,
         class: "help is-danger mt-0"
     },
-    LR = {
+    FR = {
         class: "control has-icons-left is-expanded"
     },
-    FR = m("span", {
+    BR = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-pizza-slice"
     })], -1),
-    BR = m("p", {
+    HR = m("p", {
         class: "control"
     }, [m("a", {
         class: "button is-static"
     }, "g / 100g")], -1),
-    HR = {
+    zR = {
         key: 1,
         class: "help is-danger mt-0"
     },
-    zR = {
+    VR = {
         class: "control has-icons-left is-expanded"
     },
-    VR = m("span", {
+    jR = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-bacon"
     })], -1),
-    jR = m("p", {
+    UR = m("p", {
         class: "control"
     }, [m("a", {
         class: "button is-static"
     }, "g / 100g")], -1),
-    UR = {
+    WR = {
         key: 2,
         class: "help is-danger mt-0"
     },
-    WR = {
+    qR = {
         class: "control has-icons-left is-expanded"
     },
-    qR = m("span", {
+    KR = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-drumstick-bite"
     })], -1),
-    KR = m("p", {
+    JR = m("p", {
         class: "control"
     }, [m("a", {
         class: "button is-static"
     }, "g / 100g")], -1),
-    JR = {
+    GR = {
         key: 3,
         class: "help is-danger mt-0"
     },
-    GR = {
+    YR = {
         class: "control has-icons-left is-expanded"
     },
-    YR = m("span", {
+    XR = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-seedling"
     })], -1),
-    XR = m("p", {
+    QR = m("p", {
         class: "control"
     }, [m("a", {
         class: "button is-static"
     }, "g / 100g")], -1),
-    QR = {
+    ZR = {
         key: 4,
         class: "help is-danger mt-0"
     },
-    ZR = {
+    eD = {
         class: "control has-icons-left is-expanded"
     },
-    eD = m("span", {
+    tD = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-hand-spock"
     })], -1),
-    tD = m("p", {
+    nD = m("p", {
         class: "control"
     }, [m("a", {
         class: "button is-static"
     }, "g / 100g")], -1),
-    nD = {
+    rD = {
         key: 5,
         class: "help is-danger mt-0"
     },
-    rD = {
+    sD = {
         key: 6,
         class: "message is-danger"
     },
-    sD = {
+    iD = {
         class: "message-body"
     },
-    iD = {
+    oD = {
         class: "field has-addons"
     },
-    oD = {
+    lD = {
         class: "control is-expanded"
     },
-    lD = m("i", {
+    aD = m("i", {
         class: "fas fa-save"
     }, null, -1),
-    aD = m("span", {
+    cD = m("span", {
         class: "ml-2"
     }, "Save", -1),
-    cD = [lD, aD],
-    uD = {
+    uD = [aD, cD],
+    dD = {
         class: "control is-expanded"
     },
-    dD = m("i", {
+    fD = m("i", {
         class: "fas fa-times"
     }, null, -1),
-    fD = m("span", {
+    hD = m("span", {
         class: "ml-2"
     }, "Cancel", -1),
-    hD = [dD, fD];
+    pD = [fD, hD];
 
-function pD(t, e, n, r, s, i) {
-    return C(), R("div", null, [m("div", AR, [m("div", NR, [We(m("input", {
+function mD(t, e, n, r, s, i) {
+    return C(), R("div", null, [m("div", NR, [m("div", RR, [We(m("input", {
         "onUpdate:modelValue": e[0] || (e[0] = o => s.ingredient.name = o),
         class: "input",
         type: "text",
         placeholder: "name"
     }, null, 512), [
         [st, s.ingredient.name]
-    ]), RR])]), m("div", {
-        class: he({
+    ]), DR])]), m("div", {
+        class: fe({
             field: !0,
             "has-addons": !0,
             "mb-0": isNaN(parseFloat(s.ingredient.energy))
         })
-    }, [m("div", DR, [We(m("input", {
+    }, [m("div", IR, [We(m("input", {
         "onUpdate:modelValue": e[1] || (e[1] = o => s.ingredient.energy = o),
         type: "number",
-        class: he({
+        class: fe({
             input: !0,
             "is-danger": isNaN(parseFloat(s.ingredient.energy))
         }),
         placeholder: "energy"
     }, null, 2), [
         [st, s.ingredient.energy, void 0, {
             number: !0
         }]
-    ]), IR]), PR], 2), isNaN(parseFloat(s.ingredient.energy)) ? (C(), R("p", $R, "Must be a number...")) : re("", !0), m("div", {
-        class: he({
+    ]), PR]), $R], 2), isNaN(parseFloat(s.ingredient.energy)) ? (C(), R("p", LR, "Must be a number...")) : re("", !0), m("div", {
+        class: fe({
             field: !0,
             "has-addons": !0,
             "mb-0": isNaN(parseFloat(s.ingredient.carbs))
         })
-    }, [m("div", LR, [We(m("input", {
+    }, [m("div", FR, [We(m("input", {
         "onUpdate:modelValue": e[2] || (e[2] = o => s.ingredient.carbs = o),
-        class: he({
+        class: fe({
             input: !0,
             "is-danger": isNaN(parseFloat(s.ingredient.carbs))
         }),
         placeholder: "carbs"
     }, null, 2), [
         [st, s.ingredient.carbs]
-    ]), FR]), BR], 2), isNaN(parseFloat(s.ingredient.carbs)) ? (C(), R("p", HR, "Must be a number...")) : re("", !0), m("div", {
-        class: he({
+    ]), BR]), HR], 2), isNaN(parseFloat(s.ingredient.carbs)) ? (C(), R("p", zR, "Must be a number...")) : re("", !0), m("div", {
+        class: fe({
             field: !0,
             "has-addons": !0,
             "mb-0": isNaN(parseFloat(s.ingredient.fats))
         })
-    }, [m("div", zR, [We(m("input", {
+    }, [m("div", VR, [We(m("input", {
         "onUpdate:modelValue": e[3] || (e[3] = o => s.ingredient.fats = o),
-        class: he({
+        class: fe({
             input: !0,
             "is-danger": isNaN(parseFloat(s.ingredient.fats))
         }),
         placeholder: "fats"
     }, null, 2), [
         [st, s.ingredient.fats]
-    ]), VR]), jR], 2), isNaN(parseFloat(s.ingredient.fats)) ? (C(), R("p", UR, "Must be a number...")) : re("", !0), m("div", {
-        class: he({
+    ]), jR]), UR], 2), isNaN(parseFloat(s.ingredient.fats)) ? (C(), R("p", WR, "Must be a number...")) : re("", !0), m("div", {
+        class: fe({
             field: !0,
             "has-addons": !0,
             "mb-0": isNaN(parseFloat(s.ingredient.proteins))
         })
-    }, [m("div", WR, [We(m("input", {
+    }, [m("div", qR, [We(m("input", {
         "onUpdate:modelValue": e[4] || (e[4] = o => s.ingredient.proteins = o),
-        class: he({
+        class: fe({
             input: !0,
             "is-danger": isNaN(parseFloat(s.ingredient.proteins))
         }),
         placeholder: "proteins"
     }, null, 2), [
         [st, s.ingredient.proteins]
-    ]), qR]), KR], 2), isNaN(parseFloat(s.ingredient.proteins)) ? (C(), R("p", JR, "Must be a number...")) : re("", !0), m("div", {
-        class: he({
+    ]), KR]), JR], 2), isNaN(parseFloat(s.ingredient.proteins)) ? (C(), R("p", GR, "Must be a number...")) : re("", !0), m("div", {
+        class: fe({
             field: !0,
             "has-addons": !0,
             "mb-0": isNaN(parseFloat(s.ingredient.fibres))
         })
-    }, [m("div", GR, [We(m("input", {
+    }, [m("div", YR, [We(m("input", {
         "onUpdate:modelValue": e[5] || (e[5] = o => s.ingredient.fibres = o),
-        class: he({
+        class: fe({
             input: !0,
             "is-danger": isNaN(parseFloat(s.ingredient.fibres))
         }),
         placeholder: "fibres"
     }, null, 2), [
         [st, s.ingredient.fibres]
-    ]), YR]), XR], 2), isNaN(parseFloat(s.ingredient.fibres)) ? (C(), R("p", QR, "Must be a number...")) : re("", !0), m("div", {
-        class: he({
+    ]), XR]), QR], 2), isNaN(parseFloat(s.ingredient.fibres)) ? (C(), R("p", ZR, "Must be a number...")) : re("", !0), m("div", {
+        class: fe({
             field: !0,
             "has-addons": !0,
             "mb-0": isNaN(parseFloat(s.ingredient.salt))
         })
-    }, [m("div", ZR, [We(m("input", {
+    }, [m("div", eD, [We(m("input", {
         "onUpdate:modelValue": e[6] || (e[6] = o => s.ingredient.salt = o),
-        class: he({
+        class: fe({
             input: !0,
             "is-danger": isNaN(parseFloat(s.ingredient.salt))
         }),
         placeholder: "salt"
     }, null, 2), [
         [st, s.ingredient.salt]
-    ]), eD]), tD], 2), isNaN(parseFloat(s.ingredient.salt)) ? (C(), R("p", nD, "Must be a number...")) : re("", !0), s.postError ? (C(), R("article", rD, [m("div", sD, le(s.postError), 1)])) : re("", !0), m("div", iD, [m("p", oD, [m("a", {
+    ]), tD]), nD], 2), isNaN(parseFloat(s.ingredient.salt)) ? (C(), R("p", rD, "Must be a number...")) : re("", !0), s.postError ? (C(), R("article", sD, [m("div", iD, le(s.postError), 1)])) : re("", !0), m("div", oD, [m("p", lD, [m("a", {
         onClick: e[7] || (e[7] = (...o) => i.save && i.save(...o)),
         class: "button is-fullwidth is-success"
-    }, cD)]), m("p", uD, [m("a", {
+    }, uD)]), m("p", dD, [m("a", {
         onClick: e[8] || (e[8] = (...o) => i.cancel && i.cancel(...o)),
         class: "button is-fullwidth is-danger"
-    }, hD)])])])
+    }, pD)])])])
 }
-const hg = Ue(MR, [
-        ["render", pD]
+const pg = Be(AR, [
+        ["render", mD]
     ]),
-    mD = {
+    gD = {
         components: {
-            IngredientForm: hg
+            IngredientForm: pg
         },
         props: ["ingredient"],
         data() {
             return {
                 error: null,
                 edit: !1
             }
         },
         methods: {
             posted(t) {
                 this.ingredient = t, this.edit = !1
             },
             deleteIngredient() {
                 const t = `${ke.HOST_URL}/ingredients/${this.ingredient.id}`;
-                console.info(`Deleting: ${t}`), Le.delete(t).then(() => {
+                Fe.delete(t).then(() => {
                     this.$emit("ingredientDeleted")
                 }).catch(e => {
                     this.error = `${e.response.data}.`
                 })
             }
         }
     },
-    gD = {
+    yD = {
         class: "box m-0 my-1 p-4"
     },
-    yD = {
+    bD = {
         class: "level is-mobile my-1"
     },
-    bD = {
+    vD = {
         class: "level-left"
     },
-    vD = {
+    xD = {
         class: "level-item"
     },
-    xD = {
+    kD = {
         class: "title is-5"
     },
-    kD = {
+    wD = {
         class: "level-right"
     },
-    wD = {
+    SD = {
         key: 0,
         class: "level-item"
     },
-    SD = m("span", {
+    _D = m("span", {
         class: "icon"
     }, [m("i", {
         class: "fas fa-trash"
     })], -1),
-    _D = [SD],
-    CD = {
+    CD = [_D],
+    ED = {
         class: "level-item"
     },
-    ED = m("span", {
+    TD = m("span", {
         class: "icon"
     }, [m("i", {
         class: "fas fa-pen"
     })], -1),
-    TD = [ED],
-    OD = {
+    OD = [TD],
+    MD = {
         key: 0,
         class: "level mt-3 mb-0 py-0"
     },
-    MD = {
-        class: "level-left"
-    },
     AD = {
-        class: "tags my-0"
+        class: "level-left"
     },
     ND = {
-        class: "tag"
+        class: "tags my-0"
     },
     RD = {
         class: "tag"
     },
     DD = {
         class: "tag"
     },
@@ -23880,281 +23860,286 @@
     PD = {
         class: "tag"
     },
     $D = {
         class: "tag"
     },
     LD = {
+        class: "tag"
+    },
+    FD = {
         key: 1,
         class: "level-item"
     },
-    FD = {
+    BD = {
         class: "help is-danger"
     },
-    BD = {
+    HD = {
         key: 2
     },
-    HD = m("hr", null, null, -1);
+    zD = m("hr", null, null, -1);
 
-function zD(t, e, n, r, s, i) {
+function VD(t, e, n, r, s, i) {
     const o = Oe("IngredientForm");
-    return C(), R("div", gD, [m("nav", yD, [m("div", bD, [m("div", vD, [m("p", xD, le(n.ingredient.name.toUpperCase()), 1)])]), m("div", kD, [s.error ? re("", !0) : (C(), R("div", wD, [m("button", {
+    return C(), R("div", yD, [m("nav", bD, [m("div", vD, [m("div", xD, [m("p", kD, le(n.ingredient.name.toUpperCase()), 1)])]), m("div", wD, [s.error ? re("", !0) : (C(), R("div", SD, [m("button", {
         onClick: e[0] || (e[0] = l => i.deleteIngredient()),
         class: "button has-icons is-danger"
-    }, _D)])), m("div", CD, [m("button", {
+    }, CD)])), m("div", ED, [m("button", {
         onClick: e[1] || (e[1] = l => s.edit = !s.edit),
         class: "button has-icons is-warning"
-    }, TD)])])]), s.edit ? re("", !0) : (C(), R("nav", OD, [m("div", MD, [m("div", AD, [m("span", ND, [Ge("energy: "), m("strong", null, le(n.ingredient.energy) + " kcal", 1)]), m("span", RD, [Ge("carbs: "), m("strong", null, le(n.ingredient.carbs) + " g", 1)]), m("span", DD, [Ge("fats: "), m("strong", null, le(n.ingredient.fats) + " g", 1)]), m("span", ID, [Ge("protein: "), m("strong", null, le(n.ingredient.proteins) + " g", 1)]), m("span", PD, [Ge("fibers: "), m("strong", null, le(n.ingredient.fibres) + " g", 1)]), m("span", $D, [Ge("salt: "), m("strong", null, le(n.ingredient.salt) + " g", 1)])])])])), s.error ? (C(), R("div", LD, [m("p", FD, le(s.error), 1)])) : re("", !0), s.edit ? (C(), R("div", BD, [HD, ce(o, {
+    }, OD)])])]), s.edit ? re("", !0) : (C(), R("nav", MD, [m("div", AD, [m("div", ND, [m("span", RD, [Ge("energy: "), m("strong", null, le(n.ingredient.energy) + " kcal", 1)]), m("span", DD, [Ge("carbs: "), m("strong", null, le(n.ingredient.carbs) + " g", 1)]), m("span", ID, [Ge("fats: "), m("strong", null, le(n.ingredient.fats) + " g", 1)]), m("span", PD, [Ge("protein: "), m("strong", null, le(n.ingredient.proteins) + " g", 1)]), m("span", $D, [Ge("fibers: "), m("strong", null, le(n.ingredient.fibres) + " g", 1)]), m("span", LD, [Ge("salt: "), m("strong", null, le(n.ingredient.salt) + " g", 1)])])])])), s.error ? (C(), R("div", FD, [m("p", BD, le(s.error), 1)])) : re("", !0), s.edit ? (C(), R("div", HD, [zD, ce(o, {
         ingredientProp: n.ingredient,
         onCancel: e[2] || (e[2] = l => s.edit = !1),
         onPosted: i.posted
     }, null, 8, ["ingredientProp", "onPosted"])])) : re("", !0)])
 }
-const VD = Ue(mD, [
-        ["render", zD]
+const jD = Be(gD, [
+        ["render", VD]
     ]),
-    jD = {
+    UD = {
         data() {
             return {
                 allIngredients: [],
                 ingredients: [],
                 error: null,
                 search: null
             }
         },
         components: {
-            IngredientListItem: VD
+            IngredientListItem: jD
         },
         methods: {
             refresh() {
                 if (this.ingredients = this.allIngredients, !(!this.search || this.search === "")) {
                     var t = new RegExp(ke.methods.replaceUnicode(this.search.toLowerCase()));
                     this.ingredients = this.allIngredients.filter(e => {
                         var n = t.exec(ke.methods.replaceUnicode(e.name.toLowerCase()));
                         return !!n
                     })
                 }
             },
             reload() {
                 const t = `${ke.HOST_URL}/ingredients`;
-                Le.get(t).then(e => {
+                Fe.get(t).then(e => {
                     e.status !== "success" && e.data && (this.ingredients = e.data, this.allIngredients = e.data)
                 }).catch(e => this.error = e)
             }
         },
         created() {
             this.reload()
         }
     },
-    UD = {
+    WD = {
         class: "title is-4"
     },
-    WD = {
+    qD = {
         class: "control has-icons-left"
     },
-    qD = m("span", {
+    KD = m("span", {
         class: "icon is-small is-left"
     }, [m("i", {
         class: "fas fa-search"
     })], -1),
-    KD = {
+    JD = {
         class: "section px-3 pt-4"
     };
 
-function JD(t, e, n, r, s, i) {
+function GD(t, e, n, r, s, i) {
     const o = Oe("IngredientListItem");
-    return C(), R("div", null, [m("h1", UD, le(s.ingredients.length) + " Ingredients", 1), m("p", WD, [We(m("input", {
+    return C(), R("div", null, [m("h1", WD, le(s.ingredients.length) + " Ingredients", 1), m("p", qD, [We(m("input", {
         "onUpdate:modelValue": e[0] || (e[0] = l => s.search = l),
         onInput: e[1] || (e[1] = (...l) => i.refresh && i.refresh(...l)),
         class: "input is-rounded",
         type: "text",
         placeholder: "search"
     }, null, 544), [
         [st, s.search]
-    ]), qD]), m("div", KD, [(C(!0), R(Fe, null, Dt(s.ingredients, (l, a) => (C(), yt(o, {
+    ]), KD]), m("div", JD, [(C(!0), R(Le, null, Dt(s.ingredients, (l, a) => (C(), yt(o, {
         key: l + a + "list",
         ingredient: l,
         onIngredientDeleted: e[2] || (e[2] = c => {
             i.reload(), i.refresh()
         })
     }, null, 8, ["ingredient"]))), 128))])])
 }
-const GD = Ue(jD, [
-        ["render", JD]
+const YD = Be(UD, [
+        ["render", GD]
     ]),
-    YD = {
+    XD = {
         components: {
-            IngredientForm: hg,
+            IngredientForm: pg,
             NotFound: fg
         },
         data() {
             return {
                 ingredient: null,
                 error: null,
                 edit: !1,
                 attributes: {}
             }
         },
         methods: {
             fetchIngredient() {
                 const t = `${ke.HOST_URL}/ingredients/${this.$route.params.id}`;
-                console.info(`Getting: ${t}`), Le.get(t).then(e => {
+                Fe.get(t).then(e => {
                     e.status !== "success" && e.data && (this.ingredient = e.data, this.attributes = {
                         energy: `${this.ingredient.energy} kcal`,
                         carbs: `${this.ingredient.carbs} g`,
                         fats: `${this.ingredient.fats} g`,
                         proteins: `${this.ingredient.proteins} g`,
                         fibres: `${this.ingredient.fibres} g`,
                         salt: `${this.ingredient.salt} g`
                     })
-                }).catch(e => this.error = e)
+                }).catch(e => {
+                    this.error = e, console.error(e)
+                })
             },
             deleteIngredient() {
                 const t = `${ke.HOST_URL}/ingredients/${this.ingredient.id}`;
-                console.info(`Deleting: ${t}`), Le.delete(t).then(() => {
+                Fe.delete(t).then(() => {
                     this.$emit("ingredientDeleted")
                 }).catch(e => {
-                    this.error = `${e.response.data}.`
+                    this.error = `${e.response.data}.`, console.error(e)
                 })
             }
         },
         created() {
             this.fetchIngredient()
         }
     },
-    XD = {
+    QD = {
         key: 0
     },
-    QD = {
+    ZD = {
         key: 0,
         class: "level-item"
     },
-    ZD = {
+    eI = {
         class: "help is-danger"
     },
-    eI = {
+    tI = {
         class: "level is-mobile my-1"
     },
-    tI = {
+    nI = {
         class: "level-left"
     },
-    nI = {
+    rI = {
         class: "level-item"
     },
-    rI = {
+    sI = {
         class: "title is-5"
     },
-    sI = {
+    iI = {
         class: "level-right"
     },
-    iI = {
+    oI = {
         key: 0,
         class: "level-item"
     },
-    oI = m("span", {
+    lI = m("span", {
         class: "icon"
     }, [m("i", {
         class: "fas fa-trash"
     })], -1),
-    lI = [oI],
-    aI = {
+    aI = [lI],
+    cI = {
         class: "level-item"
     },
-    cI = m("span", {
+    uI = m("span", {
         class: "icon"
     }, [m("i", {
         class: "fas fa-pen"
     })], -1),
-    uI = [cI],
-    dI = m("hr", null, null, -1),
-    fI = {
+    dI = [uI],
+    fI = m("hr", null, null, -1),
+    hI = {
         key: 1
     },
-    hI = {
+    pI = {
         class: "level-left"
     },
-    pI = {
+    mI = {
         class: "level-item"
     },
-    mI = {
+    gI = {
         class: "tag"
     },
-    gI = {
+    yI = {
         class: "level-right"
     },
-    yI = {
+    bI = {
         class: "level-item"
     },
-    bI = {
+    vI = {
         key: 2
     },
-    vI = {
+    xI = {
         key: 1
     };
 
-function xI(t, e, n, r, s, i) {
+function kI(t, e, n, r, s, i) {
     const o = Oe("IngredientForm"),
         l = Oe("NotFound");
-    return C(), R("div", null, [s.ingredient ? (C(), R("div", XD, [s.error ? (C(), R("div", QD, [m("p", ZD, le(s.error), 1)])) : re("", !0), m("nav", eI, [m("div", tI, [m("div", nI, [m("p", rI, le(s.ingredient.name.toUpperCase()), 1)])]), m("div", sI, [s.error ? re("", !0) : (C(), R("div", iI, [m("button", {
+    return C(), R("div", null, [s.ingredient ? (C(), R("div", QD, [s.error ? (C(), R("div", ZD, [m("p", eI, le(s.error), 1)])) : re("", !0), m("nav", tI, [m("div", nI, [m("div", rI, [m("p", sI, le(s.ingredient.name.toUpperCase()), 1)])]), m("div", iI, [s.error ? re("", !0) : (C(), R("div", oI, [m("button", {
         onClick: e[0] || (e[0] = a => i.deleteIngredient()),
         class: "button has-icons is-danger"
-    }, lI)])), m("div", aI, [m("button", {
+    }, aI)])), m("div", cI, [m("button", {
         onClick: e[1] || (e[1] = a => s.edit = !s.edit),
         class: "button has-icons is-warning"
-    }, uI)])])]), dI, s.edit ? re("", !0) : (C(), R("div", fI, [(C(!0), R(Fe, null, Dt(s.attributes, (a, c) => (C(), R("div", {
+    }, dI)])])]), fI, s.edit ? re("", !0) : (C(), R("div", hI, [(C(!0), R(Le, null, Dt(s.attributes, (a, c) => (C(), R("div", {
         key: c + "ingredientDetail",
         class: "level is-mobile px-5"
-    }, [m("div", hI, [m("div", pI, [m("span", mI, le(c), 1)])]), m("div", gI, [m("div", yI, [m("strong", null, le(a), 1)])])]))), 128))])), s.edit ? (C(), R("div", bI, [ce(o, {
+    }, [m("div", pI, [m("div", mI, [m("span", gI, le(c), 1)])]), m("div", yI, [m("div", bI, [m("strong", null, le(a), 1)])])]))), 128))])), s.edit ? (C(), R("div", vI, [ce(o, {
         ingredientProp: s.ingredient,
         onCancel: e[2] || (e[2] = a => s.edit = !1),
         onPosted: e[3] || (e[3] = a => {
             s.edit = !1, i.fetchIngredient()
         })
-    }, null, 8, ["ingredientProp"])])) : re("", !0)])) : (C(), R("div", vI, [ce(l)]))])
+    }, null, 8, ["ingredientProp"])])) : re("", !0)])) : (C(), R("div", xI, [ce(l)]))])
 }
-const kI = Ue(YD, [
-        ["render", xI]
+const wI = Be(XD, [
+        ["render", kI]
     ]),
-    wI = xv({
-        history: $0("/"),
+    SI = wv({
+        history: F0("/"),
         routes: [{
             path: "/",
             name: "home",
-            component: Ek
+            component: Ok
         }, {
             path: "/recipes",
             name: "recipes",
-            component: Ak
+            component: Rk
         }, {
             path: "/ingredients",
             name: "Ingredients",
-            component: GD
+            component: YD
         }, {
             path: "/ingredients/:id",
             name: "Ingredient",
-            component: kI
+            component: wI
         }, {
             path: "/recipes/new",
             name: "new",
-            component: OR
+            component: MR
         }, {
             path: "/recipes/newcategory",
             name: "newcategory",
-            component: wR
+            component: SR
         }, {
             path: "/recipes/:id",
             name: "recipe",
-            component: iR
+            component: oR
         }, {
             path: "/categories/:id",
             name: "category",
-            component: gR
+            component: yR
         }],
         scrollBehavior(t, e, n) {
-            return console.info(`saved: ${n}`), console.info(n), n || {
+            return n || {
                 top: 0
             }
         }
     }),
-    pg = Gb(y0);
-pg.use(wI);
-pg.mount("#app");
+    mg = Yb(v0);
+mg.use(SI);
+mg.mount("#app");
```

### Comparing `chef_recipes-1.0.1/src/js/chef/dist/favicon.ico` & `chef_recipes-1.0.2/src/js/chef/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/api/__init__.py` & `chef_recipes-1.0.2/src/python/chef/api/__init__.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/api/categories.py` & `chef_recipes-1.0.2/src/python/chef/api/categories.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/api/common.py` & `chef_recipes-1.0.2/src/python/chef/api/common.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/api/images.py` & `chef_recipes-1.0.2/src/python/chef/api/images.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/api/ingredients.py` & `chef_recipes-1.0.2/src/python/chef/api/ingredients.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/api/recipes.py` & `chef_recipes-1.0.2/src/python/chef/api/recipes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+import asyncio
 from typing import List
 
 from fastapi import APIRouter
 from sqlalchemy.orm import Session
 
 from chef.controllers import RecipesController
-from chef.schemas import Recipe, CreateOrUpdateRecipe
 from chef.models import engine
+from chef.schemas import Recipe, CreateOrUpdateRecipe
 
 router = APIRouter()
 recipes = RecipesController()
 
 
 # Store the current recipe id in memory
 CURRENT_RECIPES_IDS = []
 
 
 @router.get("")
-async def get_recipes(category: int = None) -> List[Recipe]:
+async def get_recipes(category: int = None, favorite: bool = False) -> List[Recipe]:
     with Session(engine()) as session:
+        if favorite:
+            return await recipes.get_all_and_filter(session, favorite=favorite)
         if category:
             return await recipes.get_by_category(session, category)
         return await recipes.get_all(session)
 
 
 @router.get("/{item_id}")
 async def get_recipe(item_id: int) -> Recipe:
@@ -39,9 +42,10 @@
 async def create_recipe(create_data: CreateOrUpdateRecipe) -> Recipe:
     with Session(engine()) as session:
         return await recipes.create(session, create_data)
 
 
 @router.put('/{item_id}')
 async def update_recipe(item_id: int, update_data: CreateOrUpdateRecipe) -> Recipe:
+    await asyncio.sleep(1)
     with Session(engine()) as session:
         return await recipes.update(session, item_id, update_data)
```

### Comparing `chef_recipes-1.0.1/src/python/chef/api/tags.py` & `chef_recipes-1.0.2/src/python/chef/api/tags.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/controllers.py` & `chef_recipes-1.0.2/src/python/chef/controllers.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,9 +198,16 @@
             .limit(1)
         ).first()
         if cat:
             result = [recipe for tag in cat.tags for recipe in tag.recipes]
             return [self.read_schema(**r.dictionary) for r in result]
         return []
 
+    async def get_all_and_filter(self, session: Session, **filters: typing.Any) -> List[Recipe]:
+        recipes = session.scalars(
+            select(self.read_schema.Meta.orm_model)
+            .filter_by(**filters)
+        ).all()
+        return [self.read_schema(**r.dictionary) for r in recipes]
+
     async def create_or_update(self, session: Session, data: Union[U, C]) -> R:
         raise ValueError("Not allowed on this controller!")
```

### Comparing `chef_recipes-1.0.1/src/python/chef/images.py` & `chef_recipes-1.0.2/src/python/chef/images.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/main.py` & `chef_recipes-1.0.2/src/python/chef/main.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/models.py` & `chef_recipes-1.0.2/src/python/chef/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,22 +163,33 @@
         secondary=category_tags,
         back_populates="categories"
     )
 
 
 class Recipe(Base):
     __tablename__ = "recipe"
-    __items__ = ["id", "title", "subtitle", "ingredients", "body",
-                 "source", "source_name", "tags", "portions"]
+    __items__ = [
+        "id",
+        "title",
+        "subtitle",
+        "ingredients",
+        "favorite",
+        "body",
+        "source",
+        "source_name",
+        "tags",
+        "portions"
+    ]
 
     title = Column(String(80), nullable=False)
     subtitle = Column(String(50), nullable=True)
     source_name = Column(String(100), nullable=True)
     source = Column(String(100), nullable=True)
     draft = Column(Boolean(), default=False)
+    favorite = Column(Boolean(), default=False)
     portions = Column(Integer, default=4)
     ingredients: Mapped[List[IngredientItem]] = relationship(
         secondary=ingredients,
         cascade="all"
     )
     tags = relationship(
         Tag,
```

### Comparing `chef_recipes-1.0.1/src/python/chef/schemas.py` & `chef_recipes-1.0.2/src/python/chef/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 
 
 class BaseRecipe(BaseModel):
     subtitle: Union[str, None] = None
     source_name: Union[str, None] = None
     source: Union[str, None] = None
     draft: bool = False
+    favorite: bool = False
     portions: int = 4
     ingredients: List[IngredientItem] = Field(default_factory=list)
     tags: List[Tag] = []
 
     # HTML content + rich text editor on the frontend
     body: Union[str, None] = None
```

### Comparing `chef_recipes-1.0.1/src/python/chef/session.py` & `chef_recipes-1.0.2/src/python/chef/session.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/src/python/chef/settings.py` & `chef_recipes-1.0.2/src/python/chef/settings.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.1/setup.py` & `chef_recipes-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'uvicorn>=0.22.0,<0.23.0']
 
 entry_points = \
 {'console_scripts': ['chef = chef.main:serve']}
 
 setup_kwargs = {
     'name': 'chef-recipes',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Home recipe management app.',
     'long_description': 'None',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `chef_recipes-1.0.1/PKG-INFO` & `chef_recipes-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chef-recipes
-Version: 1.0.1
+Version: 1.0.2
 Summary: Home recipe management app.
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

