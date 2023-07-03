# Comparing `tmp/mediafile-0.8.1.tar.gz` & `tmp/mediafile-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediafile-0.8.1.tar", last modified: Tue Sep 28 20:43:30 2021, max compression
+gzip compressed data, was "mediafile-0.9.0.tar", last modified: Sat Nov 27 16:48:06 2021, max compression
```

## Comparing `mediafile-0.8.1.tar` & `mediafile-0.9.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0     1754 2021-08-31 12:33:42.664955 mediafile-0.8.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1006 2016-11-27 01:46:20.000000 mediafile-0.8.1/.gitignore
--rw-r--r--   0        0        0     1075 2016-11-26 22:12:31.000000 mediafile-0.8.1/LICENSE
--rw-r--r--   0        0        0     1484 2020-03-30 01:16:00.466949 mediafile-0.8.1/README.rst
--rw-r--r--   0        0        0     7618 2016-11-27 01:14:22.000000 mediafile-0.8.1/docs/Makefile
--rw-r--r--   0        0        0      706 2020-03-30 02:04:54.311634 mediafile-0.8.1/docs/conf.py
--rw-r--r--   0        0        0     5611 2021-09-28 20:43:00.903553 mediafile-0.8.1/docs/index.rst
--rw-r--r--   0        0        0    79286 2021-09-28 20:42:32.916817 mediafile-0.8.1/mediafile.py
--rw-r--r--   0        0        0      841 2021-08-31 12:09:34.558611 mediafile-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      781 2016-11-26 22:12:31.000000 mediafile-0.8.1/setup.cfg
--rw-r--r--   0        0        0       90 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/__init__.py
--rw-r--r--   0        0        0     1737 2016-11-27 00:07:21.000000 mediafile-0.8.1/test/_common.py
--rw-r--r--   0        0        0    88396 2021-09-01 13:50:00.000000 mediafile-0.8.1/test/rsrc/backup.wav
--rw-r--r--   0        0        0    12820 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/bpm.mp3
--rw-r--r--   0        0        0     8765 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/coverart.ogg
--rw-r--r--   0        0        0     8562 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/date_with_slashes.ogg
--rw-r--r--   0        0        0     8818 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/discc.ogg
--rw-r--r--   0        0        0    88254 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.aiff
--rw-r--r--   0        0        0     6884 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.alac.m4a
--rw-r--r--   0        0        0    13420 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.ape
--rw-r--r--   0        0        0     4188 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/empty.dsf
--rw-r--r--   0        0        0    21890 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.flac
--rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.m4a
--rw-r--r--   0        0        0     8567 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.mp3
--rw-r--r--   0        0        0     2196 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.mpc
--rw-r--r--   0        0        0     8543 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.ogg
--rw-r--r--   0        0        0     8243 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.opus
--rw-r--r--   0        0        0    88278 2021-09-01 13:50:00.000000 mediafile-0.8.1/test/rsrc/empty.wav
--rw-r--r--   0        0        0    23608 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.wma
--rw-r--r--   0        0        0    12840 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/empty.wv
--rw-r--r--   0        0        0     8192 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/emptylist.mp3
--rw-r--r--   0        0        0    89296 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.aiff
--rw-r--r--   0        0        0     6884 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.alac.m4a
--rw-r--r--   0        0        0    14076 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.ape
--rw-r--r--   0        0        0   114582 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.dsf
--rw-r--r--   0        0        0    21890 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.flac
--rw-r--r--   0        0        0     5862 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.m4a
--rw-r--r--   0        0        0    12820 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.mp3
--rw-r--r--   0        0        0     3020 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.mpc
--rw-r--r--   0        0        0    10176 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.ogg
--rw-r--r--   0        0        0     8349 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.opus
--rw-r--r--   0        0        0    89398 2021-09-01 13:50:00.000000 mediafile-0.8.1/test/rsrc/full.wav
--rw-r--r--   0        0        0    26883 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.wma
--rw-r--r--   0        0        0    13664 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/full.wv
--rw-r--r--   0        0        0      628 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image-2x3.jpg
--rw-r--r--   0        0        0      155 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image-2x3.png
--rw-r--r--   0        0        0      206 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image-2x3.tiff
--rw-r--r--   0        0        0    14279 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image.ape
--rw-r--r--   0        0        0    21890 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image.flac
--rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image.m4a
--rw-r--r--   0        0        0    10452 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image.mp3
--rw-r--r--   0        0        0     9786 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image.ogg
--rw-r--r--   0        0        0    24561 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image.wma
--rwxr-xr-x   0        0        0    10452 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/image_unknown_type.mp3
--rw-r--r--   0        0        0    13955 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/oldape.ape
--rw-r--r--   0        0        0      622 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/only-magic-bytes.jpg
--rw-r--r--   0        0        0    21890 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/partial.flac
--rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/partial.m4a
--rw-r--r--   0        0        0    12820 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/partial.mp3
--rw-r--r--   0        0        0    23680 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/pure.wma
--rw-r--r--   0        0        0     5862 2020-03-29 20:18:16.229553 mediafile-0.8.1/test/rsrc/read_only_tag.m4a
--rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/soundcheck-nonascii.m4a
--rw-r--r--   0        0        0    12820 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/space_time.mp3
--rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/t_time.m4a
--rw-r--r--   0        0        0    88272 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.aiff
--rw-r--r--   0        0        0     6884 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.alac.m4a
--rw-r--r--   0        0        0    13444 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.ape
--rw-r--r--   0        0        0     5243 2019-05-31 00:21:07.000000 mediafile-0.8.1/test/rsrc/unparseable.dsf
--rw-r--r--   0        0        0    21890 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.flac
--rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.m4a
--rw-r--r--   0        0        0     9601 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.mp3
--rw-r--r--   0        0        0     2284 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.mpc
--rw-r--r--   0        0        0     8563 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.ogg
--rw-r--r--   0        0        0     8263 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.opus
--rw-r--r--   0        0        0    88278 2021-09-01 13:50:00.000000 mediafile-0.8.1/test/rsrc/unparseable.wav
--rw-r--r--   0        0        0    23664 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.wma
--rw-r--r--   0        0        0    12928 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/unparseable.wv
--rw-r--r--   0        0        0     8556 2016-11-26 22:12:31.000000 mediafile-0.8.1/test/rsrc/year.ogg
--rw-r--r--   0        0        0    34678 2021-09-01 13:50:00.000000 mediafile-0.8.1/test/test_mediafile.py
--rw-r--r--   0        0        0    15850 2021-08-19 20:23:12.000000 mediafile-0.8.1/test/test_mediafile_edge.py
--rw-r--r--   0        0        0     1051 2021-08-31 12:33:42.665767 mediafile-0.8.1/tox.ini
--rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 mediafile-0.8.1/setup.py
--rw-r--r--   0        0        0      229 1970-01-01 00:00:00.000000 mediafile-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1754 2021-08-31 12:33:42.664955 mediafile-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1006 2016-11-27 01:46:20.000000 mediafile-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1075 2016-11-26 22:12:31.000000 mediafile-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1484 2020-03-30 01:16:00.466949 mediafile-0.9.0/README.rst
+-rw-r--r--   0        0        0     7618 2016-11-27 01:14:22.000000 mediafile-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0      706 2021-11-26 20:13:43.079020 mediafile-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0     5813 2021-11-26 20:13:43.079349 mediafile-0.9.0/docs/index.rst
+-rw-r--r--   0        0        0    80652 2021-11-26 20:13:43.079976 mediafile-0.9.0/mediafile.py
+-rw-r--r--   0        0        0      841 2021-08-31 12:09:34.558611 mediafile-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      781 2016-11-26 22:12:31.000000 mediafile-0.9.0/setup.cfg
+-rw-r--r--   0        0        0       90 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/__init__.py
+-rw-r--r--   0        0        0     1737 2016-11-27 00:07:21.000000 mediafile-0.9.0/test/_common.py
+-rw-r--r--   0        0        0    88396 2021-09-01 13:50:00.000000 mediafile-0.9.0/test/rsrc/backup.wav
+-rw-r--r--   0        0        0    12820 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/bpm.mp3
+-rw-r--r--   0        0        0    13343 2021-11-26 20:13:43.082091 mediafile-0.9.0/test/rsrc/cbr.mp3
+-rw-r--r--   0        0        0     8765 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/coverart.ogg
+-rw-r--r--   0        0        0     8562 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/date_with_slashes.ogg
+-rw-r--r--   0        0        0     8818 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/discc.ogg
+-rw-r--r--   0        0        0    88254 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.aiff
+-rw-r--r--   0        0        0     6884 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.alac.m4a
+-rw-r--r--   0        0        0    13420 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.ape
+-rw-r--r--   0        0        0     4188 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/empty.dsf
+-rw-r--r--   0        0        0    21890 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.flac
+-rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.m4a
+-rw-r--r--   0        0        0     8567 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.mp3
+-rw-r--r--   0        0        0     2196 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.mpc
+-rw-r--r--   0        0        0     8543 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.ogg
+-rw-r--r--   0        0        0     8243 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.opus
+-rw-r--r--   0        0        0    88278 2021-09-01 13:50:00.000000 mediafile-0.9.0/test/rsrc/empty.wav
+-rw-r--r--   0        0        0    23608 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.wma
+-rw-r--r--   0        0        0    12840 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/empty.wv
+-rw-r--r--   0        0        0     8192 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/emptylist.mp3
+-rw-r--r--   0        0        0    89296 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.aiff
+-rw-r--r--   0        0        0     6884 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.alac.m4a
+-rw-r--r--   0        0        0    14076 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.ape
+-rw-r--r--   0        0        0   114582 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.dsf
+-rw-r--r--   0        0        0    21890 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.flac
+-rw-r--r--   0        0        0     5862 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.m4a
+-rw-r--r--   0        0        0    12820 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.mp3
+-rw-r--r--   0        0        0     3020 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.mpc
+-rw-r--r--   0        0        0    10176 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.ogg
+-rw-r--r--   0        0        0     8349 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.opus
+-rw-r--r--   0        0        0    89398 2021-09-01 13:50:00.000000 mediafile-0.9.0/test/rsrc/full.wav
+-rw-r--r--   0        0        0    26883 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.wma
+-rw-r--r--   0        0        0    13664 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/full.wv
+-rw-r--r--   0        0        0      628 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image-2x3.jpg
+-rw-r--r--   0        0        0      155 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image-2x3.png
+-rw-r--r--   0        0        0      206 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image-2x3.tiff
+-rw-r--r--   0        0        0    14279 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image.ape
+-rw-r--r--   0        0        0    21890 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image.flac
+-rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image.m4a
+-rw-r--r--   0        0        0    10452 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image.mp3
+-rw-r--r--   0        0        0     9786 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image.ogg
+-rw-r--r--   0        0        0    24561 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image.wma
+-rwxr-xr-x   0        0        0    10452 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/image_unknown_type.mp3
+-rw-r--r--   0        0        0    13955 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/oldape.ape
+-rw-r--r--   0        0        0      622 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/only-magic-bytes.jpg
+-rw-r--r--   0        0        0    21890 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/partial.flac
+-rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/partial.m4a
+-rw-r--r--   0        0        0    12820 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/partial.mp3
+-rw-r--r--   0        0        0    23680 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/pure.wma
+-rw-r--r--   0        0        0     5862 2020-03-29 20:18:16.229553 mediafile-0.9.0/test/rsrc/read_only_tag.m4a
+-rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/soundcheck-nonascii.m4a
+-rw-r--r--   0        0        0    12820 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/space_time.mp3
+-rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/t_time.m4a
+-rw-r--r--   0        0        0    88272 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.aiff
+-rw-r--r--   0        0        0     6884 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.alac.m4a
+-rw-r--r--   0        0        0    13444 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.ape
+-rw-r--r--   0        0        0     5243 2019-05-31 00:21:07.000000 mediafile-0.9.0/test/rsrc/unparseable.dsf
+-rw-r--r--   0        0        0    21890 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.flac
+-rw-r--r--   0        0        0     5862 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.m4a
+-rw-r--r--   0        0        0     9601 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.mp3
+-rw-r--r--   0        0        0     2284 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.mpc
+-rw-r--r--   0        0        0     8563 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.ogg
+-rw-r--r--   0        0        0     8263 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.opus
+-rw-r--r--   0        0        0    88278 2021-09-01 13:50:00.000000 mediafile-0.9.0/test/rsrc/unparseable.wav
+-rw-r--r--   0        0        0    23664 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.wma
+-rw-r--r--   0        0        0    12928 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/unparseable.wv
+-rw-r--r--   0        0        0     8556 2016-11-26 22:12:31.000000 mediafile-0.9.0/test/rsrc/year.ogg
+-rw-r--r--   0        0        0    36265 2021-11-26 20:13:43.082924 mediafile-0.9.0/test/test_mediafile.py
+-rw-r--r--   0        0        0    15850 2021-08-19 20:23:12.000000 mediafile-0.9.0/test/test_mediafile_edge.py
+-rw-r--r--   0        0        0     1051 2021-08-31 12:33:42.665767 mediafile-0.9.0/tox.ini
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 mediafile-0.9.0/setup.py
+-rw-r--r--   0        0        0      229 1970-01-01 00:00:00.000000 mediafile-0.9.0/PKG-INFO
```

### Comparing `mediafile-0.8.1/.github/workflows/build.yml` & `mediafile-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/.gitignore` & `mediafile-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/LICENSE` & `mediafile-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/README.rst` & `mediafile-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/docs/Makefile` & `mediafile-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/docs/conf.py` & `mediafile-0.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 master_doc = 'index'
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 project = 'MediaFile'
 copyright = '2016, the beets project'
 author = 'the beets project'
 
