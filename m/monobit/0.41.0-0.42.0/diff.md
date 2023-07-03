# Comparing `tmp/monobit-0.41.0.tar.gz` & `tmp/monobit-0.42.0.tar.gz`

## Comparing `monobit-0.41.0.tar` & `monobit-0.42.0.tar`

### file list

```diff
@@ -1,516 +1,517 @@
--rw-r--r--   0        0        0    27029 2020-02-02 00:00:00.000000 monobit-0.41.0/YAFF.md
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.41.0/banner.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.41.0/convert.py
--rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.41.0/explore.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/__init__.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/basetypes.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/binary.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/cachedprops.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/chart.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/constants.py
--rw-r--r--   0        0        0    58243 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/encoding.py
--rw-r--r--   0        0        0    47906 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/font.py
--rw-r--r--   0        0        0    31912 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/glyph.py
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/glyphmap.py
--rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/labels.py
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/magic.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/pack.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/properties.py
--rw-r--r--   0        0        0    24178 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/raster.py
--rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/renderer.py
--rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/scripting.py
--rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/storage.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/streams.py
--rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/struct.py
--rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/taggers.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/vector.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/__init__.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/adobe/ReadMe.txt
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/adobe/stdenc.txt
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/adobe/symbol.txt
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/adobe/zdingbat.txt
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/agl/LICENSE.md
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/agl/README.md
--rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/agl/aglfn.txt
--rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/agl/glyphlist.txt
--rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ARABIC.TXT
--rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CELTIC.TXT
--rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CENTEURO.TXT
--rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CHINSIMP.TXT
--rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CHINTRAD.TXT
--rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CORPCHAR.TXT
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CROATIAN.TXT
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CYRILLIC.TXT
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/DEVANAGA.TXT
--rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/DINGBATS.TXT
--rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/FARSI.TXT
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/GAELIC.TXT
--rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/GREEK.TXT
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/GUJARATI.TXT
--rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/GURMUKHI.TXT
--rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/HEBREW.TXT
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ICELAND.TXT
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/INUIT.TXT
--rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/JAPANESE.TXT
--rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/KEYBOARD.TXT
--rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/KOREAN.TXT
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ROMAN.TXT
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ROMANIAN.TXT
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ReadMe.txt
--rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/SYMBOL.TXT
--rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/THAI.TXT
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/TURKISH.TXT
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/UKRAINE.TXT
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/README.md
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/bulgarian-mik.txt
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/cp866.txt
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/gost19768-87.txt
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/hp-roman8.txt
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi-0.txt
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi-7.txt
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-a.txt
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-b.txt
--rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-e.txt
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-f.txt
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-r.txt
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-u.txt
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-ca
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-ca2
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-cn
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-cu
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-de
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-dk
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-es
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-es2
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-fr
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-gb
--rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-hu
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-it
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-jp
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-jp-ocr-b
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-kr
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-us
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-yu
--rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/jis_x0201
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/x0201-7
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-ethiopic.map
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-ipa.map
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-is13194.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-lviscii.map
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-sisheng.map
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-tibetan.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-uviscii.map
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/README.md
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/evertype/ARMENIAN.TXT
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/evertype/GEORGIAN.TXT
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/evertype/README.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1116.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1117.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1118.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1119.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1125.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/113.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1131.ucp
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30000.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30001.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30002.ucp
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30003.ucp
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30004.ucp
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30005.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30006.ucp
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30007.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30008.ucp
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30009.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30010.ucp
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30011.ucp
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30013.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30014.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30015.ucp
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30016.ucp
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30017.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30018.ucp
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30019.ucp
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30020.ucp
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30021.ucp
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30022.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30023.ucp
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30024.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30025.ucp
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30026.ucp
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30027.ucp
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30028.ucp
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30029.ucp
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30030.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30031.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30032.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30033.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30034.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30039.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30040.ucp
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3021.ucp
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3845.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3846.ucp
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3848.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/437.ucp
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/57781.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/58152.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/58210.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/58335.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/59234.ucp
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/59829.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/60258.ucp
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/60853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/61282.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/62306.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/667.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/668.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/737.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/770.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/771.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/772.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/773.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/774.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/775.ucp
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/777.ucp
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/778.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/790.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/808.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/848.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/849.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/850.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/851.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/852.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/855.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/856.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/857.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/858.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/859.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/860.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/861.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/862.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/863.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/864.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/865.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/866.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/867.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/869.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/872.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/895.ucp
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/899.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/991.ucp
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/__init__.py
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iana/Amiga-1251
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iana/PTCP154
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iana/README.md
--rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
--rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
--rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
--rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/readme.txt
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/README.md
--rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
--rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/cns-11643-1992.ucm
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
--rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm
--rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm
--rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/windows-1361-2000.ucm
--rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/windows-936-2000.ucm
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-1.TXT
--rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-10.TXT
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-11.TXT
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-13.TXT
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-14.TXT
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-15.TXT
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-16.TXT
--rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-2.TXT
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-3.TXT
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-4.TXT
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-5.TXT
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-6.TXT
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-7.TXT
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-8.TXT
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-9.TXT
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/ReadMe.txt
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/AMSCPC.TXT
--rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/AMSCPM.TXT
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT
--rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8II.TXT
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT
--rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARISTI.TXT
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARISTV.TXT
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/C64IALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/C64IPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/C64VALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/C64VPRI.TXT
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/COCOICHG.TXT
--rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CPETIALT.TXT
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CPETVALT.TXT
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CVICIALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CVICVALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT
--rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/MINITLG0.TXT
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/MINITLG1.TXT
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/MSX.TXT
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ORICG0.TXT
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ORICG1.TXT
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/RISCEFF.TXT
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSB.TXT
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSI.TXT
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSV.TXT
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ReadMe.txt
--rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TI994A.TXT
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
--rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
--rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
--rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZX80.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZX81.TXT
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
--rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/c0-pictures.txt
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/currency-sign-0x9c.ucp
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/currency-sign-0xdb.ucp
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/dec-vt100.ucp
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/hp48.txt
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/ibm897graph.ucp
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/iso2047.txt
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/mac-system.ucp
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/ms-linedraw.txt
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/russup3.ucp
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/russup4ac.ucp
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/russup4na.ucp
--rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/windows-1.0.txt
--rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/windows-2.0.txt
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/windows-3.1.txt
--rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
--rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
--rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
--rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/GREEK.TXT
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP437.TXT
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP737.TXT
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP775.TXT
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP850.TXT
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP852.TXT
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP855.TXT
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP857.TXT
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP860.TXT
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP861.TXT
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP862.TXT
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP863.TXT
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP864.TXT
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP865.TXT
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP866.TXT
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP869.TXT
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP874.TXT
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
--rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
--rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
--rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
--rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
--rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT
--rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/ATARIST.TXT
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/CP1006.TXT
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/CP424.TXT
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/CP856.TXT
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/GSM0338.TXT
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/IBMGRAPH.TXT
--rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/JIS0208.TXT
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/KOI8-R.TXT
--rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/KOI8-U.TXT
--rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/KPS9566.TXT
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/KZ1048.TXT
--rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/NEXTSTEP.TXT
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/README.md
--rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/SGML.TXT
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/dashen-map.txt
--rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/ibm-ugl.txt
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/ALTVAR.TXT
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-7.TXT
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-8.TXT
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/DECMCS.TXT
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/GEO-ITA.TXT
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/GEO-PS.TXT
--rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/KOI8RU.TXT
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/OSNOVAR.TXT
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/README.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/TIS620.TXT
--rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/moztw/big5_2003-b2u.txt
--rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/moztw/eten.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/moztw/url
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/python/README.md
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/python/TCVN5712-1.TXT
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/python/TCVN5712-2.TXT
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/python/TCVN5712-3.TXT
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/vietstd/unicode.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/vietstd/url
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/vietstd/viscii1.1.txt
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/README.md
--rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/abicomp.html
--rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/brascii.html
--rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/cp853.html
--rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/cwi2.html
--rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/dec-special.html
--rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/dec-technical.html
--rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/gem.html
--rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/kamenicky.html
--rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/lics.html
--rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/mattel-aquarius.html
--rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/mazovia.html
--rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/pascii.html
--rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/ventura.html
--rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/windows-1252.html
--rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/wingdings.html
--rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/wiscii.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/README.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-0.enc
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-1.enc
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-2.enc
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/mulelao-1.enc
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/suneu-greek.enc
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/viscii1.1-1.enc
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/__init__.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/compressors.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/container.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/directory.py
--rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/mac.py
--rw-r--r--   0        0        0    15795 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/source.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/tar.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/zip.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/__init__.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/amiga.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/bbc.py
--rw-r--r--   0        0        0    40817 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/bmfont.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/borland.py
--rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/cpi.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/daisydot.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/dashen.py
--rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/dec.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/dosstart.py
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/figlet.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/fontx.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/fzx.py
--rw-r--r--   0        0        0    26408 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/gdos.py
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/geos.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/hurt.py
--rw-r--r--   0        0        0    10961 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/image.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mousegraphics.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mzfon.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/nearlyraw.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/palm.py
--rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/pcl.py
--rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/pcpaint.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/pdf.py
--rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/pkfont.py
--rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/prebuilt.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/printshop.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/psf.py
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/raw.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/signum.py
--rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/svg.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/vfont.py
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xerox.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/__init__.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/dfont.py
--rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/fond.py
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/iigs.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/lisa.py
--rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/nfnt.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/os2/__init__.py
--rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/os2/gpifont.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/os2/lx.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/os2/ne.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/__init__.py
--rw-r--r--   0        0        0    30773 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/sfnt.py
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/sfnt_writer.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/E_B_S_C_.py
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/_b_d_a_t.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/_b_h_e_d.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/_b_l_o_c.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/text/__init__.py
--rw-r--r--   0        0        0    16758 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/text/draw.py
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/text/hex.py
--rw-r--r--   0        0        0    14275 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/text/yaff.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/LICENSE.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/__init__.py
--rw-r--r--   0        0        0    33222 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/fnt.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/mz.py
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/ne.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/pe.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/__init__.py
--rw-r--r--   0        0        0    18398 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/bdf.py
--rw-r--r--   0        0        0    18469 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/hbf.py
--rw-r--r--   0        0        0    33745 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/pcf.py
--rw-r--r--   0        0        0    25969 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/xlfd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/scripts/__init__.py
--rwxr-xr-x   0        0        0     9148 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/scripts/banner.py
--rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/scripts/convert.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.41.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.41.0/LICENSE
--rw-r--r--   0        0        0    18353 2020-02-02 00:00:00.000000 monobit-0.41.0/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.41.0/pyproject.toml
--rw-r--r--   0        0        0    20306 2020-02-02 00:00:00.000000 monobit-0.41.0/PKG-INFO
+-rw-r--r--   0        0        0    27029 2020-02-02 00:00:00.000000 monobit-0.42.0/YAFF.md
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.42.0/banner.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.42.0/convert.py
+-rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.42.0/explore.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/__init__.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/basetypes.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/binary.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/blocks.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/cachedprops.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/chart.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/constants.py
+-rw-r--r--   0        0        0    58243 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/encoding.py
+-rw-r--r--   0        0        0    48238 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/font.py
+-rw-r--r--   0        0        0    34079 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/glyph.py
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/glyphmap.py
+-rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/labels.py
+-rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/magic.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/pack.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/properties.py
+-rw-r--r--   0        0        0    22774 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/raster.py
+-rw-r--r--   0        0        0    13332 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/renderer.py
+-rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/scripting.py
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/storage.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/streams.py
+-rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/struct.py
+-rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/taggers.py
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/vector.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/__init__.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/adobe/ReadMe.txt
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/adobe/stdenc.txt
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/adobe/symbol.txt
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/adobe/zdingbat.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/agl/LICENSE.md
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/agl/README.md
+-rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/agl/aglfn.txt
+-rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/agl/glyphlist.txt
+-rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/ARABIC.TXT
+-rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/CELTIC.TXT
+-rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/CENTEURO.TXT
+-rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/CHINSIMP.TXT
+-rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/CHINTRAD.TXT
+-rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/CORPCHAR.TXT
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/CROATIAN.TXT
+-rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/CYRILLIC.TXT
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/DEVANAGA.TXT
+-rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/DINGBATS.TXT
+-rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/FARSI.TXT
+-rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/GAELIC.TXT
+-rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/GREEK.TXT
+-rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/GUJARATI.TXT
+-rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/GURMUKHI.TXT
+-rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/HEBREW.TXT
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/ICELAND.TXT
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/INUIT.TXT
+-rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/JAPANESE.TXT
+-rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/KEYBOARD.TXT
+-rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/KOREAN.TXT
+-rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/ROMAN.TXT
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/ROMANIAN.TXT
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/ReadMe.txt
+-rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/SYMBOL.TXT
+-rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/THAI.TXT
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/TURKISH.TXT
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/apple/UKRAINE.TXT
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/README.md
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/bulgarian-mik.txt
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/cp866.txt
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/gost19768-87.txt
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/hp-roman8.txt
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/koi-0.txt
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/koi-7.txt
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/koi8-a.txt
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/koi8-b.txt
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/koi8-e.txt
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/koi8-f.txt
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/koi8-r.txt
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/czyborra/koi8-u.txt
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-ca
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-ca2
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-cn
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-cu
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-de
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-dk
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-es
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-es2
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-fr
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-gb
+-rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-hu
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-it
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-jp
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-jp-ocr-b
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-kr
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-us
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/iso646-yu
+-rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/jis_x0201
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/dkuug/x0201-7
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/emacs/MULE-ethiopic.map
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/emacs/MULE-ipa.map
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/emacs/MULE-is13194.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/emacs/MULE-lviscii.map
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/emacs/MULE-sisheng.map
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/emacs/MULE-tibetan.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/emacs/MULE-uviscii.map
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/emacs/README.md
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/evertype/ARMENIAN.TXT
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/evertype/GEORGIAN.TXT
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/evertype/README.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/1116.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/1117.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/1118.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/1119.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/1125.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/113.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/1131.ucp
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30000.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30001.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30002.ucp
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30003.ucp
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30004.ucp
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30005.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30006.ucp
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30007.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30008.ucp
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30009.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30010.ucp
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30011.ucp
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30013.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30014.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30015.ucp
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30016.ucp
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30017.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30018.ucp
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30019.ucp
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30020.ucp
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30021.ucp
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30022.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30023.ucp
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30024.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30025.ucp
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30026.ucp
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30027.ucp
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30028.ucp
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30029.ucp
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30030.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30031.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30032.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30033.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30034.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30039.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/30040.ucp
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/3012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/3021.ucp
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/3845.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/3846.ucp
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/3848.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/437.ucp
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/57781.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/58152.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/58210.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/58335.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/59234.ucp
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/59829.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/60258.ucp
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/60853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/61282.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/62306.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/667.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/668.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/737.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/770.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/771.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/772.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/773.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/774.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/775.ucp
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/777.ucp
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/778.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/790.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/808.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/848.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/849.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/850.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/851.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/852.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/855.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/856.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/857.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/858.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/859.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/860.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/861.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/862.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/863.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/864.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/865.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/866.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/867.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/869.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/872.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/895.ucp
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/899.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/991.ucp
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/freedos/__init__.py
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iana/Amiga-1251
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iana/PTCP154
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iana/README.md
+-rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
+-rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
+-rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
+-rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/ibm-cdra/readme.txt
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/README.md
+-rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
+-rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/cns-11643-1992.ucm
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
+-rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm
+-rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm
+-rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/windows-1361-2000.ucm
+-rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/icu/windows-936-2000.ucm
+-rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-1.TXT
+-rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-10.TXT
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-11.TXT
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-13.TXT
+-rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-14.TXT
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-15.TXT
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-16.TXT
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-2.TXT
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-3.TXT
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-4.TXT
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-5.TXT
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-6.TXT
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-7.TXT
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-8.TXT
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/8859-9.TXT
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/iso-8859/ReadMe.txt
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/AMSCPC.TXT
+-rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/AMSCPM.TXT
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ATARI8II.TXT
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT
+-rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ATARISTI.TXT
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ATARISTV.TXT
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/C64IALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/C64IPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/C64VALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/C64VPRI.TXT
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/COCOICHG.TXT
+-rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/CPETIALT.TXT
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/CPETVALT.TXT
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/CVICIALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/CVICVALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT
+-rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/MINITLG0.TXT
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/MINITLG1.TXT
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/MSX.TXT
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ORICG0.TXT
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ORICG1.TXT
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/RISCEFF.TXT
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/RISCOSB.TXT
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/RISCOSI.TXT
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/RISCOSV.TXT
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ReadMe.txt
+-rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TI994A.TXT
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
+-rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ZX80.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ZX81.TXT
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/c0-pictures.txt
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/currency-sign-0x9c.ucp
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/currency-sign-0xdb.ucp
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/dec-vt100.ucp
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/hp48.txt
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/ibm897graph.ucp
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/iso2047.txt
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/mac-system.ucp
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/ms-linedraw.txt
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/russup3.ucp
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/russup4ac.ucp
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/russup4na.ucp
+-rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/windows-1.0.txt
+-rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/windows-2.0.txt
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/manual/windows-3.1.txt
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
+-rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
+-rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/MAC/GREEK.TXT
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP437.TXT
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP737.TXT
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP775.TXT
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP850.TXT
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP852.TXT
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP855.TXT
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP857.TXT
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP860.TXT
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP861.TXT
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP862.TXT
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP863.TXT
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP864.TXT
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP865.TXT
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP866.TXT
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP869.TXT
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/PC/CP874.TXT
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
+-rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
+-rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
+-rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
+-rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
+-rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT
+-rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/ATARIST.TXT
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/CP1006.TXT
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/CP424.TXT
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/CP856.TXT
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/GSM0338.TXT
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/IBMGRAPH.TXT
+-rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/JIS0208.TXT
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/KOI8-R.TXT
+-rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/KOI8-U.TXT
+-rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/KPS9566.TXT
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/KZ1048.TXT
+-rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/NEXTSTEP.TXT
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/README.md
+-rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/SGML.TXT
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/dashen-map.txt
+-rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/misc/ibm-ugl.txt
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/ALTVAR.TXT
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/ARMSCII-7.TXT
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/ARMSCII-8.TXT
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/DECMCS.TXT
+-rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/GEO-ITA.TXT
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/GEO-PS.TXT
+-rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/KOI8RU.TXT
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/OSNOVAR.TXT
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/README.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/mleisher/TIS620.TXT
+-rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/moztw/big5_2003-b2u.txt
+-rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/moztw/eten.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/moztw/url
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/python/README.md
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/python/TCVN5712-1.TXT
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/python/TCVN5712-2.TXT
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/python/TCVN5712-3.TXT
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/vietstd/unicode.html
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/vietstd/url
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/vietstd/viscii1.1.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/README.md
+-rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/abicomp.html
+-rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/brascii.html
+-rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/cp853.html
+-rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/cwi2.html
+-rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/dec-special.html
+-rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/dec-technical.html
+-rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/gem.html
+-rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/kamenicky.html
+-rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/lics.html
+-rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/mattel-aquarius.html
+-rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/mazovia.html
+-rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/pascii.html
+-rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/ventura.html
+-rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/windows-1252.html
+-rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/wingdings.html
+-rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/wikipedia/wiscii.html
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/xfonts/README.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/xfonts/mulearabic-0.enc
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/xfonts/mulearabic-1.enc
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/xfonts/mulearabic-2.enc
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/xfonts/mulelao-1.enc
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/xfonts/suneu-greek.enc
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/charmaps/xfonts/viscii1.1-1.enc
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/containers/__init__.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/containers/compressors.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/containers/container.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/containers/directory.py
+-rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/containers/mac.py
+-rw-r--r--   0        0        0    15795 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/containers/source.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/containers/tar.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/containers/zip.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/__init__.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/amiga.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/bbc.py
+-rw-r--r--   0        0        0    40817 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/bmfont.py
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/borland.py
+-rw-r--r--   0        0        0    22580 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/cpi.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/daisydot.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/dashen.py
+-rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/dec.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/dosstart.py
+-rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/figlet.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/fontx.py
+-rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/fzx.py
+-rw-r--r--   0        0        0    26219 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/gdos.py
+-rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/geos.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/hurt.py
+-rw-r--r--   0        0        0    10961 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/image.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/mousegraphics.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/mzfon.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/nearlyraw.py
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/palm.py
+-rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/pcl.py
+-rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/pcpaint.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/pdf.py
+-rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/pkfont.py
+-rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/prebuilt.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/printshop.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/psf.py
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/raw.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/signum.py
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/svg.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/vfont.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/xerox.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/mac/__init__.py
+-rw-r--r--   0        0        0    21349 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/mac/dfont.py
+-rw-r--r--   0        0        0    29289 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/mac/fond.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/mac/iigs.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/mac/lisa.py
+-rw-r--r--   0        0        0    27120 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/mac/nfnt.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/os2/__init__.py
+-rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/os2/gpifont.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/os2/lx.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/os2/ne.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/sfnt/__init__.py
+-rw-r--r--   0        0        0    30762 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/sfnt/sfnt.py
+-rw-r--r--   0        0        0    17916 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/sfnt/sfnt_writer.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/sfnt/fonttools/E_B_S_C_.py
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/sfnt/fonttools/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/sfnt/fonttools/_b_d_a_t.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/sfnt/fonttools/_b_h_e_d.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/sfnt/fonttools/_b_l_o_c.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/text/__init__.py
+-rw-r--r--   0        0        0    16751 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/text/draw.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/text/hex.py
+-rw-r--r--   0        0        0    14764 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/text/yaff.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/windows/LICENSE.md
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/windows/__init__.py
+-rw-r--r--   0        0        0    32356 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/windows/fnt.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/windows/mz.py
+-rw-r--r--   0        0        0    14160 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/windows/ne.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/windows/pe.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/xlfd/__init__.py
+-rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/xlfd/bdf.py
+-rw-r--r--   0        0        0    18217 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/xlfd/hbf.py
+-rw-r--r--   0        0        0    33895 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/xlfd/pcf.py
+-rw-r--r--   0        0        0    25950 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/formats/xlfd/xlfd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/scripts/__init__.py
+-rwxr-xr-x   0        0        0     9544 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/scripts/banner.py
+-rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.42.0/monobit/scripts/convert.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.42.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.42.0/LICENSE
+-rw-r--r--   0        0        0    18478 2020-02-02 00:00:00.000000 monobit-0.42.0/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.42.0/pyproject.toml
+-rw-r--r--   0        0        0    20431 2020-02-02 00:00:00.000000 monobit-0.42.0/PKG-INFO
```

### Comparing `monobit-0.41.0/YAFF.md` & `monobit-0.42.0/YAFF.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/explore.py` & `monobit-0.42.0/explore.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/__init__.py` & `monobit-0.42.0/monobit/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/basetypes.py` & `monobit-0.42.0/monobit/basetypes.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/binary.py` & `monobit-0.42.0/monobit/binary.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/cachedprops.py` & `monobit-0.42.0/monobit/cachedprops.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,31 +26,32 @@
         self._props = {}
 
     def __repr__(self):
         return (
             type(self).__name__
             + '(\n    ' +
             '\n    '.join(
-                f'{_k}={_v!r},' for _k, _v in self._props.items()
-                if not _k.startswith('_')
+                f'{_k}={_v!r},'
+                for _k, _v in self._props.items()
             )
             + '\n)'
         )
 
     def _get_property(self, field):
         try:
             return self._props[field]
         except KeyError:
             return type(self)._defaults[field]
 
     def __getattr__(self, field):
