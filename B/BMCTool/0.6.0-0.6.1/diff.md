# Comparing `tmp/BMCTool-0.6.0.tar.gz` & `tmp/BMCTool-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BMCTool-0.6.0.tar", last modified: Fri Mar 10 12:34:15 2023, max compression
+gzip compressed data, was "BMCTool-0.6.1.tar", last modified: Mon Jul  3 13:48:44 2023, max compression
```

## Comparing `BMCTool-0.6.0.tar` & `BMCTool-0.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.936381 BMCTool-0.6.0/
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.756099 BMCTool-0.6.0/BMCTool.egg-info/
--rw-rw-rw-   0        0        0     6364 2023-03-10 12:34:15.000000 BMCTool-0.6.0/BMCTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      907 2023-03-10 12:34:15.000000 BMCTool-0.6.0/BMCTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 12:34:15.000000 BMCTool-0.6.0/BMCTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-03-10 12:34:15.000000 BMCTool-0.6.0/BMCTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-10 12:34:15.000000 BMCTool-0.6.0/BMCTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2020-11-18 11:02:45.000000 BMCTool-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      425 2021-04-07 16:12:54.000000 BMCTool-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6364 2023-03-10 12:34:15.929906 BMCTool-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     5809 2022-12-13 06:37:29.000000 BMCTool-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.803796 BMCTool-0.6.0/bmctool/
--rw-rw-rw-   0        0        0       20 2023-03-07 15:32:15.000000 BMCTool-0.6.0/bmctool/__init__.py
--rw-rw-rw-   0        0        0    13056 2023-03-10 10:20:38.000000 BMCTool-0.6.0/bmctool/bmc_solver.py
--rw-rw-rw-   0        0        0    10929 2023-03-10 12:01:59.000000 BMCTool-0.6.0/bmctool/bmc_tool.py
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.812815 BMCTool-0.6.0/bmctool/library/
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.819495 BMCTool-0.6.0/bmctool/library/maintenance/
--rw-rw-rw-   0        0        0      977 2023-01-05 16:05:04.000000 BMCTool-0.6.0/bmctool/library/maintenance/valid_params.yaml
--rw-rw-rw-   0        0        0      889 2023-01-05 16:05:04.000000 BMCTool-0.6.0/bmctool/library/readme.md
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.826689 BMCTool-0.6.0/bmctool/library/seq-library/
--rw-rw-rw-   0        0        0     7077 2023-01-05 16:05:04.000000 BMCTool-0.6.0/bmctool/library/seq-library/WASABI.seq
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.834857 BMCTool-0.6.0/bmctool/library/sim-library/
--rw-rw-rw-   0        0        0     1678 2023-03-10 10:51:54.000000 BMCTool-0.6.0/bmctool/library/sim-library/config_wasabi.yaml
--rw-rw-rw-   0        0        0    11355 2023-03-09 10:59:30.000000 BMCTool-0.6.0/bmctool/params.py
--rw-rw-rw-   0        0        0    11291 2023-03-09 10:00:07.000000 BMCTool-0.6.0/bmctool/set_params.py
--rw-rw-rw-   0        0        0     2114 2023-03-09 11:19:11.000000 BMCTool-0.6.0/bmctool/simulate.py
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.849998 BMCTool-0.6.0/bmctool/utils/
--rw-rw-rw-   0        0        0        0 2023-01-05 16:05:04.000000 BMCTool-0.6.0/bmctool/utils/__init__.py
--rw-rw-rw-   0        0        0     5879 2023-03-09 09:20:41.000000 BMCTool-0.6.0/bmctool/utils/eval.py
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.902022 BMCTool-0.6.0/bmctool/utils/pulses/
--rw-rw-rw-   0        0        0        0 2023-01-05 16:05:04.000000 BMCTool-0.6.0/bmctool/utils/pulses/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-03-10 12:12:56.000000 BMCTool-0.6.0/bmctool/utils/pulses/calc_power_equivalents.py
--rw-rw-rw-   0        0        0      812 2023-03-10 12:07:26.000000 BMCTool-0.6.0/bmctool/utils/pulses/calculate_phase.py
--rw-rw-rw-   0        0        0     1756 2023-03-10 10:58:25.000000 BMCTool-0.6.0/bmctool/utils/pulses/create_arbitrary_pulse_with_phase.py
--rw-rw-rw-   0        0        0     1876 2023-03-07 15:32:16.000000 BMCTool-0.6.0/bmctool/utils/pulses/make_hanning.py
--rw-rw-rw-   0        0        0     7704 2023-03-07 15:32:16.000000 BMCTool-0.6.0/bmctool/utils/pulses/make_hsexp.py
--rw-rw-rw-   0        0        0     3171 2023-03-07 15:32:16.000000 BMCTool-0.6.0/bmctool/utils/pulses/make_hypsec_half_passage.py
-drwxrwxrwx   0        0        0        0 2023-03-10 12:34:15.921649 BMCTool-0.6.0/bmctool/utils/seq/
--rw-rw-rw-   0        0        0        0 2023-01-05 16:05:04.000000 BMCTool-0.6.0/bmctool/utils/seq/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-03-09 08:05:38.000000 BMCTool-0.6.0/bmctool/utils/seq/auxiliary.py
--rw-rw-rw-   0        0        0     4790 2023-03-09 13:15:36.000000 BMCTool-0.6.0/bmctool/utils/seq/write.py
--rw-rw-rw-   0        0        0       42 2023-03-10 12:34:15.936381 BMCTool-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-03-09 11:25:27.000000 BMCTool-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:44.095588 BMCTool-0.6.1/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:43.920405 BMCTool-0.6.1/BMCTool.egg-info/
+-rw-rw-rw-   0        0        0     5808 2023-07-03 13:48:43.000000 BMCTool-0.6.1/BMCTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      907 2023-07-03 13:48:43.000000 BMCTool-0.6.1/BMCTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 13:48:43.000000 BMCTool-0.6.1/BMCTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-03 13:48:43.000000 BMCTool-0.6.1/BMCTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 13:48:43.000000 BMCTool-0.6.1/BMCTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-07-03 10:57:02.000000 BMCTool-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0      425 2023-07-03 10:57:02.000000 BMCTool-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5808 2023-07-03 13:48:44.089578 BMCTool-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5253 2023-07-03 10:57:02.000000 BMCTool-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:43.968836 BMCTool-0.6.1/bmctool/
+-rw-rw-rw-   0        0        0       20 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/__init__.py
+-rw-rw-rw-   0        0        0    13056 2023-07-03 12:57:23.000000 BMCTool-0.6.1/bmctool/bmc_solver.py
+-rw-rw-rw-   0        0        0    11138 2023-07-03 13:28:10.000000 BMCTool-0.6.1/bmctool/bmc_tool.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:43.975820 BMCTool-0.6.1/bmctool/library/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:43.983794 BMCTool-0.6.1/bmctool/library/maintenance/
+-rw-rw-rw-   0        0        0      977 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/library/maintenance/valid_params.yaml
+-rw-rw-rw-   0        0        0      889 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/library/readme.md
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:43.989746 BMCTool-0.6.1/bmctool/library/seq-library/
+-rw-rw-rw-   0        0        0     7077 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/library/seq-library/WASABI.seq
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:43.998791 BMCTool-0.6.1/bmctool/library/sim-library/
+-rw-rw-rw-   0        0        0     1678 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/library/sim-library/config_wasabi.yaml
+-rw-rw-rw-   0        0        0    11355 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/params.py
+-rw-rw-rw-   0        0        0    11291 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/set_params.py
+-rw-rw-rw-   0        0        0     2114 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/simulate.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:44.010724 BMCTool-0.6.1/bmctool/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/__init__.py
+-rw-rw-rw-   0        0        0     5879 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/eval.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:44.061651 BMCTool-0.6.1/bmctool/utils/pulses/
+-rw-rw-rw-   0        0        0        0 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/pulses/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/pulses/calc_power_equivalents.py
+-rw-rw-rw-   0        0        0      812 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/pulses/calculate_phase.py
+-rw-rw-rw-   0        0        0     1756 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/pulses/create_arbitrary_pulse_with_phase.py
+-rw-rw-rw-   0        0        0     1876 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/pulses/make_hanning.py
+-rw-rw-rw-   0        0        0     7704 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/pulses/make_hsexp.py
+-rw-rw-rw-   0        0        0     3171 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/pulses/make_hypsec_half_passage.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:48:44.080944 BMCTool-0.6.1/bmctool/utils/seq/
+-rw-rw-rw-   0        0        0        0 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/seq/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/seq/auxiliary.py
+-rw-rw-rw-   0        0        0     4790 2023-07-03 10:57:02.000000 BMCTool-0.6.1/bmctool/utils/seq/write.py
+-rw-rw-rw-   0        0        0       42 2023-07-03 13:48:44.095588 BMCTool-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      958 2023-07-03 13:30:51.000000 BMCTool-0.6.1/setup.py
```

### Comparing `BMCTool-0.6.0/BMCTool.egg-info/PKG-INFO` & `BMCTool-0.6.1/BMCTool.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BMCTool
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python tool to perform Bloch-McConnell (BMC) simulations.
 Home-page: https://github.com/schuenke/BMCTool
 Author: Patrick Schuenke
 Author-email: patrick.schuenke@ptb.de
 Keywords: MRI,Bloch,CEST,simulations
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
@@ -12,96 +12,95 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Bloch-McConnell (BMC) Simulation Tool
 