-version = '0.5'
-release = '0.5.0'
+version = '0.9'
+release = '0.9.0'
 
 pygments_style = 'sphinx'
 htmlhelp_basename = 'mediafiledoc'
 
 # LaTeX output.
 latex_documents = [
     (master_doc, 'MediaFile.tex', 'MediaFile Documentation',
```

### Comparing `mediafile-0.8.1/docs/index.rst` & `mediafile-0.9.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 * plural/list variants like ``artists`` and ``albumartists``,
 * identifiers like ``asin``, ``isrc`` or ``mb_releasegroupid``,
 * dates like the release ``year``, ``month`` and ``day`` with convenience wrapper ``date``,
 * detailed metadata like ``language`` or ``media``,
 * ``lyrics``, ``copyright``, ``url``
 * calculated metadata like ``bpm`` (beats per minute) and ``r128_track_gain`` (ReplayGain),
 * embedded images (e.g. album art),
-* file metadata like ``bitrate`` and ``length``.
+* file metadata like ``samplerate``, ``bitdepth``, ``channels``, ``bitrate``, ``bitrate_mode``, ``encoder_info``, ``encoder_settings`` and ``length``.
 
 Compatibility
 -------------
 The ID3 and MPEG-4 test cases were created with iTunes and the FLAC and Ogg test
 cases were created (mostly) with
 `MediaRage`_. The Monkey's Audio tags were mainly fabricated using the open-source
 `Tag`_. Thus, MediaFile's tag support most closely aligns with those three applications.
@@ -131,14 +131,20 @@
 
     g.save()
 
 
 Changelog
 ---------
 
+v0.9.0
+''''''
+
+- Add the properties ``bitrate_mode``, ``encoder_info`` and
+  ``encoder_settings``.
+
 v0.8.1
 ''''''
 
 - Fix a regression in v0.8.0 that caused a crash on Python versions below 3.8.
 
 v0.8.0
 ''''''
```

### Comparing `mediafile-0.8.1/mediafile.py` & `mediafile-0.9.0/mediafile.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 data from the tags. In turn ``MediaField`` uses a number of
 ``StorageStyle`` strategies to handle format specific logic.
 """
 from __future__ import division, absolute_import, print_function
 
 import mutagen
 import mutagen.id3
+import mutagen.mp3
 import mutagen.mp4
 import mutagen.flac
 import mutagen.asf
 import mutagen._util
 
 import base64
 import binascii
@@ -54,15 +55,15 @@
 import os
 import re
 import six
 import struct
 import traceback
 
 
-__version__ = '0.8.1'
+__version__ = '0.9.0'
 __all__ = ['UnreadableFileError', 'FileTypeError', 'MediaFile']
 
 log = logging.getLogger(__name__)
 
 # Human-readable type names.
 TYPES = {
     'mp3':  'MP3',
@@ -1717,15 +1718,16 @@
     def readable_fields(cls):
         """Get all metadata fields: the writable ones from
         :meth:`fields` and also other audio properties.
         """
         for property in cls.fields():
             yield property
         for property in ('length', 'samplerate', 'bitdepth', 'bitrate',
-                         'channels', 'format'):
+                         'bitrate_mode', 'channels', 'encoder_info',
+                         'encoder_settings', 'format'):
             yield property
 
     @classmethod
     def add_field(cls, name, descriptor):
         """Add a field to store custom tags.
 
         :param name: the name of the property the field is accessed
@@ -2323,10 +2325,46 @@
             # is the case for all of the lossless formats.)
             if not self.length:
                 # Avoid division by zero if length is not available.
                 return 0
             return int(self.filesize * 8 / self.length)
 
     @property
+    def bitrate_mode(self):
+        """The mode of the bitrate used in the audio coding
+        (a string, eg. "CBR", "VBR" or "ABR").
+        Only available for the MP3 file format (empty where unavailable).
+        """
+        if hasattr(self.mgfile.info, 'bitrate_mode'):
+            return {
+                mutagen.mp3.BitrateMode.CBR: 'CBR',
+                mutagen.mp3.BitrateMode.VBR: 'VBR',
+                mutagen.mp3.BitrateMode.ABR: 'ABR',
+            }.get(self.mgfile.info.bitrate_mode, '')
+        else:
+            return ''
+
+    @property
+    def encoder_info(self):
+        """The name and/or version of the encoder used
+        (a string, eg. "LAME 3.97.0").
+        Only available for some formats (empty where unavailable).
+        """
+        if hasattr(self.mgfile.info, 'encoder_info'):
+            return self.mgfile.info.encoder_info
+        else:
+            return ''
+
+    @property
+    def encoder_settings(self):
+        """A guess of the settings used for the encoder (a string, eg. "-V2").
+        Only available for the MP3 file format (empty where unavailable).
+        """
+        if hasattr(self.mgfile.info, 'encoder_settings'):
+            return self.mgfile.info.encoder_settings
+        else:
+            return ''
+
+    @property
     def format(self):
         """A string describing the file format/codec."""
         return TYPES[self.type]
```

### Comparing `mediafile-0.8.1/pyproject.toml` & `mediafile-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/setup.cfg` & `mediafile-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/_common.py` & `mediafile-0.9.0/test/_common.py`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/backup.wav` & `mediafile-0.9.0/test/rsrc/backup.wav`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/bpm.mp3` & `mediafile-0.9.0/test/rsrc/bpm.mp3`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/coverart.ogg` & `mediafile-0.9.0/test/rsrc/coverart.ogg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/date_with_slashes.ogg` & `mediafile-0.9.0/test/rsrc/date_with_slashes.ogg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/discc.ogg` & `mediafile-0.9.0/test/rsrc/discc.ogg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.aiff` & `mediafile-0.9.0/test/rsrc/empty.aiff`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.alac.m4a` & `mediafile-0.9.0/test/rsrc/empty.alac.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.ape` & `mediafile-0.9.0/test/rsrc/empty.ape`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.dsf` & `mediafile-0.9.0/test/rsrc/empty.dsf`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.flac` & `mediafile-0.9.0/test/rsrc/empty.flac`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.m4a` & `mediafile-0.9.0/test/rsrc/empty.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.mp3` & `mediafile-0.9.0/test/rsrc/empty.mp3`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.mpc` & `mediafile-0.9.0/test/rsrc/empty.mpc`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.ogg` & `mediafile-0.9.0/test/rsrc/empty.ogg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.opus` & `mediafile-0.9.0/test/rsrc/empty.opus`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.wav` & `mediafile-0.9.0/test/rsrc/empty.wav`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.wma` & `mediafile-0.9.0/test/rsrc/empty.wma`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/empty.wv` & `mediafile-0.9.0/test/rsrc/empty.wv`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/emptylist.mp3` & `mediafile-0.9.0/test/rsrc/emptylist.mp3`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.aiff` & `mediafile-0.9.0/test/rsrc/full.aiff`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.alac.m4a` & `mediafile-0.9.0/test/rsrc/full.alac.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.ape` & `mediafile-0.9.0/test/rsrc/full.ape`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.dsf` & `mediafile-0.9.0/test/rsrc/full.dsf`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.flac` & `mediafile-0.9.0/test/rsrc/full.flac`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.m4a` & `mediafile-0.9.0/test/rsrc/full.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.mp3` & `mediafile-0.9.0/test/rsrc/full.mp3`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.mpc` & `mediafile-0.9.0/test/rsrc/full.mpc`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.ogg` & `mediafile-0.9.0/test/rsrc/full.ogg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.opus` & `mediafile-0.9.0/test/rsrc/full.opus`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.wav` & `mediafile-0.9.0/test/rsrc/full.wav`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.wma` & `mediafile-0.9.0/test/rsrc/full.wma`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/full.wv` & `mediafile-0.9.0/test/rsrc/full.wv`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/image-2x3.jpg` & `mediafile-0.9.0/test/rsrc/image-2x3.jpg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/image.ape` & `mediafile-0.9.0/test/rsrc/image.ape`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/image.flac` & `mediafile-0.9.0/test/rsrc/image.flac`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/image.m4a` & `mediafile-0.9.0/test/rsrc/image.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/image.mp3` & `mediafile-0.9.0/test/rsrc/image.mp3`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/image.ogg` & `mediafile-0.9.0/test/rsrc/image.ogg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/image.wma` & `mediafile-0.9.0/test/rsrc/image.wma`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/image_unknown_type.mp3` & `mediafile-0.9.0/test/rsrc/image_unknown_type.mp3`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/oldape.ape` & `mediafile-0.9.0/test/rsrc/oldape.ape`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/only-magic-bytes.jpg` & `mediafile-0.9.0/test/rsrc/only-magic-bytes.jpg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/partial.flac` & `mediafile-0.9.0/test/rsrc/partial.flac`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/partial.m4a` & `mediafile-0.9.0/test/rsrc/partial.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/partial.mp3` & `mediafile-0.9.0/test/rsrc/partial.mp3`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/pure.wma` & `mediafile-0.9.0/test/rsrc/pure.wma`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/read_only_tag.m4a` & `mediafile-0.9.0/test/rsrc/read_only_tag.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/soundcheck-nonascii.m4a` & `mediafile-0.9.0/test/rsrc/soundcheck-nonascii.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/space_time.mp3` & `mediafile-0.9.0/test/rsrc/space_time.mp3`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/t_time.m4a` & `mediafile-0.9.0/test/rsrc/t_time.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.aiff` & `mediafile-0.9.0/test/rsrc/unparseable.aiff`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.alac.m4a` & `mediafile-0.9.0/test/rsrc/unparseable.alac.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.ape` & `mediafile-0.9.0/test/rsrc/unparseable.ape`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.dsf` & `mediafile-0.9.0/test/rsrc/unparseable.dsf`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.flac` & `mediafile-0.9.0/test/rsrc/unparseable.flac`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.m4a` & `mediafile-0.9.0/test/rsrc/unparseable.m4a`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.mp3` & `mediafile-0.9.0/test/rsrc/unparseable.mp3`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.mpc` & `mediafile-0.9.0/test/rsrc/unparseable.mpc`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.ogg` & `mediafile-0.9.0/test/rsrc/unparseable.ogg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.opus` & `mediafile-0.9.0/test/rsrc/unparseable.opus`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.wav` & `mediafile-0.9.0/test/rsrc/unparseable.wav`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.wma` & `mediafile-0.9.0/test/rsrc/unparseable.wma`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/unparseable.wv` & `mediafile-0.9.0/test/rsrc/unparseable.wv`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/rsrc/year.ogg` & `mediafile-0.9.0/test/rsrc/year.ogg`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/test/test_mediafile.py` & `mediafile-0.9.0/test/test_mediafile.py`

 * *Files 12% similar despite different names*

```diff
@@ -757,31 +757,49 @@
 class MP3Test(ReadWriteTestBase, PartialTestMixin,
               ExtendedImageStructureTestMixin,
               unittest.TestCase):
     extension = 'mp3'
     audio_properties = {
         'length': 1.0,
         'bitrate': 80000,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': 'MP3',
         'samplerate': 44100,
         'bitdepth': 0,
         'channels': 1,
     }
 
     def test_unknown_apic_type(self):
         mediafile = self._mediafile_fixture('image_unknown_type')
         self.assertEqual(mediafile.images[0].type, ImageType.other)
 
+    def test_bitrate_mode(self):
+        mediafile = self._mediafile_fixture('cbr')
+        self.assertEqual(mediafile.bitrate_mode, 'CBR')
+
+    def test_encoder_info(self):
+        mediafile = self._mediafile_fixture('cbr')
+        self.assertEqual(mediafile.encoder_info, 'LAME 3.100.0+')
+
+    def test_encoder_settings(self):
+        mediafile = self._mediafile_fixture('cbr')
+        self.assertEqual(mediafile.encoder_settings, '-b 80')
+
 
 class MP4Test(ReadWriteTestBase, PartialTestMixin,
               ImageStructureTestMixin, unittest.TestCase):
     extension = 'm4a'
     audio_properties = {
         'length': 1.0,
         'bitrate': 64000,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': 'AAC',
         'samplerate': 44100,
         'bitdepth': 16,
         'channels': 2,
     }
 
     def test_add_tiff_image_fails(self):
@@ -795,39 +813,48 @@
 
 
 class AlacTest(ReadWriteTestBase, unittest.TestCase):
     extension = 'alac.m4a'
     audio_properties = {
         'length': 1.0,
         'bitrate': 21830,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         # 'format': 'ALAC',
         'samplerate': 44100,
         'bitdepth': 16,
         'channels': 1,
     }
 
 
 class MusepackTest(ReadWriteTestBase, unittest.TestCase):
     extension = 'mpc'
     audio_properties = {
         'length': 1.0,
         'bitrate': 24023,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'Musepack',
         'samplerate': 44100,
         'bitdepth': 0,
         'channels': 2,
     }
 
 
 class WMATest(ReadWriteTestBase, ExtendedImageStructureTestMixin,
               unittest.TestCase):
     extension = 'wma'
     audio_properties = {
         'length': 1.0,
         'bitrate': 128000,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'Windows Media',
         'samplerate': 44100,
         'bitdepth': 0,
         'channels': 1,
     }
 
     def test_write_genre_list_get_first(self):
@@ -848,14 +875,17 @@
 
 class OggTest(ReadWriteTestBase, ExtendedImageStructureTestMixin,
               unittest.TestCase):
     extension = 'ogg'
     audio_properties = {
         'length': 1.0,
         'bitrate': 48000,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'OGG',
         'samplerate': 44100,
         'bitdepth': 0,
         'channels': 1,
     }
 
     def test_read_date_from_year_tag(self):
@@ -892,75 +922,93 @@
 class FlacTest(ReadWriteTestBase, PartialTestMixin,
                ExtendedImageStructureTestMixin,
                unittest.TestCase):
     extension = 'flac'
     audio_properties = {
         'length': 1.0,
         'bitrate': 108688,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'FLAC',
         'samplerate': 44100,
         'bitdepth': 16,
         'channels': 1,
     }
 
 
 class ApeTest(ReadWriteTestBase, ExtendedImageStructureTestMixin,
               unittest.TestCase):
     extension = 'ape'
     audio_properties = {
         'length': 1.0,
         'bitrate': 112608,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'APE',
         'samplerate': 44100,
         'bitdepth': 16,
         'channels': 1,
     }
 
 
 class WavpackTest(ReadWriteTestBase, unittest.TestCase):
     extension = 'wv'
     audio_properties = {
         'length': 1.0,
         'bitrate': 109312,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'WavPack',
         'samplerate': 44100,
         'bitdepth': 16 if mutagen.version >= (1, 45, 0) else 0,
         'channels': 1,
     }
 
 
 class OpusTest(ReadWriteTestBase, unittest.TestCase):
     extension = 'opus'
     audio_properties = {
         'length': 1.0,
         'bitrate': 66792,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'Opus',
         'samplerate': 48000,
         'bitdepth': 0,
         'channels': 1,
     }
 
 
 class AIFFTest(ReadWriteTestBase, unittest.TestCase):
     extension = 'aiff'
     audio_properties = {
         'length': 1.0,
         'bitrate': 705600,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'AIFF',
         'samplerate': 44100,
         'bitdepth': 16,
         'channels': 1,
     }
 
 
 class WAVETest(ReadWriteTestBase, unittest.TestCase):
     extension = 'wav'
     audio_properties = {
         'length': 1.0,
         'bitrate': 88200,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'WAVE',
         'samplerate': 44100,
         'bitdepth': 16,
         'channels': 1,
     }
 
     full_initial_tags = {
@@ -1029,14 +1077,17 @@
 
 @unittest.skipIf(not HAVE_DSF, "Mutagen does not have DSF support")
 class DSFTest(ReadWriteTestBase, unittest.TestCase):
     extension = 'dsf'
     audio_properties = {
         'length': 0.01,
         'bitrate': 11289600,
+        'bitrate_mode': '',
+        'encoder_info': '',
+        'encoder_settings': '',
         'format': u'DSD Stream File',
         'samplerate': 5644800,
         'bitdepth': 1,
         'channels': 2,
     }
```

### Comparing `mediafile-0.8.1/test/test_mediafile_edge.py` & `mediafile-0.9.0/test/test_mediafile_edge.py`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/tox.ini` & `mediafile-0.9.0/tox.ini`

 * *Files identical despite different names*

### Comparing `mediafile-0.8.1/setup.py` & `mediafile-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = \
 ['six>=1.9', 'mutagen>=1.45']
 
 extras_require = \
 {'test': ['tox']}
 
 setup(name='mediafile',
-      version='0.8.1',
+      version='0.9.0',
       description="Handles low-level interfacing for files' tags. Wraps Mutagen to",
       author='Adrian Sampson',
       author_email='adrian@radbox.org',
       url='https://github.com/beetbox/mediafile',
       py_modules=['mediafile'],
       install_requires=install_requires,
       extras_require=extras_require,
```

