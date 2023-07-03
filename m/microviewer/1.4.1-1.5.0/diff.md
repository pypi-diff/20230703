# Comparing `tmp/microviewer-1.4.1.tar.gz` & `tmp/microviewer-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.4.1.tar", last modified: Sat Jul  1 18:43:23 2023, max compression
+gzip compressed data, was "microviewer-1.5.0.tar", last modified: Mon Jul  3 19:25:41 2023, max compression
```

## Comparing `microviewer-1.4.1.tar` & `microviewer-1.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.284656 microviewer-1.4.1/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-01 18:43:23.000000 microviewer-1.4.1/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     2941 2023-07-01 18:43:23.000000 microviewer-1.4.1/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.4.1/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.4.1/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     2663 2023-07-01 18:43:23.284840 microviewer-1.4.1/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1649 2023-06-28 21:32:21.000000 microviewer-1.4.1/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.278924 microviewer-1.4.1/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.4.1/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     9295 2023-06-30 16:44:34.000000 microviewer-1.4.1/microviewer/crackle.js
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.283769 microviewer-1.4.1/microviewer/cursors/
--rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/exact-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/exact.png
--rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/large-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/large.png
--rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/medium-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/medium.png
--rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/small-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/small.png
--rw-r--r--   0 wms        (501) staff       (20)    42363 2023-07-01 18:42:55.000000 microviewer-1.4.1/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.4.1/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    31097 2023-06-30 19:47:12.000000 microviewer-1.4.1/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.4.1/microviewer/jquery-3.7.0.min.js
--rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-06-30 16:44:34.000000 microviewer-1.4.1/microviewer/libcrackle.wasm
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.282141 microviewer-1.4.1/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     2663 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.4.1/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.284320 microviewer-1.4.1/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.4.1/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.4.1/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.4.1/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)   297931 2023-06-28 20:05:35.000000 microviewer-1.4.1/seg-demo.png
--rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-01 18:43:23.285490 microviewer-1.4.1/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.4.1/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.758931 microviewer-1.5.0/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-03 19:25:41.000000 microviewer-1.5.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     3317 2023-07-03 19:25:41.000000 microviewer-1.5.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.5.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.5.0/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     2663 2023-07-03 19:25:41.759113 microviewer-1.5.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1649 2023-06-28 21:32:21.000000 microviewer-1.5.0/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.754207 microviewer-1.5.0/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.5.0/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     9574 2023-07-02 05:39:04.000000 microviewer-1.5.0/microviewer/crackle.js
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.758033 microviewer-1.5.0/microviewer/cursors/
+-rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/exact-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/exact.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/large-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/large.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/medium-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/medium.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/small-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/small.png
+-rw-r--r--   0 wms        (501) staff       (20)    42723 2023-07-03 19:24:55.000000 microviewer-1.5.0/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.5.0/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    35771 2023-07-03 18:34:37.000000 microviewer-1.5.0/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.5.0/microviewer/jquery-3.7.0.min.js
+-rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-07-03 19:24:55.000000 microviewer-1.5.0/microviewer/libcrackle.wasm
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.756336 microviewer-1.5.0/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     2663 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.5.0/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.758602 microviewer-1.5.0/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.5.0/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.5.0/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.5.0/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)   297931 2023-06-28 20:05:35.000000 microviewer-1.5.0/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-03 19:25:41.759784 microviewer-1.5.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.5.0/setup.py
```

### Comparing `microviewer-1.4.1/ChangeLog` & `microviewer-1.5.0/ChangeLog`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 CHANGES
 =======
 
+1.5.0
+-----
+
+* fix: undo/redo seemingly working now
+* feat: add date to file names
+* feat: adjust canvas dimensions on axis rotation
+* feat: add controls info about ctrl+z and ctrl+shift+z (undo/redo)
+* feat: not perfect, but partly working undo/redo function
+* feat: add segment selection to undo
+* feat: add undo for painting
+* fix: insertSquare can handle more data types
+
 1.4.1
 -----
 
 * refactor: make HyperVolume a child class of SegmentationVolume
 * fix: painting was broken for rectangular images
 * fix: automatically select a new port if 8080 in use
```

### Comparing `microviewer-1.4.1/LICENSE` & `microviewer-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/PKG-INFO` & `microviewer-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.4.1
+Version: 1.5.0
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.4.1/README.md` & `microviewer-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/__init__.py` & `microviewer-1.5.0/microviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/crackle.js` & `microviewer-1.5.0/microviewer/crackle.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -125,16 +125,15 @@
         if (op[0] & 5) throw op[1];
         return {
             value: op[0] ? op[1] : void 0,
             done: true
         };
     }
 };
