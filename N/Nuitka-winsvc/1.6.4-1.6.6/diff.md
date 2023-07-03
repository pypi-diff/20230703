# Comparing `tmp/Nuitka-winsvc-1.6.4.tar.gz` & `tmp/Nuitka-winsvc-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nuitka-winsvc-1.6.4.tar", last modified: Sun Jun 25 06:03:00 2023, max compression
+gzip compressed data, was "Nuitka-winsvc-1.6.6.tar", last modified: Mon Jul  3 06:36:42 2023, max compression
```

## Comparing `Nuitka-winsvc-1.6.4.tar` & `Nuitka-winsvc-1.6.6.tar`

### file list

```diff
@@ -1,1798 +1,1798 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 06:03:00.103581 Nuitka-winsvc-1.6.4/
--rw-rw-rw-   0        0        0   825587 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/Changelog.rst
--rw-rw-rw-   0        0        0   152515 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/Developer_Manual.rst
--rw-rw-rw-   0        0        0    11348 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1733 2023-06-25 05:59:12.000000 Nuitka-winsvc-1.6.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.282402 Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/
--rw-rw-rw-   0        0        0     4626 2023-06-25 06:02:51.000000 Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    76624 2023-06-25 06:02:51.000000 Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 06:02:51.000000 Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      308 2023-06-25 06:02:51.000000 Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-28 09:21:19.000000 Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-06-25 06:02:51.000000 Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-25 06:02:51.000000 Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4626 2023-06-25 06:03:00.102582 Nuitka-winsvc-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     2651 2023-06-25 05:59:11.000000 Nuitka-winsvc-1.6.4/README.md
--rw-rw-rw-   0        0        0    75940 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.379814 Nuitka-winsvc-1.6.4/bin/
--rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/bin/autoformat-nuitka-source
--rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/bin/check-nuitka-with-pylint
--rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/bin/compare_with_cpython
--rw-rw-rw-   0        0        0     3079 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/bin/compare_with_xml
--rw-rw-rw-   0        0        0     1163 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/bin/measure-construct-performance
--rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/bin/nuitka
--rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/bin/nuitka-run
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.002486 Nuitka-winsvc-1.6.4/doc/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.433981 Nuitka-winsvc-1.6.4/doc/Logo/
--rw-rw-rw-   0        0        0     7321 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/doc/Logo/Nuitka-Logo-Horizontal.svg
--rw-rw-rw-   0        0        0     7401 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-rw-rw-   0        0        0    17917 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/doc/Logo/Nuitka-Logo-Vertical.svg
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.459169 Nuitka-winsvc-1.6.4/doc/images/
--rw-rw-rw-   0        0        0     7585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/doc/images/Nuitka-Logo-Horizontal.png
--rw-rw-rw-   0        0        0     4452 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/doc/images/Nuitka-Logo-Symbol.png
--rw-rw-rw-   0        0        0     9828 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/doc/images/Nuitka-Logo-Vertical.png
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.460164 Nuitka-winsvc-1.6.4/lib/
--rw-rw-rw-   0        0        0     4250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/lib/hints.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.487821 Nuitka-winsvc-1.6.4/misc/
--rwxrwxrwx   0        0        0      901 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/misc/nuitka-run.bat
--rwxrwxrwx   0        0        0     1038 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/misc/nuitka.bat
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.522806 Nuitka-winsvc-1.6.4/nuitka/
--rw-rw-rw-   0        0        0     7331 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/Builtins.py
--rw-rw-rw-   0        0        0     5437 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/BytecodeCaching.py
--rw-rw-rw-   0        0        0     3440 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/Bytecodes.py
--rw-rw-rw-   0        0        0     1884 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/CacheCleanup.py
--rw-rw-rw-   0        0        0    11148 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/Constants.py
--rw-rw-rw-   0        0        0     2447 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/Errors.py
--rw-rw-rw-   0        0        0    37317 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.4/nuitka/MainControl.py
--rw-rw-rw-   0        0        0     8064 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/ModuleRegistry.py
--rw-rw-rw-   0        0        0    57087 2023-06-25 05:59:12.000000 Nuitka-winsvc-1.6.4/nuitka/OptionParsing.py
--rw-rw-rw-   0        0        0    66046 2023-06-25 05:59:12.000000 Nuitka-winsvc-1.6.4/nuitka/Options.py
--rw-rw-rw-   0        0        0     5022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/OutputDirectories.py
--rw-rw-rw-   0        0        0    14550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/PostProcessing.py
--rw-rw-rw-   0        0        0     5770 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/Progress.py
--rw-rw-rw-   0        0        0     7472 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/PythonFlavors.py
--rw-rw-rw-   0        0        0     4061 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/PythonOperators.py
--rw-rw-rw-   0        0        0    12179 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/PythonVersions.py
--rw-rw-rw-   0        0        0     8514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/Serialization.py
--rw-rw-rw-   0        0        0     4670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/SourceCodeReferences.py
--rw-rw-rw-   0        0        0    11235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/Tracing.py
--rw-rw-rw-   0        0        0     3395 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/TreeXML.py
--rw-rw-rw-   0        0        0    15235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/Variables.py
--rw-rw-rw-   0        0        0     2055 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.4/nuitka/Version.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/__init__.py
--rw-rw-rw-   0        0        0     5615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/__main__.py
--rw-rw-rw-   0        0        0     5295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/__past__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.556807 Nuitka-winsvc-1.6.4/nuitka/build/
--rw-rw-rw-   0        0        0    33528 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/Backend.scons
--rw-rw-rw-   0        0        0     8314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/CCompilerVersion.scons
--rw-rw-rw-   0        0        0     2433 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/DataComposerInterface.py
--rw-rw-rw-   0        0        0    18807 2023-06-25 05:59:12.000000 Nuitka-winsvc-1.6.4/nuitka/build/Onefile.scons
--rw-rw-rw-   0        0        0    15635 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/SconsCaching.py
--rw-rw-rw-   0        0        0    30984 2023-06-25 05:59:12.000000 Nuitka-winsvc-1.6.4/nuitka/build/SconsCompilerSettings.py
--rw-rw-rw-   0        0        0     5527 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/SconsHacks.py
--rw-rw-rw-   0        0        0    15532 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/SconsInterface.py
--rw-rw-rw-   0        0        0     2361 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/SconsProgress.py
--rw-rw-rw-   0        0        0    11964 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/build/SconsSpawn.py
--rw-rw-rw-   0        0        0    24338 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/build/SconsUtils.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.005486 Nuitka-winsvc-1.6.4/nuitka/build/include/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.617824 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/
--rw-rw-rw-   0        0        0     7972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/allocator.h
--rw-rw-rw-   0        0        0     3423 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/builtins.h
--rw-rw-rw-   0        0        0     4604 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/calling.h
--rw-rw-rw-   0        0        0     1977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/checkers.h
--rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/checksum_tools.h
--rw-rw-rw-   0        0        0     9571 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-rw-rw-   0        0        0     2002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_cell.h
--rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-rw-rw-   0        0        0    16949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_frame.h
--rw-rw-rw-   0        0        0     5972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_function.h
--rw-rw-rw-   0        0        0     9136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_generator.h
--rw-rw-rw-   0        0        0     1838 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_method.h
--rw-rw-rw-   0        0        0     7408 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/constants.h
--rw-rw-rw-   0        0        0     1293 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/constants_blob.h
--rw-rw-rw-   0        0        0    34083 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/exceptions.h
--rw-rw-rw-   0        0        0     3221 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/filesystem_paths.h
--rw-rw-rw-   0        0        0     6253 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/freelists.h
--rw-rw-rw-   0        0        0    86326 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/hedley.h
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.722823 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/
--rw-rw-rw-   0        0        0     3275 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/attributes.h
--rw-rw-rw-   0        0        0     2663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/boolean.h
--rw-rw-rw-   0        0        0     1181 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/bytes.h
--rw-rw-rw-   0        0        0     9335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-rw-rw-   0        0        0    10615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-rw-rw-   0        0        0    13139 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-rw-rw-   0        0        0     1743 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/complex.h
--rw-rw-rw-   0        0        0    13109 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-rw-rw-   0        0        0     1206 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/floats.h
--rw-rw-rw-   0        0        0     3674 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/import_hard.h
--rw-rw-rw-   0        0        0     1798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/indexes.h
--rw-rw-rw-   0        0        0     2941 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/ints.h
--rw-rw-rw-   0        0        0     9992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/iterators.h
--rw-rw-rw-   0        0        0     3411 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/lists.h
--rw-rw-rw-   0        0        0     1633 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-rw-rw-   0        0        0     1328 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/mappings.h
--rw-rw-rw-   0        0        0     4573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations.h
--rw-rw-rw-   0        0        0    12685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-rw-rw-   0        0        0     5641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-rw-rw-   0        0        0     5422 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-rw-rw-   0        0        0     5460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-rw-rw-   0        0        0     2799 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-rw-rw-   0        0        0    15778 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-rw-rw-   0        0        0    13210 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-rw-rw-   0        0        0     5791 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-rw-rw-   0        0        0     4714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-rw-rw-   0        0        0     5824 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-rw-rw-   0        0        0     5438 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-rw-rw-   0        0        0    15100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-rw-rw-   0        0        0     8670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-rw-rw-   0        0        0     3753 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-rw-rw-   0        0        0     4846 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-rw-rw-   0        0        0    10626 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-rw-rw-   0        0        0     9201 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-rw-rw-   0        0        0     5147 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-rw-rw-   0        0        0     4349 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-rw-rw-   0        0        0     4975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-rw-rw-   0        0        0     4826 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-rw-rw-   0        0        0     3297 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/raising.h
--rw-rw-rw-   0        0        0     2178 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-rw-rw-   0        0        0     1146 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-rw-rw-   0        0        0     1112 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/sequences.h
--rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/sets.h
--rw-rw-rw-   0        0        0     8419 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/slices.h
--rw-rw-rw-   0        0        0     1242 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/strings.h
--rw-rw-rw-   0        0        0    17575 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/subscripts.h
--rw-rw-rw-   0        0        0     5720 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/tuples.h
--rw-rw-rw-   0        0        0    14412 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helpers.h
--rw-rw-rw-   0        0        0     5375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/importing.h
--rw-rw-rw-   0        0        0    12979 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/incbin.h
--rw-rw-rw-   0        0        0    14427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/prelude.h
--rw-rw-rw-   0        0        0     2870 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/printing.h
--rw-rw-rw-   0        0        0     1761 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/python_pgo.h
--rw-rw-rw-   0        0        0     2119 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/safe_string_ops.h
--rw-rw-rw-   0        0        0     3840 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/threading.h
--rw-rw-rw-   0        0        0     3144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/tracing.h
--rw-rw-rw-   0        0        0     2936 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/unfreezing.h
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.051684 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.739811 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/appdirs/
--rw-rw-rw-   0        0        0     1097 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/appdirs/LICENSE.txt
--rw-rw-rw-   0        0        0    24824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/appdirs/appdirs.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.752818 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/atomicwrites/
--rw-rw-rw-   0        0        0     1069 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.753809 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/bin/
--rw-rw-rw-   0        0        0     1331 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/bin/scons.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.011486 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/clcache/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.767815 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/clcache/clcache/
--rw-rw-rw-   0        0        0     1585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-rw-rw-   0        0        0       93 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-rw-rw-   0        0        0    65424 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.777835 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/
--rw-rw-rw-   0        0        0     1491 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.789812 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/
--rw-rw-rw-   0        0        0      243 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-rw-rw-   0        0        0    10517 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.806810 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/
--rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.820813 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/glob2/
--rw-rw-rw-   0        0        0       82 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-rw-rw-   0        0        0     6859 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-rw-rw-   0        0        0     4463 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-rw-rw-   0        0        0     8304 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/glob2/impl.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.839810 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/
--rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/LICENSE.rst
--rw-rw-rw-   0        0        0       85 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.884812 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/
--rw-rw-rw-   0        0        0     2423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17473 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.900818 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/
--rw-rw-rw-   0        0        0     1466 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
--rw-rw-rw-   0        0        0       84 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.937813 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.034734 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.018485 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.973825 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-rw-rw-   0        0        0    47844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
--rw-rw-rw-   0        0        0    33996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-rw-rw-   0        0        0     8083 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     6938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    17622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7358 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    21540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16000 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.981815 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-rw-rw-   0        0        0     4197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   121420 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     4164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    49503 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.988814 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-rw-rw-   0        0        0     1965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-rw-rw-   0        0        0     2736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-rw-rw-   0        0        0     2614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-rw-rw-   0        0        0     8467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.004813 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-rw-rw-   0        0        0     9314 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3131 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     1989 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1718 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1605 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     2170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4179 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1882 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0    14948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    39700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    12950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.013815 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3233 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2011 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    14663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.020815 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-rw-rw-   0        0        0    14029 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    52665 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    40719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    24133 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-rw-rw-   0        0        0    34903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    40510 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.139814 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2166 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-rw-rw-   0        0        0     2859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-rw-rw-   0        0        0    18084 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.150817 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0     9248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    14869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    19499 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    20832 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-rw-rw-   0        0        0     5149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-rw-rw-   0        0        0     2657 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-rw-rw-   0        0        0    31283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2267 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-rw-rw-   0        0        0     2720 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     2796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2147 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2936 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2935 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     2777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-rw-rw-   0        0        0      142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.151815 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-rw-rw-   0        0        0     1844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     4782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-rw-rw-   0        0        0     2025 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-rw-rw-   0        0        0     2256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-rw-rw-   0        0        0     2460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2077 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    18600 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     3328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-rw-rw-   0        0        0     8394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     3953 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2309 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2945 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     6919 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4381 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2168 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    13881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1804 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    11380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    72761 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6841 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     4695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1927 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     2349 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     5992 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13016 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3415 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    48938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.164816 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3007 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11034 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.178820 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-rw-rw-   0        0        0     8120 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     3596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-rw-rw-   0        0        0     1818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-rw-rw-   0        0        0     1742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     2465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-rw-rw-   0        0        0     1776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-rw-rw-   0        0        0    19253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-rw-rw-   0        0        0    44500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-rw-rw-   0        0        0    19664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     7509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.027487 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.219818 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-rw-rw-   0        0        0    53545 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
--rw-rw-rw-   0        0        0    34985 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-rw-rw-   0        0        0    13596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    28403 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    20988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    22350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16068 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9565 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.225821 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-rw-rw-   0        0        0     5239 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   135413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     5758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8354 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.251817 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-rw-rw-   0        0        0    11500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2227 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1767 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1654 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4476 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     4003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    16962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41186 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    13880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.259822 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3812 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.272835 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-rw-rw-   0        0        0    13779 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53260 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    39394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14489 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    35863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    42204 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.420975 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    18207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.433978 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2152 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    10674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    33537 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    21762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    50660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     8618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2226 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2978 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3389 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.435976 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      313 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3631 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3444 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     8494 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.436976 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3686 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2580 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1645 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2189 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1944 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    15791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    26195 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0    13924 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     4041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2351 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2987 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     7808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4956 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     5235 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1847 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    82939 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4904 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1868 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     5335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6756 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3773 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3201 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    53803 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.449975 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4459 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1647 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.452976 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-rw-rw-   0        0        0     6869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0    19816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     9002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.034734 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.502976 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-rw-rw-   0        0        0    56578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-rw-rw-   0        0        0    35213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
--rw-rw-rw-   0        0        0    11061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27408 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7884 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-rw-rw-   0        0        0    21423 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-rw-rw-   0        0        0    97269 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-rw-rw-   0        0        0     3979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
--rw-rw-rw-   0        0        0     7515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-rw-rw-   0        0        0    21937 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-rw-rw-   0        0        0    16583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.517977 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-rw-rw-   0        0        0     5126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   136271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     6167 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63768 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.538979 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-rw-rw-   0        0        0    12836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4356 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    14831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41983 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-rw-rw-   0        0        0    14673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.549980 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-rw-rw-   0        0        0     7394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     4357 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3546 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     1972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.555978 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-rw-rw-   0        0        0    13597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    42760 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26676 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    36753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-rw-rw-   0        0        0    41191 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.680980 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-rw-rw-   0        0        0     2122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    15570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.697981 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2014 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    13182 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2734 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15027 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    38783 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    22570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4368 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    32724 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     7993 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2141 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     1661 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2893 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-rw-rw-   0        0        0     2889 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.699981 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      343 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3259 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     7461 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-rw-rw-   0        0        0     3379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2377 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2526 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2677 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2206 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2096 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     1954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     1995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    19180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     2588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.703990 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-rw-rw-   0        0        0     4649 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-rw-rw-   0        0        0     7652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-rw-rw-   0        0        0     6064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-rw-rw-   0        0        0     3931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2266 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2900 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     8622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    84784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3576 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2479 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1780 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     1999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1569 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2419 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2429 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6412 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    12548 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     4076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    71693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.708980 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-rw-rw-   0        0        0     6632 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-rw-rw-   0        0        0    15278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.718979 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-rw-rw-   0        0        0     3134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3896 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4672 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    12708 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-rw-rw-   0        0        0      353 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.722980 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-rw-rw-   0        0        0     4307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     3395 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-rw-rw-   0        0        0    21614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-rw-rw-   0        0        0     9295 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-rw-rw-   0        0        0     2032 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.749987 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/
--rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.755980 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-rw-rw-   0        0        0    10126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-rw-rw-   0        0        0      558 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-rw-rw-   0        0        0     4690 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.045062 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/pkg_resources/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.762986 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-rw-rw-   0        0        0   107452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      538 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.046062 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.919983 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/
--rw-rw-rw-   0        0        0     1591 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-rw-rw-   0        0        0      287 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
--rw-rw-rw-   0        0        0      307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-rw-rw-   0        0        0      596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-rw-rw-   0        0        0     1106 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-rw-rw-   0        0        0     1376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-rw-rw-   0        0        0     5943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/gui.py
--rw-rw-rw-   0        0        0    10790 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-rw-rw-   0        0        0    57572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-rw-rw-   0        0        0     6948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/tk.py
--rw-rw-rw-   0        0        0     9533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-rw-rw-   0        0        0      333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/version.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.935984 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:53.967006 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/
--rw-rw-rw-   0        0        0    13170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-rw-rw-   0        0        0     4883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-rw-rw-   0        0        0    28639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-rw-rw-   0        0        0     3851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2837 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/dumper.py
--rw-rw-rw-   0        0        0    43006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-rw-rw-   0        0        0     2061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-rw-rw-   0        0        0    14184 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-rw-rw-   0        0        0     8999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-rw-rw-   0        0        0    51277 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.002990 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.033990 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/
--rw-rw-rw-   0        0        0     9776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-rw-rw-   0        0        0     4921 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-rw-rw-   0        0        0    25145 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-rw-rw-   0        0        0     3290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
--rw-rw-rw-   0        0        0    43298 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-rw-rw-   0        0        0     2559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-rw-rw-   0        0        0     1132 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-rw-rw-   0        0        0    25542 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-rw-rw-   0        0        0     6746 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-rw-rw-   0        0        0    17711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-rw-rw-   0        0        0     9122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-rw-rw-   0        0        0    52446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-rw-rw-   0        0        0     4171 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.053990 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.088984 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/
--rw-rw-rw-   0        0        0     9607 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-rw-rw-   0        0        0    25554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-rw-rw-   0        0        0     3294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
--rw-rw-rw-   0        0        0    42954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-rw-rw-   0        0        0     1138 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-rw-rw-   0        0        0     6854 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-rw-rw-   0        0        0    14097 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-rw-rw-   0        0        0     8970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-rw-rw-   0        0        0    51695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.097988 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/
--rw-rw-rw-   0        0        0     1530 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.129987 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/
--rw-rw-rw-   0        0        0    18198 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-rw-rw-   0        0        0    10157 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/compiler.h
--rw-rw-rw-   0        0        0     4455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/debug.h
--rw-rw-rw-   0        0        0    13662 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-rw-rw-   0        0        0     3009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-rw-rw-   0        0        0     2441 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-rw-rw-   0        0        0    34422 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/fse.h
--rw-rw-rw-   0        0        0    14748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-rw-rw-   0        0        0    20216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/huf.h
--rw-rw-rw-   0        0        0    13930 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/mem.h
--rw-rw-rw-   0        0        0    26976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-rw-rw-   0        0        0    11706 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-rw-rw-   0        0        0     2497 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-rw-rw-   0        0        0     3828 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-rw-rw-   0        0        0    15880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/zstd_internal.h
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.140985 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/
--rw-rw-rw-   0        0        0    54982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-rw-rw-   0        0        0     9164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-rw-rw-   0        0        0     1321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-rw-rw-   0        0        0    80283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-rw-rw-   0        0        0    66784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-rw-rw-   0        0        0     2253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-rw-rw-   0        0        0     7906 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-rw-rw-   0        0        0   138334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/zstd.h
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.308418 Nuitka-winsvc-1.6.4/nuitka/build/static_src/
--rw-rw-rw-   0        0        0    82114 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-rw-rw-   0        0        0     8250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledCellType.c
--rw-rw-rw-   0        0        0    62733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-rw-rw-   0        0        0    70973 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledCoroutineType.c
--rw-rw-rw-   0        0        0    35861 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledFrameType.c
--rw-rw-rw-   0        0        0   100376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledFunctionType.c
--rw-rw-rw-   0        0        0    60649 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledGeneratorType.c
--rw-rw-rw-   0        0        0    48526 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-rw-rw-   0        0        0    21638 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledMethodType.c
--rw-rw-rw-   0        0        0    18993 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersAllocator.c
--rw-rw-rw-   0        0        0    32849 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersAttributes.c
--rw-rw-rw-   0        0        0    21783 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersBuiltin.c
--rw-rw-rw-   0        0        0   107641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-rw-rw-   0        0        0     3033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersBytes.c
--rw-rw-rw-   0        0        0    13057 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersCalling.c
--rw-rw-rw-   0        0        0   470655 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-rw-rw-   0        0        0     1617 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersChecksumTools.c
--rw-rw-rw-   0        0        0     2991 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersClasses.c
--rw-rw-rw-   0        0        0   317872 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonEq.c
--rw-rw-rw-   0        0        0     4673 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-rw-rw-   0        0        0   313003 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonGe.c
--rw-rw-rw-   0        0        0   312414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonGt.c
--rw-rw-rw-   0        0        0   316217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonLe.c
--rw-rw-rw-   0        0        0   315628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonLt.c
--rw-rw-rw-   0        0        0   314618 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonNe.c
--rw-rw-rw-   0        0        0    36068 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-rw-rw-   0        0        0    19313 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersDeepcopy.c
--rw-rw-rw-   0        0        0    38364 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersDictionaries.c
--rw-rw-rw-   0        0        0    24295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-rw-rw-   0        0        0     7035 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersExceptions.c
--rw-rw-rw-   0        0        0     6668 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersFiles.c
--rw-rw-rw-   0        0        0    11199 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-rw-rw-   0        0        0     2426 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersFloats.c
--rw-rw-rw-   0        0        0     1774 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersHeapStorage.c
--rw-rw-rw-   0        0        0    14585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersImport.c
--rw-rw-rw-   0        0        0    13589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersImportHard.c
--rw-rw-rw-   0        0        0    18433 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersLists.c
--rw-rw-rw-   0        0        0    13915 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersListsGenerated.c
--rw-rw-rw-   0        0        0     1640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersMappings.c
--rw-rw-rw-   0        0        0     3513 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersMatching.c
--rw-rw-rw-   0        0        0   181243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-rw-rw-   0        0        0    16700 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-rw-rw-   0        0        0    77782 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
--rw-rw-rw-   0        0        0    67487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-rw-rw-   0        0        0    68748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-rw-rw-   0        0        0     6274 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-rw-rw-   0        0        0    83405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-rw-rw-   0        0        0    13776 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-rw-rw-   0        0        0   183202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-rw-rw-   0        0        0   188514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-rw-rw-   0        0        0     3404 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-rw-rw-   0        0        0    66453 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-rw-rw-   0        0        0    78891 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-rw-rw-   0        0        0     1023 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-rw-rw-   0        0        0    77305 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-rw-rw-   0        0        0    70465 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-rw-rw-   0        0        0    68005 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-rw-rw-   0        0        0   149580 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-rw-rw-   0        0        0     4071 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-rw-rw-   0        0        0    53122 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-rw-rw-   0        0        0    76512 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-rw-rw-   0        0        0    47568 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-rw-rw-   0        0        0    17742 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-rw-rw-   0        0        0   136100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-rw-rw-   0        0        0   142211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-rw-rw-   0        0        0    74142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-rw-rw-   0        0        0    82669 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-rw-rw-   0        0        0    45052 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-rw-rw-   0        0        0    82842 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-rw-rw-   0        0        0    76343 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-rw-rw-   0        0        0     3219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersProfiling.c
--rw-rw-rw-   0        0        0     3805 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersPythonPgo.c
--rw-rw-rw-   0        0        0    15369 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersRaising.c
--rw-rw-rw-   0        0        0    11926 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersSafeStrings.c
--rw-rw-rw-   0        0        0     3730 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersSequences.c
--rw-rw-rw-   0        0        0     1946 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersSlices.c
--rw-rw-rw-   0        0        0    26642 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersStrings.c
--rw-rw-rw-   0        0        0     4037 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersTuples.c
--rw-rw-rw-   0        0        0     5578 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersTypes.c
--rw-rw-rw-   0        0        0    11986 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/InspectPatcher.c
--rw-rw-rw-   0        0        0    41670 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/MainProgram.c
--rw-rw-rw-   0        0        0    58634 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-rw-rw-   0        0        0     4537 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-rw-rw-   0        0        0     6427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-rw-rw-   0        0        0    17065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-rw-rw-   0        0        0    36617 2023-06-25 05:59:12.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/OnefileBootstrap.c
--rw-rw-rw-   0        0        0     7984 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/build/static_src/OnefileSplashScreen.cpp
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.401235 Nuitka-winsvc-1.6.4/nuitka/code_generation/
--rw-rw-rw-   0        0        0     6414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/AsyncgenCodes.py
--rw-rw-rw-   0        0        0    10153 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/AttributeCodes.py
--rw-rw-rw-   0        0        0    21864 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-rw-rw-   0        0        0     2339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/BranchCodes.py
--rw-rw-rw-   0        0        0    16009 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/BuiltinCodes.py
--rw-rw-rw-   0        0        0    35905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/CallCodes.py
--rw-rw-rw-   0        0        0     4896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ClassCodes.py
--rw-rw-rw-   0        0        0    51116 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/CodeGeneration.py
--rw-rw-rw-   0        0        0     2375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/CodeHelperSelection.py
--rw-rw-rw-   0        0        0    14392 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/CodeHelpers.py
--rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/CodeObjectCodes.py
--rw-rw-rw-   0        0        0    17570 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ComparisonCodes.py
--rw-rw-rw-   0        0        0     4446 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-rw-rw-   0        0        0     7335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ConditionalCodes.py
--rw-rw-rw-   0        0        0     6539 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ConstantCodes.py
--rw-rw-rw-   0        0        0    31186 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/Contexts.py
--rw-rw-rw-   0        0        0     8484 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/CoroutineCodes.py
--rw-rw-rw-   0        0        0     1574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/CtypesCodes.py
--rw-rw-rw-   0        0        0    28478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/DictCodes.py
--rw-rw-rw-   0        0        0     2125 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/Emission.py
--rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ErrorCodes.py
--rw-rw-rw-   0        0        0    12304 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/EvalCodes.py
--rw-rw-rw-   0        0        0     8975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ExceptionCodes.py
--rw-rw-rw-   0        0        0     7350 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-rw-rw-   0        0        0     2093 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ExpressionCodes.py
--rw-rw-rw-   0        0        0    17725 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/FrameCodes.py
--rw-rw-rw-   0        0        0    27345 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/FunctionCodes.py
--rw-rw-rw-   0        0        0     7690 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/GeneratorCodes.py
--rw-rw-rw-   0        0        0     5721 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/GlobalConstants.py
--rw-rw-rw-   0        0        0     6911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-rw-rw-   0        0        0     1794 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/IdCodes.py
--rw-rw-rw-   0        0        0    13318 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ImportCodes.py
--rw-rw-rw-   0        0        0     1396 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/Indentation.py
--rw-rw-rw-   0        0        0     1506 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/IndexCodes.py
--rw-rw-rw-   0        0        0     1033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/InjectCCodes.py
--rw-rw-rw-   0        0        0     3432 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/IntegerCodes.py
--rw-rw-rw-   0        0        0    12010 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/IteratorCodes.py
--rw-rw-rw-   0        0        0     2022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/LabelCodes.py
--rw-rw-rw-   0        0        0     2612 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/LineNumberCodes.py
--rw-rw-rw-   0        0        0    15906 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ListCodes.py
--rw-rw-rw-   0        0        0     6375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/LoaderCodes.py
--rw-rw-rw-   0        0        0     9951 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/LocalsDictCodes.py
--rw-rw-rw-   0        0        0     3135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/LoopCodes.py
--rw-rw-rw-   0        0        0     1597 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/MatchCodes.py
--rw-rw-rw-   0        0        0     6291 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ModuleCodes.py
--rw-rw-rw-   0        0        0     8118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/Namify.py
--rw-rw-rw-   0        0        0    12777 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/OperationCodes.py
--rw-rw-rw-   0        0        0    28231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/PackageResourceCodes.py
--rw-rw-rw-   0        0        0     3021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/PrintCodes.py
--rw-rw-rw-   0        0        0     5474 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/PythonAPICodes.py
--rw-rw-rw-   0        0        0    13095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/RaisingCodes.py
--rw-rw-rw-   0        0        0     3443 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/Reports.py
--rw-rw-rw-   0        0        0     5234 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/ReturnCodes.py
--rw-rw-rw-   0        0        0     6517 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/SetCodes.py
--rw-rw-rw-   0        0        0    13949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/SliceCodes.py
--rw-rw-rw-   0        0        0     9809 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/StringCodes.py
--rw-rw-rw-   0        0        0     8188 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/SubscriptCodes.py
--rw-rw-rw-   0        0        0    11176 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/TryCodes.py
--rw-rw-rw-   0        0        0     3786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/TupleCodes.py
--rw-rw-rw-   0        0        0    14717 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/VariableCodes.py
--rw-rw-rw-   0        0        0     9121 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/VariableDeclarations.py
--rw-rw-rw-   0        0        0     8099 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/YieldCodes.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.417234 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/
--rw-rw-rw-   0        0        0     6069 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeBases.py
--rw-rw-rw-   0        0        0     3399 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-rw-rw-   0        0        0     1804 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-rw-rw-   0        0        0     1378 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-rw-rw-   0        0        0     3610 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-rw-rw-   0        0        0     5128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-rw-rw-   0        0        0     5211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-rw-rw-   0        0        0     3955 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-rw-rw-   0        0        0    19628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-rw-rw-   0        0        0     2852 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeVoids.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:54.438235 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/
--rw-rw-rw-   0        0        0     2845 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-rw-rw-   0        0        0     5865 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-rw-rw-   0        0        0     2921 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-rw-rw-   0        0        0     2290 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-rw-rw-   0        0        0     6339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-rw-rw-   0        0        0     3321 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-rw-rw-   0        0        0     3306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-rw-rw-   0        0        0     2335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-rw-rw-   0        0        0     4217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-rw-rw-   0        0        0    21441 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-rw-rw-   0        0        0     6640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-rw-rw-   0        0        0     2475 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.360374 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/
--rw-rw-rw-   0        0        0    11231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-rw-rw-   0        0        0     5847 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-rw-rw-   0        0        0    23760 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-rw-rw-   0        0        0     5238 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-rw-rw-   0        0        0     1843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-rw-rw-   0        0        0     2817 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-rw-rw-   0        0        0    12819 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-rw-rw-   0        0        0     2044 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-rw-rw-   0        0        0     2762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-rw-rw-   0        0        0     1544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-rw-rw-   0        0        0     7197 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-rw-rw-   0        0        0    12850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-rw-rw-   0        0        0     4288 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-rw-rw-   0        0        0     2088 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-rw-rw-   0        0        0     2118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-rw-rw-   0        0        0     3933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-rw-rw-   0        0        0     7407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-rw-rw-   0        0        0     4292 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-rw-rw-   0        0        0     3860 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-rw-rw-   0        0        0     4487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-rw-rw-   0        0        0    11579 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-rw-rw-   0        0        0    19317 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-rw-rw-   0        0        0     2843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-rw-rw-   0        0        0     3635 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-rw-rw-   0        0        0    11102 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-rw-rw-   0        0        0    15380 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-rw-rw-   0        0        0     2979 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-rw-rw-   0        0        0    10421 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-rw-rw-   0        0        0     2557 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-rw-rw-   0        0        0     3020 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-rw-rw-   0        0        0     2984 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-rw-rw-   0        0        0     3173 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.369372 Nuitka-winsvc-1.6.4/nuitka/containers/
--rw-rw-rw-   0        0        0     1435 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/containers/Namedtuples.py
--rw-rw-rw-   0        0        0     6553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/containers/OrderedDicts.py
--rw-rw-rw-   0        0        0      554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/containers/OrderedSets.py
--rw-rw-rw-   0        0        0     4397 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/containers/OrderedSetsFallback.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.373383 Nuitka-winsvc-1.6.4/nuitka/distutils/
--rw-rw-rw-   0        0        0     1964 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/distutils/Build.py
--rw-rw-rw-   0        0        0    14219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/distutils/DistutilCommands.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/distutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.376956 Nuitka-winsvc-1.6.4/nuitka/finalizations/
--rw-rw-rw-   0        0        0     1224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/finalizations/Finalization.py
--rw-rw-rw-   0        0        0     6110 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/finalizations/FinalizeMarkups.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/finalizations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.391954 Nuitka-winsvc-1.6.4/nuitka/freezer/
--rw-rw-rw-   0        0        0     7311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/DependsExe.py
--rw-rw-rw-   0        0        0     2584 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/DllDependenciesCommon.py
--rw-rw-rw-   0        0        0    10811 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/DllDependenciesMacOS.py
--rw-rw-rw-   0        0        0     7211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/DllDependenciesPosix.py
--rw-rw-rw-   0        0        0     6620 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/DllDependenciesWin32.py
--rw-rw-rw-   0        0        0    17336 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/IncludedDataFiles.py
--rw-rw-rw-   0        0        0     9492 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/IncludedEntryPoints.py
--rw-rw-rw-   0        0        0    10112 2023-06-25 05:59:12.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/Onefile.py
--rw-rw-rw-   0        0        0    26319 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/Standalone.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/freezer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.403953 Nuitka-winsvc-1.6.4/nuitka/importing/
--rw-rw-rw-   0        0        0    11007 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.4/nuitka/importing/IgnoreListing.py
--rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/importing/ImportCache.py
--rw-rw-rw-   0        0        0     6455 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/importing/ImportResolving.py
--rw-rw-rw-   0        0        0    28463 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/importing/Importing.py
--rw-rw-rw-   0        0        0     4738 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/importing/PreloadedPackages.py
--rw-rw-rw-   0        0        0    16375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/importing/Recursion.py
--rw-rw-rw-   0        0        0    10981 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/importing/StandardLibrary.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/importing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.535573 Nuitka-winsvc-1.6.4/nuitka/nodes/
--rw-rw-rw-   0        0        0     3637 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/AsyncgenNodes.py
--rw-rw-rw-   0        0        0     4082 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/AttributeLookupNodes.py
--rw-rw-rw-   0        0        0    12004 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/AttributeNodes.py
--rw-rw-rw-   0        0        0   378745 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/AttributeNodesGenerated.py
--rw-rw-rw-   0        0        0     3823 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinAllNodes.py
--rw-rw-rw-   0        0        0     4098 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinAnyNodes.py
--rw-rw-rw-   0        0        0     2496 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinComplexNodes.py
--rw-rw-rw-   0        0        0     1698 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinDecodingNodes.py
--rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-rw-rw-   0        0        0     4694 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinDictNodes.py
--rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinFormatNodes.py
--rw-rw-rw-   0        0        0     2142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinHashNodes.py
--rw-rw-rw-   0        0        0     5334 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinIntegerNodes.py
--rw-rw-rw-   0        0        0    12723 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinIteratorNodes.py
--rw-rw-rw-   0        0        0     1996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinLenNodes.py
--rw-rw-rw-   0        0        0     3606 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinNextNodes.py
--rw-rw-rw-   0        0        0     3240 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinOpenNodes.py
--rw-rw-rw-   0        0        0   245536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-rw-rw-   0        0        0    18589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinRangeNodes.py
--rw-rw-rw-   0        0        0     9067 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinRefNodes.py
--rw-rw-rw-   0        0        0     3307 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinSumNodes.py
--rw-rw-rw-   0        0        0    13543 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinTypeNodes.py
--rw-rw-rw-   0        0        0     1573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinVarsNodes.py
--rw-rw-rw-   0        0        0    26113 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/BytesNodes.py
--rw-rw-rw-   0        0        0     6478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/CallNodes.py
--rw-rw-rw-   0        0        0     1550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/Checkers.py
--rw-rw-rw-   0        0        0   605501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ChildrenHavingMixins.py
--rw-rw-rw-   0        0        0     8448 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ClassNodes.py
--rw-rw-rw-   0        0        0     6585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/CodeObjectSpecs.py
--rw-rw-rw-   0        0        0    21683 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ComparisonNodes.py
--rw-rw-rw-   0        0        0    30314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ConditionalNodes.py
--rw-rw-rw-   0        0        0    46536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ConstantRefNodes.py
--rw-rw-rw-   0        0        0    12213 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ContainerMakingNodes.py
--rw-rw-rw-   0        0        0     2834 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ContainerOperationNodes.py
--rw-rw-rw-   0        0        0     4581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/CoroutineNodes.py
--rw-rw-rw-   0        0        0     1714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/CtypesNodes.py
--rw-rw-rw-   0        0        0    51021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/DictionaryNodes.py
--rw-rw-rw-   0        0        0     7856 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ExceptionNodes.py
--rw-rw-rw-   0        0        0     7317 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ExecEvalNodes.py
--rw-rw-rw-   0        0        0    44996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ExpressionBases.py
--rw-rw-rw-   0        0        0    45091 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ExpressionBasesGenerated.py
--rw-rw-rw-   0        0        0    21278 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ExpressionShapeMixins.py
--rw-rw-rw-   0        0        0    12156 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/FrameNodes.py
--rw-rw-rw-   0        0        0     3544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/FunctionAttributeNodes.py
--rw-rw-rw-   0        0        0    39803 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/FunctionNodes.py
--rw-rw-rw-   0        0        0     5376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/FutureSpecs.py
--rw-rw-rw-   0        0        0     6256 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/GeneratorNodes.py
--rw-rw-rw-   0        0        0     6850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/GlobalsLocalsNodes.py
--rw-rw-rw-   0        0        0    74177 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/HardImportNodesGenerated.py
--rw-rw-rw-   0        0        0     5511 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ImportHardNodes.py
--rw-rw-rw-   0        0        0    45692 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ImportNodes.py
--rw-rw-rw-   0        0        0     2733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/IndicatorMixins.py
--rw-rw-rw-   0        0        0     1502 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/InjectCNodes.py
--rw-rw-rw-   0        0        0    11228 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/IterationHandles.py
--rw-rw-rw-   0        0        0    11002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/KeyValuePairNodes.py
--rw-rw-rw-   0        0        0    16320 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ListOperationNodes.py
--rw-rw-rw-   0        0        0    23094 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/LocalsDictNodes.py
--rw-rw-rw-   0        0        0    14922 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/LocalsScopes.py
--rw-rw-rw-   0        0        0    15581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/LoopNodes.py
--rw-rw-rw-   0        0        0     1712 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/MatchNodes.py
--rw-rw-rw-   0        0        0     6534 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ModuleAttributeNodes.py
--rw-rw-rw-   0        0        0    30829 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ModuleNodes.py
--rw-rw-rw-   0        0        0    24899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/NodeBases.py
--rw-rw-rw-   0        0        0    15128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/NodeMakingHelpers.py
--rw-rw-rw-   0        0        0     5550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/NodeMetaClasses.py
--rw-rw-rw-   0        0        0    31894 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/OperatorNodes.py
--rw-rw-rw-   0        0        0     9134 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/OperatorNodesUnary.py
--rw-rw-rw-   0        0        0     4202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/OsSysNodes.py
--rw-rw-rw-   0        0        0    12442 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/OutlineNodes.py
--rw-rw-rw-   0        0        0    31330 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/PackageMetadataNodes.py
--rw-rw-rw-   0        0        0     4464 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/PackageResourceNodes.py
--rw-rw-rw-   0        0        0     3407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/PrintNodes.py
--rw-rw-rw-   0        0        0     6772 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/ReturnNodes.py
--rw-rw-rw-   0        0        0     4715 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/SideEffectNodes.py
--rw-rw-rw-   0        0        0    12501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/SliceNodes.py
--rw-rw-rw-   0        0        0    94880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/StatementBasesGenerated.py
--rw-rw-rw-   0        0        0     9430 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/StatementNodes.py
--rw-rw-rw-   0        0        0    28658 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/StrNodes.py
--rw-rw-rw-   0        0        0     3504 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/StringConcatenationNodes.py
--rw-rw-rw-   0        0        0     8640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/SubscriptNodes.py
--rw-rw-rw-   0        0        0    17853 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/TryNodes.py
--rw-rw-rw-   0        0        0     2405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/TypeMatchNodes.py
--rw-rw-rw-   0        0        0    10911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/TypeNodes.py
--rw-rw-rw-   0        0        0    39522 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/VariableAssignNodes.py
--rw-rw-rw-   0        0        0    10746 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/VariableDelNodes.py
--rw-rw-rw-   0        0        0     4574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/VariableNameNodes.py
--rw-rw-rw-   0        0        0    30982 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/VariableRefNodes.py
--rw-rw-rw-   0        0        0     4748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/VariableReleaseNodes.py
--rw-rw-rw-   0        0        0     3902 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/YieldNodes.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.540575 Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/
--rw-rw-rw-   0        0        0   156243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-rw-rw-   0        0        0     4387 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-rw-rw-   0        0        0     4567 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/ShapeMixins.py
--rw-rw-rw-   0        0        0    42374 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/StandardShapes.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.553574 Nuitka-winsvc-1.6.4/nuitka/optimizations/
--rw-rw-rw-   0        0        0     3279 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/optimizations/BytecodeDemotion.py
--rw-rw-rw-   0        0        0     3920 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/optimizations/FunctionInlining.py
--rw-rw-rw-   0        0        0     2144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/optimizations/Graphs.py
--rw-rw-rw-   0        0        0    10762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/optimizations/Optimization.py
--rw-rw-rw-   0        0        0    52058 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.4/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-rw-rw-   0        0        0     2272 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/optimizations/Tags.py
--rw-rw-rw-   0        0        0    40896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/optimizations/TraceCollections.py
--rw-rw-rw-   0        0        0    23977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/optimizations/ValueTraces.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/optimizations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.555574 Nuitka-winsvc-1.6.4/nuitka/pgo/
--rw-rw-rw-   0        0        0     4663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/pgo/PGO.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/pgo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.558574 Nuitka-winsvc-1.6.4/nuitka/plugins/
--rw-rw-rw-   0        0        0    40054 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/PluginBase.py
--rw-rw-rw-   0        0        0    56200 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/Plugins.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.614578 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/
--rw-rw-rw-   0        0        0    19102 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-rw-rw-   0        0        0     3460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-rw-rw-   0        0        0     9939 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/DataFilesPlugin.py
--rw-rw-rw-   0        0        0     4404 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/DelvewheelPlugin.py
--rw-rw-rw-   0        0        0     5675 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/DillPlugin.py
--rw-rw-rw-   0        0        0    13757 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/DllFilesPlugin.py
--rw-rw-rw-   0        0        0     2062 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/EnumPlugin.py
--rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/EventletPlugin.py
--rw-rw-rw-   0        0        0     1880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/GeventPlugin.py
--rw-rw-rw-   0        0        0     3482 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/GiPlugin.py
--rw-rw-rw-   0        0        0     5027 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/GlfwPlugin.py
--rw-rw-rw-   0        0        0    18335 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/ImplicitImports.py
--rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/KivyPlugin.py
--rw-rw-rw-   0        0        0     7258 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-rw-rw-   0        0        0     6667 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-rw-rw-   0        0        0     1187 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/NumpyPlugin.py
--rw-rw-rw-   0        0        0     6554 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-rw-rw-   0        0        0     1917 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PbrPlugin.py
--rw-rw-rw-   0        0        0     4665 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-rw-rw-   0        0        0     6992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PmwPlugin.py
--rw-rw-rw-   0        0        0    50023 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-rw-rw-   0        0        0     2933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PywebViewPlugin.py
--rw-rw-rw-   0        0        0     1160 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TensorflowPlugin.py
--rw-rw-rw-   0        0        0    12180 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TkinterPlugin.py
--rw-rw-rw-   0        0        0     1140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TorchPlugin.py
--rw-rw-rw-   0        0        0     9855 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TransformersPlugin.py
--rw-rw-rw-   0        0        0     3175 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TrioPlugin.py
--rw-rw-rw-   0        0        0     5640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/UpxPlugin.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/__init__.py
--rw-rw-rw-   0        0        0   150488 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     2221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.635575 Nuitka-winsvc-1.6.4/nuitka/reports/
--rw-rw-rw-   0        0        0     2209 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/reports/LicenseReport.rst.j2
--rw-rw-rw-   0        0        0    17538 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/reports/Reports.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.651576 Nuitka-winsvc-1.6.4/nuitka/specs/
--rw-rw-rw-   0        0        0     5911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-rw-rw-   0        0        0     2786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-rw-rw-   0        0        0     2541 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinListOperationSpecs.py
--rw-rw-rw-   0        0        0    26455 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinParameterSpecs.py
--rw-rw-rw-   0        0        0     6065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-rw-rw-   0        0        0     4802 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-rw-rw-   0        0        0     5133 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/HardImportSpecs.py
--rw-rw-rw-   0        0        0    18740 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/ParameterSpecs.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/specs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.654576 Nuitka-winsvc-1.6.4/nuitka/tools/
--rw-rw-rw-   0        0        0     1603 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/Basics.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.655575 Nuitka-winsvc-1.6.4/nuitka/tools/commercial/
--rw-rw-rw-   0        0        0      815 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/commercial/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.658575 Nuitka-winsvc-1.6.4/nuitka/tools/data_composer/
--rw-rw-rw-   0        0        0    14054 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/data_composer/DataComposer.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/data_composer/__init__.py
--rw-rw-rw-   0        0        0     1306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/data_composer/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.665577 Nuitka-winsvc-1.6.4/nuitka/tools/environments/
--rw-rw-rw-   0        0        0     2449 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/environments/CreateEnvironment.py
--rw-rw-rw-   0        0        0     3735 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/environments/Virtualenv.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/environments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.666576 Nuitka-winsvc-1.6.4/nuitka/tools/general/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/general/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.668578 Nuitka-winsvc-1.6.4/nuitka/tools/general/dll_report/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/general/dll_report/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/general/dll_report/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.671578 Nuitka-winsvc-1.6.4/nuitka/tools/general/find_module/
--rw-rw-rw-   0        0        0     3798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/general/find_module/FindModuleCode.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/general/find_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.674576 Nuitka-winsvc-1.6.4/nuitka/tools/onefile_compressor/
--rw-rw-rw-   0        0        0    10194 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/onefile_compressor/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/onefile_compressor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.676576 Nuitka-winsvc-1.6.4/nuitka/tools/profiler/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/profiler/__init__.py
--rw-rw-rw-   0        0        0     2529 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/profiler/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.682577 Nuitka-winsvc-1.6.4/nuitka/tools/scanning/
--rw-rw-rw-   0        0        0     3344 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/scanning/DisplayPackageData.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/scanning/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.687577 Nuitka-winsvc-1.6.4/nuitka/tools/specialize/
--rw-rw-rw-   0        0        0    51143 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/specialize/CTypeDescriptions.py
--rw-rw-rw-   0        0        0     7685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/specialize/Common.py
--rw-rw-rw-   0        0        0    39625 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/specialize/SpecializeC.py
--rw-rw-rw-   0        0        0    33585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/specialize/SpecializePython.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.4/nuitka/tools/specialize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.699063 Nuitka-winsvc-1.6.4/nuitka/tools/testing/
--rw-rw-rw-   0        0        0    55396 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/Common.py
--rw-rw-rw-   0        0        0     1483 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/Constructs.py
--rw-rw-rw-   0        0        0     8940 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/OutputComparison.py
--rw-rw-rw-   0        0        0     1278 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/Pythons.py
--rw-rw-rw-   0        0        0     7888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/RuntimeTracing.py
--rw-rw-rw-   0        0        0     5371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/SearchModes.py
--rw-rw-rw-   0        0        0     3375 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/Valgrind.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.702059 Nuitka-winsvc-1.6.4/nuitka/tools/testing/check_reference_counts/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-rw-rw-   0        0        0     3064 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/check_reference_counts/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.704059 Nuitka-winsvc-1.6.4/nuitka/tools/testing/compare_with_cpython/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-rw-rw-   0        0        0    29429 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/compare_with_cpython/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.706060 Nuitka-winsvc-1.6.4/nuitka/tools/testing/find_sxs_modules/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/find_sxs_modules/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/find_sxs_modules/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.709060 Nuitka-winsvc-1.6.4/nuitka/tools/testing/measure_construct_performance/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-rw-rw-   0        0        0     8755 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/measure_construct_performance/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.712062 Nuitka-winsvc-1.6.4/nuitka/tools/testing/run_nuitka_tests/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/run_nuitka_tests/__init__.py
--rw-rw-rw-   0        0        0    36321 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/testing/run_nuitka_tests/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.716060 Nuitka-winsvc-1.6.4/nuitka/tools/watch/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/watch/__init__.py
--rw-rw-rw-   0        0        0     9503 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tools/watch/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.768845 Nuitka-winsvc-1.6.4/nuitka/tree/
--rw-rw-rw-   0        0        0    47126 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/Building.py
--rw-rw-rw-   0        0        0    74608 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ComplexCallHelperFunctions.py
--rw-rw-rw-   0        0        0     1700 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/Extractions.py
--rw-rw-rw-   0        0        0     2572 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/InternalModule.py
--rw-rw-rw-   0        0        0     1511 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/Operations.py
--rw-rw-rw-   0        0        0     2807 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationAssertStatements.py
--rw-rw-rw-   0        0        0    42768 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationAssignmentStatements.py
--rw-rw-rw-   0        0        0     2948 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationBooleanExpressions.py
--rw-rw-rw-   0        0        0    11693 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationCallExpressions.py
--rw-rw-rw-   0        0        0    15072 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationClasses.py
--rw-rw-rw-   0        0        0    37638 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationClasses3.py
--rw-rw-rw-   0        0        0     6430 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationComparisonExpressions.py
--rw-rw-rw-   0        0        0    22111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationContractionExpressions.py
--rw-rw-rw-   0        0        0    11061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationDictionaryCreation.py
--rw-rw-rw-   0        0        0    14607 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationExecStatements.py
--rw-rw-rw-   0        0        0     7782 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationForLoopStatements.py
--rw-rw-rw-   0        0        0    26215 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationFunctionStatements.py
--rw-rw-rw-   0        0        0    13437 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationImportStatements.py
--rw-rw-rw-   0        0        0     6577 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationLambdaExpressions.py
--rw-rw-rw-   0        0        0    20962 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationMatchStatements.py
--rw-rw-rw-   0        0        0     2409 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationMultidist.py
--rw-rw-rw-   0        0        0     8194 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationNamespacePackages.py
--rw-rw-rw-   0        0        0     4658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationPrintStatements.py
--rw-rw-rw-   0        0        0    15371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationSequenceCreation.py
--rw-rw-rw-   0        0        0     4824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-rw-rw-   0        0        0    14615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationTryExceptStatements.py
--rw-rw-rw-   0        0        0     6982 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-rw-rw-   0        0        0     5674 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-rw-rw-   0        0        0    14341 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationWithStatements.py
--rw-rw-rw-   0        0        0     3088 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationYieldExpressions.py
--rw-rw-rw-   0        0        0    12746 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/SourceHandling.py
--rw-rw-rw-   0        0        0     3757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/SyntaxErrors.py
--rw-rw-rw-   0        0        0    22973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/TreeHelpers.py
--rw-rw-rw-   0        0        0    20012 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/VariableClosure.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.807833 Nuitka-winsvc-1.6.4/nuitka/utils/
--rw-rw-rw-   0        0        0     2655 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/AppDirs.py
--rw-rw-rw-   0        0        0     3248 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/CStrings.py
--rw-rw-rw-   0        0        0     3653 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/CommandLineOptions.py
--rw-rw-rw-   0        0        0     4297 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Distributions.py
--rw-rw-rw-   0        0        0     5794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Download.py
--rw-rw-rw-   0        0        0    12376 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Execution.py
--rw-rw-rw-   0        0        0    36129 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/FileOperations.py
--rw-rw-rw-   0        0        0     2885 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Hashing.py
--rw-rw-rw-   0        0        0     2362 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Images.py
--rw-rw-rw-   0        0        0     6816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Importing.py
--rw-rw-rw-   0        0        0     8149 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/InstalledPythons.py
--rw-rw-rw-   0        0        0     2224 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/InstanceCounters.py
--rw-rw-rw-   0        0        0     4336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Jinja2.py
--rw-rw-rw-   0        0        0     1238 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Json.py
--rw-rw-rw-   0        0        0     4304 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.4/nuitka/utils/MacOSApp.py
--rw-rw-rw-   0        0        0     5040 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/MemoryUsage.py
--rw-rw-rw-   0        0        0     9057 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/ModuleNames.py
--rw-rw-rw-   0        0        0     4309 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/ReExecute.py
--rw-rw-rw-   0        0        0     3815 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Rest.py
--rw-rw-rw-   0        0        0    22714 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/SharedLibraries.py
--rw-rw-rw-   0        0        0     3664 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Shebang.py
--rw-rw-rw-   0        0        0     2591 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Signing.py
--rw-rw-rw-   0        0        0     6207 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/StaticLibraries.py
--rw-rw-rw-   0        0        0     2602 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/ThreadedExecutor.py
--rw-rw-rw-   0        0        0     2772 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Timing.py
--rw-rw-rw-   0        0        0    10826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Utils.py
--rw-rw-rw-   0        0        0    10574 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/WindowsFileUsage.py
--rw-rw-rw-   0        0        0    19540 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/WindowsResources.py
--rw-rw-rw-   0        0        0     6108 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/Yaml.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/nuitka/utils/__init__.py
--rw-rw-rw-   0        0        0      834 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 06:03:00.103581 Nuitka-winsvc-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0    15001 2023-06-25 05:59:12.000000 Nuitka-winsvc-1.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:55.816833 Nuitka-winsvc-1.6.4/tests/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.068194 Nuitka-winsvc-1.6.4/tests/basics/
--rw-rw-rw-   0        0        0     1766 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/AssertsTest.py
--rw-rw-rw-   0        0        0     5934 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/AssignmentsTest.py
--rw-rw-rw-   0        0        0     5866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/AssignmentsTest32.py
--rw-rw-rw-   0        0        0     4055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/BranchingTest.py
--rw-rw-rw-   0        0        0     1104 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/BuiltinOverload.py
--rw-rw-rw-   0        0        0     3749 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/BuiltinSuperTest.py
--rw-rw-rw-   0        0        0    17080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/BuiltinsTest.py
--rw-rw-rw-   0        0        0      866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ClassMinimalTest.py
--rw-rw-rw-   0        0        0     4764 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ClassesTest.py
--rw-rw-rw-   0        0        0     3414 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ClassesTest32.py
--rw-rw-rw-   0        0        0     1406 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ClassesTest34.py
--rw-rw-rw-   0        0        0     4698 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ComparisonChainsTest.py
--rw-rw-rw-   0        0        0     4639 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ConstantsTest.py
--rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ConstantsTest27.py
--rw-rw-rw-   0        0        0     1628 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/DecoratorsTest.py
--rw-rw-rw-   0        0        0     2317 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/DefaultParametersTest.py
--rw-rw-rw-   0        0        0     1127 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/DoubleDeletionsTest.py
--rw-rw-rw-   0        0        0      806 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/EmptyModuleTest.py
--rw-rw-rw-   0        0        0    14387 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ExceptionRaisingTest.py
--rw-rw-rw-   0        0        0      961 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ExceptionRaisingTest32.py
--rw-rw-rw-   0        0        0     1458 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ExceptionRaisingTest33.py
--rw-rw-rw-   0        0        0     6747 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ExecEvalTest.py
--rw-rw-rw-   0        0        0     1417 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ExtremeClosureTest.py
--rw-rw-rw-   0        0        0     1658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/FunctionObjectsTest.py
--rw-rw-rw-   0        0        0    12335 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/FunctionsTest.py
--rw-rw-rw-   0        0        0     3603 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/FunctionsTest32.py
--rw-rw-rw-   0        0        0     2627 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/FunctionsTest_2.py
--rw-rw-rw-   0        0        0      890 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/FutureTest32.py
--rw-rw-rw-   0        0        0     5809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/GeneratorExpressionsTest.py
--rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/GeneratorExpressionsTest_37.py
--rw-rw-rw-   0        0        0     3824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/GlobalStatementTest.py
--rw-rw-rw-   0        0        0     1286 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/HelloWorldTest_2.py
--rw-rw-rw-   0        0        0     2469 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ImportingTest.py
--rw-rw-rw-   0        0        0     1296 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/InplaceOperationsTest.py
--rw-rw-rw-   0        0        0     4227 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/InspectionTest.py
--rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/InspectionTest_35.py
--rw-rw-rw-   0        0        0     1618 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/InspectionTest_36.py
--rw-rw-rw-   0        0        0     1671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/LambdasTest.py
--rw-rw-rw-   0        0        0     2731 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/LateClosureAssignmentTest.py
--rw-rw-rw-   0        0        0     2923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ListContractionsTest.py
--rw-rw-rw-   0        0        0     3329 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/LoopingTest.py
--rw-rw-rw-   0        0        0     1536 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/MainProgramsTest.py
--rw-rw-rw-   0        0        0     1925 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ModuleAttributesTest.py
--rw-rw-rw-   0        0        0     1988 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/OperatorsTest.py
--rw-rw-rw-   0        0        0    14903 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/OrderChecksTest.py
--rw-rw-rw-   0        0        0     1827 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/OrderChecksTest27.py
--rw-rw-rw-   0        0        0     1452 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/OverflowFunctionsTest_2.py
--rw-rw-rw-   0        0        0     5853 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ParameterErrorsTest.py
--rw-rw-rw-   0        0        0     1899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ParameterErrorsTest32.py
--rw-rw-rw-   0        0        0      863 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/PrintFutureTest.py
--rw-rw-rw-   0        0        0     1413 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/PrintingTest_2.py
--rw-rw-rw-   0        0        0      878 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/RecursionTest.py
--rw-rw-rw-   0        0        0    23840 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest.py
--rw-rw-rw-   0        0        0     2076 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest27.py
--rw-rw-rw-   0        0        0     7819 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest33.py
--rw-rw-rw-   0        0        0     4902 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest35.py
--rw-rw-rw-   0        0        0     5092 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest36.py
--rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest_2.py
--rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/SlotsTest.py
--rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/ThreadedGeneratorsTest.py
--rw-rw-rw-   0        0        0    22966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/TrickAssignmentsTest32.py
--rw-rw-rw-   0        0        0     1541 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/TrickAssignmentsTest35.py
--rw-rw-rw-   0        0        0     1788 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/TrickAssignmentsTest_2.py
--rw-rw-rw-   0        0        0     2086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/TryContinueFinallyTest.py
--rw-rw-rw-   0        0        0     2212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/TryExceptContinueTest.py
--rw-rw-rw-   0        0        0     2275 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/TryExceptFinallyTest.py
--rw-rw-rw-   0        0        0     2304 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/TryExceptFramesTest.py
--rw-rw-rw-   0        0        0     2842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/TryReturnFinallyTest.py
--rw-rw-rw-   0        0        0     2328 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/TryYieldFinallyTest.py
--rw-rw-rw-   0        0        0     1093 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/UnicodeTest.py
--rw-rw-rw-   0        0        0     1877 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/UnpackingTest35.py
--rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/VarargsTest.py
--rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/WithStatementsTest.py
--rw-rw-rw-   0        0        0     3070 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/YieldFromTest33.py
--rw-rw-rw-   0        0        0     3821 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/run_all.py
--rw-rw-rw-   0        0        0     2271 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/basics/run_xml.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.123195 Nuitka-winsvc-1.6.4/tests/onefile/
--rw-rw-rw-   0        0        0     1213 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/onefile/HelloWorldTest.py
--rw-rw-rw-   0        0        0     1307 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/onefile/KeyboardInterruptTest.py
--rw-rw-rw-   0        0        0     5816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/onefile/run_all.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.281787 Nuitka-winsvc-1.6.4/tests/optimizations/
--rw-rw-rw-   0        0        0      958 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/ArgumentTypes.py
--rw-rw-rw-   0        0        0     1055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/Attributes.py
--rw-rw-rw-   0        0        0     1021 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/Calls.py
--rw-rw-rw-   0        0        0      921 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/Conditions.py
--rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/DecodingOperations.py
--rw-rw-rw-   0        0        0     1212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/FormatStrings36.py
--rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/HardImports.py
--rw-rw-rw-   0        0        0      974 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/HardImports_2.py
--rw-rw-rw-   0        0        0      918 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/Iterations.py
--rw-rw-rw-   0        0        0     1260 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/Len.py
--rw-rw-rw-   0        0        0     2262 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/Operations.py
--rw-rw-rw-   0        0        0     1333 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/Subscripts.py
--rw-rw-rw-   0        0        0     8736 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/optimizations/run_all.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.289826 Nuitka-winsvc-1.6.4/tests/packages/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.299797 Nuitka-winsvc-1.6.4/tests/packages/package_import_success_after_failure/
--rw-rw-rw-   0        0        0     2382 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.315796 Nuitka-winsvc-1.6.4/tests/packages/package_import_success_after_failure/variable_package/
--rw-rw-rw-   0        0        0      942 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
--rw-rw-rw-   0        0        0     1168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rw-rw-rw-   0        0        0     3671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/run_all.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.085054 Nuitka-winsvc-1.6.4/tests/packages/sub_package/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.352419 Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/
--rw-rw-rw-   0        0        0     1230 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/__init__.py
--rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/bigkitty.py
--rw-rw-rw-   0        0        0      910 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/smallkitty.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.402076 Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/speak/
--rw-rw-rw-   0        0        0      929 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/speak/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/speak/hello.py
--rw-rw-rw-   0        0        0      966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/speak/miau.py
--rw-rw-rw-   0        0        0      968 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/speak/purr.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.086053 Nuitka-winsvc-1.6.4/tests/packages/top_level_attributes_3/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.426083 Nuitka-winsvc-1.6.4/tests/packages/top_level_attributes_3/some_package/
--rw-rw-rw-   0        0        0     2336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-rw-rw-   0        0        0      907 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.440084 Nuitka-winsvc-1.6.4/tests/plugins/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.442078 Nuitka-winsvc-1.6.4/tests/plugins/code_signing/
--rw-rw-rw-   0        0        0     1170 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/plugins/code_signing/CodeSigningMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.458691 Nuitka-winsvc-1.6.4/tests/plugins/data_files/
--rw-rw-rw-   0        0        0     1332 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/plugins/data_files/DataFilesMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.473703 Nuitka-winsvc-1.6.4/tests/plugins/data_files/data_files_package/
--rw-rw-rw-   0        0        0      924 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/plugins/data_files/data_files_package/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/tests/plugins/data_files/data_files_package/lala.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.474702 Nuitka-winsvc-1.6.4/tests/plugins/data_files/data_files_package/sub_dir/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-rw-rw-   0        0        0      255 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/tests/plugins/data_files/test_case.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.538702 Nuitka-winsvc-1.6.4/tests/plugins/parameters/
--rw-rw-rw-   0        0        0     1019 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/plugins/parameters/ParametersMain.py
--rw-rw-rw-   0        0        0     2168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/plugins/parameters/parameter-using-plugin.py
--rw-rw-rw-   0        0        0     3861 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/plugins/run_all.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.554710 Nuitka-winsvc-1.6.4/tests/programs/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.573718 Nuitka-winsvc-1.6.4/tests/programs/absolute_import/
--rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.631884 Nuitka-winsvc-1.6.4/tests/programs/absolute_import/foobar/
--rw-rw-rw-   0        0        0      796 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/absolute_import/foobar/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/absolute_import/foobar/foobar.py
--rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/absolute_import/foobar/local.py
--rw-rw-rw-   0        0        0      860 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/absolute_import/foobar/util.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.638883 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.655883 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path1/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.670883 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path1/Some_Package/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.687579 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path2/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path2/some_module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.704580 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path2/some_package/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path2/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.714588 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.726597 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path1/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path1/some_module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.740587 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path1/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.748582 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path2/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.754587 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path2/Some_Package/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.768582 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/
--rw-rw-rw-   0        0        0     1075 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.775588 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path1/
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.785588 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path1/Some_Package/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.800589 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path2/
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.807589 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path2/Some_Package/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.818582 Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/
--rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.867784 Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
--rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.919078 Nuitka-winsvc-1.6.4/tests/programs/dash_import/
--rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/dash_import/DashImportMain.py
--rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/dash_import/dash-module.py
--rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/dash_import/plus+module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.926078 Nuitka-winsvc-1.6.4/tests/programs/dash_main/
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/dash_main/Dash-Main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.937078 Nuitka-winsvc-1.6.4/tests/programs/deep/
--rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/deep/DeepProgramMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:57.967078 Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/
--rw-rw-rw-   0        0        0      980 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/DeepBrother.py
--rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/DeepChild.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.003080 Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/deep_package/
--rw-rw-rw-   0        0        0      876 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
--rw-rw-rw-   0        0        0      952 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/deep_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.010079 Nuitka-winsvc-1.6.4/tests/programs/dunderinit_imports/
--rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.040079 Nuitka-winsvc-1.6.4/tests/programs/dunderinit_imports/package/
--rw-rw-rw-   0        0        0      797 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/dunderinit_imports/package/SubModule.py
--rw-rw-rw-   0        0        0      857 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/dunderinit_imports/package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.053113 Nuitka-winsvc-1.6.4/tests/programs/import_variants/
--rw-rw-rw-   0        0        0     1005 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/import_variants/ImportVariationsMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.097089 Nuitka-winsvc-1.6.4/tests/programs/import_variants/some_package/
--rw-rw-rw-   0        0        0      946 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/import_variants/some_package/Child1.py
--rw-rw-rw-   0        0        0     1098 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/import_variants/some_package/Child2.py
--rw-rw-rw-   0        0        0      822 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/import_variants/some_package/Child3.py
--rw-rw-rw-   0        0        0      994 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/import_variants/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.137078 Nuitka-winsvc-1.6.4/tests/programs/main_raises/
--rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/main_raises/ErrorMain.py
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/main_raises/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.163085 Nuitka-winsvc-1.6.4/tests/programs/main_raises2/
--rw-rw-rw-   0        0        0     1080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/main_raises2/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.174081 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/
--rw-rw-rw-   0        0        0     1529 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.201082 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/
--rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/Nearby1.py
--rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.215083 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/
--rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.224081 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.252080 Nuitka-winsvc-1.6.4/tests/programs/module_exits/
--rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_exits/ErrorExitingModule.py
--rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_exits/Main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.287079 Nuitka-winsvc-1.6.4/tests/programs/module_object_replacing/
--rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-rw-rw-   0        0        0     1359 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.301082 Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/
--rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.353736 Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/foo/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/foo/__init__.py
--rw-rw-rw-   0        0        0      836 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/foo/__main__.py
--rw-rw-rw-   0        0        0     1758 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/foo/entry.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.370707 Nuitka-winsvc-1.6.4/tests/programs/named_imports/
--rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/named_imports/NamedImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.401279 Nuitka-winsvc-1.6.4/tests/programs/named_imports/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/named_imports/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/named_imports/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.404279 Nuitka-winsvc-1.6.4/tests/programs/named_imports/some_package/sub_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.416285 Nuitka-winsvc-1.6.4/tests/programs/package_code/
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_code/PackageInitCodeMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.434282 Nuitka-winsvc-1.6.4/tests/programs/package_code/some_package/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_code/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_code/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.471282 Nuitka-winsvc-1.6.4/tests/programs/package_contains_main/
--rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_contains_main/PackageContainsMain.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_contains_main/__init__.py
--rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_contains_main/local.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.488283 Nuitka-winsvc-1.6.4/tests/programs/package_init_import/
--rw-rw-rw-   0        0        0      823 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_init_import/PackageInitImportMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.518289 Nuitka-winsvc-1.6.4/tests/programs/package_init_import/some_package/
--rw-rw-rw-   0        0        0     1008 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_init_import/some_package/PackageLocal.py
--rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_init_import/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.525289 Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/
--rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.536321 Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/some_package/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.570284 Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/some_package/child_package/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-rw-rw-   0        0        0      795 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/some_package/child_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.587285 Nuitka-winsvc-1.6.4/tests/programs/package_missing_init/
--rw-rw-rw-   0        0        0      926 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.594285 Nuitka-winsvc-1.6.4/tests/programs/package_missing_init/some_package/
--rw-rw-rw-   0        0        0      965 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_missing_init/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.604282 Nuitka-winsvc-1.6.4/tests/programs/package_missing_init/some_package/sub_package/
--rw-rw-rw-   0        0        0      977 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.637297 Nuitka-winsvc-1.6.4/tests/programs/package_module_collision/
--rw-rw-rw-   0        0        0      901 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.644292 Nuitka-winsvc-1.6.4/tests/programs/package_module_collision/Something/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_module_collision/Something/__init__.py
--rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_module_collision/something.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.658318 Nuitka-winsvc-1.6.4/tests/programs/package_overload/
--rw-rw-rw-   0        0        0      852 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_overload/Main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.688448 Nuitka-winsvc-1.6.4/tests/programs/package_overload/foo/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_overload/foo/__init__.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_overload/foo/bar.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_overload/foo/bar2.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.706445 Nuitka-winsvc-1.6.4/tests/programs/package_prevents_submodule/
--rw-rw-rw-   0        0        0     2972 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.733459 Nuitka-winsvc-1.6.4/tests/programs/package_prevents_submodule/some_package/
--rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:52.131055 Nuitka-winsvc-1.6.4/tests/programs/package_program/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.761482 Nuitka-winsvc-1.6.4/tests/programs/package_program/PackageAsMain/
--rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_program/PackageAsMain/__init__.py
--rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/package_program/PackageAsMain/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.782447 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/
--rw-rw-rw-   0        0        0     1728 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.793457 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.819453 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.848453 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.868456 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_usage/
--rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.893087 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_usage/package/
--rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
--rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-rw-rw-   0        0        0     1553 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/pkgutil_usage/package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.903089 Nuitka-winsvc-1.6.4/tests/programs/plugin_import/
--rw-rw-rw-   0        0        0      859 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/plugin_import/PluginImportMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.939221 Nuitka-winsvc-1.6.4/tests/programs/plugin_import/some_package/
--rw-rw-rw-   0        0        0      771 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/plugin_import/some_package/__init__.py
--rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/plugin_import/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.956212 Nuitka-winsvc-1.6.4/tests/programs/reimport_main_dynamic/
--rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:58.972213 Nuitka-winsvc-1.6.4/tests/programs/reimport_main_static/
--rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.000219 Nuitka-winsvc-1.6.4/tests/programs/relative_import/
--rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/relative_import/RelativeImportMain.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/relative_import/dircache.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.015213 Nuitka-winsvc-1.6.4/tests/programs/resource_reader37/
--rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.031214 Nuitka-winsvc-1.6.4/tests/programs/resource_reader37/some_package/
--rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.4/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/resource_reader37/some_package/__init__.py
--rw-rw-rw-   0        0        0     6615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/run_all.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.058220 Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/
--rw-rw-rw-   0        0        0     1171 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/pyexpat.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.119215 Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/some_package/__init__.py
--rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/some_package/normal_importing.py
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/some_package/star_importing.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.172129 Nuitka-winsvc-1.6.4/tests/programs/syntax_errors/
--rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/syntax_errors/IndentationErroring.py
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/syntax_errors/SyntaxErroring.py
--rw-rw-rw-   0        0        0     1079 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/syntax_errors/SyntaxErrorsMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.202718 Nuitka-winsvc-1.6.4/tests/programs/unicode_bom/
--rw-rw-rw-   0        0        0      963 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/unicode_bom/unicode_bom.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.219718 Nuitka-winsvc-1.6.4/tests/programs/with space/
--rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/programs/with space/Space Main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.238755 Nuitka-winsvc-1.6.4/tests/reflected/
--rw-rw-rw-   0        0        0    14061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/reflected/compile_itself.py
--rw-rw-rw-   0        0        0     1243 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/run-tests
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.668129 Nuitka-winsvc-1.6.4/tests/standalone/
--rw-rw-rw-   0        0        0     1058 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/BrotliUsing.py
--rw-rw-rw-   0        0        0     2554 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/CtypesUsing.py
--rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/FlaskUsing.py
--rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/GlfwUsing.py
--rw-rw-rw-   0        0        0     1184 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/GtkUsing.py
--rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/HexEncodingTest_2.py
--rw-rw-rw-   0        0        0     1086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/IdnaUsing.py
--rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/LxmlUsing.py
--rw-rw-rw-   0        0        0     1431 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/MatplotlibUsing.py
--rw-rw-rw-   0        0        0     2538 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/MetadataPackagesUsing.py
--rw-rw-rw-   0        0        0     1727 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/NumpyUsing.py
--rw-rw-rw-   0        0        0      947 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/OpenGLUsing.py
--rw-rw-rw-   0        0        0     1379 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PandasUsing.py
--rw-rw-rw-   0        0        0     1066 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PasslibUsing.py
--rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PendulumUsing.py
--rw-rw-rw-   0        0        0     2074 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PkgResourcesRequiresUsing.py
--rw-rw-rw-   0        0        0     1067 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PmwUsing.py
--rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PyQt5Plugins.py
--rw-rw-rw-   0        0        0     1105 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PyQt5SSLSupport.py
--rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PyQt5Using.py
--rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PyQt6Plugins.py
--rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PyQt6Using.py
--rw-rw-rw-   0        0        0     1091 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PySide6Plugins.py
--rw-rw-rw-   0        0        0     1757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/PySide6Using.py
--rw-rw-rw-   0        0        0     1323 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/RsaUsing.py
--rw-rw-rw-   0        0        0      973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/ShlibUsing.py
--rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/SocketUsing.py
--rw-rw-rw-   0        0        0     1941 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/TkInterUsing.py
--rw-rw-rw-   0        0        0     3228 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/Urllib3Using.py
--rw-rw-rw-   0        0        0     1200 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/Win32ComUsing.py
--rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/run_all.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:02:59.676125 Nuitka-winsvc-1.6.4/tests/standalone/zip_importer/
--rw-rw-rw-   0        0        0     1264 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/standalone/zip_importer/ZipImporterMain.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:03:00.101580 Nuitka-winsvc-1.6.4/tests/syntax/
--rw-rw-rw-   0        0        0      811 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/AsyncgenReturn36.py
--rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/BreakWithoutLoop.py
--rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/ClassReturn.py
--rw-rw-rw-   0        0        0      970 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/ClosureDel_2.py
--rw-rw-rw-   0        0        0      849 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/ContinueWithoutLoop.py
--rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/DuplicateArgument.py
--rw-rw-rw-   0        0        0     1111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/ExecWithNesting_2.py
--rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/FutureBraces.py
--rw-rw-rw-   0        0        0      805 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/FutureUnknown.py
--rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/GeneratorExpressions38.py
--rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/GeneratorReturn_2.py
--rw-rw-rw-   0        0        0      792 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/GlobalForParameter.py
--rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/Importing32.py
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/IndentationError.py
--rw-rw-rw-   0        0        0      915 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/LateFutureImport.py
--rw-rw-rw-   0        0        0      841 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/MisplacedFutureImport.py
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/ModuleReturn.py
--rw-rw-rw-   0        0        0      883 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/NonlocalForParameter32.py
--rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/NonlocalNotFound32.py
--rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/StarImportExtra.py
--rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/SyntaxError.py
--rw-rw-rw-   0        0        0      874 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/TryExceptAllNotLast.py
--rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/TryFinallyContinue_37.py
--rw-rw-rw-   0        0        0      776 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/UnpackNoTuple.py
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/UnpackTwoStars32.py
--rw-rw-rw-   0        0        0      793 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/YieldFromInModule.py
--rw-rw-rw-   0        0        0      804 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/YieldInAsync35.py
--rw-rw-rw-   0        0        0      923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/YieldInGenexp38.py
--rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/YieldInModule.py
--rw-rw-rw-   0        0        0     2203 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.4/tests/syntax/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:42.569789 Nuitka-winsvc-1.6.6/
+-rw-rw-rw-   0        0        0   825587 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/Changelog.rst
+-rw-rw-rw-   0        0        0   152515 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/Developer_Manual.rst
+-rw-rw-rw-   0        0        0    11348 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1733 2023-07-03 04:11:23.000000 Nuitka-winsvc-1.6.6/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.283284 Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/
+-rw-rw-rw-   0        0        0     4626 2023-07-03 06:36:32.000000 Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    76624 2023-07-03 06:36:32.000000 Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:36:32.000000 Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      308 2023-07-03 06:36:32.000000 Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-28 09:21:19.000000 Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-07-03 06:36:32.000000 Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 06:36:32.000000 Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4626 2023-07-03 06:36:42.569789 Nuitka-winsvc-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2651 2023-07-03 04:11:21.000000 Nuitka-winsvc-1.6.6/README.md
+-rw-rw-rw-   0        0        0    75940 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.413366 Nuitka-winsvc-1.6.6/bin/
+-rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/bin/autoformat-nuitka-source
+-rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/bin/check-nuitka-with-pylint
+-rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/bin/compare_with_cpython
+-rw-rw-rw-   0        0        0     3079 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/bin/compare_with_xml
+-rw-rw-rw-   0        0        0     1163 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/bin/measure-construct-performance
+-rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/bin/nuitka
+-rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/bin/nuitka-run
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:32.962337 Nuitka-winsvc-1.6.6/doc/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.467105 Nuitka-winsvc-1.6.6/doc/Logo/
+-rw-rw-rw-   0        0        0     7321 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/doc/Logo/Nuitka-Logo-Horizontal.svg
+-rw-rw-rw-   0        0        0     7401 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-rw-rw-   0        0        0    17917 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/doc/Logo/Nuitka-Logo-Vertical.svg
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.497355 Nuitka-winsvc-1.6.6/doc/images/
+-rw-rw-rw-   0        0        0     7585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/doc/images/Nuitka-Logo-Horizontal.png
+-rw-rw-rw-   0        0        0     4452 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/doc/images/Nuitka-Logo-Symbol.png
+-rw-rw-rw-   0        0        0     9828 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/doc/images/Nuitka-Logo-Vertical.png
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.499305 Nuitka-winsvc-1.6.6/lib/
+-rw-rw-rw-   0        0        0     4250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/lib/hints.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.533591 Nuitka-winsvc-1.6.6/misc/
+-rwxrwxrwx   0        0        0      901 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/misc/nuitka-run.bat
+-rwxrwxrwx   0        0        0     1038 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/misc/nuitka.bat
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.651811 Nuitka-winsvc-1.6.6/nuitka/
+-rw-rw-rw-   0        0        0     7331 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/Builtins.py
+-rw-rw-rw-   0        0        0     5437 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/BytecodeCaching.py
+-rw-rw-rw-   0        0        0     3440 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/Bytecodes.py
+-rw-rw-rw-   0        0        0     1884 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/CacheCleanup.py
+-rw-rw-rw-   0        0        0    11148 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/Constants.py
+-rw-rw-rw-   0        0        0     2447 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/Errors.py
+-rw-rw-rw-   0        0        0    37317 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.6/nuitka/MainControl.py
+-rw-rw-rw-   0        0        0     8064 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/ModuleRegistry.py
+-rw-rw-rw-   0        0        0    57087 2023-07-03 04:11:23.000000 Nuitka-winsvc-1.6.6/nuitka/OptionParsing.py
+-rw-rw-rw-   0        0        0    66046 2023-07-03 04:11:22.000000 Nuitka-winsvc-1.6.6/nuitka/Options.py
+-rw-rw-rw-   0        0        0     5022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/OutputDirectories.py
+-rw-rw-rw-   0        0        0    14550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/PostProcessing.py
+-rw-rw-rw-   0        0        0     5770 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/Progress.py
+-rw-rw-rw-   0        0        0     7472 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/PythonFlavors.py
+-rw-rw-rw-   0        0        0     4061 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/PythonOperators.py
+-rw-rw-rw-   0        0        0    12179 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/PythonVersions.py
+-rw-rw-rw-   0        0        0     8514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/Serialization.py
+-rw-rw-rw-   0        0        0     4670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/SourceCodeReferences.py
+-rw-rw-rw-   0        0        0    11235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/Tracing.py
+-rw-rw-rw-   0        0        0     3395 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/TreeXML.py
+-rw-rw-rw-   0        0        0    15235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/Variables.py
+-rw-rw-rw-   0        0        0     2055 2023-07-03 04:01:20.000000 Nuitka-winsvc-1.6.6/nuitka/Version.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/__init__.py
+-rw-rw-rw-   0        0        0     5615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/__main__.py
+-rw-rw-rw-   0        0        0     5295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/__past__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.717238 Nuitka-winsvc-1.6.6/nuitka/build/
+-rw-rw-rw-   0        0        0    33528 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/Backend.scons
+-rw-rw-rw-   0        0        0     8314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/CCompilerVersion.scons
+-rw-rw-rw-   0        0        0     2433 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/DataComposerInterface.py
+-rw-rw-rw-   0        0        0    18807 2023-07-03 04:11:22.000000 Nuitka-winsvc-1.6.6/nuitka/build/Onefile.scons
+-rw-rw-rw-   0        0        0    15698 2023-07-03 04:01:20.000000 Nuitka-winsvc-1.6.6/nuitka/build/SconsCaching.py
+-rw-rw-rw-   0        0        0    30984 2023-07-03 04:11:22.000000 Nuitka-winsvc-1.6.6/nuitka/build/SconsCompilerSettings.py
+-rw-rw-rw-   0        0        0     5527 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/SconsHacks.py
+-rw-rw-rw-   0        0        0    15827 2023-07-03 04:01:20.000000 Nuitka-winsvc-1.6.6/nuitka/build/SconsInterface.py
+-rw-rw-rw-   0        0        0     2361 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/SconsProgress.py
+-rw-rw-rw-   0        0        0    11964 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/build/SconsSpawn.py
+-rw-rw-rw-   0        0        0    24338 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/build/SconsUtils.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:32.966205 Nuitka-winsvc-1.6.6/nuitka/build/include/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.842757 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/
+-rw-rw-rw-   0        0        0     7972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/allocator.h
+-rw-rw-rw-   0        0        0     3423 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/builtins.h
+-rw-rw-rw-   0        0        0     4604 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/calling.h
+-rw-rw-rw-   0        0        0     1977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/checkers.h
+-rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/checksum_tools.h
+-rw-rw-rw-   0        0        0     9571 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-rw-rw-   0        0        0     2002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_cell.h
+-rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-rw-rw-   0        0        0    16949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_frame.h
+-rw-rw-rw-   0        0        0     5972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_function.h
+-rw-rw-rw-   0        0        0     9136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_generator.h
+-rw-rw-rw-   0        0        0     1838 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_method.h
+-rw-rw-rw-   0        0        0     7408 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/constants.h
+-rw-rw-rw-   0        0        0     1293 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/constants_blob.h
+-rw-rw-rw-   0        0        0    34083 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/exceptions.h
+-rw-rw-rw-   0        0        0     3221 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-rw-rw-   0        0        0     6253 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/freelists.h
+-rw-rw-rw-   0        0        0    86326 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/hedley.h
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.969682 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/
+-rw-rw-rw-   0        0        0     3275 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/attributes.h
+-rw-rw-rw-   0        0        0     2663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/boolean.h
+-rw-rw-rw-   0        0        0     1181 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/bytes.h
+-rw-rw-rw-   0        0        0     9335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-rw-rw-   0        0        0    10615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-rw-rw-   0        0        0    13139 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-rw-rw-   0        0        0     1743 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/complex.h
+-rw-rw-rw-   0        0        0    13109 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-rw-rw-   0        0        0     1206 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/floats.h
+-rw-rw-rw-   0        0        0     3674 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-rw-rw-   0        0        0     1798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/indexes.h
+-rw-rw-rw-   0        0        0     2941 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/ints.h
+-rw-rw-rw-   0        0        0     9992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/iterators.h
+-rw-rw-rw-   0        0        0     3411 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/lists.h
+-rw-rw-rw-   0        0        0     1633 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-rw-rw-   0        0        0     1328 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/mappings.h
+-rw-rw-rw-   0        0        0     4573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations.h
+-rw-rw-rw-   0        0        0    12685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-rw-rw-   0        0        0     5641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-rw-rw-   0        0        0     5422 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-rw-rw-   0        0        0     5460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-rw-rw-   0        0        0     2799 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-rw-rw-   0        0        0    15778 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-rw-rw-   0        0        0    13210 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-rw-rw-   0        0        0     5791 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-rw-rw-   0        0        0     4714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-rw-rw-   0        0        0     5824 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-rw-rw-   0        0        0     5438 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-rw-rw-   0        0        0    15100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-rw-rw-   0        0        0     8670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-rw-rw-   0        0        0     3753 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-rw-rw-   0        0        0     4846 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-rw-rw-   0        0        0    10626 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-rw-rw-   0        0        0     9201 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-rw-rw-   0        0        0     5147 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-rw-rw-   0        0        0     4349 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-rw-rw-   0        0        0     4975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-rw-rw-   0        0        0     4826 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-rw-rw-   0        0        0     3297 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/raising.h
+-rw-rw-rw-   0        0        0     2178 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-rw-rw-   0        0        0     1146 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-rw-rw-   0        0        0     1112 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/sequences.h
+-rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/sets.h
+-rw-rw-rw-   0        0        0     8419 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/slices.h
+-rw-rw-rw-   0        0        0     1242 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/strings.h
+-rw-rw-rw-   0        0        0    17575 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-rw-rw-   0        0        0     5720 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/tuples.h
+-rw-rw-rw-   0        0        0    14412 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helpers.h
+-rw-rw-rw-   0        0        0     5375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/importing.h
+-rw-rw-rw-   0        0        0    12979 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/incbin.h
+-rw-rw-rw-   0        0        0    14427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/prelude.h
+-rw-rw-rw-   0        0        0     2870 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/printing.h
+-rw-rw-rw-   0        0        0     1761 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/python_pgo.h
+-rw-rw-rw-   0        0        0     2119 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-rw-rw-   0        0        0     3840 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/threading.h
+-rw-rw-rw-   0        0        0     3144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/tracing.h
+-rw-rw-rw-   0        0        0     2936 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/unfreezing.h
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.007221 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.980430 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/appdirs/
+-rw-rw-rw-   0        0        0     1097 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/appdirs/LICENSE.txt
+-rw-rw-rw-   0        0        0    24824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/appdirs/appdirs.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.992141 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/atomicwrites/
+-rw-rw-rw-   0        0        0     1069 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.994096 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/bin/
+-rw-rw-rw-   0        0        0     1331 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/bin/scons.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:32.971089 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/clcache/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.008740 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/clcache/clcache/
+-rw-rw-rw-   0        0        0     1585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-rw-rw-   0        0        0    65424 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.015581 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/
+-rw-rw-rw-   0        0        0     1491 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.027296 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/
+-rw-rw-rw-   0        0        0      243 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10517 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.041952 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/
+-rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.050738 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/glob2/
+-rw-rw-rw-   0        0        0       82 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-rw-rw-   0        0        0     6859 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-rw-rw-   0        0        0     4463 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-rw-rw-   0        0        0     8304 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/glob2/impl.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.067338 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/
+-rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/LICENSE.rst
+-rw-rw-rw-   0        0        0       85 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.127873 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-rw-rw-   0        0        0     2423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17473 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.144476 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/
+-rw-rw-rw-   0        0        0     1466 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+-rw-rw-rw-   0        0        0       84 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.198183 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:32.992570 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:32.978898 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.261657 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-rw-rw-   0        0        0    47844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    33996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0     8083 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     6938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    17622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7358 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16000 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.267518 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-rw-rw-   0        0        0     4197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   121420 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     4164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    49503 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.295839 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-rw-rw-   0        0        0     1965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-rw-rw-   0        0        0     2736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-rw-rw-   0        0        0     2614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-rw-rw-   0        0        0     8467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.328063 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-rw-rw-   0        0        0     9314 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3131 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     1989 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1718 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1605 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     2170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4179 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1882 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0    14948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    39700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    12950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.343684 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3233 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2011 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    14663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.356376 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-rw-rw-   0        0        0    14029 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    52665 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    40719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    24133 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-rw-rw-   0        0        0    34903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    40510 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.539571 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2166 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-rw-rw-   0        0        0     2859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-rw-rw-   0        0        0    18084 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.552262 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0     9248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    14869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    19499 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    20832 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-rw-rw-   0        0        0     5149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-rw-rw-   0        0        0     2657 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-rw-rw-   0        0        0    31283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2267 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-rw-rw-   0        0        0     2720 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     2796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2147 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2936 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2935 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     2777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0      142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.556184 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-rw-rw-   0        0        0     1844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     4782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-rw-rw-   0        0        0     2025 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-rw-rw-   0        0        0     2256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-rw-rw-   0        0        0     2460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2077 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    18600 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     3328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-rw-rw-   0        0        0     8394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     3953 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2309 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2945 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     6919 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4381 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2168 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    13881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1804 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    11380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    72761 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6841 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     4695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1927 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     2349 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     5992 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13016 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3415 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    48938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.567884 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3007 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11034 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.593275 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-rw-rw-   0        0        0     8120 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     3596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-rw-rw-   0        0        0     1818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-rw-rw-   0        0        0     1742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     2465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-rw-rw-   0        0        0     1776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-rw-rw-   0        0        0    19253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-rw-rw-   0        0        0    44500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-rw-rw-   0        0        0    19664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     7509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:32.984759 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.643077 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-rw-rw-   0        0        0    53545 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    34985 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0    13596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    28403 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    20988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    22350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16068 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9565 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.651866 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-rw-rw-   0        0        0     5239 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   135413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     5758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8354 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.678232 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-rw-rw-   0        0        0    11500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2227 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1767 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1654 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4476 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     4003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    16962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41186 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    13880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.685066 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3812 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.694839 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-rw-rw-   0        0        0    13779 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53260 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    39394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14489 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    35863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    42204 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.924270 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    18207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.939893 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2152 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    10674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    33537 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    21762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    50660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     8618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2226 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2978 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3389 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.941844 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      313 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3631 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3444 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     8494 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.943797 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3686 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2580 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1645 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2189 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1944 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    15791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    26195 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0    13924 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     4041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2351 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2987 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     7808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4956 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     5235 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1847 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    82939 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4904 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1868 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     5335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6756 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3773 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3201 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    53803 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.952588 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4459 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1647 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.958447 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-rw-rw-   0        0        0     6869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0    19816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:32.992570 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:34.999468 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-rw-rw-   0        0        0    56578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-rw-rw-   0        0        0    35213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+-rw-rw-rw-   0        0        0    11061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27408 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7884 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-rw-rw-   0        0        0    21423 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    97269 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-rw-rw-   0        0        0     3979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+-rw-rw-rw-   0        0        0     7515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21937 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.005319 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-rw-rw-   0        0        0     5126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   136271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     6167 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63768 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.038523 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-rw-rw-   0        0        0    12836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4356 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    14831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41983 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-rw-rw-   0        0        0    14673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.052192 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-rw-rw-   0        0        0     7394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     4357 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3546 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     1972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.066856 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-rw-rw-   0        0        0    13597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    42760 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26676 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    36753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-rw-rw-   0        0        0    41191 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.322691 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-rw-rw-   0        0        0     2122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    15570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.346326 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2014 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    13182 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2734 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15027 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    38783 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    22570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4368 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    32724 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     7993 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2141 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     1661 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2893 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-rw-rw-   0        0        0     2889 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.348279 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      343 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3259 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     7461 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0     3379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2377 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2526 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2677 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2206 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2096 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     1954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     1995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    19180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     2588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.353162 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-rw-rw-   0        0        0     4649 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-rw-rw-   0        0        0     7652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-rw-rw-   0        0        0     6064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-rw-rw-   0        0        0     3931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2266 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2900 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     8622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    84784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3576 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2479 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1780 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     1999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1569 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2419 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2429 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6412 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    12548 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     4076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    71693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.361956 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-rw-rw-   0        0        0     6632 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-rw-rw-   0        0        0    15278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.373670 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-rw-rw-   0        0        0     3134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3896 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4672 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    12708 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-rw-rw-   0        0        0      353 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.377576 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-rw-rw-   0        0        0     4307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     3395 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-rw-rw-   0        0        0    21614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9295 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2032 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.401011 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/
+-rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.408823 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-rw-rw-   0        0        0    10126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-rw-rw-   0        0        0     4690 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.000397 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/pkg_resources/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.411753 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-rw-rw-   0        0        0   107452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.002337 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.435733 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-rw-rw-   0        0        0     1591 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-rw-rw-   0        0        0      287 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
+-rw-rw-rw-   0        0        0      307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-rw-rw-   0        0        0      596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-rw-rw-   0        0        0     1106 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-rw-rw-   0        0        0     1376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-rw-rw-   0        0        0     5943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py
+-rw-rw-rw-   0        0        0    10790 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-rw-rw-   0        0        0    57572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-rw-rw-   0        0        0     6948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+-rw-rw-rw-   0        0        0     9533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-rw-rw-   0        0        0      333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/version.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.450380 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.478699 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/
+-rw-rw-rw-   0        0        0    13170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-rw-rw-   0        0        0    28639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2837 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-rw-rw-   0        0        0     2061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-rw-rw-   0        0        0    14184 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-rw-rw-   0        0        0     8999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51277 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.484558 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.509948 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-rw-rw-   0        0        0     9776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4921 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-rw-rw-   0        0        0    25145 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43298 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-rw-rw-   0        0        0     1132 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25542 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-rw-rw-   0        0        0     6746 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-rw-rw-   0        0        0    17711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-rw-rw-   0        0        0     9122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-rw-rw-   0        0        0    52446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4171 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.520693 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.557796 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-rw-rw-   0        0        0     9607 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-rw-rw-   0        0        0    25554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+-rw-rw-rw-   0        0        0    42954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-rw-rw-   0        0        0     1138 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-rw-rw-   0        0        0     6854 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-rw-rw-   0        0        0    14097 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-rw-rw-   0        0        0     8970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.565609 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/
+-rw-rw-rw-   0        0        0     1530 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.590998 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/
+-rw-rw-rw-   0        0        0    18198 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-rw-rw-   0        0        0    10157 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/compiler.h
+-rw-rw-rw-   0        0        0     4455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-rw-rw-   0        0        0    13662 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-rw-rw-   0        0        0     3009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-rw-rw-   0        0        0     2441 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-rw-rw-   0        0        0    34422 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-rw-rw-   0        0        0    14748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-rw-rw-   0        0        0    20216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-rw-rw-   0        0        0    13930 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-rw-rw-   0        0        0    26976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-rw-rw-   0        0        0    11706 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-rw-rw-   0        0        0     2497 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-rw-rw-   0        0        0     3828 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-rw-rw-   0        0        0    15880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.599786 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/
+-rw-rw-rw-   0        0        0    54982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-rw-rw-   0        0        0     9164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-rw-rw-   0        0        0     1321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-rw-rw-   0        0        0    80283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-rw-rw-   0        0        0    66784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-rw-rw-   0        0        0     2253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-rw-rw-   0        0        0     7906 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-rw-   0        0        0   138334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/zstd.h
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.808776 Nuitka-winsvc-1.6.6/nuitka/build/static_src/
+-rw-rw-rw-   0        0        0    82114 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-rw-rw-   0        0        0     8250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledCellType.c
+-rw-rw-rw-   0        0        0    62733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-rw-rw-   0        0        0    70973 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-rw-rw-   0        0        0    35861 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledFrameType.c
+-rw-rw-rw-   0        0        0   100376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledFunctionType.c
+-rw-rw-rw-   0        0        0    60649 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-rw-rw-   0        0        0    48526 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-rw-rw-   0        0        0    21638 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledMethodType.c
+-rw-rw-rw-   0        0        0    18993 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersAllocator.c
+-rw-rw-rw-   0        0        0    32849 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersAttributes.c
+-rw-rw-rw-   0        0        0    21783 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersBuiltin.c
+-rw-rw-rw-   0        0        0   107641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-rw-rw-   0        0        0     3033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersBytes.c
+-rw-rw-rw-   0        0        0    13057 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersCalling.c
+-rw-rw-rw-   0        0        0   470655 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-rw-rw-   0        0        0     1617 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-rw-rw-   0        0        0     2991 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersClasses.c
+-rw-rw-rw-   0        0        0   317872 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-rw-rw-   0        0        0     4673 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-rw-rw-   0        0        0   313003 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-rw-rw-   0        0        0   312414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-rw-rw-   0        0        0   316217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-rw-rw-   0        0        0   315628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-rw-rw-   0        0        0   314618 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-rw-rw-   0        0        0    36068 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-rw-rw-   0        0        0    19313 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-rw-rw-   0        0        0    38364 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersDictionaries.c
+-rw-rw-rw-   0        0        0    24295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-rw-rw-   0        0        0     7035 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersExceptions.c
+-rw-rw-rw-   0        0        0     6668 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersFiles.c
+-rw-rw-rw-   0        0        0    11199 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-rw-rw-   0        0        0     2426 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersFloats.c
+-rw-rw-rw-   0        0        0     1774 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-rw-rw-   0        0        0    14585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersImport.c
+-rw-rw-rw-   0        0        0    13589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersImportHard.c
+-rw-rw-rw-   0        0        0    18433 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersLists.c
+-rw-rw-rw-   0        0        0    13915 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-rw-rw-   0        0        0     1640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersMappings.c
+-rw-rw-rw-   0        0        0     3513 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersMatching.c
+-rw-rw-rw-   0        0        0   181243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-rw-rw-   0        0        0    16700 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-rw-rw-   0        0        0    77782 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+-rw-rw-rw-   0        0        0    67487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-rw-rw-   0        0        0    68748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-rw-rw-   0        0        0     6274 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-rw-rw-   0        0        0    83405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-rw-rw-   0        0        0    13776 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-rw-rw-   0        0        0   183202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-rw-rw-   0        0        0   188514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-rw-rw-   0        0        0     3404 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-rw-rw-   0        0        0    66453 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-rw-rw-   0        0        0    78891 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-rw-rw-   0        0        0     1023 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-rw-rw-   0        0        0    77305 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-rw-rw-   0        0        0    70465 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-rw-rw-   0        0        0    68005 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-rw-rw-   0        0        0   149580 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-rw-rw-   0        0        0     4071 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-rw-rw-   0        0        0    53122 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-rw-rw-   0        0        0    76512 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-rw-rw-   0        0        0    47568 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-rw-rw-   0        0        0    17742 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-rw-rw-   0        0        0   136100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-rw-rw-   0        0        0   142211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-rw-rw-   0        0        0    74142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-rw-rw-   0        0        0    82669 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-rw-rw-   0        0        0    45052 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-rw-rw-   0        0        0    82842 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-rw-rw-   0        0        0    76343 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-rw-rw-   0        0        0     3219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersProfiling.c
+-rw-rw-rw-   0        0        0     3805 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-rw-rw-   0        0        0    15369 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersRaising.c
+-rw-rw-rw-   0        0        0    11926 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-rw-rw-   0        0        0     3730 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersSequences.c
+-rw-rw-rw-   0        0        0     1946 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersSlices.c
+-rw-rw-rw-   0        0        0    26642 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersStrings.c
+-rw-rw-rw-   0        0        0     4037 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersTuples.c
+-rw-rw-rw-   0        0        0     5578 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersTypes.c
+-rw-rw-rw-   0        0        0    11986 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/InspectPatcher.c
+-rw-rw-rw-   0        0        0    41866 2023-07-03 04:01:20.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/MainProgram.c
+-rw-rw-rw-   0        0        0    58634 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-rw-rw-   0        0        0     4537 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-rw-rw-   0        0        0     6427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-rw-rw-   0        0        0    17065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-rw-rw-   0        0        0    36705 2023-07-03 04:11:22.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/OnefileBootstrap.c
+-rw-rw-rw-   0        0        0     7984 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/build/static_src/OnefileSplashScreen.cpp
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.931099 Nuitka-winsvc-1.6.6/nuitka/code_generation/
+-rw-rw-rw-   0        0        0     6414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/AsyncgenCodes.py
+-rw-rw-rw-   0        0        0    10153 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/AttributeCodes.py
+-rw-rw-rw-   0        0        0    21864 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-rw-rw-   0        0        0     2339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/BranchCodes.py
+-rw-rw-rw-   0        0        0    16009 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/BuiltinCodes.py
+-rw-rw-rw-   0        0        0    35905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/CallCodes.py
+-rw-rw-rw-   0        0        0     4896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ClassCodes.py
+-rw-rw-rw-   0        0        0    51116 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/CodeGeneration.py
+-rw-rw-rw-   0        0        0     2375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/CodeHelperSelection.py
+-rw-rw-rw-   0        0        0    14392 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/CodeHelpers.py
+-rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/CodeObjectCodes.py
+-rw-rw-rw-   0        0        0    17570 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ComparisonCodes.py
+-rw-rw-rw-   0        0        0     4446 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-rw-rw-   0        0        0     7335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ConditionalCodes.py
+-rw-rw-rw-   0        0        0     6539 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ConstantCodes.py
+-rw-rw-rw-   0        0        0    31186 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/Contexts.py
+-rw-rw-rw-   0        0        0     8484 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/CoroutineCodes.py
+-rw-rw-rw-   0        0        0     1574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/CtypesCodes.py
+-rw-rw-rw-   0        0        0    28478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/DictCodes.py
+-rw-rw-rw-   0        0        0     2125 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/Emission.py
+-rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ErrorCodes.py
+-rw-rw-rw-   0        0        0    12304 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/EvalCodes.py
+-rw-rw-rw-   0        0        0     8975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ExceptionCodes.py
+-rw-rw-rw-   0        0        0     7350 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-rw-rw-   0        0        0     2093 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ExpressionCodes.py
+-rw-rw-rw-   0        0        0    17725 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/FrameCodes.py
+-rw-rw-rw-   0        0        0    27345 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/FunctionCodes.py
+-rw-rw-rw-   0        0        0     7690 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/GeneratorCodes.py
+-rw-rw-rw-   0        0        0     5721 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/GlobalConstants.py
+-rw-rw-rw-   0        0        0     6911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-rw-rw-   0        0        0     1794 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/IdCodes.py
+-rw-rw-rw-   0        0        0    13318 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ImportCodes.py
+-rw-rw-rw-   0        0        0     1396 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/Indentation.py
+-rw-rw-rw-   0        0        0     1506 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/IndexCodes.py
+-rw-rw-rw-   0        0        0     1033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/InjectCCodes.py
+-rw-rw-rw-   0        0        0     3432 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/IntegerCodes.py
+-rw-rw-rw-   0        0        0    12010 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/IteratorCodes.py
+-rw-rw-rw-   0        0        0     2022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/LabelCodes.py
+-rw-rw-rw-   0        0        0     2612 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/LineNumberCodes.py
+-rw-rw-rw-   0        0        0    15906 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ListCodes.py
+-rw-rw-rw-   0        0        0     6375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/LoaderCodes.py
+-rw-rw-rw-   0        0        0     9951 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/LocalsDictCodes.py
+-rw-rw-rw-   0        0        0     3135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/LoopCodes.py
+-rw-rw-rw-   0        0        0     1597 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/MatchCodes.py
+-rw-rw-rw-   0        0        0     6291 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ModuleCodes.py
+-rw-rw-rw-   0        0        0     8118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/Namify.py
+-rw-rw-rw-   0        0        0    12777 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/OperationCodes.py
+-rw-rw-rw-   0        0        0    28231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/PackageResourceCodes.py
+-rw-rw-rw-   0        0        0     3021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/PrintCodes.py
+-rw-rw-rw-   0        0        0     5474 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/PythonAPICodes.py
+-rw-rw-rw-   0        0        0    13095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/RaisingCodes.py
+-rw-rw-rw-   0        0        0     3443 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/Reports.py
+-rw-rw-rw-   0        0        0     5234 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/ReturnCodes.py
+-rw-rw-rw-   0        0        0     6517 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/SetCodes.py
+-rw-rw-rw-   0        0        0    13949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/SliceCodes.py
+-rw-rw-rw-   0        0        0     9809 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/StringCodes.py
+-rw-rw-rw-   0        0        0     8188 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/SubscriptCodes.py
+-rw-rw-rw-   0        0        0    11176 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/TryCodes.py
+-rw-rw-rw-   0        0        0     3786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/TupleCodes.py
+-rw-rw-rw-   0        0        0    14717 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/VariableCodes.py
+-rw-rw-rw-   0        0        0     9121 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/VariableDeclarations.py
+-rw-rw-rw-   0        0        0     8099 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/YieldCodes.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.948689 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/
+-rw-rw-rw-   0        0        0     6069 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeBases.py
+-rw-rw-rw-   0        0        0     3399 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-rw-rw-   0        0        0     1804 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-rw-rw-   0        0        0     1378 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-rw-rw-   0        0        0     3610 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-rw-rw-   0        0        0     5128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-rw-rw-   0        0        0     5211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-rw-rw-   0        0        0     3955 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-rw-rw-   0        0        0    19628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-rw-rw-   0        0        0     2852 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:35.968221 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/
+-rw-rw-rw-   0        0        0     2845 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-rw-rw-   0        0        0     5865 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-rw-rw-   0        0        0     2921 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-rw-rw-   0        0        0     2290 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-rw-rw-   0        0        0     6339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-rw-rw-   0        0        0     3321 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-rw-rw-   0        0        0     3306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-rw-rw-   0        0        0     2335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-rw-rw-   0        0        0     4217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-rw-rw-   0        0        0    21441 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-rw-rw-   0        0        0     6640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-rw-rw-   0        0        0     2475 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.563914 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/
+-rw-rw-rw-   0        0        0    11231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-rw-rw-   0        0        0     5847 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-rw-rw-   0        0        0    23760 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-rw-rw-   0        0        0     5238 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-rw-rw-   0        0        0     1843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-rw-rw-   0        0        0     2817 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-rw-rw-   0        0        0    12819 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-rw-rw-   0        0        0     2044 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-rw-rw-   0        0        0     2762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-rw-rw-   0        0        0     1544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-rw-rw-   0        0        0     7197 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-rw-rw-   0        0        0    12850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-rw-rw-   0        0        0     4288 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-rw-rw-   0        0        0     2088 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-rw-rw-   0        0        0     2118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-rw-rw-   0        0        0     3933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-rw-rw-   0        0        0     7407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-rw-rw-   0        0        0     4292 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-rw-rw-   0        0        0     3860 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-rw-rw-   0        0        0     4487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-rw-rw-   0        0        0    11579 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-rw-rw-   0        0        0    19317 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-rw-rw-   0        0        0     2843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-rw-rw-   0        0        0     3635 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-rw-rw-   0        0        0    11102 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-rw-rw-   0        0        0    15380 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-rw-rw-   0        0        0     2979 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-rw-rw-   0        0        0    10421 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-rw-rw-   0        0        0     2557 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-rw-rw-   0        0        0     3020 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-rw-rw-   0        0        0     2984 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-rw-rw-   0        0        0     3173 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.573669 Nuitka-winsvc-1.6.6/nuitka/containers/
+-rw-rw-rw-   0        0        0     1435 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/containers/Namedtuples.py
+-rw-rw-rw-   0        0        0     6553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/containers/OrderedDicts.py
+-rw-rw-rw-   0        0        0      554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/containers/OrderedSets.py
+-rw-rw-rw-   0        0        0     4397 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/containers/OrderedSetsFallback.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.578548 Nuitka-winsvc-1.6.6/nuitka/distutils/
+-rw-rw-rw-   0        0        0     1964 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/distutils/Build.py
+-rw-rw-rw-   0        0        0    14219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/distutils/DistutilCommands.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/distutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.584406 Nuitka-winsvc-1.6.6/nuitka/finalizations/
+-rw-rw-rw-   0        0        0     1224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/finalizations/Finalization.py
+-rw-rw-rw-   0        0        0     6110 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/finalizations/FinalizeMarkups.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/finalizations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.601513 Nuitka-winsvc-1.6.6/nuitka/freezer/
+-rw-rw-rw-   0        0        0     7311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/DependsExe.py
+-rw-rw-rw-   0        0        0     2584 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/DllDependenciesCommon.py
+-rw-rw-rw-   0        0        0    10811 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/DllDependenciesMacOS.py
+-rw-rw-rw-   0        0        0     7211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/DllDependenciesPosix.py
+-rw-rw-rw-   0        0        0     6620 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/DllDependenciesWin32.py
+-rw-rw-rw-   0        0        0    17336 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/IncludedDataFiles.py
+-rw-rw-rw-   0        0        0     9492 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/IncludedEntryPoints.py
+-rw-rw-rw-   0        0        0     9980 2023-07-03 04:11:22.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/Onefile.py
+-rw-rw-rw-   0        0        0    26319 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/Standalone.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/freezer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.616160 Nuitka-winsvc-1.6.6/nuitka/importing/
+-rw-rw-rw-   0        0        0    11007 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.6/nuitka/importing/IgnoreListing.py
+-rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/importing/ImportCache.py
+-rw-rw-rw-   0        0        0     6455 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/importing/ImportResolving.py
+-rw-rw-rw-   0        0        0    28463 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/importing/Importing.py
+-rw-rw-rw-   0        0        0     4738 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/importing/PreloadedPackages.py
+-rw-rw-rw-   0        0        0    16375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/importing/Recursion.py
+-rw-rw-rw-   0        0        0    10981 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/importing/StandardLibrary.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/importing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.745651 Nuitka-winsvc-1.6.6/nuitka/nodes/
+-rw-rw-rw-   0        0        0     3637 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/AsyncgenNodes.py
+-rw-rw-rw-   0        0        0     4082 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/AttributeLookupNodes.py
+-rw-rw-rw-   0        0        0    12004 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/AttributeNodes.py
+-rw-rw-rw-   0        0        0   378745 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/AttributeNodesGenerated.py
+-rw-rw-rw-   0        0        0     3823 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinAllNodes.py
+-rw-rw-rw-   0        0        0     4098 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinAnyNodes.py
+-rw-rw-rw-   0        0        0     2496 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinComplexNodes.py
+-rw-rw-rw-   0        0        0     1698 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-rw-rw-   0        0        0     4694 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinDictNodes.py
+-rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinFormatNodes.py
+-rw-rw-rw-   0        0        0     2142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinHashNodes.py
+-rw-rw-rw-   0        0        0     5334 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-rw-rw-   0        0        0    12723 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-rw-rw-   0        0        0     1996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinLenNodes.py
+-rw-rw-rw-   0        0        0     3606 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinNextNodes.py
+-rw-rw-rw-   0        0        0     3240 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinOpenNodes.py
+-rw-rw-rw-   0        0        0   245536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-rw-rw-   0        0        0    18589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinRangeNodes.py
+-rw-rw-rw-   0        0        0     9067 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinRefNodes.py
+-rw-rw-rw-   0        0        0     3307 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinSumNodes.py
+-rw-rw-rw-   0        0        0    13543 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinTypeNodes.py
+-rw-rw-rw-   0        0        0     1573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinVarsNodes.py
+-rw-rw-rw-   0        0        0    26113 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/BytesNodes.py
+-rw-rw-rw-   0        0        0     6478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/CallNodes.py
+-rw-rw-rw-   0        0        0     1550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/Checkers.py
+-rw-rw-rw-   0        0        0   605501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ChildrenHavingMixins.py
+-rw-rw-rw-   0        0        0     8448 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ClassNodes.py
+-rw-rw-rw-   0        0        0     6585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/CodeObjectSpecs.py
+-rw-rw-rw-   0        0        0    21683 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ComparisonNodes.py
+-rw-rw-rw-   0        0        0    30314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ConditionalNodes.py
+-rw-rw-rw-   0        0        0    46536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ConstantRefNodes.py
+-rw-rw-rw-   0        0        0    12213 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ContainerMakingNodes.py
+-rw-rw-rw-   0        0        0     2834 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ContainerOperationNodes.py
+-rw-rw-rw-   0        0        0     4581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/CoroutineNodes.py
+-rw-rw-rw-   0        0        0     1714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/CtypesNodes.py
+-rw-rw-rw-   0        0        0    51021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/DictionaryNodes.py
+-rw-rw-rw-   0        0        0     7856 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ExceptionNodes.py
+-rw-rw-rw-   0        0        0     7317 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ExecEvalNodes.py
+-rw-rw-rw-   0        0        0    44996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ExpressionBases.py
+-rw-rw-rw-   0        0        0    45091 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-rw-rw-   0        0        0    21278 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ExpressionShapeMixins.py
+-rw-rw-rw-   0        0        0    12156 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/FrameNodes.py
+-rw-rw-rw-   0        0        0     3544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/FunctionAttributeNodes.py
+-rw-rw-rw-   0        0        0    39803 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/FunctionNodes.py
+-rw-rw-rw-   0        0        0     5376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/FutureSpecs.py
+-rw-rw-rw-   0        0        0     6256 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/GeneratorNodes.py
+-rw-rw-rw-   0        0        0     6850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-rw-rw-   0        0        0    74177 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/HardImportNodesGenerated.py
+-rw-rw-rw-   0        0        0     5511 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ImportHardNodes.py
+-rw-rw-rw-   0        0        0    45692 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ImportNodes.py
+-rw-rw-rw-   0        0        0     2733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/IndicatorMixins.py
+-rw-rw-rw-   0        0        0     1502 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/InjectCNodes.py
+-rw-rw-rw-   0        0        0    11228 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/IterationHandles.py
+-rw-rw-rw-   0        0        0    11002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/KeyValuePairNodes.py
+-rw-rw-rw-   0        0        0    16320 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ListOperationNodes.py
+-rw-rw-rw-   0        0        0    23094 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/LocalsDictNodes.py
+-rw-rw-rw-   0        0        0    14922 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/LocalsScopes.py
+-rw-rw-rw-   0        0        0    15581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/LoopNodes.py
+-rw-rw-rw-   0        0        0     1712 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/MatchNodes.py
+-rw-rw-rw-   0        0        0     6534 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ModuleAttributeNodes.py
+-rw-rw-rw-   0        0        0    30829 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ModuleNodes.py
+-rw-rw-rw-   0        0        0    24899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/NodeBases.py
+-rw-rw-rw-   0        0        0    15128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/NodeMakingHelpers.py
+-rw-rw-rw-   0        0        0     5550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/NodeMetaClasses.py
+-rw-rw-rw-   0        0        0    31894 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/OperatorNodes.py
+-rw-rw-rw-   0        0        0     9134 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/OperatorNodesUnary.py
+-rw-rw-rw-   0        0        0     4202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/OsSysNodes.py
+-rw-rw-rw-   0        0        0    12442 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/OutlineNodes.py
+-rw-rw-rw-   0        0        0    31330 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/PackageMetadataNodes.py
+-rw-rw-rw-   0        0        0     4464 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/PackageResourceNodes.py
+-rw-rw-rw-   0        0        0     3407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/PrintNodes.py
+-rw-rw-rw-   0        0        0     6772 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/ReturnNodes.py
+-rw-rw-rw-   0        0        0     4715 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/SideEffectNodes.py
+-rw-rw-rw-   0        0        0    12501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/SliceNodes.py
+-rw-rw-rw-   0        0        0    94880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/StatementBasesGenerated.py
+-rw-rw-rw-   0        0        0     9430 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/StatementNodes.py
+-rw-rw-rw-   0        0        0    28658 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/StrNodes.py
+-rw-rw-rw-   0        0        0     3504 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/StringConcatenationNodes.py
+-rw-rw-rw-   0        0        0     8640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/SubscriptNodes.py
+-rw-rw-rw-   0        0        0    17853 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/TryNodes.py
+-rw-rw-rw-   0        0        0     2405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/TypeMatchNodes.py
+-rw-rw-rw-   0        0        0    10911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/TypeNodes.py
+-rw-rw-rw-   0        0        0    39522 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/VariableAssignNodes.py
+-rw-rw-rw-   0        0        0    10746 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/VariableDelNodes.py
+-rw-rw-rw-   0        0        0     4574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/VariableNameNodes.py
+-rw-rw-rw-   0        0        0    30982 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/VariableRefNodes.py
+-rw-rw-rw-   0        0        0     4748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/VariableReleaseNodes.py
+-rw-rw-rw-   0        0        0     3902 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/YieldNodes.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.751512 Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/
+-rw-rw-rw-   0        0        0   156243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-rw-rw-   0        0        0     4387 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-rw-rw-   0        0        0     4567 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/ShapeMixins.py
+-rw-rw-rw-   0        0        0    42374 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/StandardShapes.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.767480 Nuitka-winsvc-1.6.6/nuitka/optimizations/
+-rw-rw-rw-   0        0        0     3279 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/optimizations/BytecodeDemotion.py
+-rw-rw-rw-   0        0        0     3920 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/optimizations/FunctionInlining.py
+-rw-rw-rw-   0        0        0     2144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/optimizations/Graphs.py
+-rw-rw-rw-   0        0        0    10762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/optimizations/Optimization.py
+-rw-rw-rw-   0        0        0    52058 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.6/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-rw-rw-   0        0        0     2272 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/optimizations/Tags.py
+-rw-rw-rw-   0        0        0    40896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/optimizations/TraceCollections.py
+-rw-rw-rw-   0        0        0    23977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/optimizations/ValueTraces.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/optimizations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.770413 Nuitka-winsvc-1.6.6/nuitka/pgo/
+-rw-rw-rw-   0        0        0     4663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/pgo/PGO.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/pgo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.778222 Nuitka-winsvc-1.6.6/nuitka/plugins/
+-rw-rw-rw-   0        0        0    40180 2023-07-03 04:01:20.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/PluginBase.py
+-rw-rw-rw-   0        0        0    56200 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/Plugins.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.843794 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/
+-rw-rw-rw-   0        0        0    19102 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-rw-rw-   0        0        0     3460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-rw-rw-   0        0        0     9939 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-rw-rw-   0        0        0     4404 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/DelvewheelPlugin.py
+-rw-rw-rw-   0        0        0     5675 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/DillPlugin.py
+-rw-rw-rw-   0        0        0    13757 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-rw-rw-   0        0        0     2062 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/EnumPlugin.py
+-rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/EventletPlugin.py
+-rw-rw-rw-   0        0        0     1880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/GeventPlugin.py
+-rw-rw-rw-   0        0        0     3482 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/GiPlugin.py
+-rw-rw-rw-   0        0        0     5027 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/GlfwPlugin.py
+-rw-rw-rw-   0        0        0    18335 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/ImplicitImports.py
+-rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/KivyPlugin.py
+-rw-rw-rw-   0        0        0     7258 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-rw-rw-   0        0        0     6667 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-rw-rw-   0        0        0     1187 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/NumpyPlugin.py
+-rw-rw-rw-   0        0        0     6554 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-rw-rw-   0        0        0     1917 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PbrPlugin.py
+-rw-rw-rw-   0        0        0     4665 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-rw-rw-   0        0        0     6992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PmwPlugin.py
+-rw-rw-rw-   0        0        0    50023 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-rw-rw-   0        0        0     2933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-rw-rw-   0        0        0     1160 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-rw-rw-   0        0        0    12180 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TkinterPlugin.py
+-rw-rw-rw-   0        0        0     1140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TorchPlugin.py
+-rw-rw-rw-   0        0        0     9855 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TransformersPlugin.py
+-rw-rw-rw-   0        0        0     3175 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TrioPlugin.py
+-rw-rw-rw-   0        0        0     5640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/UpxPlugin.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/__init__.py
+-rw-rw-rw-   0        0        0   153198 2023-07-03 04:01:20.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     2221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.861380 Nuitka-winsvc-1.6.6/nuitka/reports/
+-rw-rw-rw-   0        0        0     2209 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/reports/LicenseReport.rst.j2
+-rw-rw-rw-   0        0        0    17538 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/reports/Reports.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.877974 Nuitka-winsvc-1.6.6/nuitka/specs/
+-rw-rw-rw-   0        0        0     5911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-rw-rw-   0        0        0     2786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-rw-rw-   0        0        0     2541 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-rw-rw-   0        0        0    26455 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinParameterSpecs.py
+-rw-rw-rw-   0        0        0     6065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-rw-rw-   0        0        0     4802 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-rw-rw-   0        0        0     5133 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/HardImportSpecs.py
+-rw-rw-rw-   0        0        0    18740 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/ParameterSpecs.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/specs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.881880 Nuitka-winsvc-1.6.6/nuitka/tools/
+-rw-rw-rw-   0        0        0     1603 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/Basics.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.882856 Nuitka-winsvc-1.6.6/nuitka/tools/commercial/
+-rw-rw-rw-   0        0        0      815 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/commercial/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.890670 Nuitka-winsvc-1.6.6/nuitka/tools/data_composer/
+-rw-rw-rw-   0        0        0    14054 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/data_composer/DataComposer.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/data_composer/__init__.py
+-rw-rw-rw-   0        0        0     1306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/data_composer/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.897502 Nuitka-winsvc-1.6.6/nuitka/tools/environments/
+-rw-rw-rw-   0        0        0     2449 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/environments/CreateEnvironment.py
+-rw-rw-rw-   0        0        0     3735 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/environments/Virtualenv.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/environments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.899455 Nuitka-winsvc-1.6.6/nuitka/tools/general/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/general/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.903105 Nuitka-winsvc-1.6.6/nuitka/tools/general/dll_report/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/general/dll_report/__init__.py
+-rw-rw-rw-   0        0        0     2366 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/general/dll_report/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.908920 Nuitka-winsvc-1.6.6/nuitka/tools/general/find_module/
+-rw-rw-rw-   0        0        0     3798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/general/find_module/FindModuleCode.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/general/find_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.913805 Nuitka-winsvc-1.6.6/nuitka/tools/onefile_compressor/
+-rw-rw-rw-   0        0        0    10194 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/onefile_compressor/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/onefile_compressor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.916734 Nuitka-winsvc-1.6.6/nuitka/tools/profiler/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/profiler/__init__.py
+-rw-rw-rw-   0        0        0     2529 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/profiler/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.920638 Nuitka-winsvc-1.6.6/nuitka/tools/scanning/
+-rw-rw-rw-   0        0        0     3344 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/scanning/DisplayPackageData.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/scanning/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.930404 Nuitka-winsvc-1.6.6/nuitka/tools/specialize/
+-rw-rw-rw-   0        0        0    51143 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-rw-rw-   0        0        0     7685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/specialize/Common.py
+-rw-rw-rw-   0        0        0    39625 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/specialize/SpecializeC.py
+-rw-rw-rw-   0        0        0    33585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/specialize/SpecializePython.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.6/nuitka/tools/specialize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.941146 Nuitka-winsvc-1.6.6/nuitka/tools/testing/
+-rw-rw-rw-   0        0        0    55396 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/Common.py
+-rw-rw-rw-   0        0        0     1483 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/Constructs.py
+-rw-rw-rw-   0        0        0     8940 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/OutputComparison.py
+-rw-rw-rw-   0        0        0     1278 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/Pythons.py
+-rw-rw-rw-   0        0        0     7888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/RuntimeTracing.py
+-rw-rw-rw-   0        0        0     5371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/SearchModes.py
+-rw-rw-rw-   0        0        0     3375 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/Valgrind.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.944074 Nuitka-winsvc-1.6.6/nuitka/tools/testing/check_reference_counts/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/check_reference_counts/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.946036 Nuitka-winsvc-1.6.6/nuitka/tools/testing/compare_with_cpython/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-rw-rw-   0        0        0    29429 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/compare_with_cpython/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.949944 Nuitka-winsvc-1.6.6/nuitka/tools/testing/find_sxs_modules/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/find_sxs_modules/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/find_sxs_modules/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.951896 Nuitka-winsvc-1.6.6/nuitka/tools/testing/measure_construct_performance/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-rw-rw-   0        0        0     8755 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/measure_construct_performance/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.955797 Nuitka-winsvc-1.6.6/nuitka/tools/testing/run_nuitka_tests/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/run_nuitka_tests/__init__.py
+-rw-rw-rw-   0        0        0    36321 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/testing/run_nuitka_tests/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:36.959698 Nuitka-winsvc-1.6.6/nuitka/tools/watch/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/watch/__init__.py
+-rw-rw-rw-   0        0        0     9503 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tools/watch/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:37.005606 Nuitka-winsvc-1.6.6/nuitka/tree/
+-rw-rw-rw-   0        0        0    47126 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/Building.py
+-rw-rw-rw-   0        0        0    74608 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-rw-rw-   0        0        0     1700 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/Extractions.py
+-rw-rw-rw-   0        0        0     2572 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/InternalModule.py
+-rw-rw-rw-   0        0        0     1511 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/Operations.py
+-rw-rw-rw-   0        0        0     2807 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationAssertStatements.py
+-rw-rw-rw-   0        0        0    42768 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-rw-rw-   0        0        0     2948 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-rw-rw-   0        0        0    11693 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationCallExpressions.py
+-rw-rw-rw-   0        0        0    15072 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationClasses.py
+-rw-rw-rw-   0        0        0    37638 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationClasses3.py
+-rw-rw-rw-   0        0        0     6430 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-rw-rw-   0        0        0    22111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationContractionExpressions.py
+-rw-rw-rw-   0        0        0    11061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-rw-rw-   0        0        0    14607 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationExecStatements.py
+-rw-rw-rw-   0        0        0     7782 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationForLoopStatements.py
+-rw-rw-rw-   0        0        0    26215 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationFunctionStatements.py
+-rw-rw-rw-   0        0        0    13437 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationImportStatements.py
+-rw-rw-rw-   0        0        0     6577 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-rw-rw-   0        0        0    20962 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationMatchStatements.py
+-rw-rw-rw-   0        0        0     2409 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationMultidist.py
+-rw-rw-rw-   0        0        0     8194 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationNamespacePackages.py
+-rw-rw-rw-   0        0        0     4658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationPrintStatements.py
+-rw-rw-rw-   0        0        0    15371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationSequenceCreation.py
+-rw-rw-rw-   0        0        0     4824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-rw-rw-   0        0        0    14615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-rw-rw-   0        0        0     6982 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-rw-rw-   0        0        0     5674 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-rw-rw-   0        0        0    14341 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationWithStatements.py
+-rw-rw-rw-   0        0        0     3088 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationYieldExpressions.py
+-rw-rw-rw-   0        0        0    12746 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/SourceHandling.py
+-rw-rw-rw-   0        0        0     3757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/SyntaxErrors.py
+-rw-rw-rw-   0        0        0    22973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/TreeHelpers.py
+-rw-rw-rw-   0        0        0    20012 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/VariableClosure.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:37.046616 Nuitka-winsvc-1.6.6/nuitka/utils/
+-rw-rw-rw-   0        0        0     2655 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/AppDirs.py
+-rw-rw-rw-   0        0        0     3248 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/CStrings.py
+-rw-rw-rw-   0        0        0     3653 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/CommandLineOptions.py
+-rw-rw-rw-   0        0        0     4297 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Distributions.py
+-rw-rw-rw-   0        0        0     5794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Download.py
+-rw-rw-rw-   0        0        0    12376 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Execution.py
+-rw-rw-rw-   0        0        0    36129 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/FileOperations.py
+-rw-rw-rw-   0        0        0     2885 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Hashing.py
+-rw-rw-rw-   0        0        0     2362 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Images.py
+-rw-rw-rw-   0        0        0     6816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Importing.py
+-rw-rw-rw-   0        0        0     8149 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/InstalledPythons.py
+-rw-rw-rw-   0        0        0     2224 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/InstanceCounters.py
+-rw-rw-rw-   0        0        0     4336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Jinja2.py
+-rw-rw-rw-   0        0        0     1238 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Json.py
+-rw-rw-rw-   0        0        0     4304 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.6/nuitka/utils/MacOSApp.py
+-rw-rw-rw-   0        0        0     5040 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/MemoryUsage.py
+-rw-rw-rw-   0        0        0     9057 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/ModuleNames.py
+-rw-rw-rw-   0        0        0     4309 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/ReExecute.py
+-rw-rw-rw-   0        0        0     3815 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Rest.py
+-rw-rw-rw-   0        0        0    22714 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/SharedLibraries.py
+-rw-rw-rw-   0        0        0     3664 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Shebang.py
+-rw-rw-rw-   0        0        0     2591 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Signing.py
+-rw-rw-rw-   0        0        0     6207 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/StaticLibraries.py
+-rw-rw-rw-   0        0        0     2602 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/ThreadedExecutor.py
+-rw-rw-rw-   0        0        0     2772 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Timing.py
+-rw-rw-rw-   0        0        0    10826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Utils.py
+-rw-rw-rw-   0        0        0    10574 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/WindowsFileUsage.py
+-rw-rw-rw-   0        0        0    19540 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/WindowsResources.py
+-rw-rw-rw-   0        0        0     6108 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/Yaml.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/nuitka/utils/__init__.py
+-rw-rw-rw-   0        0        0      834 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:36:42.570765 Nuitka-winsvc-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0    15001 2023-07-03 04:11:22.000000 Nuitka-winsvc-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:37.053454 Nuitka-winsvc-1.6.6/tests/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.282161 Nuitka-winsvc-1.6.6/tests/basics/
+-rw-rw-rw-   0        0        0     1766 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/AssertsTest.py
+-rw-rw-rw-   0        0        0     5934 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/AssignmentsTest.py
+-rw-rw-rw-   0        0        0     5866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/AssignmentsTest32.py
+-rw-rw-rw-   0        0        0     4055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/BranchingTest.py
+-rw-rw-rw-   0        0        0     1104 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/BuiltinOverload.py
+-rw-rw-rw-   0        0        0     3749 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/BuiltinSuperTest.py
+-rw-rw-rw-   0        0        0    17080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/BuiltinsTest.py
+-rw-rw-rw-   0        0        0      866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ClassMinimalTest.py
+-rw-rw-rw-   0        0        0     4764 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ClassesTest.py
+-rw-rw-rw-   0        0        0     3414 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ClassesTest32.py
+-rw-rw-rw-   0        0        0     1406 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ClassesTest34.py
+-rw-rw-rw-   0        0        0     4698 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ComparisonChainsTest.py
+-rw-rw-rw-   0        0        0     4639 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ConstantsTest.py
+-rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ConstantsTest27.py
+-rw-rw-rw-   0        0        0     1628 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/DecoratorsTest.py
+-rw-rw-rw-   0        0        0     2317 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/DefaultParametersTest.py
+-rw-rw-rw-   0        0        0     1127 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/DoubleDeletionsTest.py
+-rw-rw-rw-   0        0        0      806 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/EmptyModuleTest.py
+-rw-rw-rw-   0        0        0    14387 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ExceptionRaisingTest.py
+-rw-rw-rw-   0        0        0      961 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ExceptionRaisingTest32.py
+-rw-rw-rw-   0        0        0     1458 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ExceptionRaisingTest33.py
+-rw-rw-rw-   0        0        0     6747 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ExecEvalTest.py
+-rw-rw-rw-   0        0        0     1417 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ExtremeClosureTest.py
+-rw-rw-rw-   0        0        0     1658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/FunctionObjectsTest.py
+-rw-rw-rw-   0        0        0    12335 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/FunctionsTest.py
+-rw-rw-rw-   0        0        0     3603 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/FunctionsTest32.py
+-rw-rw-rw-   0        0        0     2627 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/FunctionsTest_2.py
+-rw-rw-rw-   0        0        0      890 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/FutureTest32.py
+-rw-rw-rw-   0        0        0     5809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/GeneratorExpressionsTest.py
+-rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/GeneratorExpressionsTest_37.py
+-rw-rw-rw-   0        0        0     3824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/GlobalStatementTest.py
+-rw-rw-rw-   0        0        0     1286 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/HelloWorldTest_2.py
+-rw-rw-rw-   0        0        0     2469 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ImportingTest.py
+-rw-rw-rw-   0        0        0     1296 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/InplaceOperationsTest.py
+-rw-rw-rw-   0        0        0     4227 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/InspectionTest.py
+-rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/InspectionTest_35.py
+-rw-rw-rw-   0        0        0     1618 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/InspectionTest_36.py
+-rw-rw-rw-   0        0        0     1671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/LambdasTest.py
+-rw-rw-rw-   0        0        0     2731 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/LateClosureAssignmentTest.py
+-rw-rw-rw-   0        0        0     2923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ListContractionsTest.py
+-rw-rw-rw-   0        0        0     3329 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/LoopingTest.py
+-rw-rw-rw-   0        0        0     1536 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/MainProgramsTest.py
+-rw-rw-rw-   0        0        0     1925 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ModuleAttributesTest.py
+-rw-rw-rw-   0        0        0     1988 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/OperatorsTest.py
+-rw-rw-rw-   0        0        0    14903 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/OrderChecksTest.py
+-rw-rw-rw-   0        0        0     1827 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/OrderChecksTest27.py
+-rw-rw-rw-   0        0        0     1452 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/OverflowFunctionsTest_2.py
+-rw-rw-rw-   0        0        0     5853 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ParameterErrorsTest.py
+-rw-rw-rw-   0        0        0     1899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ParameterErrorsTest32.py
+-rw-rw-rw-   0        0        0      863 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/PrintFutureTest.py
+-rw-rw-rw-   0        0        0     1413 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/PrintingTest_2.py
+-rw-rw-rw-   0        0        0      878 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/RecursionTest.py
+-rw-rw-rw-   0        0        0    23840 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest.py
+-rw-rw-rw-   0        0        0     2076 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest27.py
+-rw-rw-rw-   0        0        0     7819 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest33.py
+-rw-rw-rw-   0        0        0     4902 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest35.py
+-rw-rw-rw-   0        0        0     5092 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest36.py
+-rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest_2.py
+-rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/SlotsTest.py
+-rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/ThreadedGeneratorsTest.py
+-rw-rw-rw-   0        0        0    22966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/TrickAssignmentsTest32.py
+-rw-rw-rw-   0        0        0     1541 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/TrickAssignmentsTest35.py
+-rw-rw-rw-   0        0        0     1788 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/TrickAssignmentsTest_2.py
+-rw-rw-rw-   0        0        0     2086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/TryContinueFinallyTest.py
+-rw-rw-rw-   0        0        0     2212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/TryExceptContinueTest.py
+-rw-rw-rw-   0        0        0     2275 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/TryExceptFinallyTest.py
+-rw-rw-rw-   0        0        0     2304 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/TryExceptFramesTest.py
+-rw-rw-rw-   0        0        0     2842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/TryReturnFinallyTest.py
+-rw-rw-rw-   0        0        0     2328 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/TryYieldFinallyTest.py
+-rw-rw-rw-   0        0        0     1093 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/UnicodeTest.py
+-rw-rw-rw-   0        0        0     1877 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/UnpackingTest35.py
+-rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/VarargsTest.py
+-rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/WithStatementsTest.py
+-rw-rw-rw-   0        0        0     3070 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/YieldFromTest33.py
+-rw-rw-rw-   0        0        0     3821 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/run_all.py
+-rw-rw-rw-   0        0        0     2271 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/basics/run_xml.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.331963 Nuitka-winsvc-1.6.6/tests/onefile/
+-rw-rw-rw-   0        0        0     1213 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/onefile/HelloWorldTest.py
+-rw-rw-rw-   0        0        0     1307 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/onefile/KeyboardInterruptTest.py
+-rw-rw-rw-   0        0        0     5816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/onefile/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.498011 Nuitka-winsvc-1.6.6/tests/optimizations/
+-rw-rw-rw-   0        0        0      958 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/ArgumentTypes.py
+-rw-rw-rw-   0        0        0     1055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/Attributes.py
+-rw-rw-rw-   0        0        0     1021 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/Calls.py
+-rw-rw-rw-   0        0        0      921 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/Conditions.py
+-rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/DecodingOperations.py
+-rw-rw-rw-   0        0        0     1212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/FormatStrings36.py
+-rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/HardImports.py
+-rw-rw-rw-   0        0        0      974 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/HardImports_2.py
+-rw-rw-rw-   0        0        0      918 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/Iterations.py
+-rw-rw-rw-   0        0        0     1260 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/Len.py
+-rw-rw-rw-   0        0        0     2262 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/Operations.py
+-rw-rw-rw-   0        0        0     1333 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/Subscripts.py
+-rw-rw-rw-   0        0        0     8736 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/optimizations/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.506765 Nuitka-winsvc-1.6.6/tests/packages/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.516572 Nuitka-winsvc-1.6.6/tests/packages/package_import_success_after_failure/
+-rw-rw-rw-   0        0        0     2382 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.533183 Nuitka-winsvc-1.6.6/tests/packages/package_import_success_after_failure/variable_package/
+-rw-rw-rw-   0        0        0      942 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+-rw-rw-rw-   0        0        0     1168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rw-rw-rw-   0        0        0     3671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.040418 Nuitka-winsvc-1.6.6/tests/packages/sub_package/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.578091 Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/
+-rw-rw-rw-   0        0        0     1230 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/__init__.py
+-rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/bigkitty.py
+-rw-rw-rw-   0        0        0      910 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/smallkitty.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.627871 Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/speak/
+-rw-rw-rw-   0        0        0      929 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/speak/hello.py
+-rw-rw-rw-   0        0        0      966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/speak/miau.py
+-rw-rw-rw-   0        0        0      968 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/speak/purr.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.042374 Nuitka-winsvc-1.6.6/tests/packages/top_level_attributes_3/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.652285 Nuitka-winsvc-1.6.6/tests/packages/top_level_attributes_3/some_package/
+-rw-rw-rw-   0        0        0     2336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.666934 Nuitka-winsvc-1.6.6/tests/plugins/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.668879 Nuitka-winsvc-1.6.6/tests/plugins/code_signing/
+-rw-rw-rw-   0        0        0     1170 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/plugins/code_signing/CodeSigningMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.693309 Nuitka-winsvc-1.6.6/tests/plugins/data_files/
+-rw-rw-rw-   0        0        0     1332 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/plugins/data_files/DataFilesMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.708916 Nuitka-winsvc-1.6.6/tests/plugins/data_files/data_files_package/
+-rw-rw-rw-   0        0        0      924 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/plugins/data_files/data_files_package/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/tests/plugins/data_files/data_files_package/lala.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.711845 Nuitka-winsvc-1.6.6/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-rw-rw-   0        0        0      255 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/tests/plugins/data_files/test_case.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.739194 Nuitka-winsvc-1.6.6/tests/plugins/parameters/
+-rw-rw-rw-   0        0        0     1019 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/plugins/parameters/ParametersMain.py
+-rw-rw-rw-   0        0        0     2168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/plugins/parameters/parameter-using-plugin.py
+-rw-rw-rw-   0        0        0     3861 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/plugins/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.755824 Nuitka-winsvc-1.6.6/tests/programs/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.775327 Nuitka-winsvc-1.6.6/tests/programs/absolute_import/
+-rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.847675 Nuitka-winsvc-1.6.6/tests/programs/absolute_import/foobar/
+-rw-rw-rw-   0        0        0      796 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/absolute_import/foobar/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/absolute_import/foobar/foobar.py
+-rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/absolute_import/foobar/local.py
+-rw-rw-rw-   0        0        0      860 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/absolute_import/foobar/util.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.853534 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.865253 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path1/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.880909 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path1/Some_Package/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.896500 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path2/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path2/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.915079 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path2/some_package/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path2/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.923837 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.936555 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path1/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path1/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.942410 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path1/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.948846 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path2/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.955683 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path2/Some_Package/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.977740 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/
+-rw-rw-rw-   0        0        0     1075 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:39.986512 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path1/
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.003136 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path1/Some_Package/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.015806 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path2/
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.022643 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path2/Some_Package/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.035357 Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/
+-rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.081232 Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+-rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.127121 Nuitka-winsvc-1.6.6/tests/programs/dash_import/
+-rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/dash_import/DashImportMain.py
+-rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/dash_import/dash-module.py
+-rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/dash_import/plus+module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.134973 Nuitka-winsvc-1.6.6/tests/programs/dash_main/
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/dash_main/Dash-Main.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.147661 Nuitka-winsvc-1.6.6/tests/programs/deep/
+-rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/deep/DeepProgramMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.184742 Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/
+-rw-rw-rw-   0        0        0      980 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/DeepBrother.py
+-rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/DeepChild.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.219889 Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/deep_package/
+-rw-rw-rw-   0        0        0      876 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+-rw-rw-rw-   0        0        0      952 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/deep_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.229686 Nuitka-winsvc-1.6.6/tests/programs/dunderinit_imports/
+-rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.255072 Nuitka-winsvc-1.6.6/tests/programs/dunderinit_imports/package/
+-rw-rw-rw-   0        0        0      797 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-rw-rw-   0        0        0      857 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/dunderinit_imports/package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.268714 Nuitka-winsvc-1.6.6/tests/programs/import_variants/
+-rw-rw-rw-   0        0        0     1005 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/import_variants/ImportVariationsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.315613 Nuitka-winsvc-1.6.6/tests/programs/import_variants/some_package/
+-rw-rw-rw-   0        0        0      946 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/import_variants/some_package/Child1.py
+-rw-rw-rw-   0        0        0     1098 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/import_variants/some_package/Child2.py
+-rw-rw-rw-   0        0        0      822 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/import_variants/some_package/Child3.py
+-rw-rw-rw-   0        0        0      994 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/import_variants/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.343912 Nuitka-winsvc-1.6.6/tests/programs/main_raises/
+-rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/main_raises/ErrorMain.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/main_raises/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.372224 Nuitka-winsvc-1.6.6/tests/programs/main_raises2/
+-rw-rw-rw-   0        0        0     1080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/main_raises2/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.383945 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/
+-rw-rw-rw-   0        0        0     1529 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.417186 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/
+-rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/Nearby1.py
+-rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.431803 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/
+-rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.442166 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.466578 Nuitka-winsvc-1.6.6/tests/programs/module_exits/
+-rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_exits/ErrorExitingModule.py
+-rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_exits/Main.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.495873 Nuitka-winsvc-1.6.6/tests/programs/module_object_replacing/
+-rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-rw-rw-   0        0        0     1359 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.506650 Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/
+-rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.546655 Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/foo/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-rw-rw-   0        0        0      836 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-rw-rw-   0        0        0     1758 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/foo/entry.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.564260 Nuitka-winsvc-1.6.6/tests/programs/named_imports/
+-rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/named_imports/NamedImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.592548 Nuitka-winsvc-1.6.6/tests/programs/named_imports/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/named_imports/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/named_imports/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.596453 Nuitka-winsvc-1.6.6/tests/programs/named_imports/some_package/sub_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.615005 Nuitka-winsvc-1.6.6/tests/programs/package_code/
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_code/PackageInitCodeMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.632583 Nuitka-winsvc-1.6.6/tests/programs/package_code/some_package/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_code/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_code/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.663835 Nuitka-winsvc-1.6.6/tests/programs/package_contains_main/
+-rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_contains_main/PackageContainsMain.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_contains_main/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_contains_main/local.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.681120 Nuitka-winsvc-1.6.6/tests/programs/package_init_import/
+-rw-rw-rw-   0        0        0      823 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_init_import/PackageInitImportMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.710454 Nuitka-winsvc-1.6.6/tests/programs/package_init_import/some_package/
+-rw-rw-rw-   0        0        0     1008 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_init_import/some_package/PackageLocal.py
+-rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_init_import/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.719235 Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/
+-rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.729945 Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/some_package/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.764577 Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/some_package/child_package/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-rw-rw-   0        0        0      795 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/some_package/child_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.779239 Nuitka-winsvc-1.6.6/tests/programs/package_missing_init/
+-rw-rw-rw-   0        0        0      926 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.787037 Nuitka-winsvc-1.6.6/tests/programs/package_missing_init/some_package/
+-rw-rw-rw-   0        0        0      965 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_missing_init/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.799760 Nuitka-winsvc-1.6.6/tests/programs/package_missing_init/some_package/sub_package/
+-rw-rw-rw-   0        0        0      977 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.829979 Nuitka-winsvc-1.6.6/tests/programs/package_module_collision/
+-rw-rw-rw-   0        0        0      901 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.836823 Nuitka-winsvc-1.6.6/tests/programs/package_module_collision/Something/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_module_collision/Something/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_module_collision/something.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.850488 Nuitka-winsvc-1.6.6/tests/programs/package_overload/
+-rw-rw-rw-   0        0        0      852 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_overload/Main.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.880791 Nuitka-winsvc-1.6.6/tests/programs/package_overload/foo/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_overload/foo/__init__.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_overload/foo/bar.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_overload/foo/bar2.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.899314 Nuitka-winsvc-1.6.6/tests/programs/package_prevents_submodule/
+-rw-rw-rw-   0        0        0     2972 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.932514 Nuitka-winsvc-1.6.6/tests/programs/package_prevents_submodule/some_package/
+-rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:33.099655 Nuitka-winsvc-1.6.6/tests/programs/package_program/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.963763 Nuitka-winsvc-1.6.6/tests/programs/package_program/PackageAsMain/
+-rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_program/PackageAsMain/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/package_program/PackageAsMain/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.982347 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/
+-rw-rw-rw-   0        0        0     1728 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:40.994032 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.019455 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.046781 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.059461 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_usage/
+-rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.086808 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_usage/package/
+-rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+-rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-rw-rw-   0        0        0     1553 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/pkgutil_usage/package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.103410 Nuitka-winsvc-1.6.6/tests/programs/plugin_import/
+-rw-rw-rw-   0        0        0      859 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/plugin_import/PluginImportMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.137606 Nuitka-winsvc-1.6.6/tests/programs/plugin_import/some_package/
+-rw-rw-rw-   0        0        0      771 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/plugin_import/some_package/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/plugin_import/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.151254 Nuitka-winsvc-1.6.6/tests/programs/reimport_main_dynamic/
+-rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.166882 Nuitka-winsvc-1.6.6/tests/programs/reimport_main_static/
+-rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.192265 Nuitka-winsvc-1.6.6/tests/programs/relative_import/
+-rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/relative_import/RelativeImportMain.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/relative_import/dircache.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.205976 Nuitka-winsvc-1.6.6/tests/programs/resource_reader37/
+-rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.230382 Nuitka-winsvc-1.6.6/tests/programs/resource_reader37/some_package/
+-rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.6/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/resource_reader37/some_package/__init__.py
+-rw-rw-rw-   0        0        0     6615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.261597 Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/
+-rw-rw-rw-   0        0        0     1171 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/pyexpat.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.318241 Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/some_package/star_importing.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.365118 Nuitka-winsvc-1.6.6/tests/programs/syntax_errors/
+-rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/syntax_errors/IndentationErroring.py
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-rw-rw-   0        0        0     1079 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/syntax_errors/SyntaxErrorsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.403224 Nuitka-winsvc-1.6.6/tests/programs/unicode_bom/
+-rw-rw-rw-   0        0        0      963 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/unicode_bom/unicode_bom.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.420767 Nuitka-winsvc-1.6.6/tests/programs/with space/
+-rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/programs/with space/Space Main.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:41.439429 Nuitka-winsvc-1.6.6/tests/reflected/
+-rw-rw-rw-   0        0        0    14061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/reflected/compile_itself.py
+-rw-rw-rw-   0        0        0     1243 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/run-tests
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:42.093076 Nuitka-winsvc-1.6.6/tests/standalone/
+-rw-rw-rw-   0        0        0     1058 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/BrotliUsing.py
+-rw-rw-rw-   0        0        0     2554 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/CtypesUsing.py
+-rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/FlaskUsing.py
+-rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/GlfwUsing.py
+-rw-rw-rw-   0        0        0     1184 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/GtkUsing.py
+-rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/HexEncodingTest_2.py
+-rw-rw-rw-   0        0        0     1086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/IdnaUsing.py
+-rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/LxmlUsing.py
+-rw-rw-rw-   0        0        0     1431 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/MatplotlibUsing.py
+-rw-rw-rw-   0        0        0     2538 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/MetadataPackagesUsing.py
+-rw-rw-rw-   0        0        0     1727 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/NumpyUsing.py
+-rw-rw-rw-   0        0        0      947 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/OpenGLUsing.py
+-rw-rw-rw-   0        0        0     1379 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PandasUsing.py
+-rw-rw-rw-   0        0        0     1066 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PasslibUsing.py
+-rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PendulumUsing.py
+-rw-rw-rw-   0        0        0     2074 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-rw-rw-   0        0        0     1067 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PmwUsing.py
+-rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PyQt5Plugins.py
+-rw-rw-rw-   0        0        0     1105 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PyQt5SSLSupport.py
+-rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PyQt5Using.py
+-rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PyQt6Plugins.py
+-rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PyQt6Using.py
+-rw-rw-rw-   0        0        0     1091 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PySide6Plugins.py
+-rw-rw-rw-   0        0        0     1757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/PySide6Using.py
+-rw-rw-rw-   0        0        0     1323 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/RsaUsing.py
+-rw-rw-rw-   0        0        0      973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/ShlibUsing.py
+-rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/SocketUsing.py
+-rw-rw-rw-   0        0        0     1941 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/TkInterUsing.py
+-rw-rw-rw-   0        0        0     3228 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/Urllib3Using.py
+-rw-rw-rw-   0        0        0     1200 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/Win32ComUsing.py
+-rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:42.108694 Nuitka-winsvc-1.6.6/tests/standalone/zip_importer/
+-rw-rw-rw-   0        0        0     1264 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/standalone/zip_importer/ZipImporterMain.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:36:42.567871 Nuitka-winsvc-1.6.6/tests/syntax/
+-rw-rw-rw-   0        0        0      811 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/AsyncgenReturn36.py
+-rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/BreakWithoutLoop.py
+-rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/ClassReturn.py
+-rw-rw-rw-   0        0        0      970 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/ClosureDel_2.py
+-rw-rw-rw-   0        0        0      849 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/ContinueWithoutLoop.py
+-rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/DuplicateArgument.py
+-rw-rw-rw-   0        0        0     1111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/ExecWithNesting_2.py
+-rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/FutureBraces.py
+-rw-rw-rw-   0        0        0      805 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/FutureUnknown.py
+-rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/GeneratorExpressions38.py
+-rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/GeneratorReturn_2.py
+-rw-rw-rw-   0        0        0      792 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/GlobalForParameter.py
+-rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/Importing32.py
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/IndentationError.py
+-rw-rw-rw-   0        0        0      915 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/LateFutureImport.py
+-rw-rw-rw-   0        0        0      841 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/MisplacedFutureImport.py
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/ModuleReturn.py
+-rw-rw-rw-   0        0        0      883 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/NonlocalForParameter32.py
+-rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/NonlocalNotFound32.py
+-rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/StarImportExtra.py
+-rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/SyntaxError.py
+-rw-rw-rw-   0        0        0      874 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/TryExceptAllNotLast.py
+-rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/TryFinallyContinue_37.py
+-rw-rw-rw-   0        0        0      776 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/UnpackNoTuple.py
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/UnpackTwoStars32.py
+-rw-rw-rw-   0        0        0      793 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/YieldFromInModule.py
+-rw-rw-rw-   0        0        0      804 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/YieldInAsync35.py
+-rw-rw-rw-   0        0        0      923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/YieldInGenexp38.py
+-rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/YieldInModule.py
+-rw-rw-rw-   0        0        0     2203 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.6/tests/syntax/run_all.py
```

### Comparing `Nuitka-winsvc-1.6.4/Changelog.rst` & `Nuitka-winsvc-1.6.6/Changelog.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/Developer_Manual.rst` & `Nuitka-winsvc-1.6.6/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/LICENSE.txt` & `Nuitka-winsvc-1.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/MANIFEST.in` & `Nuitka-winsvc-1.6.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/PKG-INFO` & `Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 1.6.4
+Version: 1.6.6
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `Nuitka-winsvc-1.6.4/Nuitka_winsvc.egg-info/SOURCES.txt` & `Nuitka-winsvc-1.6.6/Nuitka_winsvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/PKG-INFO` & `Nuitka-winsvc-1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 1.6.4
+Version: 1.6.6
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `Nuitka-winsvc-1.6.4/README.md` & `Nuitka-winsvc-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/README.rst` & `Nuitka-winsvc-1.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/bin/autoformat-nuitka-source` & `Nuitka-winsvc-1.6.6/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/bin/check-nuitka-with-pylint` & `Nuitka-winsvc-1.6.6/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/bin/compare_with_cpython` & `Nuitka-winsvc-1.6.6/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/bin/compare_with_xml` & `Nuitka-winsvc-1.6.6/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/bin/measure-construct-performance` & `Nuitka-winsvc-1.6.6/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/bin/nuitka` & `Nuitka-winsvc-1.6.6/bin/nuitka`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/bin/nuitka-run` & `Nuitka-winsvc-1.6.6/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/doc/Logo/Nuitka-Logo-Horizontal.svg` & `Nuitka-winsvc-1.6.6/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/doc/Logo/Nuitka-Logo-Symbol.svg` & `Nuitka-winsvc-1.6.6/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/doc/Logo/Nuitka-Logo-Vertical.svg` & `Nuitka-winsvc-1.6.6/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/doc/images/Nuitka-Logo-Horizontal.png` & `Nuitka-winsvc-1.6.6/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/doc/images/Nuitka-Logo-Symbol.png` & `Nuitka-winsvc-1.6.6/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/doc/images/Nuitka-Logo-Vertical.png` & `Nuitka-winsvc-1.6.6/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/lib/hints.py` & `Nuitka-winsvc-1.6.6/lib/hints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/misc/nuitka-run.bat` & `Nuitka-winsvc-1.6.6/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/misc/nuitka.bat` & `Nuitka-winsvc-1.6.6/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Builtins.py` & `Nuitka-winsvc-1.6.6/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/BytecodeCaching.py` & `Nuitka-winsvc-1.6.6/nuitka/BytecodeCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Bytecodes.py` & `Nuitka-winsvc-1.6.6/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/CacheCleanup.py` & `Nuitka-winsvc-1.6.6/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Constants.py` & `Nuitka-winsvc-1.6.6/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Errors.py` & `Nuitka-winsvc-1.6.6/nuitka/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/MainControl.py` & `Nuitka-winsvc-1.6.6/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/ModuleRegistry.py` & `Nuitka-winsvc-1.6.6/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/OptionParsing.py` & `Nuitka-winsvc-1.6.6/nuitka/OptionParsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Options.py` & `Nuitka-winsvc-1.6.6/nuitka/Options.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/OutputDirectories.py` & `Nuitka-winsvc-1.6.6/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/PostProcessing.py` & `Nuitka-winsvc-1.6.6/nuitka/PostProcessing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Progress.py` & `Nuitka-winsvc-1.6.6/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/PythonFlavors.py` & `Nuitka-winsvc-1.6.6/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/PythonOperators.py` & `Nuitka-winsvc-1.6.6/nuitka/PythonOperators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/PythonVersions.py` & `Nuitka-winsvc-1.6.6/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Serialization.py` & `Nuitka-winsvc-1.6.6/nuitka/Serialization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/SourceCodeReferences.py` & `Nuitka-winsvc-1.6.6/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Tracing.py` & `Nuitka-winsvc-1.6.6/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/TreeXML.py` & `Nuitka-winsvc-1.6.6/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Variables.py` & `Nuitka-winsvc-1.6.6/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/Version.py` & `Nuitka-winsvc-1.6.6/nuitka/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V1.6.4
+Nuitka V1.6.6
 Copyright (C) 2023 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `Nuitka-winsvc-1.6.4/nuitka/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/__past__.py` & `Nuitka-winsvc-1.6.6/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/Backend.scons` & `Nuitka-winsvc-1.6.6/nuitka/build/Backend.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/CCompilerVersion.scons` & `Nuitka-winsvc-1.6.6/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/DataComposerInterface.py` & `Nuitka-winsvc-1.6.6/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/Onefile.scons` & `Nuitka-winsvc-1.6.6/nuitka/build/Onefile.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/SconsCaching.py` & `Nuitka-winsvc-1.6.6/nuitka/build/SconsCaching.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,15 @@
 
 
 def enableClcache(env, source_dir):
     # We allow using Python2 still
     if sys.version_info < (3, 5):
         return
 
