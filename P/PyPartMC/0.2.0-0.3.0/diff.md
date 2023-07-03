# Comparing `tmp/PyPartMC-0.2.0.tar.gz` & `tmp/PyPartMC-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPartMC-0.2.0.tar", last modified: Wed Jun 14 17:11:15 2023, max compression
+gzip compressed data, was "PyPartMC-0.3.0.tar", last modified: Mon Jul  3 00:20:53 2023, max compression
```

## Comparing `PyPartMC-0.2.0.tar` & `PyPartMC-0.3.0.tar`

### file list

```diff
@@ -1,763 +1,931 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.793418 PyPartMC-0.2.0/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.430844 PyPartMC-0.2.0/.binder/
--rwxr-xr-x   0 runner     (501) staff       (20)       58 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.binder/postBuild
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.binder/requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.402376 PyPartMC-0.2.0/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.437341 PyPartMC-0.2.0/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)      283 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/cancel.yml
--rw-r--r--   0 runner     (501) staff       (20)      735 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/conda.yml
--rw-r--r--   0 runner     (501) staff       (20)      278 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/cpplint.yml
--rw-r--r--   0 runner     (501) staff       (20)      301 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/forlint.yml
--rw-r--r--   0 runner     (501) staff       (20)      831 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/pdoc.yml
--rw-r--r--   0 runner     (501) staff       (20)      414 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner     (501) staff       (20)      888 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/pylint.yml
--rw-r--r--   0 runner     (501) staff       (20)      778 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/readme_julia.yml
--rw-r--r--   0 runner     (501) staff       (20)      994 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/readme_matlab.yml
--rw-r--r--   0 runner     (501) staff       (20)      742 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/readme_python.yml
--rw-r--r--   0 runner     (501) staff       (20)      687 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/stale.yml
--rw-r--r--   0 runner     (501) staff       (20)     5008 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.github/workflows/tests+pypi.yml
--rw-r--r--   0 runner     (501) staff       (20)     1355 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.gitmodules
--rw-r--r--   0 runner     (501) staff       (20)      455 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner     (501) staff       (20)    12663 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    35149 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     3272 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     9203 2023-06-14 17:11:15.790246 PyPartMC-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.437822 PyPartMC-0.2.0/PyPartMC/
--rw-r--r--   0 runner     (501) staff       (20)     1372 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/PyPartMC/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.440758 PyPartMC-0.2.0/PyPartMC.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     9203 2023-06-14 17:11:15.000000 PyPartMC-0.2.0/PyPartMC.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    30090 2023-06-14 17:11:15.000000 PyPartMC-0.2.0/PyPartMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-14 17:11:15.000000 PyPartMC-0.2.0/PyPartMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-14 17:11:15.000000 PyPartMC-0.2.0/PyPartMC.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       57 2023-06-14 17:11:15.000000 PyPartMC-0.2.0/PyPartMC.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       19 2023-06-14 17:11:15.000000 PyPartMC-0.2.0/PyPartMC.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     8735 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.447641 PyPartMC-0.2.0/examples/
--rw-r--r--   0 runner     (501) staff       (20)     2071 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/examples/hello_world.ipynb
--rw-r--r--   0 runner     (501) staff       (20)    17290 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/examples/lognorm_ex.ipynb
--rw-r--r--   0 runner     (501) staff       (20)  1702898 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/examples/particle_simulation.ipynb
--rw-r--r--   0 runner     (501) staff       (20)    45392 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/examples/terminal_velocities.ipynb
--rw-r--r--   0 runner     (501) staff       (20)     6252 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/examples/widgets_playground.ipynb
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.415895 PyPartMC-0.2.0/gitmodules/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.406635 PyPartMC-0.2.0/gitmodules/SuiteSparse/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.404093 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.448686 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Include/
--rw-r--r--   0 runner     (501) staff       (20)    17821 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Include/amd.h
--rw-r--r--   0 runner     (501) staff       (20)     8238 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Include/amd_internal.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.456592 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/
--rw-r--r--   0 runner     (501) staff       (20)    52625 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd.f
--rw-r--r--   0 runner     (501) staff       (20)     5710 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_1.c
--rw-r--r--   0 runner     (501) staff       (20)    64825 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_2.c
--rw-r--r--   0 runner     (501) staff       (20)     4847 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_aat.c
--rw-r--r--   0 runner     (501) staff       (20)     1867 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_control.c
--rw-r--r--   0 runner     (501) staff       (20)     1253 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_defaults.c
--rw-r--r--   0 runner     (501) staff       (20)     5012 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_dump.c
--rw-r--r--   0 runner     (501) staff       (20)      837 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_global.c
--rw-r--r--   0 runner     (501) staff       (20)     4293 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_info.c
--rw-r--r--   0 runner     (501) staff       (20)     6031 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_order.c
--rw-r--r--   0 runner     (501) staff       (20)     3703 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_post_tree.c
--rw-r--r--   0 runner     (501) staff       (20)     5509 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_postorder.c
--rw-r--r--   0 runner     (501) staff       (20)     3808 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_preprocess.c
--rw-r--r--   0 runner     (501) staff       (20)     2980 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_valid.c
--rw-r--r--   0 runner     (501) staff       (20)    52282 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amdbar.f
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.404746 PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.457850 PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Include/
--rw-r--r--   0 runner     (501) staff       (20)    12382 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Include/btf.h
--rw-r--r--   0 runner     (501) staff       (20)     1427 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Include/btf_internal.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.459334 PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Source/
--rw-r--r--   0 runner     (501) staff       (20)    15950 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Source/btf_maxtrans.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Source/btf_order.c
--rw-r--r--   0 runner     (501) staff       (20)    24167 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Source/btf_strongcomp.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.405593 PyPartMC-0.2.0/gitmodules/SuiteSparse/COLAMD/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.459883 PyPartMC-0.2.0/gitmodules/SuiteSparse/COLAMD/Include/
--rw-r--r--   0 runner     (501) staff       (20)     8361 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/COLAMD/Include/colamd.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.460364 PyPartMC-0.2.0/gitmodules/SuiteSparse/COLAMD/Source/
--rw-r--r--   0 runner     (501) staff       (20)   107525 2023-06-14 17:10:15.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/COLAMD/Source/colamd.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.406375 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.462261 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Include/
--rw-r--r--   0 runner     (501) staff       (20)    29763 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Include/klu.h
--rw-r--r--   0 runner     (501) staff       (20)     6581 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Include/klu_internal.h
--rw-r--r--   0 runner     (501) staff       (20)    19461 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Include/klu_version.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.471456 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/
--rw-r--r--   0 runner     (501) staff       (20)    24701 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu.c
--rw-r--r--   0 runner     (501) staff       (20)    16732 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_analyze.c
--rw-r--r--   0 runner     (501) staff       (20)    11585 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_analyze_given.c
--rw-r--r--   0 runner     (501) staff       (20)     1923 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_defaults.c
--rw-r--r--   0 runner     (501) staff       (20)    16659 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_diagnostics.c
--rw-r--r--   0 runner     (501) staff       (20)     4560 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_dump.c
--rw-r--r--   0 runner     (501) staff       (20)     8011 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_extract.c
--rw-r--r--   0 runner     (501) staff       (20)    18700 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_factor.c
--rw-r--r--   0 runner     (501) staff       (20)     1992 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_free_numeric.c
--rw-r--r--   0 runner     (501) staff       (20)      982 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_free_symbolic.c
--rw-r--r--   0 runner     (501) staff       (20)    34162 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_kernel.c
--rw-r--r--   0 runner     (501) staff       (20)     7002 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_memory.c
--rw-r--r--   0 runner     (501) staff       (20)    17034 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_refactor.c
--rw-r--r--   0 runner     (501) staff       (20)     4627 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_scale.c
--rw-r--r--   0 runner     (501) staff       (20)    13209 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_solve.c
--rw-r--r--   0 runner     (501) staff       (20)     4261 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_sort.c
--rw-r--r--   0 runner     (501) staff       (20)    15641 2023-06-14 17:10:17.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_tsolve.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.472604 PyPartMC-0.2.0/gitmodules/SuiteSparse/SuiteSparse_config/
--rw-r--r--   0 runner     (501) staff       (20)    16453 2023-06-14 17:10:18.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c
--rw-r--r--   0 runner     (501) staff       (20)     7692 2023-06-14 17:10:18.000000 PyPartMC-0.2.0/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.407061 PyPartMC-0.2.0/gitmodules/camp/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.496934 PyPartMC-0.2.0/gitmodules/camp/src/
--rw-r--r--   0 runner     (501) staff       (20)     9605 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/Jacobian.c
--rw-r--r--   0 runner     (501) staff       (20)     5319 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/Jacobian.h
--rw-r--r--   0 runner     (501) staff       (20)    24549 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_phase_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     9949 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_phase_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     1311 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_phase_solver.h
--rw-r--r--   0 runner     (501) staff       (20)    29175 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_rep_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    14653 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_rep_factory.F90
--rw-r--r--   0 runner     (501) staff       (20)    23664 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_rep_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     2489 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_rep_solver.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.499179 PyPartMC-0.2.0/gitmodules/camp/src/aero_reps/
--rw-r--r--   0 runner     (501) staff       (20)    48515 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.F90
--rw-r--r--   0 runner     (501) staff       (20)    29575 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.c
--rw-r--r--   0 runner     (501) staff       (20)    27555 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_reps/aero_rep_single_particle.F90
--rw-r--r--   0 runner     (501) staff       (20)    18689 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_reps/aero_rep_single_particle.c
--rw-r--r--   0 runner     (501) staff       (20)     7067 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/aero_reps.h
--rw-r--r--   0 runner     (501) staff       (20)    11196 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/camp_common.h
--rw-r--r--   0 runner     (501) staff       (20)    67931 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/camp_core.F90
--rw-r--r--   0 runner     (501) staff       (20)     8991 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/camp_debug.h
--rw-r--r--   0 runner     (501) staff       (20)    71748 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/camp_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     3852 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/camp_solver.h
--rw-r--r--   0 runner     (501) staff       (20)    40570 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/camp_solver_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     5666 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/camp_state.F90
--rw-r--r--   0 runner     (501) staff       (20)    27287 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/chem_spec_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     3018 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/constants.F90
--rw-r--r--   0 runner     (501) staff       (20)     1076 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/debug_diff_check.F90
--rw-r--r--   0 runner     (501) staff       (20)    12725 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/debug_diff_check.c
--rw-r--r--   0 runner     (501) staff       (20)      722 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/debug_diff_check.h
--rw-r--r--   0 runner     (501) staff       (20)    14448 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/env_state.F90
--rw-r--r--   0 runner     (501) staff       (20)    14432 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/mechanism_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    53674 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/mpi.F90
--rw-r--r--   0 runner     (501) staff       (20)    28496 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/property.F90
--rw-r--r--   0 runner     (501) staff       (20)    18982 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rand.F90
--rw-r--r--   0 runner     (501) staff       (20)     4783 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rand_gsl.c
--rw-r--r--   0 runner     (501) staff       (20)    24830 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxn_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    18392 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxn_factory.F90
--rw-r--r--   0 runner     (501) staff       (20)    31580 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxn_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     1741 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxn_solver.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.515208 PyPartMC-0.2.0/gitmodules/camp/src/rxns/
--rw-r--r--   0 runner     (501) staff       (20)    10318 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.F90
--rw-r--r--   0 runner     (501) staff       (20)     8481 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.c
--rw-r--r--   0 runner     (501) staff       (20)    11012 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.F90
--rw-r--r--   0 runner     (501) staff       (20)     8771 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.c
--rw-r--r--   0 runner     (501) staff       (20)    18534 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.F90
--rw-r--r--   0 runner     (501) staff       (20)    21458 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.c
--rw-r--r--   0 runner     (501) staff       (20)    19588 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.F90
--rw-r--r--   0 runner     (501) staff       (20)    33890 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.c
--rw-r--r--   0 runner     (501) staff       (20)    19694 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.F90
--rw-r--r--   0 runner     (501) staff       (20)    23125 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.c
--rw-r--r--   0 runner     (501) staff       (20)    10732 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_arrhenius.F90
--rw-r--r--   0 runner     (501) staff       (20)     8214 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_arrhenius.c
--rw-r--r--   0 runner     (501) staff       (20)    19396 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.F90
--rw-r--r--   0 runner     (501) staff       (20)    17290 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.c
--rw-r--r--   0 runner     (501) staff       (20)    12259 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_emission.F90
--rw-r--r--   0 runner     (501) staff       (20)     7225 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_emission.c
--rw-r--r--   0 runner     (501) staff       (20)    12745 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_first_order_loss.F90
--rw-r--r--   0 runner     (501) staff       (20)     7978 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_first_order_loss.c
--rw-r--r--   0 runner     (501) staff       (20)    16156 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_photolysis.F90
--rw-r--r--   0 runner     (501) staff       (20)    10155 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_photolysis.c
--rw-r--r--   0 runner     (501) staff       (20)    11433 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.F90
--rw-r--r--   0 runner     (501) staff       (20)     9118 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.c
--rw-r--r--   0 runner     (501) staff       (20)    10906 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_troe.F90
--rw-r--r--   0 runner     (501) staff       (20)     8616 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_troe.c
--rw-r--r--   0 runner     (501) staff       (20)    12325 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.F90
--rw-r--r--   0 runner     (501) staff       (20)    10741 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.c
--rw-r--r--   0 runner     (501) staff       (20)     9518 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.F90
--rw-r--r--   0 runner     (501) staff       (20)     8366 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.c
--rw-r--r--   0 runner     (501) staff       (20)    14382 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wet_deposition.F90
--rw-r--r--   0 runner     (501) staff       (20)     8365 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wet_deposition.c
--rw-r--r--   0 runner     (501) staff       (20)    21601 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/rxns.h
--rw-r--r--   0 runner     (501) staff       (20)     5440 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/solver_stats.F90
--rw-r--r--   0 runner     (501) staff       (20)    21468 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_model_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     8903 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_model_factory.F90
--rw-r--r--   0 runner     (501) staff       (20)    20633 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_model_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     1390 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_model_solver.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.518845 PyPartMC-0.2.0/gitmodules/camp/src/sub_models/
--rw-r--r--   0 runner     (501) staff       (20)    35354 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_PDFiTE.F90
--rw-r--r--   0 runner     (501) staff       (20)    23405 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_PDFiTE.c
--rw-r--r--   0 runner     (501) staff       (20)    31875 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_UNIFAC.F90
--rw-r--r--   0 runner     (501) staff       (20)    34859 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_UNIFAC.c
--rw-r--r--   0 runner     (501) staff       (20)    29725 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.F90
--rw-r--r--   0 runner     (501) staff       (20)    22008 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.c
--rw-r--r--   0 runner     (501) staff       (20)     4665 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/sub_models.h
--rw-r--r--   0 runner     (501) staff       (20)     3081 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/time_derivative.c
--rw-r--r--   0 runner     (501) staff       (20)     2734 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/time_derivative.h
--rw-r--r--   0 runner     (501) staff       (20)    56058 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/util.F90
--rw-r--r--   0 runner     (501) staff       (20)     6750 2023-06-14 17:10:20.000000 PyPartMC-0.2.0/gitmodules/camp/src/util.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.409079 PyPartMC-0.2.0/gitmodules/json/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.409238 PyPartMC-0.2.0/gitmodules/json/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.555189 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/
--rw-r--r--   0 runner     (501) staff       (20)     2000 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/adl_serializer.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3183 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/byte_container_with_subtype.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.559907 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.561517 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/conversions/
--rw-r--r--   0 runner     (501) staff       (20)    18439 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/conversions/from_json.hpp
--rw-r--r--   0 runner     (501) staff       (20)    38114 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/conversions/to_chars.hpp
--rw-r--r--   0 runner     (501) staff       (20)    14612 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/conversions/to_json.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8820 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/exceptions.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3710 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/hash.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.566002 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/
--rw-r--r--   0 runner     (501) staff       (20)    95726 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/binary_reader.hpp
--rw-r--r--   0 runner     (501) staff       (20)    17017 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/input_adapters.hpp
--rw-r--r--   0 runner     (501) staff       (20)    20782 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/json_sax.hpp
--rw-r--r--   0 runner     (501) staff       (20)    54235 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/lexer.hpp
--rw-r--r--   0 runner     (501) staff       (20)    18415 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/parser.hpp
--rw-r--r--   0 runner     (501) staff       (20)      605 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/position_t.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.569235 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/
--rw-r--r--   0 runner     (501) staff       (20)      720 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/internal_iterator.hpp
--rw-r--r--   0 runner     (501) staff       (20)    23112 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/iter_impl.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5838 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/iteration_proxy.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1404 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/iterator_traits.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3509 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/json_reverse_iterator.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2918 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/primitive_iterator.hpp
--rw-r--r--   0 runner     (501) staff       (20)    32304 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/json_pointer.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1460 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/json_ref.hpp
--rw-r--r--   0 runner     (501) staff       (20)    41851 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/macro_scope.hpp
--rw-r--r--   0 runner     (501) staff       (20)      749 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/macro_unscope.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.572529 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.573772 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/call_std/
--rw-r--r--   0 runner     (501) staff       (20)      143 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/call_std/begin.hpp
--rw-r--r--   0 runner     (501) staff       (20)      142 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/call_std/end.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4609 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/cpp_future.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1800 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/detected.hpp
--rw-r--r--   0 runner     (501) staff       (20)      174 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/identity_tag.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6609 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/is_sax.hpp
--rw-r--r--   0 runner     (501) staff       (20)    22856 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/type_traits.hpp
--rw-r--r--   0 runner     (501) staff       (20)      244 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/void_t.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.576156 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/output/
--rw-r--r--   0 runner     (501) staff       (20)    69584 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/output/binary_writer.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3773 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/output/output_adapters.hpp
--rw-r--r--   0 runner     (501) staff       (20)    39511 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/output/serializer.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5697 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/string_concat.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1860 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/string_escape.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3098 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/value_t.hpp
--rw-r--r--   0 runner     (501) staff       (20)   186996 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/json.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2118 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/json_fwd.hpp
--rw-r--r--   0 runner     (501) staff       (20)     7469 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/ordered_map.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.411569 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/thirdparty/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.577513 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/thirdparty/hedley/
--rw-r--r--   0 runner     (501) staff       (20)    86041 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5205 2023-06-14 17:10:32.000000 PyPartMC-0.2.0/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.408181 PyPartMC-0.2.0/gitmodules/json-fortran/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.525331 PyPartMC-0.2.0/gitmodules/json-fortran/src/
--rw-r--r--   0 runner     (501) staff       (20)   121590 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_file_module.F90
--rw-r--r--   0 runner     (501) staff       (20)      842 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_get_scalar_by_path.inc
--rw-r--r--   0 runner     (501) staff       (20)      767 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_get_vec_by_path.inc
--rw-r--r--   0 runner     (501) staff       (20)     1264 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_get_vec_by_path_alloc.inc
--rw-r--r--   0 runner     (501) staff       (20)     4725 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_initialize_arguments.inc
--rw-r--r--   0 runner     (501) staff       (20)      499 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_initialize_dummy_arguments.inc
--rw-r--r--   0 runner     (501) staff       (20)     5759 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_kinds.F90
--rw-r--r--   0 runner     (501) staff       (20)     2480 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_macros.inc
--rw-r--r--   0 runner     (501) staff       (20)     4027 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_module.F90
--rw-r--r--   0 runner     (501) staff       (20)     9238 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_parameters.F90
--rw-r--r--   0 runner     (501) staff       (20)    31512 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_string_utilities.F90
--rw-r--r--   0 runner     (501) staff       (20)   456578 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/json_value_module.F90
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.551611 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.552227 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/introspection/
--rw-r--r--   0 runner     (501) staff       (20)     1194 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/introspection/test_iso_10646_support.f90
--rw-r--r--   0 runner     (501) staff       (20)    16922 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_01.F90
--rw-r--r--   0 runner     (501) staff       (20)    14591 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_02.F90
--rw-r--r--   0 runner     (501) staff       (20)     4824 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_03.F90
--rw-r--r--   0 runner     (501) staff       (20)     5454 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_04.F90
--rw-r--r--   0 runner     (501) staff       (20)     3597 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_05.F90
--rw-r--r--   0 runner     (501) staff       (20)     4648 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_06.F90
--rw-r--r--   0 runner     (501) staff       (20)     7880 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_07.F90
--rw-r--r--   0 runner     (501) staff       (20)     4903 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_08.F90
--rw-r--r--   0 runner     (501) staff       (20)     4843 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_09.F90
--rw-r--r--   0 runner     (501) staff       (20)    11909 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_10.F90
--rw-r--r--   0 runner     (501) staff       (20)     9207 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_11.F90
--rw-r--r--   0 runner     (501) staff       (20)     8710 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_12.F90
--rw-r--r--   0 runner     (501) staff       (20)     2173 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_13.F90
--rw-r--r--   0 runner     (501) staff       (20)     4981 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_14.F90
--rw-r--r--   0 runner     (501) staff       (20)     8746 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_15.F90
--rw-r--r--   0 runner     (501) staff       (20)     7282 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_16.F90
--rw-r--r--   0 runner     (501) staff       (20)     5649 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_17.F90
--rw-r--r--   0 runner     (501) staff       (20)     3614 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_18.F90
--rw-r--r--   0 runner     (501) staff       (20)     5793 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_19.F90
--rw-r--r--   0 runner     (501) staff       (20)     7724 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_20.F90
--rw-r--r--   0 runner     (501) staff       (20)     2620 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_21.F90
--rw-r--r--   0 runner     (501) staff       (20)     2648 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_22.F90
--rw-r--r--   0 runner     (501) staff       (20)     8627 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_23.F90
--rw-r--r--   0 runner     (501) staff       (20)     6317 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_24.F90
--rw-r--r--   0 runner     (501) staff       (20)     4863 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_25.F90
--rw-r--r--   0 runner     (501) staff       (20)     2645 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_26.F90
--rw-r--r--   0 runner     (501) staff       (20)     2569 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_27.F90
--rw-r--r--   0 runner     (501) staff       (20)     3824 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_28.F90
--rw-r--r--   0 runner     (501) staff       (20)     5889 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_29.F90
--rw-r--r--   0 runner     (501) staff       (20)     2342 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_30.F90
--rw-r--r--   0 runner     (501) staff       (20)     4697 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_31.F90
--rw-r--r--   0 runner     (501) staff       (20)     3853 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_32.F90
--rw-r--r--   0 runner     (501) staff       (20)     3607 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_33.F90
--rw-r--r--   0 runner     (501) staff       (20)     5045 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_34.F90
--rw-r--r--   0 runner     (501) staff       (20)     3079 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_35.F90
--rw-r--r--   0 runner     (501) staff       (20)     4194 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_36.F90
--rw-r--r--   0 runner     (501) staff       (20)     3650 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_37.F90
--rw-r--r--   0 runner     (501) staff       (20)     4150 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_38.F90
--rw-r--r--   0 runner     (501) staff       (20)     2407 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_39.F90
--rw-r--r--   0 runner     (501) staff       (20)     1803 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_40.F90
--rw-r--r--   0 runner     (501) staff       (20)     3928 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_41.F90
--rw-r--r--   0 runner     (501) staff       (20)     4079 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_42.F90
--rw-r--r--   0 runner     (501) staff       (20)     2687 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_43.F90
--rw-r--r--   0 runner     (501) staff       (20)     3060 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_44.F90
--rw-r--r--   0 runner     (501) staff       (20)     4378 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_45.F90
--rw-r--r--   0 runner     (501) staff       (20)    12438 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_46.F90
--rw-r--r--   0 runner     (501) staff       (20)     4331 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_47.F90
--rw-r--r--   0 runner     (501) staff       (20)     2691 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_48.F90
--rw-r--r--   0 runner     (501) staff       (20)     1976 2023-06-14 17:10:34.000000 PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_49.F90
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.412001 PyPartMC-0.2.0/gitmodules/partmc/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.616186 PyPartMC-0.2.0/gitmodules/partmc/src/
--rw-r--r--   0 runner     (501) staff       (20)    18941 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_binned.F90
--rw-r--r--   0 runner     (501) staff       (20)    37336 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    17040 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_dist.F90
--rw-r--r--   0 runner     (501) staff       (20)     4584 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_info.F90
--rw-r--r--   0 runner     (501) staff       (20)     9722 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_info_array.F90
--rw-r--r--   0 runner     (501) staff       (20)    49450 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_mode.F90
--rw-r--r--   0 runner     (501) staff       (20)    36702 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_particle.F90
--rw-r--r--   0 runner     (501) staff       (20)    10615 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_particle_array.F90
--rw-r--r--   0 runner     (501) staff       (20)    23922 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_sorted.F90
--rw-r--r--   0 runner     (501) staff       (20)   124072 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_state.F90
--rw-r--r--   0 runner     (501) staff       (20)    13932 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_weight.F90
--rw-r--r--   0 runner     (501) staff       (20)    27073 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/aero_weight_array.F90
--rw-r--r--   0 runner     (501) staff       (20)     2924 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/bin_average_comp.F90
--rw-r--r--   0 runner     (501) staff       (20)     3825 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/bin_average_size.F90
--rw-r--r--   0 runner     (501) staff       (20)    20694 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/bin_grid.F90
--rw-r--r--   0 runner     (501) staff       (20)     7275 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/camp_interface.F90
--rw-r--r--   0 runner     (501) staff       (20)     8917 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/chamber.F90
--rw-r--r--   0 runner     (501) staff       (20)    19523 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel.F90
--rw-r--r--   0 runner     (501) staff       (20)    11888 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_additive.F90
--rw-r--r--   0 runner     (501) staff       (20)     7285 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_brown.F90
--rw-r--r--   0 runner     (501) staff       (20)     4941 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_brown_cont.F90
--rw-r--r--   0 runner     (501) staff       (20)     5034 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_brown_free.F90
--rw-r--r--   0 runner     (501) staff       (20)     4927 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_constant.F90
--rw-r--r--   0 runner     (501) staff       (20)    11071 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_sedi.F90
--rw-r--r--   0 runner     (501) staff       (20)     7469 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_zero.F90
--rw-r--r--   0 runner     (501) staff       (20)    35666 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coagulation.F90
--rw-r--r--   0 runner     (501) staff       (20)    34136 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/coagulation_dist.F90
--rw-r--r--   0 runner     (501) staff       (20)    30924 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/condense.F90
--rw-r--r--   0 runner     (501) staff       (20)     8820 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/condense_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     2913 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/constants.F90
--rw-r--r--   0 runner     (501) staff       (20)    20205 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/env_state.F90
--rw-r--r--   0 runner     (501) staff       (20)     4419 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/exact_soln.F90
--rw-r--r--   0 runner     (501) staff       (20)     3949 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/extract_aero_particles.F90
--rw-r--r--   0 runner     (501) staff       (20)     6528 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/extract_aero_size.F90
--rw-r--r--   0 runner     (501) staff       (20)     5072 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/extract_aero_time.F90
--rw-r--r--   0 runner     (501) staff       (20)     4227 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/extract_env.F90
--rw-r--r--   0 runner     (501) staff       (20)     3867 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/extract_gas.F90
--rw-r--r--   0 runner     (501) staff       (20)     5692 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/extract_sectional_aero_size.F90
--rw-r--r--   0 runner     (501) staff       (20)     4858 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/extract_sectional_aero_time.F90
--rw-r--r--   0 runner     (501) staff       (20)    23458 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/fractal.F90
--rw-r--r--   0 runner     (501) staff       (20)    16247 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/gas_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    22073 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/gas_state.F90
--rw-r--r--   0 runner     (501) staff       (20)     7566 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/getopt.F90
--rw-r--r--   0 runner     (501) staff       (20)    15007 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/integer_rmap.F90
--rw-r--r--   0 runner     (501) staff       (20)    19200 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/integer_rmap2.F90
--rw-r--r--   0 runner     (501) staff       (20)     8378 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/integer_varray.F90
--rw-r--r--   0 runner     (501) staff       (20)    18380 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/mosaic.F90
--rw-r--r--   0 runner     (501) staff       (20)    47083 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/mpi.F90
--rw-r--r--   0 runner     (501) staff       (20)    27550 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/netcdf.F90
--rw-r--r--   0 runner     (501) staff       (20)     8579 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/nucleate.F90
--rw-r--r--   0 runner     (501) staff       (20)     7062 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/numeric_average.F90
--rw-r--r--   0 runner     (501) staff       (20)    10911 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/numeric_diff.F90
--rw-r--r--   0 runner     (501) staff       (20)    30038 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/output.F90
--rw-r--r--   0 runner     (501) staff       (20)    48249 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/partmc.F90
--rw-r--r--   0 runner     (501) staff       (20)     8459 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/photolysis.F90
--rw-r--r--   0 runner     (501) staff       (20)    18343 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/rand.F90
--rw-r--r--   0 runner     (501) staff       (20)     4712 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/rand_gsl.c
--rw-r--r--   0 runner     (501) staff       (20)     2837 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/run_exact.F90
--rw-r--r--   0 runner     (501) staff       (20)    32432 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/run_part.F90
--rw-r--r--   0 runner     (501) staff       (20)    12069 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/run_sect.F90
--rw-r--r--   0 runner     (501) staff       (20)    47571 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/scenario.F90
--rw-r--r--   0 runner     (501) staff       (20)     1563 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/sort.c
--rw-r--r--   0 runner     (501) staff       (20)    23797 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/spec_file.F90
--rw-r--r--   0 runner     (501) staff       (20)     3063 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/spec_line.F90
--rw-r--r--   0 runner     (501) staff       (20)    23957 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/stats.F90
--rw-r--r--   0 runner     (501) staff       (20)    49470 2023-06-14 17:10:36.000000 PyPartMC-0.2.0/gitmodules/partmc/src/util.F90
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.616809 PyPartMC-0.2.0/gitmodules/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    10999 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.412686 PyPartMC-0.2.0/gitmodules/pybind11/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.630078 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    23883 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner     (501) staff       (20)     7069 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner     (501) staff       (20)    65224 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner     (501) staff       (20)     8458 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner     (501) staff       (20)      120 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner     (501) staff       (20)     2096 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.634355 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner     (501) staff       (20)    28078 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner     (501) staff       (20)    49007 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner     (501) staff       (20)     5491 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner     (501) staff       (20)    17971 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner     (501) staff       (20)    23981 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner     (501) staff       (20)    44230 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner     (501) staff       (20)     1513 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner     (501) staff       (20)    31685 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner     (501) staff       (20)    10728 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner     (501) staff       (20)     4731 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner     (501) staff       (20)     4658 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner     (501) staff       (20)     6923 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner     (501) staff       (20)     8851 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner     (501) staff       (20)    78946 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner     (501) staff       (20)     9051 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner     (501) staff       (20)     2181 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner     (501) staff       (20)   125304 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner     (501) staff       (20)    80981 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.634845 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner     (501) staff       (20)     4185 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner     (501) staff       (20)    14535 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner     (501) staff       (20)    27013 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.636357 PyPartMC-0.2.0/gitmodules/pybind11/tools/
--rw-r--r--   0 runner     (501) staff       (20)    10455 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner     (501) staff       (20)    13460 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner     (501) staff       (20)     7270 2023-06-14 17:10:38.000000 PyPartMC-0.2.0/gitmodules/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.414019 PyPartMC-0.2.0/gitmodules/pybind11_json/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.414201 PyPartMC-0.2.0/gitmodules/pybind11_json/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.636836 PyPartMC-0.2.0/gitmodules/pybind11_json/include/pybind11_json/
--rw-r--r--   0 runner     (501) staff       (20)     7219 2023-06-14 17:10:39.000000 PyPartMC-0.2.0/gitmodules/pybind11_json/include/pybind11_json/pybind11_json.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.414637 PyPartMC-0.2.0/gitmodules/span/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.414801 PyPartMC-0.2.0/gitmodules/span/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.637315 PyPartMC-0.2.0/gitmodules/span/include/tcb/
--rw-r--r--   0 runner     (501) staff       (20)    18165 2023-06-14 17:10:40.000000 PyPartMC-0.2.0/gitmodules/span/include/tcb/span.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.415235 PyPartMC-0.2.0/gitmodules/string_view-standalone/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.415395 PyPartMC-0.2.0/gitmodules/string_view-standalone/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.637836 PyPartMC-0.2.0/gitmodules/string_view-standalone/include/bpstd/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.638428 PyPartMC-0.2.0/gitmodules/string_view-standalone/include/bpstd/detail/
--rw-r--r--   0 runner     (501) staff       (20)    29304 2023-06-14 17:10:40.000000 PyPartMC-0.2.0/gitmodules/string_view-standalone/include/bpstd/detail/string_view.inl
--rw-r--r--   0 runner     (501) staff       (20)    20256 2023-06-14 17:10:40.000000 PyPartMC-0.2.0/gitmodules/string_view-standalone/include/bpstd/string_view.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.418159 PyPartMC-0.2.0/gitmodules/sundials/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.639928 PyPartMC-0.2.0/gitmodules/sundials/cmake/
--rw-r--r--   0 runner     (501) staff       (20)     2962 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/cmake/SundialsIndexSize.cmake
--rw-r--r--   0 runner     (501) staff       (20)    10395 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/cmake/SundialsSetupCompilers.cmake
--rw-r--r--   0 runner     (501) staff       (20)     4883 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/cmake/SundialsSetupConfig.cmake
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.417912 PyPartMC-0.2.0/gitmodules/sundials/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.644511 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/
--rw-r--r--   0 runner     (501) staff       (20)     9544 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode.h
--rw-r--r--   0 runner     (501) staff       (20)     1525 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_bandpre.h
--rw-r--r--   0 runner     (501) staff       (20)     2182 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_bbdpre.h
--rw-r--r--   0 runner     (501) staff       (20)     1790 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_diag.h
--rw-r--r--   0 runner     (501) staff       (20)     2035 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_direct.h
--rw-r--r--   0 runner     (501) staff       (20)    10422 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_hypamgpre.h
--rw-r--r--   0 runner     (501) staff       (20)     6515 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_ls.h
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_proj.h
--rw-r--r--   0 runner     (501) staff       (20)     2873 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_spils.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.652007 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/
--rw-r--r--   0 runner     (501) staff       (20)     9721 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_cuda.h
--rw-r--r--   0 runner     (501) staff       (20)     9653 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_hip.h
--rw-r--r--   0 runner     (501) staff       (20)     8671 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_manyvector.h
--rw-r--r--   0 runner     (501) staff       (20)     9959 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_mpimanyvector.h
--rw-r--r--   0 runner     (501) staff       (20)     1644 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_mpiplusx.h
--rw-r--r--   0 runner     (501) staff       (20)     9487 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_openmp.h
--rw-r--r--   0 runner     (501) staff       (20)     9612 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_openmpdev.h
--rw-r--r--   0 runner     (501) staff       (20)    10795 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_parallel.h
--rw-r--r--   0 runner     (501) staff       (20)     9697 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_parhyp.h
--rw-r--r--   0 runner     (501) staff       (20)     9419 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_petsc.h
--rw-r--r--   0 runner     (501) staff       (20)    11042 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_pthreads.h
--rw-r--r--   0 runner     (501) staff       (20)     8267 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_raja.h
--rw-r--r--   0 runner     (501) staff       (20)     8934 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_serial.h
--rw-r--r--   0 runner     (501) staff       (20)    10053 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_sycl.h
--rw-r--r--   0 runner     (501) staff       (20)     5824 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_trilinos.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.652969 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/trilinos/
--rw-r--r--   0 runner     (501) staff       (20)     1819 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorInterface.hpp
--rw-r--r--   0 runner     (501) staff       (20)    23964 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorKernels.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.664642 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/
--rw-r--r--   0 runner     (501) staff       (20)     7791 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_band.h
--rw-r--r--   0 runner     (501) staff       (20)     5329 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_config.in
--rw-r--r--   0 runner     (501) staff       (20)     5520 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_cuda_policies.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8997 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_dense.h
--rw-r--r--   0 runner     (501) staff       (20)    13330 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_direct.h
--rw-r--r--   0 runner     (501) staff       (20)     1690 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_fconfig.in
--rw-r--r--   0 runner     (501) staff       (20)     1123 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_fnvector.h
--rw-r--r--   0 runner     (501) staff       (20)     1128 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_futils.h
--rw-r--r--   0 runner     (501) staff       (20)     5478 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_hip_policies.hpp
--rw-r--r--   0 runner     (501) staff       (20)    10283 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_iterative.h
--rw-r--r--   0 runner     (501) staff       (20)    10707 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_lapack.h
--rw-r--r--   0 runner     (501) staff       (20)     9633 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_linearsolver.h
--rw-r--r--   0 runner     (501) staff       (20)     7839 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_math.h
--rw-r--r--   0 runner     (501) staff       (20)     5466 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_matrix.h
--rw-r--r--   0 runner     (501) staff       (20)     4527 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_memory.h
--rw-r--r--   0 runner     (501) staff       (20)     1399 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_mpi_types.h
--rw-r--r--   0 runner     (501) staff       (20)     9190 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_nonlinearsolver.h
--rw-r--r--   0 runner     (501) staff       (20)    12719 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_nvector.h
--rw-r--r--   0 runner     (501) staff       (20)     4744 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_nvector_senswrapper.h
--rw-r--r--   0 runner     (501) staff       (20)     4567 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_sycl_policies.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5165 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_types.h
--rw-r--r--   0 runner     (501) staff       (20)     1266 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_version.h
--rw-r--r--   0 runner     (501) staff       (20)     4024 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_xbraid.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.671864 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/
--rw-r--r--   0 runner     (501) staff       (20)     2649 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_band.h
--rw-r--r--   0 runner     (501) staff       (20)     4768 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_cusolversp_batchqr.h
--rw-r--r--   0 runner     (501) staff       (20)     2983 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_dense.h
--rw-r--r--   0 runner     (501) staff       (20)     5603 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_klu.h
--rw-r--r--   0 runner     (501) staff       (20)     3142 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackband.h
--rw-r--r--   0 runner     (501) staff       (20)     3171 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackdense.h
--rw-r--r--   0 runner     (501) staff       (20)     2751 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_magmadense.h
--rw-r--r--   0 runner     (501) staff       (20)     3052 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_onemkldense.h
--rw-r--r--   0 runner     (501) staff       (20)     4553 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_pcg.h
--rw-r--r--   0 runner     (501) staff       (20)     4872 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spbcgs.h
--rw-r--r--   0 runner     (501) staff       (20)     5330 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spfgmr.h
--rw-r--r--   0 runner     (501) staff       (20)     5237 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spgmr.h
--rw-r--r--   0 runner     (501) staff       (20)     4959 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_sptfqmr.h
--rw-r--r--   0 runner     (501) staff       (20)     5621 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_superludist.h
--rw-r--r--   0 runner     (501) staff       (20)     4533 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_superlumt.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.675344 PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/
--rw-r--r--   0 runner     (501) staff       (20)     4552 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_band.h
--rw-r--r--   0 runner     (501) staff       (20)     5233 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_cusparse.h
--rw-r--r--   0 runner     (501) staff       (20)     3647 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_dense.h
--rw-r--r--   0 runner     (501) staff       (20)     5083 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_magmadense.h
--rw-r--r--   0 runner     (501) staff       (20)     5776 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_onemkldense.h
--rw-r--r--   0 runner     (501) staff       (20)     3245 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_slunrloc.h
--rw-r--r--   0 runner     (501) staff       (20)     5136 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_sparse.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.676812 PyPartMC-0.2.0/gitmodules/sundials/include/sunnonlinsol/
--rw-r--r--   0 runner     (501) staff       (20)     6202 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_fixedpoint.h
--rw-r--r--   0 runner     (501) staff       (20)     5449 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_newton.h
--rw-r--r--   0 runner     (501) staff       (20)     4071 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_petscsnes.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.424325 PyPartMC-0.2.0/gitmodules/sundials/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.689884 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/
--rw-r--r--   0 runner     (501) staff       (20)     1972 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/CHANGES
--rw-r--r--   0 runner     (501) staff       (20)     3549 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1576 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     1166 2023-06-14 17:10:53.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/NOTICE
--rw-r--r--   0 runner     (501) staff       (20)     2708 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/README.md
--rw-r--r--   0 runner     (501) staff       (20)   135753 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode.c
--rw-r--r--   0 runner     (501) staff       (20)    18212 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_bandpre.c
--rw-r--r--   0 runner     (501) staff       (20)     2383 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_bandpre_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    22668 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_bbdpre.c
--rw-r--r--   0 runner     (501) staff       (20)     2621 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_bbdpre_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    13629 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_diag.c
--rw-r--r--   0 runner     (501) staff       (20)     2240 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_diag_impl.h
--rw-r--r--   0 runner     (501) staff       (20)     1956 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_direct.c
--rw-r--r--   0 runner     (501) staff       (20)    14722 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_fused_gpu.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5554 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_fused_stubs.c
--rw-r--r--   0 runner     (501) staff       (20)    14959 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_hypamgpre.c
--rw-r--r--   0 runner     (501) staff       (20)     2766 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_hypamgpre_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    29404 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    28172 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_io.c
--rw-r--r--   0 runner     (501) staff       (20)    58312 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_ls.c
--rw-r--r--   0 runner     (501) staff       (20)     8077 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_ls_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    12911 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_nls.c
--rw-r--r--   0 runner     (501) staff       (20)    12603 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_proj.c
--rw-r--r--   0 runner     (501) staff       (20)     3079 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_proj_impl.h
--rw-r--r--   0 runner     (501) staff       (20)     2943 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_spils.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.699401 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/
--rw-r--r--   0 runner     (501) staff       (20)     1734 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     4616 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/Makefile.in
--rw-r--r--   0 runner     (501) staff       (20)     3464 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvband.c
--rw-r--r--   0 runner     (501) staff       (20)     4950 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvbbd.c
--rw-r--r--   0 runner     (501) staff       (20)    22548 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvbbd.h
--rw-r--r--   0 runner     (501) staff       (20)     2063 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvbp.c
--rw-r--r--   0 runner     (501) staff       (20)    14934 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvbp.h
--rw-r--r--   0 runner     (501) staff       (20)     2952 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvdense.c
--rw-r--r--   0 runner     (501) staff       (20)     2046 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvewt.c
--rw-r--r--   0 runner     (501) staff       (20)     3904 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvjtimes.c
--rw-r--r--   0 runner     (501) staff       (20)     1370 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvnulllinsol.c
--rw-r--r--   0 runner     (501) staff       (20)     1344 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvnullmatrix.c
--rw-r--r--   0 runner     (501) staff       (20)     1502 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvnullnonlinsol.c
--rw-r--r--   0 runner     (501) staff       (20)    15564 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvode.c
--rw-r--r--   0 runner     (501) staff       (20)    49120 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvode.h
--rw-r--r--   0 runner     (501) staff       (20)     4190 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvpreco.c
--rw-r--r--   0 runner     (501) staff       (20)     2399 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvroot.c
--rw-r--r--   0 runner     (501) staff       (20)     4974 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvroot.h
--rw-r--r--   0 runner     (501) staff       (20)     2921 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvsparse.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.700976 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1483 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    43017 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fmod/fcvode_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    83166 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fmod/fcvode_mod.f90
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.701645 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/
--rw-r--r--   0 runner     (501) staff       (20)     1562 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.703512 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/
--rw-r--r--   0 runner     (501) staff       (20)     1648 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.705062 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fmod/
--rw-r--r--   0 runner     (501) staff       (20)      979 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    25549 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    40279 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     3740 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fnvector_serial.c
--rw-r--r--   0 runner     (501) staff       (20)     2693 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fnvector_serial.h
--rw-r--r--   0 runner     (501) staff       (20)    47581 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/nvector_serial.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.715693 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/
--rw-r--r--   0 runner     (501) staff       (20)     3022 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.722622 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1109 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     7228 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.c
--rw-r--r--   0 runner     (501) staff       (20)     2922 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)    13682 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    19932 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     9392 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.c
--rw-r--r--   0 runner     (501) staff       (20)     9541 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)    11515 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    12797 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)    24749 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    42038 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     6561 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.c
--rw-r--r--   0 runner     (501) staff       (20)      957 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     6784 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_band.c
--rw-r--r--   0 runner     (501) staff       (20)     3712 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_cuda.h
--rw-r--r--   0 runner     (501) staff       (20)     7056 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_cuda_kernels.cuh
--rw-r--r--   0 runner     (501) staff       (20)     1403 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_debug.h
--rw-r--r--   0 runner     (501) staff       (20)     9098 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_dense.c
--rw-r--r--   0 runner     (501) staff       (20)     6468 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_direct.c
--rw-r--r--   0 runner     (501) staff       (20)      964 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_futils.c
--rw-r--r--   0 runner     (501) staff       (20)     2500 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_hip.h
--rw-r--r--   0 runner     (501) staff       (20)     7260 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_hip_kernels.hip.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8008 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_iterative.c
--rw-r--r--   0 runner     (501) staff       (20)     5667 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_linearsolver.c
--rw-r--r--   0 runner     (501) staff       (20)     2956 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_math.c
--rw-r--r--   0 runner     (501) staff       (20)     4633 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_matrix.c
--rw-r--r--   0 runner     (501) staff       (20)     4810 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_memory.c
--rw-r--r--   0 runner     (501) staff       (20)     6479 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_nonlinearsolver.c
--rw-r--r--   0 runner     (501) staff       (20)    20704 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_nvector.c
--rw-r--r--   0 runner     (501) staff       (20)    13469 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_nvector_senswrapper.c
--rw-r--r--   0 runner     (501) staff       (20)     3051 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_sycl.h
--rw-r--r--   0 runner     (501) staff       (20)     1592 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_version.c
--rw-r--r--   0 runner     (501) staff       (20)     6371 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_xbraid.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.723110 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/
--rw-r--r--   0 runner     (501) staff       (20)     1481 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.725218 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/
--rw-r--r--   0 runner     (501) staff       (20)     1798 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.726724 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1085 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     9961 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.c
--rw-r--r--   0 runner     (501) staff       (20)     7950 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     2963 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.c
--rw-r--r--   0 runner     (501) staff       (20)     1892 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.h
--rw-r--r--   0 runner     (501) staff       (20)     7118 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/sunlinsol_band.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.728692 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/
--rw-r--r--   0 runner     (501) staff       (20)     1844 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.730247 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1091 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     9982 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.c
--rw-r--r--   0 runner     (501) staff       (20)     8001 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     2978 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.c
--rw-r--r--   0 runner     (501) staff       (20)     1930 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.h
--rw-r--r--   0 runner     (501) staff       (20)     6580 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/sunlinsol_dense.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.732282 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/
--rw-r--r--   0 runner     (501) staff       (20)     1796 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.733795 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1053 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    13106 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    13874 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     4522 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.c
--rw-r--r--   0 runner     (501) staff       (20)     3046 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.h
--rw-r--r--   0 runner     (501) staff       (20)    13160 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/sunlinsol_klu.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.734751 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/pcg/
--rw-r--r--   0 runner     (501) staff       (20)     1709 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/pcg/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    16843 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/pcg/sunlinsol_pcg.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.735900 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spbcgs/
--rw-r--r--   0 runner     (501) staff       (20)     1743 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spbcgs/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    22722 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spbcgs/sunlinsol_spbcgs.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.736980 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spfgmr/
--rw-r--r--   0 runner     (501) staff       (20)     1700 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spfgmr/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    25504 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spfgmr/sunlinsol_spfgmr.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.738086 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spgmr/
--rw-r--r--   0 runner     (501) staff       (20)     1687 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spgmr/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    26697 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spgmr/sunlinsol_spgmr.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.739110 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/sptfqmr/
--rw-r--r--   0 runner     (501) staff       (20)     1713 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/sptfqmr/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    28426 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/sptfqmr/sunlinsol_sptfqmr.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.739694 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/
--rw-r--r--   0 runner     (501) staff       (20)     1085 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.740689 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/band/
--rw-r--r--   0 runner     (501) staff       (20)     1691 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/band/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    13124 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/band/sunmatrix_band.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.741689 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/dense/
--rw-r--r--   0 runner     (501) staff       (20)     1742 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/dense/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     8906 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/dense/sunmatrix_dense.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.742661 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/sparse/
--rw-r--r--   0 runner     (501) staff       (20)     1760 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/sparse/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    34432 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/sparse/sunmatrix_sparse.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.743288 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/
--rw-r--r--   0 runner     (501) staff       (20)      842 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.745258 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/
--rw-r--r--   0 runner     (501) staff       (20)     1855 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.747031 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1064 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    12989 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    13798 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     2718 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.c
--rw-r--r--   0 runner     (501) staff       (20)     2126 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.h
--rw-r--r--   0 runner     (501) staff       (20)    23849 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/sunnonlinsol_fixedpoint.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.749304 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/
--rw-r--r--   0 runner     (501) staff       (20)     1801 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.750952 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1039 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    13234 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    14015 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     2672 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.c
--rw-r--r--   0 runner     (501) staff       (20)     2051 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.h
--rw-r--r--   0 runner     (501) staff       (20)    16132 2023-06-14 17:10:54.000000 PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/sunnonlinsol_newton.c
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-06-14 17:11:15.793624 PyPartMC-0.2.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     6723 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.778006 PyPartMC-0.2.0/src/
--rw-r--r--   0 runner     (501) staff       (20)     5588 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     5798 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_data.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2474 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_dist.F90
--rw-r--r--   0 runner     (501) staff       (20)     2299 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_dist.hpp
--rw-r--r--   0 runner     (501) staff       (20)     7465 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_mode.F90
--rw-r--r--   0 runner     (501) staff       (20)     7830 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_mode.hpp
--rw-r--r--   0 runner     (501) staff       (20)    14256 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_particle.F90
--rw-r--r--   0 runner     (501) staff       (20)     9957 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_particle.hpp
--rw-r--r--   0 runner     (501) staff       (20)     9208 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_state.F90
--rw-r--r--   0 runner     (501) staff       (20)     8850 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/aero_state.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4355 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/bin_grid.F90
--rw-r--r--   0 runner     (501) staff       (20)     1984 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/bin_grid.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3337 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/bin_grid.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1104 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/camp_core.F90
--rw-r--r--   0 runner     (501) staff       (20)      802 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/camp_core.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2152 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/condense.F90
--rw-r--r--   0 runner     (501) staff       (20)     1073 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/condense.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1108 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/condense.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4224 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/env_state.F90
--rw-r--r--   0 runner     (501) staff       (20)     3676 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/env_state.hpp
--rw-r--r--   0 runner     (501) staff       (20)     7255 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/fake_netcdf.F90
--rw-r--r--   0 runner     (501) staff       (20)     2206 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/fake_netcdf.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9942 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/fake_spec_file.F90
--rw-r--r--   0 runner     (501) staff       (20)     6791 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/fake_spec_file.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2228 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/gas_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     2406 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/gas_data.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3220 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/gas_state.F90
--rw-r--r--   0 runner     (501) staff       (20)     4086 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/gas_state.hpp
--rw-r--r--   0 runner     (501) staff       (20)      695 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/gimmicks.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9002 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/gimmicks.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1070 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/photolysis.F90
--rw-r--r--   0 runner     (501) staff       (20)      810 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/photolysis.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1127 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/pmc_resource.hpp
--rw-r--r--   0 runner     (501) staff       (20)    20580 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/pypartmc.cpp
--rw-r--r--   0 runner     (501) staff       (20)      944 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/rand.F90
--rw-r--r--   0 runner     (501) staff       (20)      720 2023-06-14 17:09:55.000000 PyPartMC-0.2.0/src/rand.cpp
--rw-r--r--   0 runner     (501) staff       (20)      729 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/rand.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8174 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/run_part.F90
--rw-r--r--   0 runner     (501) staff       (20)     2647 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/run_part.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2400 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/run_part.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5679 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/run_part_opt.F90
--rw-r--r--   0 runner     (501) staff       (20)     1592 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/run_part_opt.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6950 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/scenario.F90
--rw-r--r--   0 runner     (501) staff       (20)     1189 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/scenario.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5931 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/scenario.hpp
--rw-r--r--   0 runner     (501) staff       (20)      782 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/sys.F90
--rw-r--r--   0 runner     (501) staff       (20)      711 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/sys.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1373 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/util.F90
--rw-r--r--   0 runner     (501) staff       (20)      988 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/util.cpp
--rw-r--r--   0 runner     (501) staff       (20)      971 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/src/util.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 17:11:15.789490 PyPartMC-0.2.0/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       47 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/conftest.py
--rw-r--r--   0 runner     (501) staff       (20)    10474 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_aero_data.py
--rw-r--r--   0 runner     (501) staff       (20)     4304 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_aero_dist.py
--rw-r--r--   0 runner     (501) staff       (20)     6501 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_aero_mode.py
--rw-r--r--   0 runner     (501) staff       (20)    15729 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_aero_particle.py
--rw-r--r--   0 runner     (501) staff       (20)     7255 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_aero_state.py
--rw-r--r--   0 runner     (501) staff       (20)     5955 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_bin_grid.py
--rw-r--r--   0 runner     (501) staff       (20)     2426 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_condense.py
--rw-r--r--   0 runner     (501) staff       (20)     1745 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_dtors.py
--rw-r--r--   0 runner     (501) staff       (20)     2366 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_env_state.py
--rw-r--r--   0 runner     (501) staff       (20)     1622 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_gas_data.py
--rw-r--r--   0 runner     (501) staff       (20)     3225 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_gas_state.py
--rw-r--r--   0 runner     (501) staff       (20)     2847 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_loss_rate.py
--rw-r--r--   0 runner     (501) staff       (20)     1027 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_rand.py
--rw-r--r--   0 runner     (501) staff       (20)     1999 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_run_part.py
--rw-r--r--   0 runner     (501) staff       (20)     2058 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_run_part_opt.py
--rw-r--r--   0 runner     (501) staff       (20)     8656 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_scenario.py
--rw-r--r--   0 runner     (501) staff       (20)      644 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_units.py
--rw-r--r--   0 runner     (501) staff       (20)     1624 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_util.py
--rw-r--r--   0 runner     (501) staff       (20)      580 2023-06-14 17:09:56.000000 PyPartMC-0.2.0/tests/test_version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.753481 PyPartMC-0.3.0/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.241914 PyPartMC-0.3.0/.binder/
+-rwxr-xr-x   0 runner     (501) staff       (20)       58 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.binder/postBuild
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.binder/requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.200015 PyPartMC-0.3.0/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.248515 PyPartMC-0.3.0/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)      283 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/cancel.yml
+-rw-r--r--   0 runner     (501) staff       (20)      735 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/conda.yml
+-rw-r--r--   0 runner     (501) staff       (20)      278 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/cpplint.yml
+-rw-r--r--   0 runner     (501) staff       (20)      301 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/forlint.yml
+-rw-r--r--   0 runner     (501) staff       (20)      831 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/pdoc.yml
+-rw-r--r--   0 runner     (501) staff       (20)      414 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner     (501) staff       (20)      903 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner     (501) staff       (20)      778 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/readme_julia.yml
+-rw-r--r--   0 runner     (501) staff       (20)      994 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/readme_matlab.yml
+-rw-r--r--   0 runner     (501) staff       (20)      742 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/readme_python.yml
+-rw-r--r--   0 runner     (501) staff       (20)      687 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/stale.yml
+-rw-r--r--   0 runner     (501) staff       (20)     4723 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.github/workflows/tests+pypi.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1623 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.gitmodules
+-rw-r--r--   0 runner     (501) staff       (20)      455 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    18207 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    11188 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    10831 2023-07-03 00:20:53.752840 PyPartMC-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.249184 PyPartMC-0.3.0/PyPartMC/
+-rw-r--r--   0 runner     (501) staff       (20)     1372 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/PyPartMC/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.255011 PyPartMC-0.3.0/PyPartMC.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    10831 2023-07-03 00:20:53.000000 PyPartMC-0.3.0/PyPartMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    36818 2023-07-03 00:20:53.000000 PyPartMC-0.3.0/PyPartMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-03 00:20:53.000000 PyPartMC-0.3.0/PyPartMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-03 00:20:53.000000 PyPartMC-0.3.0/PyPartMC.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       57 2023-07-03 00:20:53.000000 PyPartMC-0.3.0/PyPartMC.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       19 2023-07-03 00:20:53.000000 PyPartMC-0.3.0/PyPartMC.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)    10363 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.263788 PyPartMC-0.3.0/examples/
+-rw-r--r--   0 runner     (501) staff       (20)     2071 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/examples/hello_world.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)    17290 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/examples/lognorm_ex.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)  1702898 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/examples/particle_simulation.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)    31389 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/examples/process_simulation_output.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)    45392 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/examples/terminal_velocities.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)     6252 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/examples/widgets_playground.ipynb
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.221130 PyPartMC-0.3.0/gitmodules/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.264323 PyPartMC-0.3.0/gitmodules/SuiteSparse/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.201972 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.265796 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Include/
+-rw-r--r--   0 runner     (501) staff       (20)    17821 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Include/amd.h
+-rw-r--r--   0 runner     (501) staff       (20)     8238 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Include/amd_internal.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.278830 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/
+-rw-r--r--   0 runner     (501) staff       (20)    52625 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd.f
+-rw-r--r--   0 runner     (501) staff       (20)     5710 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_1.c
+-rw-r--r--   0 runner     (501) staff       (20)    64825 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_2.c
+-rw-r--r--   0 runner     (501) staff       (20)     4847 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_aat.c
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_control.c
+-rw-r--r--   0 runner     (501) staff       (20)     1253 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_defaults.c
+-rw-r--r--   0 runner     (501) staff       (20)     5012 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_dump.c
+-rw-r--r--   0 runner     (501) staff       (20)      837 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_global.c
+-rw-r--r--   0 runner     (501) staff       (20)     4293 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_info.c
+-rw-r--r--   0 runner     (501) staff       (20)     6031 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_order.c
+-rw-r--r--   0 runner     (501) staff       (20)     3703 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_post_tree.c
+-rw-r--r--   0 runner     (501) staff       (20)     5509 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_postorder.c
+-rw-r--r--   0 runner     (501) staff       (20)     3808 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_preprocess.c
+-rw-r--r--   0 runner     (501) staff       (20)     2980 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_valid.c
+-rw-r--r--   0 runner     (501) staff       (20)    52282 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amdbar.f
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.202646 PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.280174 PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Include/
+-rw-r--r--   0 runner     (501) staff       (20)    12382 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Include/btf.h
+-rw-r--r--   0 runner     (501) staff       (20)     1427 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Include/btf_internal.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.282106 PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Source/
+-rw-r--r--   0 runner     (501) staff       (20)    15950 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Source/btf_maxtrans.c
+-rw-r--r--   0 runner     (501) staff       (20)     5073 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Source/btf_order.c
+-rw-r--r--   0 runner     (501) staff       (20)    24167 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Source/btf_strongcomp.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.203414 PyPartMC-0.3.0/gitmodules/SuiteSparse/COLAMD/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.282769 PyPartMC-0.3.0/gitmodules/SuiteSparse/COLAMD/Include/
+-rw-r--r--   0 runner     (501) staff       (20)     8361 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/COLAMD/Include/colamd.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.283455 PyPartMC-0.3.0/gitmodules/SuiteSparse/COLAMD/Source/
+-rw-r--r--   0 runner     (501) staff       (20)   107525 2023-07-03 00:19:27.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/COLAMD/Source/colamd.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.204087 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.285683 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Include/
+-rw-r--r--   0 runner     (501) staff       (20)    29763 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Include/klu.h
+-rw-r--r--   0 runner     (501) staff       (20)     6581 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Include/klu_internal.h
+-rw-r--r--   0 runner     (501) staff       (20)    19461 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Include/klu_version.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.296444 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/
+-rw-r--r--   0 runner     (501) staff       (20)    24701 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu.c
+-rw-r--r--   0 runner     (501) staff       (20)    16732 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_analyze.c
+-rw-r--r--   0 runner     (501) staff       (20)    11585 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_analyze_given.c
+-rw-r--r--   0 runner     (501) staff       (20)     1923 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_defaults.c
+-rw-r--r--   0 runner     (501) staff       (20)    16659 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_diagnostics.c
+-rw-r--r--   0 runner     (501) staff       (20)     4560 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_dump.c
+-rw-r--r--   0 runner     (501) staff       (20)     8011 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_extract.c
+-rw-r--r--   0 runner     (501) staff       (20)    18700 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_factor.c
+-rw-r--r--   0 runner     (501) staff       (20)     1992 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_free_numeric.c
+-rw-r--r--   0 runner     (501) staff       (20)      982 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_free_symbolic.c
+-rw-r--r--   0 runner     (501) staff       (20)    34162 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_kernel.c
+-rw-r--r--   0 runner     (501) staff       (20)     7002 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_memory.c
+-rw-r--r--   0 runner     (501) staff       (20)    17034 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_refactor.c
+-rw-r--r--   0 runner     (501) staff       (20)     4627 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_scale.c
+-rw-r--r--   0 runner     (501) staff       (20)    13209 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_solve.c
+-rw-r--r--   0 runner     (501) staff       (20)     4261 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_sort.c
+-rw-r--r--   0 runner     (501) staff       (20)    15641 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_tsolve.c
+-rw-r--r--   0 runner     (501) staff       (20)    51560 2023-07-03 00:19:29.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/LICENSE.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.297816 PyPartMC-0.3.0/gitmodules/SuiteSparse/SuiteSparse_config/
+-rw-r--r--   0 runner     (501) staff       (20)    16453 2023-07-03 00:19:30.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c
+-rw-r--r--   0 runner     (501) staff       (20)     7692 2023-07-03 00:19:30.000000 PyPartMC-0.3.0/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.298513 PyPartMC-0.3.0/gitmodules/camp/
+-rw-r--r--   0 runner     (501) staff       (20)     1122 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/COPYING
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.329831 PyPartMC-0.3.0/gitmodules/camp/src/
+-rw-r--r--   0 runner     (501) staff       (20)     9605 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/Jacobian.c
+-rw-r--r--   0 runner     (501) staff       (20)     5319 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/Jacobian.h
+-rw-r--r--   0 runner     (501) staff       (20)    24549 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_phase_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9949 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_phase_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     1311 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_phase_solver.h
+-rw-r--r--   0 runner     (501) staff       (20)    29175 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_rep_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    14653 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_rep_factory.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23664 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_rep_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     2489 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_rep_solver.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.332784 PyPartMC-0.3.0/gitmodules/camp/src/aero_reps/
+-rw-r--r--   0 runner     (501) staff       (20)    48515 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.F90
+-rw-r--r--   0 runner     (501) staff       (20)    29575 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.c
+-rw-r--r--   0 runner     (501) staff       (20)    27555 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_reps/aero_rep_single_particle.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18689 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_reps/aero_rep_single_particle.c
+-rw-r--r--   0 runner     (501) staff       (20)     7067 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/aero_reps.h
+-rw-r--r--   0 runner     (501) staff       (20)    11196 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/camp_common.h
+-rw-r--r--   0 runner     (501) staff       (20)    67931 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/camp_core.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8991 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/camp_debug.h
+-rw-r--r--   0 runner     (501) staff       (20)    71748 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/camp_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     3852 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/camp_solver.h
+-rw-r--r--   0 runner     (501) staff       (20)    40570 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/camp_solver_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5666 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/camp_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)    27287 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/chem_spec_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3018 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/constants.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1076 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/debug_diff_check.F90
+-rw-r--r--   0 runner     (501) staff       (20)    12725 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/debug_diff_check.c
+-rw-r--r--   0 runner     (501) staff       (20)      722 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/debug_diff_check.h
+-rw-r--r--   0 runner     (501) staff       (20)    14448 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/env_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)    14432 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/mechanism_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    53674 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/mpi.F90
+-rw-r--r--   0 runner     (501) staff       (20)    28496 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/property.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18982 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rand.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4783 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rand_gsl.c
+-rw-r--r--   0 runner     (501) staff       (20)    24830 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxn_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18392 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxn_factory.F90
+-rw-r--r--   0 runner     (501) staff       (20)    31580 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxn_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     1741 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxn_solver.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.352783 PyPartMC-0.3.0/gitmodules/camp/src/rxns/
+-rw-r--r--   0 runner     (501) staff       (20)    10318 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8481 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.c
+-rw-r--r--   0 runner     (501) staff       (20)    11012 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8771 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.c
+-rw-r--r--   0 runner     (501) staff       (20)    18534 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.F90
+-rw-r--r--   0 runner     (501) staff       (20)    21458 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.c
+-rw-r--r--   0 runner     (501) staff       (20)    19588 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.F90
+-rw-r--r--   0 runner     (501) staff       (20)    33890 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.c
+-rw-r--r--   0 runner     (501) staff       (20)    19694 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23125 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.c
+-rw-r--r--   0 runner     (501) staff       (20)    10732 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_arrhenius.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8214 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_arrhenius.c
+-rw-r--r--   0 runner     (501) staff       (20)    19396 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.F90
+-rw-r--r--   0 runner     (501) staff       (20)    17290 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.c
+-rw-r--r--   0 runner     (501) staff       (20)    12259 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_emission.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7225 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_emission.c
+-rw-r--r--   0 runner     (501) staff       (20)    12745 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_first_order_loss.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7978 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_first_order_loss.c
+-rw-r--r--   0 runner     (501) staff       (20)    16156 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_photolysis.F90
+-rw-r--r--   0 runner     (501) staff       (20)    10155 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_photolysis.c
+-rw-r--r--   0 runner     (501) staff       (20)    11433 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9118 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.c
+-rw-r--r--   0 runner     (501) staff       (20)    10906 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_troe.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8616 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_troe.c
+-rw-r--r--   0 runner     (501) staff       (20)    12325 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.F90
+-rw-r--r--   0 runner     (501) staff       (20)    10741 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.c
+-rw-r--r--   0 runner     (501) staff       (20)     9518 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8366 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.c
+-rw-r--r--   0 runner     (501) staff       (20)    14382 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wet_deposition.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8365 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wet_deposition.c
+-rw-r--r--   0 runner     (501) staff       (20)    21601 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/rxns.h
+-rw-r--r--   0 runner     (501) staff       (20)     5440 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/solver_stats.F90
+-rw-r--r--   0 runner     (501) staff       (20)    21468 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_model_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8903 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_model_factory.F90
+-rw-r--r--   0 runner     (501) staff       (20)    20633 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_model_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     1390 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_model_solver.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.357015 PyPartMC-0.3.0/gitmodules/camp/src/sub_models/
+-rw-r--r--   0 runner     (501) staff       (20)    35354 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_PDFiTE.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23405 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_PDFiTE.c
+-rw-r--r--   0 runner     (501) staff       (20)    31875 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_UNIFAC.F90
+-rw-r--r--   0 runner     (501) staff       (20)    34859 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_UNIFAC.c
+-rw-r--r--   0 runner     (501) staff       (20)    29725 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.F90
+-rw-r--r--   0 runner     (501) staff       (20)    22008 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.c
+-rw-r--r--   0 runner     (501) staff       (20)     4665 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/sub_models.h
+-rw-r--r--   0 runner     (501) staff       (20)     3081 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/time_derivative.c
+-rw-r--r--   0 runner     (501) staff       (20)     2734 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/time_derivative.h
+-rw-r--r--   0 runner     (501) staff       (20)    56058 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/util.F90
+-rw-r--r--   0 runner     (501) staff       (20)     6750 2023-07-03 00:19:33.000000 PyPartMC-0.3.0/gitmodules/camp/src/util.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.358037 PyPartMC-0.3.0/gitmodules/json/
+-rw-r--r--   0 runner     (501) staff       (20)     1076 2023-07-03 00:19:50.000000 PyPartMC-0.3.0/gitmodules/json/LICENSE.MIT
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.207389 PyPartMC-0.3.0/gitmodules/json/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.399564 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/
+-rw-r--r--   0 runner     (501) staff       (20)     2000 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/adl_serializer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3183 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/byte_container_with_subtype.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.404747 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.406507 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/conversions/
+-rw-r--r--   0 runner     (501) staff       (20)    18439 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/conversions/from_json.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    38114 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/conversions/to_chars.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    14612 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/conversions/to_json.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8820 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/exceptions.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3710 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/hash.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.410761 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/
+-rw-r--r--   0 runner     (501) staff       (20)    95726 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/binary_reader.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    17017 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/input_adapters.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    20782 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/json_sax.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    54235 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/lexer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    18415 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/parser.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      605 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/position_t.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.414246 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/
+-rw-r--r--   0 runner     (501) staff       (20)      720 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/internal_iterator.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    23112 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/iter_impl.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5838 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/iteration_proxy.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1404 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/iterator_traits.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3509 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/json_reverse_iterator.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2918 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/primitive_iterator.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    32304 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/json_pointer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1460 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/json_ref.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    41851 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/macro_scope.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      749 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/macro_unscope.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.418033 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.419155 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/call_std/
+-rw-r--r--   0 runner     (501) staff       (20)      143 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/call_std/begin.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      142 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/call_std/end.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4609 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/cpp_future.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1800 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/detected.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      174 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/identity_tag.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     6609 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/is_sax.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    22856 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/type_traits.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      244 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/void_t.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.421208 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/output/
+-rw-r--r--   0 runner     (501) staff       (20)    69584 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/output/binary_writer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3773 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/output/output_adapters.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    39511 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/output/serializer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5697 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/string_concat.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1860 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/string_escape.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3098 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/value_t.hpp
+-rw-r--r--   0 runner     (501) staff       (20)   186996 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/json.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2118 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/json_fwd.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     7469 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/ordered_map.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.211682 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/thirdparty/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.422575 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/thirdparty/hedley/
+-rw-r--r--   0 runner     (501) staff       (20)    86041 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5205 2023-07-03 00:19:51.000000 PyPartMC-0.3.0/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.358729 PyPartMC-0.3.0/gitmodules/json-fortran/
+-rw-r--r--   0 runner     (501) staff       (20)     2849 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.366948 PyPartMC-0.3.0/gitmodules/json-fortran/src/
+-rw-r--r--   0 runner     (501) staff       (20)   121590 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_file_module.F90
+-rw-r--r--   0 runner     (501) staff       (20)      842 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_get_scalar_by_path.inc
+-rw-r--r--   0 runner     (501) staff       (20)      767 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_get_vec_by_path.inc
+-rw-r--r--   0 runner     (501) staff       (20)     1264 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_get_vec_by_path_alloc.inc
+-rw-r--r--   0 runner     (501) staff       (20)     4725 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_initialize_arguments.inc
+-rw-r--r--   0 runner     (501) staff       (20)      499 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_initialize_dummy_arguments.inc
+-rw-r--r--   0 runner     (501) staff       (20)     5759 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_kinds.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2480 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_macros.inc
+-rw-r--r--   0 runner     (501) staff       (20)     4027 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_module.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9238 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_parameters.F90
+-rw-r--r--   0 runner     (501) staff       (20)    31512 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_string_utilities.F90
+-rw-r--r--   0 runner     (501) staff       (20)   456578 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/json_value_module.F90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.395408 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.395931 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/introspection/
+-rw-r--r--   0 runner     (501) staff       (20)     1194 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/introspection/test_iso_10646_support.f90
+-rw-r--r--   0 runner     (501) staff       (20)    16922 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_01.F90
+-rw-r--r--   0 runner     (501) staff       (20)    14591 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_02.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4824 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_03.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5454 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_04.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3597 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_05.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4648 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_06.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7880 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_07.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4903 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_08.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4843 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_09.F90
+-rw-r--r--   0 runner     (501) staff       (20)    11909 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_10.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9207 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_11.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8710 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_12.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2173 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_13.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4981 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_14.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8746 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_15.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7282 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_16.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5649 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_17.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3614 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_18.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5793 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_19.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7724 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_20.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2620 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_21.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2648 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_22.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8627 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_23.F90
+-rw-r--r--   0 runner     (501) staff       (20)     6317 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_24.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4863 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_25.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2645 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_26.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2569 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_27.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3824 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_28.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5889 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_29.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2342 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_30.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4697 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_31.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3853 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_32.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3607 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_33.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5045 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_34.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3079 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_35.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4194 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_36.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_37.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4150 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_38.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2407 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_39.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1803 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_40.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3928 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_41.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4079 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_42.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2687 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_43.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3060 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_44.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4378 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_45.F90
+-rw-r--r--   0 runner     (501) staff       (20)    12438 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_46.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4331 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_47.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2691 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_48.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1976 2023-07-03 00:19:53.000000 PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_49.F90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.424599 PyPartMC-0.3.0/gitmodules/netcdf-c/
+-rw-r--r--   0 runner     (501) staff       (20)    90875 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1452 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/COPYRIGHT
+-rw-r--r--   0 runner     (501) staff       (20)    18999 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/config.h.cmake.in
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.444292 PyPartMC-0.3.0/gitmodules/netcdf-c/include/
+-rw-r--r--   0 runner     (501) staff       (20)      643 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/fbits.h
+-rw-r--r--   0 runner     (501) staff       (20)     4907 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nc.h
+-rw-r--r--   0 runner     (501) staff       (20)     5614 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nc3dispatch.h
+-rw-r--r--   0 runner     (501) staff       (20)     8982 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nc3internal.h
+-rw-r--r--   0 runner     (501) staff       (20)     6820 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nc4dispatch.h
+-rw-r--r--   0 runner     (501) staff       (20)    23203 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nc4internal.h
+-rw-r--r--   0 runner     (501) staff       (20)     1659 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nc_logging.h
+-rw-r--r--   0 runner     (501) staff       (20)     2621 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nc_provenance.h
+-rw-r--r--   0 runner     (501) staff       (20)     2062 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncauth.h
+-rw-r--r--   0 runner     (501) staff       (20)     2261 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncbytes.h
+-rw-r--r--   0 runner     (501) staff       (20)     3295 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncconfigure.h
+-rw-r--r--   0 runner     (501) staff       (20)      410 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nccrc.h
+-rw-r--r--   0 runner     (501) staff       (20)     7474 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncdispatch.h
+-rw-r--r--   0 runner     (501) staff       (20)      674 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncexternl.h
+-rw-r--r--   0 runner     (501) staff       (20)     3607 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nchashmap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1906 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nchttp.h
+-rw-r--r--   0 runner     (501) staff       (20)     3226 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncindex.h
+-rw-r--r--   0 runner     (501) staff       (20)     2254 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nclist.h
+-rw-r--r--   0 runner     (501) staff       (20)     1851 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/nclog.h
+-rw-r--r--   0 runner     (501) staff       (20)     1086 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncmodel.h
+-rw-r--r--   0 runner     (501) staff       (20)     2215 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncoffsets.h
+-rw-r--r--   0 runner     (501) staff       (20)     8248 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncpathmgr.h
+-rw-r--r--   0 runner     (501) staff       (20)     3396 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncrc.h
+-rw-r--r--   0 runner     (501) staff       (20)     2079 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncs3sdk.h
+-rw-r--r--   0 runner     (501) staff       (20)     4264 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncuri.h
+-rw-r--r--   0 runner     (501) staff       (20)     1420 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncutf8.h
+-rw-r--r--   0 runner     (501) staff       (20)     1210 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/ncxml.h
+-rw-r--r--   0 runner     (501) staff       (20)    73732 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/netcdf.h
+-rw-r--r--   0 runner     (501) staff       (20)     4090 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/netcdf_aux.h
+-rw-r--r--   0 runner     (501) staff       (20)    13091 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/netcdf_dispatch.h.in
+-rw-r--r--   0 runner     (501) staff       (20)     1606 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/netcdf_f.h
+-rw-r--r--   0 runner     (501) staff       (20)     4065 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/netcdf_filter.h
+-rw-r--r--   0 runner     (501) staff       (20)     1337 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/netcdf_mem.h
+-rw-r--r--   0 runner     (501) staff       (20)     3835 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/netcdf_meta.h.in
+-rw-r--r--   0 runner     (501) staff       (20)     1971 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/onstack.h
+-rw-r--r--   0 runner     (501) staff       (20)      569 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/include/rnd.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.472022 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/
+-rw-r--r--   0 runner     (501) staff       (20)     6128 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/datt.c
+-rw-r--r--   0 runner     (501) staff       (20)    23572 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dattget.c
+-rw-r--r--   0 runner     (501) staff       (20)    13788 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dattinq.c
+-rw-r--r--   0 runner     (501) staff       (20)    21685 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dattput.c
+-rw-r--r--   0 runner     (501) staff       (20)    12111 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dauth.c
+-rw-r--r--   0 runner     (501) staff       (20)    27254 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/daux.c
+-rw-r--r--   0 runner     (501) staff       (20)    14827 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dcompound.c
+-rw-r--r--   0 runner     (501) staff       (20)    21188 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dcopy.c
+-rw-r--r--   0 runner     (501) staff       (20)    10910 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dcrc64.c
+-rw-r--r--   0 runner     (501) staff       (20)    16745 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/ddim.c
+-rw-r--r--   0 runner     (501) staff       (20)     3272 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/ddispatch.c
+-rw-r--r--   0 runner     (501) staff       (20)     5448 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/denum.c
+-rw-r--r--   0 runner     (501) staff       (20)    10328 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/derror.c
+-rw-r--r--   0 runner     (501) staff       (20)    75413 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dfile.c
+-rw-r--r--   0 runner     (501) staff       (20)    16459 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dfilter.c
+-rw-r--r--   0 runner     (501) staff       (20)     9601 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dgroup.c
+-rw-r--r--   0 runner     (501) staff       (20)    43874 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dinfermodel.c
+-rw-r--r--   0 runner     (501) staff       (20)    16008 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dinstance.c
+-rw-r--r--   0 runner     (501) staff       (20)    19387 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dinstance_intern.c
+-rw-r--r--   0 runner     (501) staff       (20)     6562 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dmissing.c
+-rw-r--r--   0 runner     (501) staff       (20)    15177 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dnotnc4.c
+-rw-r--r--   0 runner     (501) staff       (20)    11901 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/doffsets.c
+-rw-r--r--   0 runner     (501) staff       (20)     2170 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dopaque.c
+-rw-r--r--   0 runner     (501) staff       (20)    32961 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dpathmgr.c
+-rw-r--r--   0 runner     (501) staff       (20)    32946 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/drc.c
+-rw-r--r--   0 runner     (501) staff       (20)     9341 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/ds3util.c
+-rw-r--r--   0 runner     (501) staff       (20)     7588 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dstring.c
+-rw-r--r--   0 runner     (501) staff       (20)     5453 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dtype.c
+-rw-r--r--   0 runner     (501) staff       (20)     4527 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dutf8.c
+-rw-r--r--   0 runner     (501) staff       (20)    10862 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dutil.c
+-rw-r--r--   0 runner     (501) staff       (20)    52386 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dvar.c
+-rw-r--r--   0 runner     (501) staff       (20)    41839 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dvarget.c
+-rw-r--r--   0 runner     (501) staff       (20)    22318 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dvarinq.c
+-rw-r--r--   0 runner     (501) staff       (20)    38016 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dvarput.c
+-rw-r--r--   0 runner     (501) staff       (20)     5687 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/dvlen.c
+-rw-r--r--   0 runner     (501) staff       (20)     4039 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/nc.c
+-rw-r--r--   0 runner     (501) staff       (20)     4595 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/ncbytes.c
+-rw-r--r--   0 runner     (501) staff       (20)   149230 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/nchashmap.c
+-rw-r--r--   0 runner     (501) staff       (20)     6328 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/nclist.c
+-rw-r--r--   0 runner     (501) staff       (20)     6507 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/nclistmgr.c
+-rw-r--r--   0 runner     (501) staff       (20)     7281 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/nclog.c
+-rw-r--r--   0 runner     (501) staff       (20)    34144 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/ncuri.c
+-rw-r--r--   0 runner     (501) staff       (20)    30569 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/utf8proc.c
+-rw-r--r--   0 runner     (501) staff       (20)    29211 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/utf8proc.h
+-rw-r--r--   0 runner     (501) staff       (20)  1621941 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libdispatch/utf8proc_data.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.476461 PyPartMC-0.3.0/gitmodules/netcdf-c/liblib/
+-rw-r--r--   0 runner     (501) staff       (20)     4004 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/liblib/nc_initialize.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.485080 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/
+-rw-r--r--   0 runner     (501) staff       (20)    22640 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/attr.m4
+-rw-r--r--   0 runner     (501) staff       (20)    10107 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/dim.c
+-rw-r--r--   0 runner     (501) staff       (20)    20016 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/memio.c
+-rw-r--r--   0 runner     (501) staff       (20)    12218 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/nc3dispatch.c
+-rw-r--r--   0 runner     (501) staff       (20)    42563 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/nc3internal.c
+-rw-r--r--   0 runner     (501) staff       (20)     5804 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/ncio.c
+-rw-r--r--   0 runner     (501) staff       (20)     4986 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/ncio.h
+-rw-r--r--   0 runner     (501) staff       (20)    38570 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/ncx.h
+-rw-r--r--   0 runner     (501) staff       (20)    91027 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/ncx.m4
+-rw-r--r--   0 runner     (501) staff       (20)    45195 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/posixio.c
+-rw-r--r--   0 runner     (501) staff       (20)    56656 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/putget.m4
+-rw-r--r--   0 runner     (501) staff       (20)    34650 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/v1hpg.c
+-rw-r--r--   0 runner     (501) staff       (20)    17812 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc/var.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.489085 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc4/
+-rw-r--r--   0 runner     (501) staff       (20)     6166 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc4/nc4cache.c
+-rw-r--r--   0 runner     (501) staff       (20)     1933 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc4/nc4dispatch.c
+-rw-r--r--   0 runner     (501) staff       (20)    12192 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc4/nc4grp.c
+-rw-r--r--   0 runner     (501) staff       (20)    60959 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc4/nc4internal.c
+-rw-r--r--   0 runner     (501) staff       (20)    22718 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc4/nc4type.c
+-rw-r--r--   0 runner     (501) staff       (20)    62575 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc4/nc4var.c
+-rw-r--r--   0 runner     (501) staff       (20)    10546 2023-07-03 00:20:01.000000 PyPartMC-0.3.0/gitmodules/netcdf-c/libsrc4/ncindex.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.489746 PyPartMC-0.3.0/gitmodules/netcdf-fortran/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.490310 PyPartMC-0.3.0/gitmodules/netcdf-fortran/CMakeExtras/
+-rw-r--r--   0 runner     (501) staff       (20)     2443 2023-07-03 00:20:02.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/CMakeExtras/MatchNetCDFFortranTypes.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     2417 2023-07-03 00:20:02.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/COPYRIGHT
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.512710 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/
+-rwxr-xr-x   0 runner     (501) staff       (20)    35483 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/module_netcdf4_nc_interfaces.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    33291 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/module_netcdf4_nf_interfaces.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    17109 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_data.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    80960 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_interfaces.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    15589 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_data.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    56443 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_interfaces.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2732 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf4.F90
+-rw-r--r--   0 runner     (501) staff       (20)    38904 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf4_eightbyte.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1899 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf4_externals.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5233 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf4_file.F90
+-rw-r--r--   0 runner     (501) staff       (20)    33491 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf4_func.F90
+-rw-r--r--   0 runner     (501) staff       (20)      789 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf4_overloads.F90
+-rw-r--r--   0 runner     (501) staff       (20)    16715 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf4_variables.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf4_visibility.F90
+-rw-r--r--   0 runner     (501) staff       (20)    16718 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_attributes.F90
+-rw-r--r--   0 runner     (501) staff       (20)    11047 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_constants.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1719 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_dims.F90
+-rw-r--r--   0 runner     (501) staff       (20)   124466 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_expanded.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3537 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_externals.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5101 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_file.F90
+-rw-r--r--   0 runner     (501) staff       (20)     6806 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_overloads.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23015 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_text_variables.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3802 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_variables.F90
+-rw-r--r--   0 runner     (501) staff       (20)      959 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/netcdf_visibility.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    20393 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_attio.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    16094 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_control.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)     6572 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_dim.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)     8623 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_genatt.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)     5086 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_geninq.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    10775 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_genvar.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)     7909 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_lib.c
+-rwxr-xr-x   0 runner     (501) staff       (20)     4428 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_misc.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    58343 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_nc4.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_nc_noparallel.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    23742 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_var1io.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    31119 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_varaio.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    38708 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_varmio.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    37941 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/nf_varsio.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2601 2023-07-03 00:20:03.000000 PyPartMC-0.3.0/gitmodules/netcdf-fortran/fortran/typeSizes.F90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.513170 PyPartMC-0.3.0/gitmodules/partmc/
+-rw-r--r--   0 runner     (501) staff       (20)    18015 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/COPYING
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.552390 PyPartMC-0.3.0/gitmodules/partmc/src/
+-rw-r--r--   0 runner     (501) staff       (20)    18941 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_binned.F90
+-rw-r--r--   0 runner     (501) staff       (20)    37336 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    17040 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_dist.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4584 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_info.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9722 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_info_array.F90
+-rw-r--r--   0 runner     (501) staff       (20)    49450 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_mode.F90
+-rw-r--r--   0 runner     (501) staff       (20)    36702 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_particle.F90
+-rw-r--r--   0 runner     (501) staff       (20)    10615 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_particle_array.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23922 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_sorted.F90
+-rw-r--r--   0 runner     (501) staff       (20)   124072 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)    13932 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_weight.F90
+-rw-r--r--   0 runner     (501) staff       (20)    27073 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/aero_weight_array.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2924 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/bin_average_comp.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3825 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/bin_average_size.F90
+-rw-r--r--   0 runner     (501) staff       (20)    20694 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/bin_grid.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7275 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/camp_interface.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8917 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/chamber.F90
+-rw-r--r--   0 runner     (501) staff       (20)    19523 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel.F90
+-rw-r--r--   0 runner     (501) staff       (20)    11888 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_additive.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7285 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_brown.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4941 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_brown_cont.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5034 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_brown_free.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4927 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_constant.F90
+-rw-r--r--   0 runner     (501) staff       (20)    11071 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_sedi.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7469 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_zero.F90
+-rw-r--r--   0 runner     (501) staff       (20)    35666 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coagulation.F90
+-rw-r--r--   0 runner     (501) staff       (20)    34136 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/coagulation_dist.F90
+-rw-r--r--   0 runner     (501) staff       (20)    30924 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/condense.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8820 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/condense_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     2913 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/constants.F90
+-rw-r--r--   0 runner     (501) staff       (20)    20205 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/env_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4419 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/exact_soln.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3949 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/extract_aero_particles.F90
+-rw-r--r--   0 runner     (501) staff       (20)     6528 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/extract_aero_size.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5072 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/extract_aero_time.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4227 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/extract_env.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3867 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/extract_gas.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5692 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/extract_sectional_aero_size.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4858 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/extract_sectional_aero_time.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23458 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/fractal.F90
+-rw-r--r--   0 runner     (501) staff       (20)    16247 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/gas_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    22073 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/gas_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7566 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/getopt.F90
+-rw-r--r--   0 runner     (501) staff       (20)    15007 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/integer_rmap.F90
+-rw-r--r--   0 runner     (501) staff       (20)    19200 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/integer_rmap2.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8378 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/integer_varray.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18380 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/mosaic.F90
+-rw-r--r--   0 runner     (501) staff       (20)    47083 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/mpi.F90
+-rw-r--r--   0 runner     (501) staff       (20)    27550 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/netcdf.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8579 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/nucleate.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7062 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/numeric_average.F90
+-rw-r--r--   0 runner     (501) staff       (20)    10911 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/numeric_diff.F90
+-rw-r--r--   0 runner     (501) staff       (20)    30038 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/output.F90
+-rw-r--r--   0 runner     (501) staff       (20)    48249 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/partmc.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8459 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/photolysis.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18343 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/rand.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4712 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/rand_gsl.c
+-rw-r--r--   0 runner     (501) staff       (20)     2837 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/run_exact.F90
+-rw-r--r--   0 runner     (501) staff       (20)    32432 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/run_part.F90
+-rw-r--r--   0 runner     (501) staff       (20)    12069 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/run_sect.F90
+-rw-r--r--   0 runner     (501) staff       (20)    47571 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/scenario.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1563 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/sort.c
+-rw-r--r--   0 runner     (501) staff       (20)    23797 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/spec_file.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3063 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/spec_line.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23957 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/stats.F90
+-rw-r--r--   0 runner     (501) staff       (20)    49470 2023-07-03 00:20:06.000000 PyPartMC-0.3.0/gitmodules/partmc/src/util.F90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.553908 PyPartMC-0.3.0/gitmodules/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    10999 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1684 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.215754 PyPartMC-0.3.0/gitmodules/pybind11/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.565616 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    23883 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner     (501) staff       (20)     7069 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner     (501) staff       (20)    65224 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner     (501) staff       (20)     8458 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner     (501) staff       (20)      120 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     2096 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.569951 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner     (501) staff       (20)    28078 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner     (501) staff       (20)    49007 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     5491 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner     (501) staff       (20)    17971 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner     (501) staff       (20)    23981 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner     (501) staff       (20)    44230 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner     (501) staff       (20)     1513 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner     (501) staff       (20)    31685 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner     (501) staff       (20)    10728 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner     (501) staff       (20)     4731 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner     (501) staff       (20)     4658 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner     (501) staff       (20)     6923 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner     (501) staff       (20)     8851 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner     (501) staff       (20)    78946 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner     (501) staff       (20)     9051 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner     (501) staff       (20)     2181 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner     (501) staff       (20)   125304 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner     (501) staff       (20)    80981 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.570509 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner     (501) staff       (20)     4185 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner     (501) staff       (20)    14535 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner     (501) staff       (20)    27013 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.572239 PyPartMC-0.3.0/gitmodules/pybind11/tools/
+-rw-r--r--   0 runner     (501) staff       (20)    10455 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner     (501) staff       (20)    13460 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     7270 2023-07-03 00:20:09.000000 PyPartMC-0.3.0/gitmodules/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.217928 PyPartMC-0.3.0/gitmodules/pybind11_json/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.218092 PyPartMC-0.3.0/gitmodules/pybind11_json/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.572764 PyPartMC-0.3.0/gitmodules/pybind11_json/include/pybind11_json/
+-rw-r--r--   0 runner     (501) staff       (20)     7219 2023-07-03 00:20:10.000000 PyPartMC-0.3.0/gitmodules/pybind11_json/include/pybind11_json/pybind11_json.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.573305 PyPartMC-0.3.0/gitmodules/span/
+-rw-r--r--   0 runner     (501) staff       (20)     1338 2023-07-03 00:20:11.000000 PyPartMC-0.3.0/gitmodules/span/LICENSE_1_0.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.219003 PyPartMC-0.3.0/gitmodules/span/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.573817 PyPartMC-0.3.0/gitmodules/span/include/tcb/
+-rw-r--r--   0 runner     (501) staff       (20)    18165 2023-07-03 00:20:11.000000 PyPartMC-0.3.0/gitmodules/span/include/tcb/span.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.574412 PyPartMC-0.3.0/gitmodules/string_view-standalone/
+-rw-r--r--   0 runner     (501) staff       (20)     1077 2023-07-03 00:20:12.000000 PyPartMC-0.3.0/gitmodules/string_view-standalone/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.220200 PyPartMC-0.3.0/gitmodules/string_view-standalone/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.575003 PyPartMC-0.3.0/gitmodules/string_view-standalone/include/bpstd/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.575560 PyPartMC-0.3.0/gitmodules/string_view-standalone/include/bpstd/detail/
+-rw-r--r--   0 runner     (501) staff       (20)    29304 2023-07-03 00:20:12.000000 PyPartMC-0.3.0/gitmodules/string_view-standalone/include/bpstd/detail/string_view.inl
+-rw-r--r--   0 runner     (501) staff       (20)    20256 2023-07-03 00:20:12.000000 PyPartMC-0.3.0/gitmodules/string_view-standalone/include/bpstd/string_view.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.576813 PyPartMC-0.3.0/gitmodules/sundials/
+-rw-r--r--   0 runner     (501) staff       (20)     8077 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1576 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.578418 PyPartMC-0.3.0/gitmodules/sundials/cmake/
+-rw-r--r--   0 runner     (501) staff       (20)     2962 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/cmake/SundialsIndexSize.cmake
+-rw-r--r--   0 runner     (501) staff       (20)    10395 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/cmake/SundialsSetupCompilers.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     4883 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/cmake/SundialsSetupConfig.cmake
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.224026 PyPartMC-0.3.0/gitmodules/sundials/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.583658 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/
+-rw-r--r--   0 runner     (501) staff       (20)     9544 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode.h
+-rw-r--r--   0 runner     (501) staff       (20)     1525 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_bandpre.h
+-rw-r--r--   0 runner     (501) staff       (20)     2182 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_bbdpre.h
+-rw-r--r--   0 runner     (501) staff       (20)     1790 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_diag.h
+-rw-r--r--   0 runner     (501) staff       (20)     2035 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_direct.h
+-rw-r--r--   0 runner     (501) staff       (20)    10422 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_hypamgpre.h
+-rw-r--r--   0 runner     (501) staff       (20)     6515 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_ls.h
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_proj.h
+-rw-r--r--   0 runner     (501) staff       (20)     2873 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_spils.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.591553 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/
+-rw-r--r--   0 runner     (501) staff       (20)     9721 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_cuda.h
+-rw-r--r--   0 runner     (501) staff       (20)     9653 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_hip.h
+-rw-r--r--   0 runner     (501) staff       (20)     8671 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_manyvector.h
+-rw-r--r--   0 runner     (501) staff       (20)     9959 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_mpimanyvector.h
+-rw-r--r--   0 runner     (501) staff       (20)     1644 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_mpiplusx.h
+-rw-r--r--   0 runner     (501) staff       (20)     9487 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_openmp.h
+-rw-r--r--   0 runner     (501) staff       (20)     9612 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_openmpdev.h
+-rw-r--r--   0 runner     (501) staff       (20)    10795 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_parallel.h
+-rw-r--r--   0 runner     (501) staff       (20)     9697 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_parhyp.h
+-rw-r--r--   0 runner     (501) staff       (20)     9419 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_petsc.h
+-rw-r--r--   0 runner     (501) staff       (20)    11042 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_pthreads.h
+-rw-r--r--   0 runner     (501) staff       (20)     8267 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_raja.h
+-rw-r--r--   0 runner     (501) staff       (20)     8934 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_serial.h
+-rw-r--r--   0 runner     (501) staff       (20)    10053 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_sycl.h
+-rw-r--r--   0 runner     (501) staff       (20)     5824 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_trilinos.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.592857 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/trilinos/
+-rw-r--r--   0 runner     (501) staff       (20)     1819 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorInterface.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    23964 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorKernels.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.606082 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/
+-rw-r--r--   0 runner     (501) staff       (20)     7791 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_band.h
+-rw-r--r--   0 runner     (501) staff       (20)     5329 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_config.in
+-rw-r--r--   0 runner     (501) staff       (20)     5520 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_cuda_policies.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8997 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_dense.h
+-rw-r--r--   0 runner     (501) staff       (20)    13330 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_direct.h
+-rw-r--r--   0 runner     (501) staff       (20)     1690 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_fconfig.in
+-rw-r--r--   0 runner     (501) staff       (20)     1123 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_fnvector.h
+-rw-r--r--   0 runner     (501) staff       (20)     1128 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_futils.h
+-rw-r--r--   0 runner     (501) staff       (20)     5478 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_hip_policies.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    10283 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_iterative.h
+-rw-r--r--   0 runner     (501) staff       (20)    10707 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_lapack.h
+-rw-r--r--   0 runner     (501) staff       (20)     9633 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_linearsolver.h
+-rw-r--r--   0 runner     (501) staff       (20)     7839 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_math.h
+-rw-r--r--   0 runner     (501) staff       (20)     5466 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_matrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     4527 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_memory.h
+-rw-r--r--   0 runner     (501) staff       (20)     1399 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_mpi_types.h
+-rw-r--r--   0 runner     (501) staff       (20)     9190 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_nonlinearsolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    12719 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_nvector.h
+-rw-r--r--   0 runner     (501) staff       (20)     4744 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_nvector_senswrapper.h
+-rw-r--r--   0 runner     (501) staff       (20)     4567 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_sycl_policies.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5165 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_types.h
+-rw-r--r--   0 runner     (501) staff       (20)     1266 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_version.h
+-rw-r--r--   0 runner     (501) staff       (20)     4024 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_xbraid.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.614534 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/
+-rw-r--r--   0 runner     (501) staff       (20)     2649 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_band.h
+-rw-r--r--   0 runner     (501) staff       (20)     4768 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_cusolversp_batchqr.h
+-rw-r--r--   0 runner     (501) staff       (20)     2983 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_dense.h
+-rw-r--r--   0 runner     (501) staff       (20)     5603 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_klu.h
+-rw-r--r--   0 runner     (501) staff       (20)     3142 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackband.h
+-rw-r--r--   0 runner     (501) staff       (20)     3171 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackdense.h
+-rw-r--r--   0 runner     (501) staff       (20)     2751 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_magmadense.h
+-rw-r--r--   0 runner     (501) staff       (20)     3052 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_onemkldense.h
+-rw-r--r--   0 runner     (501) staff       (20)     4553 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_pcg.h
+-rw-r--r--   0 runner     (501) staff       (20)     4872 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spbcgs.h
+-rw-r--r--   0 runner     (501) staff       (20)     5330 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spfgmr.h
+-rw-r--r--   0 runner     (501) staff       (20)     5237 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spgmr.h
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_sptfqmr.h
+-rw-r--r--   0 runner     (501) staff       (20)     5621 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_superludist.h
+-rw-r--r--   0 runner     (501) staff       (20)     4533 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_superlumt.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.618503 PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/
+-rw-r--r--   0 runner     (501) staff       (20)     4552 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_band.h
+-rw-r--r--   0 runner     (501) staff       (20)     5233 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_cusparse.h
+-rw-r--r--   0 runner     (501) staff       (20)     3647 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_dense.h
+-rw-r--r--   0 runner     (501) staff       (20)     5083 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_magmadense.h
+-rw-r--r--   0 runner     (501) staff       (20)     5776 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_onemkldense.h
+-rw-r--r--   0 runner     (501) staff       (20)     3245 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_slunrloc.h
+-rw-r--r--   0 runner     (501) staff       (20)     5136 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_sparse.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.620282 PyPartMC-0.3.0/gitmodules/sundials/include/sunnonlinsol/
+-rw-r--r--   0 runner     (501) staff       (20)     6202 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_fixedpoint.h
+-rw-r--r--   0 runner     (501) staff       (20)     5449 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_newton.h
+-rw-r--r--   0 runner     (501) staff       (20)     4071 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_petscsnes.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.233846 PyPartMC-0.3.0/gitmodules/sundials/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.636689 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/
+-rw-r--r--   0 runner     (501) staff       (20)     1972 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/CHANGES
+-rw-r--r--   0 runner     (501) staff       (20)     3549 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1576 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     1166 2023-07-03 00:20:29.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/NOTICE
+-rw-r--r--   0 runner     (501) staff       (20)     2708 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/README.md
+-rw-r--r--   0 runner     (501) staff       (20)   135753 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode.c
+-rw-r--r--   0 runner     (501) staff       (20)    18212 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_bandpre.c
+-rw-r--r--   0 runner     (501) staff       (20)     2383 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_bandpre_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    22668 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_bbdpre.c
+-rw-r--r--   0 runner     (501) staff       (20)     2621 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_bbdpre_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    13629 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_diag.c
+-rw-r--r--   0 runner     (501) staff       (20)     2240 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_diag_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)     1956 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_direct.c
+-rw-r--r--   0 runner     (501) staff       (20)    14722 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_fused_gpu.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5554 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_fused_stubs.c
+-rw-r--r--   0 runner     (501) staff       (20)    14959 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_hypamgpre.c
+-rw-r--r--   0 runner     (501) staff       (20)     2766 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_hypamgpre_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    29404 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    28172 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_io.c
+-rw-r--r--   0 runner     (501) staff       (20)    58312 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_ls.c
+-rw-r--r--   0 runner     (501) staff       (20)     8077 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_ls_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    12911 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_nls.c
+-rw-r--r--   0 runner     (501) staff       (20)    12603 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_proj.c
+-rw-r--r--   0 runner     (501) staff       (20)     3079 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_proj_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)     2943 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_spils.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.649374 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/
+-rw-r--r--   0 runner     (501) staff       (20)     1734 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     4616 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/Makefile.in
+-rw-r--r--   0 runner     (501) staff       (20)     3464 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvband.c
+-rw-r--r--   0 runner     (501) staff       (20)     4950 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvbbd.c
+-rw-r--r--   0 runner     (501) staff       (20)    22548 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvbbd.h
+-rw-r--r--   0 runner     (501) staff       (20)     2063 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvbp.c
+-rw-r--r--   0 runner     (501) staff       (20)    14934 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvbp.h
+-rw-r--r--   0 runner     (501) staff       (20)     2952 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvdense.c
+-rw-r--r--   0 runner     (501) staff       (20)     2046 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvewt.c
+-rw-r--r--   0 runner     (501) staff       (20)     3904 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvjtimes.c
+-rw-r--r--   0 runner     (501) staff       (20)     1370 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvnulllinsol.c
+-rw-r--r--   0 runner     (501) staff       (20)     1344 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvnullmatrix.c
+-rw-r--r--   0 runner     (501) staff       (20)     1502 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvnullnonlinsol.c
+-rw-r--r--   0 runner     (501) staff       (20)    15564 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvode.c
+-rw-r--r--   0 runner     (501) staff       (20)    49120 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvode.h
+-rw-r--r--   0 runner     (501) staff       (20)     4190 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvpreco.c
+-rw-r--r--   0 runner     (501) staff       (20)     2399 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvroot.c
+-rw-r--r--   0 runner     (501) staff       (20)     4974 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvroot.h
+-rw-r--r--   0 runner     (501) staff       (20)     2921 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvsparse.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.651435 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1483 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    43017 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fmod/fcvode_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    83166 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fmod/fcvode_mod.f90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.652225 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/
+-rw-r--r--   0 runner     (501) staff       (20)     1562 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.654354 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/
+-rw-r--r--   0 runner     (501) staff       (20)     1648 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.656754 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)      979 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    25549 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    40279 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     3740 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fnvector_serial.c
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fnvector_serial.h
+-rw-r--r--   0 runner     (501) staff       (20)    47581 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/nvector_serial.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.669346 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/
+-rw-r--r--   0 runner     (501) staff       (20)     3022 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.677736 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1109 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     7228 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)     2922 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)    13682 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    19932 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     9392 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)     9541 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)    11515 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    12797 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)    24749 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    42038 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     6561 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)      957 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     6784 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_band.c
+-rw-r--r--   0 runner     (501) staff       (20)     3712 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_cuda.h
+-rw-r--r--   0 runner     (501) staff       (20)     7056 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_cuda_kernels.cuh
+-rw-r--r--   0 runner     (501) staff       (20)     1403 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_debug.h
+-rw-r--r--   0 runner     (501) staff       (20)     9098 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_dense.c
+-rw-r--r--   0 runner     (501) staff       (20)     6468 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_direct.c
+-rw-r--r--   0 runner     (501) staff       (20)      964 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_futils.c
+-rw-r--r--   0 runner     (501) staff       (20)     2500 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_hip.h
+-rw-r--r--   0 runner     (501) staff       (20)     7260 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_hip_kernels.hip.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8008 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_iterative.c
+-rw-r--r--   0 runner     (501) staff       (20)     5667 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_linearsolver.c
+-rw-r--r--   0 runner     (501) staff       (20)     2956 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_math.c
+-rw-r--r--   0 runner     (501) staff       (20)     4633 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_matrix.c
+-rw-r--r--   0 runner     (501) staff       (20)     4810 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_memory.c
+-rw-r--r--   0 runner     (501) staff       (20)     6479 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_nonlinearsolver.c
+-rw-r--r--   0 runner     (501) staff       (20)    20704 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_nvector.c
+-rw-r--r--   0 runner     (501) staff       (20)    13469 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_nvector_senswrapper.c
+-rw-r--r--   0 runner     (501) staff       (20)     3051 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_sycl.h
+-rw-r--r--   0 runner     (501) staff       (20)     1592 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_version.c
+-rw-r--r--   0 runner     (501) staff       (20)     6371 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_xbraid.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.678338 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/
+-rw-r--r--   0 runner     (501) staff       (20)     1481 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.680473 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/
+-rw-r--r--   0 runner     (501) staff       (20)     1798 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.682318 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1085 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     9961 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)     7950 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     2963 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.c
+-rw-r--r--   0 runner     (501) staff       (20)     1892 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.h
+-rw-r--r--   0 runner     (501) staff       (20)     7118 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/sunlinsol_band.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.684756 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/
+-rw-r--r--   0 runner     (501) staff       (20)     1844 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.686358 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     9982 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)     8001 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     2978 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.c
+-rw-r--r--   0 runner     (501) staff       (20)     1930 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.h
+-rw-r--r--   0 runner     (501) staff       (20)     6580 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/sunlinsol_dense.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.690185 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.692576 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1053 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    13106 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    13874 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     4522 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.c
+-rw-r--r--   0 runner     (501) staff       (20)     3046 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.h
+-rw-r--r--   0 runner     (501) staff       (20)    13160 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/sunlinsol_klu.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.693645 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/pcg/
+-rw-r--r--   0 runner     (501) staff       (20)     1709 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/pcg/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    16843 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/pcg/sunlinsol_pcg.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.694782 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spbcgs/
+-rw-r--r--   0 runner     (501) staff       (20)     1743 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spbcgs/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    22722 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spbcgs/sunlinsol_spbcgs.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.695929 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spfgmr/
+-rw-r--r--   0 runner     (501) staff       (20)     1700 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spfgmr/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    25504 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spfgmr/sunlinsol_spfgmr.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.697152 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spgmr/
+-rw-r--r--   0 runner     (501) staff       (20)     1687 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spgmr/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    26697 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spgmr/sunlinsol_spgmr.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.698498 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/sptfqmr/
+-rw-r--r--   0 runner     (501) staff       (20)     1713 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/sptfqmr/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    28426 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/sptfqmr/sunlinsol_sptfqmr.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.699098 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/
+-rw-r--r--   0 runner     (501) staff       (20)     1085 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.700201 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/band/
+-rw-r--r--   0 runner     (501) staff       (20)     1691 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/band/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    13124 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/band/sunmatrix_band.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.701273 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/dense/
+-rw-r--r--   0 runner     (501) staff       (20)     1742 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/dense/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     8906 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/dense/sunmatrix_dense.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.702704 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/sparse/
+-rw-r--r--   0 runner     (501) staff       (20)     1760 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/sparse/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    34432 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/sparse/sunmatrix_sparse.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.703406 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/
+-rw-r--r--   0 runner     (501) staff       (20)      842 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.705913 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/
+-rw-r--r--   0 runner     (501) staff       (20)     1855 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.707855 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1064 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    12989 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    13798 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     2718 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.c
+-rw-r--r--   0 runner     (501) staff       (20)     2126 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.h
+-rw-r--r--   0 runner     (501) staff       (20)    23849 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/sunnonlinsol_fixedpoint.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.709972 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/
+-rw-r--r--   0 runner     (501) staff       (20)     1801 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.711768 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1039 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    13234 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    14015 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     2672 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.c
+-rw-r--r--   0 runner     (501) staff       (20)     2051 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.h
+-rw-r--r--   0 runner     (501) staff       (20)    16132 2023-07-03 00:20:30.000000 PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/sunnonlinsol_newton.c
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-03 00:20:53.753612 PyPartMC-0.3.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     6723 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.740309 PyPartMC-0.3.0/src/
+-rw-r--r--   0 runner     (501) staff       (20)     5588 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5798 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_data.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2474 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_dist.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2299 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_dist.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     7465 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_mode.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7830 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_mode.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    14256 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_particle.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9957 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_particle.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     9208 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8850 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/aero_state.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4355 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/bin_grid.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1984 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/bin_grid.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     3337 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/bin_grid.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1104 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/camp_core.F90
+-rw-r--r--   0 runner     (501) staff       (20)      802 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/camp_core.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2152 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/condense.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1073 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/condense.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1108 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/condense.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4224 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/env_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3676 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/env_state.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     9942 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/fake_spec_file.F90
+-rw-r--r--   0 runner     (501) staff       (20)     6791 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/fake_spec_file.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2228 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/gas_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2406 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/gas_data.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3220 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/gas_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4086 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/gas_state.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      695 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/gimmicks.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     9002 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/gimmicks.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3808 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/output.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1826 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/output.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1781 2023-07-03 00:19:01.000000 PyPartMC-0.3.0/src/output.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1070 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/photolysis.F90
+-rw-r--r--   0 runner     (501) staff       (20)      810 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/photolysis.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1127 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/pmc_resource.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    20848 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/pypartmc.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      944 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/rand.F90
+-rw-r--r--   0 runner     (501) staff       (20)      720 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/rand.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      729 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/rand.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8174 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/run_part.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2647 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/run_part.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2400 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/run_part.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5918 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/run_part_opt.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1592 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/run_part_opt.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     6950 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/scenario.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1189 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/scenario.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5931 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/scenario.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      782 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/sys.F90
+-rw-r--r--   0 runner     (501) staff       (20)      711 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/sys.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1373 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/util.F90
+-rw-r--r--   0 runner     (501) staff       (20)      988 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/util.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      971 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/src/util.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-03 00:20:53.752158 PyPartMC-0.3.0/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       47 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner     (501) staff       (20)    10474 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_aero_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     4441 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_aero_dist.py
+-rw-r--r--   0 runner     (501) staff       (20)     6795 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_aero_mode.py
+-rw-r--r--   0 runner     (501) staff       (20)    15729 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_aero_particle.py
+-rw-r--r--   0 runner     (501) staff       (20)     7255 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_aero_state.py
+-rw-r--r--   0 runner     (501) staff       (20)     5955 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_bin_grid.py
+-rw-r--r--   0 runner     (501) staff       (20)     2426 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_condense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1745 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_dtors.py
+-rw-r--r--   0 runner     (501) staff       (20)     2366 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_env_state.py
+-rw-r--r--   0 runner     (501) staff       (20)     1622 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_gas_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     3225 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_gas_state.py
+-rw-r--r--   0 runner     (501) staff       (20)     2847 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_loss_rate.py
+-rw-r--r--   0 runner     (501) staff       (20)     3726 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_output.py
+-rw-r--r--   0 runner     (501) staff       (20)     1027 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_rand.py
+-rw-r--r--   0 runner     (501) staff       (20)     1999 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_run_part.py
+-rw-r--r--   0 runner     (501) staff       (20)     2554 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_run_part_opt.py
+-rw-r--r--   0 runner     (501) staff       (20)     9284 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_scenario.py
+-rw-r--r--   0 runner     (501) staff       (20)      644 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_units.py
+-rw-r--r--   0 runner     (501) staff       (20)     1624 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_util.py
+-rw-r--r--   0 runner     (501) staff       (20)      580 2023-07-03 00:19:02.000000 PyPartMC-0.3.0/tests/test_version.py
```

### Comparing `PyPartMC-0.2.0/.github/workflows/conda.yml` & `PyPartMC-0.3.0/.github/workflows/conda.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/.github/workflows/pdoc.yml` & `PyPartMC-0.3.0/.github/workflows/pdoc.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/.github/workflows/pylint.yml` & `PyPartMC-0.3.0/.github/workflows/pylint.yml`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         python-version: 3.9
     - run: |
         python -m pip install --upgrade pip
         pip install pylint nbqa
         pip install -e .[tests]
         pip install -r .binder/requirements.txt
     - run: pylint --unsafe-load-any-extension=y --disable=fixme,no-member,trailing-newlines,missing-module-docstring,missing-class-docstring,missing-function-docstring,unnecessary-pass $(git ls-files '*.py')
-    - run: nbqa pylint --unsafe-load-any-extension=y --disable=fixme,no-member,wrong-import-position,ungrouped-imports,trailing-whitespace,missing-function-docstring,missing-module-docstring $(git ls-files '*.ipynb')
+    - run: nbqa pylint --unsafe-load-any-extension=y --disable=fixme,no-member,duplicate-code,wrong-import-position,ungrouped-imports,trailing-whitespace,missing-function-docstring,missing-module-docstring $(git ls-files '*.ipynb')
```

