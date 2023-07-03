# Comparing `tmp/electricalsim-0.0.7.0.tar.gz` & `tmp/electricalsim-0.0.7.1.tar.gz`

## Comparing `electricalsim-0.0.7.0.tar` & `electricalsim-0.0.7.1.tar`

### file list

```diff
@@ -1,84 +1,85 @@
--rw-r--r--   0        0        0    18506 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/README.md
--rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/10_PF4.png
--rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/11_PF_tooltips.png
--rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/12_App_settings.png
--rw-r--r--   0        0        0    50389 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/13_Disabling_nodes.png
--rw-r--r--   0        0        0    69759 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/14_Context_menu.png
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/15_Extension_manager.png
--rw-r--r--   0        0        0   124772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/1_Main_Window.png
--rw-r--r--   0        0        0   122916 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/1_Main_Window_dark.png
--rw-r--r--   0        0        0   149680 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/2_Dialogs.png
--rw-r--r--   0        0        0    25172 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/3_Widgets.png
--rw-r--r--   0        0        0   134645 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/4_Pandapower_DataFrames.png
--rw-r--r--   0        0        0    16870 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/5_Connections_angle_b.png
--rw-r--r--   0        0        0    21425 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/5_Connections_curved_b.png
--rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/5_Connections_straight_b.png
--rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/6_Line_and_transformer_nodes.png
--rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/7_PF1.png
--rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/8_PF2.png
--rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/9_PF3.png
--rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/app_icon.png
--rw-r--r--   0        0        0    22462 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/Electrical_Grid_Simulator.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/__init__.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/config.ini
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/egs_create_shortcut.py
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/egs_run.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/version.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/electricalsim.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/modules.xml
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/workspace.xml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/extensions/extension_classes.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/hotkeys/hotkey_functions.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/hotkeys/hotkeys.json
--rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.ico
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.png
--rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.svg
--rw-r--r--   0        0        0    30015 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/auxiliary.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/calculations.py
--rw-r--r--   0        0        0   208285 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/electricalGraph.py
--rw-r--r--   0        0        0    83266 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/main_components.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/table_widget.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/about_dialog.ui
--rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/aload_dialog.ui
--rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/asgen_dialog.ui
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/bus_dialog.ui
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_bus_switch.ui
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_generator_type.ui
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_line_type.ui
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_load_type.ui
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_transformer_type.ui
--rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/dcline_dialog.ui
--rw-r--r--   0        0        0   138693 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/dialogs.py
--rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/ext_grid_dialog.ui
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/extension.ui
--rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/gen_dialog.ui
--rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/impedance_dialog.ui
--rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/line_dialog.ui
--rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/load_dialog.ui
--rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/main_window.ui
--rw-r--r--   0        0        0    12741 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/main_window_backup.ui
--rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/motor_dialog.ui
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/network_settings_dialog.ui
--rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/pf_settings_widget.ui
--rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/power_flow_dialog.ui
--rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/settings_dialog.ui
--rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/sgen_dialog.ui
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/shunt_dialog.ui
--rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/stdline_dialog.ui
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/stdtransformer3w_dialog.ui
--rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/stdtransformer_dialog.ui
--rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/storage_dialog.ui
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/switch_dialog.ui
--rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/transformer3w_dialog.ui
--rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/transformer_dialog.ui
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/ward_dialog.ui
--rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/xward_dialog.ui
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/LICENSE
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/README_PyPI.md
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    18645 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/README.md
+-rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/10_PF4.png
+-rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/11_PF_tooltips.png
+-rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/12_App_settings.png
+-rw-r--r--   0        0        0    50389 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/13_Disabling_nodes.png
+-rw-r--r--   0        0        0   114751 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/14_Context_menu.png
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/15_Extension_manager.png
+-rw-r--r--   0        0        0   124772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/1_Main_Window.png
+-rw-r--r--   0        0        0   122916 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/1_Main_Window_dark.png
+-rw-r--r--   0        0        0   149680 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/2_Dialogs.png
+-rw-r--r--   0        0        0    25172 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/3_Widgets.png
+-rw-r--r--   0        0        0   134645 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/4_Pandapower_DataFrames.png
+-rw-r--r--   0        0        0    16870 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/5_Connections_angle_b.png
+-rw-r--r--   0        0        0    21425 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/5_Connections_curved_b.png
+-rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/5_Connections_straight_b.png
+-rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/6_Line_and_transformer_nodes.png
+-rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/7_PF1.png
+-rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/8_PF2.png
+-rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/9_PF3.png
+-rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/app_icon.png
+-rw-r--r--   0        0        0    22462 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/Electrical_Grid_Simulator.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/__init__.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/config.ini
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/egs_create_shortcut.py
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/egs_run.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/version.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/electricalsim.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/modules.xml
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/workspace.xml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/extensions/extension_classes.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/hotkeys/hotkey_functions.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/hotkeys/hotkeys.json
+-rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.ico
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.png
+-rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.svg
+-rw-r--r--   0        0        0    30015 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/auxiliary.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/calculations.py
+-rw-r--r--   0        0        0   213066 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/electricalGraph.py
+-rw-r--r--   0        0        0    81561 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/main_components.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/table_widget.py
+-rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/about_dialog.ui
+-rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/aload_dialog.ui
+-rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/asgen_dialog.ui
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/bus_dialog.ui
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_bus_switch.ui
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_generator_type.ui
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_line_type.ui
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_load_type.ui
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_transformer_type.ui
+-rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/dcline_dialog.ui
+-rw-r--r--   0        0        0   138693 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/dialogs.py
+-rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/ext_grid_dialog.ui
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/extension.ui
+-rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/gen_dialog.ui
+-rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/impedance_dialog.ui
+-rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/line_dialog.ui
+-rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/load_dialog.ui
+-rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/main_window.ui
+-rw-r--r--   0        0        0    12741 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/main_window_backup.ui
+-rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/motor_dialog.ui
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/network_settings_dialog.ui
+-rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/pf_settings_widget.ui
+-rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/power_flow_dialog.ui
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/settings_dialog.ui
+-rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/sgen_dialog.ui
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/shunt_dialog.ui
+-rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/stdline_dialog.ui
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/stdtransformer3w_dialog.ui
+-rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/stdtransformer_dialog.ui
+-rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/storage_dialog.ui
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/switch_dialog.ui
+-rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/transformer3w_dialog.ui
+-rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/transformer_dialog.ui
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/ward_dialog.ui
+-rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/xward_dialog.ui
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/LICENSE
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/README_PyPI.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/PKG-INFO
```