+    # spell-checker: ignore atomicwrites
     importFromInlineCopy("atomicwrites", must_exist=True)
     importFromInlineCopy("clcache", must_exist=True)
 
     # Avoid importing this in threads, triggers CPython 3.9 importing bugs at least,
     # do it now, so it's not a race issue.
     import concurrent.futures.thread  # pylint: disable=I0021,unused-import,unused-variable
 
@@ -229,15 +230,16 @@
 
     # The compiler is passed via environment.
     setEnvironmentVariable(env, "CLCACHE_CL", cl_binary)
     env["CXX"] = env["CC"] = "<clcache>"
 
     setEnvironmentVariable(env, "CLCACHE_HIDE_OUTPUTS", "1")
 
-    # Use the mode of clcache that is not dependent on MSVC filenames output
+    # Use the mode of "clcache" that is not dependent on MSVC filenames output
+    # spell-checker: ignore CLCACHE_NODIRECT
     if "CLCACHE_NODIRECT" not in os.environ:
         setEnvironmentVariable(env, "CLCACHE_NODIRECT", "1")
 
     # The clcache stats filename needs absolute path, otherwise it will not work.
     clcache_stats_filename = os.path.abspath(
         os.path.join(source_dir, "clcache-stats.%d.txt" % os.getpid())
     )