-        try:
-            return self._get_property(field)
-        except KeyError:
-            pass
+        if not field.startswith('_'):
+            try:
+                return self._get_property(field)
+            except KeyError:
+                pass
         raise AttributeError(field)
 
     @staticmethod
     def get_converters(typeclass):
         # types, converters and default values for overriding/custom properties
         return {
             _field: CONVERTERS.get(_type, _type)
```

### Comparing `monobit-0.41.0/monobit/chart.py` & `monobit-0.42.0/monobit/chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,19 @@
     """Create font chart matrix."""
     font = font.label(codepoint_from=font.encoding)
     font = font.equalise_horizontal()
     if not codepoint_range:
         codepoints = font.get_codepoints()
         if not codepoints:
             raise ValueError('No codepoint labels found.')
-        codepoint_range = int(min(codepoints)), int(max(codepoints))
+        codepoint_range = (
+            # start at a codepoint that is a multple of the number of columns
+            columns * (int(min(codepoints)) // columns),
+            int(max(codepoints))
+        )
     # make contiguous
     glyphs = tuple(
         font.get_glyph(_codepoint, missing='empty')
         for _codepoint in range(codepoint_range[0], codepoint_range[1]+1)
     )
     font = font.modify(glyphs)
     glyph_map = grid_map(
```

### Comparing `monobit-0.41.0/monobit/encoding.py` & `monobit-0.42.0/monobit/encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1045,27 +1045,27 @@
         return b''
 
     def __repr__(self):
         """Representation."""
         return type(self).__name__ + '()'
 
 
-class Index(Encoder):
+class Indexer(Encoder):
     """Convert from index to ordinals."""
 
-    def __init__(self, code_range=(0,)):
+    def __init__(self, code_range='0-'):
         """Index converter."""
         super().__init__('index')
         # generator
         self._code_range = to_labels(code_range)
 
     @staticmethod
     def char(*labels):
         """Convert codepoint to character, return empty string if missing."""
-        raise TypeError('Can only use Index encoder to set codepoints, not character labels.')
+        raise TypeError('Can only use Indexer to set codepoints, not character labels.')
 
     def codepoint(self, *labels):
         """Convert character to codepoint."""
         try:
             return next(self._code_range)
         except StopIteration:
             return b''
@@ -1315,27 +1315,27 @@
         return initialiser
     if initialiser is None or not str(initialiser):
         return None
     initialiser = str(initialiser)
     # numeric ranges - interpreted as indexer
     if initialiser[:1].isdigit():
         initialiser = to_labels(initialiser)
-        return Index(code_range=initialiser)
+        return Indexer(code_range=initialiser)
     try:
         return charmaps[initialiser]
     except KeyError:
         pass
     try:
         return Charmap.load(initialiser)
     except NotFoundError:
         return None
 
 
 charmaps = CharmapRegistry()
-charmaps.add_type('index', Index)
+charmaps.add_type('index', Indexer)
 
 # unicode aliases
 charmaps.add_type('unicode', Unicode)
 charmaps.alias('ucs', 'unicode')
 charmaps.alias('iso10646', 'unicode')
 charmaps.alias('iso10646-1', 'unicode')
```

### Comparing `monobit-0.41.0/monobit/font.py` & `monobit-0.42.0/monobit/font.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from unicodedata import normalize
 
 from .scripting import scriptable, get_scriptables, Any
 from .glyph import Glyph
 from .raster import turn_method, NOT_SET
 from .basetypes import Coord, Bounds
 from .basetypes import to_int
-from .encoding import charmaps, encoder, EncodingName, Encoder
+from .encoding import charmaps, encoder, EncodingName, Encoder, Indexer
 from .taggers import tagger
 from .labels import Tag, Char, Codepoint, Label, to_label
 from .binary import ceildiv
 from .properties import extend_string
 from .cachedprops import HasProps, writable_property, checked_property
 from .taggers import tagmaps
 
@@ -377,36 +377,46 @@
         # where a glyph may take up 0, 1 or 2 cells.
         #
         # a _monospace_ font is a font where all glyphs have equal advance_width.
         #
         if not self.glyphs:
             return 'character-cell'
         if any(
-                _glyph.advance_width < 0 or _glyph.right_kerning
+                _glyph.right_kerning or _glyph.left_kerning
                 for _glyph in self.glyphs
             ):
             return 'proportional'
-        # don't count void glyphs (0 width and/or height)
-        # to determine whether it's monospace
-        advances = set(
-            _glyph.advance_width
-            for _glyph in self.glyphs if _glyph.advance_width
-        )
+        if self.has_vertical_metrics():
+            advances = set(
+                (_glyph.advance_width, _glyph.advance_height)
+                for _glyph in self.glyphs if _glyph.advance_width
+            )
+        else:
+            # don't count void glyphs (0 width and/or height)
+            # to determine whether it's monospace
+            advances = set(
+                _glyph.advance_width
+                for _glyph in self.glyphs if _glyph.advance_width
+            )
         if len(set(advances)) > 2:
             return 'proportional'
         monospaced = len(set(advances)) == 1
-        # horizontal rendering
         # check if all glyphs are rendered within the line height
         # if there are vertical overlaps, it is not a charcell font
-        if self.ink_bounds.top - self.ink_bounds.bottom > self.line_height:
+        if (
+                (self.ink_bounds.top - self.ink_bounds.bottom > self.line_height)
+                or self.has_vertical_metrics() and (
+                    self.ink_bounds.right - self.ink_bounds.left > self.line_width
+                )
+            ):
             return 'monospace' if monospaced else 'proportional'
         if all(
                 (-_g.left_bearing <= _g.padding.left)
                 and (-_g.right_bearing <= _g.padding.right)
-                # if no negative metrics, these will be zero and hence satisfied.
+                # if no vertical metrics, these will be zero and hence satisfied.
                 and (-_g.top_bearing <= _g.padding.top)
                 and (-_g.bottom_bearing <= _g.padding.bottom)
                 for _g in self.glyphs
             ):
             return 'character-cell' if monospaced else 'multi-cell'
         return 'monospace' if monospaced else 'proportional'
 
@@ -427,31 +437,31 @@
             self.raster.right - self.raster.left,
             self.raster.top - self.raster.bottom
         )
 
     @checked_property
     def cell_size(self):
         """Width, height of the character cell."""
-        if not self.glyphs or self.spacing == 'proportional':
+        if not self.glyphs or self.spacing not in ('character-cell', 'multi-cell'):
             return Coord(0, 0)
-        # smaller of the (at most two) advance widths is the cell size
-        # in a multi-cell font, some glyphs may take up two cells.
         if self.has_vertical_metrics():
             cells = tuple(
                 (_g.advance_width, _g.advance_height)
                 for _g in self.glyphs
             )
         else:
             cells = tuple(
                 (_g.advance_width, self.line_height)
                 for _g in self.glyphs
             )
         sizes = tuple(_c for _c in cells if all(_c))
         if not sizes:
             return Coord(0, 0)
+        # smaller of the (at most two) advance widths is the cell size
+        # in a multi-cell font, some glyphs may take up two cells.
         return Coord(*min(sizes))
 
     @checked_property
     def ink_bounds(self):
         """
         Minimum bounding box encompassing all glyphs at fixed origin,
         bottom-left origin cordinates.
@@ -984,17 +994,22 @@
         if nargs == 0 and self.encoding:
             char_from = encoder(self.encoding)
             if char_from is NOT_SET:
                 logging.warning(f'Encoding `{self.encoding}` not recognised.')
                 return self
         encoding = self.encoding
         if overwrite or not self.encoding:
-            if char_from is not NOT_SET and isinstance(char_from, Encoder):
+            # don't set encoding if we use a Tagger
+            if isinstance(char_from, Encoder):
                 encoding = char_from.name
-            elif codepoint_from is not NOT_SET and codepoint_from is not None:
+            # don't set encoding if we use an Indexer
+        elif (
+                isinstance(codepoint_from, Encoder)
+                and not isinstance(codepoint_from, Indexer)
+            ):
                 encoding = codepoint_from.name
         kwargs = dict(
             overwrite=overwrite,
             match_whitespace=match_whitespace,
             match_graphical=match_graphical,
         )
         if codepoint_from is not NOT_SET:
@@ -1233,33 +1248,29 @@
         # fix line-advances to ensure they remain unchanged
         return font.modify(
             line_height=self.line_height,
             line_width=self.line_width,
         )
 
     @scriptable
-    def reduce(self, *, adjust_metrics:bool=True, create_vertical_metrics:bool=False):
+    def reduce(self, *, adjust_metrics:bool=True):
         """
         Reduce glyphs to their bounding box.
 
         adjust_metrics: make the operation render-invariant (default: True)
-        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
-        create_vertical_metrics = (
-            create_vertical_metrics or self.has_vertical_metrics()
-        )
         font = self._apply_to_all_glyphs(
             Glyph.reduce,
             adjust_metrics=adjust_metrics,
-            create_vertical_metrics=create_vertical_metrics,
+            create_vertical_metrics=self.has_vertical_metrics(),
         )
         if not adjust_metrics:
             return font
-        if not create_vertical_metrics:
-            # fix line-advances to ensure they remain unchanged
+        # fix line-advances to ensure they remain unchanged
+        if not self.has_vertical_metrics():
             return font.modify(line_height=self.line_height)
         return font.modify(
             line_height=self.line_height, line_width=self.line_width
         )
 
     @scriptable
     def equalise_horizontal(self):
```

### Comparing `monobit-0.41.0/monobit/glyph.py` & `monobit-0.42.0/monobit/glyph.py`

 * *Files 19% similar despite different names*

```diff
@@ -339,15 +339,16 @@
                 if match_graphical and not self.is_blank() and char and not is_graphical(char):
                     return self
                 return self.modify(char=char)
         if tag_from is not NOT_SET:
             if not tag_from:
                 if overwrite:
                     return self.modify(tag=None)
-            return self.modify(tag=tag_from.tag(*labels))
+            elif overwrite or not self.tag:
+                return self.modify(tag=tag_from.tag(*labels))
         if comment_from is not NOT_SET:
             if not comment_from:
                 return self.modify(comment=None)
             return self.modify(comment=comment_from.comment(*labels))
         return self
 
     def append(
@@ -518,17 +519,17 @@
         """Return matrix of user-specified foreground and background objects."""
         return self._pixels.as_matrix(ink=ink, paper=paper)
 
     def as_text(self, *, ink='@', paper='.', start='', end='\n'):
         """Convert glyph to text."""
         return self._pixels.as_text(ink=ink, paper=paper, start=start, end=end)
 
-    def as_blocks(self):
+    def as_blocks(self, resolution=(2, 2)):
         """Convert glyph to a string of quadrant block characters."""
-        return self._pixels.as_blocks()
+        return self._pixels.as_blocks(resolution)
 
     def as_vector(self, ink=1, paper=0):
         """Return flat tuple of user-specified foreground and background objects."""
         return self._pixels.as_vector(ink=ink, paper=paper)
 
     def as_bits(self, ink=1, paper=0):
         """Return flat bits as bytes string."""
@@ -561,50 +562,64 @@
 
     ##########################################################################
     # glyph transformations
 
     # orthogonal transformations
 
     @scriptable
-    def mirror(self, *, adjust_metrics:bool=True):
+    def mirror(
+            self, *,
+            adjust_metrics:bool=True, create_vertical_metrics:bool=False,
+        ):
         """
         Reverse pixels horizontally.
 
         adjust_metrics: also reverse metrics (default: True)
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         pixels = self._pixels.mirror()
+        new_metrics = {}
         if adjust_metrics:
-            return self.modify(
-                pixels,
+            new_metrics |= dict(
                 left_bearing=self.right_bearing,
                 right_bearing=self.left_bearing,
-                shift_left=-self.shift_left
-                #shift_left around central axis, so should differ at most 1 pixel
             )
-        return self.modify(pixels)
+            if create_vertical_metrics or self.has_vertical_metrics():
+                new_metrics |= dict(
+                    shift_left=-self.shift_left
+                    #shift_left around central axis, so should differ at most 1 pixel
+                )
+        return self.modify(pixels, **new_metrics)
 
     @scriptable
-    def flip(self, *, adjust_metrics:bool=True):
+    def flip(
+            self, *,
+            adjust_metrics:bool=True, create_vertical_metrics:bool=False,
+        ):
         """
         Reverse pixels vertically.
 
         adjust_metrics: also reverse metrics (default: True)
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         pixels = self._pixels.flip()
+        new_metrics = {}
         if adjust_metrics:
             # pylint: disable=invalid-unary-operand-type
-            return self.modify(
-                pixels,
-                top_bearing=self.bottom_bearing,
-                bottom_bearing=self.top_bearing,
+            new_metrics |= dict(
                 # flip about baseline
                 shift_up=-self.height - self.shift_up
             )
+            if create_vertical_metrics or self.has_vertical_metrics():
+                new_metrics |= dict(
+                    top_bearing=self.bottom_bearing,
+                    bottom_bearing=self.top_bearing,
+                )
         # Font should adjust ascent <-> descent and global bearings
-        return self.modify(pixels)
+        return self.modify(pixels, **new_metrics)
 
     @scriptable
     def transpose(self, *, adjust_metrics:bool=True):
         """
         Transpose glyph.
 
         adjust_metrics: also transpose metrics (default: True)
@@ -626,95 +641,93 @@
     turn = scriptable(turn_method)
 
     # raster resizing
 
     @scriptable
     def crop(
             self, left:int=0, bottom:int=0, right:int=0, top:int=0,
-            *, adjust_metrics:bool=True, create_vertical_metrics:bool=False
+            *, adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Crop the raster.
 
         left: number of columns to remove from left
         bottom: number of rows to remove from bottom
         right: number of columns to remove from right
         top: number of rows to remove from top
         adjust_metrics: make the operation render-invariant (default: True)
         create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         if not any((left, bottom, right, top)):
             return self
-        create_vertical_metrics = (
-            create_vertical_metrics or self.has_vertical_metrics()
-        )
         # reduce raster
         pixels = self._pixels.crop(left, bottom, right, top)
-        if not adjust_metrics:
-            return self.modify(pixels)
-        else:
-            # shift-left adjustment rounds differently for odd-width than even width
-            sign = 1 if (self.width%2) else -1
-            if not create_vertical_metrics:
-                return self.modify(
-                    pixels,
-                    left_bearing=self.left_bearing + left,
-                    right_bearing=self.right_bearing + right,
-                    shift_up=self.shift_up + bottom,
-                )
-            else:
-                return self.modify(
-                    pixels,
-                    # horizontal metrics
-                    left_bearing=self.left_bearing + left,
-                    right_bearing=self.right_bearing + right,
-                    shift_up=self.shift_up + bottom,
-                    # vertical metrics
+        new_metrics = {}
+        if adjust_metrics:
+            # horizontal metrics
+            new_metrics |= dict(
+                left_bearing=self.left_bearing + left,
+                right_bearing=self.right_bearing + right,
+                shift_up=self.shift_up + bottom,
+            )
+            # vertical metrics
+            if create_vertical_metrics or self.has_vertical_metrics():
+                # shift-left adjustment rounds differently for odd-width than even width
+                sign = 1 if (self.width%2) else -1
+                new_metrics |= dict(
                     top_bearing=self.top_bearing + top,
                     bottom_bearing=self.bottom_bearing + bottom,
                     shift_left=self.shift_left + sign*((sign*(right-left))//2),
                 )
+        return self.modify(pixels, **new_metrics)
 
     @scriptable
     def expand(
             self, left:int=0, bottom:int=0, right:int=0, top:int=0,
-            *, adjust_metrics:bool=True
+            *, adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Add blank space to raster.
 
         left: number of columns to add on left
         bottom: number of rows to add on bottom
         right: number of columns to add on right
         top: number of rows to add on top
         adjust_metrics: make the operation render-invariant (default: True)
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         if not any((left, bottom, right, top)):
             return self
         # reduce raster
         pixels = self._pixels.expand(left, bottom, right, top)
+        new_metrics = {}
         if adjust_metrics:
-            # shift-left adjustment rounds differently for odd-width than even width
-            sign = 1 if (self.width%2) else -1
-            return self.modify(
-                pixels,
-                # horizontal metrics
+            # horizontal metrics
+            new_metrics |= dict(
                 left_bearing=self.left_bearing - left,
                 right_bearing=self.right_bearing - right,
                 shift_up=self.shift_up - bottom,
-                # vertical metrics
-                top_bearing=self.top_bearing - top,
-                bottom_bearing=self.bottom_bearing - bottom,
-                # for shift-left, expand left is like crop right, and v.v.
-                shift_left=self.shift_left + sign*((sign*(left-right))//2),
             )
-        return self.modify(pixels)
+            # vertical metrics
+            if create_vertical_metrics or self.has_vertical_metrics():
+                # shift-left adjustment rounds differently for odd-width than even width
+                sign = 1 if (self.width%2) else -1
+                new_metrics |= dict(
+                    top_bearing=self.top_bearing - top,
+                    bottom_bearing=self.bottom_bearing - bottom,
+                    # for shift-left, expand left is like crop right, and v.v.
+                    shift_left=self.shift_left + sign*((sign*(left-right))//2),
+                )
+        return self.modify(pixels, **new_metrics)
 
     @scriptable
-    def reduce(self, *, adjust_metrics:bool=True, create_vertical_metrics:bool=False):
+    def reduce(
+            self, *,
+            adjust_metrics:bool=True, create_vertical_metrics:bool=False,
+        ):
         """
         Return a glyph reduced to the bounding box.
 
         adjust_metrics: make the operation render-invariant (default: True)
         create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         # pylint: disable=not-an-iterable
@@ -725,98 +738,118 @@
 
 
     # scaling
 
     @scriptable
     def stretch(
             self, factor_x:int=1, factor_y:int=1,
-            *, adjust_metrics:bool=True
+            *, adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Stretch glyph by repeating rows and/or columns.
 
         factor_x: number of times to repeat horizontally
         factor_y: number of times to repeat vertically
         adjust_metrics: also stretch metrics (default: True)
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         if factor_x == factor_y == 1:
             return self
         pixels = self._pixels.stretch(factor_x, factor_y)
+        new_metrics = {}
         if adjust_metrics:
-            return self.modify(
-                pixels,
+            new_metrics |= dict(
                 left_bearing=factor_x*self.left_bearing,
                 right_bearing=factor_x*self.right_bearing,
-                top_bearing=factor_y*self.top_bearing,
-                bottom_bearing=factor_y*self.bottom_bearing,
                 shift_up=factor_y*self.shift_up,
-                shift_left=factor_x*self.shift_left,
             )
-        return self.modify(pixels)
+            if create_vertical_metrics or self.has_vertical_metrics():
+                new_metrics |= dict(
+                    top_bearing=factor_y*self.top_bearing,
+                    bottom_bearing=factor_y*self.bottom_bearing,
+                    shift_left=factor_x*self.shift_left,
+                )
+        return self.modify(pixels, **new_metrics)
 
     @scriptable
     def shrink(
             self, factor_x:int=1, factor_y:int=1,
-            *, adjust_metrics:bool=True
+            *, adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Shrink by removing rows and/or columns.
 
         factor_x: factor to shrink horizontally
         factor_y: factor to shrink vertically
         adjust_metrics: also stretch metrics (default: True)
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         if factor_x == factor_y == 1:
             return self
         pixels = self._pixels.shrink(factor_x, factor_y)
+        new_metrics = {}
         if adjust_metrics:
-            return self.modify(
-                pixels,
+            new_metrics |= dict(
                 left_bearing=self.left_bearing // factor_x,
                 right_bearing=self.right_bearing // factor_x,
-                top_bearing=self.top_bearing // factor_y,
-                bottom_bearing=self.bottom_bearing // factor_y,
                 shift_up=self.shift_up // factor_y,
-                shift_left=self.shift_left // factor_x,
             )
-        return self.modify(pixels)
+            if create_vertical_metrics or self.has_vertical_metrics():
+                new_metrics |= dict(
+                    top_bearing=self.top_bearing // factor_y,
+                    bottom_bearing=self.bottom_bearing // factor_y,
+                    shift_left=self.shift_left // factor_x,
+                )
+        return self.modify(pixels, **new_metrics)
 
     # shear
 
     @scriptable
-    def shear(self, *, direction:str='right', pitch:Coord=(1, 1)):
+    def shear(
+            self, *, direction:str='right', pitch:Coord=(1, 1),
+            create_vertical_metrics:bool=False,
+        ):
         """
         Create a slant by dislocating diagonally, keeping
         the horizontal baseline fixed.
 
         direction: direction to move the top of the glyph (default: 'right').
         pitch: angle of the slant, given as (x, y) coordinate (default: 1,1).
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         if not self.height:
             return self
         pitch_x, pitch_y = pitch
         direction = direction[0].lower()
         extra_width = (self.height-1) * pitch_x // pitch_y
         # adjustment to start diagonal at baseline
         modulo = pitch_y - (-self.shift_up*pitch_x) % pitch_y
         # adjust for shift at baseline height, to keep it fixed
         pre = (-self.shift_up * pitch_x + modulo) // pitch_y - (modulo==pitch_y)
         if direction == 'r':
-            work = self.modify(
+            new_metrics = dict(
                 left_bearing=self.left_bearing-pre,
                 right_bearing=self.right_bearing+pre,
-                shift_left=self.shift_left+pre,
             )
+            if create_vertical_metrics or self.has_vertical_metrics():
+                new_metrics |= dict(
+                    shift_left=self.shift_left+pre,
+                )
+            work = self.modify(**new_metrics)
             work = work.expand(right=extra_width)
         elif direction == 'l':
-            work = self.modify(
+            new_metrics = dict(
                 left_bearing=self.left_bearing+pre,
                 right_bearing=self.right_bearing-pre,
-                shift_left=self.shift_left-pre,
             )
+            if create_vertical_metrics or self.has_vertical_metrics():
+                new_metrics |= dict(
+                    shift_left=self.shift_left-pre,
+                )
+            work = self.modify(**new_metrics)
             work = work.expand(left=extra_width)
         else:
             raise ValueError(
                 f'Shear direction must be `left` or `right`, not `{direction}`'
             )
         pixels = work._pixels.shear(
             direction=direction, pitch=pitch, modulo=modulo,
@@ -824,45 +857,49 @@
         return work.modify(pixels)
 
     # ink effects
 
     @scriptable
     def smear(
             self, *, left:int=0, down:int=0, right:int=1, up:int=0,
-            adjust_metrics:bool=True
+            adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Repeat inked pixels.
 
         left: number of times to repeat inked pixel leftwards
         right: number of times to repeat inked pixel rightwards
         up: number of times to repeat inked pixel upwards
         down: number of times to repeat inked pixel downwards
         adjust_metrics: ensure advances stay the same (default: True)
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         # pylint: disable=unpacking-non-sequence
         pleft, pdown, pright, pup = self.padding
         work = self.expand(
             max(0, left-pleft), max(0, down-pdown),
             max(0, right-pright), max(0, up-pup),
-            adjust_metrics=adjust_metrics
+            adjust_metrics=adjust_metrics,
+            create_vertical_metrics=create_vertical_metrics,
         )
         return work.modify(work._pixels.smear(
             left=left, right=right, up=up, down=down,
         ))
 
     @scriptable
-    def outline(self, *, thickness:int=1):
+    def outline(self, *, thickness:int=1, create_vertical_metrics:bool=False):
         """
         Outline glyph.
 
         thickness: number of pixels in outline in each direction
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         thicker = self.smear(
-            left=thickness, down=thickness, right=thickness, up=thickness
+            left=thickness, down=thickness, right=thickness, up=thickness,
+            create_vertical_metrics=create_vertical_metrics,
         )
         return thicker.overlay(self, operator=lambda x: bool(sum(x) % 2))
 
     @scriptable
     def underline(self, descent:int=1, thickness:int=1):
         """
         Add a line.
```

### Comparing `monobit-0.41.0/monobit/glyphmap.py` & `monobit-0.42.0/monobit/glyphmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 try:
     from PIL import Image
 except ImportError:
     Image = None
 
 from .properties import Props
-from .raster import Raster, blockstr
+from .raster import Raster
+from .blocks import  blockstr
 
 
 class GlyphMap:
 
     def __init__(self, map=()):
         self._map = list(map)
         self._turns = 0
@@ -124,18 +125,18 @@
         ):
         """Convert glyph map to text."""
         canvas = self.to_canvas(sheet=sheet)
         return canvas.as_text(
             ink=ink, paper=paper, border=border, start=start, end=end
         )
 
-    def as_blocks(self, *, ink='@', paper='.', start='', end='\n', sheet=0):
+    def as_blocks(self, resolution=(2, 2)):
         """Convert glyph map to a string of quadrant block characters."""
-        canvas = self.to_canvas(sheet=sheet)
-        return canvas.as_blocks(ink=ink, paper=paper, start=start, end=end)
+        canvas = self.to_canvas(sheet=0)
+        return canvas.as_blocks(resolution)
 
 
 class Canvas(Raster):
     """Mutable raster for glyph maps."""
 
     _inner = list
     _outer = list
```

### Comparing `monobit-0.41.0/monobit/labels.py` & `monobit-0.42.0/monobit/labels.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 (c) 2020--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 from string import ascii_letters, digits
 from unicodedata import normalize
+from itertools import count
 
 from .binary import ceildiv, int_to_bytes, bytes_to_int
 from .scripting import to_int
 from .basetypes import CONVERTERS
 
 
 def is_enclosed(from_str, char):
@@ -189,14 +190,19 @@
 
     def __int__(self):
         """Get integer value."""
         if not self:
             raise ValueError('Empty codepoint cannot be converted to int.')
         return bytes_to_int(self)
 
+    def __add__(self, value):
+        """Add integer value."""
+        return Codepoint(int(self) + value)
+
+
 
 ##############################################################################
 # tags
 
 class Tag(Label):
     """Tag label."""
 
@@ -263,16 +269,18 @@
 def to_range(set_str, converter=to_int, inclusive_range=lambda _l, _u: range(_l, _u+1)):
     """Convert from iterable or string representation to generator."""
     if not isinstance(set_str, str):
         return (converter(_item) for _item in set_str)
     elements = set_str.split(',')
     elements = (_e.partition('-') for _e in elements)
     elements = (
-        inclusive_range(converter(_e[0]), converter(_e[2]))
-        if all(_e) else (converter(_e[0]),)
+        inclusive_range(converter(_e[0]), converter(_e[2])) if _e[2]
+        # deal with '1-' . This will only work for numbers
+        else count(converter(_e[0]),) if _e[1]
+        else (converter(_e[0]),)
         for _e in elements
     )
     elements = (_i for _e in elements for _i in _e)
     return (converter(_i) for _i in elements)
 
 def label_range(lower, upper):
     """Range of labels, inclusive of bounds."""
```

### Comparing `monobit-0.41.0/monobit/magic.py` & `monobit-0.42.0/monobit/magic.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/pack.py` & `monobit-0.42.0/monobit/pack.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,10 +60,15 @@
             )
         )
 
     def list_by(self, property):
         """List property of fonts in collection."""
         return tuple(getattr(_font, property) for _font in self._fonts)
 
+    def itergroups(self, property):
+        """Iterate over subpacks with one value for a property."""
+        for value in sorted(set(self.list_by(property))):
+            yield value, self.select(**{property: value})
+
 
 # scriptable font/glyph operations
 operations = get_scriptables(Pack)
```

### Comparing `monobit-0.41.0/monobit/properties.py` & `monobit-0.42.0/monobit/properties.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/raster.py` & `monobit-0.42.0/monobit/raster.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import zip_longest
 
-from .binary import ceildiv, reverse_by_group
+from .binary import ceildiv, reverse_by_group, bytes_to_bits
 from .basetypes import Bounds, Coord
+from .blocks import matrix_to_blocks, blockstr
+
 
 # sentinel object
 NOT_SET = object()
 
 
 # turn function for Raster, Glyph and Font
 
@@ -43,20 +45,14 @@
     elif turns == 1:
         return self.transpose().mirror()
     return self
 
 turn_method = turn
 
 
-class blockstr(str):
-    """str that is shown as block text in interactive session."""
-    def __repr__(self):
-        return f'"""\\\n{self}"""'
-
-
 # immutable bit matrix
 
 class Raster:
     """Bit matrix."""
 
     _0 = '0'
     _1 = '1'
@@ -192,52 +188,20 @@
             swap = paper
         contents = (
             contents.replace(self._0, swap).replace(self._1, ink)
             .replace(swap, paper).replace(delim, end+start)
         )
         return blockstr(''.join((start, contents, end)))
 
-    def as_blocks(self, *, ink='@', paper='.', start='', end='\n'):
-        """Convert glyph to a string of quadrant block characters."""
+    def as_blocks(self, resolution=(2, 2)):
+        """Convert glyph to a string of block characters."""
         if not self.height:
             return ''
         matrix = self.as_matrix()
-        quartets = tuple(
-            tuple(
-                _quartet
-                for _quartet in zip_longest(
-                    _row[::2], _row[1::2], _next[::2], _next[1::2],
-                    fillvalue=0
-                )
-            )
-            for _row, _next in zip_longest(matrix[::2], matrix[1::2], fillvalue=())
-        )
-        blockdict = {
-            (0, 0, 0, 0): ' ',
-            (0, 0, 0, 1): '\u2597',
-            (0, 0, 1, 0): '\u2596',
-            (0, 0, 1, 1): '\u2584',
-            (0, 1, 0, 0): '\u259d',
-            (0, 1, 0, 1): '\u2590',
-            (0, 1, 1, 0): '\u259e',
-            (0, 1, 1, 1): '\u259f',
-            (1, 0, 0, 0): '\u2598',
-            (1, 0, 0, 1): '\u259a',
-            (1, 0, 1, 0): '\u258c',
-            (1, 0, 1, 1): '\u2599',
-            (1, 1, 0, 0): '\u2580',
-            (1, 1, 0, 1): '\u259c',
-            (1, 1, 1, 0): '\u259b',
-            (1, 1, 1, 1): '\u2588',
-        }
-        quartets = '\n'.join(
-            ''.join(blockdict[_quartet] for _quartet in _row)
-            for _row in quartets
-        )
-        return blockstr(quartets + '\n')
+        return matrix_to_blocks(matrix, *resolution)
 
     @classmethod
     def from_vector(
             cls, bitseq, *,
             stride, width=NOT_SET, height=NOT_SET, align='left',
             _0=NOT_SET, _1=NOT_SET
         ):
@@ -247,28 +211,22 @@
         if width is NOT_SET:
             width = stride
         if align.startswith('r'):
             offset = stride - width
         else:
             offset = 0
         excess = len(bitseq) % stride
-        if excess:
-            if _1 in bitseq[-excess:]:
-                raise ValueError(
-                    'Bit string overruns by nonzero %d-bit sequence [%s].'
-                    % (excess, bitseq[-excess:])
-                )
-            bitseq = bitseq[:-excess]
-        if height is NOT_SET:
-            # used as slice bound, None means all
-            height = None
         rows = tuple(
             bitseq[_offs:_offs+width]
-            for _offs in range(offset, len(bitseq), stride)
-        )[:height]
+            for _offs in range(offset, len(bitseq) - excess, stride)
+        )
+        if height is not NOT_SET:
+            if len(rows) < height:
+                raise ValueError('Bit string too short')
+            rows = rows[:height]
         return cls(rows, _0=_0, _1=_1)
 
     def as_vector(self, ink=1, paper=0):
         """Return flat tuple of user-specified foreground and background objects."""
         return tuple(
             ink if _c == self._1 else paper
             for _c in ''.join(self._pixels)
```

### Comparing `monobit-0.41.0/monobit/renderer.py` & `monobit-0.42.0/monobit/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def grapheme_clusters(text):
         """Use NFC as poor-man's grapheme cluster. This works... sometimes."""
         for c in normalize('NFC', text):
             yield c
 
 from .binary import ceildiv
 from .labels import Char, Codepoint
-from .raster import Raster, blockstr
+from .raster import Raster
 from .properties import Props
 from .glyph import Glyph
 from .glyphmap import GlyphMap
 
 
 DIRECTIONS = {
     'n': 'normal',
```

### Comparing `monobit-0.41.0/monobit/scripting.py` & `monobit-0.42.0/monobit/scripting.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/storage.py` & `monobit-0.42.0/monobit/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,16 @@
     """
     pack = Pack(pack_or_font)
     outfile = outfile or sys.stdout
     if outfile == sys.stdout:
         # errors can occur if the strings we write contain surrogates
         # these may come from filesystem names using 'surrogateescape'
         sys.stdout.reconfigure(errors='replace')
+    if not pack:
+        raise ValueError('No fonts to save')
     with open_location(outfile, 'w') as (stream, subpath):
         save_stream(
             pack, stream,
             format=format, subpath=subpath, overwrite=overwrite,
             **kwargs
         )
     return pack_or_font
```

### Comparing `monobit-0.41.0/monobit/streams.py` & `monobit-0.42.0/monobit/streams.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/struct.py` & `monobit-0.42.0/monobit/struct.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/taggers.py` & `monobit-0.42.0/monobit/taggers.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/vector.py` & `monobit-0.42.0/monobit/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 from collections import deque
 from functools import cached_property
 from itertools import accumulate
 from typing import NamedTuple
 
 from .basetypes import Coord, Bounds
-from .raster import Raster, blockstr
+from .raster import Raster
 
 
 class StrokeMove(NamedTuple):
     """Stroke path element."""
     command: str
     dx: int
     dy: int
```

### Comparing `monobit-0.41.0/monobit/charmaps/adobe/ReadMe.txt` & `monobit-0.42.0/monobit/charmaps/adobe/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/adobe/stdenc.txt` & `monobit-0.42.0/monobit/charmaps/adobe/stdenc.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/adobe/symbol.txt` & `monobit-0.42.0/monobit/charmaps/adobe/symbol.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/adobe/zdingbat.txt` & `monobit-0.42.0/monobit/charmaps/adobe/zdingbat.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/agl/LICENSE.md` & `monobit-0.42.0/monobit/charmaps/agl/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/agl/README.md` & `monobit-0.42.0/monobit/charmaps/agl/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/agl/aglfn.txt` & `monobit-0.42.0/monobit/charmaps/agl/aglfn.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/agl/glyphlist.txt` & `monobit-0.42.0/monobit/charmaps/agl/glyphlist.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/ARABIC.TXT` & `monobit-0.42.0/monobit/charmaps/apple/ARABIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/CELTIC.TXT` & `monobit-0.42.0/monobit/charmaps/apple/CELTIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/CENTEURO.TXT` & `monobit-0.42.0/monobit/charmaps/apple/CENTEURO.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/CHINSIMP.TXT` & `monobit-0.42.0/monobit/charmaps/apple/CHINSIMP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/CHINTRAD.TXT` & `monobit-0.42.0/monobit/charmaps/apple/CHINTRAD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/CORPCHAR.TXT` & `monobit-0.42.0/monobit/charmaps/apple/CORPCHAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/CROATIAN.TXT` & `monobit-0.42.0/monobit/charmaps/apple/CROATIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/CYRILLIC.TXT` & `monobit-0.42.0/monobit/charmaps/apple/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/DEVANAGA.TXT` & `monobit-0.42.0/monobit/charmaps/apple/DEVANAGA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/DINGBATS.TXT` & `monobit-0.42.0/monobit/charmaps/apple/DINGBATS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/FARSI.TXT` & `monobit-0.42.0/monobit/charmaps/apple/FARSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/GAELIC.TXT` & `monobit-0.42.0/monobit/charmaps/apple/GAELIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/GREEK.TXT` & `monobit-0.42.0/monobit/charmaps/apple/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/GUJARATI.TXT` & `monobit-0.42.0/monobit/charmaps/apple/GUJARATI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/GURMUKHI.TXT` & `monobit-0.42.0/monobit/charmaps/apple/GURMUKHI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/HEBREW.TXT` & `monobit-0.42.0/monobit/charmaps/apple/HEBREW.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/ICELAND.TXT` & `monobit-0.42.0/monobit/charmaps/apple/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/INUIT.TXT` & `monobit-0.42.0/monobit/charmaps/apple/INUIT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/JAPANESE.TXT` & `monobit-0.42.0/monobit/charmaps/apple/JAPANESE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/KEYBOARD.TXT` & `monobit-0.42.0/monobit/charmaps/apple/KEYBOARD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/KOREAN.TXT` & `monobit-0.42.0/monobit/charmaps/apple/KOREAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/ROMAN.TXT` & `monobit-0.42.0/monobit/charmaps/apple/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/ROMANIAN.TXT` & `monobit-0.42.0/monobit/charmaps/apple/ROMANIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/ReadMe.txt` & `monobit-0.42.0/monobit/charmaps/apple/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/SYMBOL.TXT` & `monobit-0.42.0/monobit/charmaps/apple/SYMBOL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/THAI.TXT` & `monobit-0.42.0/monobit/charmaps/apple/THAI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/TURKISH.TXT` & `monobit-0.42.0/monobit/charmaps/apple/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/apple/UKRAINE.TXT` & `monobit-0.42.0/monobit/charmaps/apple/UKRAINE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/README.md` & `monobit-0.42.0/monobit/charmaps/czyborra/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/bulgarian-mik.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/bulgarian-mik.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/cp866.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/cp866.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/gost19768-87.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/gost19768-87.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/hp-roman8.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/hp-roman8.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/koi-0.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/koi-0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/koi-7.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/koi-7.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/koi8-a.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/koi8-a.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/koi8-b.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/koi8-b.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/koi8-e.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/koi8-e.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/koi8-f.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/koi8-f.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/koi8-r.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/koi8-r.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/czyborra/koi8-u.txt` & `monobit-0.42.0/monobit/charmaps/czyborra/koi8-u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-ca` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-ca`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-ca2` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-ca2`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-cn` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-cn`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-cu` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-cu`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-de` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-de`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-dk` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-dk`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-es` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-es`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-es2` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-es2`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-fr` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-fr`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-gb` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-gb`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-hu` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-hu`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-it` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-it`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-jp` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-jp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-jp-ocr-b` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-jp-ocr-b`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-kr` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-kr`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-us` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-us`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/iso646-yu` & `monobit-0.42.0/monobit/charmaps/dkuug/iso646-yu`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/jis_x0201` & `monobit-0.42.0/monobit/charmaps/dkuug/jis_x0201`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/dkuug/x0201-7` & `monobit-0.42.0/monobit/charmaps/dkuug/x0201-7`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/emacs/MULE-ethiopic.map` & `monobit-0.42.0/monobit/charmaps/emacs/MULE-ethiopic.map`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/emacs/MULE-ipa.map` & `monobit-0.42.0/monobit/charmaps/emacs/MULE-ipa.map`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/emacs/MULE-is13194.map` & `monobit-0.42.0/monobit/charmaps/emacs/MULE-is13194.map`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/emacs/MULE-lviscii.map` & `monobit-0.42.0/monobit/charmaps/emacs/MULE-lviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/emacs/MULE-sisheng.map` & `monobit-0.42.0/monobit/charmaps/emacs/MULE-sisheng.map`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/emacs/MULE-tibetan.map` & `monobit-0.42.0/monobit/charmaps/emacs/MULE-tibetan.map`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/emacs/MULE-uviscii.map` & `monobit-0.42.0/monobit/charmaps/emacs/MULE-uviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/emacs/README.md` & `monobit-0.42.0/monobit/charmaps/emacs/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/evertype/ARMENIAN.TXT` & `monobit-0.42.0/monobit/charmaps/evertype/ARMENIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/evertype/GEORGIAN.TXT` & `monobit-0.42.0/monobit/charmaps/evertype/GEORGIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/evertype/README.md` & `monobit-0.42.0/monobit/charmaps/evertype/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/1116.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/1116.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/1117.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/1117.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/1118.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/1118.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/1119.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/1119.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/1125.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/1125.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/113.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/113.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/1131.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/1131.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30000.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30000.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30001.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30001.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30002.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30002.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30003.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30003.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30004.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30004.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30005.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30005.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30006.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30006.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30007.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30007.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30008.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30008.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30009.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30009.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30010.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30010.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30011.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30011.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30012.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30013.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30013.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30014.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30014.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30015.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30015.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30016.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30016.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30017.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30017.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30018.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30018.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30019.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30019.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30020.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30020.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30021.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30022.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30022.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30023.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30023.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30024.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30024.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30025.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30025.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30026.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30026.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30027.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30027.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30028.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30028.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30029.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30029.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30030.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30030.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30031.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30031.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30032.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30032.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30033.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30033.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30034.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30034.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30039.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30039.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/30040.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/30040.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/3012.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/3012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/3021.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/3021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/3845.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/3845.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/3846.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/3846.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/3848.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/3848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/437.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/437.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/57781.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/57781.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/58152.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/58152.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/58210.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/58210.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/58335.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/58335.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/59234.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/59234.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/59829.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/59829.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/60258.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/60258.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/60853.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/60853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/61282.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/61282.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/62306.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/62306.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/667.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/667.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/668.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/668.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/737.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/737.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/770.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/770.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/771.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/771.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/772.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/772.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/773.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/773.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/774.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/774.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/775.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/775.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/777.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/777.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/778.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/778.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/790.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/790.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/808.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/808.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/848.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/849.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/849.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/850.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/850.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/851.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/851.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/852.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/852.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/853.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/855.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/855.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/856.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/856.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/857.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/857.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/858.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/858.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/859.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/859.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/860.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/860.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/861.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/861.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/862.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/862.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/863.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/863.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/864.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/864.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/865.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/865.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/866.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/866.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/867.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/867.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/869.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/869.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/872.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/872.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/895.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/895.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/899.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/899.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/991.ucp` & `monobit-0.42.0/monobit/charmaps/freedos/991.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/freedos/README.md` & `monobit-0.42.0/monobit/charmaps/freedos/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iana/Amiga-1251` & `monobit-0.42.0/monobit/charmaps/iana/Amiga-1251`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iana/PTCP154` & `monobit-0.42.0/monobit/charmaps/iana/PTCP154`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100` & `monobit-0.42.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100` & `monobit-0.42.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101` & `monobit-0.42.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100` & `monobit-0.42.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/ibm-cdra/readme.txt` & `monobit-0.42.0/monobit/charmaps/ibm-cdra/readme.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/README.md` & `monobit-0.42.0/monobit/charmaps/icu/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm` & `monobit-0.42.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/cns-11643-1992.ucm` & `monobit-0.42.0/monobit/charmaps/icu/cns-11643-1992.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm` & `monobit-0.42.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm` & `monobit-0.42.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm` & `monobit-0.42.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm` & `monobit-0.42.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm` & `monobit-0.42.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm` & `monobit-0.42.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm` & `monobit-0.42.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm` & `monobit-0.42.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/windows-1361-2000.ucm` & `monobit-0.42.0/monobit/charmaps/icu/windows-1361-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/icu/windows-936-2000.ucm` & `monobit-0.42.0/monobit/charmaps/icu/windows-936-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-1.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-10.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-10.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-11.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-11.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-13.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-13.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-14.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-14.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-15.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-15.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-16.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-16.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-2.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-3.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-4.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-5.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-6.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-7.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-8.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/8859-9.TXT` & `monobit-0.42.0/monobit/charmaps/iso-8859/8859-9.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/iso-8859/ReadMe.txt` & `monobit-0.42.0/monobit/charmaps/iso-8859/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/AMSCPC.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/AMSCPC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/AMSCPM.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/AMSCPM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8II.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ATARI8II.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARISTI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ATARISTI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARISTV.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ATARISTV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/C64IALT.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/C64IALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/C64IPRI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/C64IPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/C64VALT.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/C64VALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/C64VPRI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/C64VPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/COCOICHG.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/COCOICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/CPETIALT.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/CPETIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/CPETVALT.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/CPETVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/CVICIALT.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/CVICIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/CVICVALT.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/CVICVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/MINITLG0.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/MINITLG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/MINITLG1.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/MINITLG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/MSX.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/MSX.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ORICG0.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ORICG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ORICG1.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ORICG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/RISCEFF.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/RISCEFF.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSB.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/RISCOSB.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/RISCOSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSV.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/RISCOSV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ReadMe.txt` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TI994A.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TI994A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ZX80.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ZX80.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ZX81.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ZX81.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT` & `monobit-0.42.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/dec-vt100.ucp` & `monobit-0.42.0/monobit/charmaps/manual/dec-vt100.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/hp48.txt` & `monobit-0.42.0/monobit/charmaps/manual/hp48.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/ibm897graph.ucp` & `monobit-0.42.0/monobit/charmaps/manual/ibm897graph.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/iso2047.txt` & `monobit-0.42.0/monobit/charmaps/manual/iso2047.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/mac-system.ucp` & `monobit-0.42.0/monobit/charmaps/manual/mac-system.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/ms-linedraw.txt` & `monobit-0.42.0/monobit/charmaps/manual/ms-linedraw.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/russup3.ucp` & `monobit-0.42.0/monobit/charmaps/manual/russup3.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/russup4ac.ucp` & `monobit-0.42.0/monobit/charmaps/manual/russup4ac.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/russup4na.ucp` & `monobit-0.42.0/monobit/charmaps/manual/russup4na.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/windows-1.0.txt` & `monobit-0.42.0/monobit/charmaps/manual/windows-1.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/windows-2.0.txt` & `monobit-0.42.0/monobit/charmaps/manual/windows-2.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/manual/windows-3.1.txt` & `monobit-0.42.0/monobit/charmaps/manual/windows-3.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/MAC/GREEK.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/MAC/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP437.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP437.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP737.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP737.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP775.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP775.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP850.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP850.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP852.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP852.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP855.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP855.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP857.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP857.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP860.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP860.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP861.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP861.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP862.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP862.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP863.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP863.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP864.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP864.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP865.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP865.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP866.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP866.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP869.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP869.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP874.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/PC/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT` & `monobit-0.42.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT` & `monobit-0.42.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/ATARIST.TXT` & `monobit-0.42.0/monobit/charmaps/misc/ATARIST.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/CP1006.TXT` & `monobit-0.42.0/monobit/charmaps/misc/CP1006.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/CP424.TXT` & `monobit-0.42.0/monobit/charmaps/misc/CP424.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/CP856.TXT` & `monobit-0.42.0/monobit/charmaps/misc/CP856.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/GSM0338.TXT` & `monobit-0.42.0/monobit/charmaps/misc/GSM0338.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/IBMGRAPH.TXT` & `monobit-0.42.0/monobit/charmaps/misc/IBMGRAPH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/JIS0208.TXT` & `monobit-0.42.0/monobit/charmaps/misc/JIS0208.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/KOI8-R.TXT` & `monobit-0.42.0/monobit/charmaps/misc/KOI8-R.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/KOI8-U.TXT` & `monobit-0.42.0/monobit/charmaps/misc/KOI8-U.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/KPS9566.TXT` & `monobit-0.42.0/monobit/charmaps/misc/KPS9566.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/KZ1048.TXT` & `monobit-0.42.0/monobit/charmaps/misc/KZ1048.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/NEXTSTEP.TXT` & `monobit-0.42.0/monobit/charmaps/misc/NEXTSTEP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/SGML.TXT` & `monobit-0.42.0/monobit/charmaps/misc/SGML.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT` & `monobit-0.42.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/dashen-map.txt` & `monobit-0.42.0/monobit/charmaps/misc/dashen-map.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/misc/ibm-ugl.txt` & `monobit-0.42.0/monobit/charmaps/misc/ibm-ugl.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/ALTVAR.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/ALTVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-7.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/ARMSCII-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-8.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/ARMSCII-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/DECMCS.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/DECMCS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/GEO-ITA.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/GEO-ITA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/GEO-PS.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/GEO-PS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/KOI8RU.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/KOI8RU.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/OSNOVAR.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/OSNOVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/README.md` & `monobit-0.42.0/monobit/charmaps/mleisher/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/mleisher/TIS620.TXT` & `monobit-0.42.0/monobit/charmaps/mleisher/TIS620.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/moztw/big5_2003-b2u.txt` & `monobit-0.42.0/monobit/charmaps/moztw/big5_2003-b2u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/moztw/eten.txt` & `monobit-0.42.0/monobit/charmaps/moztw/eten.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/python/TCVN5712-1.TXT` & `monobit-0.42.0/monobit/charmaps/python/TCVN5712-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/python/TCVN5712-2.TXT` & `monobit-0.42.0/monobit/charmaps/python/TCVN5712-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/python/TCVN5712-3.TXT` & `monobit-0.42.0/monobit/charmaps/python/TCVN5712-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/vietstd/unicode.html` & `monobit-0.42.0/monobit/charmaps/vietstd/unicode.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/vietstd/viscii1.1.txt` & `monobit-0.42.0/monobit/charmaps/vietstd/viscii1.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/abicomp.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/abicomp.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/brascii.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/brascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/cp853.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/cp853.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/cwi2.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/cwi2.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/dec-special.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/dec-special.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/dec-technical.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/dec-technical.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/gem.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/gem.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/kamenicky.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/kamenicky.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/lics.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/lics.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/mattel-aquarius.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/mattel-aquarius.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/mazovia.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/mazovia.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/pascii.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/pascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/ventura.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/ventura.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/windows-1252.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/windows-1252.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/wingdings.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/wingdings.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/wikipedia/wiscii.html` & `monobit-0.42.0/monobit/charmaps/wikipedia/wiscii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-1.enc` & `monobit-0.42.0/monobit/charmaps/xfonts/mulearabic-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-2.enc` & `monobit-0.42.0/monobit/charmaps/xfonts/mulearabic-2.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/xfonts/mulelao-1.enc` & `monobit-0.42.0/monobit/charmaps/xfonts/mulelao-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/xfonts/suneu-greek.enc` & `monobit-0.42.0/monobit/charmaps/xfonts/suneu-greek.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/charmaps/xfonts/viscii1.1-1.enc` & `monobit-0.42.0/monobit/charmaps/xfonts/viscii1.1-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/containers/compressors.py` & `monobit-0.42.0/monobit/containers/compressors.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/containers/container.py` & `monobit-0.42.0/monobit/containers/container.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/containers/directory.py` & `monobit-0.42.0/monobit/containers/directory.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/containers/mac.py` & `monobit-0.42.0/monobit/containers/mac.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/containers/source.py` & `monobit-0.42.0/monobit/containers/source.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/containers/tar.py` & `monobit-0.42.0/monobit/containers/tar.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/containers/zip.py` & `monobit-0.42.0/monobit/containers/zip.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/amiga.py` & `monobit-0.42.0/monobit/formats/amiga.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/bbc.py` & `monobit-0.42.0/monobit/formats/bbc.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 
 from ..properties import Props
 from ..storage import loaders, savers
 from ..font import Font
 from ..glyph import Glyph
 from ..magic import FileFormatError
 
-# common utilities
-from .gdos import _subset_storable
-
 
 _BBC_VDU = b'\x17'
 
 # storable code points
 _BBC_RANGE = range(32, 256)
 
 
@@ -66,15 +63,15 @@
 def _write_bbc(outstream, font):
     """Write bbc glyphs to binary file."""
     if font.cell_size != (8, 8):
         raise FileFormatError(
             'BBC font file can only store an 8x8 character-cell font.'
         )
     font = font.label(codepoint_from=font.encoding)
-    font = _subset_storable(font, _BBC_RANGE)
+    font = font.subset(_BBC_RANGE)
     # expand into horizontal bearings, align vertically
     font = font.equalise_horizontal()
     glyph_bytes = tuple(
         b''.join((_BBC_VDU, bytes(_g.codepoint), _g.as_bytes()))
         for _g in font.glyphs
     )
     bitmap = b''.join(glyph_bytes)
```

### Comparing `monobit-0.41.0/monobit/formats/bmfont.py` & `monobit-0.42.0/monobit/formats/bmfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/borland.py` & `monobit-0.42.0/monobit/formats/borland.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/cpi.py` & `monobit-0.42.0/monobit/formats/cpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from ..storage import loaders, savers
 from ..magic import FileFormatError, Magic
 from ..font import Font
 from ..glyph import Glyph
 from ..properties import Props
 
 from .raw import load_bitmap
-from .gdos import _subset_storable
 
 
 _ID_MS = b'FONT   '
 _ID_NT = b'FONT.NT'
 _ID_DR = b'DRFONT '
 
 
@@ -416,15 +415,15 @@
         logging.warning(
             'CP fonts must have encoding set to a numbered codepage'
         )
         return None
     # ensure codepoint values are set, if possible
     font = font.label(codepoint_from=font.encoding)
     # take only the glyphs that will fit
-    font = _subset_storable(font, _RANGE)
+    font = font.subset(_RANGE)
     font = font.equalise_horizontal()
     font = _fill_contiguous(font, _RANGE, Glyph.blank(*font.cell_size))
     return font
 
 
 def _fill_contiguous(font, full_range, filler):
     """Get contiguous range, fill gaps with empties."""
```

### Comparing `monobit-0.41.0/monobit/formats/daisydot.py` & `monobit-0.42.0/monobit/formats/daisydot.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/dashen.py` & `monobit-0.42.0/monobit/formats/dashen.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/dec.py` & `monobit-0.42.0/monobit/formats/dec.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/dosstart.py` & `monobit-0.42.0/monobit/formats/dosstart.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/figlet.py` & `monobit-0.42.0/monobit/formats/figlet.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/fontx.py` & `monobit-0.42.0/monobit/formats/fontx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/fzx.py` & `monobit-0.42.0/monobit/formats/fzx.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,20 +237,14 @@
     """Convert monobit font to FZX properties and glyphs."""
     # ensure codepoint values are set if possible
     font = font.label(codepoint_from=font.encoding)
     # select glyphs that can be included
     # only codepoints 32--255 inclusive
     # on extraction 32--127 will be assumed to be ASCII
     includable = font.subset(codepoints=set(_FZX_RANGE))
-    dropped = font.exclude(codepoints=set(_FZX_RANGE))
-    if dropped.glyphs:
-        logging.warning(
-            'FZX format can only store codepoints 32--255. '
-            'Not all glyphs in this font can be included.'
-        )
     # get contiguous range, fill gaps with empties
     glyphs = tuple(
         includable.get_glyph(codepoint=_cp, missing='empty').modify(codepoint=_cp)
         for _cp in _FZX_RANGE
     )
     # remove empties at end
     while glyphs and glyphs[-1].is_blank() and not glyphs[-1].advance_width:
```

### Comparing `monobit-0.41.0/monobit/formats/gdos.py` & `monobit-0.42.0/monobit/formats/gdos.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 from ..storage import loaders, savers
 from ..font import Font
 from ..glyph import Glyph
 from ..magic import FileFormatError, Magic
 from ..binary import bytes_to_bits, ceildiv
 from ..raster import Raster
 
-# common utilities
-from .windows import _normalise_metrics
-
 
 @loaders.register(
     name='gdos',
     patterns=('*.fnt', '*.gft', '*.[cev]ga'),
     # maybe - this is the usual value for 'lighten' and 'skew'
     magic=(Magic.offset(62) + b'UUUU',),
 )
@@ -558,17 +555,21 @@
 ################################################################################
 # GDOS writer
 
 def _convert_to_gdos(font, endianness):
     """Convert monobit font to GDOS properties and glyphs."""
     # ensure codepoint values are set if possible
     font = font.label(codepoint_from=font.encoding)
-    font = _subset_storable(font, _GDOS_RANGE)
+    font = font.subset(_GDOS_RANGE)
     font = _make_contiguous(font)
-    font, add_shift_up = _normalise_metrics(font)
+    # bring to padded normal form with equalised upshifts
+    font = font.equalise_horizontal()
+    upshifts = set(_g.shift_up for _g in font.glyphs)
+    shift_up, *remainder = upshifts
+    assert not remainder
     # check glyph dimensions / bitfield ranges
     if any(_g.left_bearing < -127 or _g.right_bearing < -127 for _g in font.glyphs):
         raise FileFormatError(
             'GDOS format: negative bearings must not exceed 127.'
         )
     # keep namespace properties
     if 'gdos' in font.get_properties():
@@ -588,21 +589,23 @@
     )
     header = _FNT_HEADER[endian](
         font_id=add_props.get('font-id', 255),
         point=font.point_size,
         name=font.name.encode('ascii', 'replace')[:32],
         first_ade=int(min(font.get_codepoints())),
         last_ade=int(max(font.get_codepoints())),
-        top=font.raster_size.y+add_shift_up,
+        # common shift up must be negative as we brought to padded normal form
+        top=font.raster_size.y + shift_up,
         ascent=font.ascent-1,
         # Half line distance expressed as a positive offset from baseline.
         # interpreting as x-height
         half=font.x_height,
         descent=font.descent,
-        bottom=add_shift_up,
+        # common shift up must be negative as we brought to padded normal form
+        bottom=-shift_up,
         # Width of the widest character.
         # I'm interpreting this as the widest per-glyph bounding box
         max_char_width=max(_g.bounding_box.x for _g in font.glyphs),
         # Width of the widest character cell.
         # interpreting as widest advance width
         max_cell_width=font.max_width,
         left_offset=add_props.get('left-offset', 0),
@@ -612,24 +615,14 @@
         lighten=add_props.get('lighten_mask', 0x5555),
         skew=add_props.get('skew_mask', 0x5555),
         flags=flags,
         #hor_table, off_table, dat_table, form_width, form_height
     )
     return header, font.glyphs
 
-def _subset_storable(font, storable_range):
-    """Select glyphs that can be included."""
-    # only codepoints 0--255 inclusive
-    if any(int(_c) not in storable_range for _c in font.get_codepoints()):
-        logging.warning(
-            'Output format can only store codepoints 0--255. '
-            'Not all glyphs in this font can be included.'
-        )
-    font = font.subset(codepoints=set(storable_range))
-    return font
 
 def _make_contiguous(font):
     """Get contiguous range, fill gaps with empties."""
     glyphs = tuple(
         font.get_glyph(codepoint=_cp, missing='empty').modify(codepoint=_cp)
         for _cp in range(
             int(min(font.get_codepoints())),
```

### Comparing `monobit-0.41.0/monobit/formats/geos.py` & `monobit-0.42.0/monobit/formats/geos.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/hurt.py` & `monobit-0.42.0/monobit/formats/hurt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/image.py` & `monobit-0.42.0/monobit/formats/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         ):
         """
         Export font to grid-based image.
 
         image_format: image file format (default: png)
         columns: number of columns in glyph chart (default: 32)
         margin: number of pixels in X,Y direction around glyph chart (default: 0x0)
-        padding: number of pixels in X,Y direction between glyph (default: 0x0)
+        padding: number of pixels in X,Y direction between glyph (default: 1x1)
         scale: number of pixels in X,Y direction per glyph bit (default: 1x1)
         order: start with "r" for row-major order (default), "c" for column-major order
         direction: X, Y direction where +1, -1 (default) means left-to-right, top-to-bottom
         paper: background colour R,G,B 0--255 (default: 0,0,0)
         ink: foreground colour R,G,B 0--255 (default: 255,255,255)
         border: border colour R,G,B 0--255 (default 32,32,32)
         codepoint_range: first and last codepoint to include (includes bounds and undefined codepoints; default: all codepoints)
```

### Comparing `monobit-0.41.0/monobit/formats/mousegraphics.py` & `monobit-0.42.0/monobit/formats/mousegraphics.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/mzfon.py` & `monobit-0.42.0/monobit/formats/mzfon.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 
 from ..storage import loaders, savers
 from ..streams import Stream
 from ..magic import FileFormatError
 
 from .windows.mz import MZ_HEADER, create_mz_stub
-from .windows.ne import create_ne, read_ne, _NE_HEADER
+from .windows.ne import create_ne, read_ne, NE_HEADER
 from .windows.pe import read_pe
 from .windows.fnt import (
     convert_win_fnt_resource,
     FNT_MAGIC_1, FNT_MAGIC_2, FNT_MAGIC_3
 )
 from .os2.lx import read_lx
 from .os2.ne import read_os2_ne
@@ -33,15 +33,15 @@
     """
     Load fonts from a Windows or OS/2 .FON container.
 
     all_type_ids: try to extract font from any resource, regardless of type id
     """
     mz_header = MZ_HEADER.read_from(instream)
     if mz_header.e_magic == b'MZ':
-        header = _NE_HEADER.read_from(instream, mz_header.e_lfanew)
+        header = NE_HEADER.read_from(instream, mz_header.e_lfanew)
         instream.seek(mz_header.e_lfanew)
         format = header.ne_magic
     elif mz_header.e_magic == b'ZM':
         raise FileFormatError('Big-endian MZ executables not supported')
     else:
         # apparently LX files don't always have an MZ stub
         # we allow stubless NE and PE too, in case they exist
```

### Comparing `monobit-0.41.0/monobit/formats/nearlyraw.py` & `monobit-0.42.0/monobit/formats/nearlyraw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/palm.py` & `monobit-0.42.0/monobit/formats/palm.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from ..struct import big_endian as be
 from ..properties import Props
 from ..storage import loaders, savers
 from ..font import Font
 from ..magic import FileFormatError, Magic
 
-from .mac.nfnt import _extract_nfnt, _convert_nfnt
+from .mac.nfnt import extract_nfnt, convert_nfnt
 
 
 # offset magic: b'FontFont' at offset 0x3c (type, creator fields)
 @loaders.register(
     name='palm',
     magic=(Magic.offset(0x3c) + b'FontFont',),
     patterns=('*.pdb',),
@@ -161,15 +161,15 @@
     for entry in entries:
         instream.seek(entry.localChunkID)
         data = instream.read()
         # can be `NFNT` (0x9000) or `nfnt` (0x9200)
         # or `afnx` format (?)
         # currently we're just assuming NFNT
         try:
-            nfnt = _extract_nfnt(data, offset=0)
+            nfnt = extract_nfnt(data, offset=0)
         except ValueError as e:
             logging.warning('Could not read record: %s', e)
             continue
         nfnts.append(nfnt)
     return props | Props(entries=tuple(entries), records=nfnts)
 
 
@@ -189,26 +189,26 @@
             continue
         if entry.type == b'nfnt':
             logging.warning('Palm v2 (nfnt) format not implemented.')
         instream.seek(entry.localChunkID)
         data = instream.read()
         # currently we're just assuming NFNT
         try:
-            nfnt = _extract_nfnt(data, offset=0)
+            nfnt = extract_nfnt(data, offset=0)
         except ValueError as e:
             logging.warning('Could not read record: %s', e)
             continue
         nfnts.append(nfnt)
     return props | Props(entries=tuple(entries), records=nfnts)
 
 
 def _convert_palm(palm_data):
     """Convert a Palm OS font data structure to Font."""
     fonts = (
-        _convert_nfnt({}, **_nfnt)
+        convert_nfnt({}, **_nfnt)
         for _nfnt in palm_data.records
     )
     fonts = tuple(
         _font.modify(
             family=palm_data.header.name.decode('latin-1'),
             revision=palm_data.header.modificationNumber,
             source_format=f'[Palm] {_font.source_format}',
```

### Comparing `monobit-0.41.0/monobit/formats/pcl.py` & `monobit-0.42.0/monobit/formats/pcl.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/pcpaint.py` & `monobit-0.42.0/monobit/formats/pcpaint.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/pdf.py` & `monobit-0.42.0/monobit/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/pkfont.py` & `monobit-0.42.0/monobit/formats/pkfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/prebuilt.py` & `monobit-0.42.0/monobit/formats/prebuilt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/printshop.py` & `monobit-0.42.0/monobit/formats/printshop.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/psf.py` & `monobit-0.42.0/monobit/formats/psf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/raw.py` & `monobit-0.42.0/monobit/formats/raw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/signum.py` & `monobit-0.42.0/monobit/formats/signum.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/svg.py` & `monobit-0.42.0/monobit/formats/svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from ..storage import loaders, savers
 from ..magic import FileFormatError
 from ..vector import StrokePath
 from ..font import Font
 from ..glyph import Glyph
 from ..properties import Props, reverse_dict
-from .windows.fnt import _WEIGHT_MAP, _WEIGHT_REVERSE_MAP
+from .windows import WEIGHT_MAP, WEIGHT_REVERSE_MAP
 
 
 _STYLE_MAP = {
     'normal': 'roman',
     'italic': 'italic',
     'oblique': 'oblique'
 }
@@ -55,15 +55,15 @@
         props |= Props(
             ascent=int(font_face.attrib.get('ascent')),
             descent=-int(font_face.attrib.get('descent')),
             family=font_face.attrib.get('font-family'),
             line_height=int(font_face.attrib.get('font-size', font_face.attrib.get('units-per-em'))),
             underline_thickness=int(font_face.attrib.get('underline-thickness')),
             underline_descent=-int(font_face.attrib.get('underline-position')),
-            weight=_WEIGHT_MAP[round(weight, -2)],
+            weight=WEIGHT_MAP[round(weight, -2)],
             slant=_STYLE_MAP.get(font_face.attrib.get('font-style')),
         )
     glyph_elems = list(font.iterfind('{*}glyph'))
     missing_glyph = font.find('{*}missing-glyph')
     if missing_glyph is not None:
         glyph_elems.append(missing_glyph)
     # get the first element containing a path definition
@@ -189,15 +189,15 @@
         'font-size': font.line_height,
         'ascent': font.ascent,
         'descent': -font.descent,
         'cap-height': font.cap_height,
         'x-height': font.x_height,
         'underline-thickness': font.underline_thickness,
         'underline-position': -font.underline_descent,
-        'font-weight': _WEIGHT_REVERSE_MAP.get(font.weight, 400),
+        'font-weight': WEIGHT_REVERSE_MAP.get(font.weight, 400),
         'font-style': _STYLE_REVERSE_MAP.get(font.slant, 'normal'),
     }
     outfile.write(f'  <font-face{attr_str(font_face, indent=6)}/>\n')
     if font.default_char:
         _write_glyph(outfile, font, font.get_default_glyph(), tag='missing-glyph')
     for i, glyph in enumerate(font.glyphs):
         if font.default_char in glyph.tags and len(glyph.get_labels()) == 1:
```

### Comparing `monobit-0.41.0/monobit/formats/vfont.py` & `monobit-0.42.0/monobit/formats/vfont.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 from ..struct import bitfield, little_endian as le, big_endian as be
 from ..properties import Props
 from ..storage import loaders, savers
 from ..font import Font
 from ..glyph import Glyph
 from ..magic import FileFormatError
 
-# common utilities
-from .gdos import _subset_storable
-
 
 @loaders.register(
     name='vfont',
     magic=(b'\x01\x1e', b'\x1e\x01'),
     patterns=('*.vfont',),
 )
 def load_vfont(instream, first_codepoint:int=0):
@@ -167,15 +164,15 @@
 ###############################################################################
 # writer
 
 def _convert_to_vfont(font):
     """Convert monobit font to vfont properties and glyphs."""
     # ensure codepoint values are set if possible
     font = font.label(codepoint_from=font.encoding)
-    font = _subset_storable(font, _VFONT_RANGE)
+    font = font.subset(_VFONT_RANGE)
     font = _make_contiguous(font)
     # set glyph properties
     glyphs = tuple(
         _glyph.modify(
             vfont=dict(
                 left=-_glyph.left_bearing,
                 right=_glyph.width+_glyph.left_bearing,
```

### Comparing `monobit-0.41.0/monobit/formats/xerox.py` & `monobit-0.42.0/monobit/formats/xerox.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/mac/__init__.py` & `monobit-0.42.0/monobit/formats/mac/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,30 +5,39 @@
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
 from ...storage import loaders, savers
 
-from .dfont import _parse_mac_resource
-from .nfnt import _extract_nfnt, _convert_nfnt, _create_nfnt
+from .dfont import parse_resource_fork, save_dfont
+from .nfnt import extract_nfnt, convert_nfnt, create_nfnt
 from .lisa import _load_lisa
 from .iigs import _load_iigs, _save_iigs
 
 
 @loaders.register(
     name='mac',
     # the magic is optional - a 'maybe magic'
     magic=(b'\0\0\1\0\0',),
     patterns=('*.dfont', '*.suit', '*.rsrc',),
 )
 def load_mac_dfont(instream):
-    """Load font from a MacOS suitcase."""
+    """Load font from MacOS resource fork or data-fork resource."""
     data = instream.read()
-    return _parse_mac_resource(data)
+    return parse_resource_fork(data)
+
+
+@savers.register(linked=load_mac_dfont)
+def save_mac_dfont(fonts, outstream, resource_type:str='NFNT', family_id:int=None):
+    """Save font to MacOS resource fork or data-fork resource.
+
+    resource_type: type of resource to store font in. One of `sfnt`, `NFNT`.
+    """
+    save_dfont(fonts, outstream, resource_type)
 
 
 @loaders.register(
     name='nfnt',
     # \x90\0 is not a formal signature, but the most common set of FONT_TYPE flags
     # the \x80 sigs are LISA compressed NFNTs
     magic=(b'\x90\0', b'\xb0\0', b'\x90\x80', b'\xb0\x80'),
@@ -38,16 +47,16 @@
     """
     Load font from a bare FONT/NFNT resource.
 
     offset: starting offset in bytes of the NFNT record in the file (default 0)
     """
     instream.seek(offset)
     data = instream.read()
-    fontdata = _extract_nfnt(data, 0)
-    return _convert_nfnt({}, **fontdata)
+    fontdata = extract_nfnt(data, 0)
+    return convert_nfnt({}, **fontdata)
 
 
 @loaders.register(name='lisa')
 def load_lisa(instream):
     """Load a LISA font library."""
     return _load_lisa(instream)
 
@@ -71,14 +80,27 @@
     if len(fonts) > 1:
         logging.warning('IIgs font file can only store one font.')
     font = fonts[0]
     _save_iigs(outstream, font, version=version)
 
 
 @savers.register(linked=load_nfnt)
-def save_nfnt(fonts, outstream):
-    """Write font to a bare FONT/NFNT resource."""
+def save_nfnt(
+        fonts, outstream,
+        create_width_table:bool=True,
+        create_height_table:bool=False,
+    ):
+    """
+    Write font to a bare FONT/NFNT resource.
+
+    create_width_table: include a fractional glyph-width table in the resource (default: True)
+    create_height_table: include an image-height table in the resource (default: False)
+    """
     if len(fonts) > 1:
         logging.warning('NFNT resource can only store one font.')
     font = fonts[0]
-    data, _, _ = _create_nfnt(font, endian='big', ndescent_is_high=True)
+    data, _, _ = create_nfnt(
+        font, endian='big', ndescent_is_high=True,
+        create_width_table=create_width_table,
+        create_height_table=create_height_table,
+    )
     outstream.write(data)
```

### Comparing `monobit-0.41.0/monobit/formats/mac/iigs.py` & `monobit-0.42.0/monobit/formats/mac/iigs.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from ...struct import bitfield, little_endian as le
 from ... import struct
 from ...storage import loaders, savers
 from ...font import Font, Coord
 from ...glyph import Glyph, KernTable
 from ...magic import FileFormatError
 
-from .nfnt import _convert_nfnt, _extract_nfnt, _create_nfnt
-from .dfont import _FONT_NAMES, _NON_ROMAN_NAMES
+from .nfnt import convert_nfnt, extract_nfnt, create_nfnt
+from .dfont import NON_ROMAN_NAMES
 
 
 # IIgs font file is essentially a little-endian MacOS FONT resource,
 # without the resource, plus an extra header.
 # Documented in the Apple IIgs Toolbox Reference Volume II, chapter 16-41
 # https://archive.org/details/AppleIIGSToolboxReferenceVolume2/
 
@@ -74,32 +74,32 @@
     # extended header for IIgs
     if header.version >= 0x0105: #  and len(extra) >= 2:
         eh = _EXTENDED_HEADER.from_bytes(extra)
         logging.debug('extended header: %s', eh)
     else:
         eh = _EXTENDED_HEADER()
     # read IIgs-style NFNT resource
-    fontdata = _extract_nfnt(
+    fontdata = extract_nfnt(
         data, offset, endian='little',
         owt_loc_high=eh.owTLocHigh, font_type=b'\0\0'
     )
     return _convert_iigs(**fontdata, header=header, name=name)
 
 
 def _convert_iigs(glyphs, fontrec, header, name):
     """Convert IIgs font data to monobit font."""
-    font = _convert_nfnt({}, glyphs, fontrec)
+    font = convert_nfnt({}, glyphs, fontrec)
     # properties from IIgs header
     properties = {
         'family': name,
         'point_size': header.pointSize,
         'source_format': 'IIgs v{}.{}'.format(*divmod(header.version, 256)),
         'iigs.family_id': header.family,
     }
-    if name not in _NON_ROMAN_NAMES:
+    if name not in NON_ROMAN_NAMES:
         properties['encoding'] = 'mac-roman'
     # decode style field
     if header.style.bold:
         properties['weight'] = 'bold'
     if header.style.italic:
         properties['slant'] = 'italic'
     decoration = []
@@ -111,16 +111,17 @@
         decoration.append('shadow')
     properties['decoration'] = ' '.join(decoration);
     return font.modify(**properties).label()
 
 
 def _save_iigs(outstream, font, version=None):
     """Save an Apple IIgs font file."""
-    nfnt, owt_loc_high, fbr_extent = _create_nfnt(
-        font, endian='little', ndescent_is_high=False
+    nfnt, owt_loc_high, fbr_extent = create_nfnt(
+        font, endian='little', ndescent_is_high=False,
+        create_width_table=False, create_height_table=False,
     )
     # if offset > 32 bits, need to use iigs format v1.05
     if version is None:
         if owt_loc_high:
             version = 0x0105
         else:
             version = 0x0101
```

### Comparing `monobit-0.41.0/monobit/formats/mac/lisa.py` & `monobit-0.42.0/monobit/formats/mac/lisa.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import logging
 
 from ...struct import big_endian as be
 from ...binary import align
 from ...magic import FileFormatError
 
-from .nfnt import _extract_nfnt, _convert_nfnt
+from .nfnt import extract_nfnt, convert_nfnt
 
 
 # https://www.kreativekorp.com/swdownload/lisa/AppleLisaFontFormat.pdf
 
 _LISA_HEADER = be.Struct(
     # numer of words in header, less 4
     headerLength='uint16',
@@ -46,16 +46,16 @@
         instream.seek(4 + 2*(rcd.fontResourceStart + header.headerLength))
         resources.append(
             instream.read(2*(rcd.fontResourceEnd - rcd.fontResourceStart))
         )
     fonts = []
     for name, data in zip(names, resources):
         try:
-            fontdata = _extract_nfnt(data, 0)
-            font = _convert_nfnt({}, **fontdata)
+            fontdata = extract_nfnt(data, 0)
+            font = convert_nfnt({}, **fontdata)
             font = font.modify(
                 name=name.decode('mac-roman'),
                 source_format=f'[Lisa] {font.source_format}',
             )
             fonts.append(font)
         except (ValueError, FileFormatError):
             pass
```

### Comparing `monobit-0.41.0/monobit/formats/mac/nfnt.py` & `monobit-0.42.0/monobit/formats/mac/nfnt.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 from ...struct import bitfield, big_endian as be, little_endian as le
 from ...font import Font
 from ...glyph import Glyph, KernTable
 from ...magic import FileFormatError
 from ...labels import Char
 from ...encoding import charmaps
 from ...raster import Raster
+from ...properties import Props
 
-from .fond import _fixed_to_float
+from .fond import fixed_to_float
 
 
 ##############################################################################
 # NFNT/FONT resource
 
 # the Font Type Element
 # https://developer.apple.com/library/archive/documentation/mac/Text/Text-251.html#MARKER-9-442
@@ -133,18 +134,24 @@
 # distance from the glyph origin to the left edge of the bit image of the glyph, in pixels. If this
 # sum is negative, the glyph origin  is to the right of the glyph image's left edge, meaning the
 # glyph kerns to the left.  If the sum is positive, the origin is to the left of the image's left
 # edge. If the sum equals zero, the glyph origin corresponds with the left edge of the bit image.
 # Missing glyphs are represented by a word value of -1. The last word of this table is also -1,
 # representing the end.
 def wo_entry_struct(base):
-    return base.Struct(
-        offset='uint8',
-        width='uint8',
-    )
+    if base == be:
+        return base.Struct(
+            offset='uint8',
+            width='uint8',
+        )
+    else:
+        return base.Struct(
+            width='uint8',
+            offset='uint8',
+        )
 
 # glyph width table entry
 # > Glyph-width table. For every glyph in the font, this table contains a word
 # > that specifies the glyph's fixed-point glyph width at the given point size
 # > and font style, in pixels. The Font Manager gives precedence to the values
 # > in this table over those in the font family glyph-width table. There is an
 # > unsigned integer in the high-order byte and a fractional part in the
@@ -166,15 +173,15 @@
 def height_entry_struct(base):
     return base.Struct(
         offset='uint8',
         height='uint8',
     )
 
 
-def _extract_nfnt(data, offset, endian='big', owt_loc_high=0, font_type=None):
+def extract_nfnt(data, offset, endian='big', owt_loc_high=0, font_type=None):
     """Read a MacOS NFNT or FONT resource."""
     # create struct types; IIgs NFNTs are little-endian
     base = {'b': be, 'l': le}[endian[:1].lower()]
     NFNTHeader = nfnt_header_struct(base)
     LocEntry = loc_entry_struct(base)
     WOEntry = wo_entry_struct(base)
     WidthEntry = width_entry_struct(base)
@@ -213,23 +220,22 @@
     if fontrec.nDescent > 0:
         owt_loc_high = fontrec.nDescent
     wo_offset = (fontrec.owTLoc + (owt_loc_high << 16)) * 2
     # owtTLoc is offset "from itself" to table
     wo_table = WOEntry.array(n_chars).from_bytes(data, offset + 16 + wo_offset)
     # scalable width table
     width_offset = wo_offset + WOEntry.size * n_chars
+    height_offset = width_offset
     if fontrec.fontType.has_width_table:
         width_table = WidthEntry.array(n_chars).from_bytes(data, width_offset)
+        height_offset += WidthEntry.size * n_chars
     # image height table: this can be deduced from the bitmaps
     # https://developer.apple.com/library/archive/documentation/mac/Text/Text-250.html#MARKER-9-414
     # > The Font Manager creates this table.
     if fontrec.fontType.has_height_table:
-        height_offset = width_offset
-        if fontrec.fontType.has_width_table:
-            height_offset += WidthEntry.size * n_chars
         height_table = HeightEntry.array(n_chars).from_bytes(data, height_offset)
     # parse bitmap strike
     bitmap_strike = bytes_to_bits(strike)
     rows = [
         bitmap_strike[_offs:_offs+fontrec.rowWords*16]
         for _offs in range(0, len(bitmap_strike), fontrec.rowWords*16)
     ]
@@ -298,15 +304,15 @@
                     output.append(next(iter))
                 except StopIteration:
                     break
     # bitmap rows still need to be XORed afterwards
     return bytes((data[0], data[1] ^ 0x80)) + bytes(reversed(output))
 
 
-def _convert_nfnt(properties, glyphs, fontrec):
+def convert_nfnt(properties, glyphs, fontrec):
     """Convert mac glyph metrics to monobit glyph metrics."""
     # the 'width' in the width/offset table is the pen advance
     # while the 'offset' is the (positive) offset after applying the
     # (positive or negative) 'kernMax' global offset
     #
     # since
     #   (glyph) advance_width == left_bearing + width + right_bearing
@@ -332,20 +338,16 @@
         if _glyph.wo_width != 0xff and _glyph.wo_offset != 0xff else _glyph
         for _glyph in glyphs
     )
     # store glyph-name encoding table
     # do this before setting codepoint labels so we don't drop the tag on the 'missing' glyph
     encoding_table = properties.pop('encoding-table', None)
     if encoding_table:
-        tag_table = {
-            _entry[:1]: _entry[1:].decode('mac-roman')
-            for _entry in encoding_table
-        }
         glyphs = tuple(
-            _glyph.modify(tag=tag_table.get(_glyph.codepoint, ''))
+            _glyph.modify(tag=encoding_table.get(_glyph.codepoint, ''))
             for _glyph in glyphs
         )
     # codepoint labels
     labelled = [
         _glyph.modify(codepoint=(_codepoint,))
         for _codepoint, _glyph in enumerate(glyphs[:-1], start=fontrec.firstChar)
     ]
@@ -358,24 +360,27 @@
     )
     # drop mac glyph metrics
     # keep scalable_width
     glyphs = tuple(_glyph.drop('wo_offset', 'wo_width') for _glyph in glyphs)
     # store kerning table
     # last as this needs to refer to codepoint labels
     kerning_table = properties.pop('kerning-table', None)
+    twos_complement = properties.pop('twos-complement', True)
     if kerning_table:
         # > Kerning distance. The kerning distance, in pixels, for the two glyphs
         # > at a point size of 1. This is a 16-bit fixed point value, with the
         # > integer part in the high-order 4 bits, and the fractional part in
         # > the low-order 12 bits. The Font Manager measures the distance in pixels
         # > and then multiplies it by the requested point size
         kern_table = sorted(
             (
                 _entry.kernFirst, _entry.kernSecond,
-                _fixed_to_float(_entry.kernWidth) * properties['point_size']
+                properties['point_size'] * fixed_to_float(
+                    _entry.kernWidth, twos_complement=twos_complement
+                )
             )
             for _entry in kerning_table
         )
         glyphs = tuple(
             _glyph.modify(right_kerning=KernTable({
                 _right: f'{_width:.2f}'
                 for _left, _right, _width in kern_table
@@ -400,30 +405,51 @@
     return Font(glyphs, **properties)
 
 
 
 ###############################################################################
 # NFNT writer
 
+def create_nfnt(
+        font, endian, ndescent_is_high, create_width_table, create_height_table
+    ):
+    """Create NFNT/FONT resource."""
+    # subset to characters storable in NFNT
+    font = subset_for_nfnt(font)
+    nfnt_data = convert_to_nfnt(
+        font, endian, ndescent_is_high, create_width_table, create_height_table
+    )
+    data = nfnt_data_to_bytes(nfnt_data)
+    return data, nfnt_data.owt_loc_high, nfnt_data.fbr_extent
+
 
-def _subset(font):
+def subset_for_nfnt(font):
     """Subset to glyphs storable in NFNT and append default glyph."""
     font = font.label(codepoint_from=font.encoding)
-    if font.encoding in ('mac-roman', 'mac-symbol', 'raw', '', None):
+    resample = False
+    if font.encoding.startswith('mac') or font.encoding in ('raw', '', None):
+        # it's not clear to me if/how NFNT resources are used for MBCS
+        # currently we just use the single-byte sector
+        # this affects mac-japanese, mac-korean which have multibyte codepoints
         labels = tuple(range(0, 256))
     elif font.encoding == 'ascii':
         labels = tuple(range(0, 128))
     else:
+        resample = True
+        # NFNT can only store encodings from a pre-defined list of 'scripts'
+        # for fonts with other encodings, get glyphs corresponding to mac-roman
         font = font.label()
-        labels = tuple(Char(_c) for _c in charmaps['mac-roman'].mapping.values())
+        labels = tuple(Char(_c) for _i, _c in sorted(charmaps['mac-roman'].mapping.items()))
     subfont = font.subset(labels=labels)
     if not subfont.glyphs:
         raise FileFormatError('No suitable characters for NFNT font')
-    glyphs = [*subfont.glyphs, font.get_default_glyph()]
+    glyphs = [*subfont.glyphs, font.get_default_glyph().modify(labels=(), tag='missing')]
     font = font.modify(glyphs, encoding=None)
+    if resample:
+        font = font.label(codepoint_from='mac-roman', overwrite=True)
     return font
 
 
 def _normalize_glyph(g, ink_bounds):
     """
     Trim the horizontal to glyph's ink bounds
     and expand the vertical to font's ink bounds
@@ -436,116 +462,191 @@
     return g.expand(
         bottom=g.shift_up - ink_bounds.bottom,
         top=ink_bounds.top-g.height-g.shift_up
     )
 
 
 def _normalize_metrics(font):
-    """Calculate metrics for NFNT format."""
-    # reduce to ink bounds horizontally, font ink bounds vertically
+    """Reduce to ink bounds horizontally, font ink bounds vertically."""
     glyphs = tuple(_normalize_glyph(_g, font.ink_bounds) for _g in font.glyphs)
-    # calculate kerning. only negative kerning is handled
-    kern = min(_g.left_bearing for _g in glyphs)
-    kern = max(0, -kern)
+    font = font.modify(glyphs)
+    return font
+
+
+def _calculate_nfnt_glyph_metrics(glyphs):
+    """Calculate metrics for NFNT format."""
+    # calculate maximum kerning (=most negative bearing), zero if all bearings positive
+    # this equals the kernMax field of the fontRec
+    kern_max = min(0, min(_g.left_bearing for _g in glyphs if _g))
     # add apple metrics to glyphs
     glyphs = tuple(
-        _g.modify(wo_offset=_g.left_bearing+kern, wo_width=_g.advance_width)
+        (
+            None if _g is None else
+            _g.modify(wo_offset=_g.left_bearing-kern_max, wo_width=_g.advance_width)
+        )
         for _g in glyphs
     )
     # check that glyph widths and offsets fit
-    if any(_g.wo_width >= 255 for _g in glyphs):
+    if any(_g.wo_width >= 255 for _g in glyphs if _g):
         raise FileFormatError('NFNT character width must be < 255')
-    if any(_g.wo_offset >= 255 for _g in glyphs):
+    if any(_g.wo_offset >= 255 for _g in glyphs if _g):
         raise FileFormatError('NFNT character offset must be < 255')
-    font = font.modify(glyphs)
-    return font, kern
+    empty = Glyph(wo_offset=255, wo_width=255)
+    glyphs = tuple(empty if _g is None else _g for _g in glyphs)
+    return glyphs
 
 
-def _create_nfnt(font, endian, ndescent_is_high):
-    """Create FONT/NFNT resource."""
-    # fontType is ignored
-    # glyph-width table and image-height table not included
+def generate_nfnt_header(font, endian):
+    """Generate a bare NFNT header with no bitmaps yet."""
     base = {'b': be, 'l': le}[endian[:1].lower()]
     NFNTHeader = nfnt_header_struct(base)
     FontType = NFNTHeader.element_types['fontType']
+    # subset_for_nfnt has sorted on codepoint and added a 'missing' glyph
+    first_char = int(min(font.get_codepoints()))
+    last_char = int(max(font.get_codepoints()))
+    # generate NFNT header
+    fontrec = NFNTHeader(
+        # this seems to be always 0x9000, 0xb000
+        # even if docs say reserved_15 should be 0
+        # we don't provide a scalable width or height tables
+        fontType=FontType(
+            reserved_15=1, reserved_12=1,
+            fixed_width=font.spacing in ('monospace', 'character-cell'),
+        ),
+        firstChar=first_char,
+        lastChar=last_char,
+        widMax=font.max_width,
+        # An integer value that specifies the distance from the font rectangle's glyph origin
+        # to the left edge of the font rectangle, in pixels. If a glyph in the font kerns
+        # to the left, the amount is represented as a negative number. If the glyph origin
+        # lies on the left edge of the font rectangle, the value of the kernMax field is 0
+        kernMax=min(0, min(_g.left_bearing for _g in font.glyphs)),
+        nDescent=font.ink_bounds.bottom,
+        # font rectangle == font bounding box
+        fRectWidth=font.bounding_box.x,
+        fRectHeight=font.bounding_box.y,
+        # word offset to width/offset table
+        # keep 0 for empty NFNT
+        owTLoc=0,
+        # docs define fRectHeight = ascent + descent
+        # and generally suggest ascent and descent equal ink bounds
+        # that's also monobit's *default* ascent & descent but is overridable
+        ascent=font.ink_bounds.top,
+        descent=-font.ink_bounds.bottom,
+        # define leading in terms of bounding box, not pixel-height
+        leading=font.line_height - font.bounding_box.y,
+        # rowWords is 0 for empty NFNT, strike width in words for NFNT with bitmaps.
+        rowWords=0,
+    )
+    logging.debug('NFNT header: %s', fontrec)
+    return Props(
+        fontrec=fontrec,
+        font_strike=b'', loc_table=b'', wo_table=b'',
+        width_table=b'', height_table=b'',
+    )
+
+
+def convert_to_nfnt(
+        font, endian, ndescent_is_high, create_width_table, create_height_table
+    ):
+    """Convert monobit font to NFNT/FONT data structures."""
+    # fontType is ignored
+    # glyph-width table and image-height table not included
+    base = {'b': be, 'l': le}[endian[:1].lower()]
     LocEntry = loc_entry_struct(base)
     WOEntry = wo_entry_struct(base)
-    # subset the font. we need a font structure to calculate ink bounds
-    font = _subset(font)
-    font, kern = _normalize_metrics(font)
+    WidthEntry = width_entry_struct(base)
+    font = _normalize_metrics(font)
     # build the font-strike data
     strike_raster = Raster.concatenate(*(_g.pixels for _g in font.glyphs))
     # word-align strike
     strike_raster = strike_raster.expand(right=16-(strike_raster.width%16))
     font_strike = strike_raster.as_bytes()
     # get contiguous glyph list
-    glyphs = font.glyphs
-    first_char = int(glyphs[0].codepoint)
-    last_char = int(glyphs[-2].codepoint)
-    empty = Glyph(wo_offset=255, wo_width=255)
+    # subset_for_nfnt has sorted on codepoint and added a 'missing' glyph
+    first_char = int(min(font.get_codepoints()))
+    last_char = int(max(font.get_codepoints()))
     glyph_table = [
-        font.get_glyph(codepoint=_code, missing=empty)
+        font.get_glyph(codepoint=_code, missing=None)
         for _code in range(first_char, last_char+1)
     ]
-    missing = glyphs[-1]
-    glyph_table.append(missing)
+    # reappend 'missing' glyph
+    glyph_table.append(font.glyphs[-1])
+    # calculate glyph metrics and fill in empties
+    glyph_table = _calculate_nfnt_glyph_metrics(glyph_table)
     # build the width-offset table
+    empty = Glyph(wo_offset=255, wo_width=255)
     wo_table = b''.join(
         # glyph.wo_width and .wo_offset set in normalise_metrics
         bytes(WOEntry(width=_g.wo_width, offset=_g.wo_offset))
-        # empty entry needed at the end.
+        # extra empty entry needed at the end.
         for _g in chain(glyph_table, [empty])
     )
     # build the location table
     loc_table = b''.join(
         bytes(LocEntry(offset=_offset))
         for _offset in accumulate((_g.width for _g in glyph_table), initial=0)
     )
+    # build the glyph-width table
+    if create_width_table:
+        width_table = b''.join(
+            bytes(WidthEntry(width=int(round(_g.scalable_width * 256))))
+            for _g in glyph_table
+        )
+    else:
+        width_table = b''
+    # build the image-height table
+    # this isn't tested and probably won't be - seems this table gets ignored
+    if create_height_table:
+        height_table = b''.join(
+            bytes(HeightEntry(
+                # offset from top line to first ink row
+                # for normalised glyphs, this is the same as top padding
+                offset=font.ink_bounds.top-_g.ink_bounds.top,
+                height=_g.bounding_box.y
+            ))
+            for _g in glyph_table
+        )
+    else:
+        height_table = b''
+    # generate base fontrec
+    fontrec = generate_nfnt_header(font, endian).fontrec
+    fontrec.fontType.has_width_table = create_width_table
+    fontrec.fontType.has_height_table = create_height_table
+    # word offset to width/offset table
     # owTLoc is the offset from the field itself
     # the remaining size of the header including owTLoc is 5 words
     owt_loc = (len(font_strike) + len(loc_table) + 10) >> 1
-    # generate NFNT header
-    fontrec = NFNTHeader(
-        # this seems to be always 0x9000, 0xb000
-        # even if docs say reserved_15 should be 0
-        # we don't provide a scalable width or height tables
-        fontType=FontType(
-            reserved_15=1, reserved_12=1,
-            fixed_width=font.spacing in ('monospace', 'character-cell'),
-        ),
-        firstChar=first_char,
-        lastChar=last_char,
-        widMax=max(_g.advance_width for _g in glyphs),
-        kernMax=-kern,
-        nDescent=font.ink_bounds.bottom,
-        # font rectangle == font bounding box
-        #max(_g.width + _g.left_bearing + kern for _g in glyphs),
-        fRectWidth=font.bounding_box.x,
-        fRectHeight=font.bounding_box.y,
-        # word offset to width/offset table
-        owTLoc=owt_loc & 0xffff,
-        # docs define fRectHeight = ascent + descent
-        # and generally suggest ascent and descent equal ink bounds
-        # that's also monobit's *default* ascent & descent but is overridable
-        ascent=font.ink_bounds.top,
-        descent=-font.ink_bounds.bottom,
-        # define leading in terms of bounding box, not pixel-height
-        leading=font.line_height - font.bounding_box.y,
-        rowWords=strike_raster.width // 16,
-    )
+    fontrec.owTLoc = owt_loc & 0xffff
     owt_loc_high = owt_loc >> 16
     if ndescent_is_high and owt_loc_high:
         fontrec.nDescent = owt_loc_high
-    logging.debug('NFNT header: %s', fontrec)
-    data = b''.join((
-        bytes(fontrec),
-        font_strike,
-        loc_table,
-        wo_table
-    ))
+    # fill in the rowWords, indicating that we do have a strike.
+    fontrec.rowWords = strike_raster.width // 16
     # fbr = max width from origin (including whitespace) and right kerned pixels
     # for IIgs header
     fbr_extent = max(
         _g.width + _g.left_bearing + max(_g.right_bearing, 0)
-        for _g in glyphs
+        for _g in font.glyphs
     )
-    return data, owt_loc_high, fbr_extent
+    return Props(
+        fontrec=fontrec,
+        font_strike=font_strike,
+        loc_table=loc_table,
+        wo_table=wo_table,
+        width_table=width_table,
+        height_table=height_table,
+        owt_loc_high=owt_loc_high,
+        fbr_extent=fbr_extent,
+    )
+
+
+def nfnt_data_to_bytes(nfnt_data):
+    """Convert NFNT/FONT dtata structure to binary representation."""
+    return b''.join((
+        bytes(nfnt_data.fontrec),
+        nfnt_data.font_strike,
+        nfnt_data.loc_table,
+        nfnt_data.wo_table,
+        nfnt_data.width_table,
+        nfnt_data.height_table,
+    ))
```

### Comparing `monobit-0.41.0/monobit/formats/os2/__init__.py` & `monobit-0.42.0/monobit/formats/os2/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/os2/gpifont.py` & `monobit-0.42.0/monobit/formats/os2/gpifont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/os2/lx.py` & `monobit-0.42.0/monobit/formats/os2/lx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/os2/ne.py` & `monobit-0.42.0/monobit/formats/os2/ne.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
 from ...magic import FileFormatError
 from ...struct import little_endian as le
-from ..windows.ne import _NE_HEADER
+from ..windows.ne import NE_HEADER
 from .gpifont import parse_os2_font_directory
 
 # resource ids
 OS2RES_FONTDIR = 6
 OS2RES_FONTFACE = 7
 
 # Resource table entry
@@ -39,15 +39,15 @@
 )
 
 
 def read_os2_ne(instream, all_type_ids):
     """Read an OS/2 16-bit NE executable."""
     # the header is the same as for the Windows NE format
     ne_offset = instream.tell()
-    header = _NE_HEADER.read_from(instream)
+    header = NE_HEADER.read_from(instream)
     if header.ne_exetyp != 1:
         logging.warning(
             'Not an OS/2 NE file: EXE type %d', header.ne_exetyp
         )
     logging.debug(header)
     # parse the segment table
     seg_table = ST_ENTRY.array(header.ne_cseg).read_from(
```

### Comparing `monobit-0.41.0/monobit/formats/sfnt/sfnt.py` & `monobit-0.42.0/monobit/formats/sfnt/sfnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from ...properties import Props
 from ...font import Font
 from ...glyph import Glyph
 from ...raster import Raster
 from ...labels import Tag, Char, Codepoint
 from ...storage import loaders, savers
 from ...magic import FileFormatError
-from ..windows.fnt import _WEIGHT_MAP, CHARSET_MAP
+from ..windows import WEIGHT_MAP, CHARSET_MAP
 
 
 # errors that invalidate only one strike or resource, not the whole file
 
 class ResourceFormatError(FileFormatError):
     """Unsupported parameters in resource."""
 
@@ -694,28 +694,28 @@
     return props
 
 
 ###############################################################################
 # 'head' or 'bhed' table
 
 # interpretation of head.macStyle flags
-_STYLE_MAP = {
+STYLE_MAP = {
     0: 'bold',
     1: 'italic',
     2: 'underline',
     3: 'outline',
     4: 'shadow',
     5: 'condensed',
     6: 'extended',
 }
 
 def mac_style_name(font_style):
     """Get human-readable representation of font style."""
     return ' '.join(
-        _tag for _bit, _tag in _STYLE_MAP.items() if font_style & (1 << _bit)
+        _tag for _bit, _tag in STYLE_MAP.items() if font_style & (1 << _bit)
     )
 
 def _convert_head_props(head):
     """Convert font properties from head/bhed table."""
     if not head:
         return Props()
     props = Props(
@@ -844,18 +844,18 @@
 
 
 ###############################################################################
 # 'OS/2' table
 
 # usWeightClass
 # these align with Windows values
-#_WEIGHT_MAP
+#WEIGHT_MAP
 
 # usWidthClass
-_SETWIDTH_MAP = {
+SETWIDTH_MAP = {
     1: 'ultra-condensed',
     2: 'extra-condensed',
     3: 'condensed',
     4: 'semi-condensed',
     5: 'normal', #'medium',
     6: 'semi-expanded',
     7: 'expanded',
@@ -865,16 +865,16 @@
 
 def _convert_os_2_props(os_2, vert_fu_p_pix, hori_fu_p_pix):
     """Convert font properties from OS/2 table."""
     if not os_2:
         return Props()
     weight = min(900, max(100, 100 * round(os_2.usWeightClass / 100)))
     props = Props(
-        weight=_WEIGHT_MAP.get(weight, None),
-        setwidth=_SETWIDTH_MAP.get(os_2.usWidthClass, None),
+        weight=WEIGHT_MAP.get(weight, None),
+        setwidth=SETWIDTH_MAP.get(os_2.usWidthClass, None),
         subscript_size=os_2.ySubscriptYSize // vert_fu_p_pix,
         subscript_offset=(
             int(os_2.ySubscriptXOffset // hori_fu_p_pix),
             -int(os_2.ySubscriptYOffset // vert_fu_p_pix)
         ),
         superscript_size=os_2.ySuperscriptYSize // vert_fu_p_pix,
         superscript_offset=(
```

### Comparing `monobit-0.41.0/monobit/formats/sfnt/sfnt_writer.py` & `monobit-0.42.0/monobit/formats/sfnt/sfnt_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import logging
 
 from ...glyph import Glyph
 from ...binary import ceildiv
 from ...storage import loaders, savers
 from ...properties import reverse_dict
-from .sfnt import _WEIGHT_MAP, _SETWIDTH_MAP, check_fonttools
+from .sfnt import WEIGHT_MAP, SETWIDTH_MAP, check_fonttools
 from .sfnt import load_sfnt, load_collection
 from ...labels import Tag
 from ...taggers import CodepointTagger
 from ...basetypes import to_number
 
 from . import fonttools
 from .fonttools import check_fonttools
@@ -102,16 +102,16 @@
 
 def _convert_to_os_2_props(font, _to_funits):
     """Convert font properties to `OS/2` table."""
     # weight = min(900, max(100, 100 * round(os_2.usWeightClass / 100)))
     props = dict(
         version=3,
         # characteristics
-        usWeightClass=reverse_dict(_WEIGHT_MAP).get(font.weight, 400),
-        usWidthClass=reverse_dict(_SETWIDTH_MAP).get(font.setwidth, 5),
+        usWeightClass=reverse_dict(WEIGHT_MAP).get(font.weight, 400),
+        usWidthClass=reverse_dict(SETWIDTH_MAP).get(font.setwidth, 5),
         sxHeight=_to_funits(font.x_height),
         sCapHeight=_to_funits(font.cap_height),
         # subscript metrics
         ySubscriptXSize=_to_funits(font.subscript_size),
         ySubscriptYSize=_to_funits(font.subscript_size),
         ySubscriptXOffset=_to_funits(font.subscript_offset.x),
         ySubscriptYOffset=-_to_funits(font.subscript_offset.y),
@@ -138,48 +138,52 @@
         usBreakChar=_label_to_utf16(font, font.word_boundary, 0x20),
         # vendor ID - can be left blank (four spaces)
         achVendID=b'    ',
     )
     return props
 
 
+def to_postscript_name(name):
+    """Postscript name must be printable ascii, no [](){}<>/%, max 63 chars."""
+    ps_name = ''.join(
+        _c if _c.isalnum() and _c.isascii() else '-'
+        for _c in name
+    )
+    ps_name = ps_name[:63]
+    # expected to be Title-Cased (at least on Mac, see FontForge code comments)
+    return ps_name.title()
+
+
 def _convert_to_name_props(font):
     """Convert font properties to `name` table."""
     # `name` table should only store x.y version numbers
     # while font.revision could be any string
     try:
         version_number = to_number(font.revision)
         extra = ''
     except ValueError:
         version_number = 0.0
         extra = f'; {font.revision}'
-    # must start with 'Version x.y'
-    # but may contain additional info after `;`
-    version_string = f'Version {version_number:1.1f}{extra}'
-    # postscript name must be printable ascii, no [](){}<>/%, max 63 chars
-    ps_name = ''.join(
-        _c if _c.isalnum() and _c.isascii() else '-'
-        for _c in font.name
-    )
-    ps_name = ps_name[:63]
     props = dict(
         # 0
         copyright=font.copyright,
         # 1
         familyName=font.family,
         # 2
         styleName=font.subfamily,
         # 3
-        uniqueFontIdentifier=font.font_id or ps_name,
+        uniqueFontIdentifier=font.font_id or to_postscript_name(font.name),
         # 4
         fullName=font.name,
         # 5
-        version=version_string,
+        # must start with 'Version x.y'
+        # but may contain additional info after `;`
+        version=f'Version {version_number:1.1f}{extra}',
         # 6
-        psName=ps_name,
+        psName=to_postscript_name(font.name),
         # trademark (nameID 7)
         # 8
         manufacturer=font.foundry,
         # 9
         designer=font.author,
         # 10
         # description=font.description,
```

### Comparing `monobit-0.41.0/monobit/formats/sfnt/fonttools/E_B_S_C_.py` & `monobit-0.42.0/monobit/formats/sfnt/fonttools/E_B_S_C_.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/sfnt/fonttools/__init__.py` & `monobit-0.42.0/monobit/formats/sfnt/fonttools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 def ebdt_monkey_patch():
     """Monkey patch to fix a bug in fontTools (as of 4.39.3)"""
     from fontTools.ttLib.tables import E_B_D_T_
     from fontTools.ttLib.tables.E_B_D_T_ import bytesjoin, byteord, bytechr
 
     def _reverseBytes(data):
-        if len(data) != 1:
+        if isinstance(data, bytes) and len(data) != 1:
             # this is where the bug was
-            return bytesjoin(map(_reverseBytes, map(chr, data)))
+            return bytesjoin(map(_reverseBytes, data))
         byte = byteord(data)
         result = 0
         for i in range(8):
             result = result << 1
             result |= byte & 1
             byte = byte >> 1
         return bytechr(result)
```

### Comparing `monobit-0.41.0/monobit/formats/text/draw.py` & `monobit-0.42.0/monobit/formats/text/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     ink: character used for inked/foreground pixels (default #)
     paper: character used for uninked/background pixels (default -)
     unicode: interpret codepoint as Unicode (default: True)
     """
     DrawGlyph.ink = ink
     DrawGlyph.paper = paper
-    return _load_draw(
+    return load_draw(
         instream.text, blocktypes=(DrawGlyph, DrawComment, Empty),
         unicode=unicode
     )
 
 
 @savers.register(linked=load_hexdraw)
 def save_hexdraw(fonts, outstream, ink:str='#', paper:str='-', unicode:bool=True):
@@ -52,15 +52,15 @@
     if len(fonts) > 1:
         raise FileFormatError("Can only save one font to hexdraw file.")
     _save_draw(fonts[0], outstream.text, ink=ink, paper=paper, unicode=unicode)
 
 
 # read hexdraw file
 
-def _load_draw(text_stream, *, blocktypes, unicode):
+def load_draw(text_stream, *, blocktypes, unicode):
     """Parse a hexdraw-style file."""
     glyphs = []
     font_comments = []
     current_comment = []
     for block in iter_blocks(text_stream, blocktypes):
         if isinstance(block, DrawComment):
             if not glyphs:
@@ -136,15 +136,15 @@
     )
 
 
 ###############################################################################
 # mkwinfon .fd
 
 from ...properties import Props
-from ..windows.fnt import _WEIGHT_MAP, CHARSET_MAP
+from ..windows import WEIGHT_MAP, CHARSET_MAP
 
 
 FD_KEYS = {
     'facename',
     'copyright',
     'height',
     'ascent',
```

### Comparing `monobit-0.41.0/monobit/formats/text/hex.py` & `monobit-0.42.0/monobit/formats/text/hex.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import logging
 import string
 
 from ...storage import loaders, savers
 from ...magic import FileFormatError
 from ...font import Font
 from ...glyph import Glyph
-from .draw import _load_draw, DrawGlyph, DrawComment, Empty
+from .draw import load_draw, DrawGlyph, DrawComment, Empty
 
 
 @loaders.register(name='pcbasic',)
 def load_hext(instream):
     """Load 8xN multi-cell font from PC-BASIC extended .HEX file."""
     return _load_hex(instream)
 
@@ -44,15 +44,15 @@
     _save_hex(font, outstream.text, _fits_in_hext)
 
 
 # loader
 
 def _load_hex(instream):
     """Load 8x16 multi-cell font from Unifont .HEX file."""
-    return _load_draw(
+    return load_draw(
         instream.text, blocktypes=(HexGlyph, DrawComment, Empty), unicode=True
     )
 
 
 class HexGlyph(DrawGlyph):
 
     def ends(self, line):
```

### Comparing `monobit-0.41.0/monobit/formats/text/yaff.py` & `monobit-0.42.0/monobit/formats/text/yaff.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from itertools import count, zip_longest
 from collections import deque
 from functools import cached_property
 
 from ...storage import loaders, savers
 from ...encoding import charmaps
 from ...magic import FileFormatError
-from ...font import Font
+from ...font import Font, FontProperties
 from ...glyph import Glyph
 from ...raster import Raster
 from ...labels import Label, strip_matching
 from ...properties import Props
 from ...basetypes import Coord, passthrough
 from .draw import NonEmptyBlock, DrawComment, Empty, Unparsed, iter_blocks
 from .draw import format_comment
@@ -265,29 +265,38 @@
 
     get_glyph_value = get_value
 
 
 
 def normalise_property(field):
     # preserve distinction between starting underscore (internal) and starting dash (user property)
-    return field[:1] + field[1:].replace('-', '_')
+    return field.replace('-', '_')
 
 
+# keywords that take a label value
+# these need special treatment as quotes must not be stripped
+_LABEL_VALUED_KEYS = tuple(
+    _k for _k, _v in FontProperties.__annotations__.items() if _v == Label
+)
+
 
 class YaffProperty(NonEmptyBlock, YaffParams):
 
     def starts(self, line):
         return (
             line[:1] not in self.whitespace
             and line[-1:] != self.separator
             and self.separator in line
         )
 
     def get_value(self):
-        _, _, value = self.lines[0].partition(self.separator)
+        key, _, value = self.lines[0].partition(self.separator)
+        # label values need special treatment as quotes must not be stripped
+        if key in _LABEL_VALUED_KEYS:
+            return value
         return _strip_quotes(value)
 
     def get_key(self):
         key, _, _ = self.lines[0].partition(self.separator)
         return normalise_property(key)
 
 
@@ -324,20 +333,21 @@
         # we need to check the contents
         return first[:1] in (self.ink, self.paper) or set(first) == set(self.empty)
 
 
 ##############################################################################
 # write file
 
-def _globalise_glyph_metrics(glyphs):
+def globalise_glyph_metrics(glyphs):
     """If all glyph props are equal, take them global."""
     properties = {}
     for key in (
             'shift_up', 'left_bearing', 'right_bearing',
             'shift_left', 'top_bearing', 'bottom_bearing',
+            'scalable_width',
         ):
         distinct = set(_g.get_defined(key) for _g in glyphs)
         if len(distinct) == 1:
             value = distinct.pop()
             if value is not None:
                 properties[key] = value
     return properties
@@ -362,16 +372,20 @@
             'spacing': font.spacing,
         }
         if font.spacing in ('character-cell', 'multi-cell'):
             props['cell_size'] = font.cell_size
         else:
             props['bounding_box'] = font.bounding_box
         props.update(font.get_properties())
-        global_metrics = _globalise_glyph_metrics(font.glyphs)
-        props.update(global_metrics)
+        global_metrics = globalise_glyph_metrics(font.glyphs)
+        # keep only nonzero or non-default globalised properties
+        props.update({
+            _k: _v for _k, _v in global_metrics.items()
+            if _v or _v != Glyph.get_default(_k)
+        })
         if props:
             # write recognised yaff properties first, in defined order
             for key, value in props.items():
                 if value != font.get_default(key):
                     _write_property(outstream, key, value, font.get_comment(key))
             outstream.write('\n')
         for glyph in font.glyphs:
@@ -415,22 +429,21 @@
     if value is None:
         return
     # write property comment
     if comments:
         outstream.write(
             f'\n{indent}{format_comment(comments, YaffParams.comment)}\n'
         )
-    if not key.startswith('_'):
-        key = key.replace('_', '-')
+    key = key.replace('_', '-')
     # write key-value pair
     if isinstance(value, Label) or not isinstance(value, str):
         # do not quote converted non-strings (plus Tag and Char which are str)
-        # FIXME: reader will strip quotes and misinterpret some labels
+        # note that these need special treatment in the reader, or it
+        # will strip quotes and misinterpret some labels
         # so non-ascii or single-char tags will be converted to Char not Tag
-        # common cases (.notdef, missing, default, uniFFFD) will be OK
         quoter = passthrough
     else:
         quoter = _quote_if_needed
     value = str(value)
     if '\n' not in value:
         outstream.write(f'{indent}{key}: {quoter(value)}\n')
     else:
```

### Comparing `monobit-0.41.0/monobit/formats/windows/LICENSE.md` & `monobit-0.42.0/monobit/formats/windows/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/windows/__init__.py` & `monobit-0.42.0/monobit/formats/windows/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from ...storage import loaders, savers
 from ...magic import FileFormatError
 from .fnt import create_fnt
 from .fnt import convert_win_fnt_resource, FNT_MAGIC_1, FNT_MAGIC_2, FNT_MAGIC_3
 
 # used by other formats
-from .fnt import _normalise_metrics, CHARSET_MAP, CHARSET_REVERSE_MAP
+from .fnt import WEIGHT_MAP, WEIGHT_REVERSE_MAP, CHARSET_MAP, CHARSET_REVERSE_MAP
 
 
 @loaders.register(
     name='win',
     magic=(FNT_MAGIC_1, FNT_MAGIC_2, FNT_MAGIC_3),
     patterns=('*.fnt',),
 )
```

### Comparing `monobit-0.41.0/monobit/formats/windows/fnt.py` & `monobit-0.42.0/monobit/formats/windows/fnt.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 _FALLBACK_CHARSET = 0xff
 # "dfDefaultChar should indicate a special character in the font which is not a space."
 # codepoint 0x80 is unmapped in windows-ansi-2.0 and commonly used for default
 _FALLBACK_DEFAULT = 0x80
 # "dfBreakChar is normally (32 - dfFirstChar), which is an ASCII space."
 _FALLBACK_BREAK = 0x20
 
+# despite the presence of MBCS character set codes,
+# FNT can only hold single-byte codepoints
+# as firstChar and lastChar are byte-sized
+_FNT_RANGE = range(256)
 
 # official but vague documentation:
 # https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-wmf/0d0b32ac-a836-4bd2-a112-b6000a1b4fc9
 #
 # The CharacterSet Enumeration defines the possible sets of character glyphs that are defined in fonts for graphics output.
 #      typedef  enum
 #      {
@@ -186,27 +190,27 @@
 # FW_SEMIBOLD	600
 # FW_DEMIBOLD	600
 # FW_BOLD	700
 # FW_EXTRABOLD	800
 # FW_ULTRABOLD	800
 # FW_HEAVY	900
 # FW_BLACK	900
-_WEIGHT_MAP = {
+WEIGHT_MAP = {
     0: '', # undefined/unknown
     100: 'thin', # bdf 'ultra-light' is windows' 'thin'
     200: 'extra-light', # windows 'ultralight' equals 'extralight'
     300: 'light',
     400: 'regular', # 'regular' is 'normal' but less than 'medium' :/ ... bdf has a semi-light here
     500: 'medium',
     600: 'semi-bold',
     700: 'bold',
     800: 'extra-bold', # windows 'ultrabold' equals 'extrabold'
     900: 'heavy', # bdf 'ultra-bold' is 'heavy'
 }
-_WEIGHT_REVERSE_MAP = reverse_dict(_WEIGHT_MAP)
+WEIGHT_REVERSE_MAP = reverse_dict(WEIGHT_MAP)
 
 # pitch and family
 # low bit: 1 - proportional 0 - monospace
 # upper bits: family (like bdf add_style_name)
 #
 # Don't care or don't know.
 _FF_DONTCARE = 0<<4
@@ -563,15 +567,15 @@
     if win_props.dfStrikeOut:
         deco.append('strikethrough')
     if deco:
         properties['decoration'] = ' '.join(deco)
     weight = win_props.dfWeight
     if weight:
         weight = max(100, min(900, weight))
-        properties['weight'] = _WEIGHT_MAP.get(round(weight, -2), None)
+        properties['weight'] = WEIGHT_MAP.get(round(weight, -2), None)
     charset = win_props.dfCharSet
     if charset in CHARSET_MAP:
         properties['encoding'] = CHARSET_MAP[charset]
     else:
         properties['windows.dfCharSet'] = str(charset)
     properties['style'] = _STYLE_MAP.get(win_props.dfPitchAndFamily & 0xff00, None)
     if win_props.dfBreakChar:
@@ -602,101 +606,69 @@
             raise FileFormatError('ABC spacing properties not supported')
     return properties
 
 
 ##############################################################################
 # windows .FNT writer
 
-def _subset_storable(font):
-    """Subset glyphs storable in Windows font."""
-    # ensure codepoint values are set, if possible
-    font = font.label(codepoint_from=font.encoding)
-    # only include single-byte encoded glyphs
-    # FNT can hold at most the codepoints 0..256 as these fields are byte-sized
-    codepoints = tuple(
-        _cp for _cp in font.get_codepoints() if len(_cp) == 1
-    )
-    if not codepoints:
-        raise FileFormatError(
-            'Windows font can only encode glyphs with single-byte codepoints; none found in font.'
-        )
-    font = font.subset(codepoints=codepoints)
-    return font
 
-def _make_contiguous(font, pix_width):
+def _make_contiguous(font):
     """Fill out a contiguous range of glyphs."""
+    # x_width should equal average width
+    # this is 0 for proportional fonts
+    pix_width = font.cell_size.x
     # blank glyph of standard size
     blank = Glyph.blank(pix_width, font.raster_size.y)
     # char table; we need a contiguous range between the min and max codepoints
     codepoints = font.get_codepoints()
     ord_glyphs = [
         font.get_glyph(_codepoint, missing=blank)
         for _codepoint in range(min(codepoints)[0], max(codepoints)[0]+1)
     ]
     # add the guaranteed-blank glyph
     ord_glyphs.append(blank)
     font = font.modify(ord_glyphs)
     return font
 
-def _normalise_metrics(font):
-    """Normalise glyph representation for Windows."""
-    # fix auto-generated values
-    font = font.modify(ascent=font.ascent, descent=font.descent)
-    add_shift_up = max(0, -min(_g.shift_up for _g in font.glyphs))
-    ord_glyphs = tuple(
-        _g.expand(
-            # bring all glyphs to same height
-            top=max(0, font.raster_size.y-_g.height - add_shift_up),
-            # expand into horizontal bearings
-            left=max(0, _g.left_bearing),
-            right=max(0, _g.right_bearing),
-            # expand by positive shift to make all upshifts equal
-            bottom=_g.shift_up + add_shift_up
-        ).drop('shift_up')
-        for _g in font.glyphs
-    )
-    font = font.modify(ord_glyphs)
-    return font, add_shift_up
-
 
 def create_fnt(font, version=0x200, vector=False):
     """Create .FNT from monobit font."""
-    # take only the glyphs we can store
-    font = _subset_storable(font)
-    font, add_shift_up = _normalise_metrics(font)
-    if font.spacing == 'proportional':
-        pix_width = 0
-    else:
-        # x_width should equal average width
-        pix_width = font.raster_size.x
-    font = _make_contiguous(font, pix_width)
+    # ensure codepoint values are set, if possible
+    font = font.label(codepoint_from=font.encoding)
+    # only include single-byte encoded glyphs
+    # as firstChar and lastChar are byte-sized
+    font = font.subset(codepoints=_FNT_RANGE)
+    font = _make_contiguous(font)
+    # bring to equal-height, equal-upshift, padded normal form
+    font = font.equalise_horizontal()
     bitmaps, char_table, offset_bitmaps, byte_width = _convert_to_fnt_glyphs(
-        font, version, vector, add_shift_up
+        font, version, vector
     )
     bitmap_size = sum(len(_b) for _b in bitmaps)
     win_props, header_ext, stringtable = _convert_to_fnt_props(
         font, version, vector,
         offset_bitmaps, bitmap_size, byte_width,
-        add_shift_up
     )
     data = (
         bytes(win_props) + bytes(header_ext)
         + b''.join(char_table)
         + b''.join(bitmaps)
         + b''.join(stringtable)
     )
     return data
 
 
 def _convert_to_fnt_props(
         font, version, vector,
         offset_bitmaps, bitmap_size, byte_width,
-        add_shift_up
     ):
     """Convert font to FNT headers."""
+    upshifts = set(_g.shift_up for _g in font.glyphs)
+    shift_up, *remainder = upshifts
+    assert not remainder
     # get lowest and highest codepoints (contiguous glyphs followed by blank)
     min_ord = font.glyphs[0].codepoint[0]
     max_ord = font.glyphs[-2].codepoint[0]
     # if encoding is compatible, use it; otherwise set to fallback value
     charset = CHARSET_REVERSE_MAP.get(font.encoding, _FALLBACK_CHARSET)
     default = font.get_glyph(font.default_char, missing='empty').codepoint
     if len(default) == 1:
@@ -725,41 +697,42 @@
     device_name_offset = face_name_offset + len(face_name)
     device_name = font.device.encode('latin-1', 'replace') + b'\0'
     file_size = device_name_offset + len(device_name)
     # set device name pointer to zero for 'generic font'
     if not device_name or device_name == b'\0':
         device_name_offset = 0
     try:
-        weight = _WEIGHT_REVERSE_MAP[font.weight]
+        weight = WEIGHT_REVERSE_MAP[font.weight]
     except KeyError:
         logging.warning(
             f'Weight `{font.weight}` not supported by Windows FNT resource format, '
             '`regular` will be used instead.'
         )
-        weight = _WEIGHT_REVERSE_MAP['regular']
+        weight = WEIGHT_REVERSE_MAP['regular']
     # create FNT file
     win_props = _FNT_HEADER(
         dfVersion=version,
         dfSize=file_size,
         dfCopyright=font.copyright.encode('ascii', 'replace')[:60].ljust(60, b'\0'),
         dfType=1 if vector else 0,
         dfPoints=int(font.point_size),
         dfVertRes=font.dpi.y,
         dfHorizRes=font.dpi.x,
         # Windows dfAscent means distance between matrix top and baseline
-        dfAscent=font.raster_size.y - add_shift_up,
+        # common shift_up is negative or zero in padded normal form
+        dfAscent=font.raster_size.y + shift_up,
         #'ascent': win_props.dfAscent - win_props.dfInternalLeading,
-        dfInternalLeading=font.raster_size.y - add_shift_up - font.ascent,
+        dfInternalLeading=font.raster_size.y + shift_up - font.ascent,
         #'line_height': win_props.dfPixHeight + win_props.dfExternalLeading,
         dfExternalLeading=font.line_height-font.raster_size.y,
         dfItalic=(font.slant in ('italic', 'oblique')),
         dfUnderline=('underline' in font.decoration),
         dfStrikeOut=('strikethrough' in font.decoration),
-        dfWeight=_WEIGHT_REVERSE_MAP.get(
-            font.weight, _WEIGHT_REVERSE_MAP['regular']
+        dfWeight=WEIGHT_REVERSE_MAP.get(
+            font.weight, WEIGHT_REVERSE_MAP['regular']
         ),
         dfCharSet=charset,
         dfPixWidth=pix_width,
         dfPixHeight=font.raster_size.y,
         dfPitchAndFamily=pitch_and_family,
         # for 2.0+, we use actual average advance here (like fontforge but unlike mkwinfont)
         dfAvgWidth=round(font.average_width),
@@ -781,20 +754,23 @@
     if version == 0x300:
         # all are zeroes (default) except the flags for v3
         header_ext.dfFlags = v3_flags
     stringtable = face_name, device_name
     return win_props, header_ext, stringtable
 
 
-def _convert_to_fnt_glyphs(font, version, vector, add_shift_up):
+def _convert_to_fnt_glyphs(font, version, vector):
     """Convert glyphs to FNT bitmaps and offset tables."""
     if vector:
+        upshifts = set(_g.shift_up for _g in font.glyphs)
+        shift_up, *remainder = upshifts
+        assert not remainder
         # vector glyph data
         # this should equal the dfAscent value
-        win_ascent = font.raster_size.y - add_shift_up
+        win_ascent = font.raster_size.y + shift_up
         bitmaps = _convert_vector_glyphs_to_fnt(font.glyphs, win_ascent)
         byte_width = 0
     elif version == 0x100:
         strike = Raster.concatenate(*(_g.pixels for _g in font.glyphs))
         # spacer to ensure we'll be word-aligned (as_bytes will byte-align)
         spacer = Raster.blank(width=16-(strike.width%16), height=strike.height)
         strike = Raster.concatenate(strike, spacer)
```

### Comparing `monobit-0.41.0/monobit/formats/windows/mz.py` & `monobit-0.42.0/monobit/formats/windows/mz.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/windows/ne.py` & `monobit-0.42.0/monobit/formats/windows/ne.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 #   http://www.csn.ul.ie/~caolan/pub/winresdump/winresdump/doc/winexe.txt
 #   http://www.fileformat.info/format/exe/corion-ne.htm
 #   https://wiki.osdev.org/NE
 #   http://benoit.papillault.free.fr/c/disc2/exefmt.txt
 #
 
 # Windows executable (NE) header
-_NE_HEADER = le.Struct(
+NE_HEADER = le.Struct(
     # 00 Magic number NE_MAGIC
     ne_magic='2s',
     # 02 Linker Version number
     ne_ver='uint8',
     # 03 Linker Revision number
     ne_rev='uint8',
     # Offset of Entry Table
@@ -142,15 +142,15 @@
 def read_ne(instream, all_type_ids):
     """Read font resources from a Windows NE-format FON file."""
     # stream pointer is at the start of the NE header
     # but some offsets in the file are given from the MZ header before that
     ne_offset = instream.tell()
     instream.seek(0)
     data = instream.read()
-    header = _NE_HEADER.from_bytes(data, ne_offset)
+    header = NE_HEADER.from_bytes(data, ne_offset)
     logging.debug(header)
     if header.ne_exetyp not in (0, 2, 4):
         # 0 unknown (but used by Windows 1.0)
         # 1 OS/2
         # 2 Windows
         # 3 European MS_DOS 4.x
         # 4 Windows 386
@@ -355,36 +355,36 @@
     nonres = _create_nonresident_name_table(pack)
     res = _create_resident_name_table(pack)
     # entry table / imported names table should contain a zero word.
     entry = b'\0\0'
     # the actual font data
     resdata, font_start = _create_resource_data(pack, version, vector)
     # create resource table and align
-    header_size = stubsize + _NE_HEADER.size
+    header_size = stubsize + NE_HEADER.size
     post_size = len(res) + len(entry) + len(nonres)
     restable = _create_resource_table(header_size, post_size, len(resdata), n_fonts, font_start)
     # calculate offsets of stuff after the NE header.
-    off_res = _NE_HEADER.size + len(restable)
+    off_res = NE_HEADER.size + len(restable)
     off_entry = off_res + len(res)
     off_nonres = off_entry + len(entry)
     size_aligned = align(off_nonres + len(nonres), ALIGN_SHIFT)
     # create the NE header and put everything in place
-    ne_header = _NE_HEADER(
+    ne_header = NE_HEADER(
         ne_magic=b'NE',
         ne_ver=5,
         ne_rev=10,
         ne_enttab=off_entry,
         ne_cbenttab=len(entry),
         # 1<<3: protected mode only
         # 0x03: uses windows/p.m. api | 1<<7: dll or driver
         ne_flags=0x8308,
         ne_cbnrestab=len(nonres),
         # seg table is empty
-        ne_segtab=_NE_HEADER.size,
-        ne_rsrctab=_NE_HEADER.size,
+        ne_segtab=NE_HEADER.size,
+        ne_rsrctab=NE_HEADER.size,
         ne_restab=off_res,
         # point to empty table
         ne_modtab=off_entry,
         # point to empty table
         ne_imptab=off_entry,
         # nonresident names table offset is w.r.t. file start
         ne_nrestab=stubsize + off_nonres,
```

### Comparing `monobit-0.41.0/monobit/formats/windows/pe.py` & `monobit-0.42.0/monobit/formats/windows/pe.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/monobit/formats/xlfd/bdf.py` & `monobit-0.42.0/monobit/formats/xlfd/bdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from ...font import Font, Coord
 from ...raster import Raster
 from ...glyph import Glyph
 from ...encoding import charmaps, NotFoundError
 from ...taggers import tagmaps
 from ...labels import Char, Codepoint, Tag
 
-from .xlfd import _parse_xlfd_properties, _create_xlfd_properties
-from .xlfd import _create_xlfd_name, CUSTOM_PROP
+from .xlfd import parse_xlfd_properties, create_xlfd_properties
+from .xlfd import create_xlfd_name, CUSTOM_PROP
 
 
 @loaders.register(
     name='bdf',
     magic=(b'STARTFONT ',),
     patterns=('*.bdf',),
 )
@@ -167,15 +167,15 @@
 
 def _convert_from_bdf(bdf_glyphs, bdf_props, x_props):
     """Convert BDF data to monobit glyphs and properties."""
     # parse meaningful metadata
     known, global_metrics, bdf_unparsed = _extract_known_bdf_properties(bdf_props)
     properties = _convert_bdf_properties(known)
     glyphs = _convert_bdf_glyphs(bdf_glyphs, global_metrics, known)
-    xlfd_props = _parse_xlfd_properties(x_props, known['FONT'])
+    xlfd_props = parse_xlfd_properties(x_props, known['FONT'])
     # consistency checks
     if known['NCHARS'] != len(bdf_glyphs):
         logging.warning('Number of characters found does not match CHARS declaration.')
     for key, value in bdf_unparsed.items():
         logging.warning(f'Unrecognised BDF property {key}={value}')
         # preserve as custom property namespace, avoid clashes with yaff props
         properties[f'{CUSTOM_PROP}.{key}'] = value
@@ -357,16 +357,16 @@
         round(dwidth / (point_size / 1000) / (dpi / 72))
     )
 
 
 def _save_bdf(font, outstream):
     """Write one font to X11 BDF 2.1."""
     # property table
-    xlfd_props = _create_xlfd_properties(font)
-    xlfd_name = _create_xlfd_name(xlfd_props)
+    xlfd_props = create_xlfd_properties(font)
+    xlfd_name = create_xlfd_name(xlfd_props)
     bdf_props = _convert_to_bdf_properties(font, xlfd_name)
     # minimize glyphs to ink-bounds (BBX) before storing, except "cell" fonts
     if font.spacing not in ('character-cell', 'multi-cell'):
         font = font.reduce()
     # ensure character labels exist if needed
     if charmaps.is_unicode(font.encoding):
         font = font.label(match_whitespace=False, match_graphical=False)
```

### Comparing `monobit-0.41.0/monobit/formats/xlfd/hbf.py` & `monobit-0.42.0/monobit/formats/xlfd/hbf.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 from ...storage import loaders, savers
 from ...magic import FileFormatError
 from ...font import Font, Coord
 from ...glyph import Glyph
 from ...binary import ceildiv
 
 from .bdf import read_props
-from .xlfd import _parse_xlfd_properties, _create_xlfd_properties
-from .xlfd import _create_xlfd_name
-# from ..text.yaff import _globalise_glyph_metrics
-from ..windows import _normalise_metrics
+from .xlfd import parse_xlfd_properties, create_xlfd_properties
+from .xlfd import create_xlfd_name
+from ..text.yaff import globalise_glyph_metrics
 
 
 @loaders.register(
     name='hbf',
     magic=(b'HBF_START_FONT ',),
     patterns=('*.hbf',),
 )
@@ -51,23 +50,25 @@
     properties = _parse_properties(hbf_props, x_props)
     font = Font(glyphs, comment=comments, **properties)
     # label glyphs with code scheme, if known and recognised
     font = font.label()
     return font
 
 @savers.register(linked=load_hbf)
-def save_hbf(fonts, outstream):
+def save_hbf(fonts, outstream, code_scheme:str=''):
     """
     Save font to Hanzi Bitmap Format (HBF) file.
+
+    code_scheme: override HBF_CODE_SCHEME value (default: use encoding)
     """
     if len(fonts) > 1:
         raise FileFormatError('Can only save one font to HBF file.')
     # ensure codepoint values are set
     font = fonts[0]
-    _save_hbf(font, outstream.text, outstream.where)
+    _save_hbf(font, outstream.text, outstream.where, code_scheme)
 
 
 ##############################################################################
 # HBF reader
 
 # https://www.ibiblio.org/pub/packages/ccic/software/info/HBF-1.1/Format.html
 # https://www.ibiblio.org/pub/packages/ccic/software/info/HBF-1.1/BitmapFile.html
@@ -261,15 +262,15 @@
 
 
 def _parse_properties(hbf_props, x_props):
     """Parse metrics and metadata."""
     # parse meaningful metadata
     properties, unparsed, plane = _parse_hbf_properties(hbf_props)
     # the FONT field *may* conform to xlfd but doesn't have to. don't parse it
-    xlfd_props = _parse_xlfd_properties(x_props, xlfd_name='', to_int=hbf_int)
+    xlfd_props = parse_xlfd_properties(x_props, xlfd_name='', to_int=hbf_int)
     for key, value in unparsed.items():
         logging.info(f'Unrecognised HBF property {key}={value}')
         # preserve as property
         properties[key] = value
     for key, value in xlfd_props.items():
         if key in properties and properties[key] != value:
             logging.debug(
@@ -329,67 +330,70 @@
     # keep unparsed hbf props
     return properties, hbf_props, plane
 
 
 ##############################################################################
 # hbf writer
 
-def _save_hbf(font, outstream, container):
+def _save_hbf(font, outstream, container, code_scheme):
     """Write one font to HBF."""
-    bitmap_name = outstream.name + '.bin'
-    hbf_props, bitmaps = _convert_to_hbf(font, bitmap_name)
+    bitmap_name = container.unused_name(outstream.name + '.bin')
+    hbf_props, bitmaps = _convert_to_hbf(font, bitmap_name, code_scheme)
     for name, value in hbf_props:
         logging.info('    %s: %s', name, value)
     with container.open(bitmap_name, 'w') as binfile:
         for bitmap in bitmaps:
             binfile.write(bitmap)
     for name, value in hbf_props:
         outstream.write(f'{name} {value}\n')
 
 
-def _convert_to_hbf(font, bitmap_name):
+def _convert_to_hbf(font, bitmap_name, code_scheme):
     """Convert to HBF properties."""
     # set codepoints
     font = font.label(codepoint_from=font.encoding)
     # get ranges
     cps, cranges, b2ranges, b3ranges = _get_code_ranges(font)
     font = font.subset(cps)
     # check if the remaining glyphs mae for a cell font
     if font.spacing != 'character-cell':
         raise FileFormatError(
             'Only character-cell fonts can be stored in HBF format.'
         )
-    # bring font to normal form
-    font, shift_up = _normalise_metrics(font)
-    #TODO
-    left_bearing = 0
-    #glyphs, properties = _globalise_glyph_metrics(font)
+    # bring font to padded, equalised normal form
+    # then extract common bearings
+    font = font.equalise_horizontal()
+    padding = font.padding
+    font = font.crop(*padding)
     # convert properties
-    xlfd_props = _create_xlfd_properties(font)
+    xlfd_props = create_xlfd_properties(font)
     if 'hbf.font' in font.get_properties():
         fontname = font.get_property('hbf.font')
         xlfd_props.pop('HBF.FONT')
     else:
-        fontname = _create_xlfd_name(xlfd_props)
+        fontname = create_xlfd_name(xlfd_props)
     bbx = (
-        f'{font.cell_size.x} {font.cell_size.y} '
-        f'{left_bearing} {shift_up}'
+        f'{font.raster_size.x} {font.raster_size.y} '
+        f'{padding.left} {padding.bottom}'
+    )
+    font_bbx = (
+        f'{font.raster_size.x+padding.right} {font.raster_size.y+padding.top} '
+        f'{padding.left} {padding.bottom}'
     )
-    #TODO
     code_scheme = font.encoding
     props = [
         ('HBF_START_FONT', '1.1'),
         ('HBF_CODE_SCHEME', code_scheme),
     ] + [
         ('COMMENT', _comment) for _comment in font.get_comment().splitlines()
     ] + [
         ('FONT', fontname),
         ('SIZE', f'{font.point_size} {font.dpi.x} {font.dpi.y}'),
         ('HBF_BITMAP_BOUNDING_BOX', bbx),
-        ('FONTBOUNDINGBOX', bbx),
+        ('FONTBOUNDINGBOX', font_bbx),
     ]
     if xlfd_props:
         props.append(('STARTPROPERTIES', str(len(xlfd_props))))
         props.extend(xlfd_props.items())
         props.append(('ENDPROPERTIES', ''))
     props.append(('CHARS', f'{len(font.glyphs)}'))
     # byte-2 ranges
@@ -457,32 +461,14 @@
     # determine code ranges subject to byte-2, byte-3 ranges already found
     start_crange = range(int(cps[0]), int(cps[-1])+1)
     gen = indexer(None, start_crange, b2ranges, b3ranges)
     cranges = _find_ranges(cps, gen)
     logging.debug('CODE_RANGES %s', cranges)
     return cps, cranges, b2ranges, b3ranges
 
-#
-# def __old_find_ranges(cps):
-#     """Convert a sorted list/tuple to a list of ranges."""
-#     start = int(cps[0])
-#     logging.debug(start)
-#     cur_range = [start, start]
-#     ranges = []
-#     for cp in cps[1:]:
-#         cp = int(cp)
-#         if cp == cur_range[1] + 1:
-#             cur_range[1] = cp
-#         else:
-#             ranges.append(range(cur_range[0], cur_range[1]+1))
-#             cur_range = [cp, cp]
-#     ranges.append(range(cur_range[0], cur_range[1]+1))
-#     logging.debug(ranges)
-#     return ranges
-
 
 def _find_ranges(cps, indexgen=None):
     """Find code range subject to indexer."""
     cur_start = int(cps[0])
     cur_end = cur_start
     if not indexgen:
         indexgen = iter(range(cur_start, int(cps[-1])+1))
```

### Comparing `monobit-0.41.0/monobit/formats/xlfd/pcf.py` & `monobit-0.42.0/monobit/formats/xlfd/pcf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from ...glyph import Glyph
 from ...raster import Raster
 from ...labels import Tag, Codepoint
 from ...binary import align, ceildiv
 
 from .bdf import swidth_to_pixel, pixel_to_swidth
 from .xlfd import (
-    _parse_xlfd_properties, _create_xlfd_properties, _create_xlfd_name,
-    _from_quoted_string
+    parse_xlfd_properties, create_xlfd_properties, create_xlfd_name,
+    from_quoted_string
 )
 
 MAGIC = b'\1fcp'
 
 @loaders.register(
     name='pcf',
     magic=(MAGIC,),
@@ -290,24 +290,26 @@
 
 
 def _read_metrics(instream):
     """Read the Metrics or Ink-Metrics table."""
     format, base = _read_format(instream)
     if format & PCF_COMPRESSED_METRICS:
         compressed_metrics = base.Struct(**_COMPRESSED_METRICS)
-        count = base.int16.read_from(instream)
+        # documented as signed int, but unsigned it makes more sense
+        # also this is used as uint by bdftopcf for e.g. unifont
+        count = base.uint16.read_from(instream)
         metrics = (compressed_metrics * count).read_from(instream)
         # adjust unsigned bytes by 0x80 offset
         metrics = tuple(
             Props(**{_k: _v-0x80 for _k, _v in vars(_m).items()})
             for _m in metrics
         )
     else:
         uncompressed_metrics = base.Struct(**_UNCOMPRESSED_METRICS)
-        count = base.int32.read_from(instream)
+        count = base.uint32.read_from(instream)
         metrics = (uncompressed_metrics * count).read_from(instream)
     return metrics
 
 
 def _read_bitmaps(instream):
     """Read the Bitmaps table."""
     format, base = _read_format(instream)
@@ -475,15 +477,15 @@
     return glyphs
 
 
 def _convert_props(pcf_data):
     """Convert properties for PCF to monobit."""
     xlfd_name = pcf_data.xlfd_props.pop('FONT', '')
     pcf_data.xlfd_props = {_k: str(_v) for _k, _v in pcf_data.xlfd_props.items()}
-    props = _parse_xlfd_properties(pcf_data.xlfd_props, xlfd_name)
+    props = parse_xlfd_properties(pcf_data.xlfd_props, xlfd_name)
     props.update(dict(
         default_char=Codepoint(pcf_data.default_char),
     ))
     # ascent and descent - these are stored in accelerator table rather than XLFD props
     if hasattr(pcf_data, 'bdf_acc_props'):
         props.update(dict(
             ascent=pcf_data.bdf_acc_props.fontAscent,
@@ -566,27 +568,27 @@
             outstream.write(bytes(next.offset - outstream.tell()))
 
 
 
 def _create_properties_table(font, format, base):
     """Create the Properties table."""
     propstrings = bytearray()
-    xlfd_props = _create_xlfd_properties(font)
-    xlfd_props['FONT'] = _create_xlfd_name(xlfd_props)
+    xlfd_props = create_xlfd_properties(font)
+    xlfd_props['FONT'] = create_xlfd_name(xlfd_props)
     props = []
     props_struct = base.Struct(**_PROPS)
     for key, value in xlfd_props.items():
         prop = props_struct(
             name_offset=len(propstrings),
             isStringProp=isinstance(value, str),
         )
         propstrings += key.encode('ascii', 'replace') + b'\0'
         if prop.isStringProp:
             prop.value = len(propstrings)
-            value = _from_quoted_string(value)
+            value = from_quoted_string(value)
             propstrings += value.encode('ascii', 'replace') + b'\0'
         else:
             prop.value = int(value)
         props.append(prop)
     table_bytes = (
         bytes(le.uint32(format))
         + bytes(base.uint32(len(props)))
@@ -725,16 +727,17 @@
             and (maxbounds.character_ascent <= fontAscent)
             and (-minbounds.character_descent <= fontAscent)
             and (maxbounds.character_descent <= fontDescent)
         ),
         # /* true if the ink metrics differ from the metrics somewhere */
         inkMetrics=create_ink_bounds and any(_m != _i for _m, _i in zip(metrics, ink_metrics)),
         # /* 0=>left to right, 1=>right to left */
-        # CHECK is this ever set to rtl even in rtl fonts?
-        drawDirection=1 if font.direction == 'right-to-left' else 0,
+        # however in practice this is set to 0 even on fonts with RTL glyphs
+        # e.g. /usr/share/fonts/arabic24.pcf.gz
+        drawDirection=0,
         padding=0,
         fontAscent=fontAscent,
         fontDescent=fontDescent,
         # where set in X11 code?
         maxOverlap=maxOverlap,
         # minbounds=_UNCOMPRESSED_METRICS,
         # maxbounds=_UNCOMPRESSED_METRICS,
```

### Comparing `monobit-0.41.0/monobit/formats/xlfd/xlfd.py` & `monobit-0.42.0/monobit/formats/xlfd/xlfd.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,23 +456,23 @@
             if _key and _value
         }
     else:
         logging.warning('Could not parse X font name string `%s`', xlfd_str)
         return {}
     return properties
 
-def _from_quoted_string(quoted):
+def from_quoted_string(quoted):
     """Strip quotes"""
     return quoted.strip('"').replace('""', '"')
 
 def _all_ints(*value, to_int=int):
     """Convert all items in tuple to int."""
     return tuple(to_int(_x) for _x in value)
 
-def _parse_xlfd_properties(x_props, xlfd_name, to_int=int):
+def parse_xlfd_properties(x_props, xlfd_name, to_int=int):
     """Parse X metadata."""
     xlfd_name_props = _parse_xlfd_name(xlfd_name)
     # find fields in XLFD FontName that do not match the FontProperties
     conflicting = '\n'.join(
         f'{_k}={repr(_v)} vs {_k}={repr(x_props[_k])}' for _k, _v in xlfd_name_props.items()
         if _k in x_props and not (
             str(_v) == str(x_props[_k])
@@ -482,33 +482,33 @@
     if conflicting:
         logging.info('Conflicts between XLFD FontName and FontProperties: %s', conflicting)
     # continue with the XLFD FontProperties overriding the XLFD FontName fields if given
     x_props = {**xlfd_name_props, **x_props}
     # PIXEL_SIZE = ROUND((RESOLUTION_Y * POINT_SIZE) / 722.7)
     properties = {
         # FULL_NAME is deprecated
-        'name': _from_quoted_string(
+        'name': from_quoted_string(
             x_props.pop('FACE_NAME', x_props.pop('FULL_NAME', ''))
         ),
-        'revision': _from_quoted_string(x_props.pop('FONT_VERSION', '')),
-        'foundry': _from_quoted_string(x_props.pop('FOUNDRY', '')),
-        'copyright': _from_quoted_string(x_props.pop('COPYRIGHT', '')),
-        'notice': _from_quoted_string(x_props.pop('NOTICE', '')),
-        'family': _from_quoted_string(x_props.pop('FAMILY_NAME', '')),
-        'style': _from_quoted_string(x_props.pop('ADD_STYLE_NAME', '')).lower(),
+        'revision': from_quoted_string(x_props.pop('FONT_VERSION', '')),
+        'foundry': from_quoted_string(x_props.pop('FOUNDRY', '')),
+        'copyright': from_quoted_string(x_props.pop('COPYRIGHT', '')),
+        'notice': from_quoted_string(x_props.pop('NOTICE', '')),
+        'family': from_quoted_string(x_props.pop('FAMILY_NAME', '')),
+        'style': from_quoted_string(x_props.pop('ADD_STYLE_NAME', '')).lower(),
         'ascent': x_props.pop('FONT_ASCENT', None),
         'descent': x_props.pop('FONT_DESCENT', None),
         'x_height': x_props.pop('X_HEIGHT', None),
         'cap_height': x_props.pop('CAP_HEIGHT', None),
         'pixel_size': x_props.pop('PIXEL_SIZE', None),
         'slant': _SLANT_MAP.get(
-            _from_quoted_string(x_props.pop('SLANT', '')), None
+            from_quoted_string(x_props.pop('SLANT', '')), None
         ),
         'spacing': _SPACING_MAP.get(
-            _from_quoted_string(x_props.pop('SPACING', '')), None
+            from_quoted_string(x_props.pop('SPACING', '')), None
         ),
         'underline_descent': x_props.pop('UNDERLINE_POSITION', None),
         'underline_thickness': x_props.pop('UNDERLINE_THICKNESS', None),
         'superscript_size': x_props.pop('SUPERSCRIPT_SIZE', None),
         'subscript_size': x_props.pop('SUBSCRIPT_SIZE', None),
         'small_cap_size': x_props.pop('SMALL_CAP_SIZE', None),
         'digit_width': x_props.pop('FIGURE_WIDTH', None),
@@ -527,22 +527,22 @@
     # prefer the more precise relative weight and setwidth measures
     if 'RELATIVE_SETWIDTH' in x_props:
         properties['setwidth'] = _SETWIDTH_MAP.get(
             x_props.pop('RELATIVE_SETWIDTH'), None
         )
         x_props.pop('SETWIDTH_NAME', None)
     if 'setwidth' not in properties or not properties['setwidth']:
-        properties['setwidth'] = _from_quoted_string(
+        properties['setwidth'] = from_quoted_string(
             x_props.pop('SETWIDTH_NAME', '')
         ).lower()
     if 'RELATIVE_WEIGHT' in x_props:
         properties['weight'] = _WEIGHT_MAP.get(x_props.pop('RELATIVE_WEIGHT'), None)
         x_props.pop('WEIGHT_NAME', None)
     if 'weight' not in properties or not properties['weight']:
-        properties['weight'] = _from_quoted_string(x_props.pop('WEIGHT_NAME', '')).lower()
+        properties['weight'] = from_quoted_string(x_props.pop('WEIGHT_NAME', '')).lower()
     # resolution
     if 'RESOLUTION_X' in x_props and 'RESOLUTION_Y' in x_props:
         properties['dpi'] = _all_ints(
             x_props.pop('RESOLUTION_X'), x_props.pop('RESOLUTION_Y')
         )
         x_props.pop('RESOLUTION', None)
     elif 'RESOLUTION' in x_props:
@@ -557,16 +557,16 @@
         )
     if 'SUBSCRIPT_X' in x_props and 'SUBSCRIPT_Y' in x_props:
         properties['subscript_offset'] = _all_ints(
             x_props.pop('SUBSCRIPT_X'), x_props.pop('SUBSCRIPT_Y'),
             to_int=to_int
         )
     # encoding
-    registry = _from_quoted_string(x_props.pop('CHARSET_REGISTRY', '')).lower()
-    encoding = _from_quoted_string(x_props.pop('CHARSET_ENCODING', '')).lower()
+    registry = from_quoted_string(x_props.pop('CHARSET_REGISTRY', '')).lower()
+    encoding = from_quoted_string(x_props.pop('CHARSET_ENCODING', '')).lower()
     if registry and encoding and encoding != '0':
         properties['encoding'] = f'{registry}-{encoding}'
     elif registry:
         properties['encoding'] = registry
     elif encoding != '0':
         properties['encoding'] = encoding
     if properties['encoding'] in _UNDEFINED_ENCODINGS:
@@ -588,49 +588,49 @@
     # keep unparsed but known properties
     for key in _XLFD_UNPARSED:
         try:
             value = x_props.pop(key)
         except KeyError:
             continue
         key = key.lower()
-        value = _from_quoted_string(value)
+        value = from_quoted_string(value)
         if value:
             properties[f'xlfd.{key}'] = value
     # drop empty known properties
     properties = {
         _k: _v for _k, _v in properties.items()
         if _v is not None and _v != ''
     }
     # keep unrecognised properties but in separate namespace
     # to avoid any clashes with yaff properties
     properties.update({
-        f'{CUSTOM_PROP}.{_k}'.lower(): _from_quoted_string(_v)
+        f'{CUSTOM_PROP}.{_k}'.lower(): from_quoted_string(_v)
         for _k, _v in x_props.items()
     })
     return properties
 
 
 
 ##############################################################################
 
-def _create_xlfd_name(xlfd_props):
+def create_xlfd_name(xlfd_props):
     """Construct XLFD name from properties."""
     # if we stored a font name explicitly, keep it
     try:
         return xlfd_props['FONT_NAME']
     except KeyError:
         pass
     xlfd_fields = [xlfd_props.get(prop, '') for prop in _XLFD_NAME_FIELDS]
     return '-'.join(str(_field).strip('"').replace('-', '~') for _field in xlfd_fields)
 
 def _quoted_string(unquoted):
     """Return quoted version of string, if any."""
     return '"{}"'.format(unquoted.replace('"', '""'))
 
-def _create_xlfd_properties(font):
+def create_xlfd_properties(font):
     """Construct XLFD properties."""
     # construct the fields needed for FontName if not defined, leave others optional
     xlfd_props = {
         'FONT_ASCENT': font.get_defined('ascent'),
         'FONT_DESCENT': font.get_defined('descent'),
         'PIXEL_SIZE': font.pixel_size,
         'X_HEIGHT': font.get_defined('x_height'),
```

### Comparing `monobit-0.41.0/monobit/scripts/banner.py` & `monobit-0.42.0/monobit/scripts/banner.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,23 @@
     codecs.register_error(handler_name, _handler)
 
 
 def main():
     # parse command line
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        'text', nargs='*', type=str,
+        'text', nargs='*', type=str, action='extend',
+        help=(
+            'text to be printed. '
+            'multiple text arguments represent consecutive lines. '
+            'if not given, read from standard input'
+        )
+    )
+    parser.add_argument(
+        '--text', nargs='*', type=str, action='extend',
         help=(
             'text to be printed. '
             'multiple text arguments represent consecutive lines. '
             'if not given, read from standard input'
         )
     )
     parser.add_argument(
@@ -125,16 +133,16 @@
         )
     )
     parser.add_argument(
         '--image',  action='store_true',
         help=('output as image')
     )
     parser.add_argument(
-        '--blocks',  action='store_true',
-        help=('output as quadrant blocks')
+        '--blocks',  nargs='?', const='2x2', default='',
+        help=('output as block element characters')
     )
     # font / glyph effects
     parser.add_argument(
         '--bold', action='store_true',
         help='apply algorithmic bold effect'
     )
     parser.add_argument(
@@ -233,15 +241,16 @@
             image = glyph_map.as_image(ink=ink, paper=paper, border=border)
             if args.output:
                 image.save(args.output)
             else:
                 image.show()
         else:
             if args.blocks:
-                text = glyph_map.as_blocks()
+                resolution = tuple(int(_v) for _v in args.blocks.split('x'))
+                text = glyph_map.as_blocks(resolution)
             else:
                 ink = args.ink or '@'
                 paper = args.paper or '.'
                 border = args.border or paper
                 text = glyph_map.as_text(ink=ink, paper=paper, border=border) + '\n'
             if not args.output:
                 sys.stdout.write(text)
```

### Comparing `monobit-0.41.0/monobit/scripts/convert.py` & `monobit-0.42.0/monobit/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/LICENSE` & `monobit-0.42.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monobit-0.41.0/README.md` & `monobit-0.42.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 | Extended Hex          | `pcbasic`  | `.hex`                      | ✔     | ✔     |
 | hexdraw               | `hexdraw`  | `.draw`                     | ✔     | ✔     |
 | Bitmap image [P]      | `image`    | `.png` `.gif` `.bmp`        | ✔     | ✔     |
 | Apple IIgs font       | `iigs`     | `.fon`                      | ✔     | ✔     |
 | Bare codepage         | `kbd`      | `.cp`                       | ✔     | ✔     |
 | REXXCOM Font Mania    | `mania`    | `.com`                      | ✔     |       |
 | LISA font library     | `lisa`     | `.bin`                      | ✔     |       |
-| MacOS font            | `mac`      | `.dfont` `.suit`            | ✔     |       |
+| MacOS font            | `mac`      | `.dfont` `.suit`            | ✔     | ✔     |
 | mkwinfon text format  | `mkwinfon` | `.fd`                       | ✔     |       |
 | X11 Portable Compiled Format |  `pcf` | `.pcf`                   | ✔     | ✔     |
 | Xerox Alto PrePress   | `prepress` | `.ac`                       | ✔     |       |
 | PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
 | Bare NFNT resource    | `nfnt`     | `.f`                        | ✔     | ✔     |
 | Palm OS font (v1/NFNT)| `palm`     | `.pdb`                      | ✔     |       |
 | Optiks PCR Font       | `pcr`      | `.pcr`                      | ✔     |       |
@@ -200,17 +200,17 @@
 Here is a comparison of what you can and cannot store in selected formats supported by `monobit`.
 
 | Format        | Unicode | Unicode sequences | Encoding | MBCS | Multiple fonts | Cell size | Proportional | Kerning | Colour/antialiasing | Glyph representation
 |---------------|---|---|---|---|---|------|---|---|---|--------------
 | `yaff`        | ✔ | ✔ | ✔ | ✔ | ✔ | any  | ✔ | ✔ |   | visual text
 | `sfnt`        | ✔ | ✔ | ✔ | ✔ | ✔ | any  | ✔ | ✔ | ✔ | binary
 | `bmfont`      | ✔ |   | ✔ | ✔ |   | any  | ✔ | ✔ | ✔ | image
+| `mac`         |   |   | ✔ |   |   | any  | ✔ | ✔ | ✔ | binary
 | `bdf`         | ✔ |   | ✔ | ✔ |   | any  | ✔ |   |   | hex
-| `nfnt`        |   |   | ✔ | ✔ | ✔ | any  | ✔ | ✔ | ✔ | binary
-| `win`         |   |   | ✔ | ✔ | ✔ | any  | ✔ |   |   | binary
+| `win`         |   |   | ✔ |   | ✔ | any  | ✔ |   |   | binary
 | `hexdraw`     | ✔ |   |   |   |   | any  | ✔ |   |   | visual text
 | `amiga`       |   |   |   |   | ✔ | any  | ✔ |   | ✔ | binary
 | `gdos`        |   |   |   |   |   | any  | ✔ |   |   | binary
 | `fzx`         |   |   |   |   |   | any  | ✔ |   |   | binary
 | `figlet`      | ✔ |   |   |   |   | any  | ✔ |   | ✔ | visual text
 | `vfont`       |   |   |   |   |   | any  | ✔ |   |   | binary
 | `pcbasic`     | ✔ | ✔ |   |   |   | 8xN  | multi-cell |   |   | hex
@@ -294,16 +294,17 @@
 `monobit` and the `yaff` specification are copyright 2019--2023 Rob Hagemans and
 released under the [MIT licence](https://opensource.org/licenses/MIT).
 
 `monobit` contains code from:  
 - [`mkwinfont`](https://www.chiark.greenend.org.uk/~sgtatham/fonts/) copyright 2001 Simon Tatham. All rights reserved.  
 - [`dewinfont`](https://www.chiark.greenend.org.uk/~sgtatham/fonts/) copyright 2001,2017 Simon Tatham. All rights reserved.  
 - [OS/2 GPI Font Tools](https://github.com/altsan/os2-gpi-font-tools) (C) 2012 Alexander Taylor  
+- [FONDU](https://sourceforge.net/projects/fondu/) copyright (C) 2000,2001,2002,2003 by George Williams
 
-Please refer to the notices in the `windows` and `os2` subpackages for licences and more information.
+Please refer to the notices in the `windows` and `os2` subpackages and `mac/fond.py` module for licences and more information.
 
 The font files in `tests/fonts` are subject to their own
 licences, some of which are more restrictive. These are files used for testing
 and development and are not included in the packaged distribution. See `tests/fonts/README.md` and notices included with individual files.
 
 
 Acknowledgements
```

### Comparing `monobit-0.41.0/pyproject.toml` & `monobit-0.42.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "monobit"
-version = "0.41.0"
+version = "0.42.0"
 authors = [
     { name = "Rob Hagemans", email = "rob.hagemans@hotmail.com" },
 ]
 description = "Tools for working with monochrome bitmap fonts."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `monobit-0.41.0/PKG-INFO` & `monobit-0.42.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monobit
-Version: 0.41.0
+Version: 0.42.0
 Summary: Tools for working with monochrome bitmap fonts.
 Project-URL: Homepage, https://github.com/robhagemans/monobit
 Author-email: Rob Hagemans <rob.hagemans@hotmail.com>
 License: MIT License
         
         Copyright (c) 2019--2023 Rob Hagemans
         
@@ -161,15 +161,15 @@
 | Extended Hex          | `pcbasic`  | `.hex`                      | ✔     | ✔     |
 | hexdraw               | `hexdraw`  | `.draw`                     | ✔     | ✔     |
 | Bitmap image [P]      | `image`    | `.png` `.gif` `.bmp`        | ✔     | ✔     |
 | Apple IIgs font       | `iigs`     | `.fon`                      | ✔     | ✔     |
 | Bare codepage         | `kbd`      | `.cp`                       | ✔     | ✔     |
 | REXXCOM Font Mania    | `mania`    | `.com`                      | ✔     |       |
 | LISA font library     | `lisa`     | `.bin`                      | ✔     |       |
-| MacOS font            | `mac`      | `.dfont` `.suit`            | ✔     |       |
+| MacOS font            | `mac`      | `.dfont` `.suit`            | ✔     | ✔     |
 | mkwinfon text format  | `mkwinfon` | `.fd`                       | ✔     |       |
 | X11 Portable Compiled Format |  `pcf` | `.pcf`                   | ✔     | ✔     |
 | Xerox Alto PrePress   | `prepress` | `.ac`                       | ✔     |       |
 | PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
 | Bare NFNT resource    | `nfnt`     | `.f`                        | ✔     | ✔     |
 | Palm OS font (v1/NFNT)| `palm`     | `.pdb`                      | ✔     |       |
 | Optiks PCR Font       | `pcr`      | `.pcr`                      | ✔     |       |
@@ -242,17 +242,17 @@
 Here is a comparison of what you can and cannot store in selected formats supported by `monobit`.
 
 | Format        | Unicode | Unicode sequences | Encoding | MBCS | Multiple fonts | Cell size | Proportional | Kerning | Colour/antialiasing | Glyph representation
 |---------------|---|---|---|---|---|------|---|---|---|--------------
 | `yaff`        | ✔ | ✔ | ✔ | ✔ | ✔ | any  | ✔ | ✔ |   | visual text
 | `sfnt`        | ✔ | ✔ | ✔ | ✔ | ✔ | any  | ✔ | ✔ | ✔ | binary
 | `bmfont`      | ✔ |   | ✔ | ✔ |   | any  | ✔ | ✔ | ✔ | image
+| `mac`         |   |   | ✔ |   |   | any  | ✔ | ✔ | ✔ | binary
 | `bdf`         | ✔ |   | ✔ | ✔ |   | any  | ✔ |   |   | hex
-| `nfnt`        |   |   | ✔ | ✔ | ✔ | any  | ✔ | ✔ | ✔ | binary
-| `win`         |   |   | ✔ | ✔ | ✔ | any  | ✔ |   |   | binary
+| `win`         |   |   | ✔ |   | ✔ | any  | ✔ |   |   | binary
 | `hexdraw`     | ✔ |   |   |   |   | any  | ✔ |   |   | visual text
 | `amiga`       |   |   |   |   | ✔ | any  | ✔ |   | ✔ | binary
 | `gdos`        |   |   |   |   |   | any  | ✔ |   |   | binary
 | `fzx`         |   |   |   |   |   | any  | ✔ |   |   | binary
 | `figlet`      | ✔ |   |   |   |   | any  | ✔ |   | ✔ | visual text
 | `vfont`       |   |   |   |   |   | any  | ✔ |   |   | binary
 | `pcbasic`     | ✔ | ✔ |   |   |   | 8xN  | multi-cell |   |   | hex
@@ -336,16 +336,17 @@
 `monobit` and the `yaff` specification are copyright 2019--2023 Rob Hagemans and
 released under the [MIT licence](https://opensource.org/licenses/MIT).
 
 `monobit` contains code from:  
 - [`mkwinfont`](https://www.chiark.greenend.org.uk/~sgtatham/fonts/) copyright 2001 Simon Tatham. All rights reserved.  
 - [`dewinfont`](https://www.chiark.greenend.org.uk/~sgtatham/fonts/) copyright 2001,2017 Simon Tatham. All rights reserved.  
 - [OS/2 GPI Font Tools](https://github.com/altsan/os2-gpi-font-tools) (C) 2012 Alexander Taylor  
+- [FONDU](https://sourceforge.net/projects/fondu/) copyright (C) 2000,2001,2002,2003 by George Williams
 
-Please refer to the notices in the `windows` and `os2` subpackages for licences and more information.
+Please refer to the notices in the `windows` and `os2` subpackages and `mac/fond.py` module for licences and more information.
 
 The font files in `tests/fonts` are subject to their own
 licences, some of which are more restrictive. These are files used for testing
 and development and are not included in the packaged distribution. See `tests/fonts/README.md` and notices included with individual files.
 
 
 Acknowledgements
```