### Comparing `PyPartMC-0.2.0/.github/workflows/readme_julia.yml` & `PyPartMC-0.3.0/.github/workflows/readme_julia.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/.github/workflows/readme_matlab.yml` & `PyPartMC-0.3.0/.github/workflows/readme_matlab.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/.github/workflows/readme_python.yml` & `PyPartMC-0.3.0/.github/workflows/readme_python.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/.github/workflows/stale.yml` & `PyPartMC-0.3.0/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/.github/workflows/tests+pypi.yml` & `PyPartMC-0.3.0/.github/workflows/tests+pypi.yml`

 * *Files 8% similar despite different names*

```diff
@@ -44,21 +44,20 @@
         uses: msys2/setup-msys2@v2
         with:
           msystem: MINGW64
           update: false
           install: >-
             mingw-w64-x86_64-gcc-fortran
             mingw-w64-x86_64-ninja
+            m4
 
       - if: matrix.platform == 'windows-latest'
         run: |
-          echo CMAKE_ARGS="-DCMAKE_Fortran_COMPILER=D:/a/_temp/msys64/mingw64/bin/gfortran.exe" >> $GITHUB_ENV
-          echo CMAKE_ARGS="-DCMAKE_C_COMPILER=D:/a/_temp/msys64/mingw64/bin/gcc.exe" >> $GITHUB_ENV
-          echo CMAKE_ARGS="-DCMAKE_CXX_COMPILER=D:/a/_temp/msys64/mingw64/bin/g++.exe" >> $GITHUB_ENV
           echo CMAKE_ARGS="-DCMAKE_MAKE_PROGRAM=D:/a/_temp/msys64/mingw64/bin/ninja.exe" >> $GITHUB_ENV
+          echo CMAKE_PROGRAM_PATH="D:/a/_temp/msys64/usr/bin" >> $GITHUB_ENV
           echo CMAKE_GENERATOR="Ninja" >> $GITHUB_ENV
           echo TEMP="D:/a/_temp/" >> $GITHUB_ENV
 
       - uses: actions/checkout@v2
         with:
           submodules: recursive
           fetch-depth: 0  # https://github.com/pypa/setuptools_scm/issues/480
@@ -135,21 +134,20 @@
         path: dist
     - run: twine check --strict dist/*
     - run: for i in dist/*-manylinux*.whl; do auditwheel show $i; done;
 
   dist_upload:
     runs-on: ubuntu-latest
     needs: [dist_check]
+    permissions:
+      id-token: write
     steps:
     - uses: actions/download-artifact@v2
       with:
         name: dist
         path: dist
     - if: github.event_name == 'push' && github.ref == 'refs/heads/main'
-      uses: pypa/gh-action-pypi-publish@master
+      uses: pypa/gh-action-pypi-publish@unstable/v1
       with:
-        password: ${{ secrets.TEST_PYPI_API_TOKEN }}
         repository_url: https://test.pypi.org/legacy/
     - if: startsWith(github.ref, 'refs/tags')
-      uses: pypa/gh-action-pypi-publish@master
-      with:
-        password: ${{ secrets.PYPI_API_TOKEN }}
+      uses: pypa/gh-action-pypi-publish@unstable/v1
```