@@ -358,43 +360,43 @@
 
             for _command, result in stats.items():
                 # These are not important to our users, time based decisions differentiate these.
                 if result in (
                     "cache hit (direct)",
                     "cache hit (preprocessed)",
                     "local_storage_hit",
+                    "primary_storage_hit",
                 ):
                     result = "cache hit"
+                elif result == "cache_miss":
+                    result = "cache miss"
 
                 # Newer ccache has these, but they duplicate:
                 if result in (
                     "direct_cache_hit",
                     "direct_cache_miss",
                     "preprocessed_cache_hit",
                     "preprocessed_cache_miss",
                     "primary_storage_miss",
                     "called_for_link",
                     "local_storage_read_hit",
                     "local_storage_read_miss",
                     "local_storage_write",
                     "local_storage_miss",
+                    # Usage of incbin causes this for the constants blob integration.
+                    "unsupported code directive",
+                    "disabled",
                 ):
                     continue
-                if result == "primary_storage_hit":
-                    result = "cache hit"
-                if result == "cache_miss":
-                    result = "cache miss"
-
-                # Usage of incbin causes this for the constants blob integration.
-                if result in ("unsupported code directive", "disabled"):
-                    continue
 
                 counts[result] += 1
 
-            scons_logger.info("Compiled %d C files using ccache." % len(stats))
+            scons_logger.info(
+                "Compiled %d C files using ccache." % sum(counts.values())
+            )
             for result, count in sorted(counts.items()):
                 scons_logger.info(
                     "Cached C files (using ccache) with result '%s': %d"
                     % (result, count)
                 )
 
     if os.name == "nt":