### Comparing `electricalsim-0.0.7.0/README.md` & `electricalsim-0.0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,15 @@
 | ```Ctrl+Z``` | Undo |
 | ```Ctrl+Shift+Z``` | Redo |
 | ```Del``` | Delete selected components in the **Graph** |
 | ```Ctrl+A``` | Select all the nodes in the **Graph** |
 | ```Ctrl+Shift+A``` | Unselect what is selected |
 | ```D``` | Disable the selected nodes |
 | ```R``` | Flip the selected nodes (works only with nodes that have only one port) |
+| ```Ctrl+D``` | Duplicate the selected nodes (switches cannot be duplicated) |
 | ```Ctrl++``` | Zoom in |
 | ```Ctrl+-``` | Zoom out |
 | ```=``` | Reset zoom |
 | ```F``` | Adjust the zoom level according to the selection |
 | ```V``` | Change selected nodes to the vertical layout |
 | ```H``` | Change selected nodes to the horizontal layout |
 | ```Shift+V``` | Apply a vertical alignment to selected nodes |
@@ -305,21 +306,21 @@
 python -m pip uninstall electricalsim
 ```
 
 Note that shortcuts added with the ```egs-create-shortcut``` command are not removed. So you must delete them manually.
 
 ## Installing extensions
 
-Extensions available in the PyPI repository can be installed using ```pip```. For example, the Optimal Power Flow extension is installed with:
+Extensions available in the PyPI repository can be installed using ```pip```. For example, the [Optimal Power Flow extension](https://github.com/aloytag/electricalsim-opf-quadratic) is installed with:
 
 ```bash
 pip install electricalsim-opf-quadratic
 ```
 
 On MS Windows:
 ```bash
 python -m pip install electricalsim-opf-quadratic
 ```
 
 # License
 
-This project uses the [MIT license](https://github.com/aloytag/electrical-grid-simulator/blob/main/LICENSE).
+This project uses the [MIT license](https://github.com/aloytag/electrical-grid-simulator/blob/main/LICENSE).
```

