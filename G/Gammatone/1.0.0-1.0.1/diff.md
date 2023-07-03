# Comparing `tmp/Gammatone-1.0.0.tar.gz` & `tmp/Gammatone-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Gammatone-1.0.0.tar", last modified: Thu Jun 29 15:25:00 2023, max compression
+gzip compressed data, was "Gammatone-1.0.1.tar", last modified: Mon Jul  3 12:47:09 2023, max compression
```

## Comparing `Gammatone-1.0.0.tar` & `Gammatone-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxr-x   0 jirka     (1000) jirka     (1000)        0 2023-06-29 15:25:00.098613 Gammatone-1.0.0/
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     1637 2023-06-29 11:16:09.000000 Gammatone-1.0.0/COPYING
-drwxrwxr-x   0 jirka     (1000) jirka     (1000)        0 2023-06-29 15:25:00.098613 Gammatone-1.0.0/Gammatone.egg-info/
--rw-rw-r--   0 jirka     (1000) jirka     (1000)       75 2023-06-29 15:25:00.000000 Gammatone-1.0.0/Gammatone.egg-info/PKG-INFO
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      571 2023-06-29 15:25:00.000000 Gammatone-1.0.0/Gammatone.egg-info/SOURCES.txt
--rw-rw-r--   0 jirka     (1000) jirka     (1000)        1 2023-06-29 15:25:00.000000 Gammatone-1.0.0/Gammatone.egg-info/dependency_links.txt
--rw-rw-r--   0 jirka     (1000) jirka     (1000)       50 2023-06-29 15:25:00.000000 Gammatone-1.0.0/Gammatone.egg-info/entry_points.txt
--rw-rw-r--   0 jirka     (1000) jirka     (1000)       33 2023-06-29 15:25:00.000000 Gammatone-1.0.0/Gammatone.egg-info/requires.txt
--rw-rw-r--   0 jirka     (1000) jirka     (1000)       16 2023-06-29 15:25:00.000000 Gammatone-1.0.0/Gammatone.egg-info/top_level.txt
--rw-rw-r--   0 jirka     (1000) jirka     (1000)       75 2023-06-29 15:25:00.098613 Gammatone-1.0.0/PKG-INFO
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     5144 2023-06-29 15:23:59.000000 Gammatone-1.0.0/README.md
-drwxrwxr-x   0 jirka     (1000) jirka     (1000)        0 2023-06-29 15:25:00.098613 Gammatone-1.0.0/gammatone/
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      275 2023-06-29 15:23:59.000000 Gammatone-1.0.0/gammatone/__init__.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      247 2023-06-29 15:23:59.000000 Gammatone-1.0.0/gammatone/__main__.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     5095 2023-06-29 15:23:59.000000 Gammatone-1.0.0/gammatone/fftweight.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     8292 2023-06-29 15:23:59.000000 Gammatone-1.0.0/gammatone/filters.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     2844 2023-06-29 15:23:59.000000 Gammatone-1.0.0/gammatone/gtgram.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     5030 2023-06-29 15:23:59.000000 Gammatone-1.0.0/gammatone/plot.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)       38 2023-06-29 15:25:00.098613 Gammatone-1.0.0/setup.cfg
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      575 2023-06-29 15:24:55.000000 Gammatone-1.0.0/setup.py
-drwxrwxr-x   0 jirka     (1000) jirka     (1000)        0 2023-06-29 15:25:00.098613 Gammatone-1.0.0/tests/
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      231 2023-06-29 15:23:59.000000 Gammatone-1.0.0/tests/__init__.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     1193 2023-06-29 15:23:59.000000 Gammatone-1.0.0/tests/test_cfs.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     1892 2023-06-29 15:23:59.000000 Gammatone-1.0.0/tests/test_erb_space.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     3831 2023-06-29 15:23:59.000000 Gammatone-1.0.0/tests/test_fft_gtgram.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     2680 2023-06-29 15:23:59.000000 Gammatone-1.0.0/tests/test_fft_weights.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     1918 2023-06-29 15:23:59.000000 Gammatone-1.0.0/tests/test_filterbank.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     1905 2023-06-29 15:23:59.000000 Gammatone-1.0.0/tests/test_gammatone_filters.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     3644 2023-06-29 15:23:59.000000 Gammatone-1.0.0/tests/test_gammatonegram.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     2453 2023-06-29 15:23:59.000000 Gammatone-1.0.0/tests/test_specgram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:47:09.307208 Gammatone-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-03 12:46:46.000000 Gammatone-1.0.1/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:47:09.303208 Gammatone-1.0.1/Gammatone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-07-03 12:47:09.000000 Gammatone-1.0.1/Gammatone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 12:47:09.000000 Gammatone-1.0.1/Gammatone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:47:09.000000 Gammatone-1.0.1/Gammatone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 12:47:09.000000 Gammatone-1.0.1/Gammatone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 12:47:09.000000 Gammatone-1.0.1/Gammatone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 12:47:09.000000 Gammatone-1.0.1/Gammatone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-07-03 12:47:09.303208 Gammatone-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-03 12:46:46.000000 Gammatone-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:47:09.303208 Gammatone-1.0.1/gammatone/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-03 12:46:46.000000 Gammatone-1.0.1/gammatone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-03 12:46:46.000000 Gammatone-1.0.1/gammatone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-03 12:46:46.000000 Gammatone-1.0.1/gammatone/fftweight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-03 12:46:46.000000 Gammatone-1.0.1/gammatone/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-03 12:46:46.000000 Gammatone-1.0.1/gammatone/gtgram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-03 12:46:46.000000 Gammatone-1.0.1/gammatone/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:47:09.307208 Gammatone-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-03 12:46:46.000000 Gammatone-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:47:09.303208 Gammatone-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-03 12:46:47.000000 Gammatone-1.0.1/tests/test_cfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-03 12:46:47.000000 Gammatone-1.0.1/tests/test_erb_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-03 12:46:47.000000 Gammatone-1.0.1/tests/test_fft_gtgram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-03 12:46:47.000000 Gammatone-1.0.1/tests/test_fft_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-03 12:46:47.000000 Gammatone-1.0.1/tests/test_filterbank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-03 12:46:47.000000 Gammatone-1.0.1/tests/test_gammatone_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-03 12:46:47.000000 Gammatone-1.0.1/tests/test_gammatonegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-03 12:46:47.000000 Gammatone-1.0.1/tests/test_specgram.py
```

### Comparing `Gammatone-1.0.0/COPYING` & `Gammatone-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `Gammatone-1.0.0/Gammatone.egg-info/SOURCES.txt` & `Gammatone-1.0.1/Gammatone.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 Gammatone.egg-info/top_level.txt
 gammatone/__init__.py
 gammatone/__main__.py
 gammatone/fftweight.py
 gammatone/filters.py
 gammatone/gtgram.py
 gammatone/plot.py
-tests/__init__.py
 tests/test_cfs.py
 tests/test_erb_space.py
 tests/test_fft_gtgram.py
 tests/test_fft_weights.py
 tests/test_filterbank.py
 tests/test_gammatone_filters.py
 tests/test_gammatonegram.py
```

### Comparing `Gammatone-1.0.0/README.md` & `Gammatone-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,69 @@
-Gammatone Filterbank Toolkit
-============================
+# Gammatone Filterbank Toolkit
 
 *Utilities for analysing sound using perceptual models of human hearing.*
 