```

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/SconsCompilerSettings.py` & `Nuitka-winsvc-1.6.6/nuitka/build/SconsCompilerSettings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/SconsHacks.py` & `Nuitka-winsvc-1.6.6/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/SconsInterface.py` & `Nuitka-winsvc-1.6.6/nuitka/build/SconsInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import os
 import subprocess
 import sys
 
 from nuitka import Options, Tracing
 from nuitka.__past__ import unicode
 from nuitka.containers.OrderedDicts import OrderedDict
+from nuitka.Options import getOnefileChildGraceTime, isOnefileMode
 from nuitka.plugins.Plugins import Plugins
 from nuitka.PythonFlavors import (
     isAnacondaPython,
     isMSYS2MingwPython,
     isNuitkaPython,
 )
 from nuitka.PythonVersions import (
@@ -491,8 +492,15 @@
     if isNuitkaPython() and not isWin32OrPosixWindows():
         # Override environment CC and CXX to match build compiler.
         import sysconfig
 
         env_values["CC"] = sysconfig.get_config_var("CC").split()[0]
         env_values["CXX"] = sysconfig.get_config_var("CXX").split()[0]
 
+    # Onefile grace time is shared, because client will also suicide based on
+    # it.
+    if isOnefileMode():
+        env_values["_NUITKA_ONEFILE_CHILD_GRACE_TIME_INT"] = str(
+            getOnefileChildGraceTime()
+        )
+
     return env_values
```

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/SconsProgress.py` & `Nuitka-winsvc-1.6.6/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/SconsSpawn.py` & `Nuitka-winsvc-1.6.6/nuitka/build/SconsSpawn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/SconsUtils.py` & `Nuitka-winsvc-1.6.6/nuitka/build/SconsUtils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/allocator.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/builtins.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/calling.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/checkers.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/checksum_tools.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_asyncgen.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_cell.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_coroutine.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_frame.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_function.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_generator.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/compiled_method.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/constants.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/constants.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/constants_blob.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/exceptions.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/filesystem_paths.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/freelists.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/hedley.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/attributes.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/boolean.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/bytearrays.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/bytes.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/calling_generated.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_le.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/complex.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/dictionaries.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/floats.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/import_hard.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/indexes.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/ints.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/iterators.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/lists.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/lists_generated.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/mappings.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/raising.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/rangeobjects.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/richcomparisons.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/sequences.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/sets.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/slices.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/strings.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/subscripts.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helper/tuples.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/helpers.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/helpers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/importing.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/incbin.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/prelude.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/prelude.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/printing.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/python_pgo.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/safe_string_ops.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/threading.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/tracing.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/include/nuitka/unfreezing.h` & `Nuitka-winsvc-1.6.6/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/appdirs/appdirs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/atomicwrites/LICENSE` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/bin/scons.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/clcache/clcache/caching.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/LICENSE.txt` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/win32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/LICENSE` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/glob2/compat.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/glob2/glob2/impl.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/gui.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/LICENSE` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/composer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/error.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/events.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/loader.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/parser.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/reader.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/representer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/LICENSE` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/LICENSE` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/LICENSE.txt` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/bitstream.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/compiler.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/cpu.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/debug.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/error_private.c` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/error_private.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/fse.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/huf.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/mem.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/xxhash.c` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/xxhash.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/inline_copy/zstd/zstd.h` & `Nuitka-winsvc-1.6.6/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledAsyncgenType.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledCellType.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledCodeHelpers.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledCoroutineType.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledFrameType.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledFunctionType.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledGeneratorType.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/CompiledMethodType.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersAllocator.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersAttributes.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersBuiltin.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersBytes.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersCalling.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersCallingGenerated.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersChecksumTools.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersClasses.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonEq.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonGe.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonGt.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonLe.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonLt.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersComparisonNe.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersConstantsBlob.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersDeepcopy.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersDictionaries.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersExceptions.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersFiles.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersFilesystemPaths.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersFloats.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersHeapStorage.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersImport.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersImportHard.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersLists.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersLists.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersListsGenerated.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersMappings.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersMatching.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinarySub.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplacePow.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersProfiling.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersPythonPgo.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersRaising.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersSafeStrings.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersSequences.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersSlices.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersStrings.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersTuples.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/HelpersTypes.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/InspectPatcher.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/MainProgram.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/MainProgram.c`

 * *Files 1% similar despite different names*