### Comparing `PyPartMC-0.2.0/.gitmodules` & `PyPartMC-0.3.0/.gitmodules`

 * *Files 13% similar despite different names*

```diff
@@ -38,7 +38,15 @@
 	path = gitmodules/json-fortran
 	url = https://github.com/jacobwilliams/json-fortran
 	shallow = true
 [submodule "gitmodules/devops_tests"]
 	path = gitmodules/devops_tests
 	url = https://github.com/open-atmos/devops_tests
 	shallow = true
+[submodule "gitmodules/netcdf-fortran"]
+	path = gitmodules/netcdf-fortran
+	url = https://github.com/Unidata/netcdf-fortran.git
+	shallow = true
+[submodule "gitmodules/netcdf-c"]
+	path = gitmodules/netcdf-c
+	url = https://github.com/Unidata/netcdf-c.git
+	shallow = true
```

### Comparing `PyPartMC-0.2.0/LICENSE` & `PyPartMC-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/PKG-INFO` & `PyPartMC-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPartMC
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python interface to PartMC
 Author: Sylwester Arabas
 Author-email: sarabas@illinois.edu
 License: GPL-3.0
 Project-URL: Tracker, https://github.com/open-atmos/PyPartMC/issues
 Project-URL: Documentation, https://open-atmos.github.io/PyPartMC
 Project-URL: Source, https://github.com/open-atmos/PyPartMC/