### Comparing `electricalsim-0.0.7.0/img/10_PF4.png` & `electricalsim-0.0.7.1/img/10_PF4.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/11_PF_tooltips.png` & `electricalsim-0.0.7.1/img/11_PF_tooltips.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/12_App_settings.png` & `electricalsim-0.0.7.1/img/12_App_settings.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/13_Disabling_nodes.png` & `electricalsim-0.0.7.1/img/13_Disabling_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/15_Extension_manager.png` & `electricalsim-0.0.7.1/img/15_Extension_manager.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/1_Main_Window.png` & `electricalsim-0.0.7.1/img/1_Main_Window.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/1_Main_Window_dark.png` & `electricalsim-0.0.7.1/img/1_Main_Window_dark.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/2_Dialogs.png` & `electricalsim-0.0.7.1/img/2_Dialogs.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/3_Widgets.png` & `electricalsim-0.0.7.1/img/3_Widgets.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/4_Pandapower_DataFrames.png` & `electricalsim-0.0.7.1/img/4_Pandapower_DataFrames.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/5_Connections_angle_b.png` & `electricalsim-0.0.7.1/img/5_Connections_angle_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/5_Connections_curved_b.png` & `electricalsim-0.0.7.1/img/5_Connections_curved_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/5_Connections_straight_b.png` & `electricalsim-0.0.7.1/img/5_Connections_straight_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/6_Line_and_transformer_nodes.png` & `electricalsim-0.0.7.1/img/6_Line_and_transformer_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/7_PF1.png` & `electricalsim-0.0.7.1/img/7_PF1.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/8_PF2.png` & `electricalsim-0.0.7.1/img/8_PF2.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/9_PF3.png` & `electricalsim-0.0.7.1/img/9_PF3.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/Logo_CIESE_2021 y UTN_Sta_Fe.png` & `electricalsim-0.0.7.1/img/Logo_CIESE_2021 y UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/img/app_icon.png` & `electricalsim-0.0.7.1/img/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/Electrical_Grid_Simulator.py` & `electricalsim-0.0.7.1/src/electricalsim/Electrical_Grid_Simulator.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/config.ini` & `electricalsim-0.0.7.1/src/electricalsim/config.ini`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/egs_create_shortcut.py` & `electricalsim-0.0.7.1/src/electricalsim/egs_create_shortcut.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/.idea/workspace.xml` & `electricalsim-0.0.7.1/src/electricalsim/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `electricalsim-0.0.7.0/src/electricalsim/.idea/workspace.xml` & `electricalsim-0.0.7.1/src/electricalsim/.idea/workspace.xml`

```diff
@@ -6,14 +6,17 @@
   <component name="ChangeListManager">
     <list default="true" id="7ae9bfe0-2313-4170-a51d-1d820a8ea6bd" name="Changes" comment=""/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
+  <component name="ProblemsViewState">
+    <option name="selectedTabId" value="CurrentFile"/>
+  </component>
   <component name="ProjectId" id="2MKCBopZy5dPlZhrEXWU7Iz8rBU"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showExcludedFiles" value="false"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">{
```

