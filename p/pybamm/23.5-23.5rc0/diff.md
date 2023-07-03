# Comparing `tmp/pybamm-23.5.tar.gz` & `tmp/pybamm-23.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybamm-23.5.tar", last modified: Mon Jul  3 10:39:30 2023, max compression
+gzip compressed data, was "pybamm-23.5rc0.tar", last modified: Mon Jun 19 14:33:45 2023, max compression
```

## Comparing `pybamm-23.5.tar` & `pybamm-23.5rc0.tar`

### file list

```diff
@@ -1,376 +1,376 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.092914 pybamm-23.5/
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-07-03 10:39:23.000000 pybamm-23.5/CMakeBuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-03 10:39:23.000000 pybamm-23.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    43197 2023-07-03 10:39:30.092914 pybamm-23.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40154 2023-07-03 10:39:23.000000 pybamm-23.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.044914 pybamm-23.5/pybamm/
--rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/CITATIONS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/batch_study.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/citations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.044914 pybamm-23.5/pybamm/discretisations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/discretisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/discretisations/discretisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/doc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.044914 pybamm-23.5/pybamm/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/experiment/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.048914 pybamm-23.5/pybamm/expression_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/averages.py
--rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/binary_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/broadcasts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/concatenations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/independent_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/input_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/interpolant.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.048914 pybamm-23.5/pybamm/expression_tree/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/operations/convert_to_casadi.py
--rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/operations/evaluate_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/operations/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/operations/latexify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/operations/unpack_symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.048914 pybamm-23.5/pybamm/expression_tree/printing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/printing/print_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/printing/sympy_overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/state_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    32988 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/unary_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/expression_tree/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.048914 pybamm-23.5/pybamm/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/geometry/battery_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/geometry/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/geometry/standard_spatial_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.048914 pybamm-23.5/pybamm/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.040914 pybamm-23.5/pybamm/input/discharge_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.048914 pybamm-23.5/pybamm/input/discharge_data/Ecker2015/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Ecker2015/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.052914 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/
--rw-r--r--   0 runner    (1001) docker     (123)   685399 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)   180796 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)   156316 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt
--rw-r--r--   0 runner    (1001) docker     (123)   129670 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38056 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)   125368 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt
--rw-r--r--   0 runner    (1001) docker     (123)    63563 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)   158837 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30602 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    13539 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    13828 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.052914 pybamm-23.5/pybamm/input/drive_cycles/
--rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/drive_cycles/UDDS.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/drive_cycles/US06.csv
--rw-r--r--   0 runner    (1001) docker     (123)   299508 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/drive_cycles/WLTC.csv
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/drive_cycles/car_current.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.052914 pybamm-23.5/pybamm/input/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.052914 pybamm-23.5/pybamm/input/parameters/ecm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/ecm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.052914 pybamm-23.5/pybamm/input/parameters/ecm/data/
--rw-r--r--   0 runner    (1001) docker     (123)   135520 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_c1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149886 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_r0.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149222 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_r1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/ecm/example_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.052914 pybamm-23.5/pybamm/input/parameters/lead_acid/
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lead_acid/Sulzer2019.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lead_acid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.056914 pybamm-23.5/pybamm/input/parameters/lithium_ion/
--rw-r--r--   0 runner    (1001) docker     (123)    25833 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/Chen2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/Chen2020_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/Ecker2015.py
--rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/Marquis2019.py
--rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/Mohtat2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py
--rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/OKane2022.py
--rw-r--r--   0 runner    (1001) docker     (123)    30791 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/ORegan2022.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/Prada2013.py
--rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/Ramadass2004.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/Xu2019.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.056914 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/install_odes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.056914 pybamm-23.5/pybamm/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/meshes/meshes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/meshes/one_dimensional_submeshes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/meshes/scikit_fem_submeshes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/meshes/zero_dimensional_submesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.056914 pybamm-23.5/pybamm/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47327 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.056914 pybamm-23.5/pybamm/models/full_battery_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56548 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/base_battery_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.056914 pybamm-23.5/pybamm/models/full_battery_models/equivalent_circuit/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/equivalent_circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.060914 pybamm-23.5/pybamm/models/full_battery_models/lead_acid/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lead_acid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lead_acid/basic_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lead_acid/full.py
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lead_acid/loqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.060914 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/Yang2017.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/basic_spm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/dfn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/mpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/spm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/spme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.060914 pybamm-23.5/pybamm/models/submodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.064914 pybamm-23.5/pybamm/models/submodels/active_material/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/active_material/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/active_material/base_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/active_material/constant_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/active_material/loss_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/active_material/total_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/base_submodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.064914 pybamm-23.5/pybamm/models/submodels/convection/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/base_convection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.064914 pybamm-23.5/pybamm/models/submodels/convection/through_cell/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/through_cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/through_cell/explicit_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/through_cell/full_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/through_cell/no_convection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.064914 pybamm-23.5/pybamm/models/submodels/convection/transverse/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/transverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/transverse/base_transverse_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/transverse/full_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/transverse/no_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/convection/transverse/uniform_convection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.064914 pybamm-23.5/pybamm/models/submodels/current_collector/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/current_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/current_collector/base_current_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/current_collector/homogeneous_current_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/current_collector/potential_pair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.064914 pybamm-23.5/pybamm/models/submodels/electrode/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrode/base_electrode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.068914 pybamm-23.5/pybamm/models/submodels/electrode/ohm/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrode/ohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrode/ohm/base_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrode/ohm/composite_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrode/ohm/full_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrode/ohm/leading_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrode/ohm/li_metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.068914 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.068914 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.068914 pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.072914 pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.072914 pybamm-23.5/pybamm/models/submodels/external_circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/external_circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/external_circuit/base_external_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/external_circuit/function_control_external_circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.072914 pybamm-23.5/pybamm/models/submodels/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/base_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.072914 pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.076914 pybamm-23.5/pybamm/models/submodels/interface/kinetics/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/base_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/butler_volmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/diffusion_limited.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.076914 pybamm-23.5/pybamm/models/submodels/interface/kinetics/inverse_kinetics/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/inverse_kinetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/marcus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/no_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/tafel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.076914 pybamm-23.5/pybamm/models/submodels/interface/lithium_plating/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/lithium_plating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/lithium_plating/base_plating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/lithium_plating/no_plating.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/lithium_plating/plating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.076914 pybamm-23.5/pybamm/models/submodels/interface/open_circuit_potential/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/open_circuit_potential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.076914 pybamm-23.5/pybamm/models/submodels/interface/sei/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/sei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/sei/base_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/sei/constant_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/sei/no_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/sei/sei_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/sei/total_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/interface/total_interfacial_current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.076914 pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.080914 pybamm-23.5/pybamm/models/submodels/particle/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle/base_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle/fickian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle/polynomial_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle/total_particle_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.080914 pybamm-23.5/pybamm/models/submodels/particle_mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle_mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle_mechanics/base_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle_mechanics/crack_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle_mechanics/no_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/particle_mechanics/swelling_only.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.080914 pybamm-23.5/pybamm/models/submodels/porosity/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/porosity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/porosity/base_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/porosity/constant_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/porosity/reaction_driven_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.080914 pybamm-23.5/pybamm/models/submodels/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/thermal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/thermal/base_thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/thermal/isothermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/thermal/lumped.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.080914 pybamm-23.5/pybamm/models/submodels/thermal/pouch_cell/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/thermal/pouch_cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/thermal/x_full.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.084914 pybamm-23.5/pybamm/models/submodels/transport_efficiency/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/transport_efficiency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.084914 pybamm-23.5/pybamm/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/base_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/bpx.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/ecm_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/electrical_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/geometric_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/lead_acid_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/lithium_ion_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/parameter_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)    32021 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/parameter_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/process_parameter_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/size_distribution_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters/thermal_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/parameters_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.084914 pybamm-23.5/pybamm/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/plotting/dynamic_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/plotting/plot2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/plotting/plot_summary_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/plotting/plot_voltage_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/plotting/quick_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    47298 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.088914 pybamm-23.5/pybamm/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/algebraic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    65427 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/base_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.088914 pybamm-23.5/pybamm/solvers/c_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/c_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/casadi_algebraic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    32028 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/casadi_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/dummy_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21833 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/idaklu_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    38492 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/jax_bdf_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/jax_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/lrudict.py
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/processed_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/scikits_dae_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/scikits_ode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/scipy_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/solvers/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.092914 pybamm-23.5/pybamm/spatial_methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/spatial_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57884 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/spatial_methods/finite_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/spatial_methods/scikit_finite_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/spatial_methods/spatial_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    28643 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/spatial_methods/spectral_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/spatial_methods/zero_dimensional_method.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.092914 pybamm-23.5/pybamm/step/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/step/_steps_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/step/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 10:39:23.000000 pybamm-23.5/pybamm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:30.044914 pybamm-23.5/pybamm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43197 2023-07-03 10:39:29.000000 pybamm-23.5/pybamm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-07-03 10:39:30.000000 pybamm-23.5/pybamm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:39:29.000000 pybamm-23.5/pybamm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-03 10:39:29.000000 pybamm-23.5/pybamm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-03 10:39:29.000000 pybamm-23.5/pybamm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 10:39:29.000000 pybamm-23.5/pybamm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:39:30.092914 pybamm-23.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-07-03 10:39:23.000000 pybamm-23.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-06-19 14:33:41.000000 pybamm-23.5rc0/CMakeBuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-19 14:33:41.000000 pybamm-23.5rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-06-19 14:33:45.928978 pybamm-23.5rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40154 2023-06-19 14:33:41.000000 pybamm-23.5rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.896978 pybamm-23.5rc0/pybamm/
+-rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/CITATIONS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/batch_study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/citations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.896978 pybamm-23.5rc0/pybamm/discretisations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/discretisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/discretisations/discretisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/doc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.896978 pybamm-23.5rc0/pybamm/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/expression_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/averages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/binary_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/broadcasts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/concatenations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/independent_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/input_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/interpolant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/expression_tree/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/convert_to_casadi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/evaluate_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/latexify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/unpack_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/expression_tree/printing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/printing/print_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/printing/sympy_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/state_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32988 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/unary_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/geometry/battery_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/geometry/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/geometry/standard_spatial_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.888978 pybamm-23.5rc0/pybamm/input/discharge_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/
+-rw-r--r--   0 runner    (1001) docker     (123)   685399 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   180796 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   156316 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   129670 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38056 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   125368 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    63563 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   158837 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30602 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13539 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13828 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/drive_cycles/
+-rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/drive_cycles/UDDS.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/drive_cycles/US06.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   299508 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/drive_cycles/WLTC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/drive_cycles/car_current.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/parameters/ecm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   135520 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_c1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149886 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_r0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149222 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_r1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/example_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/input/parameters/lead_acid/
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lead_acid/Sulzer2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lead_acid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/
+-rw-r--r--   0 runner    (1001) docker     (123)    25833 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Chen2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Chen2020_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ecker2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Marquis2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Mohtat2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/OKane2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30791 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/ORegan2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Prada2013.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ramadass2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Xu2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/install_odes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/one_dimensional_submeshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/scikit_fem_submeshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/zero_dimensional_submesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47327 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/models/full_battery_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56548 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/base_battery_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/basic_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/loqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/Yang2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_spm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/dfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/mpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/spm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/spme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/active_material/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/base_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/constant_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/loss_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/total_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/base_submodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/convection/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/base_convection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/explicit_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/full_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/no_convection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/base_transverse_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/full_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/no_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/uniform_convection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/current_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/base_current_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/homogeneous_current_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/potential_pair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrode/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/base_electrode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/base_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/composite_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/full_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/leading_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/li_metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/base_external_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/function_control_external_circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/base_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/base_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/butler_volmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/diffusion_limited.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/inverse_kinetics/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/inverse_kinetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/marcus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/no_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/tafel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/base_plating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/no_plating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/plating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/base_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/constant_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/no_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/sei_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/total_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/total_interfacial_current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/particle/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/base_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/fickian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/polynomial_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/total_particle_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/base_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/crack_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/no_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/swelling_only.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/porosity/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/base_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/constant_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/reaction_driven_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/base_thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/isothermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/lumped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/x_full.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/base_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/bpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/ecm_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/electrical_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/geometric_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/lead_acid_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/lithium_ion_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/parameter_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32021 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/parameter_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/process_parameter_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/size_distribution_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/thermal_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/dynamic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/plot2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/plot_summary_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/plot_voltage_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/quick_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47298 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/pybamm/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/algebraic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65427 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/base_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/pybamm/solvers/c_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/c_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/casadi_algebraic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32028 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/casadi_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/dummy_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21833 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/idaklu_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38492 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/jax_bdf_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/jax_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/lrudict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/processed_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/scikits_dae_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/scikits_ode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/scipy_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/pybamm/spatial_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57884 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/finite_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/scikit_finite_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/spatial_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28643 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/spectral_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/zero_dimensional_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/pybamm/step/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/step/_steps_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/step/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.896978 pybamm-23.5rc0/pybamm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:33:45.928978 pybamm-23.5rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-06-19 14:33:41.000000 pybamm-23.5rc0/setup.py
```

### Comparing `pybamm-23.5/CMakeBuild.py` & `pybamm-23.5rc0/CMakeBuild.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/LICENSE.txt` & `pybamm-23.5rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/PKG-INFO` & `pybamm-23.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybamm
-Version: 23.5
+Version: 23.5rc0
 Summary: Python Battery Mathematical Modelling.
 Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN
 Description: ![PyBaMM_logo](https://user-images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-7ebef7c72a1e.png)
         
         #
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybamm Version: 23.5 Summary: Python Battery
+Metadata-Version: 2.1 Name: pybamm Version: 23.5rc0 Summary: Python Battery
 Mathematical Modelling. Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN Description: ![PyBaMM_logo](https://user-
 images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-
 7ebef7c72a1e.png) #
   [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-
   orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org) [!
      [Scheduled](https://github.com/pybamm-team/PyBaMM/actions/workflows/
```

### Comparing `pybamm-23.5/README.md` & `pybamm-23.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/CITATIONS.txt` & `pybamm-23.5rc0/pybamm/CITATIONS.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/__init__.py` & `pybamm-23.5rc0/pybamm/__init__.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/batch_study.py` & `pybamm-23.5rc0/pybamm/batch_study.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/callbacks.py` & `pybamm-23.5rc0/pybamm/callbacks.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/citations.py` & `pybamm-23.5rc0/pybamm/citations.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/discretisations/discretisation.py` & `pybamm-23.5rc0/pybamm/discretisations/discretisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/doc_utils.py` & `pybamm-23.5rc0/pybamm/doc_utils.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/experiment/experiment.py` & `pybamm-23.5rc0/pybamm/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/array.py` & `pybamm-23.5rc0/pybamm/expression_tree/array.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/averages.py` & `pybamm-23.5rc0/pybamm/expression_tree/averages.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/binary_operators.py` & `pybamm-23.5rc0/pybamm/expression_tree/binary_operators.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/broadcasts.py` & `pybamm-23.5rc0/pybamm/expression_tree/broadcasts.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/concatenations.py` & `pybamm-23.5rc0/pybamm/expression_tree/concatenations.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/exceptions.py` & `pybamm-23.5rc0/pybamm/expression_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/functions.py` & `pybamm-23.5rc0/pybamm/expression_tree/functions.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/independent_variable.py` & `pybamm-23.5rc0/pybamm/expression_tree/independent_variable.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/input_parameter.py` & `pybamm-23.5rc0/pybamm/expression_tree/input_parameter.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/interpolant.py` & `pybamm-23.5rc0/pybamm/expression_tree/interpolant.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/matrix.py` & `pybamm-23.5rc0/pybamm/expression_tree/matrix.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/operations/convert_to_casadi.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/convert_to_casadi.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/operations/evaluate_python.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/evaluate_python.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/operations/jacobian.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/jacobian.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/operations/latexify.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/latexify.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/operations/unpack_symbols.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/unpack_symbols.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/parameter.py` & `pybamm-23.5rc0/pybamm/expression_tree/parameter.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/printing/print_name.py` & `pybamm-23.5rc0/pybamm/expression_tree/printing/print_name.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/printing/sympy_overrides.py` & `pybamm-23.5rc0/pybamm/expression_tree/printing/sympy_overrides.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/scalar.py` & `pybamm-23.5rc0/pybamm/expression_tree/scalar.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/state_vector.py` & `pybamm-23.5rc0/pybamm/expression_tree/state_vector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/symbol.py` & `pybamm-23.5rc0/pybamm/expression_tree/symbol.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/unary_operators.py` & `pybamm-23.5rc0/pybamm/expression_tree/unary_operators.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/variable.py` & `pybamm-23.5rc0/pybamm/expression_tree/variable.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/expression_tree/vector.py` & `pybamm-23.5rc0/pybamm/expression_tree/vector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/geometry/battery_geometry.py` & `pybamm-23.5rc0/pybamm/geometry/battery_geometry.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/geometry/geometry.py` & `pybamm-23.5rc0/pybamm/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/geometry/standard_spatial_vars.py` & `pybamm-23.5rc0/pybamm/geometry/standard_spatial_vars.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv` & `pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv` & `pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Ecker2015/README.md` & `pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/README.md` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/drive_cycles/UDDS.csv` & `pybamm-23.5rc0/pybamm/input/drive_cycles/UDDS.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/drive_cycles/US06.csv` & `pybamm-23.5rc0/pybamm/input/drive_cycles/US06.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/drive_cycles/WLTC.csv` & `pybamm-23.5rc0/pybamm/input/drive_cycles/WLTC.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_c1.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_c1.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_r0.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_r0.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/ecm/data/ecm_example_r1.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_r1.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/ecm/example_set.py` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/example_set.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lead_acid/Sulzer2019.py` & `pybamm-23.5rc0/pybamm/input/parameters/lead_acid/Sulzer2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/Ai2020.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/Chen2020.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Chen2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/Chen2020_composite.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Chen2020_composite.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/Ecker2015.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ecker2015.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/Marquis2019.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Marquis2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/Mohtat2020.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Mohtat2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/OKane2022.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/OKane2022.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/ORegan2022.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/ORegan2022.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/Prada2013.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Prada2013.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/Ramadass2004.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ramadass2004.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/Xu2019.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Xu2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/install_odes.py` & `pybamm-23.5rc0/pybamm/install_odes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/logger.py` & `pybamm-23.5rc0/pybamm/logger.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/meshes/meshes.py` & `pybamm-23.5rc0/pybamm/meshes/meshes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/meshes/one_dimensional_submeshes.py` & `pybamm-23.5rc0/pybamm/meshes/one_dimensional_submeshes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/meshes/scikit_fem_submeshes.py` & `pybamm-23.5rc0/pybamm/meshes/scikit_fem_submeshes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/meshes/zero_dimensional_submesh.py` & `pybamm-23.5rc0/pybamm/meshes/zero_dimensional_submesh.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/base_model.py` & `pybamm-23.5rc0/pybamm/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/event.py` & `pybamm-23.5rc0/pybamm/models/event.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/base_battery_model.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/base_battery_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lead_acid/basic_full.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/basic_full.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lead_acid/full.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/full.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lead_acid/loqs.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/loqs.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/__init__.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/__init__.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/basic_spm.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_spm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/dfn.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/dfn.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/mpm.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/mpm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/spm.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/spm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/full_battery_models/lithium_ion/spme.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/spme.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/active_material/base_active_material.py` & `pybamm-23.5rc0/pybamm/models/submodels/active_material/base_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/active_material/constant_active_material.py` & `pybamm-23.5rc0/pybamm/models/submodels/active_material/constant_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/active_material/loss_active_material.py` & `pybamm-23.5rc0/pybamm/models/submodels/active_material/loss_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/active_material/total_active_material.py` & `pybamm-23.5rc0/pybamm/models/submodels/active_material/total_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/base_submodel.py` & `pybamm-23.5rc0/pybamm/models/submodels/base_submodel.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/convection/base_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/base_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/convection/through_cell/explicit_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/explicit_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/convection/through_cell/full_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/full_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/convection/through_cell/no_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/no_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/convection/transverse/base_transverse_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/base_transverse_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/convection/transverse/full_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/full_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/convection/transverse/no_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/no_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/convection/transverse/uniform_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/uniform_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/current_collector/base_current_collector.py` & `pybamm-23.5rc0/pybamm/models/submodels/current_collector/base_current_collector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py` & `pybamm-23.5rc0/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/current_collector/homogeneous_current_collector.py` & `pybamm-23.5rc0/pybamm/models/submodels/current_collector/homogeneous_current_collector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/current_collector/potential_pair.py` & `pybamm-23.5rc0/pybamm/models/submodels/current_collector/potential_pair.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrode/base_electrode.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/base_electrode.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrode/ohm/base_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/base_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrode/ohm/composite_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/composite_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrode/ohm/full_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/full_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrode/ohm/leading_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/leading_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrode/ohm/li_metal.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/li_metal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/thermal.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/thermal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/external_circuit/base_external_circuit.py` & `pybamm-23.5rc0/pybamm/models/submodels/external_circuit/base_external_circuit.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py` & `pybamm-23.5rc0/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/external_circuit/function_control_external_circuit.py` & `pybamm-23.5rc0/pybamm/models/submodels/external_circuit/function_control_external_circuit.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/base_interface.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/base_interface.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/__init__.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/__init__.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/base_kinetics.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/base_kinetics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/butler_volmer.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/butler_volmer.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/diffusion_limited.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/diffusion_limited.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/linear.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/linear.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/marcus.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/marcus.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/no_reaction.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/no_reaction.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/tafel.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/tafel.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/lithium_plating/base_plating.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/base_plating.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/lithium_plating/no_plating.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/no_plating.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/lithium_plating/plating.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/plating.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/sei/base_sei.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/base_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/sei/constant_sei.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/constant_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/sei/no_sei.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/no_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/sei/sei_growth.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/sei_growth.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/sei/total_sei.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/total_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/interface/total_interfacial_current.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/total_interfacial_current.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py` & `pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/particle/base_particle.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/base_particle.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/particle/fickian_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/fickian_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/particle/polynomial_profile.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/polynomial_profile.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/particle/total_particle_concentration.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/total_particle_concentration.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/particle_mechanics/base_mechanics.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/base_mechanics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/particle_mechanics/crack_propagation.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/crack_propagation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/particle_mechanics/no_mechanics.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/no_mechanics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/particle_mechanics/swelling_only.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/swelling_only.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/porosity/base_porosity.py` & `pybamm-23.5rc0/pybamm/models/submodels/porosity/base_porosity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/porosity/constant_porosity.py` & `pybamm-23.5rc0/pybamm/models/submodels/porosity/constant_porosity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/porosity/reaction_driven_porosity.py` & `pybamm-23.5rc0/pybamm/models/submodels/porosity/reaction_driven_porosity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py` & `pybamm-23.5rc0/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/thermal/base_thermal.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/base_thermal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/thermal/isothermal.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/isothermal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/thermal/lumped.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/lumped.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/thermal/x_full.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/x_full.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py` & `pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py` & `pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/base_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/base_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/bpx.py` & `pybamm-23.5rc0/pybamm/parameters/bpx.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/ecm_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/ecm_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/electrical_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/electrical_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/geometric_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/geometric_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/lead_acid_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/lead_acid_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/lithium_ion_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/lithium_ion_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/parameter_sets.py` & `pybamm-23.5rc0/pybamm/parameters/parameter_sets.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/parameter_values.py` & `pybamm-23.5rc0/pybamm/parameters/parameter_values.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/process_parameter_data.py` & `pybamm-23.5rc0/pybamm/parameters/process_parameter_data.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/size_distribution_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/size_distribution_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/parameters/thermal_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/thermal_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/plotting/dynamic_plot.py` & `pybamm-23.5rc0/pybamm/plotting/dynamic_plot.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/plotting/plot.py` & `pybamm-23.5rc0/pybamm/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/plotting/plot2D.py` & `pybamm-23.5rc0/pybamm/plotting/plot2D.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/plotting/plot_summary_variables.py` & `pybamm-23.5rc0/pybamm/plotting/plot_summary_variables.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/plotting/plot_voltage_components.py` & `pybamm-23.5rc0/pybamm/plotting/plot_voltage_components.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/plotting/quick_plot.py` & `pybamm-23.5rc0/pybamm/plotting/quick_plot.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/settings.py` & `pybamm-23.5rc0/pybamm/settings.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/simulation.py` & `pybamm-23.5rc0/pybamm/simulation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/algebraic_solver.py` & `pybamm-23.5rc0/pybamm/solvers/algebraic_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/base_solver.py` & `pybamm-23.5rc0/pybamm/solvers/base_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/casadi_algebraic_solver.py` & `pybamm-23.5rc0/pybamm/solvers/casadi_algebraic_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/casadi_solver.py` & `pybamm-23.5rc0/pybamm/solvers/casadi_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/dummy_solver.py` & `pybamm-23.5rc0/pybamm/solvers/dummy_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/idaklu_solver.py` & `pybamm-23.5rc0/pybamm/solvers/idaklu_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/jax_bdf_solver.py` & `pybamm-23.5rc0/pybamm/solvers/jax_bdf_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/jax_solver.py` & `pybamm-23.5rc0/pybamm/solvers/jax_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/lrudict.py` & `pybamm-23.5rc0/pybamm/solvers/lrudict.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/processed_variable.py` & `pybamm-23.5rc0/pybamm/solvers/processed_variable.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/scikits_dae_solver.py` & `pybamm-23.5rc0/pybamm/solvers/scikits_dae_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/scikits_ode_solver.py` & `pybamm-23.5rc0/pybamm/solvers/scikits_ode_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/scipy_solver.py` & `pybamm-23.5rc0/pybamm/solvers/scipy_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/solvers/solution.py` & `pybamm-23.5rc0/pybamm/solvers/solution.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/spatial_methods/finite_volume.py` & `pybamm-23.5rc0/pybamm/spatial_methods/finite_volume.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/spatial_methods/scikit_finite_element.py` & `pybamm-23.5rc0/pybamm/spatial_methods/scikit_finite_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/spatial_methods/spatial_method.py` & `pybamm-23.5rc0/pybamm/spatial_methods/spatial_method.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/spatial_methods/spectral_volume.py` & `pybamm-23.5rc0/pybamm/spatial_methods/spectral_volume.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/spatial_methods/zero_dimensional_method.py` & `pybamm-23.5rc0/pybamm/spatial_methods/zero_dimensional_method.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/step/_steps_util.py` & `pybamm-23.5rc0/pybamm/step/_steps_util.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/step/steps.py` & `pybamm-23.5rc0/pybamm/step/steps.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm/util.py` & `pybamm-23.5rc0/pybamm/util.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm.egg-info/PKG-INFO` & `pybamm-23.5rc0/pybamm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybamm
-Version: 23.5
+Version: 23.5rc0
 Summary: Python Battery Mathematical Modelling.
 Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN
 Description: ![PyBaMM_logo](https://user-images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-7ebef7c72a1e.png)
         
         #
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybamm Version: 23.5 Summary: Python Battery
+Metadata-Version: 2.1 Name: pybamm Version: 23.5rc0 Summary: Python Battery
 Mathematical Modelling. Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN Description: ![PyBaMM_logo](https://user-
 images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-
 7ebef7c72a1e.png) #
   [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-
   orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org) [!
      [Scheduled](https://github.com/pybamm-team/PyBaMM/actions/workflows/
```

### Comparing `pybamm-23.5/pybamm.egg-info/SOURCES.txt` & `pybamm-23.5rc0/pybamm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/pybamm.egg-info/entry_points.txt` & `pybamm-23.5rc0/pybamm.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.5/setup.py` & `pybamm-23.5rc0/setup.py`

 * *Files identical despite different names*

