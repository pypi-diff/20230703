# Comparing `tmp/msg2fastdds-0.0.1.tar.gz` & `tmp/msg2fastdds-0.0.2.tar.gz`

## Comparing `msg2fastdds-0.0.1.tar` & `msg2fastdds-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/.DS_Store
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/Dockerfile
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/.DS_Store
--rwxr-xr-x   0        0        0     2037 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/__init__.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/__main__.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/cli.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/main.py
--rw-r--r--   0        0        0    33404 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/parser.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/action/__init__.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/msg/__init__.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/__init__.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/action.idl.em
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/msg.idl.em
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/srv.idl.em
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/struct.idl.em
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/srv/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/__init__.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/cli.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/common.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/entry_points.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/extensions.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/__init__.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/helpers.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/generate/__init__.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/generate/api.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/generate/extensions.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/translate/__init__.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/translate/api.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/translate/extensions.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/LICENSE
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/README.md
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 msg2fastdds-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/.DS_Store
+-rwxr-xr-x   0        0        0     2212 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/__init__.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/__main__.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/cli.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/main.py
+-rw-r--r--   0        0        0    33404 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/parser.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/action/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/msg/__init__.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/__init__.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/action.idl.em
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/msg.idl.em
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/srv.idl.em
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/struct.idl.em
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/srv/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/__init__.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/cli.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/common.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/entry_points.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/extensions.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/__init__.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/helpers.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/generate/__init__.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/generate/api.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/generate/extensions.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/translate/__init__.py
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/translate/api.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/translate/extensions.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/LICENSE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/README.md
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 msg2fastdds-0.0.2/PKG-INFO
```

### Comparing `msg2fastdds-0.0.1/.DS_Store` & `msg2fastdds-0.0.2/.DS_Store`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0022  ..............."
+00000040: 0000 0000 0000 0002 0000 0000 0000 001e  ................
 00000050: 0000 0001 0000 1000 6c67 3153 636f 6d70  ........lg1Scomp
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,43 +250,43 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0022 0000 0004  ..........."....
+00001000: 0000 0000 0000 0000 0000 001e 0000 0004  ................
 00001010: 002e 0067 0069 0074 6c67 3153 636f 6d70  ...g.i.tlg1Scomp
-00001020: 0000 0000 0002 223a 0000 0004 002e 0067  ......":.......g
+00001020: 0000 0000 0002 22c5 0000 0004 002e 0067  ......"........g
 00001030: 0069 0074 6d6f 4444 626c 6f62 0000 0008  .i.tmoDDblob....
-00001040: 10a8 31e9 ed26 c541 0000 0004 002e 0067  ..1..&.A.......g
+00001040: f69e cb75 5b29 c541 0000 0004 002e 0067  ...u[).A.......g
 00001050: 0069 0074 6d6f 6444 626c 6f62 0000 0008  .i.tmodDblob....
-00001060: 10a8 31e9 ed26 c541 0000 0004 002e 0067  ..1..&.A.......g
+00001060: f69e cb75 5b29 c541 0000 0004 002e 0067  ...u[).A.......g
 00001070: 0069 0074 7068 3153 636f 6d70 0000 0000  .i.tph1Scomp....
-00001080: 0009 b000 0000 0004 0064 0069 0073 0074  .........d.i.s.t
+00001080: 0009 d000 0000 0004 0064 0069 0073 0074  .........d.i.s.t
 00001090: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
 000010a0: 7374 3030 d601 0203 0405 0607 0709 070b  st00............
 000010b0: 075d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000010c0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
 000010d0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
 000010e0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
 000010f0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
 00001100: 5369 6465 6261 7209 0908 095f 1018 7b7b  Sidebar...._..{{
 00001110: 3432 312c 2034 3431 7d2c 207b 3932 302c  421, 441}, {920,
 00001120: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
 00001130: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
 00001140: 0000 000d 0000 0000 0000 0000 0000 0000  ................
 00001150: 0000 008b 0000 0004 0064 0069 0073 0074  .........d.i.s.t
-00001160: 6c67 3153 636f 6d70 0000 0000 0001 0cfb  lg1Scomp........
+00001160: 6c67 3153 636f 6d70 0000 0000 0000 0000  lg1Scomp........
 00001170: 0000 0004 0064 0069 0073 0074 6d6f 4444  .....d.i.s.tmoDD
-00001180: 626c 6f62 0000 0008 003a d9b2 ec26 c541  blob.....:...&.A
+00001180: 626c 6f62 0000 0008 4bdb 9321 f426 c541  blob....K..!.&.A
 00001190: 0000 0004 0064 0069 0073 0074 6d6f 6444  .....d.i.s.tmodD
-000011a0: 626c 6f62 0000 0008 003a d9b2 ec26 c541  blob.....:...&.A
+000011a0: 626c 6f62 0000 0008 4bdb 9321 f426 c541  blob....K..!.&.A
 000011b0: 0000 0004 0064 0069 0073 0074 7068 3153  .....d.i.s.tph1S
-000011c0: 636f 6d70 0000 0000 0001 2000 0000 0004  comp...... .....
+000011c0: 636f 6d70 0000 0000 0000 0000 0000 0004  comp............
 000011d0: 0064 0069 0073 0074 7653 726e 6c6f 6e67  .d.i.s.tvSrnlong
 000011e0: 0000 0001 0000 000b 006d 0073 0067 0032  .........m.s.g.2
 000011f0: 0066 0061 0073 0074 0064 0064 0073 6c67  .f.a.s.t.d.d.slg
 00001200: 3153 636f 6d70 0000 0000 0000 1804 0000  1Scomp..........
 00001210: 000b 006d 0073 0067 0032 0066 0061 0073  ...m.s.g.2.f.a.s
 00001220: 0074 0064 0064 0073 6d6f 4444 626c 6f62  .t.d.d.smoDDblob
 00001230: 0000 0008 dd55 9b67 e826 c541 0000 000b  .....U.g.&.A....
@@ -331,27 +331,27 @@
 000014a0: 337b 5988 e726 c541 0000 000a 0072 006f  3{Y..&.A.....r.o
 000014b0: 0073 0069 0064 006c 005f 0063 006c 0069  .s.i.d.l._.c.l.i
 000014c0: 6d6f 6444 626c 6f62 0000 0008 337b 5988  modDblob....3{Y.
 000014d0: e726 c541 0000 000a 0072 006f 0073 0069  .&.A.....r.o.s.i
 000014e0: 0064 006c 005f 0063 006c 0069 7068 3153  .d.l._.c.l.iph1S
 000014f0: 636f 6d70 0000 0000 0001 1000 0000 0003  comp............
 00001500: 0073 0072 0063 6c67 3153 636f 6d70 0000  .s.r.clg1Scomp..
-00001510: 0000 0001 982e 0000 0003 0073 0072 0063  ...........s.r.c
+00001510: 0000 0001 98dd 0000 0003 0073 0072 0063  ...........s.r.c
 00001520: 6d6f 4444 626c 6f62 0000 0008 e662 dc8e  moDDblob.....b..
 00001530: eb26 c541 0000 0003 0073 0072 0063 6d6f  .&.A.....s.r.cmo
 00001540: 6444 626c 6f62 0000 0008 e662 dc8e eb26  dDblob.....b...&
 00001550: c541 0000 0003 0073 0072 0063 7068 3153  .A.....s.r.cph1S
-00001560: 636f 6d70 0000 0000 0002 7000 0000 0004  comp......p.....
-00001570: 0075 006e 006b 006f 6c67 3153 636f 6d70  .u.n.k.olg1Scomp
-00001580: 0000 0000 0000 0000 0000 0004 0075 006e  .............u.n
-00001590: 006b 006f 6d6f 4444 626c 6f62 0000 0008  .k.omoDDblob....
-000015a0: 4df2 5ade ed26 c541 0000 0004 0075 006e  M.Z..&.A.....u.n
-000015b0: 006b 006f 6d6f 6444 626c 6f62 0000 0008  .k.omodDblob....
-000015c0: 4df2 5ade ed26 c541 0000 0004 0075 006e  M.Z..&.A.....u.n
-000015d0: 006b 006f 7068 3153 636f 6d70 0000 0000  .k.oph1Scomp....
+00001560: 636f 6d70 0000 0000 0002 7000 0000 0000  comp......p.....
+00001570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -459,27 +459,27 @@
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
 00001cf0: 0000 0000 0140 0000 0000 0000 0000 0003  .....@..........
 00001d00: 0073 0072 0063 6c67 3153 636f 6d70 0000  .s.r.clg1Scomp..
-00001d10: 0000 0001 982e 0000 0003 0073 0072 0063  ...........s.r.c
+00001d10: 0000 0001 98dd 0000 0003 0073 0072 0063  ...........s.r.c
 00001d20: 6d6f 4444 626c 6f62 0000 0008 e662 dc8e  moDDblob.....b..
 00001d30: eb26 c541 0000 0003 0073 0072 0063 6d6f  .&.A.....s.r.cmo
 00001d40: 6444 626c 6f62 0000 0008 e662 dc8e eb26  dDblob.....b...&
 00001d50: c541 0000 0003 0073 0072 0063 7068 3153  .A.....s.r.cph1S
-00001d60: 636f 6d70 0000 0000 0002 7000 0000 0004  comp......p.....
-00001d70: 0075 006e 006b 006f 6c67 3153 636f 6d70  .u.n.k.olg1Scomp
-00001d80: 0000 0000 0000 0000 0000 0004 0075 006e  .............u.n
-00001d90: 006b 006f 6d6f 4444 626c 6f62 0000 0008  .k.omoDDblob....
-00001da0: 4df2 5ade ed26 c541 0000 0004 0075 006e  M.Z..&.A.....u.n
-00001db0: 006b 006f 6d6f 6444 626c 6f62 0000 0008  .k.omodDblob....
-00001dc0: 4df2 5ade ed26 c541 0000 0004 0075 006e  M.Z..&.A.....u.n
-00001dd0: 006b 006f 7068 3153 636f 6d70 0000 0000  .k.oph1Scomp....
+00001d60: 636f 6d70 0000 0000 0002 7000 0000 0000  comp......p.....
+00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `msg2fastdds-0.0.1/src/.DS_Store` & `msg2fastdds-0.0.2/src/.DS_Store`

 * *Files 25% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
 00000210: 006d 0073 0067 0032 0066 0061 0073 0074  .m.s.g.2.f.a.s.t
 00000220: 0064 0064 0073 6c67 3153 636f 6d70 0000  .d.d.slg1Scomp..
-00000230: 0000 0001 802a 0000 000b 006d 0073 0067  .....*.....m.s.g
+00000230: 0000 0001 80d9 0000 000b 006d 0073 0067  ...........m.s.g
 00000240: 0032 0066 0061 0073 0074 0064 0064 0073  .2.f.a.s.t.d.d.s
-00000250: 6d6f 4444 626c 6f62 0000 0008 b028 27cb  moDDblob.....('.
-00000260: ed26 c541 0000 000b 006d 0073 0067 0032  .&.A.....m.s.g.2
+00000250: 6d6f 4444 626c 6f62 0000 0008 e844 fe8e  moDDblob.....D..
+00000260: 7229 c541 0000 000b 006d 0073 0067 0032  r).A.....m.s.g.2
 00000270: 0066 0061 0073 0074 0064 0064 0073 6d6f  .f.a.s.t.d.d.smo
-00000280: 6444 626c 6f62 0000 0008 b028 27cb ed26  dDblob.....('..&
+00000280: 6444 626c 6f62 0000 0008 e844 fe8e 7229  dDblob.....D..r)
 00000290: c541 0000 000b 006d 0073 0067 0032 0066  .A.....m.s.g.2.f
 000002a0: 0061 0073 0074 0064 0064 0073 7068 3153  .a.s.t.d.d.sph1S
 000002b0: 636f 6d70 0000 0000 0002 5000 0000 0014  comp......P.....
 000002c0: 006d 0073 0067 0032 0066 0061 0073 0074  .m.s.g.2.f.a.s.t
 000002d0: 0064 0064 0073 002e 0065 0067 0067 002d  .d.d.s...e.g.g.-
 000002e0: 0069 006e 0066 006f 6c67 3153 636f 6d70  .i.n.f.olg1Scomp
 000002f0: 0000 0000 0000 070f 0000 0014 006d 0073  .............m.s
```

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/.DS_Store` & `msg2fastdds-0.0.2/src/msg2fastdds/.DS_Store`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/__init__.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/__main__.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/__main__.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/cli.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/cli.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/main.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/main.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/parser.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/parser.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/action/__init__.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/action/__init__.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/msg/__init__.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/__init__.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/action.idl.em` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/action.idl.em`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/msg.idl.em` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/msg.idl.em`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/srv.idl.em` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/srv.idl.em`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/resource/struct.idl.em` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/resource/struct.idl.em`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_adapter/srv/__init__.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_adapter/srv/__init__.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/cli.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/cli.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/common.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/common.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/entry_points.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/entry_points.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/extensions.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/extensions.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/__init__.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/__init__.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/helpers.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/helpers.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/generate/__init__.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/generate/api.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/generate/api.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/generate/extensions.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/generate/extensions.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/translate/__init__.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/translate/api.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/translate/api.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/src/msg2fastdds/rosidl_cli/command/translate/extensions.py` & `msg2fastdds-0.0.2/src/msg2fastdds/rosidl_cli/command/translate/extensions.py`

 * *Files identical despite different names*

### Comparing `msg2fastdds-0.0.1/LICENSE` & `msg2fastdds-0.0.2/LICENSE`

 * *Files identical despite different names*