### Comparing `electricalsim-0.0.7.0/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml` & `electricalsim-0.0.7.1/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/extensions/extension_classes.py` & `electricalsim-0.0.7.1/src/electricalsim/extensions/extension_classes.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/hotkeys/hotkey_functions.py` & `electricalsim-0.0.7.1/src/electricalsim/hotkeys/hotkey_functions.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # ------------------------------------------------------------------------------
 # menu command functions
 # ------------------------------------------------------------------------------
 
 import os
 
 from Qt import QtGui
+import pandapower as pp
 
 directory = os.path.dirname(__file__)
 root_directory, _ = os.path.split(directory)
 icon_app_path = os.path.join(root_directory, 'icons', 'app_icon.png')
 
 
 def horizontal_layout(graph):
@@ -230,7 +231,33 @@
     """
     selected = graph.selected_nodes()
     if selected:
         last_node = selected[-1]
         pos = last_node.x_pos()
         for node in selected[:-1]:
             node.set_x_pos(pos)
+
+
+def duplicate_nodes(graph):
+    """
+    Duplicates the selected nodes, with Switches as the only exception.
+    """
+    selected = graph.selected_nodes()
+    for node in selected:
+        if node.type_=='SwitchNode.SwitchNode':
+            continue
+        node_duplicated = list(graph.duplicate_nodes([node]))[0]
+        input_ports = node_duplicated.input_ports()
+        output_ports = node_duplicated.output_ports()
+        for port_in in input_ports:
+            port_in.clear_connections(push_undo=False)
+        for port_out in output_ports:
+            port_out.clear_connections(push_undo=False)
+        if node_duplicated.type_=='BusNode.BusNode':
+            bus_index = pp.create_bus(graph.net,
+                                      name=node_duplicated.get_property('name'),
+                                      vn_kv=graph.net.bus.at[node.get_property('bus_index'), 'vn_kv'],
+                                      min_vm_pu=graph.net.bus.at[node.get_property('bus_index'), 'min_vm_pu'],
+                                      max_vm_pu=graph.net.bus.at[node.get_property('bus_index'), 'max_vm_pu'],
+                                      in_service=graph.net.bus.at[node.get_property('bus_index'), 'in_service'],
+                                      geodata=node_duplicated.pos())
+            node_duplicated.set_property('bus_index', bus_index, push_undo=False)
```

### Comparing `electricalsim-0.0.7.0/src/electricalsim/hotkeys/hotkeys.json` & `electricalsim-0.0.7.1/src/electricalsim/hotkeys/hotkeys.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962962962962963%*

 * *Differences: {'0': "{'items': {insert: [(9, OrderedDict([('type', 'command'), ('label', 'Duplicate'), ('file', "*

 * *      "'./hotkeys/hotkey_functions.py'), ('function_name', 'duplicate_nodes'), ('shortcut', "*

 * *      "'Ctrl+D')]))]}}"}*

```diff
@@ -53,14 +53,21 @@
                 "file": "./hotkeys/hotkey_functions.py",
                 "function_name": "flip_nodes",
                 "label": "Flip",
                 "shortcut": "R",
                 "type": "command"
             },
             {
+                "file": "./hotkeys/hotkey_functions.py",
+                "function_name": "duplicate_nodes",
+                "label": "Duplicate",
+                "shortcut": "Ctrl+D",
+                "type": "command"
+            },
+            {
                 "type": "separator"
             },
             {
                 "file": "./hotkeys/hotkey_functions.py",
                 "function_name": "fit_to_selection",
                 "label": "Fit to Selection",
                 "shortcut": "F",
```

### Comparing `electricalsim-0.0.7.0/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png` & `electricalsim-0.0.7.1/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.ico` & `electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.ico`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.png` & `electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.svg` & `electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/lib/auxiliary.py` & `electricalsim-0.0.7.1/src/electricalsim/lib/auxiliary.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/lib/electricalGraph.py` & `electricalsim-0.0.7.1/src/electricalsim/lib/electricalGraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 import os
 import warnings
 from math import isnan, nan
 import pickle
 
+from NodeGraphQt.base.commands import PortConnectedCmd
 from Qt import QtGui, QtWidgets, QtCore
 
-from NodeGraphQt import NodeGraph, errors
+from NodeGraphQt import NodeGraph, errors, BaseNode
 from NodeGraphQt.constants import PortTypeEnum, PipeLayoutEnum
 import pandapower as pp
 # from pandapower.toolbox import drop_from_groups
 from pandapower.toolbox import drop_elements
 import numpy as np
 
 from lib.main_components import (BusNode, LineNode, StdLineNode, DCLineNode,
@@ -41,33 +42,33 @@
 
 warnings.simplefilter(action='ignore', category=FutureWarning)
 directory = os.path.dirname(__file__)
 root_directory, _ = os.path.split(directory)
 icon_path = os.path.join(root_directory, 'icons', 'app_icon.png')
 
 allowed_connections = (
-            set(('BusNode.BusNode', 'LineNode.LineNode')),
-            set(('BusNode.BusNode', 'StdLineNode.StdLineNode')),
-            set(('BusNode.BusNode', 'DCLineNode.DCLineNode')),
-            set(('BusNode.BusNode', 'ImpedanceNode.ImpedanceNode')),
-            set(('BusNode.BusNode', 'TrafoNode.TrafoNode')),
-            set(('BusNode.BusNode', 'StdTrafoNode.StdTrafoNode')),
-            set(('BusNode.BusNode', 'Trafo3wNode.Trafo3wNode')),
-            set(('BusNode.BusNode', 'StdTrafo3wNode.StdTrafo3wNode')),
-            set(('BusNode.BusNode', 'GenNode.GenNode')),
-            set(('BusNode.BusNode', 'SGenNode.SGenNode')),
-            set(('BusNode.BusNode', 'ASGenNode.ASGenNode')),
-            set(('BusNode.BusNode', 'ExtGridNode.ExtGridNode')),
-            set(('BusNode.BusNode', 'LoadNode.LoadNode')),
-            set(('BusNode.BusNode', 'ALoadNode.ALoadNode')),
-            set(('BusNode.BusNode', 'ShuntNode.ShuntNode')),
-            set(('BusNode.BusNode', 'MotorNode.MotorNode')),
-            set(('BusNode.BusNode', 'WardNode.WardNode')),
-            set(('BusNode.BusNode', 'XWardNode.XWardNode')),
-            set(('BusNode.BusNode', 'StorageNode.StorageNode'))
+    {'BusNode.BusNode', 'LineNode.LineNode'},
+    {'BusNode.BusNode', 'StdLineNode.StdLineNode'},
+    {'BusNode.BusNode', 'DCLineNode.DCLineNode'},
+    {'BusNode.BusNode', 'ImpedanceNode.ImpedanceNode'},
+    {'BusNode.BusNode', 'TrafoNode.TrafoNode'},
+    {'BusNode.BusNode', 'StdTrafoNode.StdTrafoNode'},
+    {'BusNode.BusNode', 'Trafo3wNode.Trafo3wNode'},
+    {'BusNode.BusNode', 'StdTrafo3wNode.StdTrafo3wNode'},
+    {'BusNode.BusNode', 'GenNode.GenNode'},
+    {'BusNode.BusNode', 'SGenNode.SGenNode'},
+    {'BusNode.BusNode', 'ASGenNode.ASGenNode'},
+    {'BusNode.BusNode', 'ExtGridNode.ExtGridNode'},
+    {'BusNode.BusNode', 'LoadNode.LoadNode'},
+    {'BusNode.BusNode', 'ALoadNode.ALoadNode'},
+    {'BusNode.BusNode', 'ShuntNode.ShuntNode'},
+    {'BusNode.BusNode', 'MotorNode.MotorNode'},
+    {'BusNode.BusNode', 'WardNode.WardNode'},
+    {'BusNode.BusNode', 'XWardNode.XWardNode'},
+    {'BusNode.BusNode', 'StorageNode.StorageNode'}
         )
 
 
 class ElectricalGraph(NodeGraph):
     """
     A graph with nodes representing components of an electrical network.
     Includes a pandapower network as an attribute.