```diff
@@ -319,18 +319,19 @@
     return argv_copy;
 }
 #endif
 
 static int HANDLE_PROGRAM_EXIT(void) {
     int exit_code;
 
-    if (ERROR_OCCURRED()) {
+    PyThreadState *thread_state = PyThreadState_GET();
+
+    if (HAS_ERROR_OCCURRED(thread_state)) {
 #if PYTHON_VERSION >= 0x300
         /* Remove the frozen importlib traceback part, which would not be compatible. */
-        PyThreadState *thread_state = PyThreadState_GET();
 
         while (thread_state->curexc_traceback) {
             PyTracebackObject *tb = (PyTracebackObject *)thread_state->curexc_traceback;
             PyFrameObject *frame = tb->tb_frame;
 
             if (0 == strcmp(PyUnicode_AsUTF8(Nuitka_Frame_GetCodeObject(frame)->co_filename),
                             "<frozen importlib._bootstrap>")) {
@@ -406,16 +407,16 @@
         return 0;
     }
 }
 #endif
 
 // This is a multiprocessing fork
 static bool is_multiprocessing_fork = false;
-// This is a multiprocessing resource tracker.
-static PyObject *multiprocessing_resource_tracker_arg = NULL;
+// This is a multiprocessing resource tracker if not -1
+static int multiprocessing_resource_tracker_arg = -1;
 
 // Parse the command line parameters and provide it to "sys" built-in module,
 // as well as decide if it's a multiprocessing usage.
 #if _NUITKA_NATIVE_WCHAR_ARGV == 0
 static void setCommandLineParameters(int argc, char **argv, bool initial) {
 #else
 static void setCommandLineParameters(int argc, wchar_t **argv, bool initial) {
@@ -441,17 +442,17 @@
 #if _NUITKA_NATIVE_WCHAR_ARGV == 0
             if ((strcmp(argv[i], "--multiprocessing-resource-tracker")) == 0 && (i + 1 < argc))
 #else
             if ((wcscmp(argv[i], L"--multiprocessing-resource-tracker")) == 0 && (i + 1 < argc))
 #endif
             {
 #if _NUITKA_NATIVE_WCHAR_ARGV == 0
-                multiprocessing_resource_tracker_arg = PyInt_FromLong(atoi(argv[i + 1]));
+                multiprocessing_resource_tracker_arg = atoi(argv[i + 1]);
 #else
-                multiprocessing_resource_tracker_arg = PyLong_FromLong(_wtoi(argv[i + 1]));
+                multiprocessing_resource_tracker_arg = _wtoi(argv[i + 1]);
 #endif
                 break;
             }
 
 #ifdef _NUITKA_PLUGIN_WINDOWS_SERVICE_ENABLED
             if (i == 1) {
 #if PYTHON_VERSION < 0x300
@@ -531,17 +532,21 @@
             if (ret == WAIT_OBJECT_0) {
                 break;
             }
         }
     }
 
     NUITKA_PRINT_TRACE("Onefile parent monitoring causes KeyboardInterrupt.");
-
     PyErr_SetInterrupt();
 
+    Sleep(_NUITKA_ONEFILE_CHILD_GRACE_TIME_INT);
+
+    NUITKA_PRINT_TRACE("Onefile parent monitoring hard kills after ignored KeyboardInterrupt.");
+    ExitProcess(1);
+
     return 0;
 }
 #endif
 
 #if defined(_WIN32) && PYTHON_VERSION < 0x300
 static char **getCommandLineToArgvA(char *lpCmdline) {
     char *s = lpCmdline;
@@ -1065,16 +1070,16 @@
 #endif
 
     // Make sure the compiled path of Python is replaced.
     Py_SetProgramName(orig_argv[0]);
 
     orig_argc = argc;
 
+    // Early command line parsing.
     NUITKA_PRINT_TRACE("main(): Calling initial setCommandLineParameters.");
-
     setCommandLineParameters(argc, argv, true);
 
     /* For Python installations that need the home set, we inject it back here. */
 #if defined(PYTHON_HOME_PATH)
 #if PYTHON_VERSION < 0x300
     NUITKA_PRINT_TRACE("main(): Prepare run environment '" PYTHON_HOME_PATH "'.");
     Py_SetPythonHome(PYTHON_HOME_PATH);
@@ -1293,21 +1298,21 @@
 
         int exit_code = HANDLE_PROGRAM_EXIT();
 
         NUITKA_PRINT_TRACE("main(): Calling __parents_main__ Py_Exit.");
 
         // TODO: Should maybe call Py_Exit here, but there were issues with that.
         exit(exit_code);
-    } else if (unlikely(multiprocessing_resource_tracker_arg != NULL)) {
+    } else if (unlikely(multiprocessing_resource_tracker_arg != -1)) {
         NUITKA_PRINT_TRACE("main(): Calling resource_tracker.");
         PyObject *resource_tracker_module = EXECUTE_MAIN_MODULE("multiprocessing.resource_tracker");
 
         PyObject *main_function = PyObject_GetAttrString(resource_tracker_module, "main");
 
-        CALL_FUNCTION_WITH_SINGLE_ARG(main_function, multiprocessing_resource_tracker_arg);
+        CALL_FUNCTION_WITH_SINGLE_ARG(main_function, PyInt_FromLong(multiprocessing_resource_tracker_arg));
 
         int exit_code = HANDLE_PROGRAM_EXIT();
 
         NUITKA_PRINT_TRACE("main(): Calling resource_tracker Py_Exit.");
         // TODO: Should maybe call Py_Exit here, but there were issues with that.
         exit(exit_code);
     } else {
```

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/MetaPathBasedLoader.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/OnefileBootstrap.c` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files 1% similar despite different names*

```diff
@@ -1020,14 +1020,16 @@
 #if defined(_WIN32)
     bool_res = SetConsoleCtrlHandler(ourConsoleCtrlHandler, true);
     if (bool_res == false) {
         fatalError("Error, failed to register signal handler.");
     }
 #else
     signal(SIGINT, ourConsoleCtrlHandler);