-// exports.__esModule = true;
-// exports.decompressCrackle = exports.compressCrackle = void 0;
+var crackleWasmDataUrl = './libcrackle.wasm';
 var libraryEnv = {
     emscripten_notify_memory_growth: function() {},
     proc_exit: function(code) {
         throw "proc exit: ".concat(code);
     }
 };
 var wasmModule = null;
@@ -144,15 +143,15 @@
         var response, wasmCode, m;
         return __generator(this, function(_a) {
             switch (_a.label) {
                 case 0:
                     if (wasmModule !== null) {
                         return [2 /*return*/ , wasmModule];
                     }
-                    return [4 /*yield*/ , fetch("./libcrackle.wasm")];
+                    return [4 /*yield*/ , fetch(crackleWasmDataUrl)];
                 case 1:
                     response = _a.sent();
                     return [4 /*yield*/ , response.arrayBuffer()];
                 case 2:
                     wasmCode = _a.sent();
                     return [4 /*yield*/ , WebAssembly.instantiate(wasmCode, {
                         env: libraryEnv,
@@ -189,14 +188,26 @@
         sx: sx,
         sy: sy,
         sz: sz,
         dataWidth: dataWidth
     };
 }
 
+function arrayType(dataWidth) {
+    if (dataWidth === 1) {
+        return Uint8Array;
+    } else if (dataWidth === 2) {
+        return Uint16Array;
+    } else if (dataWidth === 4) {
+        return Uint32Array;
+    } else if (dataWidth === 8) {
+        return BigUint64Array;
+    }
+}
+
 function compressCrackle(buffer, dataWidth, sx, sy, sz) {
     return __awaiter(this, void 0, void 0, function() {
         var m, bufPtr, streamPtr, heap, streamSize, stream;
         return __generator(this, function(_a) {
             switch (_a.label) {
                 case 0:
                     return [4 /*yield*/ , loadCrackleModule()];
@@ -225,18 +236,18 @@
                         m.instance.exports.free(streamPtr);
                     }
                     return [2 /*return*/ ];
             }
         });
     });
 }
-// exports.compressCrackle = compressCrackle;
+
 function decompressCrackle(buffer) {
     return __awaiter(this, void 0, void 0, function() {
-        var m, _a, sx, sy, sz, dataWidth, voxels, nbytes, bufPtr, imagePtr, heap, code, image;
+        var m, _a, sx, sy, sz, dataWidth, voxels, nbytes, bufPtr, imagePtr, heap, code, image, ArrayType;
         return __generator(this, function(_b) {
             switch (_b.label) {
                 case 0:
                     return [4 /*yield*/ , loadCrackleModule()];
                 case 1:
                     m = _b.sent();
                     _a = readHeader(buffer), sx = _a.sx, sy = _a.sy, sz = _a.sz, dataWidth = _a.dataWidth;
@@ -253,18 +264,19 @@
                     try {
                         if (code !== 0) {
                             throw new Error("crackle: Failed to decode image. decoder code: ".concat(code));
                         }
                         image = new Uint8Array(m.instance.exports.memory.buffer, imagePtr, nbytes);
                         // copy the array so it can be memory managed by JS
                         // and we can free the emscripten buffer
-                        return [2 /*return*/ , image.slice(0)];
+                        image = image.slice(0);
+                        ArrayType = arrayType(dataWidth);
+                        return [2 /*return*/ , new ArrayType(image.buffer)];
                     } finally {
                         m.instance.exports.free(bufPtr);
                         m.instance.exports.free(imagePtr);
                     }
                     return [2 /*return*/ ];
             }
         });
     });
-}
-// exports.decompressCrackle = decompressCrackle;
+}
```

### Comparing `microviewer-1.4.1/microviewer/cursors/exact-active.png` & `microviewer-1.5.0/microviewer/cursors/exact-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/cursors/exact.png` & `microviewer-1.5.0/microviewer/cursors/exact.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/cursors/large-active.png` & `microviewer-1.5.0/microviewer/cursors/large-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/cursors/large.png` & `microviewer-1.5.0/microviewer/cursors/large.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/cursors/medium-active.png` & `microviewer-1.5.0/microviewer/cursors/medium-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/cursors/medium.png` & `microviewer-1.5.0/microviewer/cursors/medium.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/datacube.js` & `microviewer-1.5.0/microviewer/datacube.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -922,28 +922,44 @@
      *   [1] width
      *
      * Optional:
      *   [3,4,5] x,y,z offsets into the cube for partial slice downloads  
      *
      * Return: this
      */
-    insertSquare(square, width, offsetx = 0, offsety = 0, offsetz = 0) {
+    insertSquare(
+        square, axis, slice
+    ) {
         let _this = this;
 
-        const xsize = _this.size.x,
-            ysize = _this.size.y,
-            zsize = _this.size.z;
-
-        offsetz *= xsize * ysize;
-
-        for (let i = 0; i < square.length; i++) {
-            let x = offsetx + (i % width),
-                y = offsety + (Math.floor(i / width));
-
-            _this.cube[x + xsize * y + offsetz] = square[i];
+        const sx = _this.size.x,
+            sy = _this.size.y,
+            sz = _this.size.z;
+
+        let cube = _this.cube;
+        let ArrayType = this.arrayType();
+        let sq = new ArrayType(square.buffer);
+
+        if (axis === 'z') {
+            cube.set(sq, sx * sy * slice);
+        } else if (axis === 'y') {
+            let i = 0;
+            for (let z = 0; z < sz; z++) {
+                // cube.set(sq, z * sx, sx);
+                for (let x = 0; x < sx; x++, i++) {
+                    cube[x + sx * (slice + sy * z)] = sq[i];
+                }
+            }
+        } else if (axis === 'x') {
+            let i = 0;
+            for (let z = 0; z < sz; z++) {
+                for (let y = 0; y < sy; y++, i++) {
+                    cube[slice + sx * (y + sy * z)] = sq[i];
+                }
+            }
         }
 
         _this.clean = false;
 
         return this;
     }
```

### Comparing `microviewer-1.4.1/microviewer/favicon.ico` & `microviewer-1.5.0/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/index.html` & `microviewer-1.5.0/microviewer/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -229,25 +229,177 @@
 
       canvas.paintable.large:active {
         cursor: url("./cursors/large-active.png") 53.5 53.5, crosshair
       }
     </style>
 
     <script>
+      class CircularUndo {
+        constructor(n) {
+          this.buffer = [];
+          this.n = n;
+          for (let i = 0; i < this.n; i++) {
+            this.buffer.push(null);
+          }
+          this.index = 0;
+          this.offset = 0;
+          this.length = 0;
+          this.bottom = true;
+        }
+
+        incr () {
+          if (this.bottom) {
+            this.bottom = false;
+            if (this.length > 0) {
+              return;
+            }
+          }
+
+          if (this.length > 0) {
+            this.index++;
+          }
+          if (this.index === this.n) {
+            this.index = 0;
+          }
+
+          if (this.position() < this.length) {
+            return;
+          }
+
+          this.length++;
+          if (this.length > this.n) {
+            this.length = this.n;
+            this.offset++;
+            if (this.offset === this.n) {
+              this.offset = 0;
+            }
+          }
+        }
+
+        decr () {
+          if (this.length === 0) {
+            return;
+          }
+          else if (this.index === this.offset) {
+            this.bottom = true;
+            return;
+          }
+
+          this.index--;
+          if (this.index === -1) {
+            this.index = this.n - 1;
+          }
+        }
+
+        position () {
+          if (this.index === -1) {
+            return -1;
+          }
+          else if (this.offset <= this.index) {
+            return this.index - this.offset;
+          }
+          return this.index + (this.n - this.offset);
+        }
+
+        get () {
+          return this.buffer[this.index];
+        }
+
+        isDupe (item) {
+          let last = this.get();
+
+          if (last === null) {
+            return false;
+          }
+          else if (item[0] !== last[0]) {
+            return false;
+          }
+          else if (item[0] === 'select') {
+            return JSON.stringify(item[1][0]) === JSON.stringify(last[1][0]);
+          }
+          else {
+            let [arr1,axis1,slice1] = last[1];
+            let [arr2,axis2,slice2] = item[1];
+            if (axis1 !== axis2 || slice1 !== slice2) {
+              return false;
+            }
+
+            return arr1.every( (v,i) => v === arr2[i] );
+          }
+        }
+        
+        push () {
+          let item = null;
+          if (elems.paintmode.prop("checked")) {
+            let img2d = vol.getSegmentation().slice(AXIS, SLICE[AXIS], true);
+            item = [ 'paint', [ img2d, AXIS, SLICE[AXIS] ] ];
+          }
+          else {
+            item = [ 'select', [ structuredClone(vol.segments) ] ];
+          }
+
+          if (this.isDupe(item)) {
+            return;
+          }
+
+          this.incr();
+          this.buffer[this.index] = item;
+
+          if (this.position() < this.length - 1) {
+            this.length = this.position() + 1;
+          }
+        }
+
+        undo () {
+          if (this.bottom) {
+            return;
+          }
+          this.decr();
+          this.do();
+        }
+
+        redo () {
+          if (this.position() === this.length - 1) {
+            return;
+          }
+          this.incr();
+          this.do();
+        }
+
+        do () {
+          let cur = this.get();
+          if (cur === null) {
+            return;
+          }
+          let [ action, args ] = cur;
+          if (action === 'paint') {
+            let [img2d, axis, slice] = args;
+            vol.getSegmentation().insertSquare(
+              img2d, axis, slice
+            );
+          }
+          else {
+            vol.segments = structuredClone(args[0]);
+          }
+          render(true);
+        }
+      }
+
       var AXIS = 'z';
       var SLICE = { x: 0, y: 0, z: 0 };
       var CLICK = { x: 0, y: 0, z: 0, pxvalue: [] };
       var SIZE = {};
       var PARAMETERS = {};
       var PXVALUE = [];
       var MOUSE_OVER_IMAGE = false;
       var MAGNIFICATION = 1;
       var BRUSH = 0;
       var PAINTING_MODE = 0;
       var PAINT_MOVED = false;
+      var UNDO = new CircularUndo(250);
 
       let BRUSH_DIAMETERS = {
         0: 1, // px
         1: 25,
         2: 50,
         3: 100,
       };
@@ -374,28 +526,32 @@
               var x = evt.offsetX / innerWidth, 
                 y = evt.offsetY / innerHeight;
 
               x = clamp(x, 0, 0.999999999);
               y = clamp(y, 0, 0.999999999); 
 
               if (evt.which === 1) {
+                UNDO.push();
                 vol.toggleSegment(AXIS, SLICE[AXIS], x, y);
+                UNDO.push();
               }
             })
             .on('mousedown', function (evt) {
               PAINTING_MODE = 1;
+              UNDO.push();
               if (BRUSH === 0) {
                 PAINT_MOVED = false;
                 return;
               }
               paint(evt);
               evt.stopPropagation();
             })
             .on('mouseup', function (evt) {
               PAINTING_MODE = 0;
+              UNDO.push();
               render(true);
               evt.stopPropagation();
             })
             .on('mousemove', function (evt) {
               if (PAINTING_MODE > 0) {
                 PAINT_MOVED = true;
                 if (PAINTING_MODE === 1) {
@@ -406,14 +562,15 @@
                 }
               }
               evt.stopPropagation();
             })
             .on('contextmenu', function (evt) {
               PAINTING_MODE = 2;
               PAINT_MOVED = false;
+              UNDO.push();
               erase(evt);
               evt.stopPropagation();
               evt.preventDefault();
             });
         }
       }
 