@@ -207,15 +208,140 @@
         self._undo_stack.beginMacro('move nodes')
         for node_view, prev_pos in node_data.items():
             node = self._model.nodes[node_view.id]
             self._undo_stack.push(NodeMovedCmd(node, node.pos(), prev_pos, self))  # Adding 'self' as last argument
         self._undo_stack.endMacro()
 
         self.session_change_warning(tooltip_default=False)
-        
+
+    def duplicate_nodes(self, nodes):
+        """
+        MODIFIED VERSION FROM NodeGraph CLASS WITHOUT UNDO
+
+        Create duplicate copy from the list of nodes.
+
+        Args:
+            nodes (list[NodeGraphQt.BaseNode]): list of nodes.
+        Returns:
+            list[NodeGraphQt.BaseNode]: list of duplicated node instances.
+        """
+        if not nodes:
+            return
+
+        # self._undo_stack.beginMacro('duplicate nodes')
+
+        self.clear_selection()
+        serial = self._serialize(nodes)
+        new_nodes = self._deserialize2(serial)
+        offset = 50
+        for n in new_nodes:
+            x, y = n.pos()
+            n.set_pos(x + offset, y + offset)
+            n.set_property('selected', True)
+
+        # self._undo_stack.endMacro()
+        return new_nodes
+
+    def _deserialize2(self, data, relative_pos=False, pos=None):
+        """
+        ALTERNATIVE TO _deserialize2 METHOD WITHOUT push_undo
+
+        deserialize node data.
+        (used internally by the node graph)
+
+        Args:
+            data (dict): node data.
+            relative_pos (bool): position node relative to the cursor.
+            pos (tuple or list): custom x, y position.
+
+        Returns:
+            list[NodeGraphQt.Nodes]: list of node instances.
+        """
+        # update node graph properties.
+        for attr_name, attr_value in data.get('graph', {}).items():
+            if attr_name == 'layout_direction':
+                self.set_layout_direction(attr_value)
+            elif attr_name == 'acyclic':
+                self.set_acyclic(attr_value)
+            elif attr_name == 'pipe_collision':
+                self.set_pipe_collision(attr_value)
+            elif attr_name == 'pipe_slicing':
+                self.set_pipe_slicing(attr_value)
+            elif attr_name == 'pipe_style':
+                self.set_pipe_style(attr_value)
+
+            # connection constrains.
+            elif attr_name == 'accept_connection_types':
+                self.model.accept_connection_types = attr_value
+            elif attr_name == 'reject_connection_types':
+                self.model.reject_connection_types = attr_value
+
+        # build the nodes.
+        nodes = {}
+        for n_id, n_data in data.get('nodes', {}).items():
+            identifier = n_data['type_']
+            node = self._node_factory.create_node_instance(identifier)
+            if node:
+                node.NODE_NAME = n_data.get('name', node.NODE_NAME)
+                # set properties.
+                for prop in node.model.properties.keys():
+                    if prop in n_data.keys():
+                        node.model.set_property(prop, n_data[prop])
+                # set custom properties.
+                for prop, val in n_data.get('custom', {}).items():
+                    node.model.set_property(prop, val)
+                    if isinstance(node, BaseNode):
+                        if prop in node.view.widgets:
+                            node.view.widgets[prop].set_value(val)
+
+                nodes[n_id] = node
+                self.add_node(node, n_data.get('pos'), push_undo=False)
+
+                if n_data.get('port_deletion_allowed', None):
+                    node.set_ports({
+                        'input_ports': n_data['input_ports'],
+                        'output_ports': n_data['output_ports']
+                    })
+
+        # build the connections.
+        for connection in data.get('connections', []):
+            nid, pname = connection.get('in', ('', ''))
+            in_node = nodes.get(nid) or self.get_node_by_id(nid)
+            if not in_node:
+                continue
+            in_port = in_node.inputs().get(pname) if in_node else None
+
+            nid, pname = connection.get('out', ('', ''))
+            out_node = nodes.get(nid) or self.get_node_by_id(nid)
+            if not out_node:
+                continue
+            out_port = out_node.outputs().get(pname) if out_node else None
+
+            if in_port and out_port:
+                # only connect if input port is not connected yet or input port
+                # can have multiple connections.
+                # important when duplicating nodes.
+                allow_connection = any([not in_port.model.connected_ports,
+                                        in_port.model.multi_connection])
+                if allow_connection:
+                    self._undo_stack.push(PortConnectedCmd(in_port, out_port))
+
+                # Run on_input_connected to ensure connections are fully set up after deserialization.
+                in_node.on_input_connected(in_port, out_port)
+
+        node_objs = nodes.values()
+        if relative_pos:
+            self._viewer.move_nodes([n.view for n in node_objs])
+            [setattr(n.model, 'pos', n.view.xy_pos) for n in node_objs]
+        elif pos:
+            self._viewer.move_nodes([n.view for n in node_objs], pos=pos)
+            [setattr(n.model, 'pos', n.view.xy_pos) for n in node_objs]
+
+        return node_objs
+
     def set_tooltip_default(self):
         """
         Set the default tooltip in all the nodes.
         """
         for node in self.all_nodes():
             node.set_tooltip_default()