+    signal(SIGQUIT, ourConsoleCtrlHandler);
+    signal(SIGTERM, ourConsoleCtrlHandler);
 #endif
 
 #ifdef _NUITKA_AUTO_UPDATE_BOOL
     checkAutoUpdates();
 #endif
 
     NUITKA_PRINT_TIMING("ONEFILE: Unpacking payload.");
```

### Comparing `Nuitka-winsvc-1.6.4/nuitka/build/static_src/OnefileSplashScreen.cpp` & `Nuitka-winsvc-1.6.6/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/AsyncgenCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/AttributeCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/BranchCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/BuiltinCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/BuiltinCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/CallCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ClassCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/CodeGeneration.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/CodeGeneration.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/CodeHelperSelection.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/CodeHelpers.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/CodeObjectCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ComparisonCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ComparisonHelperDefinitions.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ConditionalCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ConstantCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/Contexts.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/CoroutineCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/CtypesCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/DictCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/Emission.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ErrorCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/EvalCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ExceptionCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ExceptionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ExpressionCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/FrameCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/FunctionCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/GeneratorCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/GlobalConstants.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/GlobalConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/GlobalsLocalsCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/IdCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ImportCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/Indentation.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/IndexCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/InjectCCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/IntegerCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/IteratorCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/LabelCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/LineNumberCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ListCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/LoaderCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/LocalsDictCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/LoopCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/MatchCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ModuleCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/Namify.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/OperationCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/PackageResourceCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/PrintCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/PythonAPICodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/RaisingCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/Reports.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/ReturnCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/SetCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/SliceCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/StringCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/SubscriptCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/TryCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/TupleCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/VariableCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/VariableDeclarations.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/YieldCodes.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/YieldCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeBases.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeBooleans.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeCFloats.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeCLongs.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/CTypeVoids.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/c_types/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesModules.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `Nuitka-winsvc-1.6.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/containers/Namedtuples.py` & `Nuitka-winsvc-1.6.6/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/containers/OrderedDicts.py` & `Nuitka-winsvc-1.6.6/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/containers/OrderedSets.py` & `Nuitka-winsvc-1.6.6/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/containers/OrderedSetsFallback.py` & `Nuitka-winsvc-1.6.6/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/containers/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/distutils/Build.py` & `Nuitka-winsvc-1.6.6/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/distutils/DistutilCommands.py` & `Nuitka-winsvc-1.6.6/nuitka/distutils/DistutilCommands.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/distutils/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/finalizations/Finalization.py` & `Nuitka-winsvc-1.6.6/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/finalizations/FinalizeMarkups.py` & `Nuitka-winsvc-1.6.6/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/finalizations/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/DependsExe.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/DllDependenciesCommon.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/DllDependenciesMacOS.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/DllDependenciesPosix.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/DllDependenciesWin32.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/IncludedDataFiles.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/IncludedEntryPoints.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/Onefile.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/Onefile.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,15 @@
 from nuitka.build.SconsInterface import (
     asBoolStr,
     cleanSconsDirectory,
     getSconsDataPath,
     runScons,
     setCommonSconsOptions,
 )
-from nuitka.Options import (
-    getOnefileChildGraceTime,
-    getOnefileTempDirSpec,
-    isOnefileTempDirMode,
-)
+from nuitka.Options import getOnefileTempDirSpec, isOnefileTempDirMode
 from nuitka.OutputDirectories import getResultFullpath
 from nuitka.plugins.Plugins import Plugins
 from nuitka.PostProcessing import executePostProcessingResources
 from nuitka.PythonVersions import (
     getZstandardSupportingVersions,
     python_version,
 )
@@ -89,15 +85,14 @@
 
     env_values = setCommonSconsOptions(options)
 
     env_values["_NUITKA_ONEFILE_TEMP_SPEC"] = getOnefileTempDirSpec()
     env_values["_NUITKA_ONEFILE_TEMP_BOOL"] = "1" if isOnefileTempDirMode() else "0"
     env_values["_NUITKA_ONEFILE_COMPRESSION_BOOL"] = "1" if onefile_compression else "0"
     env_values["_NUITKA_ONEFILE_BUILD_BOOL"] = "1" if onefile_compression else "0"
-    env_values["_NUITKA_ONEFILE_CHILD_GRACE_TIME_INT"] = str(getOnefileChildGraceTime())
 
     # Allow plugins to build definitions.
     env_values.update(Plugins.getBuildDefinitions())
 
     if isWin32Windows() and Options.isWindowsServiceMode():
         env_values["_NUITKA_WINSVC_BOOL"] = "1"
         winsvcMetrics = Options.getWindowsServiceMetrics()
```

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/Standalone.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/Standalone.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/freezer/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/importing/IgnoreListing.py` & `Nuitka-winsvc-1.6.6/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/importing/ImportCache.py` & `Nuitka-winsvc-1.6.6/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/importing/ImportResolving.py` & `Nuitka-winsvc-1.6.6/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/importing/Importing.py` & `Nuitka-winsvc-1.6.6/nuitka/importing/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/importing/PreloadedPackages.py` & `Nuitka-winsvc-1.6.6/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/importing/Recursion.py` & `Nuitka-winsvc-1.6.6/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/importing/StandardLibrary.py` & `Nuitka-winsvc-1.6.6/nuitka/importing/StandardLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/importing/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/AsyncgenNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/AttributeLookupNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/AttributeNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/AttributeNodesGenerated.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinAllNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinAnyNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinComplexNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinDecodingNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinDecoratorNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinDictNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinFormatNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinHashNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinIntegerNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinIteratorNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinLenNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinNextNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinOpenNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinRangeNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinRefNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinSumNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinTypeNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BuiltinVarsNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/BytesNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/CallNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/Checkers.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ChildrenHavingMixins.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ClassNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/CodeObjectSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ComparisonNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ConditionalNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ConstantRefNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ContainerMakingNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ContainerOperationNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/CoroutineNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/CtypesNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/DictionaryNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/DictionaryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ExceptionNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ExceptionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ExecEvalNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ExpressionBases.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ExpressionBasesGenerated.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ExpressionShapeMixins.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/FrameNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/FunctionAttributeNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/FunctionNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/FunctionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/FutureSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/GeneratorNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/GlobalsLocalsNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/HardImportNodesGenerated.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ImportHardNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ImportNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ImportNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/IndicatorMixins.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/InjectCNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/IterationHandles.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/KeyValuePairNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ListOperationNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/LocalsDictNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/LocalsScopes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/LoopNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/MatchNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ModuleAttributeNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ModuleNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ModuleNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/NodeBases.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/NodeMakingHelpers.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/NodeMetaClasses.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/NodeMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/OperatorNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/OperatorNodesUnary.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/OsSysNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/OutlineNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/PackageMetadataNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/PackageResourceNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/PrintNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/ReturnNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/SideEffectNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/SliceNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/StatementBasesGenerated.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/StatementNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/StrNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/StringConcatenationNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/SubscriptNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/TryNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/TypeMatchNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/TypeNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/VariableAssignNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/VariableDelNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/VariableNameNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/VariableRefNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/VariableReleaseNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/YieldNodes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/ShapeMixins.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/StandardShapes.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/nodes/shapes/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/optimizations/BytecodeDemotion.py` & `Nuitka-winsvc-1.6.6/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/optimizations/FunctionInlining.py` & `Nuitka-winsvc-1.6.6/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/optimizations/Graphs.py` & `Nuitka-winsvc-1.6.6/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/optimizations/Optimization.py` & `Nuitka-winsvc-1.6.6/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/optimizations/OptimizeBuiltinCalls.py` & `Nuitka-winsvc-1.6.6/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/optimizations/Tags.py` & `Nuitka-winsvc-1.6.6/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/optimizations/TraceCollections.py` & `Nuitka-winsvc-1.6.6/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/optimizations/ValueTraces.py` & `Nuitka-winsvc-1.6.6/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/optimizations/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/pgo/PGO.py` & `Nuitka-winsvc-1.6.6/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/pgo/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/PluginBase.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/PluginBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,25 +111,28 @@
                 from importlib_metadata import version
 
             result = _convertVersionToTuple(version(distribution_name))
         except ImportError:
             try:
                 from pkg_resources import (
                     DistributionNotFound,
+                    extern,
                     get_distribution,
                 )
             except ImportError:
                 result = None
             else:
                 try:
                     result = _convertVersionToTuple(
                         get_distribution(distribution_name).version
                     )
                 except DistributionNotFound:
                     result = None