-This repository contains a purely python-based Bloch-McConnell (BMC) simulation tool that can be used to simulate 
+This repository contains a purely python-based Bloch-McConnell (BMC) simulation tool that can be used to simulate
 the evolution of the magnetization in various (exchanging) magnetic environments ('pools') under arbitrary
-radio-frequency (RF) irradiation. The tool was developed to simulate Chemical Exchange Saturation Transfer (CEST) or 
-related spectra, but can be used for many other MR simulations as well. 
+radio-frequency (RF) irradiation. The tool was developed to simulate Chemical Exchange Saturation Transfer (CEST) or
+related spectra, but can be used for many other MR simulations as well.
 
 The BMCTool utilizes the [pulseq](https://pulseq.github.io/) open file format to define and store all events (RF pulses,
-gradients, delays, ADCs) that shall be simulated. The scanner settings and characteristic properties of the magnetic 
+gradients, delays, ADCs) that shall be simulated. The scanner settings and characteristic properties of the magnetic
 environments (relaxation times, pool size fractions, exchange rates) are defined and stored in config-files in the
-[YAML](https://yaml.org) file format. 
+[YAML](https://yaml.org) file format.
 
-Every simulation requires exactly one seq-file (containing all events) and at least one config-file. 
+Every simulation requires exactly one seq-file (containing all events) and at least one config-file.
 
 ## Installation
+
 The BMCTool can be installed from [PyPi](https://pypi.org/) using
 
 ``
 pip install bmctool
 ``
 
-### IMPORTANT NOTE FOR RELEASE v0.5.0
-Version 0.5.0 of BMCTool requires PyPulseq >= 1.4.0, which is currently only available if installed directly from the [Dev branch](https://github.com/imr-framework/pypulseq/tree/dev) of the [PyPulseq Github Repository](https://github.com/imr-framework/pypulseq). A working version can be installed using
-
-
-``
-pip install git+https://github.com/imr-framework/pypulseq@c644fd9
-``
-
-A new version of the BMCTool with updated dependencies will be released as soon as PyPulseq v. 1.4.0 is officially released!
-
 ### Initial Test
-To make sure that the installation was successful, you can run an example simulation that is provided with both, 
+
+To make sure that the installation was successful, you can run an example simulation that is provided with both,
 the installation using pip and GitHub. To run an example simulation, simply execute the following code:
+
 ```python
 from bmctool.simulate import sim_example
 sim_example()
 ```
+
 The sim_example function uses the [WASABI.seq](bmctool/library/seq-library/WASABI.seq)
 and [config_wasabi.yaml](bmctool/library/sim-library/config_wasabi.yaml) example files. The generated plot should look
 like this:
 
 ![](https://raw.githubusercontent.com/schuenke/BMCTool/master/examples/example_wasabi_spectrum.png "Example WASABI spectrum")
 
 ## Starting a Simulation
-All simulations using the BMCTool require a config file (in the *yaml* format) that includes all simulation settings 
-and a sequence file (in the *seq* format), which defines the events to be simulated. An 
-[example seq-file](bmctool/library/seq-library/WASABI.seq) and an 
-[example yaml file](bmctool/library/sim-library/config_wasabi.yaml) can be found in the [library](bmctool/library) 
-subfolder. For more information about config and sequence files and about the 
-[pulseq-cest-library](library/pulseq-cest-library), where both types of files are shared, please read the 
+
+All simulations using the BMCTool require a config file (in the *yaml* format) that includes all simulation settings
+and a sequence file (in the *seq* format), which defines the events to be simulated. An
+[example seq-file](bmctool/library/seq-library/WASABI.seq) and an
+[example yaml file](bmctool/library/sim-library/config_wasabi.yaml) can be found in the [library](bmctool/library)
+subfolder. For more information about config and sequence files and about the
+[pulseq-cest-library](library/pulseq-cest-library), where both types of files are shared, please read the
 **Pulseq-CEST Library** section below.
 
-If you created your own files or downloaded them from the [pulseq-cest-library](https://github.com/kherz/pulseq-cest-library), 
+If you created your own files or downloaded them from the [pulseq-cest-library](https://github.com/kherz/pulseq-cest-library),
 you can start the simulation by running the following code:
+
 ```python
 from bmctool.simulate import simulate
 config_path = '<path_to_your_config>'  # can be a str or a Path
 seq_path = '<path_to_your_sequence>'  # can be a str or a Path
 sim = simulate(config_file=config_path, seq_file=seq_path, show_plot=True)
 ```
+
 The simulate function accepts several additional keyword arguments (**kwargs), that allow to adjust the plot.
-These are for example _normalize_ (bool: toggle normalization), _norm_threshold_ (value/list/array: threshold for
-normalization offsets), _offsets_ (list/array: manually defined x-values), _invert_ax_ (bool: toggle invert ax), 
-_plot_mtr_asym_ (bool:toggle plot MTR_asym) and _title_, _x_label_, _y_label_ to control the lables.
+These are for example *normalize* (bool: toggle normalization), *norm_threshold* (value/list/array: threshold for
+normalization offsets), *offsets* (list/array: manually defined x-values), *invert_ax* (bool: toggle invert ax),
+*plot_mtr_asym* (bool:toggle plot MTR_asym) and *title*, *x_label*, *y_label* to control the lables.
 
-The [examples folder](examples) in the [BMCTool GitHub repository](https://github.com/schuenke/BMCTool) contains some 
-further simulation examples as well as an example script to create your own _WASABI.seq_ file. _Please note that this
+The [examples folder](examples) in the [BMCTool GitHub repository](https://github.com/schuenke/BMCTool) contains some
+further simulation examples as well as an example script to create your own *WASABI.seq* file. _Please note that this
 file will include an additional normalization offset at -300 ppm. To use this for normalization in the simulation,
-simply add the kewword argument ``normalize=True`` to the simulate function._ 
+simply add the kewword argument ``normalize=True`` to the simulate function._
 
 ## Pulseq-CEST Project
+
 The BMCTool was developed in parallel to the [pulseq-cest project](https://pulseq-cest.github.io/) that aims to provide
-published and approved CEST saturation blocks in the [pulseq](https://pulseq.github.io/) open file format to enable an 
+published and approved CEST saturation blocks in the [pulseq](https://pulseq.github.io/) open file format to enable an
 exact comparison of CEST saturation blocks with newly developed or adapted saturation blocks for reproducible research.
 The [pulseq-cest project](https://pulseq-cest.github.io/) provides a [MATLAB implementation](https://github.com/kherz/pulseq-cest)
 and a [python implementation](https://github.com/KerstinHut/pypulseq-cest). The python implementation uses the
 [BMCTool](https://github.com/schuenke/BMCTool) and [pypulseq](https://github.com/imr-framework/pypulseq) for config and
 seq file handling. Both, the MATLAB and python implementation use the same Bloch-McConnell equation solver implemented
-in C++, which is much faster than the solver implemented in the BMCTool itself. For extensive simulations we thus 
+in C++, which is much faster than the solver implemented in the BMCTool itself. For extensive simulations we thus
 recommend checking out the [pulseq-cest implementations](https://pulseq-cest.github.io/).
 
 ### Pulseq-CEST Library
-You will find several pre-defined and approved CEST pre-saturation schemes and simulation configs in the 
-[pulseq-cest-library GitHub repository](https://github.com/kherz/pulseq-cest-library). You can clone the library using 
+
+You will find several pre-defined and approved CEST pre-saturation schemes and simulation configs in the
+[pulseq-cest-library GitHub repository](https://github.com/kherz/pulseq-cest-library). You can clone the library using
 
 ``
 git clone https://github.com/kherz/pulseq-cest-library.git
 ``
 
 or directly download the latest version as a [ZIP file](https://github.com/kherz/pulseq-cest-library/archive/master.zip).
```

### Comparing `BMCTool-0.6.0/BMCTool.egg-info/SOURCES.txt` & `BMCTool-0.6.1/BMCTool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/LICENSE` & `BMCTool-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/PKG-INFO` & `BMCTool-0.6.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BMCTool
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python tool to perform Bloch-McConnell (BMC) simulations.
 Home-page: https://github.com/schuenke/BMCTool
 Author: Patrick Schuenke
 Author-email: patrick.schuenke@ptb.de
 Keywords: MRI,Bloch,CEST,simulations
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
@@ -12,96 +12,95 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Bloch-McConnell (BMC) Simulation Tool
 
-This repository contains a purely python-based Bloch-McConnell (BMC) simulation tool that can be used to simulate 
+This repository contains a purely python-based Bloch-McConnell (BMC) simulation tool that can be used to simulate
 the evolution of the magnetization in various (exchanging) magnetic environments ('pools') under arbitrary
-radio-frequency (RF) irradiation. The tool was developed to simulate Chemical Exchange Saturation Transfer (CEST) or 
-related spectra, but can be used for many other MR simulations as well. 
+radio-frequency (RF) irradiation. The tool was developed to simulate Chemical Exchange Saturation Transfer (CEST) or
+related spectra, but can be used for many other MR simulations as well.
 
 The BMCTool utilizes the [pulseq](https://pulseq.github.io/) open file format to define and store all events (RF pulses,
-gradients, delays, ADCs) that shall be simulated. The scanner settings and characteristic properties of the magnetic 
+gradients, delays, ADCs) that shall be simulated. The scanner settings and characteristic properties of the magnetic
 environments (relaxation times, pool size fractions, exchange rates) are defined and stored in config-files in the
-[YAML](https://yaml.org) file format. 
+[YAML](https://yaml.org) file format.
 
-Every simulation requires exactly one seq-file (containing all events) and at least one config-file. 
+Every simulation requires exactly one seq-file (containing all events) and at least one config-file.
 
 ## Installation
+
 The BMCTool can be installed from [PyPi](https://pypi.org/) using
 
 ``
 pip install bmctool
 ``
 
-### IMPORTANT NOTE FOR RELEASE v0.5.0
-Version 0.5.0 of BMCTool requires PyPulseq >= 1.4.0, which is currently only available if installed directly from the [Dev branch](https://github.com/imr-framework/pypulseq/tree/dev) of the [PyPulseq Github Repository](https://github.com/imr-framework/pypulseq). A working version can be installed using
-
-
-``
-pip install git+https://github.com/imr-framework/pypulseq@c644fd9
-``
-
-A new version of the BMCTool with updated dependencies will be released as soon as PyPulseq v. 1.4.0 is officially released!
-
 ### Initial Test
-To make sure that the installation was successful, you can run an example simulation that is provided with both, 
+
+To make sure that the installation was successful, you can run an example simulation that is provided with both,
 the installation using pip and GitHub. To run an example simulation, simply execute the following code:
+
 ```python
 from bmctool.simulate import sim_example
 sim_example()
 ```
+
 The sim_example function uses the [WASABI.seq](bmctool/library/seq-library/WASABI.seq)
 and [config_wasabi.yaml](bmctool/library/sim-library/config_wasabi.yaml) example files. The generated plot should look
 like this:
 
 ![](https://raw.githubusercontent.com/schuenke/BMCTool/master/examples/example_wasabi_spectrum.png "Example WASABI spectrum")
 
 ## Starting a Simulation
-All simulations using the BMCTool require a config file (in the *yaml* format) that includes all simulation settings 
-and a sequence file (in the *seq* format), which defines the events to be simulated. An 
-[example seq-file](bmctool/library/seq-library/WASABI.seq) and an 
-[example yaml file](bmctool/library/sim-library/config_wasabi.yaml) can be found in the [library](bmctool/library) 
-subfolder. For more information about config and sequence files and about the 
-[pulseq-cest-library](library/pulseq-cest-library), where both types of files are shared, please read the 
+
+All simulations using the BMCTool require a config file (in the *yaml* format) that includes all simulation settings
+and a sequence file (in the *seq* format), which defines the events to be simulated. An
+[example seq-file](bmctool/library/seq-library/WASABI.seq) and an
+[example yaml file](bmctool/library/sim-library/config_wasabi.yaml) can be found in the [library](bmctool/library)
+subfolder. For more information about config and sequence files and about the
+[pulseq-cest-library](library/pulseq-cest-library), where both types of files are shared, please read the
 **Pulseq-CEST Library** section below.
 
-If you created your own files or downloaded them from the [pulseq-cest-library](https://github.com/kherz/pulseq-cest-library), 
+If you created your own files or downloaded them from the [pulseq-cest-library](https://github.com/kherz/pulseq-cest-library),
 you can start the simulation by running the following code:
+
 ```python
 from bmctool.simulate import simulate
 config_path = '<path_to_your_config>'  # can be a str or a Path
 seq_path = '<path_to_your_sequence>'  # can be a str or a Path
 sim = simulate(config_file=config_path, seq_file=seq_path, show_plot=True)
 ```
+
 The simulate function accepts several additional keyword arguments (**kwargs), that allow to adjust the plot.
-These are for example _normalize_ (bool: toggle normalization), _norm_threshold_ (value/list/array: threshold for
-normalization offsets), _offsets_ (list/array: manually defined x-values), _invert_ax_ (bool: toggle invert ax), 
-_plot_mtr_asym_ (bool:toggle plot MTR_asym) and _title_, _x_label_, _y_label_ to control the lables.
+These are for example *normalize* (bool: toggle normalization), *norm_threshold* (value/list/array: threshold for
+normalization offsets), *offsets* (list/array: manually defined x-values), *invert_ax* (bool: toggle invert ax),
+*plot_mtr_asym* (bool:toggle plot MTR_asym) and *title*, *x_label*, *y_label* to control the lables.
 
-The [examples folder](examples) in the [BMCTool GitHub repository](https://github.com/schuenke/BMCTool) contains some 
-further simulation examples as well as an example script to create your own _WASABI.seq_ file. _Please note that this
+The [examples folder](examples) in the [BMCTool GitHub repository](https://github.com/schuenke/BMCTool) contains some
+further simulation examples as well as an example script to create your own *WASABI.seq* file. _Please note that this
 file will include an additional normalization offset at -300 ppm. To use this for normalization in the simulation,
-simply add the kewword argument ``normalize=True`` to the simulate function._ 
+simply add the kewword argument ``normalize=True`` to the simulate function._
 
 ## Pulseq-CEST Project
+
 The BMCTool was developed in parallel to the [pulseq-cest project](https://pulseq-cest.github.io/) that aims to provide
-published and approved CEST saturation blocks in the [pulseq](https://pulseq.github.io/) open file format to enable an 
+published and approved CEST saturation blocks in the [pulseq](https://pulseq.github.io/) open file format to enable an
 exact comparison of CEST saturation blocks with newly developed or adapted saturation blocks for reproducible research.
 The [pulseq-cest project](https://pulseq-cest.github.io/) provides a [MATLAB implementation](https://github.com/kherz/pulseq-cest)
 and a [python implementation](https://github.com/KerstinHut/pypulseq-cest). The python implementation uses the
 [BMCTool](https://github.com/schuenke/BMCTool) and [pypulseq](https://github.com/imr-framework/pypulseq) for config and
 seq file handling. Both, the MATLAB and python implementation use the same Bloch-McConnell equation solver implemented
-in C++, which is much faster than the solver implemented in the BMCTool itself. For extensive simulations we thus 
+in C++, which is much faster than the solver implemented in the BMCTool itself. For extensive simulations we thus
 recommend checking out the [pulseq-cest implementations](https://pulseq-cest.github.io/).
 
 ### Pulseq-CEST Library
-You will find several pre-defined and approved CEST pre-saturation schemes and simulation configs in the 
-[pulseq-cest-library GitHub repository](https://github.com/kherz/pulseq-cest-library). You can clone the library using 
+
+You will find several pre-defined and approved CEST pre-saturation schemes and simulation configs in the
+[pulseq-cest-library GitHub repository](https://github.com/kherz/pulseq-cest-library). You can clone the library using
 
 ``
 git clone https://github.com/kherz/pulseq-cest-library.git
 ``
 
 or directly download the latest version as a [ZIP file](https://github.com/kherz/pulseq-cest-library/archive/master.zip).
```

### Comparing `BMCTool-0.6.0/README.md` & `BMCTool-0.6.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 # Bloch-McConnell (BMC) Simulation Tool
 
-This repository contains a purely python-based Bloch-McConnell (BMC) simulation tool that can be used to simulate 
+This repository contains a purely python-based Bloch-McConnell (BMC) simulation tool that can be used to simulate
 the evolution of the magnetization in various (exchanging) magnetic environments ('pools') under arbitrary
-radio-frequency (RF) irradiation. The tool was developed to simulate Chemical Exchange Saturation Transfer (CEST) or 
-related spectra, but can be used for many other MR simulations as well. 
+radio-frequency (RF) irradiation. The tool was developed to simulate Chemical Exchange Saturation Transfer (CEST) or
+related spectra, but can be used for many other MR simulations as well.
 
 The BMCTool utilizes the [pulseq](https://pulseq.github.io/) open file format to define and store all events (RF pulses,
-gradients, delays, ADCs) that shall be simulated. The scanner settings and characteristic properties of the magnetic 
+gradients, delays, ADCs) that shall be simulated. The scanner settings and characteristic properties of the magnetic
 environments (relaxation times, pool size fractions, exchange rates) are defined and stored in config-files in the
-[YAML](https://yaml.org) file format. 
+[YAML](https://yaml.org) file format.
 
-Every simulation requires exactly one seq-file (containing all events) and at least one config-file. 
+Every simulation requires exactly one seq-file (containing all events) and at least one config-file.
 
 ## Installation
+
 The BMCTool can be installed from [PyPi](https://pypi.org/) using
 
 ``
 pip install bmctool
 ``
 
-### IMPORTANT NOTE FOR RELEASE v0.5.0
-Version 0.5.0 of BMCTool requires PyPulseq >= 1.4.0, which is currently only available if installed directly from the [Dev branch](https://github.com/imr-framework/pypulseq/tree/dev) of the [PyPulseq Github Repository](https://github.com/imr-framework/pypulseq). A working version can be installed using
-
-
-``
-pip install git+https://github.com/imr-framework/pypulseq@c644fd9
-``
-
-A new version of the BMCTool with updated dependencies will be released as soon as PyPulseq v. 1.4.0 is officially released!
-
 ### Initial Test
-To make sure that the installation was successful, you can run an example simulation that is provided with both, 
+
+To make sure that the installation was successful, you can run an example simulation that is provided with both,
 the installation using pip and GitHub. To run an example simulation, simply execute the following code:
+
 ```python
 from bmctool.simulate import sim_example
 sim_example()
 ```
+
 The sim_example function uses the [WASABI.seq](bmctool/library/seq-library/WASABI.seq)
 and [config_wasabi.yaml](bmctool/library/sim-library/config_wasabi.yaml) example files. The generated plot should look
 like this:
 
 ![](https://raw.githubusercontent.com/schuenke/BMCTool/master/examples/example_wasabi_spectrum.png "Example WASABI spectrum")
 
 ## Starting a Simulation
-All simulations using the BMCTool require a config file (in the *yaml* format) that includes all simulation settings 
-and a sequence file (in the *seq* format), which defines the events to be simulated. An 
-[example seq-file](bmctool/library/seq-library/WASABI.seq) and an 
-[example yaml file](bmctool/library/sim-library/config_wasabi.yaml) can be found in the [library](bmctool/library) 
-subfolder. For more information about config and sequence files and about the 
-[pulseq-cest-library](library/pulseq-cest-library), where both types of files are shared, please read the 
+
+All simulations using the BMCTool require a config file (in the *yaml* format) that includes all simulation settings
+and a sequence file (in the *seq* format), which defines the events to be simulated. An
+[example seq-file](bmctool/library/seq-library/WASABI.seq) and an
+[example yaml file](bmctool/library/sim-library/config_wasabi.yaml) can be found in the [library](bmctool/library)
+subfolder. For more information about config and sequence files and about the
+[pulseq-cest-library](library/pulseq-cest-library), where both types of files are shared, please read the
 **Pulseq-CEST Library** section below.
 
-If you created your own files or downloaded them from the [pulseq-cest-library](https://github.com/kherz/pulseq-cest-library), 
+If you created your own files or downloaded them from the [pulseq-cest-library](https://github.com/kherz/pulseq-cest-library),
 you can start the simulation by running the following code:
+
 ```python
 from bmctool.simulate import simulate
 config_path = '<path_to_your_config>'  # can be a str or a Path
 seq_path = '<path_to_your_sequence>'  # can be a str or a Path
 sim = simulate(config_file=config_path, seq_file=seq_path, show_plot=True)
 ```
+
 The simulate function accepts several additional keyword arguments (**kwargs), that allow to adjust the plot.
-These are for example _normalize_ (bool: toggle normalization), _norm_threshold_ (value/list/array: threshold for
-normalization offsets), _offsets_ (list/array: manually defined x-values), _invert_ax_ (bool: toggle invert ax), 
-_plot_mtr_asym_ (bool:toggle plot MTR_asym) and _title_, _x_label_, _y_label_ to control the lables.
+These are for example *normalize* (bool: toggle normalization), *norm_threshold* (value/list/array: threshold for
+normalization offsets), *offsets* (list/array: manually defined x-values), *invert_ax* (bool: toggle invert ax),
+*plot_mtr_asym* (bool:toggle plot MTR_asym) and *title*, *x_label*, *y_label* to control the lables.
 
-The [examples folder](examples) in the [BMCTool GitHub repository](https://github.com/schuenke/BMCTool) contains some 
-further simulation examples as well as an example script to create your own _WASABI.seq_ file. _Please note that this
+The [examples folder](examples) in the [BMCTool GitHub repository](https://github.com/schuenke/BMCTool) contains some
+further simulation examples as well as an example script to create your own *WASABI.seq* file. _Please note that this
 file will include an additional normalization offset at -300 ppm. To use this for normalization in the simulation,
-simply add the kewword argument ``normalize=True`` to the simulate function._ 
+simply add the kewword argument ``normalize=True`` to the simulate function._
 
 ## Pulseq-CEST Project
+
 The BMCTool was developed in parallel to the [pulseq-cest project](https://pulseq-cest.github.io/) that aims to provide
-published and approved CEST saturation blocks in the [pulseq](https://pulseq.github.io/) open file format to enable an 
+published and approved CEST saturation blocks in the [pulseq](https://pulseq.github.io/) open file format to enable an
 exact comparison of CEST saturation blocks with newly developed or adapted saturation blocks for reproducible research.
 The [pulseq-cest project](https://pulseq-cest.github.io/) provides a [MATLAB implementation](https://github.com/kherz/pulseq-cest)
 and a [python implementation](https://github.com/KerstinHut/pypulseq-cest). The python implementation uses the
 [BMCTool](https://github.com/schuenke/BMCTool) and [pypulseq](https://github.com/imr-framework/pypulseq) for config and
 seq file handling. Both, the MATLAB and python implementation use the same Bloch-McConnell equation solver implemented
-in C++, which is much faster than the solver implemented in the BMCTool itself. For extensive simulations we thus 
+in C++, which is much faster than the solver implemented in the BMCTool itself. For extensive simulations we thus
 recommend checking out the [pulseq-cest implementations](https://pulseq-cest.github.io/).
 
 ### Pulseq-CEST Library
-You will find several pre-defined and approved CEST pre-saturation schemes and simulation configs in the 
-[pulseq-cest-library GitHub repository](https://github.com/kherz/pulseq-cest-library). You can clone the library using 
+
+You will find several pre-defined and approved CEST pre-saturation schemes and simulation configs in the
+[pulseq-cest-library GitHub repository](https://github.com/kherz/pulseq-cest-library). You can clone the library using
 
 ``
 git clone https://github.com/kherz/pulseq-cest-library.git
 ``
 
 or directly download the latest version as a [ZIP file](https://github.com/kherz/pulseq-cest-library/archive/master.zip).
```

### Comparing `BMCTool-0.6.0/bmctool/bmc_solver.py` & `BMCTool-0.6.1/bmctool/bmc_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         if self.is_mt_active:
             self.arr_a[:, 3 * (n_p + 1), 3 * (n_p + 1)] = (
                 -self.params.mt_pool["r1"]
                 - self.params.mt_pool["k"]
                 - rf_amp_2pi**2 * self.get_mt_shape_at_offset(rf_freq_2pi + self.dw0, self.w0)
             )
 
-    def solve_equation_pade(self, mag: np.ndarray, dtp: float) -> np.ndarray:
+    def solve_equation(self, mag: np.ndarray, dtp: float) -> np.ndarray:
         """
         Solves one step of BMC equations using the Padé approximation. This function is not used atm.
         :param mag: magnetization vector before current step
         :param dtp: duration of current step
         :return: magnetization vector after current step
         """
         arr_a = np.squeeze(self.arr_a)
@@ -216,15 +216,15 @@
 
         f = np.dot(np.linalg.pinv(d), n)
         for k in range(1, j + 1):
             f = np.dot(f, f)
         mag_ = np.dot(f, (mag_ + a_inv_t)) - a_inv_t
         return mag_[np.newaxis, :, np.newaxis]
 
-    def solve_equation(self, mag: np.ndarray, dtp: float) -> np.ndarray:
+    def solve_equation_expm(self, mag: np.ndarray, dtp: float) -> np.ndarray:
         """
         Solves one step of BMC equations using the eigenwert ansatz.
         :param mag: magnetization vector before current step
         :param dtp: duration of current step
         :return: magnetization vector after current step
         """
         arr_a = self.arr_a
```

### Comparing `BMCTool-0.6.0/bmctool/bmc_tool.py` & `BMCTool-0.6.1/bmctool/bmc_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,18 +49,25 @@
         dtp = 1e-6
         delay_after_pulse = (rf_length - idx.size) * dtp
 
     amp = amp[idx]
     ph = ph[idx]
     n_unique = max(np.unique(amp).size, np.unique(ph).size)
 
-    if n_unique == 1:
+    # block pulse for seq-files >= 1.4.0
+    if n_unique == 1 and amp.size ==2:
+        amp_ = amp[0]
+        ph_ = ph[0]
+        dtp_ = dtp
+    # block pulse for seq-files < 1.4.0
+    elif n_unique == 1:
         amp_ = amp[0]
         ph_ = ph[0]
         dtp_ = dtp * amp.size
+    # shaped pulse
     elif n_unique > max_pulse_samples:
         sample_factor = int(np.ceil(amp.size / max_pulse_samples))
         amp_ = amp[::sample_factor]
         ph_ = ph[::sample_factor]
         dtp_ = dtp * sample_factor
     else:
         raise Exception("Case with 1 < unique samples < max_pulse_samples not implemented yet. Sorry :(")
@@ -144,19 +151,19 @@
         else:
             loop_block_events = range(1, len(block_events) + 1)
 
         # code for pypulseq >= 1.4.0:
         try:
             for block_event in loop_block_events:
                 block = self.seq.get_block(block_event)
-                current_adc, accum_pahse, mag = self.run_1_4_0(block, current_adc, accum_phase, mag)
+                current_adc, accum_phase, mag = self.run_1_4_0(block, current_adc, accum_phase, mag)
         except AttributeError:
             for block_event in loop_block_events:
                 block = self.seq.get_block(block_event)
-                current_adc, accum_pahse, mag = self.run_1_3_0(block, current_adc, accum_phase, mag)
+                current_adc, accum_phase, mag = self.run_1_3_0(block, current_adc, accum_phase, mag)
 
     def run_1_4_0(self, block, current_adc, accum_phase, mag) -> Tuple[int, float, np.ndarray]:
         # pseudo ADC event
         if block.adc is not None:
             # write current magnetization to output
             self.m_out[:, current_adc] = np.squeeze(mag)
             accum_phase = 0
```

### Comparing `BMCTool-0.6.0/bmctool/library/maintenance/valid_params.yaml` & `BMCTool-0.6.1/bmctool/library/maintenance/valid_params.yaml`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/library/readme.md` & `BMCTool-0.6.1/bmctool/library/readme.md`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/library/seq-library/WASABI.seq` & `BMCTool-0.6.1/bmctool/library/seq-library/WASABI.seq`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/library/sim-library/config_wasabi.yaml` & `BMCTool-0.6.1/bmctool/library/sim-library/config_wasabi.yaml`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/params.py` & `BMCTool-0.6.1/bmctool/params.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/set_params.py` & `BMCTool-0.6.1/bmctool/set_params.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/simulate.py` & `BMCTool-0.6.1/bmctool/simulate.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/utils/eval.py` & `BMCTool-0.6.1/bmctool/utils/eval.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/utils/pulses/calc_power_equivalents.py` & `BMCTool-0.6.1/bmctool/utils/pulses/calc_power_equivalents.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/utils/pulses/calculate_phase.py` & `BMCTool-0.6.1/bmctool/utils/pulses/calculate_phase.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/utils/pulses/create_arbitrary_pulse_with_phase.py` & `BMCTool-0.6.1/bmctool/utils/pulses/create_arbitrary_pulse_with_phase.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/utils/pulses/make_hanning.py` & `BMCTool-0.6.1/bmctool/utils/pulses/make_hanning.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/utils/pulses/make_hsexp.py` & `BMCTool-0.6.1/bmctool/utils/pulses/make_hsexp.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/utils/pulses/make_hypsec_half_passage.py` & `BMCTool-0.6.1/bmctool/utils/pulses/make_hypsec_half_passage.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/utils/seq/auxiliary.py` & `BMCTool-0.6.1/bmctool/utils/seq/auxiliary.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/bmctool/utils/seq/write.py` & `BMCTool-0.6.1/bmctool/utils/seq/write.py`

 * *Files identical despite different names*

### Comparing `BMCTool-0.6.0/setup.py` & `BMCTool-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="BMCTool",
     author="Patrick Schuenke",
     author_email="patrick.schuenke@ptb.de",
-    version="0.6.0",
+    version="0.6.1",
     description="A python tool to perform Bloch-McConnell (BMC) simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/schuenke/BMCTool",
     install_requires=[
-        "numpy",
+        "numpy<1.24",
         "matplotlib",
         "tqdm",
         "PyYAML",
         "pypulseq",
     ],
     keywords="MRI, Bloch, CEST, simulations",
     packages=find_packages(),
```