@@ -429,14 +586,15 @@
           window.vol = new MonoVolume(datacube, false);
         }
 
         let vol = window.vol;
 
         vol.load('/channel', function (ratio) {
           render();
+          UNDO.push();
         }).then( () => render() );
 
         configure_segmentation_ui();
       }
 
       function setup_hyper_volume (data) {
         render_static();
@@ -446,14 +604,15 @@
         }
 
         window.vol = new HyperVolume(get_cube(0), get_cube(1));
         let vol = window.vol;
 
         vol.load(function (ratio) {
           render();
+          UNDO.push();
         }).then( () => render() );
 
         configure_segmentation_ui();
       }
 
       function toggleMenu () {
         elems.rtsidebar.toggleClass("hidden");
@@ -665,14 +824,24 @@
           BRUSH = Math.max(BRUSH - 1, 0);
           render(true);
         }
         else if (evt.keyCode === 'E'.charCodeAt(0)) {
           BRUSH = Math.min(BRUSH + 1, 3);
           render(true);
         }
+        else if (
+          evt.keyCode === 'Z'.charCodeAt(0) && evt.ctrlKey
+        ) {
+          if (evt.shiftKey) {
+            UNDO.redo();
+          }
+          else {
+            UNDO.undo();
+          }
+        }
       });
 
       $(document).on('keypress', function (evt) {
         if (evt.keyCode === 'W'.charCodeAt(0) 
           || evt.keyCode === 'w'.charCodeAt(0)
           || evt.keyCode === '.'.charCodeAt(0)
           || evt.keyCode === 190) {
@@ -693,14 +862,15 @@
           vol.shuffleColors();
           render(true);   
         }
         else if (evt.keyCode === 'X'.charCodeAt(0)
           || evt.keyCode === 'x'.charCodeAt(0)) {
           
           if (vol.clearSelected) {
+            UNDO.push();
             vol.clearSelected()
           }
           render(true);
         }
         else if (
           evt.keyCode === '='.charCodeAt(0) // '+' without shift
           || evt.keyCode === '+'.charCodeAt(0) 
@@ -777,23 +947,37 @@
           BRUSH = 3;
           render(true);
         });
 
       });
 
       function rotate_axis(delta) {
-        var index = (AXES.indexOf(AXIS) + delta) % AXES.length;
+        if (PAINTING_MODE) {
+          UNDO.push();
+        }
+
+        let index = (AXES.indexOf(AXIS) + delta) % AXES.length;
         AXIS = AXES[index];
+
+        let face_dims = vol.channel.faceDimensions(AXIS);
+
+        elems.channel.css("width", (face_dims[0] * MAGNIFICATION) + "px");
+        elems.channel.css("height", (face_dims[1] * MAGNIFICATION) + "px");
+
         render();
       }
 
       function move_slice (delta) {
+        if (PAINTING_MODE) {
+          UNDO.push();
+        }
+
         SLICE[AXIS] += delta;
         SLICE[AXIS] = clamp(SLICE[AXIS], 0, SIZE[AXIS] - 1);
-        render();  
+        render();
       }
 
       function render_static () {
         if (PARAMETERS.viewtype === 'single') {
           $('#instructions .hyperview').hide();
 
           if (PARAMETERS.layer_type === 'image') {
@@ -826,24 +1010,27 @@
         elems.bounds.text(
           `<${b[0]}, ${b[1]}, ${b[2]}>, <${b[3]}, ${b[4]}, ${b[5]}>`
         );
         elems.dtype.text( PARAMETERS.data_types.join("; ") );
         elems.resolution.text( PARAMETERS.resolution.join('x') );
         elems.shape.text( `<${SIZE.x}, ${SIZE.y}, ${SIZE.z}>` );
 
-
-
         let bytes = PARAMETERS["data_bytes"];
 
         if (Array.isArray(bytes)) {
           bytes = bytes.reduce((partialSum, a) => partialSum + a, 0);
         }
         bytes *= SIZE.x * SIZE.y * SIZE.z;
-        let megabytes = Math.floor(bytes / 1e6);
-        elems.memoryusage.text(`${megabytes}`);
+        let megabytes = bytes / 1e6;
+        if (megabytes < 1) {
+          elems.memoryusage.text(`${(megabytes * 1000)|0} kB`);
+        }
+        else {
+          elems.memoryusage.text(`${megabytes|0} MB`);
+        }
       }
 
       function update_pxvalue () {
         PXVALUE = [];
 
         vol.hover_id = null;
         if (vol.segmentation) {
@@ -978,28 +1165,24 @@
         if (_needsrender) {
           hardRender();
         }
 
         requestAnimationFrame(loop);
       }
 
-      function saveNumpy (filename) {
-        let dc = vol.channel;
-        if (vol.segmentation) {
-          dc = vol.segmentation;
-        }
-        dc.saveNumpy(filename);
+      function saveNumpy () {
+        let d = new Date();
+        let filename = `image-${d.getFullYear()}-${d.getMonth()}-${d.getDay()}.npy`;
+        vol.getSegmentation().saveNumpy(filename);
       }
 
-      function saveCrackle (filename) {
-        let dc = vol.channel;
-        if (vol.segmentation) {
-          dc = vol.segmentation;
-        }
-        dc.saveCrackle(filename);
+      function saveCrackle () {
+        let d = new Date();
+        let filename = `image-${d.getFullYear()}-${d.getMonth()}-${d.getDay()}.ckl`;
+        vol.getSegmentation().saveCrackle(filename);
       }
 
     </script>
   </head>
   <body>
     <div id="infobar">
       <span id="axis"></span> <span id="magnification"></span> <span id="coord"></span> <span id="realcoord"></span> <span id="pxvalue"></span> 
@@ -1021,15 +1204,15 @@
           <br />
           bounds: (<span id="bounds"></span>)
           <br / >
           dtype: <span id="dtype"></span>
           <br />
           resolution: <span id="resolution"></span> nm<sup>3</sup>
           <br />
-          memory: <span id="memory-usage"></span> MB
+          memory: <span id="memory-usage"></span>
         </div>
 
         <p class="segmentation">SELECTION VISIBILITY</p>
         <input class="segmentation" type="checkbox" id="show_hover" name="show_hover" checked="checked"/> <label class="segmentation" for="show_hover">Highlight (H)over?</label>
         <input class="segmentation" type="checkbox" id="show_unselected" name="show_unselected" /> <label class="segmentation" for="show_unselected">Show (U)nselected?</label> <br />
         <input class="segmentation" type="checkbox" id="paint_voxels" name="paint_voxels" /> <label class="segmentation" for="paint_voxels">Direct (P)aint?</label>
 
@@ -1049,16 +1232,16 @@
         <p class="segmentation">SELECTED SEGMENTS <button id="copy-segs">copy</button></p>
         <div class="segmentation" id="selected_segments"></div>
         <textarea id="addsegs" class="segmentation" type="text" placeholder="Input comma separated segids and press enter."></textarea>
 
         <p class="segmentation">SAVE SEGMENTATION</p>
 
         <div class="segmentation">
-          <button onclick="saveNumpy('image.npy')" title="Save as a .npy file. Might be big depending on your image size!">.npy</button> 
-          <button onclick="saveCrackle('image.ckl')" title="Save as a small .ckl file. There will be some processing time. Read more at https://github.com/seung-lab/crackle.">.ckl</button>
+          <button id="save-numpy" onclick="saveNumpy()" title="Save as a .npy file. Might be big depending on your image size!">.npy</button> 
+          <button id="save-crackle" onclick="saveCrackle()" title="Save as a small .ckl file. There will be some processing time. Read more at https://github.com/seung-lab/crackle.">.ckl</button>
         </div>
 
         <p>CONTROLS</p>
         <ul>
           <li>W/S ,/. or scroll - advance selected images</li>
           <li>A/D - switch slicing plane</li>
           <li>Space - zoom in to point</li>
@@ -1069,14 +1252,16 @@
           <li class="hyperview">+/- increase, decrease opacity</li>
           <li class='segmentation'>H - toggle hover highlight</li>
           <li class='segmentation'>U - toggle show unselected</li>
           <li class='segmentation'>P - toggle direct voxel painting</li>
           <li>1/2 - zoom out/in</li>
           <li>M - show/hide menu</li>
           <li class="segmentation">Q/E - decrease/increase brush size</li>
+          <li class="segmentation">ctrl+Z - undo</li>
+          <li class="segmentation">ctrl+shift+Z - redo</li>
         </ul>
       </div>
     </div>
 
     <canvas oncontextmenu="return false;" id="channel" class="exact" width="256" height="256"></canvas>
 
   </body>
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 ===============================================================================
 ===============================================================================
 DIMENSIONS
 shape:
 bounds: ()
 > dtype:
 resolution:  nm3
-memory:  MB
+memory:
 SELECTION VISIBILITY
 * Highlight (H)over? ⁰ Show (U)nselected?
 ⁰ Direct (P)aint?
 BRUSH SIZE
 PAINT LABEL
 [Unknown INPUT type]
 SELECTED SEGMENTS copy
@@ -37,7 +37,9 @@
     * +/- increase, decrease opacity
     * H - toggle hover highlight
     * U - toggle show unselected
     * P - toggle direct voxel painting
     * 1/2 - zoom out/in
     * M - show/hide menu
     * Q/E - decrease/increase brush size
+    * ctrl+Z - undo
+    * ctrl+shift+Z - redo
```

### Comparing `microviewer-1.4.1/microviewer/jquery-3.7.0.min.js` & `microviewer-1.5.0/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer/libcrackle.wasm` & `microviewer-1.5.0/microviewer/libcrackle.wasm`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer.egg-info/PKG-INFO` & `microviewer-1.5.0/microviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.4.1
+Version: 1.5.0
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.4.1/microviewer.egg-info/SOURCES.txt` & `microviewer-1.5.0/microviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/microviewer_cli/cli.py` & `microviewer-1.5.0/microviewer_cli/cli.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/seg-demo.png` & `microviewer-1.5.0/seg-demo.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.1/setup.cfg` & `microviewer-1.5.0/setup.cfg`

 * *Files identical despite different names*