+                except extern.packaging.version.InvalidVersion:
+                    result = None
 
         if result is None:
             # Fallback if nothing is available, which may happen if no package is installed,
             # but only source code is found.
             try:
                 result = _convertVersionToTuple(
                     __import__(
```

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/Plugins.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/AntiBloatPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/DataFilesPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/DelvewheelPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/DillPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/DllFilesPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/EnumPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/EventletPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/GeventPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/GiPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/GlfwPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/ImplicitImports.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/ImplicitImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/KivyPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/MatplotlibPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/MultiprocessingPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/NumpyPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/OptionsNannyPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PbrPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PkgResourcesPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PmwPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PySidePyQtPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/PywebViewPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TensorflowPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TkinterPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TorchPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TransformersPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TransformersPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/TrioPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/UpxPlugin.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
   implicit-imports:
     - depends:
         - 'gobject'
 
 - module-name: 'attr'
   options:
     checks:
-      - description: 'attrs is not fully supported before 23.1.0'
+      - description: "'attrs' is not fully supported before version 23.1.0"
         support_info: 'warning'
         when: 'version("attrs") < (23,1)'
 
 - module-name: 'av.audio.frame'
   implicit-imports:
     - depends:
         - 'av.frame'
@@ -262,14 +262,63 @@
       - 'VERSION'
 
 - module-name: 'cairosvg'
   data-files:
     patterns:
       - 'VERSION'
 
+- module-name: 'cassandra.cluster'
+  implicit-imports:
+    - depends:
+        - 'cassandra.auth'
+        - 'cassandra.connection'
+        - 'concurrent.futures'
+        - 'cassandra.encoder'
+        - 'cassandra.metadata'
+        - 'cassandra.timestamps'
+        - 'cassandra.datastax.insights.reporter'
+        - 'cassandra.datastax.cloud'
+        - 'cassandra.io.libevreactor'
+        - 'cassandra.io.twistedreactor'
+        - 'cassandra.io.eventletreactor'
+        - 'cassandra.io.asyncorereactor'
+        - 'six'
+        - 'uuid'
+
+- module-name: 'cassandra.connection'
+  implicit-imports:
+    - depends:
+        - 'cassandra.marshal'
+        - 'cassandra.protocol'
+        - 'cassandra.segment'
+
+- module-name: 'cassandra.cqltypes'
+  implicit-imports:
+    - depends:
+        - 'cassandra.util'
+
+- module-name: 'cassandra.metadata'
+  implicit-imports:
+    - depends:
+        - 'cassandra.query'
+        - 'cassandra.pool'
+
+- module-name: 'cassandra.protocol'
+  implicit-imports:
+    - depends:
+        - 'cassandra.type_codes'
+        - 'cassandra.cqltypes'
+        - 'cassandra.policies'
+        - 'cassandra.cython_deps'
+
+- module-name: 'cassandra.util'
+  implicit-imports:
+    - depends:
+        - 'cassandra.compat'
+
 - module-name: 'cefpython3'
   data-files:
     dirs:
       - 'locales'
     patterns:
       - '*.bin'
       - '*.pak'
@@ -492,14 +541,21 @@
 
 - module-name: 'dask.dataframe._compat'
   anti-bloat:
     - description: 'remove pandas.testing reference'
       replacements_plain:
         'import pandas.testing as tm': ''
 
+- module-name: 'dask.dot'
+  anti-bloat:
+    - description: 'remove IPython reference'
+      replacements_plain:
+        'import IPython.display as display': 'raise ImportError'
+      when: 'not use_ipython'
+
 - module-name: 'datatree'
   anti-bloat:
     - description: 'remove useless metadata usage'
       replacements_plain:
         '__version__ = get_distribution(__name__).version': 'raise DistributionNotFound'
 
 - module-name: 'dependency_injector._cwiring'
@@ -660,14 +716,30 @@
         '__parse_starttag.__code__ = sgmllib.SGMLParser.parse_starttag.__code__': "'pass'"
         'def goahead(self, i):': "'def goahead(self, end):'"
         'goahead.__code__ = sgmllib.SGMLParser.goahead.__code__': "'pass'"
       change_function:
         '__parse_starttag': 'textwrap.dedent(inspect.getsource(sgmllib.SGMLParser.parse_starttag))'
         'goahead': 'textwrap.dedent(inspect.getsource(sgmllib.SGMLParser.goahead))'
 
+- module-name: 'fiona'
+  data-files:
+    dirs:
+      - 'proj_data'
+
+- module-name: 'fiona.crs'
+  implicit-imports:
+    - depends:
+        - 'fiona.enums'
+
+- module-name: 'fiona.ogrext'
+  implicit-imports:
+    - depends:
+        - 'fiona.schema'
+        - 'fiona._shim'
+
 - module-name: 'fitz.fitz'
   implicit-imports:
     - depends:
         - 'fitz._fitz'
 
 - module-name: 'flask.app'
   implicit-imports:
@@ -689,14 +761,21 @@
         when: 'macos'
 
 - module-name: 'frozendict'
   data-files:
     patterns:
       - 'VERSION'
 
+- module-name: 'fsspec.transaction'
+  anti-bloat:
+    - description: 'remove optional dask usage'
+      replacements_plain:
+        'import distributed': 'raise ImportError'
+      when: 'not use_dask'
+
 - module-name: 'gevent'
   implicit-imports:
     - depends:
         - '_cffi_backend'
         - 'gevent._config'
         - 'gevent.core'
         - 'gevent.resolver_thread'
@@ -1993,14 +2072,18 @@
   anti-bloat:
     - description: 'remove pytest reference'
       change_function:
         'test_pandas_friendly_reshape': 'un-callable'
         'test_wide_dtype_for_and_widen': 'un-callable'
         'assert_no_pickling': 'un-callable'
       when: 'not use_pytest'
+    - description: 'remove IPython reference'
+      replacements_plain:
+        '"IPython" in sys.modules': 'False'
+      when: 'not use_ipython'
 
 - module-name: 'pendulum'
   data-files:
     empty_dir_structures:
       - 'locales'
     when: 'version("pendulum") >= (2,)'
 
@@ -2291,14 +2374,24 @@
         - 'pydantic.json'
         - 'pydantic.datetime_parse'
         - 'pydantic.dataclasses'
         - 'pydantic.class_validators'
         - 'pydantic.networks'
         - 'pydantic.errors'
 
+- module-name: 'pydantic.errors'
+  implicit-imports:
+    - depends:
+        - 'decimal'
+
+- module-name: 'pydantic.json'
+  implicit-imports:
+    - depends:
+        - 'uuid'
+
 - module-name: 'pydantic.typing'
   implicit-imports:
     - depends:
         - 'typing_extensions'
 
 - module-name: 'pyfiglet'
   implicit-imports:
@@ -2769,14 +2862,25 @@
         - '.JaroWinkler_py'
         - '.JaroWinkler_cpp'
         - '.Postfix_py'
         - '.Postfix_cpp'
         - '.Prefix_py'
         - '.Prefix_cpp'
 
+- module-name: 'rasterio._io'
+  implicit-imports:
+    - depends:
+        - 'rasterio.sample'
+        - 'rasterio.vrt'
+
+- module-name: 'rasterio._warp'
+  implicit-imports:
+    - depends:
+        - 'rasterio._features'
+
 - module-name: 'rdkit'
   anti-bloat:
     - description: 'remove IPython reference'
       replacements_plain:
         'kernel_name = get_ipython().__class__.__name__': 'raise NameError'
       when: 'not use_ipython'
 
@@ -4563,14 +4667,22 @@
   anti-bloat:
     - description: 'remove unittest reference'
       replacements_plain:
         'import unittest': ''
         'issubclass(func, unittest.TestCase)': 'False'
       when: 'not use_unittest'
 
+- module-name: 'torch._inductor.codecache'
+  anti-bloat:
+    - description: 'remove setuptools usage'
+      replacements_plain:
+        'from torch.utils import cpp_extension': ''
+      change_function:
+        'get_include_and_linking_paths': 'un-callable'
+
 - module-name: 'torch._inductor.codegen.common'
   anti-bloat:
     - description: 'remove setuptools usage'
       replacements_plain:
         'from .cpp import DTYPE_TO_CPP, INDEX_TYPE': 'raise ImportError'
         'from .cpp import DTYPE_TO_CPP': 'raise ImportError'
       when: 'not use_setuptools'
```

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `Nuitka-winsvc-1.6.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/reports/LicenseReport.rst.j2` & `Nuitka-winsvc-1.6.6/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/reports/Reports.py` & `Nuitka-winsvc-1.6.6/nuitka/reports/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/reports/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinBytesOperationSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinDictOperationSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinListOperationSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinParameterSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinStrOperationSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinTypeOperationSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/HardImportSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/ParameterSpecs.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/ParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/specs/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/Basics.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/commercial/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/data_composer/DataComposer.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/data_composer/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/data_composer/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/environments/CreateEnvironment.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/environments/Virtualenv.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/environments/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/general/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/general/dll_report/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/general/dll_report/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/general/find_module/FindModuleCode.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/general/find_module/FindModuleCode.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/general/find_module/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/onefile_compressor/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/onefile_compressor/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/profiler/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/profiler/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/scanning/DisplayPackageDLLs.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/scanning/DisplayPackageData.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/scanning/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/specialize/CTypeDescriptions.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/specialize/Common.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/specialize/SpecializeC.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/specialize/SpecializePython.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/specialize/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/Common.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/Constructs.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/OutputComparison.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/Pythons.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/RuntimeTracing.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/SearchModes.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/Valgrind.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/check_reference_counts/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/check_reference_counts/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/compare_with_cpython/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/compare_with_cpython/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/find_sxs_modules/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/find_sxs_modules/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/measure_construct_performance/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/measure_construct_performance/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/watch/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tools/watch/__main__.py` & `Nuitka-winsvc-1.6.6/nuitka/tools/watch/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/Building.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/Building.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ComplexCallHelperFunctions.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/Extractions.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/InternalModule.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/Operations.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationAssertStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationAssignmentStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationBooleanExpressions.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationCallExpressions.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationClasses.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationClasses3.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationComparisonExpressions.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationContractionExpressions.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationDictionaryCreation.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationExecStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationForLoopStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationFunctionStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationImportStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationLambdaExpressions.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationMatchStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationMultidist.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationNamespacePackages.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationPrintStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationSequenceCreation.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationSubscriptExpressions.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationTryExceptStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationTryFinallyStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationWhileLoopStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationWithStatements.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/ReformulationYieldExpressions.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/SourceHandling.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/SyntaxErrors.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/TreeHelpers.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/VariableClosure.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/tree/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/AppDirs.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/AppDirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/CStrings.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/CommandLineOptions.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Distributions.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Distributions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Download.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Execution.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Execution.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/FileOperations.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/FileOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Hashing.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Images.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Images.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Importing.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/InstalledPythons.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/InstalledPythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/InstanceCounters.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Jinja2.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Json.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/MacOSApp.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/MacOSApp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/MemoryUsage.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/ModuleNames.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/ReExecute.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/ReExecute.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Rest.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/SharedLibraries.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/SharedLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Shebang.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Signing.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/StaticLibraries.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/ThreadedExecutor.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Timing.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Utils.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/WindowsFileUsage.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/WindowsResources.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/Yaml.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/Yaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/nuitka/utils/__init__.py` & `Nuitka-winsvc-1.6.6/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/pyproject.toml` & `Nuitka-winsvc-1.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/setup.py` & `Nuitka-winsvc-1.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/AssertsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/AssignmentsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/AssignmentsTest32.py` & `Nuitka-winsvc-1.6.6/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/BranchingTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/BuiltinOverload.py` & `Nuitka-winsvc-1.6.6/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/BuiltinSuperTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/BuiltinsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ClassMinimalTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ClassesTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ClassesTest32.py` & `Nuitka-winsvc-1.6.6/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ClassesTest34.py` & `Nuitka-winsvc-1.6.6/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ComparisonChainsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ConstantsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ConstantsTest27.py` & `Nuitka-winsvc-1.6.6/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/DecoratorsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/DefaultParametersTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/DoubleDeletionsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/EmptyModuleTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ExceptionRaisingTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ExceptionRaisingTest32.py` & `Nuitka-winsvc-1.6.6/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ExceptionRaisingTest33.py` & `Nuitka-winsvc-1.6.6/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ExecEvalTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ExtremeClosureTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/FunctionObjectsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/FunctionsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/FunctionsTest32.py` & `Nuitka-winsvc-1.6.6/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/FunctionsTest_2.py` & `Nuitka-winsvc-1.6.6/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/FutureTest32.py` & `Nuitka-winsvc-1.6.6/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/GeneratorExpressionsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/GeneratorExpressionsTest_37.py` & `Nuitka-winsvc-1.6.6/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/GlobalStatementTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/HelloWorldTest_2.py` & `Nuitka-winsvc-1.6.6/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ImportingTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/InplaceOperationsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/InspectionTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/InspectionTest_35.py` & `Nuitka-winsvc-1.6.6/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/InspectionTest_36.py` & `Nuitka-winsvc-1.6.6/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/LambdasTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/LateClosureAssignmentTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ListContractionsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/LoopingTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/MainProgramsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ModuleAttributesTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/OperatorsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/OrderChecksTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/OrderChecksTest27.py` & `Nuitka-winsvc-1.6.6/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/OverflowFunctionsTest_2.py` & `Nuitka-winsvc-1.6.6/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ParameterErrorsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ParameterErrorsTest32.py` & `Nuitka-winsvc-1.6.6/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/PrintFutureTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/PrintingTest_2.py` & `Nuitka-winsvc-1.6.6/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/RecursionTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest27.py` & `Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest33.py` & `Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest35.py` & `Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest36.py` & `Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ReferencingTest_2.py` & `Nuitka-winsvc-1.6.6/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/SlotsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/ThreadedGeneratorsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/TrickAssignmentsTest32.py` & `Nuitka-winsvc-1.6.6/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/TrickAssignmentsTest35.py` & `Nuitka-winsvc-1.6.6/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/TrickAssignmentsTest_2.py` & `Nuitka-winsvc-1.6.6/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/TryContinueFinallyTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/TryExceptContinueTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/TryExceptFinallyTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/TryExceptFramesTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/TryReturnFinallyTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/TryYieldFinallyTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/UnicodeTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/UnpackingTest35.py` & `Nuitka-winsvc-1.6.6/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/VarargsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/WithStatementsTest.py` & `Nuitka-winsvc-1.6.6/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/YieldFromTest33.py` & `Nuitka-winsvc-1.6.6/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/run_all.py` & `Nuitka-winsvc-1.6.6/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/basics/run_xml.py` & `Nuitka-winsvc-1.6.6/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/onefile/HelloWorldTest.py` & `Nuitka-winsvc-1.6.6/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/onefile/KeyboardInterruptTest.py` & `Nuitka-winsvc-1.6.6/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/onefile/run_all.py` & `Nuitka-winsvc-1.6.6/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/ArgumentTypes.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/Attributes.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/Attributes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/Calls.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/Calls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/Conditions.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/Conditions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/DecodingOperations.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/DecodingOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/FormatStrings36.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/FormatStrings36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/HardImports.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/HardImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/HardImports_2.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/HardImports_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/Iterations.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/Len.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/Len.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/Operations.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/Subscripts.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/Subscripts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/optimizations/run_all.py` & `Nuitka-winsvc-1.6.6/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `Nuitka-winsvc-1.6.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `Nuitka-winsvc-1.6.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/run_all.py` & `Nuitka-winsvc-1.6.6/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/__init__.py` & `Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/bigkitty.py` & `Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/smallkitty.py` & `Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/speak/__init__.py` & `Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/speak/hello.py` & `Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/speak/miau.py` & `Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/sub_package/kitty/speak/purr.py` & `Nuitka-winsvc-1.6.6/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/top_level_attributes_3/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/packages/top_level_attributes_3/some_package/some_module.py` & `Nuitka-winsvc-1.6.6/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/plugins/code_signing/CodeSigningMain.py` & `Nuitka-winsvc-1.6.6/tests/plugins/code_signing/CodeSigningMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/plugins/data_files/DataFilesMain.py` & `Nuitka-winsvc-1.6.6/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/plugins/data_files/data_files_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/plugins/parameters/ParametersMain.py` & `Nuitka-winsvc-1.6.6/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/plugins/parameters/parameter-using-plugin.py` & `Nuitka-winsvc-1.6.6/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/plugins/run_all.py` & `Nuitka-winsvc-1.6.6/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/absolute_import/AbsoluteImportMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/absolute_import/foobar/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/absolute_import/foobar/foobar.py` & `Nuitka-winsvc-1.6.6/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/absolute_import/foobar/local.py` & `Nuitka-winsvc-1.6.6/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/absolute_import/foobar/util.py` & `Nuitka-winsvc-1.6.6/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports1/CasedImportingMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path1/Some_Module.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path2/some_module.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports1/path2/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports2/CasedImportingMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path1/some_module.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path1/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path2/Some_Module.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports3/CasedImportingMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path1/Some_Module.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path2/Some_Module.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/CyclicImportsMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/dash_import/DashImportMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/dash_import/dash-module.py` & `Nuitka-winsvc-1.6.6/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/dash_import/plus+module.py` & `Nuitka-winsvc-1.6.6/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/dash_main/Dash-Main.py` & `Nuitka-winsvc-1.6.6/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/deep/DeepProgramMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/DeepBrother.py` & `Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/DeepChild.py` & `Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/deep/some_package/deep_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/dunderinit_imports/package/SubModule.py` & `Nuitka-winsvc-1.6.6/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/dunderinit_imports/package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/import_variants/ImportVariationsMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/import_variants/some_package/Child1.py` & `Nuitka-winsvc-1.6.6/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/import_variants/some_package/Child2.py` & `Nuitka-winsvc-1.6.6/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/import_variants/some_package/Child3.py` & `Nuitka-winsvc-1.6.6/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/import_variants/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/main_raises/ErrorMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/main_raises/ErrorRaising.py` & `Nuitka-winsvc-1.6.6/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/main_raises2/ErrorInFunctionMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/main_raises2/ErrorRaising.py` & `Nuitka-winsvc-1.6.6/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_attributes/ModuleAttributesMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/Nearby1.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_exits/ErrorExitingModule.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_exits/Main.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/module_object_replacing/SelfReplacingModule.py` & `Nuitka-winsvc-1.6.6/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/foo/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/foo/__main__.py` & `Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/multiprocessing_using/foo/entry.py` & `Nuitka-winsvc-1.6.6/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/named_imports/NamedImportsMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/named_imports/some_package/SomeModule.py` & `Nuitka-winsvc-1.6.6/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/named_imports/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `Nuitka-winsvc-1.6.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_code/PackageInitCodeMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_code/some_package/SomeModule.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_code/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_contains_main/PackageContainsMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_contains_main/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_contains_main/local.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_init_import/PackageInitImportMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_init_import/some_package/PackageLocal.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_init_import/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/PackageInitIssueMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_missing_init/PackageMissingInitMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_missing_init/some_package/some_module.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_module_collision/Something/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_module_collision/something.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_overload/Main.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_overload/foo/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_overload/foo/bar.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_overload/foo/bar2.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_prevents_submodule/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_prevents_submodule/some_package/some_module.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_program/PackageAsMain/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/package_program/PackageAsMain/__main__.py` & `Nuitka-winsvc-1.6.6/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/pkgutil_usage/package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/plugin_import/PluginImportMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/plugin_import/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/plugin_import/some_package/some_module.py` & `Nuitka-winsvc-1.6.6/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/relative_import/RelativeImportMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/relative_import/dircache.py` & `Nuitka-winsvc-1.6.6/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/resource_reader37/ResourceReaderMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/resource_reader37/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/run_all.py` & `Nuitka-winsvc-1.6.6/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/pyexpat.py` & `Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/some_package/__init__.py` & `Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/some_package/normal_importing.py` & `Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/some_package/pyexpat.py` & `Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/stdlib_overload/some_package/star_importing.py` & `Nuitka-winsvc-1.6.6/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/syntax_errors/IndentationErroring.py` & `Nuitka-winsvc-1.6.6/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/syntax_errors/SyntaxErroring.py` & `Nuitka-winsvc-1.6.6/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/unicode_bom/UnicodeBomMain.py` & `Nuitka-winsvc-1.6.6/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/unicode_bom/unicode_bom.py` & `Nuitka-winsvc-1.6.6/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/programs/with space/Space Main.py` & `Nuitka-winsvc-1.6.6/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/reflected/compile_itself.py` & `Nuitka-winsvc-1.6.6/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/run-tests` & `Nuitka-winsvc-1.6.6/tests/run-tests`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/BrotliUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/CtypesUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/FlaskUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/GlfwUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/GtkUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/HexEncodingTest_2.py` & `Nuitka-winsvc-1.6.6/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/IdnaUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/LxmlUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/MatplotlibUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/MetadataPackagesUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/NumpyUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/OpenGLUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PandasUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PasslibUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PendulumUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PkgResourcesRequiresUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PmwUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PyQt5Plugins.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PyQt5SSLSupport.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PyQt5Using.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PyQt6Plugins.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PyQt6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PyQt6Using.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PySide6Plugins.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PySide6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/PySide6Using.py` & `Nuitka-winsvc-1.6.6/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/RsaUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/ShlibUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/SocketUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/TkInterUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/Urllib3Using.py` & `Nuitka-winsvc-1.6.6/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/Win32ComUsing.py` & `Nuitka-winsvc-1.6.6/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/run_all.py` & `Nuitka-winsvc-1.6.6/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/standalone/zip_importer/ZipImporterMain.py` & `Nuitka-winsvc-1.6.6/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/AsyncgenReturn36.py` & `Nuitka-winsvc-1.6.6/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/BreakWithoutLoop.py` & `Nuitka-winsvc-1.6.6/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/ClassReturn.py` & `Nuitka-winsvc-1.6.6/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/ClosureDel_2.py` & `Nuitka-winsvc-1.6.6/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/ContinueWithoutLoop.py` & `Nuitka-winsvc-1.6.6/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/DuplicateArgument.py` & `Nuitka-winsvc-1.6.6/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/ExecWithNesting_2.py` & `Nuitka-winsvc-1.6.6/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/FutureBraces.py` & `Nuitka-winsvc-1.6.6/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/FutureUnknown.py` & `Nuitka-winsvc-1.6.6/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/GeneratorExpressions38.py` & `Nuitka-winsvc-1.6.6/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/GeneratorReturn_2.py` & `Nuitka-winsvc-1.6.6/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/GlobalForParameter.py` & `Nuitka-winsvc-1.6.6/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/Importing32.py` & `Nuitka-winsvc-1.6.6/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/IndentationError.py` & `Nuitka-winsvc-1.6.6/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/LateFutureImport.py` & `Nuitka-winsvc-1.6.6/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/MisplacedFutureImport.py` & `Nuitka-winsvc-1.6.6/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/ModuleReturn.py` & `Nuitka-winsvc-1.6.6/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/NonAsciiWithoutEncoding_2.py` & `Nuitka-winsvc-1.6.6/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/NonlocalForParameter32.py` & `Nuitka-winsvc-1.6.6/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/NonlocalNotFound32.py` & `Nuitka-winsvc-1.6.6/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/StarImportExtra.py` & `Nuitka-winsvc-1.6.6/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/SyntaxError.py` & `Nuitka-winsvc-1.6.6/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/TryExceptAllNotLast.py` & `Nuitka-winsvc-1.6.6/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/TryFinallyContinue_37.py` & `Nuitka-winsvc-1.6.6/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/UnpackNoTuple.py` & `Nuitka-winsvc-1.6.6/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/UnpackTwoStars32.py` & `Nuitka-winsvc-1.6.6/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/YieldFromInModule.py` & `Nuitka-winsvc-1.6.6/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/YieldInAsync35.py` & `Nuitka-winsvc-1.6.6/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/YieldInGenexp38.py` & `Nuitka-winsvc-1.6.6/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/YieldInModule.py` & `Nuitka-winsvc-1.6.6/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6.4/tests/syntax/run_all.py` & `Nuitka-winsvc-1.6.6/tests/syntax/run_all.py`

 * *Files identical despite different names*