```

### Comparing `electricalsim-0.0.7.0/src/electricalsim/lib/main_components.py` & `electricalsim-0.0.7.1/src/electricalsim/lib/main_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from Qt import QtCore, QtGui, QtWidgets
 
 import numpy as np
 
-from NodeGraphQt import BaseNode, BaseNodeCircle
+from NodeGraphQt import BaseNode
 from NodeGraphQt.widgets.node_widgets import NodeBaseWidget
 
 from lib.auxiliary import PropertyChangedCmd
 
 
 class QSpinBoxWrapper(NodeBaseWidget):
     """
@@ -138,25 +138,14 @@
     def __init__(self):
         super().__init__()
         
         extras = ('layout_vert',)
         for prop in extras:
             self.create_property(prop, False)
         
-        # layout_vert = self.get_property('layout_vert')
-        # if layout_vert is not None and layout_vert is True:
-        #     print('Vertical!!!')
-        #     self.set_layout_direction(1)
-        # elif layout_vert is not None and layout_vert is False:
-        #     self.set_layout_direction(0)
-        #     self.model.set_property('text_color', (255, 255, 255, 180))  # default color
-        # elif layout_vert is None:
-        #     print('Recién se crea layout_vert')
-        #     self.create_property('layout_vert', False)
-        
     def set_property(self, name, value, push_undo=True):
         """
         Set the value on the node custom property.
 
         Args:
             name (str): name of the property.
             value (object): property data (python built in types).