@@ -63,15 +63,15 @@
 - ships with [a set of examples](https://github.com/open-atmos/PyPartMC/tree/main/examples) maintained in a form of Jupyter notebooks
 - Pythonic API (but retaining PartMC jargon) incl. Python GC deallocation of Fortran objects
 - specification of parameters using native Python datatypes (lists, dicts) in place of PartMC spec files
 - code snippets in README depicting how to use PyPartMC from Julia (also executed on CI)
 - auto-generated [API docs on the web](https://open-atmos.github.io/PyPartMC/)
 - support for [de]serialization of selected wrapped structures using JSON 
 - based on [unmodified PartMC code](https://github.com/open-atmos/PyPartMC/tree/main/gitmodules)
-- does not use or require shell or netCDF Fortran library
+- does not use or require shell or any pre-installed libraries
 - aiming at 100% [unit test coverage](https://github.com/open-atmos/PyPartMC/tree/main/tests)
 
 ## Usage examples
 
 #### example object instantiation in Python
 
 ```python
@@ -96,31 +96,77 @@
 PyPartMC is used within the [test workflow of the PySDM project](https://github.com/atmos-cloud-sim-uj/PySDM/tree/main/tests/smoke_tests/partmc).
 
 ## Implementation outline
 
 - PyPartMC is written in C++, Fortran and uses [pybind11](https://pybind11.readthedocs.io/en/stable/) and [CMake](https://cmake.org/).
 - JSON support is handled with [nlohmann::json](https://github.com/nlohmann/json) and [pybind11_json](https://github.com/pybind/pybind11_json)
 - PartMC and selected parts of SUNDIALS are statically linked (and compiled in during `pip install` or `python -m build`) 
-- C (SUNDIALS), C++ (pybind11, ...) and Fortran (PartMC, CAMP) dependencies are linked through [git submodules](https://github.com/open-atmos/PyPartMC/blob/main/.gitmodules)
-- MOSAIC dependency is optionally linked through setting the environmental variable MOSAIC_HOME
-- a [mock of Fortran netCDF API](https://github.com/open-atmos/PyPartMC/blob/main/src/fake_netcdf.F90) and a [mock of PartMC spec file API](https://github.com/open-atmos/PyPartMC/blob/main/src/fake_spec_file.F90) are used for i/o from/to JSON 
+- C (SUNDIALS, netCDF), C++ (pybind11, ...) and Fortran (PartMC, CAMP, netCDF-fortran) dependencies are linked through [git submodules](https://github.com/open-atmos/PyPartMC/blob/main/.gitmodules)
+- MOSAIC dependency is optionally linked through setting the environmental variable `MOSAIC_HOME`
+- a [drop-in replacement of the PartMC spec file routines](https://github.com/open-atmos/PyPartMC/blob/main/src/fake_spec_file.F90) is used for i/o from/to JSON 
+
+## Implementation architecture
+
+```mermaid
+flowchart TD
+    subgraph J ["Julia"]
+        julia_user_code["Julia user code"] --> PyCall.jl
+    end
+    subgraph P ["Python"]
+        PyCall.jl --> PyPartMC
+        python_user_code -.-> NumPy
+        python_user_code["Python user code"] ---> PyPartMC["pubind11-generated PyPartMC module"]
+    end
+    subgraph Cpp ["C++"]
+        cpp_user_code["C++ user code"] ----> ppmc_cpp
+        PyPartMC --> ppmc_cpp["PyPartMC-C++"]
+        ppmc_cpp --> pybind11_json
+        pybind11_json ---> nlohmann::JSON
+        fake_spec_file_cpp --> nlohmann::JSON
+    end
+    subgraph C ["C"]
+        fake_spec_file_c --> fake_spec_file_cpp["SpecFile-C++"]
+        ppmc_cpp --> ppmc_c["PyPartMC-C"]
+        netCDF-C
+        SUNDIALS
+        camp_c["CAMP C code"]
+    end
+    subgraph Fortran ["Fortran"]
+        PartMC -....-> MOSAIC
+        ppmc_c --> ppmc_f["PyPartMC-F"]
+        ppmc_f ---> PartMC
+        PartMC --> netCDF-F
+        netCDF-F --> netCDF-C
+        PartMC --> SUNDIALS
+        PartMC ---> camp_f
+        camp_f["CAMP"] --> camp_c
+        PartMC ----> fake_spec_file_f[SpecFile-F]
+        fake_spec_file_f --> fake_spec_file_c["SpecFile-C"]
+    end
+
+    style PartMC fill:#7ae7ff,stroke-width:2px,color:#2B2B2B
+```
 
 ## Troubleshooting 
 
 #### Common installation issues 
 ```
 error: [Errno 2] No such file or directory: 'cmake'
 ```
-Try rerunning after installing CMake (e.g., `apt-get install cmake` or `brew install cmake`)
+Try rerunning after installing CMake, e.g., using `apt-get install cmake` (Ubuntu/Debian), `brew install cmake` (homebrew on macOS) or using [MSYS2](https://www.msys2.org/docs/cmake/) on Windows.
 
 ```
 No CMAKE_Fortran_COMPILER could be found.
 ```
-Try installing a Fortran compiler (e.g., `brew reinstall gcc`)
+Try installing a Fortran compiler (e.g., `brew reinstall gcc` with Homebrew on macOS or using [MSYS2](https://packages.msys2.org/package/mingw-w64-x86_64-gcc-fortran?repo=mingw64) on Windows).
 
+```
+Could not find NC_M4 using the following names: m4, m4.exe
+```
+Try installing `m4` (e.g., using [MSYS2](https://packages.msys2.org/package/m4?repo=msys&variant=x86_64) on Windows).
 
 ## Notes for developers
 #### How to debug
 ```sh
 git clone --recursive git+https://github.com/open-atmos/PyPartMC.git
 cd PyPartMC
 DEBUG=1 VERBOSE=1 pip --verbose install -e .
```

### Comparing `PyPartMC-0.2.0/PyPartMC/__init__.py` & `PyPartMC-0.3.0/PyPartMC/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/PyPartMC.egg-info/PKG-INFO` & `PyPartMC-0.3.0/PyPartMC.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPartMC
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python interface to PartMC
 Author: Sylwester Arabas
 Author-email: sarabas@illinois.edu
 License: GPL-3.0
 Project-URL: Tracker, https://github.com/open-atmos/PyPartMC/issues
 Project-URL: Documentation, https://open-atmos.github.io/PyPartMC
 Project-URL: Source, https://github.com/open-atmos/PyPartMC/
@@ -63,15 +63,15 @@
 - ships with [a set of examples](https://github.com/open-atmos/PyPartMC/tree/main/examples) maintained in a form of Jupyter notebooks
 - Pythonic API (but retaining PartMC jargon) incl. Python GC deallocation of Fortran objects
 - specification of parameters using native Python datatypes (lists, dicts) in place of PartMC spec files
 - code snippets in README depicting how to use PyPartMC from Julia (also executed on CI)
 - auto-generated [API docs on the web](https://open-atmos.github.io/PyPartMC/)
 - support for [de]serialization of selected wrapped structures using JSON 
 - based on [unmodified PartMC code](https://github.com/open-atmos/PyPartMC/tree/main/gitmodules)
-- does not use or require shell or netCDF Fortran library
+- does not use or require shell or any pre-installed libraries
 - aiming at 100% [unit test coverage](https://github.com/open-atmos/PyPartMC/tree/main/tests)
 
 ## Usage examples
 
 #### example object instantiation in Python
 
 ```python
@@ -96,31 +96,77 @@
 PyPartMC is used within the [test workflow of the PySDM project](https://github.com/atmos-cloud-sim-uj/PySDM/tree/main/tests/smoke_tests/partmc).
 
 ## Implementation outline
 
 - PyPartMC is written in C++, Fortran and uses [pybind11](https://pybind11.readthedocs.io/en/stable/) and [CMake](https://cmake.org/).
 - JSON support is handled with [nlohmann::json](https://github.com/nlohmann/json) and [pybind11_json](https://github.com/pybind/pybind11_json)
 - PartMC and selected parts of SUNDIALS are statically linked (and compiled in during `pip install` or `python -m build`) 
-- C (SUNDIALS), C++ (pybind11, ...) and Fortran (PartMC, CAMP) dependencies are linked through [git submodules](https://github.com/open-atmos/PyPartMC/blob/main/.gitmodules)
-- MOSAIC dependency is optionally linked through setting the environmental variable MOSAIC_HOME
-- a [mock of Fortran netCDF API](https://github.com/open-atmos/PyPartMC/blob/main/src/fake_netcdf.F90) and a [mock of PartMC spec file API](https://github.com/open-atmos/PyPartMC/blob/main/src/fake_spec_file.F90) are used for i/o from/to JSON 
+- C (SUNDIALS, netCDF), C++ (pybind11, ...) and Fortran (PartMC, CAMP, netCDF-fortran) dependencies are linked through [git submodules](https://github.com/open-atmos/PyPartMC/blob/main/.gitmodules)
+- MOSAIC dependency is optionally linked through setting the environmental variable `MOSAIC_HOME`
+- a [drop-in replacement of the PartMC spec file routines](https://github.com/open-atmos/PyPartMC/blob/main/src/fake_spec_file.F90) is used for i/o from/to JSON 
+
+## Implementation architecture
+
+```mermaid
+flowchart TD
+    subgraph J ["Julia"]
+        julia_user_code["Julia user code"] --> PyCall.jl
+    end
+    subgraph P ["Python"]
+        PyCall.jl --> PyPartMC
+        python_user_code -.-> NumPy
+        python_user_code["Python user code"] ---> PyPartMC["pubind11-generated PyPartMC module"]
+    end
+    subgraph Cpp ["C++"]
+        cpp_user_code["C++ user code"] ----> ppmc_cpp
+        PyPartMC --> ppmc_cpp["PyPartMC-C++"]
+        ppmc_cpp --> pybind11_json
+        pybind11_json ---> nlohmann::JSON
+        fake_spec_file_cpp --> nlohmann::JSON
+    end
+    subgraph C ["C"]
+        fake_spec_file_c --> fake_spec_file_cpp["SpecFile-C++"]
+        ppmc_cpp --> ppmc_c["PyPartMC-C"]
+        netCDF-C
+        SUNDIALS
+        camp_c["CAMP C code"]
+    end
+    subgraph Fortran ["Fortran"]
+        PartMC -....-> MOSAIC
+        ppmc_c --> ppmc_f["PyPartMC-F"]
+        ppmc_f ---> PartMC
+        PartMC --> netCDF-F
+        netCDF-F --> netCDF-C
+        PartMC --> SUNDIALS
+        PartMC ---> camp_f
+        camp_f["CAMP"] --> camp_c
+        PartMC ----> fake_spec_file_f[SpecFile-F]
+        fake_spec_file_f --> fake_spec_file_c["SpecFile-C"]
+    end
+
+    style PartMC fill:#7ae7ff,stroke-width:2px,color:#2B2B2B
+```
 
 ## Troubleshooting 
 
 #### Common installation issues 
 ```
 error: [Errno 2] No such file or directory: 'cmake'
 ```
-Try rerunning after installing CMake (e.g., `apt-get install cmake` or `brew install cmake`)
+Try rerunning after installing CMake, e.g., using `apt-get install cmake` (Ubuntu/Debian), `brew install cmake` (homebrew on macOS) or using [MSYS2](https://www.msys2.org/docs/cmake/) on Windows.
 
 ```
 No CMAKE_Fortran_COMPILER could be found.
 ```
-Try installing a Fortran compiler (e.g., `brew reinstall gcc`)
+Try installing a Fortran compiler (e.g., `brew reinstall gcc` with Homebrew on macOS or using [MSYS2](https://packages.msys2.org/package/mingw-w64-x86_64-gcc-fortran?repo=mingw64) on Windows).
 
+```
+Could not find NC_M4 using the following names: m4, m4.exe
+```
+Try installing `m4` (e.g., using [MSYS2](https://packages.msys2.org/package/m4?repo=msys&variant=x86_64) on Windows).
 
 ## Notes for developers
 #### How to debug
 ```sh
 git clone --recursive git+https://github.com/open-atmos/PyPartMC.git
 cd PyPartMC
 DEBUG=1 VERBOSE=1 pip --verbose install -e .
```

### Comparing `PyPartMC-0.2.0/PyPartMC.egg-info/SOURCES.txt` & `PyPartMC-0.3.0/PyPartMC.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 PyPartMC.egg-info/dependency_links.txt
 PyPartMC.egg-info/not-zip-safe
 PyPartMC.egg-info/requires.txt
 PyPartMC.egg-info/top_level.txt
 examples/hello_world.ipynb
 examples/lognorm_ex.ipynb
 examples/particle_simulation.ipynb
+examples/process_simulation_output.ipynb
 examples/terminal_velocities.ipynb
 examples/widgets_playground.ipynb
+gitmodules/SuiteSparse/LICENSE.txt
 gitmodules/SuiteSparse/AMD/Include/amd.h
 gitmodules/SuiteSparse/AMD/Include/amd_internal.h
 gitmodules/SuiteSparse/AMD/Source/amd.f
 gitmodules/SuiteSparse/AMD/Source/amd_1.c
 gitmodules/SuiteSparse/AMD/Source/amd_2.c
 gitmodules/SuiteSparse/AMD/Source/amd_aat.c
 gitmodules/SuiteSparse/AMD/Source/amd_control.c
@@ -73,14 +75,15 @@
 gitmodules/SuiteSparse/KLU/Source/klu_refactor.c
 gitmodules/SuiteSparse/KLU/Source/klu_scale.c
 gitmodules/SuiteSparse/KLU/Source/klu_solve.c
 gitmodules/SuiteSparse/KLU/Source/klu_sort.c
 gitmodules/SuiteSparse/KLU/Source/klu_tsolve.c
 gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c
 gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h
+gitmodules/camp/COPYING
 gitmodules/camp/src/Jacobian.c
 gitmodules/camp/src/Jacobian.h
 gitmodules/camp/src/aero_phase_data.F90
 gitmodules/camp/src/aero_phase_solver.c
 gitmodules/camp/src/aero_phase_solver.h
 gitmodules/camp/src/aero_rep_data.F90
 gitmodules/camp/src/aero_rep_factory.F90
@@ -156,14 +159,16 @@
 gitmodules/camp/src/rxns/rxn_wet_deposition.c
 gitmodules/camp/src/sub_models/sub_model_PDFiTE.F90
 gitmodules/camp/src/sub_models/sub_model_PDFiTE.c
 gitmodules/camp/src/sub_models/sub_model_UNIFAC.F90
 gitmodules/camp/src/sub_models/sub_model_UNIFAC.c
 gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.F90
 gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.c
+gitmodules/json/LICENSE.MIT
+gitmodules/json-fortran/LICENSE
 gitmodules/json-fortran/src/json_file_module.F90
 gitmodules/json-fortran/src/json_get_scalar_by_path.inc
 gitmodules/json-fortran/src/json_get_vec_by_path.inc
 gitmodules/json-fortran/src/json_get_vec_by_path_alloc.inc
 gitmodules/json-fortran/src/json_initialize_arguments.inc
 gitmodules/json-fortran/src/json_initialize_dummy_arguments.inc
 gitmodules/json-fortran/src/json_kinds.F90
@@ -260,14 +265,161 @@
 gitmodules/json/include/nlohmann/detail/meta/call_std/begin.hpp
 gitmodules/json/include/nlohmann/detail/meta/call_std/end.hpp
 gitmodules/json/include/nlohmann/detail/output/binary_writer.hpp
 gitmodules/json/include/nlohmann/detail/output/output_adapters.hpp
 gitmodules/json/include/nlohmann/detail/output/serializer.hpp
 gitmodules/json/include/nlohmann/thirdparty/hedley/hedley.hpp
 gitmodules/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp
+gitmodules/netcdf-c/CMakeLists.txt
+gitmodules/netcdf-c/COPYRIGHT
+gitmodules/netcdf-c/config.h.cmake.in
+gitmodules/netcdf-c/include/fbits.h
+gitmodules/netcdf-c/include/nc.h
+gitmodules/netcdf-c/include/nc3dispatch.h
+gitmodules/netcdf-c/include/nc3internal.h
+gitmodules/netcdf-c/include/nc4dispatch.h
+gitmodules/netcdf-c/include/nc4internal.h
+gitmodules/netcdf-c/include/nc_logging.h
+gitmodules/netcdf-c/include/nc_provenance.h
+gitmodules/netcdf-c/include/ncauth.h
+gitmodules/netcdf-c/include/ncbytes.h
+gitmodules/netcdf-c/include/ncconfigure.h
+gitmodules/netcdf-c/include/nccrc.h
+gitmodules/netcdf-c/include/ncdispatch.h
+gitmodules/netcdf-c/include/ncexternl.h
+gitmodules/netcdf-c/include/nchashmap.h
+gitmodules/netcdf-c/include/nchttp.h
+gitmodules/netcdf-c/include/ncindex.h
+gitmodules/netcdf-c/include/nclist.h
+gitmodules/netcdf-c/include/nclog.h
+gitmodules/netcdf-c/include/ncmodel.h
+gitmodules/netcdf-c/include/ncoffsets.h
+gitmodules/netcdf-c/include/ncpathmgr.h
+gitmodules/netcdf-c/include/ncrc.h
+gitmodules/netcdf-c/include/ncs3sdk.h
+gitmodules/netcdf-c/include/ncuri.h
+gitmodules/netcdf-c/include/ncutf8.h
+gitmodules/netcdf-c/include/ncxml.h
+gitmodules/netcdf-c/include/netcdf.h
+gitmodules/netcdf-c/include/netcdf_aux.h
+gitmodules/netcdf-c/include/netcdf_dispatch.h.in
+gitmodules/netcdf-c/include/netcdf_f.h
+gitmodules/netcdf-c/include/netcdf_filter.h
+gitmodules/netcdf-c/include/netcdf_mem.h
+gitmodules/netcdf-c/include/netcdf_meta.h.in
+gitmodules/netcdf-c/include/onstack.h
+gitmodules/netcdf-c/include/rnd.h
+gitmodules/netcdf-c/libdispatch/datt.c
+gitmodules/netcdf-c/libdispatch/dattget.c
+gitmodules/netcdf-c/libdispatch/dattinq.c
+gitmodules/netcdf-c/libdispatch/dattput.c
+gitmodules/netcdf-c/libdispatch/dauth.c
+gitmodules/netcdf-c/libdispatch/daux.c
+gitmodules/netcdf-c/libdispatch/dcompound.c
+gitmodules/netcdf-c/libdispatch/dcopy.c
+gitmodules/netcdf-c/libdispatch/dcrc64.c
+gitmodules/netcdf-c/libdispatch/ddim.c
+gitmodules/netcdf-c/libdispatch/ddispatch.c
+gitmodules/netcdf-c/libdispatch/denum.c
+gitmodules/netcdf-c/libdispatch/derror.c
+gitmodules/netcdf-c/libdispatch/dfile.c
+gitmodules/netcdf-c/libdispatch/dfilter.c
+gitmodules/netcdf-c/libdispatch/dgroup.c
+gitmodules/netcdf-c/libdispatch/dinfermodel.c
+gitmodules/netcdf-c/libdispatch/dinstance.c
+gitmodules/netcdf-c/libdispatch/dinstance_intern.c
+gitmodules/netcdf-c/libdispatch/dmissing.c
+gitmodules/netcdf-c/libdispatch/dnotnc4.c
+gitmodules/netcdf-c/libdispatch/doffsets.c
+gitmodules/netcdf-c/libdispatch/dopaque.c
+gitmodules/netcdf-c/libdispatch/dpathmgr.c
+gitmodules/netcdf-c/libdispatch/drc.c
+gitmodules/netcdf-c/libdispatch/ds3util.c
+gitmodules/netcdf-c/libdispatch/dstring.c
+gitmodules/netcdf-c/libdispatch/dtype.c
+gitmodules/netcdf-c/libdispatch/dutf8.c
+gitmodules/netcdf-c/libdispatch/dutil.c
+gitmodules/netcdf-c/libdispatch/dvar.c
+gitmodules/netcdf-c/libdispatch/dvarget.c
+gitmodules/netcdf-c/libdispatch/dvarinq.c
+gitmodules/netcdf-c/libdispatch/dvarput.c
+gitmodules/netcdf-c/libdispatch/dvlen.c
+gitmodules/netcdf-c/libdispatch/nc.c
+gitmodules/netcdf-c/libdispatch/ncbytes.c
+gitmodules/netcdf-c/libdispatch/nchashmap.c
+gitmodules/netcdf-c/libdispatch/nclist.c
+gitmodules/netcdf-c/libdispatch/nclistmgr.c
+gitmodules/netcdf-c/libdispatch/nclog.c
+gitmodules/netcdf-c/libdispatch/ncuri.c
+gitmodules/netcdf-c/libdispatch/utf8proc.c
+gitmodules/netcdf-c/libdispatch/utf8proc.h
+gitmodules/netcdf-c/libdispatch/utf8proc_data.c
+gitmodules/netcdf-c/liblib/nc_initialize.c
+gitmodules/netcdf-c/libsrc/attr.m4
+gitmodules/netcdf-c/libsrc/dim.c
+gitmodules/netcdf-c/libsrc/memio.c
+gitmodules/netcdf-c/libsrc/nc3dispatch.c
+gitmodules/netcdf-c/libsrc/nc3internal.c
+gitmodules/netcdf-c/libsrc/ncio.c
+gitmodules/netcdf-c/libsrc/ncio.h
+gitmodules/netcdf-c/libsrc/ncx.h
+gitmodules/netcdf-c/libsrc/ncx.m4
+gitmodules/netcdf-c/libsrc/posixio.c
+gitmodules/netcdf-c/libsrc/putget.m4
+gitmodules/netcdf-c/libsrc/v1hpg.c
+gitmodules/netcdf-c/libsrc/var.c
+gitmodules/netcdf-c/libsrc4/nc4cache.c
+gitmodules/netcdf-c/libsrc4/nc4dispatch.c
+gitmodules/netcdf-c/libsrc4/nc4grp.c
+gitmodules/netcdf-c/libsrc4/nc4internal.c
+gitmodules/netcdf-c/libsrc4/nc4type.c
+gitmodules/netcdf-c/libsrc4/nc4var.c
+gitmodules/netcdf-c/libsrc4/ncindex.c
+gitmodules/netcdf-fortran/COPYRIGHT
+gitmodules/netcdf-fortran/CMakeExtras/MatchNetCDFFortranTypes.cmake
+gitmodules/netcdf-fortran/fortran/module_netcdf4_nc_interfaces.F90
+gitmodules/netcdf-fortran/fortran/module_netcdf4_nf_interfaces.F90
+gitmodules/netcdf-fortran/fortran/module_netcdf_nc_data.F90
+gitmodules/netcdf-fortran/fortran/module_netcdf_nc_interfaces.F90
+gitmodules/netcdf-fortran/fortran/module_netcdf_nf_data.F90
+gitmodules/netcdf-fortran/fortran/module_netcdf_nf_interfaces.F90
+gitmodules/netcdf-fortran/fortran/netcdf4.F90
+gitmodules/netcdf-fortran/fortran/netcdf4_eightbyte.F90
+gitmodules/netcdf-fortran/fortran/netcdf4_externals.F90
+gitmodules/netcdf-fortran/fortran/netcdf4_file.F90
+gitmodules/netcdf-fortran/fortran/netcdf4_func.F90
+gitmodules/netcdf-fortran/fortran/netcdf4_overloads.F90
+gitmodules/netcdf-fortran/fortran/netcdf4_variables.F90
+gitmodules/netcdf-fortran/fortran/netcdf4_visibility.F90
+gitmodules/netcdf-fortran/fortran/netcdf_attributes.F90
+gitmodules/netcdf-fortran/fortran/netcdf_constants.F90
+gitmodules/netcdf-fortran/fortran/netcdf_dims.F90
+gitmodules/netcdf-fortran/fortran/netcdf_expanded.F90
+gitmodules/netcdf-fortran/fortran/netcdf_externals.F90
+gitmodules/netcdf-fortran/fortran/netcdf_file.F90
+gitmodules/netcdf-fortran/fortran/netcdf_overloads.F90
+gitmodules/netcdf-fortran/fortran/netcdf_text_variables.F90
+gitmodules/netcdf-fortran/fortran/netcdf_variables.F90
+gitmodules/netcdf-fortran/fortran/netcdf_visibility.F90
+gitmodules/netcdf-fortran/fortran/nf_attio.F90
+gitmodules/netcdf-fortran/fortran/nf_control.F90
+gitmodules/netcdf-fortran/fortran/nf_dim.F90
+gitmodules/netcdf-fortran/fortran/nf_genatt.F90
+gitmodules/netcdf-fortran/fortran/nf_geninq.F90
+gitmodules/netcdf-fortran/fortran/nf_genvar.F90
+gitmodules/netcdf-fortran/fortran/nf_lib.c
+gitmodules/netcdf-fortran/fortran/nf_misc.F90
+gitmodules/netcdf-fortran/fortran/nf_nc4.F90
+gitmodules/netcdf-fortran/fortran/nf_nc_noparallel.F90
+gitmodules/netcdf-fortran/fortran/nf_var1io.F90
+gitmodules/netcdf-fortran/fortran/nf_varaio.F90
+gitmodules/netcdf-fortran/fortran/nf_varmio.F90
+gitmodules/netcdf-fortran/fortran/nf_varsio.F90
+gitmodules/netcdf-fortran/fortran/typeSizes.F90
+gitmodules/partmc/COPYING
 gitmodules/partmc/src/aero_binned.F90
 gitmodules/partmc/src/aero_data.F90
 gitmodules/partmc/src/aero_dist.F90
 gitmodules/partmc/src/aero_info.F90
 gitmodules/partmc/src/aero_info_array.F90
 gitmodules/partmc/src/aero_mode.F90
 gitmodules/partmc/src/aero_particle.F90
@@ -327,14 +479,15 @@
 gitmodules/partmc/src/scenario.F90
 gitmodules/partmc/src/sort.c
 gitmodules/partmc/src/spec_file.F90
 gitmodules/partmc/src/spec_line.F90
 gitmodules/partmc/src/stats.F90
 gitmodules/partmc/src/util.F90
 gitmodules/pybind11/CMakeLists.txt
+gitmodules/pybind11/LICENSE
 gitmodules/pybind11/include/pybind11/attr.h
 gitmodules/pybind11/include/pybind11/buffer_info.h
 gitmodules/pybind11/include/pybind11/cast.h
 gitmodules/pybind11/include/pybind11/chrono.h
 gitmodules/pybind11/include/pybind11/common.h
 gitmodules/pybind11/include/pybind11/complex.h
 gitmodules/pybind11/include/pybind11/eigen.h
@@ -358,17 +511,21 @@
 gitmodules/pybind11/include/pybind11/detail/type_caster_base.h
 gitmodules/pybind11/include/pybind11/detail/typeid.h
 gitmodules/pybind11/include/pybind11/stl/filesystem.h
 gitmodules/pybind11/tools/FindPythonLibsNew.cmake
 gitmodules/pybind11/tools/pybind11Common.cmake
 gitmodules/pybind11/tools/pybind11Tools.cmake
 gitmodules/pybind11_json/include/pybind11_json/pybind11_json.hpp
+gitmodules/span/LICENSE_1_0.txt
 gitmodules/span/include/tcb/span.hpp
+gitmodules/string_view-standalone/LICENSE
 gitmodules/string_view-standalone/include/bpstd/string_view.hpp
 gitmodules/string_view-standalone/include/bpstd/detail/string_view.inl
+gitmodules/sundials/CMakeLists.txt
+gitmodules/sundials/LICENSE
 gitmodules/sundials/cmake/SundialsIndexSize.cmake
 gitmodules/sundials/cmake/SundialsSetupCompilers.cmake
 gitmodules/sundials/cmake/SundialsSetupConfig.cmake
 gitmodules/sundials/include/cvode/cvode.h
 gitmodules/sundials/include/cvode/cvode_bandpre.h
 gitmodules/sundials/include/cvode/cvode_bbdpre.h
 gitmodules/sundials/include/cvode/cvode_diag.h
@@ -601,24 +758,25 @@
 src/camp_core.F90
 src/camp_core.hpp
 src/condense.F90
 src/condense.cpp
 src/condense.hpp
 src/env_state.F90
 src/env_state.hpp
-src/fake_netcdf.F90
-src/fake_netcdf.cpp
 src/fake_spec_file.F90
 src/fake_spec_file.cpp
 src/gas_data.F90
 src/gas_data.hpp
 src/gas_state.F90
 src/gas_state.hpp
 src/gimmicks.cpp
 src/gimmicks.hpp
+src/output.F90
+src/output.cpp
+src/output.hpp
 src/photolysis.F90
 src/photolysis.hpp
 src/pmc_resource.hpp
 src/pypartmc.cpp
 src/rand.F90
 src/rand.cpp
 src/rand.hpp
@@ -645,14 +803,15 @@
 tests/test_bin_grid.py
 tests/test_condense.py
 tests/test_dtors.py
 tests/test_env_state.py
 tests/test_gas_data.py
 tests/test_gas_state.py
 tests/test_loss_rate.py
+tests/test_output.py
 tests/test_rand.py
 tests/test_run_part.py
 tests/test_run_part_opt.py
 tests/test_scenario.py
 tests/test_units.py
 tests/test_util.py
 tests/test_version.py
```

### Comparing `PyPartMC-0.2.0/README.md` & `PyPartMC-0.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 - ships with [a set of examples](https://github.com/open-atmos/PyPartMC/tree/main/examples) maintained in a form of Jupyter notebooks
 - Pythonic API (but retaining PartMC jargon) incl. Python GC deallocation of Fortran objects
 - specification of parameters using native Python datatypes (lists, dicts) in place of PartMC spec files
 - code snippets in README depicting how to use PyPartMC from Julia (also executed on CI)
 - auto-generated [API docs on the web](https://open-atmos.github.io/PyPartMC/)
 - support for [de]serialization of selected wrapped structures using JSON 
 - based on [unmodified PartMC code](https://github.com/open-atmos/PyPartMC/tree/main/gitmodules)
-- does not use or require shell or netCDF Fortran library
+- does not use or require shell or any pre-installed libraries
 - aiming at 100% [unit test coverage](https://github.com/open-atmos/PyPartMC/tree/main/tests)
 
 ## Usage examples
 
 #### example object instantiation in Python
 
 ```python
@@ -81,31 +81,77 @@
 PyPartMC is used within the [test workflow of the PySDM project](https://github.com/atmos-cloud-sim-uj/PySDM/tree/main/tests/smoke_tests/partmc).
 
 ## Implementation outline
 
 - PyPartMC is written in C++, Fortran and uses [pybind11](https://pybind11.readthedocs.io/en/stable/) and [CMake](https://cmake.org/).
 - JSON support is handled with [nlohmann::json](https://github.com/nlohmann/json) and [pybind11_json](https://github.com/pybind/pybind11_json)
 - PartMC and selected parts of SUNDIALS are statically linked (and compiled in during `pip install` or `python -m build`) 
-- C (SUNDIALS), C++ (pybind11, ...) and Fortran (PartMC, CAMP) dependencies are linked through [git submodules](https://github.com/open-atmos/PyPartMC/blob/main/.gitmodules)
-- MOSAIC dependency is optionally linked through setting the environmental variable MOSAIC_HOME
-- a [mock of Fortran netCDF API](https://github.com/open-atmos/PyPartMC/blob/main/src/fake_netcdf.F90) and a [mock of PartMC spec file API](https://github.com/open-atmos/PyPartMC/blob/main/src/fake_spec_file.F90) are used for i/o from/to JSON 
+- C (SUNDIALS, netCDF), C++ (pybind11, ...) and Fortran (PartMC, CAMP, netCDF-fortran) dependencies are linked through [git submodules](https://github.com/open-atmos/PyPartMC/blob/main/.gitmodules)
+- MOSAIC dependency is optionally linked through setting the environmental variable `MOSAIC_HOME`
+- a [drop-in replacement of the PartMC spec file routines](https://github.com/open-atmos/PyPartMC/blob/main/src/fake_spec_file.F90) is used for i/o from/to JSON 
+
+## Implementation architecture
+
+```mermaid
+flowchart TD
+    subgraph J ["Julia"]
+        julia_user_code["Julia user code"] --> PyCall.jl
+    end
+    subgraph P ["Python"]
+        PyCall.jl --> PyPartMC
+        python_user_code -.-> NumPy
+        python_user_code["Python user code"] ---> PyPartMC["pubind11-generated PyPartMC module"]
+    end
+    subgraph Cpp ["C++"]
+        cpp_user_code["C++ user code"] ----> ppmc_cpp
+        PyPartMC --> ppmc_cpp["PyPartMC-C++"]
+        ppmc_cpp --> pybind11_json
+        pybind11_json ---> nlohmann::JSON
+        fake_spec_file_cpp --> nlohmann::JSON
+    end
+    subgraph C ["C"]
+        fake_spec_file_c --> fake_spec_file_cpp["SpecFile-C++"]
+        ppmc_cpp --> ppmc_c["PyPartMC-C"]
+        netCDF-C
+        SUNDIALS
+        camp_c["CAMP C code"]
+    end
+    subgraph Fortran ["Fortran"]
+        PartMC -....-> MOSAIC
+        ppmc_c --> ppmc_f["PyPartMC-F"]
+        ppmc_f ---> PartMC
+        PartMC --> netCDF-F
+        netCDF-F --> netCDF-C
+        PartMC --> SUNDIALS
+        PartMC ---> camp_f
+        camp_f["CAMP"] --> camp_c
+        PartMC ----> fake_spec_file_f[SpecFile-F]
+        fake_spec_file_f --> fake_spec_file_c["SpecFile-C"]
+    end
+
+    style PartMC fill:#7ae7ff,stroke-width:2px,color:#2B2B2B
+```
 
 ## Troubleshooting 
 
 #### Common installation issues 
 ```
 error: [Errno 2] No such file or directory: 'cmake'
 ```
-Try rerunning after installing CMake (e.g., `apt-get install cmake` or `brew install cmake`)
+Try rerunning after installing CMake, e.g., using `apt-get install cmake` (Ubuntu/Debian), `brew install cmake` (homebrew on macOS) or using [MSYS2](https://www.msys2.org/docs/cmake/) on Windows.
 
 ```
 No CMAKE_Fortran_COMPILER could be found.
 ```
-Try installing a Fortran compiler (e.g., `brew reinstall gcc`)
+Try installing a Fortran compiler (e.g., `brew reinstall gcc` with Homebrew on macOS or using [MSYS2](https://packages.msys2.org/package/mingw-w64-x86_64-gcc-fortran?repo=mingw64) on Windows).
 
+```
+Could not find NC_M4 using the following names: m4, m4.exe
+```
+Try installing `m4` (e.g., using [MSYS2](https://packages.msys2.org/package/m4?repo=msys&variant=x86_64) on Windows).
 
 ## Notes for developers
 #### How to debug
 ```sh
 git clone --recursive git+https://github.com/open-atmos/PyPartMC.git
 cd PyPartMC
 DEBUG=1 VERBOSE=1 pip --verbose install -e .
```

### Comparing `PyPartMC-0.2.0/examples/hello_world.ipynb` & `PyPartMC-0.3.0/examples/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/examples/lognorm_ex.ipynb` & `PyPartMC-0.3.0/examples/lognorm_ex.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/examples/particle_simulation.ipynb` & `PyPartMC-0.3.0/examples/particle_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/examples/terminal_velocities.ipynb` & `PyPartMC-0.3.0/examples/terminal_velocities.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/examples/widgets_playground.ipynb` & `PyPartMC-0.3.0/examples/widgets_playground.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Include/amd.h` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Include/amd.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Include/amd_internal.h` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Include/amd_internal.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd.f` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd.f`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_1.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_1.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_2.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_2.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_aat.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_aat.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_control.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_control.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_defaults.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_dump.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_dump.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_global.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_global.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_info.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_info.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_order.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_order.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_post_tree.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_postorder.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_preprocess.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amd_valid.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amd_valid.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/AMD/Source/amdbar.f` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/AMD/Source/amdbar.f`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Include/btf.h` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Include/btf.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Include/btf_internal.h` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Include/btf_internal.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Source/btf_maxtrans.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Source/btf_maxtrans.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Source/btf_order.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Source/btf_order.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/BTF/Source/btf_strongcomp.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/BTF/Source/btf_strongcomp.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/COLAMD/Include/colamd.h` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/COLAMD/Include/colamd.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/COLAMD/Source/colamd.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/COLAMD/Source/colamd.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Include/klu.h` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Include/klu.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Include/klu_internal.h` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Include/klu_internal.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Include/klu_version.h` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Include/klu_version.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_analyze.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_analyze.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_analyze_given.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_analyze_given.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_defaults.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_defaults.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_diagnostics.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_diagnostics.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_dump.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_dump.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_extract.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_extract.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_factor.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_factor.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_free_numeric.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_free_numeric.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_free_symbolic.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_free_symbolic.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_kernel.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_kernel.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_memory.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_memory.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_refactor.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_refactor.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_scale.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_scale.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_solve.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_solve.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_sort.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_sort.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/KLU/Source/klu_tsolve.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/KLU/Source/klu_tsolve.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h` & `PyPartMC-0.3.0/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/Jacobian.c` & `PyPartMC-0.3.0/gitmodules/camp/src/Jacobian.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/Jacobian.h` & `PyPartMC-0.3.0/gitmodules/camp/src/Jacobian.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_phase_data.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_phase_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_phase_solver.c` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_phase_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_phase_solver.h` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_phase_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_rep_data.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_rep_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_rep_factory.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_rep_factory.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_rep_solver.c` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_rep_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_rep_solver.h` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_rep_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.c` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_reps/aero_rep_single_particle.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_reps/aero_rep_single_particle.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_reps/aero_rep_single_particle.c` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_reps/aero_rep_single_particle.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/aero_reps.h` & `PyPartMC-0.3.0/gitmodules/camp/src/aero_reps.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/camp_common.h` & `PyPartMC-0.3.0/gitmodules/camp/src/camp_common.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/camp_core.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/camp_core.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/camp_debug.h` & `PyPartMC-0.3.0/gitmodules/camp/src/camp_debug.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/camp_solver.c` & `PyPartMC-0.3.0/gitmodules/camp/src/camp_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/camp_solver.h` & `PyPartMC-0.3.0/gitmodules/camp/src/camp_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/camp_solver_data.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/camp_solver_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/camp_state.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/camp_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/chem_spec_data.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/chem_spec_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/constants.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/constants.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/debug_diff_check.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/debug_diff_check.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/debug_diff_check.c` & `PyPartMC-0.3.0/gitmodules/camp/src/debug_diff_check.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/debug_diff_check.h` & `PyPartMC-0.3.0/gitmodules/camp/src/debug_diff_check.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/env_state.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/env_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/mechanism_data.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/mechanism_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/mpi.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/mpi.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/property.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/property.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rand.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rand.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rand_gsl.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rand_gsl.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxn_data.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxn_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxn_factory.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxn_factory.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxn_solver.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxn_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxn_solver.h` & `PyPartMC-0.3.0/gitmodules/camp/src/rxn_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_arrhenius.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_arrhenius.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_arrhenius.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_arrhenius.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_emission.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_emission.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_emission.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_emission.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_first_order_loss.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_first_order_loss.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_first_order_loss.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_first_order_loss.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_photolysis.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_photolysis.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_photolysis.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_photolysis.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_troe.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_troe.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_troe.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_troe.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wet_deposition.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wet_deposition.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns/rxn_wet_deposition.c` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns/rxn_wet_deposition.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/rxns.h` & `PyPartMC-0.3.0/gitmodules/camp/src/rxns.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/solver_stats.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/solver_stats.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_model_data.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_model_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_model_factory.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_model_factory.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_model_solver.c` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_model_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_model_solver.h` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_model_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_PDFiTE.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_PDFiTE.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_PDFiTE.c` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_PDFiTE.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_UNIFAC.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_UNIFAC.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_UNIFAC.c` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_UNIFAC.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.c` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/sub_models.h` & `PyPartMC-0.3.0/gitmodules/camp/src/sub_models.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/time_derivative.c` & `PyPartMC-0.3.0/gitmodules/camp/src/time_derivative.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/time_derivative.h` & `PyPartMC-0.3.0/gitmodules/camp/src/time_derivative.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/util.F90` & `PyPartMC-0.3.0/gitmodules/camp/src/util.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/camp/src/util.h` & `PyPartMC-0.3.0/gitmodules/camp/src/util.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/adl_serializer.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/adl_serializer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/byte_container_with_subtype.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/byte_container_with_subtype.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/conversions/from_json.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/conversions/from_json.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/conversions/to_chars.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/conversions/to_chars.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/conversions/to_json.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/conversions/to_json.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/exceptions.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/hash.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/hash.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/binary_reader.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/binary_reader.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/input_adapters.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/input_adapters.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/json_sax.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/json_sax.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/lexer.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/lexer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/parser.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/parser.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/input/position_t.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/input/position_t.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/internal_iterator.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/internal_iterator.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/iter_impl.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/iter_impl.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/iteration_proxy.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/iteration_proxy.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/iterator_traits.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/iterator_traits.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/json_reverse_iterator.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/json_reverse_iterator.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/iterators/primitive_iterator.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/iterators/primitive_iterator.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/json_pointer.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/json_pointer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/json_ref.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/json_ref.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/macro_scope.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/macro_scope.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/macro_unscope.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/macro_unscope.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/cpp_future.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/cpp_future.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/detected.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/detected.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/is_sax.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/is_sax.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/meta/type_traits.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/meta/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/output/binary_writer.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/output/binary_writer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/output/output_adapters.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/output/output_adapters.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/output/serializer.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/output/serializer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/string_concat.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/string_concat.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/string_escape.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/string_escape.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/detail/value_t.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/detail/value_t.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/json.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/json_fwd.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/json_fwd.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/ordered_map.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/ordered_map.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp` & `PyPartMC-0.3.0/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_file_module.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_file_module.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_get_scalar_by_path.inc` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_get_scalar_by_path.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_get_vec_by_path.inc` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_get_vec_by_path.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_get_vec_by_path_alloc.inc` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_get_vec_by_path_alloc.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_initialize_arguments.inc` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_initialize_arguments.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_kinds.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_kinds.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_macros.inc` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_macros.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_module.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_module.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_parameters.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_parameters.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_string_utilities.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_string_utilities.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/json_value_module.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/json_value_module.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/introspection/test_iso_10646_support.f90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/introspection/test_iso_10646_support.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_01.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_01.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_02.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_02.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_03.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_03.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_04.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_04.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_05.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_05.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_06.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_06.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_07.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_07.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_08.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_08.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_09.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_09.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_10.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_10.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_11.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_11.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_12.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_12.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_13.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_13.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_14.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_14.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_15.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_15.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_16.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_16.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_17.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_17.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_18.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_18.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_19.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_19.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_20.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_20.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_21.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_21.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_22.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_22.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_23.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_23.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_24.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_24.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_25.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_25.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_26.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_26.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_27.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_27.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_28.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_28.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_29.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_29.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_30.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_30.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_31.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_31.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_32.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_32.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_33.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_33.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_34.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_34.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_35.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_35.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_36.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_36.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_37.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_37.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_38.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_38.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_39.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_39.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_40.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_40.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_41.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_41.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_42.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_42.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_43.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_43.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_44.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_44.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_45.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_45.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_46.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_46.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_47.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_47.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_48.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_48.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/json-fortran/src/tests/jf_test_49.F90` & `PyPartMC-0.3.0/gitmodules/json-fortran/src/tests/jf_test_49.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_binned.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_binned.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_data.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_dist.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_dist.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_info.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_info.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_info_array.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_info_array.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_mode.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_mode.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_particle.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_particle.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_particle_array.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_particle_array.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_sorted.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_sorted.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_state.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_weight.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_weight.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/aero_weight_array.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/aero_weight_array.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/bin_average_comp.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/bin_average_comp.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/bin_average_size.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/bin_average_size.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/bin_grid.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/bin_grid.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/camp_interface.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/camp_interface.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/chamber.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/chamber.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_additive.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_additive.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_brown.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_brown.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_brown_cont.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_brown_cont.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_brown_free.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_brown_free.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_constant.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_constant.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_sedi.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_sedi.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coag_kernel_zero.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coag_kernel_zero.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coagulation.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coagulation.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/coagulation_dist.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/coagulation_dist.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/condense.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/condense.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/condense_solver.c` & `PyPartMC-0.3.0/gitmodules/partmc/src/condense_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/constants.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/constants.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/env_state.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/env_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/exact_soln.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/exact_soln.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/extract_aero_particles.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/extract_aero_particles.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/extract_aero_size.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/extract_aero_size.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/extract_aero_time.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/extract_aero_time.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/extract_env.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/extract_env.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/extract_gas.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/extract_gas.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/extract_sectional_aero_size.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/extract_sectional_aero_size.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/extract_sectional_aero_time.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/extract_sectional_aero_time.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/fractal.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/fractal.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/gas_data.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/gas_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/gas_state.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/gas_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/getopt.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/getopt.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/integer_rmap.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/integer_rmap.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/integer_rmap2.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/integer_rmap2.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/integer_varray.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/integer_varray.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/mosaic.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/mosaic.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/mpi.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/mpi.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/netcdf.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/netcdf.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/nucleate.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/nucleate.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/numeric_average.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/numeric_average.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/numeric_diff.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/numeric_diff.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/output.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/output.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/partmc.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/partmc.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/photolysis.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/photolysis.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/rand.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/rand.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/rand_gsl.c` & `PyPartMC-0.3.0/gitmodules/partmc/src/rand_gsl.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/run_exact.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/run_exact.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/run_part.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/run_part.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/run_sect.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/run_sect.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/scenario.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/scenario.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/sort.c` & `PyPartMC-0.3.0/gitmodules/partmc/src/sort.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/spec_file.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/spec_file.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/spec_line.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/spec_line.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/stats.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/stats.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/partmc/src/util.F90` & `PyPartMC-0.3.0/gitmodules/partmc/src/util.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/attr.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/buffer_info.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/cast.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/chrono.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/complex.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/class.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/common.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/descr.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/init.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/internals.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/type_caster_base.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/detail/typeid.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/eigen.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/embed.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/eval.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/functional.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/gil.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/iostream.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/numpy.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/operators.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/options.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/pybind11.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/pytypes.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/stl/filesystem.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/stl.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/include/pybind11/stl_bind.h` & `PyPartMC-0.3.0/gitmodules/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/tools/FindPythonLibsNew.cmake` & `PyPartMC-0.3.0/gitmodules/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/tools/pybind11Common.cmake` & `PyPartMC-0.3.0/gitmodules/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11/tools/pybind11Tools.cmake` & `PyPartMC-0.3.0/gitmodules/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/pybind11_json/include/pybind11_json/pybind11_json.hpp` & `PyPartMC-0.3.0/gitmodules/pybind11_json/include/pybind11_json/pybind11_json.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/span/include/tcb/span.hpp` & `PyPartMC-0.3.0/gitmodules/span/include/tcb/span.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/string_view-standalone/include/bpstd/detail/string_view.inl` & `PyPartMC-0.3.0/gitmodules/string_view-standalone/include/bpstd/detail/string_view.inl`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/string_view-standalone/include/bpstd/string_view.hpp` & `PyPartMC-0.3.0/gitmodules/string_view-standalone/include/bpstd/string_view.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/cmake/SundialsIndexSize.cmake` & `PyPartMC-0.3.0/gitmodules/sundials/cmake/SundialsIndexSize.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/cmake/SundialsSetupCompilers.cmake` & `PyPartMC-0.3.0/gitmodules/sundials/cmake/SundialsSetupCompilers.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/cmake/SundialsSetupConfig.cmake` & `PyPartMC-0.3.0/gitmodules/sundials/cmake/SundialsSetupConfig.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_bandpre.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_bandpre.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_bbdpre.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_bbdpre.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_diag.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_diag.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_direct.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_direct.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_hypamgpre.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_hypamgpre.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_ls.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_ls.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_proj.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_proj.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/cvode/cvode_spils.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/cvode/cvode_spils.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_cuda.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_cuda.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_hip.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_hip.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_manyvector.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_manyvector.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_mpimanyvector.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_mpimanyvector.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_mpiplusx.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_mpiplusx.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_openmp.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_openmp.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_openmpdev.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_openmpdev.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_parallel.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_parallel.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_parhyp.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_parhyp.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_petsc.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_petsc.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_pthreads.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_pthreads.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_raja.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_raja.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_serial.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_sycl.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_sycl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/nvector_trilinos.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/nvector_trilinos.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorInterface.hpp` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorInterface.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorKernels.hpp` & `PyPartMC-0.3.0/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorKernels.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_band.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_band.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_config.in` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_config.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_cuda_policies.hpp` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_cuda_policies.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_dense.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_direct.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_fconfig.in` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_fconfig.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_fnvector.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_fnvector.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_futils.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_futils.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_hip_policies.hpp` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_hip_policies.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_iterative.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_lapack.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_lapack.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_linearsolver.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_linearsolver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_math.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_math.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_matrix.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_matrix.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_memory.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_memory.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_mpi_types.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_mpi_types.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_nonlinearsolver.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_nonlinearsolver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_nvector.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_nvector_senswrapper.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_nvector_senswrapper.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_sycl_policies.hpp` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_sycl_policies.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_types.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_version.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_version.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sundials/sundials_xbraid.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sundials/sundials_xbraid.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_band.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_band.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_cusolversp_batchqr.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_cusolversp_batchqr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_dense.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_dense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_klu.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_klu.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackband.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackband.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackdense.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackdense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_magmadense.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_magmadense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_onemkldense.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_onemkldense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_pcg.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_pcg.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spbcgs.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spbcgs.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spfgmr.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spfgmr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spgmr.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_spgmr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_sptfqmr.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_superludist.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_superludist.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunlinsol/sunlinsol_superlumt.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunlinsol/sunlinsol_superlumt.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_band.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_band.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_cusparse.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_cusparse.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_dense.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_dense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_magmadense.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_magmadense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_onemkldense.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_onemkldense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_slunrloc.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_slunrloc.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunmatrix/sunmatrix_sparse.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunmatrix/sunmatrix_sparse.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_fixedpoint.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_fixedpoint.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_newton.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_newton.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_petscsnes.h` & `PyPartMC-0.3.0/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_petscsnes.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/CHANGES` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/CHANGES`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/LICENSE` & `PyPartMC-0.3.0/gitmodules/sundials/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/NOTICE` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/NOTICE`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/README.md` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/README.md`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_bandpre.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_bandpre.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_bandpre_impl.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_bbdpre.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_bbdpre.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_bbdpre_impl.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_diag.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_diag.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_diag_impl.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_diag_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_direct.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_direct.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_fused_gpu.cpp` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_fused_gpu.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_fused_stubs.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_fused_stubs.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_hypamgpre.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_hypamgpre.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_hypamgpre_impl.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_hypamgpre_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_impl.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_io.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_io.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_ls.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_ls.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_ls_impl.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_ls_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_nls.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_nls.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_proj.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_proj.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_proj_impl.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_proj_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/cvode_spils.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/cvode_spils.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/Makefile.in` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/Makefile.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvband.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvband.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvbbd.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvbbd.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvbbd.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvbbd.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvbp.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvbp.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvbp.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvbp.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvdense.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvdense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvewt.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvewt.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvjtimes.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvjtimes.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvnulllinsol.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvnulllinsol.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvnullmatrix.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvnullmatrix.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvnullnonlinsol.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvnullnonlinsol.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvode.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvode.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvode.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvode.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvpreco.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvpreco.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvroot.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvroot.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvroot.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvroot.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fcmix/fcvsparse.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fcmix/fcvsparse.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fmod/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fmod/fcvode_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fmod/fcvode_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/cvode/fmod/fcvode_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/cvode/fmod/fcvode_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/nvector/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/nvector/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fmod/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fnvector_serial.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fnvector_serial.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/fnvector_serial.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/fnvector_serial.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/nvector/serial/nvector_serial.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/nvector/serial/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_band.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_band.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_cuda.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_cuda.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_cuda_kernels.cuh` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_cuda_kernels.cuh`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_debug.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_debug.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_dense.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_direct.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_futils.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_futils.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_hip.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_hip.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_hip_kernels.hip.hpp` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_hip_kernels.hip.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_iterative.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_linearsolver.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_linearsolver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_math.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_math.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_matrix.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_matrix.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_memory.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_memory.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_nonlinearsolver.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_nonlinearsolver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_nvector.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_nvector_senswrapper.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_nvector_senswrapper.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_sycl.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_sycl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_version.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_version.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sundials/sundials_xbraid.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sundials/sundials_xbraid.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fmod/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/band/sunlinsol_band.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/band/sunlinsol_band.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fmod/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/dense/sunlinsol_dense.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/dense/sunlinsol_dense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fmod/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/klu/sunlinsol_klu.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/klu/sunlinsol_klu.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/pcg/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/pcg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/pcg/sunlinsol_pcg.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/pcg/sunlinsol_pcg.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spbcgs/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spbcgs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spbcgs/sunlinsol_spbcgs.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spbcgs/sunlinsol_spbcgs.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spfgmr/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spfgmr/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spfgmr/sunlinsol_spfgmr.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spfgmr/sunlinsol_spfgmr.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spgmr/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spgmr/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/spgmr/sunlinsol_spgmr.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/spgmr/sunlinsol_spgmr.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/sptfqmr/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/sptfqmr/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunlinsol/sptfqmr/sunlinsol_sptfqmr.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunlinsol/sptfqmr/sunlinsol_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/band/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/band/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/band/sunmatrix_band.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/band/sunmatrix_band.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/dense/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/dense/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/dense/sunmatrix_dense.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/dense/sunmatrix_dense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/sparse/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/sparse/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunmatrix/sparse/sunmatrix_sparse.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunmatrix/sparse/sunmatrix_sparse.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/sunnonlinsol_fixedpoint.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/fixedpoint/sunnonlinsol_fixedpoint.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/CMakeLists.txt` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.f90` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.h` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/gitmodules/sundials/src/sunnonlinsol/newton/sunnonlinsol_newton.c` & `PyPartMC-0.3.0/gitmodules/sundials/src/sunnonlinsol/newton/sunnonlinsol_newton.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/setup.py` & `PyPartMC-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_data.F90` & `PyPartMC-0.3.0/src/aero_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_data.hpp` & `PyPartMC-0.3.0/src/aero_data.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_dist.F90` & `PyPartMC-0.3.0/src/aero_dist.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_dist.hpp` & `PyPartMC-0.3.0/src/aero_dist.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_mode.F90` & `PyPartMC-0.3.0/src/aero_mode.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_mode.hpp` & `PyPartMC-0.3.0/src/aero_mode.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_particle.F90` & `PyPartMC-0.3.0/src/aero_particle.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_particle.hpp` & `PyPartMC-0.3.0/src/aero_particle.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_state.F90` & `PyPartMC-0.3.0/src/aero_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/aero_state.hpp` & `PyPartMC-0.3.0/src/aero_state.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/bin_grid.F90` & `PyPartMC-0.3.0/src/bin_grid.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/bin_grid.cpp` & `PyPartMC-0.3.0/src/bin_grid.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/bin_grid.hpp` & `PyPartMC-0.3.0/src/bin_grid.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/camp_core.F90` & `PyPartMC-0.3.0/src/camp_core.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/camp_core.hpp` & `PyPartMC-0.3.0/src/camp_core.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/condense.F90` & `PyPartMC-0.3.0/src/condense.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/condense.cpp` & `PyPartMC-0.3.0/src/condense.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/condense.hpp` & `PyPartMC-0.3.0/src/condense.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/env_state.F90` & `PyPartMC-0.3.0/src/env_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/env_state.hpp` & `PyPartMC-0.3.0/src/env_state.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/fake_spec_file.F90` & `PyPartMC-0.3.0/src/fake_spec_file.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/fake_spec_file.cpp` & `PyPartMC-0.3.0/src/fake_spec_file.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/gas_data.F90` & `PyPartMC-0.3.0/src/gas_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/gas_data.hpp` & `PyPartMC-0.3.0/src/gas_data.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/gas_state.F90` & `PyPartMC-0.3.0/src/gas_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/gas_state.hpp` & `PyPartMC-0.3.0/src/gas_state.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/gimmicks.cpp` & `PyPartMC-0.3.0/src/gimmicks.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/gimmicks.hpp` & `PyPartMC-0.3.0/src/gimmicks.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/photolysis.F90` & `PyPartMC-0.3.0/src/photolysis.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/photolysis.hpp` & `PyPartMC-0.3.0/src/photolysis.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/pmc_resource.hpp` & `PyPartMC-0.3.0/src/pmc_resource.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/pypartmc.cpp` & `PyPartMC-0.3.0/src/pypartmc.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #include "env_state.hpp"
 #include "gas_data.hpp"
 #include "gas_state.hpp"
 #include "condense.hpp"
 #include "bin_grid.hpp"
 #include "camp_core.hpp"
 #include "photolysis.hpp"
+#include "output.hpp"
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
 
 namespace py = pybind11;
 
 PYBIND11_MODULE(_PyPartMC, m) {
@@ -414,14 +415,22 @@
 
     m.def(
         "loss_rate", &loss_rate, py::return_value_policy::copy,
         "Evaluate a loss rate function."
     );
 
     m.def(
+        "output_state", &output_state, "Output current state to netCDF file."
+    );
+
+    m.def(
+        "input_state", &input_state, "Read current state from netCDF output file."
+    );
+
+    m.def(
         "rand_init", &rand_init, "Initializes the random number generator to the state defined by the given seed plus offset. If the seed is 0 then a seed is auto-generated from the current time plus offset"
     );
 
     m.def(
         "rand_normal", &rand_normal, "Generates a normally distributed random number with the given mean and standard deviation"
     );
 
@@ -452,11 +461,13 @@
         "histogram_2d",
         "sphere_vol2rad",
         "rad2diam",
         "sphere_rad2vol",
         "diam2rad",
         "loss_rate_dry_dep",
         "loss_rate",
+        "output_state",
+        "input_state",
         "rand_init",
         "rand_normal"
     );
 }
```

### Comparing `PyPartMC-0.2.0/src/rand.F90` & `PyPartMC-0.3.0/src/rand.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/rand.cpp` & `PyPartMC-0.3.0/src/rand.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/rand.hpp` & `PyPartMC-0.3.0/src/rand.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/run_part.F90` & `PyPartMC-0.3.0/src/run_part.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/run_part.cpp` & `PyPartMC-0.3.0/src/run_part.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/run_part.hpp` & `PyPartMC-0.3.0/src/run_part.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/run_part_opt.F90` & `PyPartMC-0.3.0/src/run_part_opt.F90`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         type(run_part_opt_t), pointer :: run_part_opt => null()
         type(c_ptr), intent(in) :: ptr_c
         type(spec_file_t) :: file
         integer(c_int) :: rand_init
 
         call c_f_pointer(ptr_c, run_part_opt)
 
+        call spec_file_read_string(file, 'output_prefix', &
+             run_part_opt%output_prefix)
+
         !!! TODO #55
         call spec_file_read_logical(file, 'do_coagulation', run_part_opt%do_coagulation)    
         if (run_part_opt%do_coagulation) then
            call spec_file_read_coag_kernel_type(file, &
                 run_part_opt%coag_kernel_type)
         else
            run_part_opt%coag_kernel_type = COAG_KERNEL_TYPE_INVALID
@@ -117,14 +120,20 @@
        call spec_file_read_logical(file, 'allow_doubling', run_part_opt%allow_doubling)
        call spec_file_read_logical(file, 'allow_halving', run_part_opt%allow_halving)
 
        call spec_file_read_logical(file, 'do_camp_chem', run_part_opt%do_camp_chem)
 
        run_part_opt%output_type = OUTPUT_TYPE_SINGLE
 
+       run_part_opt%i_repeat = 1
+       run_part_opt%n_repeat = 1
+
+       call pmc_srand(0, 0)
+       call uuid4_str(run_part_opt%uuid)
+
        call pmc_srand(rand_init, 0)
 
     end subroutine
 
     subroutine f_run_part_opt_t_max(ptr_c, t_max) bind(C)
         type(run_part_opt_t), pointer :: ptr_f => null()
         type(c_ptr), intent(in) :: ptr_c
```

### Comparing `PyPartMC-0.2.0/src/run_part_opt.hpp` & `PyPartMC-0.3.0/src/run_part_opt.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/scenario.F90` & `PyPartMC-0.3.0/src/scenario.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/scenario.cpp` & `PyPartMC-0.3.0/src/scenario.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/scenario.hpp` & `PyPartMC-0.3.0/src/scenario.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/sys.F90` & `PyPartMC-0.3.0/src/sys.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/sys.cpp` & `PyPartMC-0.3.0/src/sys.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/util.F90` & `PyPartMC-0.3.0/src/util.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/util.cpp` & `PyPartMC-0.3.0/src/util.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/src/util.hpp` & `PyPartMC-0.3.0/src/util.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_aero_data.py` & `PyPartMC-0.3.0/tests/test_aero_data.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_aero_dist.py` & `PyPartMC-0.3.0/tests/test_aero_dist.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,32 @@
 
 import numpy as np
 import pytest
 
 import PyPartMC as ppmc
 
 from .test_aero_data import AERO_DATA_CTOR_ARG_MINIMAL
-from .test_aero_mode import AERO_MODE_CTOR_LOG_NORMAL, AERO_MODE_CTOR_LOG_NORMAL_FULL
+from .test_aero_mode import (
+    AERO_MODE_CTOR_LOG_NORMAL,
+    AERO_MODE_CTOR_LOG_NORMAL_COAGULATION,
+    AERO_MODE_CTOR_LOG_NORMAL_FULL,
+)
 
 AERO_DIST_CTOR_ARG_MINIMAL = [
     AERO_MODE_CTOR_LOG_NORMAL,
 ]
 
 AERO_DIST_CTOR_ARG_FULL = [
     AERO_MODE_CTOR_LOG_NORMAL_FULL,
 ]
 
+AERO_DIST_CTOR_ARG_COAGULATION = [
+    AERO_MODE_CTOR_LOG_NORMAL_COAGULATION,
+]
+
 
 @pytest.fixture
 def sut_minimal():
     aero_data = ppmc.AeroData(AERO_DATA_CTOR_ARG_MINIMAL)
     sut = ppmc.AeroDist(aero_data, AERO_DIST_CTOR_ARG_MINIMAL)
     aero_data = None
     gc.collect()
```

### Comparing `PyPartMC-0.2.0/tests/test_aero_mode.py` & `PyPartMC-0.3.0/tests/test_aero_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,25 @@
         "mode_type": "log_normal",
         "num_conc": 100 / si.m**3,
         "geom_mean_diam": 2 * si.um,
         "log10_geom_std_dev": np.log10(1.6),
     }
 }
 
+AERO_MODE_CTOR_LOG_NORMAL_COAGULATION = {
+    "test_mode": {
+        "mass_frac": [{"SO4": [1]}],
+        "diam_type": "geometric",
+        "mode_type": "log_normal",
+        "num_conc": 1e12 / si.m**3,
+        "geom_mean_diam": 2 * si.um,
+        "log10_geom_std_dev": np.log10(1.6),
+    }
+}
+
 
 class TestAeroMode:
     @staticmethod
     def test_ctor():
         # arrange
         aero_data = ppmc.AeroData(AERO_DATA_CTOR_ARG_MINIMAL)
```

### Comparing `PyPartMC-0.2.0/tests/test_aero_particle.py` & `PyPartMC-0.3.0/tests/test_aero_particle.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_aero_state.py` & `PyPartMC-0.3.0/tests/test_aero_state.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_bin_grid.py` & `PyPartMC-0.3.0/tests/test_bin_grid.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_condense.py` & `PyPartMC-0.3.0/tests/test_condense.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_dtors.py` & `PyPartMC-0.3.0/tests/test_dtors.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_env_state.py` & `PyPartMC-0.3.0/tests/test_env_state.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_gas_data.py` & `PyPartMC-0.3.0/tests/test_gas_data.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_gas_state.py` & `PyPartMC-0.3.0/tests/test_gas_state.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_loss_rate.py` & `PyPartMC-0.3.0/tests/test_loss_rate.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_rand.py` & `PyPartMC-0.3.0/tests/test_rand.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_run_part.py` & `PyPartMC-0.3.0/tests/test_run_part.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_run_part_opt.py` & `PyPartMC-0.3.0/tests/test_run_part_opt.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import pytest
 
 import PyPartMC as ppmc
 from PyPartMC import si
 
 RUN_PART_OPT_CTOR_ARG_MINIMAL = {
+    "output_prefix": "tests/test",
     "do_coagulation": False,
     "do_parallel": False,
     "do_nucleation": False,
     "do_mosaic": False,
     "do_optical": False,
     "do_condensation": False,
     "do_camp_chem": False,
@@ -24,14 +25,33 @@
     "t_output": 0,
     "t_progress": 0,
     "rand_init": 0,
     "allow_halving": False,
     "allow_doubling": False,
 }
 
+RUN_PART_OPT_CTOR_ARG_SIMULATION = {
+    "output_prefix": "tests/test",
+    "do_coagulation": True,
+    "coag_kernel": "brown",
+    "do_parallel": False,
+    "do_nucleation": False,
+    "do_mosaic": False,
+    "do_optical": False,
+    "do_condensation": False,
+    "do_camp_chem": False,
+    "t_max": 86400.0,
+    "del_t": 60 * si.s,
+    "t_output": 3600.0,
+    "t_progress": 0.0,
+    "rand_init": 0,
+    "allow_halving": False,
+    "allow_doubling": False,
+}
+
 
 class TestRunPartOpt:
     @staticmethod
     @pytest.mark.parametrize("ctor_arg", (RUN_PART_OPT_CTOR_ARG_MINIMAL,))
     def test_ctor(ctor_arg):
         # arrange
         pass
```

### Comparing `PyPartMC-0.2.0/tests/test_scenario.py` & `PyPartMC-0.3.0/tests/test_scenario.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,33 @@
         {"time": [0]},
         {"rate": [0]},
         {"dist": [[AERO_MODE_CTOR_LOG_NORMAL]]},
     ],
     "loss_function": "none",
 }
 
+SCENARIO_CTOR_ARG_SIMULATION = {
+    "temp_profile": [{"time": [0]}, {"temp": [273]}],
+    "pressure_profile": [{"time": [0]}, {"pressure": [1e5]}],
+    "height_profile": [{"time": [0]}, {"height": [1]}],
+    "gas_emissions": [{"time": [0]}, {"rate": [1]}, {"SO2": [1e-9]}],
+    "gas_background": [{"time": [0]}, {"rate": [0]}, {"SO2": [0]}],
+    "aero_emissions": [
+        {"time": [0]},
+        {"rate": [0]},
+        {"dist": [[AERO_MODE_CTOR_LOG_NORMAL]]},
+    ],
+    "aero_background": [
+        {"time": [0]},
+        {"rate": [0]},
+        {"dist": [[AERO_MODE_CTOR_LOG_NORMAL]]},
+    ],
+    "loss_function": "none",
+}
+
 
 class TestScenario:
     @staticmethod
     @pytest.mark.parametrize(
         "params",
         (
             {
```

### Comparing `PyPartMC-0.2.0/tests/test_units.py` & `PyPartMC-0.3.0/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_util.py` & `PyPartMC-0.3.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-0.2.0/tests/test_version.py` & `PyPartMC-0.3.0/tests/test_version.py`

 * *Files identical despite different names*