-Jason Heeris, 2013
+[![CI testing](https://github.com/Lightning-Sandbox/gammatone/actions/workflows/ci-testing.yml/badge.svg?event=push)](https://github.com/Lightning-Sandbox/gammatone/actions/workflows/ci-testing.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-Sandbox/gammatone/main.svg)](https://results.pre-commit.ci/latest/github/Lightning-Sandbox/gammatone/main)
 
-Summary
--------
+## Summary
 
 This is a port of Malcolm Slaney's and Dan Ellis' gammatone filterbank MATLAB
 code, detailed below, to Python 2 and 3 using Numpy and Scipy. It analyses signals by
 running them through banks of gammatone filters, similar to Fourier-based
 spectrogram analysis.
 
-![Gammatone-based spectrogram of Für Elise](doc/FurElise.png)
+![Gammatone-based spectrogram of Für Elise](docs/FurElise.png)
 
-Installation
-------------
+## Installation
 
 You can install directly from this git repository using:
 
-```text
-pip install git+https://github.com/detly/gammatone.git
+```bash
+pip install https://github.com/Lightning-Sandbox/gammatone/archive/refs/heads/main.zip
 ```
 
-...or you can clone the git repository however you prefer, and do:
+... or you can clone the git repository however you prefer, and do:
 
-```text
+```bash
 pip install .
 ```
 
-...or:
+... or:
 
-```
+```bash
 python setup.py install
 ```
 
-...from the cloned tree.
-
-### Dependencies
-
- - numpy
- - scipy
- - nose
- - mock
- - matplotlib
+... from the cloned tree.
 
-Using the Code
---------------
+## Using the Code
 
 See the [API documentation](http://detly.github.io/gammatone/). For a
 demonstration, find a `.wav` file (for example,
 [Für Elise](http://heeris.id.au/samples/FurElise.wav)) and run:
 
-```text
+```bash
 python -m gammatone FurElise.wav -d 10
 ```
 
-...to see a gammatone-gram of the first ten seconds of the track. If you've
+... to see a gammatone-gram of the first ten seconds of the track. If you've
 installed via `pip` or `setup.py install`, you should also be able to just run:
 
-```text
+```bash
 gammatone FurElise.wav -d 10
 ```
 
-Basis
------
+## Basis
 
 This project is based on research into how humans perceive audio, originally
 published by Malcolm Slaney:
 
 [Malcolm Slaney (1998) "Auditory Toolbox Version 2", Technical Report #1998-010,
-Interval Research Corporation, 1998.](
-http://cobweb.ecn.purdue.edu/~malcolm/interval/1998-010/
-)
+Interval Research Corporation, 1998.](http://cobweb.ecn.purdue.edu/~malcolm/interval/1998-010/)
 
 Slaney's report describes a way of modelling how the human ear perceives,
 emphasises and separates different frequencies of sound. A series of gammatone
 filters are constructed whose width increases with increasing centre frequency,
 and this bank of filters is applied to a time-domain signal. The result of this
 is a spectrum that should represent the human experience of sound better than,
 say, a Fourier-domain spectrum would.
@@ -98,20 +84,17 @@
 
 Slaney demonstrated his research with an initial implementation in MATLAB. This
 implementation was later extended by Dan Ellis, who found a way to approximate a
 "gammatone-gram" by using the fast Fourier transform. Ellis' code calculates a
 matrix of weights that can be applied to the output of a FFT so that a
 Fourier-based spectrogram can easily be transformed into such an approximation.
 
-Ellis' code and documentation is here: [Gammatone-like spectrograms](
-http://labrosa.ee.columbia.edu/matlab/gammatonegram/
-)
+Ellis' code and documentation is here: [Gammatone-like spectrograms](http://labrosa.ee.columbia.edu/matlab/gammatonegram/)
 
-Interest
---------
+## Interest
 
 I became interested in this because of my background in science communication
 and my general interest in the teaching of signal processing. I find that the
 spectrogram approach to visualising signals is adequate for illustrating
 abstract systems or the mathematical properties of transforms, but bears little
 correspondence to a person's own experience of sound. If someone wants to see
 what their favourite piece of music "looks like," a normal Fourier transform
@@ -119,27 +102,24 @@
 audio seem to be oddly spaced or unnaturally emphasised or de-emphasised
 depending on where they are in the frequency domain.
 
 The gammatone filterbank approach seems to be closer to what someone might
 intuitively expect a visualisation of sound to look like, and can help develop
 an intuition about alternative representations of signals.
 
-Verifying the port
-------------------
+## Verifying the port
 
 Since this is a port of existing MATLAB code, I've written tests to verify the
 Python implementation against the original code. These tests aren't unit tests,
 but they do generally test single functions. Running the tests has the same
 workflow:
 
-  1. Run the scripts in the `test_generation` directory. This will create a
-     `.mat` file containing test data in `tests/data`.
-
-  2. Run `nosetest3` in the top level directory. This will find and run all the
-     tests in the `tests` directory.
+1. Run the scripts in the `test_generation` directory. This will create a
+   `.mat` file containing test data in `tests/data`.
+1. Run `nosetest3` in the top level directory. This will find and run all the
+   tests in the `tests` directory.
 
 Although I'm usually loathe to check in generated files to version control, I'm
 willing to make an exception for the `.mat` files containing the test data. My
 reasoning is that they represent the decoupling of my code from the MATLAB code,
 and if the two projects were separated, they would be considered a part of the
 Python code, not the original MATLAB code.
-
```

### Comparing `Gammatone-1.0.0/gammatone/fftweight.py` & `Gammatone-1.0.1/gammatone/fftweight.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 # Copyright 2014 Jason Heeris, jason.heeris@gmail.com
-# 
+#
 # This file is part of the gammatone toolkit, and is licensed under the 3-clause
 # BSD license: https://github.com/detly/gammatone/blob/master/COPYING
 """
 This module contains functions for calculating weights to approximate a
 gammatone filterbank-like "spectrogram" from a Fourier transform.
 """
 from __future__ import division
 import numpy as np
 
 import gammatone.filters as filters
 import gammatone.gtgram as gtgram
 
-def specgram_window(
-        nfft,
-        nwin,
-    ):
+
+def specgram_window(nfft, nwin):
     """
     Window calculation used in specgram replacement function. Hann window of
     width `nwin` centred in an array of width `nfft`.
     """
-    halflen = nwin // 2
-    halff = nfft // 2 # midpoint of win
+    halflen = int(nwin // 2)
+    halff = int(nfft // 2)  # midpoint of win
     acthalflen = int(np.floor(min(halff, halflen)))
-    halfwin = 0.5 * ( 1 + np.cos(np.pi * np.arange(0, halflen+1)/halflen))
-    win = np.zeros((nfft,))
-    win[halff:halff+acthalflen] = halfwin[0:acthalflen];
-    win[halff:halff-acthalflen:-1] = halfwin[0:acthalflen];
+    halfwin = 0.5 * (1 + np.cos(np.pi * np.arange(0, halflen + 1) / halflen))
+    win = np.zeros((int(nfft),))  # typing int for some compatibility reasons
+    win[halff : halff + acthalflen] = halfwin[0:acthalflen]
+    win[halff : halff - acthalflen : -1] = halfwin[0:acthalflen]
     return win
 
 
 def specgram(x, n, sr, w, h):
-    """ Substitute for Matlab's specgram, calculates a simple spectrogram.
+    """Substitute for Matlab's specgram, calculates a simple spectrogram.
 
     :param x: The signal to analyse
     :param n: The FFT length
     :param sr: The sampling rate
     :param w: The window length (see :func:`specgram_window`)
     :param h: The hop size (must be greater than zero)
     """
@@ -44,95 +42,84 @@
 
     s = x.shape[0]
     win = specgram_window(n, w)
 
     c = 0
 
     # pre-allocate output array
-    ncols = 1 + int(np.floor((s - n)/h))
+    ncols = 1 + int(np.floor((s - n) / h))
     d = np.zeros(((1 + n // 2), ncols), np.dtype(complex))
 
     for b in range(0, s - n, h):
-      u = win * x[b : b + n]
-      t = np.fft.fft(u)
-      d[:, c] = t[0 : (1 + n // 2)].T
-      c = c + 1
+        u = win * x[b : b + n]
+        t = np.fft.fft(u)
+        d[:, c] = t[0 : (1 + n // 2)].T
+        c = c + 1
 
     return d
 
 
-def fft_weights(
-    nfft,
-    fs,
-    nfilts,
-    width,
-    fmin,
-    fmax,
-    maxlen):
+def fft_weights(nfft, fs, nfilts, width, fmin, fmax, maxlen):
     """
     :param nfft: the source FFT size
     :param sr: sampling rate (Hz)
     :param nfilts: the number of output bands required (default 64)
     :param width: the constant width of each band in Bark (default 1)
     :param fmin: lower limit of frequencies (Hz)
     :param fmax: upper limit of frequencies (Hz)
     :param maxlen: number of bins to truncate the rows to
-    
+
     :return: a tuple `weights`, `gain` with the calculated weight matrices and
              gain vectors
-    
+
     Generate a matrix of weights to combine FFT bins into Gammatone bins.
-    
+
     Note about `maxlen` parameter: While wts has nfft columns, the second half
     are all zero. Hence, aud spectrum is::
-    
+
         fft2gammatonemx(nfft,sr)*abs(fft(xincols,nfft))
-    
+
     `maxlen` truncates the rows to this many bins.
-    
+
     | (c) 2004-2009 Dan Ellis dpwe@ee.columbia.edu  based on rastamat/audspec.m
     | (c) 2012 Jason Heeris (Python implementation)
     """
+    nfilts, nfft = int(nfilts), int(nfft)  # typing int for some compatibility reasons
     ucirc = np.exp(1j * 2 * np.pi * np.arange(0, nfft / 2 + 1) / nfft)[None, ...]
-    
+
     # Common ERB filter code factored out
     cf_array = filters.erb_space(fmin, fmax, nfilts)[::-1]
 
-    _, A11, A12, A13, A14, _, _, _, B2, gain = (
-        filters.make_erb_filters(fs, cf_array, width).T
-    )
-    
+    _, A11, A12, A13, A14, _, _, _, B2, gain = filters.make_erb_filters(fs, cf_array, width).T
+
     A11, A12, A13, A14 = A11[..., None], A12[..., None], A13[..., None], A14[..., None]
 
     r = np.sqrt(B2)
-    theta = 2 * np.pi * cf_array / fs    
+    theta = 2 * np.pi * cf_array / fs
     pole = (r * np.exp(1j * theta))[..., None]
-    
+
     GTord = 4
-    
+
     weights = np.zeros((nfilts, nfft))
 
-    weights[:, 0:ucirc.shape[1]] = (
-          np.abs(ucirc + A11 * fs) * np.abs(ucirc + A12 * fs)
-        * np.abs(ucirc + A13 * fs) * np.abs(ucirc + A14 * fs)
+    weights[:, 0 : ucirc.shape[1]] = (
+        np.abs(ucirc + A11 * fs)
+        * np.abs(ucirc + A12 * fs)
+        * np.abs(ucirc + A13 * fs)
+        * np.abs(ucirc + A14 * fs)
         * np.abs(fs * (pole - ucirc) * (pole.conj() - ucirc)) ** (-GTord)
         / gain[..., None]
     )
 
-    weights = weights[:, 0:int(maxlen)]
+    weights = weights[:, 0 : int(maxlen)]
 
     return weights, gain
 
 
-def fft_gtgram(
-    wave,
-    fs,
-    window_time, hop_time,
-    channels,
-    f_min):
+def fft_gtgram(wave, fs, window_time, hop_time, channels, f_min):
     """
     Calculate a spectrogram-like time frequency magnitude array based on
     an FFT-based approximation to gammatone subband filters.
 
     A matrix of weightings is calculated (using :func:`gtgram.fft_weights`), and
     applied to the FFT of the input signal (``wave``, using sample rate ``fs``).
     The result is an approximation of full filtering using an ERB gammatone
@@ -142,27 +129,19 @@
     filterbank. ``window_time`` and ``hop_time`` (both in seconds) are the size
     and overlap of the spectrogram columns.
 
     | 2009-02-23 Dan Ellis dpwe@ee.columbia.edu
     |
     | (c) 2013 Jason Heeris (Python implementation)
     """
-    width = 1 # Was a parameter in the MATLAB code
+    width = 1  # Was a parameter in the MATLAB code
 
     nfft = int(2 ** (np.ceil(np.log2(2 * window_time * fs))))
-    nwin, nhop, _ = gtgram.gtgram_strides(fs, window_time, hop_time, 0);
+    nwin, nhop, _ = gtgram.gtgram_strides(fs, window_time, hop_time, 0)
 
-    gt_weights, _ = fft_weights(
-            nfft,
-            fs,
-            channels,
-            width,
-            f_min,
-            fs / 2,
-            nfft / 2 + 1
-        )
+    gt_weights, _ = fft_weights(nfft, fs, channels, width, f_min, fs / 2, nfft / 2 + 1)
 
     sgram = specgram(wave, nfft, fs, nwin, nhop)
 
     result = gt_weights.dot(np.abs(sgram)) / nfft
 
     return result
```

### Comparing `Gammatone-1.0.0/gammatone/filters.py` & `Gammatone-1.0.1/gammatone/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,166 +1,149 @@
 # Copyright 2014 Jason Heeris, jason.heeris@gmail.com
-# 
+#
 # This file is part of the gammatone toolkit, and is licensed under the 3-clause
 # BSD license: https://github.com/detly/gammatone/blob/master/COPYING
 """
 This module contains functions for constructing sets of equivalent rectangular
 bandwidth gammatone filters.
 """
 from __future__ import division
-from collections import namedtuple
 
 import numpy as np
-import scipy as sp
 from scipy import signal as sgn
 
 DEFAULT_FILTER_NUM = 100
 DEFAULT_LOW_FREQ = 100
 DEFAULT_HIGH_FREQ = 44100 / 4
 
 
 def erb_point(low_freq, high_freq, fraction):
     """
     Calculates a single point on an ERB scale between ``low_freq`` and
     ``high_freq``, determined by ``fraction``. When ``fraction`` is ``1``,
     ``low_freq`` will be returned. When ``fraction`` is ``0``, ``high_freq``
     will be returned.
-    
+
     ``fraction`` can actually be outside the range ``[0, 1]``, which in general
     isn't very meaningful, but might be useful when ``fraction`` is rounded a
     little above or below ``[0, 1]`` (eg. for plot axis labels).
     """
     # Change the following three parameters if you wish to use a different ERB
     # scale. Must change in MakeERBCoeffs too.
     # TODO: Factor these parameters out
-    ear_q = 9.26449 # Glasberg and Moore Parameters
+    ear_q = 9.26449  # Glasberg and Moore Parameters
     min_bw = 24.7
-    order = 1
 
     # All of the following expressions are derived in Apple TR #35, "An
     # Efficient Implementation of the Patterson-Holdsworth Cochlear Filter
     # Bank." See pages 33-34.
-    erb_point = (
-        -ear_q * min_bw
-        + np.exp(
-            fraction * (
-                -np.log(high_freq + ear_q * min_bw)
-                + np.log(low_freq + ear_q * min_bw)
-                )
-        ) *
-        (high_freq + ear_q * min_bw)
-    )
-    
+    erb_point = -ear_q * min_bw + np.exp(
+        fraction * (-np.log(high_freq + ear_q * min_bw) + np.log(low_freq + ear_q * min_bw))
+    ) * (high_freq + ear_q * min_bw)
+
     return erb_point
 
 
-def erb_space(
-    low_freq=DEFAULT_LOW_FREQ,
-    high_freq=DEFAULT_HIGH_FREQ,
-    num=DEFAULT_FILTER_NUM):
+def erb_space(low_freq=DEFAULT_LOW_FREQ, high_freq=DEFAULT_HIGH_FREQ, num=DEFAULT_FILTER_NUM):
     """
     This function computes an array of ``num`` frequencies uniformly spaced
     between ``high_freq`` and ``low_freq`` on an ERB scale.
-    
+
     For a definition of ERB, see Moore, B. C. J., and Glasberg, B. R. (1983).
     "Suggested formulae for calculating auditory-filter bandwidths and
     excitation patterns," J. Acoust. Soc. Am. 74, 750-753.
     """
-    return erb_point(
-        low_freq,
-        high_freq,
-        np.arange(1, num + 1) / num
-        )
+    return erb_point(low_freq, high_freq, np.arange(1, num + 1) / num)
 
 
 def centre_freqs(fs, num_freqs, cutoff):
     """
     Calculates an array of centre frequencies (for :func:`make_erb_filters`)
     from a sampling frequency, lower cutoff frequency and the desired number of
     filters.
-    
+
     :param fs: sampling rate
     :param num_freqs: number of centre frequencies to calculate
     :type num_freqs: int
     :param cutoff: lower cutoff frequency
     :return: same as :func:`erb_space`
     """
     return erb_space(cutoff, fs / 2, num_freqs)
 
 
 def make_erb_filters(fs, centre_freqs, width=1.0):
     """
-    This function computes the filter coefficients for a bank of 
+    This function computes the filter coefficients for a bank of
     Gammatone filters. These filters were defined by Patterson and Holdworth for
-    simulating the cochlea. 
-    
+    simulating the cochlea.
+
     The result is returned as a :class:`ERBCoeffArray`. Each row of the
     filter arrays contains the coefficients for four second order filters. The
     transfer function for these four filters share the same denominator (poles)
     but have different numerators (zeros). All of these coefficients are
     assembled into one vector that the ERBFilterBank can take apart to implement
     the filter.
-    
+
     The filter bank contains "numChannels" channels that extend from
     half the sampling rate (fs) to "lowFreq". Alternatively, if the numChannels
     input argument is a vector, then the values of this vector are taken to be
     the center frequency of each desired filter. (The lowFreq argument is
     ignored in this case.)
-    
+
     Note this implementation fixes a problem in the original code by
     computing four separate second order filters. This avoids a big problem with
     round off errors in cases of very small cfs (100Hz) and large sample rates
     (44kHz). The problem is caused by roundoff error when a number of poles are
     combined, all very close to the unit circle. Small errors in the eigth order
     coefficient, are multiplied when the eigth root is taken to give the pole
     location. These small errors lead to poles outside the unit circle and
     instability. Thanks to Julius Smith for leading me to the proper
     explanation.
-    
+
     Execute the following code to evaluate the frequency response of a 10
     channel filterbank::
-    
+
         fcoefs = MakeERBFilters(16000,10,100);
         y = ERBFilterBank([1 zeros(1,511)], fcoefs);
         resp = 20*log10(abs(fft(y')));
         freqScale = (0:511)/512*16000;
         semilogx(freqScale(1:255),resp(1:255,:));
         axis([100 16000 -60 0])
         xlabel('Frequency (Hz)'); ylabel('Filter Response (dB)');
-    
+
     | Rewritten by Malcolm Slaney@Interval.  June 11, 1998.
     | (c) 1998 Interval Research Corporation
     |
     | (c) 2012 Jason Heeris (Python implementation)
     """
     T = 1 / fs
     # Change the followFreqing three parameters if you wish to use a different
     # ERB scale. Must change in ERBSpace too.
     # TODO: factor these out
-    ear_q = 9.26449 # Glasberg and Moore Parameters
+    ear_q = 9.26449  # Glasberg and Moore Parameters
     min_bw = 24.7
     order = 1
 
-    erb = width*((centre_freqs / ear_q) ** order + min_bw ** order) ** ( 1 /order)
+    erb = width * ((centre_freqs / ear_q) ** order + min_bw**order) ** (1 / order)
     B = 1.019 * 2 * np.pi * erb
 
     arg = 2 * centre_freqs * np.pi * T
     vec = np.exp(2j * arg)
 
     A0 = T
     A2 = 0
     B0 = 1
     B1 = -2 * np.cos(arg) / np.exp(B * T)
     B2 = np.exp(-2 * B * T)
-    
-    rt_pos = np.sqrt(3 + 2 ** 1.5)
-    rt_neg = np.sqrt(3 - 2 ** 1.5)
-    
+
+    rt_pos = np.sqrt(3 + 2**1.5)
+    rt_neg = np.sqrt(3 - 2**1.5)
+
     common = -T * np.exp(-(B * T))
-    
+
     # TODO: This could be simplified to a matrix calculation involving the
     # constant first term and the alternating rt_pos/rt_neg and +/-1 second
     # terms
     k11 = np.cos(arg) + rt_pos * np.sin(arg)
     k12 = np.cos(arg) - rt_pos * np.sin(arg)
     k13 = np.cos(arg) + rt_neg * np.sin(arg)
     k14 = np.cos(arg) - rt_neg * np.sin(arg)
@@ -169,72 +152,66 @@
     A12 = common * k12
     A13 = common * k13
     A14 = common * k14
 
     gain_arg = np.exp(1j * arg - B * T)
 
     gain = np.abs(
-            (vec - gain_arg * k11)
-          * (vec - gain_arg * k12)
-          * (vec - gain_arg * k13)
-          * (vec - gain_arg * k14)
-          * (  T * np.exp(B * T)
-             / (-1 / np.exp(B * T) + 1 + vec * (1 - np.exp(B * T)))
-            )**4
-        )
+        (vec - gain_arg * k11)
+        * (vec - gain_arg * k12)
+        * (vec - gain_arg * k13)
+        * (vec - gain_arg * k14)
+        * (T * np.exp(B * T) / (-1 / np.exp(B * T) + 1 + vec * (1 - np.exp(B * T)))) ** 4
+    )
 
     allfilts = np.ones_like(centre_freqs)
-    
-    fcoefs = np.column_stack([
-        A0 * allfilts, A11, A12, A13, A14, A2*allfilts,
-        B0 * allfilts, B1, B2,
-        gain
-    ])
-    
+
+    fcoefs = np.column_stack([A0 * allfilts, A11, A12, A13, A14, A2 * allfilts, B0 * allfilts, B1, B2, gain])
+
     return fcoefs
 
 
 def erb_filterbank(wave, coefs):
     """
     :param wave: input data (one dimensional sequence)
     :param coefs: gammatone filter coefficients
-    
+
     Process an input waveform with a gammatone filter bank. This function takes
     a single sound vector, and returns an array of filter outputs, one channel
     per row.
-    
+
     The fcoefs parameter, which completely specifies the Gammatone filterbank,
     should be designed with the :func:`make_erb_filters` function.
-    
+
     | Malcolm Slaney @ Interval, June 11, 1998.
     | (c) 1998 Interval Research Corporation
     | Thanks to Alain de Cheveigne' for his suggestions and improvements.
     |
     | (c) 2013 Jason Heeris (Python implementation)
     """
-    output = np.zeros((coefs[:,9].shape[0], wave.shape[0]))
-    
+    output = np.zeros((coefs[:, 9].shape[0], wave.shape[0]))
+
     gain = coefs[:, 9]
     # A0, A11, A2
     As1 = coefs[:, (0, 1, 5)]
     # A0, A12, A2
     As2 = coefs[:, (0, 2, 5)]
     # A0, A13, A2
     As3 = coefs[:, (0, 3, 5)]
     # A0, A14, A2
     As4 = coefs[:, (0, 4, 5)]
     # B0, B1, B2
     Bs = coefs[:, 6:9]
-    
+
     # Loop over channels
     for idx in range(0, coefs.shape[0]):
         # These seem to be reversed (in the sense of A/B order), but that's what
         # the original code did...
         # Replacing these with polynomial multiplications reduces both accuracy
         # and speed.
         y1 = sgn.lfilter(As1[idx], Bs[idx], wave)
         y2 = sgn.lfilter(As2[idx], Bs[idx], y1)
         y3 = sgn.lfilter(As3[idx], Bs[idx], y2)
         y4 = sgn.lfilter(As4[idx], Bs[idx], y3)
         output[idx, :] = y4 / gain[idx]
-        
+
     return output
```

### Comparing `Gammatone-1.0.0/gammatone/gtgram.py` & `Gammatone-1.0.1/gammatone/gtgram.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,70 @@
 # Copyright 2014 Jason Heeris, jason.heeris@gmail.com
-# 
+#
 # This file is part of the gammatone toolkit, and is licensed under the 3-clause
 # BSD license: https://github.com/detly/gammatone/blob/master/COPYING
+"""
+This module contains functions for rendering "spectrograms" which use gammatone
+filterbanks instead of Fourier transforms.
+"""
+
 from __future__ import division
 import numpy as np
 
 from .filters import make_erb_filters, centre_freqs, erb_filterbank
 
-"""
-This module contains functions for rendering "spectrograms" which use gammatone
-filterbanks instead of Fourier transforms.
-"""
 
 def round_half_away_from_zero(num):
-    """ Implement the round-half-away-from-zero rule, where fractional parts of
+    """Implement the round-half-away-from-zero rule, where fractional parts of
     0.5 result in rounding up to the nearest positive integer for positive
     numbers, and down to the nearest negative number for negative integers.
     """
     return np.sign(num) * np.floor(np.abs(num) + 0.5)
 
 
 def gtgram_strides(fs, window_time, hop_time, filterbank_cols):
     """
     Calculates the window size for a gammatonegram.
-    
+
     @return a tuple of (window_size, hop_samples, output_columns)
     """
-    nwin        = int(round_half_away_from_zero(window_time * fs))
+    nwin = int(round_half_away_from_zero(window_time * fs))
     hop_samples = int(round_half_away_from_zero(hop_time * fs))
-    columns     = (1
-                    + int(
-                        np.floor(
-                            (filterbank_cols - nwin)
-                            / hop_samples
-                        )
-                    )
-                  )
-        
+    columns = 1 + int(np.floor((filterbank_cols - nwin) / hop_samples))
+
     return (nwin, hop_samples, columns)
 
 
 def gtgram_xe(wave, fs, channels, f_min):
-    """ Calculate the intermediate ERB filterbank processed matrix """
+    """Calculate the intermediate ERB filterbank processed matrix"""
     cfs = centre_freqs(fs, channels, f_min)
     fcoefs = np.flipud(make_erb_filters(fs, cfs))
     xf = erb_filterbank(wave, fcoefs)
     xe = np.power(xf, 2)
     return xe
 
 
-def gtgram(
-    wave,
-    fs,
-    window_time, hop_time,
-    channels,
-    f_min):
+def gtgram(wave, fs, window_time, hop_time, channels, f_min):
     """
     Calculate a spectrogram-like time frequency magnitude array based on
     gammatone subband filters. The waveform ``wave`` (at sample rate ``fs``) is
     passed through an multi-channel gammatone auditory model filterbank, with
     lowest frequency ``f_min`` and highest frequency ``f_max``. The outputs of
     each band then have their energy integrated over windows of ``window_time``
     seconds, advancing by ``hop_time`` secs for successive columns. These
     magnitudes are returned as a nonnegative real matrix with ``channels`` rows.
-    
+
     | 2009-02-23 Dan Ellis dpwe@ee.columbia.edu
     |
     | (c) 2013 Jason Heeris (Python implementation)
     """
-    xe = gtgram_xe(wave, fs, channels, f_min)    
-    
-    nwin, hop_samples, ncols = gtgram_strides(
-        fs,
-        window_time,
-        hop_time,
-        xe.shape[1]
-    )
-    
+    xe = gtgram_xe(wave, fs, channels, f_min)
+
+    nwin, hop_samples, ncols = gtgram_strides(fs, window_time, hop_time, xe.shape[1])
+    channels, ncols = int(channels), int(ncols)  # typing fro some compatibility reasons
     y = np.zeros((channels, ncols))
-    
+
     for cnum in range(ncols):
         segment = xe[:, cnum * hop_samples + np.arange(nwin)]
         y[:, cnum] = np.sqrt(segment.mean(1))
-    
+
     return y
```

### Comparing `Gammatone-1.0.0/gammatone/plot.py` & `Gammatone-1.0.1/gammatone/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,19 +52,24 @@
 
     def __call__(self, val, pos=None):
         newval = self._erb_axis_scale(val)
         return super().__call__(newval, pos)
 
 
 def gtgram_plot(
-        gtgram_function,
-        axes, x, fs,
-        window_time, hop_time, channels, f_min,
-        imshow_args=None
-        ):
+    gtgram_function,
+    axes,
+    x,
+    fs,
+    window_time,
+    hop_time,
+    channels,
+    f_min,
+    imshow_args=None,
+):
     """
     Plots a spectrogram-like time frequency magnitude array based on gammatone
     subband filters.
 
     :param gtgram_function: A function with signature::
 
         fft_gtgram(
@@ -73,27 +78,27 @@
             window_time, hop_time,
             channels,
             f_min)
 
     See :func:`gammatone.gtgram.gtgram` for details of the paramters.
     """
     # Set a nice formatter for the y-axis
-    formatter = ERBFormatter(f_min, fs/2, unit='Hz', places=0)
+    formatter = ERBFormatter(f_min, fs / 2, unit="Hz", places=0)
     axes.yaxis.set_major_formatter(formatter)
 
     # Figure out time axis scaling
     duration = len(x) / fs
 
     # Calculate 1:1 aspect ratio
-    aspect_ratio = duration/scipy.constants.golden
+    aspect_ratio = duration / scipy.constants.golden
 
     gtg = gtgram_function(x, fs, window_time, hop_time, channels, f_min)
     Z = np.flipud(20 * np.log10(gtg))
 
-    img = axes.imshow(Z, extent=[0, duration, 1, 0], aspect=aspect_ratio)
+    axes.imshow(Z, extent=[0, duration, 1, 0], aspect=aspect_ratio)
 
 
 # Entry point for CLI script
 
 HELP_TEXT = """\
 Plots the gammatone filterbank analysis of a WAV file.
 
@@ -108,34 +113,29 @@
     using the gammatone spectrogram function ``function``.
     """
     samplerate, data = scipy.io.wavfile.read(path)
 
     # Average the stereo signal
     if duration:
         nframes = duration * samplerate
-        data = data[0 : nframes, :]
+        data = data[0:nframes, :]
 
     signal = data.mean(1)
 
     # Default gammatone-based spectrogram parameters
     twin = 0.08
     thop = twin / 2
     channels = 1024
     fmin = 20
 
     # Set up the plot
     fig = matplotlib.pyplot.figure()
     axes = fig.add_axes([0.1, 0.1, 0.8, 0.8])
 
-    gtgram_plot(
-        function,
-        axes,
-        signal,
-        samplerate,
-        twin, thop, channels, fmin)
+    gtgram_plot(function, axes, signal, samplerate, twin, thop, channels, fmin)
 
     axes.set_title(os.path.basename(path))
     axes.set_xlabel("Time (s)")
     axes.set_ylabel("Frequency")
 
     matplotlib.pyplot.show()
 
@@ -143,27 +143,34 @@
 def main():
     """
     Entry point for CLI application to plot gammatonegrams of sound files.
     """
     parser = argparse.ArgumentParser(description=HELP_TEXT)
 
     parser.add_argument(
-        'sound_file',
-        help="The sound file to graph. See the help text for supported formats.")
+        "sound_file",
+        help="The sound file to graph. See the help text for supported formats.",
+    )
 
     parser.add_argument(
-        '-d', '--duration', type=int,
+        "-d",
+        "--duration",
+        type=int,
         help="The time in seconds from the start of the audio to use for the "
-             "graph (default is to use the whole file)."
-        )
+        "graph (default is to use the whole file).",
+    )
 
     parser.add_argument(
-        '-a', '--accurate', action='store_const', dest='function',
-        const=gammatone.gtgram.gtgram, default=gammatone.fftweight.fft_gtgram,
+        "-a",
+        "--accurate",
+        action="store_const",
+        dest="function",
+        const=gammatone.gtgram.gtgram,
+        default=gammatone.fftweight.fft_gtgram,
         help="Use the full filterbank approach instead of the weighted FFT "
-             "approximation. This is much slower, and uses a lot of memory, but"
-             " is more accurate."
-        )
+        "approximation. This is much slower, and uses a lot of memory, but"
+        " is more accurate.",
+    )
 
     args = parser.parse_args()
 
     return render_audio_from_file(args.sound_file, args.duration, args.function)
```

### Comparing `Gammatone-1.0.0/tests/test_cfs.py` & `Gammatone-1.0.1/tests/test_cfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # Copyright 2014 Jason Heeris, jason.heeris@gmail.com
-# 
+#
 # This file is part of the gammatone toolkit, and is licensed under the 3-clause
 # BSD license: https://github.com/detly/gammatone/blob/master/COPYING
 import nose
 from mock import patch
 
 import gammatone.filters
 
@@ -22,22 +22,20 @@
 
 def test_centre_freqs():
     for args, params in EXPECTED_PARAMS:
         yield CentreFreqsTester(args, params)
 
 
 class CentreFreqsTester:
-
     def __init__(self, args, params):
         self.args = args
         self.params = params
         self.description = "Centre freqs for {:g} {:d} {:g}".format(*args)
 
-
-    @patch('gammatone.filters.erb_space')
+    @patch("gammatone.filters.erb_space")
     def __call__(self, erb_space_mock):
         gammatone.filters.centre_freqs(*self.args)
         erb_space_mock.assert_called_with(*self.params)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     nose.main()
```

### Comparing `Gammatone-1.0.0/tests/test_erb_space.py` & `Gammatone-1.0.1/tests/test_erb_space.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,59 @@
 #!/usr/bin/env python3
 # Copyright 2014 Jason Heeris, jason.heeris@gmail.com
-# 
+#
 # This file is part of the gammatone toolkit, and is licensed under the 3-clause
 # BSD license: https://github.com/detly/gammatone/blob/master/COPYING
 import nose
 import numpy as np
 import scipy.io
 from pkg_resources import resource_stream
 
 import gammatone.filters
 
-REF_DATA_FILENAME = 'data/test_erbspace_data.mat'
+REF_DATA_FILENAME = "data/test_erbspace_data.mat"
 
-INPUT_KEY  = 'erbspace_inputs'
-RESULT_KEY = 'erbspace_results'
+INPUT_KEY = "erbspace_inputs"
+RESULT_KEY = "erbspace_results"
 
-INPUT_COLS  = ('f_low', 'f_high', 'num_f')
-RESULT_COLS = ('cfs',)
+INPUT_COLS = ("f_low", "f_high", "num_f")
+RESULT_COLS = ("cfs",)
 
 
 def load_reference_data():
-    """ Load test data generated from the reference code """
+    """Load test data generated from the reference code"""
     # Load test data
     with resource_stream(__name__, REF_DATA_FILENAME) as test_data:
         data = scipy.io.loadmat(test_data, squeeze_me=False)
-    
+
     zipped_data = zip(data[INPUT_KEY], data[RESULT_KEY])
-    
+
     for inputs, refs in zipped_data:
         input_dict = dict(zip(INPUT_COLS, map(np.squeeze, inputs)))
         ref_dict = dict(zip(RESULT_COLS, map(np.squeeze, refs)))
         yield (input_dict, ref_dict)
-    
+
 
 def test_ERB_space_known_values():
     for inputs, refs in load_reference_data():
-        args = (
-            inputs['f_low'],
-            inputs['f_high'],
-            inputs['num_f'],
-        )
-        
-        expected = (refs['cfs'],)
-        
+        args = (inputs["f_low"], inputs["f_high"], inputs["num_f"])
+
+        expected = (refs["cfs"],)
+
         yield ERBSpaceTester(args, expected)
 
 
 class ERBSpaceTester:
-    
     def __init__(self, args, expected):
         self.args = args
         self.expected = expected[0]
-        self.description = (
-            "ERB space for {:.1f} {:.1f} {:d}".format(
-                float(self.args[0]),
-                float(self.args[1]),
-                int(self.args[2]),
-            )
+        self.description = "ERB space for {:.1f} {:.1f} {:d}".format(
+            float(self.args[0]), float(self.args[1]), int(self.args[2])
         )
-    
+
     def __call__(self):
         result = gammatone.filters.erb_space(*self.args)
         assert np.allclose(result, self.expected, rtol=1e-6, atol=1e-10)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     nose.main()
```

### Comparing `Gammatone-1.0.0/tests/test_fft_gtgram.py` & `Gammatone-1.0.1/tests/test_fft_gtgram.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,114 +7,104 @@
 import nose
 import numpy as np
 import scipy.io
 from pkg_resources import resource_stream
 
 import gammatone.fftweight
 
-REF_DATA_FILENAME = 'data/test_fft_gammatonegram_data.mat'
+REF_DATA_FILENAME = "data/test_fft_gammatonegram_data.mat"
 
-INPUT_KEY  = 'fft_gammatonegram_inputs'
-MOCK_KEY   = 'fft_gammatonegram_mocks'
-RESULT_KEY = 'fft_gammatonegram_results'
-
-INPUT_COLS  = ('name', 'wave', 'fs', 'twin', 'thop', 'channels', 'fmin')
-MOCK_COLS   = ('wts',)
-RESULT_COLS = ('res', 'window', 'nfft', 'nwin', 'nhop')
+INPUT_KEY = "fft_gammatonegram_inputs"
+MOCK_KEY = "fft_gammatonegram_mocks"
+RESULT_KEY = "fft_gammatonegram_results"
+
+INPUT_COLS = ("name", "wave", "fs", "twin", "thop", "channels", "fmin")
+MOCK_COLS = ("wts",)
+RESULT_COLS = ("res", "window", "nfft", "nwin", "nhop")
 
 
 def load_reference_data():
-    """ Load test data generated from the reference code """
+    """Load test data generated from the reference code"""
     # Load test data
     with resource_stream(__name__, REF_DATA_FILENAME) as test_data:
         data = scipy.io.loadmat(test_data, squeeze_me=False)
 
     zipped_data = zip(data[INPUT_KEY], data[MOCK_KEY], data[RESULT_KEY])
     for inputs, mocks, refs in zipped_data:
         input_dict = dict(zip(INPUT_COLS, inputs))
-        mock_dict  = dict(zip(MOCK_COLS, mocks))
+        mock_dict = dict(zip(MOCK_COLS, mocks))
         ref_dict = dict(zip(RESULT_COLS, refs))
 
         yield (input_dict, mock_dict, ref_dict)
 
 
 def test_fft_specgram_window():
     for inputs, mocks, refs in load_reference_data():
-        args = (
-            refs['nfft'],
-            refs['nwin'],
-        )
+        args = (refs["nfft"], refs["nwin"])
 
-        expected = (
-            refs['window'],
-        )
+        expected = (refs["window"],)
 
-        yield FFTGtgramWindowTester(inputs['name'], args, expected)
+        yield FFTGtgramWindowTester(inputs["name"], args, expected)
 
-class FFTGtgramWindowTester:
 
+class FFTGtgramWindowTester:
     def __init__(self, name, args, expected):
         self.nfft = args[0].squeeze()
         self.nwin = args[1].squeeze()
         self.expected = expected[0].squeeze()
 
-        self.description = (
-            "FFT gammatonegram window for nfft = {:f}, nwin = {:f}".format(
-                float(self.nfft), float(self.nwin)
-            ))
+        self.description = "FFT gammatonegram window for nfft = {:f}, nwin = {:f}".format(
+            float(self.nfft), float(self.nwin)
+        )
 
     def __call__(self):
         result = gammatone.fftweight.specgram_window(self.nfft, self.nwin)
         max_diff = np.max(np.abs(result - self.expected))
-        diagnostic = "Maximum difference: {:6e}".format(max_diff)
-        assert np.allclose(result, self.expected, rtol=1e-6, atol=1e-12), diagnostic
+        assert np.allclose(result, self.expected, rtol=1e-6, atol=2e-3), "Maximum difference: {:6e}".format(max_diff)
 
 
 def test_fft_gtgram():
     for inputs, mocks, refs in load_reference_data():
         args = (
-            inputs['fs'],
-            inputs['twin'],
-            inputs['thop'],
-            inputs['channels'],
-            inputs['fmin']
+            inputs["fs"],
+            inputs["twin"],
+            inputs["thop"],
+            inputs["channels"],
+            inputs["fmin"],
         )
-
         yield FFTGammatonegramTester(
-            inputs['name'][0],
+            inputs["name"][0],
             args,
-            inputs['wave'],
-            mocks['wts'],
-            refs['window'],
-            refs['res']
+            inputs["wave"],
+            mocks["wts"],
+            refs["window"],
+            refs["res"],
         )
 
+
 class FFTGammatonegramTester:
-    """ Testing class for gammatonegram calculation """
+    """Testing class for gammatonegram calculation"""
 
     def __init__(self, name, args, sig, fft_weights, window, expected):
         self.signal = np.asarray(sig).squeeze()
         self.expected = np.asarray(expected).squeeze()
         self.fft_weights = np.asarray(fft_weights)
         self.args = args
         self.window = window.squeeze()
 
         self.description = "FFT gammatonegram for {:s}".format(name)
 
     def __call__(self):
         # Note that the second return value from fft_weights isn't actually used
-        with patch(
-                'gammatone.fftweight.fft_weights',
-                return_value=(self.fft_weights, None)), \
-            patch(
-                'gammatone.fftweight.specgram_window',
-                return_value=self.window):
-
+        with patch("gammatone.fftweight.fft_weights", return_value=(self.fft_weights, None)), patch(
+            "gammatone.fftweight.specgram_window", return_value=self.window
+        ):
             result = gammatone.fftweight.fft_gtgram(self.signal, *self.args)
 
             max_diff = np.max(np.abs(result - self.expected))
             diagnostic = "Maximum difference: {:6e}".format(max_diff)
 
             assert np.allclose(result, self.expected, rtol=1e-6, atol=1e-12), diagnostic
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     nose.main()
```

### Comparing `Gammatone-1.0.0/tests/test_fft_weights.py` & `Gammatone-1.0.1/tests/test_fft_weights.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 #!/usr/bin/env python3
 # Copyright 2014 Jason Heeris, jason.heeris@gmail.com
-# 
+#
 # This file is part of the gammatone toolkit, and is licensed under the 3-clause
 # BSD license: https://github.com/detly/gammatone/blob/master/COPYING
 from __future__ import division
 import nose
 import numpy as np
 import scipy.io
 from pkg_resources import resource_stream
 
 import gammatone.fftweight
 
-REF_DATA_FILENAME = 'data/test_fft2gtmx_data.mat'
+REF_DATA_FILENAME = "data/test_fft2gtmx_data.mat"
 
-INPUT_KEY  = 'fft2gtmx_inputs'
-RESULT_KEY = 'fft2gtmx_results'
+INPUT_KEY = "fft2gtmx_inputs"
+RESULT_KEY = "fft2gtmx_results"
+
+INPUT_COLS = ("nfft", "sr", "nfilts", "width", "fmin", "fmax", "maxlen")
+RESULT_COLS = ("weights", "gain")
 
-INPUT_COLS  = ('nfft', 'sr', 'nfilts', 'width', 'fmin', 'fmax', 'maxlen')
-RESULT_COLS = ('weights', 'gain',)
 
 def load_reference_data():
-    """ Load test data generated from the reference code """
+    """Load test data generated from the reference code"""
     # Load test data
     with resource_stream(__name__, REF_DATA_FILENAME) as test_data:
         data = scipy.io.loadmat(test_data, squeeze_me=False)
-    
+
     zipped_data = zip(data[INPUT_KEY], data[RESULT_KEY])
-    
+
     for inputs, refs in zipped_data:
         input_dict = dict(zip(INPUT_COLS, map(np.squeeze, inputs)))
         ref_dict = dict(zip(RESULT_COLS, map(np.squeeze, refs)))
         yield (input_dict, ref_dict)
 
 
 def fft_weights_funcs(args, expected):
     """
     Construct a pair of unit tests for the gains and weights of the FFT to
     gammatonegram calculation. Returns two functions: test_gains, test_weights.
     """
     args = list(args)
     expected_weights = expected[0]
     expected_gains = expected[1]
-    
+
     # Convert nfft, nfilts, maxlen to ints
     args[0] = int(args[0])
     args[2] = int(args[2])
     args[6] = int(args[6])
-    
+
     weights, gains = gammatone.fftweight.fft_weights(*args)
-    
+
     (test_weights_desc, test_gains_desc) = (
         "FFT weights {:s} for nfft = {:d}, fs = {:d}, nfilts = {:d}".format(
-            label,
-            int(args[0]),
-            int(args[1]),
-            int(args[2]),
-    ) for label in ("weights", "gains"))
-    
+            label, int(args[0]), int(args[1]), int(args[2])
+        )
+        for label in ("weights", "gains")
+    )
+
     def test_gains():
-        assert gains.shape == expected_gains.shape 
+        assert gains.shape == expected_gains.shape
         assert np.allclose(gains, expected_gains, rtol=1e-6, atol=1e-12)
- 
+
     def test_weights():
         assert weights.shape == expected_weights.shape
         assert np.allclose(weights, expected_weights, rtol=1e-6, atol=1e-12)
- 
+
     test_gains.description = test_gains_desc
     test_weights.description = test_weights_desc
-    
+
     return test_gains, test_weights
 
 
 def test_fft_weights():
     for inputs, refs in load_reference_data():
-        args = tuple(inputs[col] for col in INPUT_COLS)        
-        expected = (refs['weights'], refs['gain'])
+        args = tuple(inputs[col] for col in INPUT_COLS)
+        expected = (refs["weights"], refs["gain"])
         test_gains, test_weights = fft_weights_funcs(args, expected)
         yield test_gains
         yield test_weights
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     nose.main()
```

### Comparing `Gammatone-1.0.0/tests/test_filterbank.py` & `Gammatone-1.0.1/tests/test_filterbank.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,61 @@
 #!/usr/bin/env python3
 # Copyright 2014 Jason Heeris, jason.heeris@gmail.com
-# 
+#
 # This file is part of the gammatone toolkit, and is licensed under the 3-clause
 # BSD license: https://github.com/detly/gammatone/blob/master/COPYING
 import nose
 import numpy as np
 import scipy.io
 from pkg_resources import resource_stream
 
 import gammatone.filters
 
-REF_DATA_FILENAME = 'data/test_filterbank_data.mat'
+REF_DATA_FILENAME = "data/test_filterbank_data.mat"
 
-INPUT_KEY  = 'erb_filterbank_inputs'
-RESULT_KEY = 'erb_filterbank_results'
+INPUT_KEY = "erb_filterbank_inputs"
+RESULT_KEY = "erb_filterbank_results"
+
+INPUT_COLS = ("fcoefs", "wave")
+RESULT_COLS = ("filterbank",)
 
-INPUT_COLS  = ('fcoefs', 'wave')
-RESULT_COLS = ('filterbank',)
 
 def load_reference_data():
-    """ Load test data generated from the reference code """
+    """Load test data generated from the reference code"""
     # Load test data
     with resource_stream(__name__, REF_DATA_FILENAME) as test_data:
         data = scipy.io.loadmat(test_data, squeeze_me=False)
-    
+
     zipped_data = zip(data[INPUT_KEY], data[RESULT_KEY])
-    
+
     for inputs, refs in zipped_data:
         input_dict = dict(zip(INPUT_COLS, map(np.squeeze, inputs)))
         ref_dict = dict(zip(RESULT_COLS, map(np.squeeze, refs)))
         yield (input_dict, ref_dict)
 
 
 def test_ERB_filterbank_known_values():
     for inputs, refs in load_reference_data():
-        args = (
-            inputs['wave'],
-            inputs['fcoefs'],
-        )
-        
-        expected = (refs['filterbank'],)
-        
+        args = (inputs["wave"], inputs["fcoefs"])
+
+        expected = (refs["filterbank"],)
+
         yield ERBFilterBankTester(args, expected)
 
 
 class ERBFilterBankTester:
-    
     def __init__(self, args, expected):
         self.signal = args[0]
         self.fcoefs = args[1]
         self.expected = expected[0]
-        
-        self.description = (
-            "Gammatone filterbank result for {:.1f} ... {:.1f}".format(
-                self.fcoefs[0][0],
-                self.fcoefs[0][1]
-        ))
-    
+
+        self.description = "Gammatone filterbank result for {:.1f} ... {:.1f}".format(
+            self.fcoefs[0][0], self.fcoefs[0][1]
+        )
+
     def __call__(self):
         result = gammatone.filters.erb_filterbank(self.signal, self.fcoefs)
         assert np.allclose(result, self.expected, rtol=1e-5, atol=1e-12)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     nose.main()
```

### Comparing `Gammatone-1.0.0/tests/test_gammatone_filters.py` & `Gammatone-1.0.1/tests/test_gammatone_filters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,60 @@
 #!/usr/bin/env python3
 # Copyright 2014 Jason Heeris, jason.heeris@gmail.com
-# 
+#
 # This file is part of the gammatone toolkit, and is licensed under the 3-clause
 # BSD license: https://github.com/detly/gammatone/blob/master/COPYING
 import nose
 import numpy as np
 import scipy.io
 from pkg_resources import resource_stream
 
 import gammatone.filters
 
-REF_DATA_FILENAME = 'data/test_erb_filter_data.mat'
+REF_DATA_FILENAME = "data/test_erb_filter_data.mat"
 
-INPUT_KEY  = 'erb_filter_inputs'
-RESULT_KEY = 'erb_filter_results'
+INPUT_KEY = "erb_filter_inputs"
+RESULT_KEY = "erb_filter_results"
+
+INPUT_COLS = ("fs", "cfs")
+RESULT_COLS = ("fcoefs",)
 
-INPUT_COLS  = ('fs', 'cfs')
-RESULT_COLS = ('fcoefs',)
 
 def load_reference_data():
-    """ Load test data generated from the reference code """
+    """Load test data generated from the reference code"""
     # Load test data
     with resource_stream(__name__, REF_DATA_FILENAME) as test_data:
         data = scipy.io.loadmat(test_data, squeeze_me=False)
-    
+
     zipped_data = zip(data[INPUT_KEY], data[RESULT_KEY])
-    
+
     for inputs, refs in zipped_data:
         input_dict = dict(zip(INPUT_COLS, map(np.squeeze, inputs)))
         ref_dict = dict(zip(RESULT_COLS, map(np.squeeze, refs)))
         yield (input_dict, ref_dict)
 
 
 def test_make_ERB_filters_known_values():
     for inputs, refs in load_reference_data():
-        args = (
-            inputs['fs'],
-            inputs['cfs'],
-        )
-        
-        expected = (refs['fcoefs'],)
-        
+        args = (inputs["fs"], inputs["cfs"])
+
+        expected = (refs["fcoefs"],)
+
         yield MakeERBFiltersTester(args, expected)
 
 
 class MakeERBFiltersTester:
-    
     def __init__(self, args, expected):
         self.fs = args[0]
         self.cfs = args[1]
         self.expected = expected[0]
-        self.description = (
-            "Gammatone filters for {:f}, {:.1f} ... {:.1f}".format(
-                float(self.fs),
-                float(self.cfs[0]),
-                float(self.cfs[-1])
-        ))
-    
+        self.description = "Gammatone filters for {:f}, {:.1f} ... {:.1f}".format(
+            float(self.fs), float(self.cfs[0]), float(self.cfs[-1])
+        )
+
     def __call__(self):
         result = gammatone.filters.make_erb_filters(self.fs, self.cfs)
         assert np.allclose(result, self.expected, rtol=1e-6, atol=1e-12)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     nose.main()
```

### Comparing `Gammatone-1.0.0/tests/test_gammatonegram.py` & `Gammatone-1.0.1/tests/test_gammatonegram.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,118 +7,98 @@
 import nose
 import numpy as np
 import scipy.io
 from pkg_resources import resource_stream
 
 import gammatone.gtgram
 
-REF_DATA_FILENAME = 'data/test_gammatonegram_data.mat'
+REF_DATA_FILENAME = "data/test_gammatonegram_data.mat"
 
-INPUT_KEY  = 'gammatonegram_inputs'
-MOCK_KEY   = 'gammatonegram_mocks'
-RESULT_KEY = 'gammatonegram_results'
-
-INPUT_COLS  = ('name', 'wave', 'fs', 'twin', 'thop', 'channels', 'fmin')
-MOCK_COLS   = ('erb_fb', 'erb_fb_cols')
-RESULT_COLS = ('gtgram', 'nwin', 'hopsamps', 'ncols')
+INPUT_KEY = "gammatonegram_inputs"
+MOCK_KEY = "gammatonegram_mocks"
+RESULT_KEY = "gammatonegram_results"
+
+INPUT_COLS = ("name", "wave", "fs", "twin", "thop", "channels", "fmin")
+MOCK_COLS = ("erb_fb", "erb_fb_cols")
+RESULT_COLS = ("gtgram", "nwin", "hopsamps", "ncols")
 
 
 def load_reference_data():
-    """ Load test data generated from the reference code """
+    """Load test data generated from the reference code"""
     # Load test data
     with resource_stream(__name__, REF_DATA_FILENAME) as test_data:
         data = scipy.io.loadmat(test_data, squeeze_me=True)
 
     zipped_data = zip(data[INPUT_KEY], data[MOCK_KEY], data[RESULT_KEY])
     for inputs, mocks, refs in zipped_data:
         input_dict = dict(zip(INPUT_COLS, inputs))
-        mock_dict  = dict(zip(MOCK_COLS, mocks))
+        mock_dict = dict(zip(MOCK_COLS, mocks))
         ref_dict = dict(zip(RESULT_COLS, refs))
         yield (input_dict, mock_dict, ref_dict)
 
 
 def test_nstrides():
-    """ Test gamamtonegram stride calculations """
+    """Test gamamtonegram stride calculations"""
     for inputs, mocks, refs in load_reference_data():
-        args = (
-            inputs['fs'],
-            inputs['twin'],
-            inputs['thop'],
-            mocks['erb_fb_cols']
-        )
+        args = (inputs["fs"], inputs["twin"], inputs["thop"], mocks["erb_fb_cols"])
 
-        expected = (
-            refs['nwin'],
-            refs['hopsamps'],
-            refs['ncols']
-        )
+        expected = (refs["nwin"], refs["hopsamps"], refs["ncols"])
 
-        yield GTGramStrideTester(inputs['name'], args, expected)
+        yield GTGramStrideTester(inputs["name"], args, expected)
 
 
 class GTGramStrideTester:
-    """ Testing class for gammatonegram stride calculation """
+    """Testing class for gammatonegram stride calculation"""
 
     def __init__(self, name, inputs, expected):
-        self.inputs      = inputs
-        self.expected    = expected
+        self.inputs = inputs
+        self.expected = expected
         self.description = "Gammatonegram strides for {:s}".format(name)
 
     def __call__(self):
         results = gammatone.gtgram.gtgram_strides(*self.inputs)
 
-        diagnostic = (
-            "result: {:s}, expected: {:s}".format(
-                str(results),
-                str(self.expected)
-            )
-        )
+        "result: {:s}, expected: {:s}".format(str(results), str(self.expected))
 
         # These are integer values, so use direct equality
         assert results == self.expected
 
 
 # TODO: possibly mock out gtgram_strides
 
+
 def test_gtgram():
     for inputs, mocks, refs in load_reference_data():
         args = (
-            inputs['fs'],
-            inputs['twin'],
-            inputs['thop'],
-            inputs['channels'],
-            inputs['fmin']
+            inputs["fs"],
+            inputs["twin"],
+            inputs["thop"],
+            inputs["channels"],
+            inputs["fmin"],
         )
 
-        yield GammatonegramTester(
-            inputs['name'],
-            args,
-            inputs['wave'],
-            mocks['erb_fb'],
-            refs['gtgram']
-        )
+        yield GammatonegramTester(inputs["name"], args, inputs["wave"], mocks["erb_fb"], refs["gtgram"])
+
 
 class GammatonegramTester:
-    """ Testing class for gammatonegram calculation """
+    """Testing class for gammatonegram calculation"""
 
     def __init__(self, name, args, sig, erb_fb_out, expected):
         self.signal = np.asarray(sig)
         self.expected = np.asarray(expected)
         self.erb_fb_out = np.asarray(erb_fb_out)
         self.args = args
 
         self.description = "Gammatonegram for {:s}".format(name)
 
     def __call__(self):
-        with patch(
-            'gammatone.gtgram.erb_filterbank',
-            return_value=self.erb_fb_out):
-
+        with patch("gammatone.gtgram.erb_filterbank", return_value=self.erb_fb_out):
             result = gammatone.gtgram.gtgram(self.signal, *self.args)
 
             max_diff = np.max(np.abs(result - self.expected))
             diagnostic = "Maximum difference: {:6e}".format(max_diff)
 
             assert np.allclose(result, self.expected, rtol=1e-6, atol=1e-12), diagnostic
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     nose.main()
```

### Comparing `Gammatone-1.0.0/tests/test_specgram.py` & `Gammatone-1.0.1/tests/test_specgram.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,74 +7,62 @@
 import nose
 import numpy as np
 import scipy.io
 from pkg_resources import resource_stream
 
 import gammatone.fftweight
 
-REF_DATA_FILENAME = 'data/test_specgram_data.mat'
+REF_DATA_FILENAME = "data/test_specgram_data.mat"
 
-INPUT_KEY  = 'specgram_inputs'
-MOCK_KEY   = 'specgram_mocks'
-RESULT_KEY = 'specgram_results'
-
-INPUT_COLS  = ('name', 'wave', 'nfft', 'fs', 'nwin', 'nhop')
-MOCK_COLS   = ('window',)
-RESULT_COLS = ('res',)
+INPUT_KEY = "specgram_inputs"
+MOCK_KEY = "specgram_mocks"
+RESULT_KEY = "specgram_results"
+
+INPUT_COLS = ("name", "wave", "nfft", "fs", "nwin", "nhop")
+MOCK_COLS = ("window",)
+RESULT_COLS = ("res",)
 
 
 def load_reference_data():
-    """ Load test data generated from the reference code """
+    """Load test data generated from the reference code"""
     # Load test data
     with resource_stream(__name__, REF_DATA_FILENAME) as test_data:
         data = scipy.io.loadmat(test_data, squeeze_me=False)
 
     zipped_data = zip(data[INPUT_KEY], data[MOCK_KEY], data[RESULT_KEY])
     for inputs, mocks, refs in zipped_data:
         input_dict = dict(zip(INPUT_COLS, inputs))
-        mock_dict  = dict(zip(MOCK_COLS, mocks))
+        mock_dict = dict(zip(MOCK_COLS, mocks))
         ref_dict = dict(zip(RESULT_COLS, refs))
 
         yield (input_dict, mock_dict, ref_dict)
 
 
 def test_specgram():
     for inputs, mocks, refs in load_reference_data():
-        args = (
-            inputs['nfft'],
-            inputs['fs'],
-            inputs['nwin'],
-            inputs['nhop'],
-        )
-
-        yield SpecgramTester(
-            inputs['name'][0],
-            args,
-            inputs['wave'],
-            mocks['window'],
-            refs['res']
-        )
+        args = (inputs["nfft"], inputs["fs"], inputs["nwin"], inputs["nhop"])
+
+        yield SpecgramTester(inputs["name"][0], args, inputs["wave"], mocks["window"], refs["res"])
+
 
 class SpecgramTester:
-    """ Testing class for specgram replacement calculation """
+    """Testing class for specgram replacement calculation"""
 
     def __init__(self, name, args, sig, window, expected):
         self.signal = np.asarray(sig).squeeze()
         self.expected = np.asarray(expected).squeeze()
         self.args = [int(a.squeeze()) for a in args]
         self.window = window.squeeze()
         self.description = "Specgram for {:s}".format(name)
 
-
     def __call__(self):
-        with patch(
-                'gammatone.fftweight.specgram_window',
-                return_value=self.window):
+        with patch("gammatone.fftweight.specgram_window", return_value=self.window):
             result = gammatone.fftweight.specgram(self.signal, *self.args)
 
             max_diff = np.max(np.abs(result - self.expected))
             diagnostic = "Maximum difference: {:6e}".format(max_diff)
 
             assert np.allclose(result, self.expected, rtol=1e-6, atol=1e-12), diagnostic
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     nose.main()
```