@@ -370,50 +359,14 @@
     def flip(self):
         """
         Flip the node (change input ports by output ports, and vice versa).
         
         THIS IS A VIRTUAL METHOD.
         """
         pass
-    
-
-class BaseNode2Circle(BaseNodeCircle):
-    def __init__(self):
-        super().__init__()
-        
-    def set_property(self, name, value, push_undo=True):
-        """
-        Set the value on the node custom property.
-
-        Args:
-            name (str): name of the property.
-            value (object): property data (python built in types).
-            push_undo (bool): register the command to the undo stack. (default: True)
-        """
-
-        # prevent signals from causing a infinite loop.
-        if self.get_property(name) == value:
-            return
-
-        if self.graph and name == 'name':
-            value = self.graph.get_unique_name(value)
-            self.NODE_NAME = value
-
-        if self.graph:
-            if push_undo:
-                undo_stack = self.graph.undo_stack()
-                undo_stack.push(PropertyChangedCmd(self, name, value))
-            else:
-                PropertyChangedCmd(self, name, value).redo()
-        else:
-            if hasattr(self.view, name):
-                setattr(self.view, name, value)
-            self.model.set_property(name, value)
-        
-        self.update()
 
 
 class BusNode(BaseNode2):
     __identifier__ = 'BusNode'
     NODE_NAME = 'BusNode'
     
     def __init__(self):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `electricalsim-0.0.7.0/src/electricalsim/lib/table_widget.py` & `electricalsim-0.0.7.1/src/electricalsim/lib/table_widget.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/about_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/aload_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/aload_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/asgen_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/asgen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/bus_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/bus_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/choose_bus_switch.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/choose_bus_switch.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/choose_generator_type.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/choose_generator_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/choose_line_type.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/choose_line_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/choose_load_type.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/choose_load_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/choose_transformer_type.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/choose_transformer_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/dcline_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/dcline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/dialogs.py` & `electricalsim-0.0.7.1/src/electricalsim/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/ext_grid_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/ext_grid_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/extension.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/extension.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/gen_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/gen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/impedance_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/impedance_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/line_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/line_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/load_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/load_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/main_window.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/main_window_backup.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/main_window_backup.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/motor_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/motor_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/network_settings_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/network_settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/pf_settings_widget.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/pf_settings_widget.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/power_flow_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/power_flow_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/settings_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/sgen_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/sgen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/shunt_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/shunt_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/stdline_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/stdline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/stdtransformer3w_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/stdtransformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/stdtransformer_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/stdtransformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/storage_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/storage_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/switch_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/switch_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/transformer3w_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/transformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/transformer_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/transformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/ward_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/ward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/src/electricalsim/ui/xward_dialog.ui` & `electricalsim-0.0.7.1/src/electricalsim/ui/xward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/LICENSE` & `electricalsim-0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/README_PyPI.md` & `electricalsim-0.0.7.1/README_PyPI.md`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.0/pyproject.toml` & `electricalsim-0.0.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "electricalsim"
-version = "0.0.7.0"
-author = "PhD Ariel S. Loyarte"
+version = "0.0.7.1"
+author = "Dr. Ing. Ariel S. Loyarte"
 authors = [
-  { name="PhD Ariel S. Loyarte", email="aloyarte@frsf.utn.edu.ar" },
+  { name="Dr. Ing. Ariel S. Loyarte", email="aloyarte@frsf.utn.edu.ar" },
 ]
 description = "Graphical user interface for simulating electrical networks based on the pandapower library"
 readme = "README_PyPI.md"
 requires-python = ">=3.8"
 dependencies = [
   "PySide2>=5.15",
   "Qt.py>=1.3.7",
```

### Comparing `electricalsim-0.0.7.0/PKG-INFO` & `electricalsim-0.0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: electricalsim
-Version: 0.0.7.0
+Version: 0.0.7.1
 Summary: Graphical user interface for simulating electrical networks based on the pandapower library
 Project-URL: Homepage, https://github.com/aloytag/electrical-grid-simulator
 Project-URL: Bug Tracker, https://github.com/aloytag/electrical-grid-simulator/issues
 Project-URL: Repository, https://github.com/aloytag/electrical-grid-simulator
-Author-email: "PhD Ariel S. Loyarte" <aloyarte@frsf.utn.edu.ar>
+Author-email: "Dr. Ing. Ariel S. Loyarte" <aloyarte@frsf.utn.edu.ar>
 License: MIT
 License-File: LICENSE
 Keywords: electrical networks,energy,power systems,simulation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

