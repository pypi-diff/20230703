# Comparing `tmp/irff-1.5.2.tar.gz` & `tmp/irff-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irff-1.5.2.tar", last modified: Fri Mar 31 05:01:30 2023, max compression
+gzip compressed data, was "irff-1.5.3.tar", last modified: Mon Jul  3 14:53:55 2023, max compression
```

## Comparing `irff-1.5.2.tar` & `irff-1.5.3.tar`

### file list

```diff
@@ -1,226 +1,178 @@
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.316149 irff-1.5.2/
--rw-r--r--   0 feng      (1000) feng      (1000)      328 2023-03-31 05:01:30.316149 irff-1.5.2/PKG-INFO
--rw-r--r--   0 feng      (1000) feng      (1000)      958 2023-03-31 04:50:46.000000 irff-1.5.2/README.md
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.296149 irff-1.5.2/irff/
--rw-r--r--   0 feng      (1000) feng      (1000)    48504 2023-03-31 04:50:49.000000 irff-1.5.2/irff/AtomDance.py
--rw-r--r--   0 feng      (1000) feng      (1000)    35628 2023-03-31 04:50:49.000000 irff-1.5.2/irff/LearningMachine.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2861 2023-03-31 04:50:49.000000 irff-1.5.2/irff/RadiusCutOff.py
--rw-r--r--   0 feng      (1000) feng      (1000)        4 2023-03-31 04:50:49.000000 irff-1.5.2/irff/__init__.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.300149 irff-1.5.2/irff/data/
--rw-r--r--   0 feng      (1000) feng      (1000)     2102 2023-03-31 04:51:09.000000 irff-1.5.2/irff/data/ColData.py
--rw-r--r--   0 feng      (1000) feng      (1000)      523 2023-03-31 04:51:09.000000 irff-1.5.2/irff/data/__init__.py
--rw-r--r--   0 feng      (1000) feng      (1000)      439 2023-03-31 04:51:09.000000 irff-1.5.2/irff/data/dpdata.py
--rw-r--r--   0 feng      (1000) feng      (1000)    21065 2023-03-31 04:51:09.000000 irff-1.5.2/irff/data/mdtodata.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3005 2023-03-31 04:51:09.000000 irff-1.5.2/irff/data/prep_data.py
--rw-r--r--   0 feng      (1000) feng      (1000)      726 2023-03-31 04:51:09.000000 irff-1.5.2/irff/data/qeout_to_traj.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.300149 irff-1.5.2/irff/deb/
--rw-r--r--   0 feng      (1000) feng      (1000)      523 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/__init__.py
--rw-r--r--   0 feng      (1000) feng      (1000)     7652 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/compare_energies.py
--rw-r--r--   0 feng      (1000) feng      (1000)    24567 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/deb_bde.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3746 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/hbdeb.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2338 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/ird.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3542 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/irdeb.py
--rw-r--r--   0 feng      (1000) feng      (1000)    27553 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/irffdeb.py
--rw-r--r--   0 feng      (1000) feng      (1000)      696 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/irnan.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4126 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/mpdeb.py
--rw-r--r--   0 feng      (1000) feng      (1000)    30455 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/reax_debug.py
--rw-r--r--   0 feng      (1000) feng      (1000)    28582 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/reax_gulp.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2602 2023-03-31 04:51:09.000000 irff-1.5.2/irff/deb/theta.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.300149 irff-1.5.2/irff/dft/
--rw-r--r--   0 feng      (1000) feng      (1000)     1764 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/CheckEmol.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4168 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/SinglePointEnergy.py
--rw-r--r--   0 feng      (1000) feng      (1000)      523 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/__init__.py
--rw-r--r--   0 feng      (1000) feng      (1000)    16923 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/cpmd.py
--rw-r--r--   0 feng      (1000) feng      (1000)    16974 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/dftb.py
--rw-r--r--   0 feng      (1000) feng      (1000)     9604 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/nwchem.py
--rw-r--r--   0 feng      (1000) feng      (1000)    32655 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/qe.py
--rw-r--r--   0 feng      (1000) feng      (1000)    34877 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/siesta.py
--rw-r--r--   0 feng      (1000) feng      (1000)    22010 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/siesta_zmatix_constrain.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4145 2023-03-31 04:51:06.000000 irff-1.5.2/irff/dft/smd_server.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1712 2023-03-31 04:50:49.000000 irff-1.5.2/irff/dingtalk.py
--rw-r--r--   0 feng      (1000) feng      (1000)    32101 2023-03-31 04:50:49.000000 irff-1.5.2/irff/emdk.py
--rw-r--r--   0 feng      (1000) feng      (1000)    44033 2023-03-31 04:50:49.000000 irff-1.5.2/irff/fitbo.py
--rw-r--r--   0 feng      (1000) feng      (1000)   220869 2023-03-31 04:50:49.000000 irff-1.5.2/irff/getNeighbor.c
--rw-r--r--   0 feng      (1000) feng      (1000)     1822 2023-03-31 04:50:48.000000 irff-1.5.2/irff/getNeighbors.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6453 2023-03-31 04:50:48.000000 irff-1.5.2/irff/intCheck.py
--rw-r--r--   0 feng      (1000) feng      (1000)    56289 2023-03-31 04:50:49.000000 irff-1.5.2/irff/irff.py
--rw-r--r--   0 feng      (1000) feng      (1000)    58518 2023-03-31 04:50:49.000000 irff-1.5.2/irff/irff_np.py
--rw-r--r--   0 feng      (1000) feng      (1000)    16472 2023-03-31 04:50:49.000000 irff-1.5.2/irff/link.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.300149 irff-1.5.2/irff/md/
--rw-r--r--   0 feng      (1000) feng      (1000)     4042 2023-03-31 04:51:06.000000 irff-1.5.2/irff/md/ReactionCapture.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3041 2023-03-31 04:51:06.000000 irff-1.5.2/irff/md/__init__.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2360 2023-03-31 04:51:06.000000 irff-1.5.2/irff/md/gofr.py
--rw-r--r--   0 feng      (1000) feng      (1000)    16600 2023-03-31 04:51:06.000000 irff-1.5.2/irff/md/gulp.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4704 2023-03-31 04:51:06.000000 irff-1.5.2/irff/md/hugoniot.py
--rw-r--r--   0 feng      (1000) feng      (1000)    16516 2023-03-31 04:51:06.000000 irff-1.5.2/irff/md/irmd.py
--rw-r--r--   0 feng      (1000) feng      (1000)    19211 2023-03-31 04:51:06.000000 irff-1.5.2/irff/md/lammps.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.304149 irff-1.5.2/irff/ml/
--rw-r--r--   0 feng      (1000) feng      (1000)        3 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/__init__.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6999 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/data.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6505 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/evaluate_data.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6774 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/evolution.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6381 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/ffield.py
--rw-r--r--   0 feng      (1000) feng      (1000)    10951 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/fit.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4110 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/fluctuation.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6011 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/gaqeq.py
--rw-r--r--   0 feng      (1000) feng      (1000)     9327 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/genetic.py
--rw-r--r--   0 feng      (1000) feng      (1000)    11038 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/gpfit_tfv2.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6406 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/harmonic.py
--rw-r--r--   0 feng      (1000) feng      (1000)    10035 2023-03-31 04:51:08.000000 irff-1.5.2/irff/ml/train.py
--rw-r--r--   0 feng      (1000) feng      (1000)    20150 2023-03-31 04:50:49.000000 irff-1.5.2/irff/mlqeq.py
--rw-r--r--   0 feng      (1000) feng      (1000)    14721 2023-03-31 04:50:49.000000 irff-1.5.2/irff/molecule.py
--rw-r--r--   0 feng      (1000) feng      (1000)    65277 2023-03-31 04:50:49.000000 irff-1.5.2/irff/mpnn.py
--rw-r--r--   0 feng      (1000) feng      (1000)   905978 2023-03-31 04:50:49.000000 irff-1.5.2/irff/neighbor.c
--rw-r--r--   0 feng      (1000) feng      (1000)     2987 2023-03-31 04:50:48.000000 irff-1.5.2/irff/neighbors.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.308149 irff-1.5.2/irff/plot/
--rw-r--r--   0 feng      (1000) feng      (1000)     1557 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/BondEnergy.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2152 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/CheckAng.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1608 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/LearningResults.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3477 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/LearningResultsAng.py
--rw-r--r--   0 feng      (1000) feng      (1000)     5896 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/MessagePassing.py
--rw-r--r--   0 feng      (1000) feng      (1000)      185 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/__init__.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1782 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/abc.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2811 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/angel_to_bond.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4040 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/bde.py
--rw-r--r--   0 feng      (1000) feng      (1000)     7652 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/compare_energies.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1766 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/fingerprint.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2360 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/gofr.py
--rw-r--r--   0 feng      (1000) feng      (1000)    18668 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/irnn_plot.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3899 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/label_md.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3813 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/labels.py
--rw-r--r--   0 feng      (1000) feng      (1000)     5155 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/morse.py
--rw-r--r--   0 feng      (1000) feng      (1000)     8837 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/morse_taper.py
--rw-r--r--   0 feng      (1000) feng      (1000)     8460 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/mpbd.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3813 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/mpnn_plbd.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3165 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/nx.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1853 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/pdf.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1120 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plbd.py
--rw-r--r--   0 feng      (1000) feng      (1000)     7085 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plbo.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1831 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/ple.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3406 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plea.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1522 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/pleb.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2451 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/pleo.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1697 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/plev.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1401 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plevdw.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4559 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/plf.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3707 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plot_atoms.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2110 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plot_atoms_matplot.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2391 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/plot_atoms_momenta.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1701 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plot_bond_energy.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1632 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plot_charge.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2454 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/plot_energy.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2183 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plot_eover.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4129 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plot_eover_atom.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2696 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plot_functions.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1358 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/plot_morse.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2543 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/plot_pes.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3304 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/plot_pressure.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2752 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/plot_zmat_pes.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1917 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/plotenergy.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1900 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/plotenergy_bond.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2240 2023-03-31 04:51:07.000000 irff-1.5.2/irff/plot/pltp.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4694 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/reax_plbd.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1821 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/reax_pldd.py
--rw-r--r--   0 feng      (1000) feng      (1000)    18380 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/reax_plot.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4402 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/reax_plov.py
--rw-r--r--   0 feng      (1000) feng      (1000)    24951 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/rffbd.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1199 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/sigmoid.py
--rw-r--r--   0 feng      (1000) feng      (1000)     8207 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/vdw_taper.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3108 2023-03-31 04:51:08.000000 irff-1.5.2/irff/plot/view.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.308149 irff-1.5.2/irff/prop/
--rw-r--r--   0 feng      (1000) feng      (1000)      523 2023-03-31 04:51:09.000000 irff-1.5.2/irff/prop/__init__.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2362 2023-03-31 04:51:09.000000 irff-1.5.2/irff/prop/gofr.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6059 2023-03-31 04:50:49.000000 irff-1.5.2/irff/qeq.py
--rw-r--r--   0 feng      (1000) feng      (1000)   102465 2023-03-31 04:50:49.000000 irff-1.5.2/irff/reax.py
--rw-r--r--   0 feng      (1000) feng      (1000)    33565 2023-03-31 04:50:49.000000 irff-1.5.2/irff/reax_data.py
--rw-r--r--   0 feng      (1000) feng      (1000)    82185 2023-03-31 04:50:48.000000 irff-1.5.2/irff/reax_nn.py
--rw-r--r--   0 feng      (1000) feng      (1000)    27071 2023-03-31 04:50:49.000000 irff-1.5.2/irff/reaxfflib.py
--rw-r--r--   0 feng      (1000) feng      (1000)    11293 2023-03-31 04:50:49.000000 irff-1.5.2/irff/spectra.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.316149 irff-1.5.2/irff/structures/
--rw-r--r--   0 feng      (1000) feng      (1000)      607 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/Al.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1242 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/AlC2F6.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     5293 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/AlO.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      767 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/C2C4.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      923 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/C2C6.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      612 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/C2H2.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      768 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/C2H4.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      924 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/C2H6.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      924 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/C3H5.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1159 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/C3H8.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      768 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/CF.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1237 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/Cline.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1247 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/F2314.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1866 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/FAlF.gen
--rw-r--r--   0 feng      (1000) feng      (1000)    28465 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/FLZ.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1866 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/Fluoro.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      534 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/H2O.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     4679 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/HMX.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     2495 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/HMX_MOL.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     4045 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/ICE.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     2495 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/NM.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     5142 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/Polytetrafluoro_ethylene.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     2651 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/TATB-H2O.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     4055 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/TATB.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     2105 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/TDI.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      434 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/__init__.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2469 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/ball.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2776 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/ball_bulk.py
--rw-r--r--   0 feng      (1000) feng      (1000)     4976 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/c60.gen
--rw-r--r--   0 feng      (1000) feng      (1000)    11544 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/cl20-c.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     3119 2023-03-31 04:51:06.000000 irff-1.5.2/irff/structures/cl20.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      167 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/cnt.py
--rw-r--r--   0 feng      (1000) feng      (1000)      919 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/diamond.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      844 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/diamond.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2749 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/fox7.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      607 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/graphene.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1194 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/graphene.py
--rw-r--r--   0 feng      (1000) feng      (1000)      607 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/graphite.gen
--rw-r--r--   0 feng      (1000) feng      (1000)    15912 2023-03-31 04:51:06.000000 irff-1.5.2/irff/structures/hmx-cl20.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1403 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/nm241.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1949 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/nm3.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     3587 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/nm6.gen
--rw-r--r--   0 feng      (1000) feng      (1000)      856 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/nmmol.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1475 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/pda.cif
--rw-r--r--   0 feng      (1000) feng      (1000)     1559 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/pda.gen
--rw-r--r--   0 feng      (1000) feng      (1000)    34085 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/pda_zhi.cif
--rw-r--r--   0 feng      (1000) feng      (1000)    42588 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/pda_zhi.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     3587 2023-03-31 04:51:06.000000 irff-1.5.2/irff/structures/polyurethane.gen
--rw-r--r--   0 feng      (1000) feng      (1000)     1697 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/tatbModels-1.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1672 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/tatbModels-3.py
--rw-r--r--   0 feng      (1000) feng      (1000)     2183 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/tatbmol.gen
--rw-r--r--   0 feng      (1000) feng      (1000)    17784 2023-03-31 04:51:07.000000 irff-1.5.2/irff/structures/zhi.gen
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.316149 irff-1.5.2/irff/tools/
--rw-r--r--   0 feng      (1000) feng      (1000)      523 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/__init__.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1189 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/eos_opt.py
--rw-r--r--   0 feng      (1000) feng      (1000)      203 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/epstopdf.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1518 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/ffield_to_json.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1422 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/ffieldtolib.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1470 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/fingerprint.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6093 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/fit_hugoniot_state.py
--rw-r--r--   0 feng      (1000) feng      (1000)     9738 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/fitnn.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1259 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/json_to_ffield.py
--rw-r--r--   0 feng      (1000) feng      (1000)     8741 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/morse_taper.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1626 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/pre_opt.py
--rw-r--r--   0 feng      (1000) feng      (1000)     6657 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/prepare_ffield.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1351 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/pressure.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3953 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/pseudo_gen.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3567 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/rsetff.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3328 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/setwb.py
--rw-r--r--   0 feng      (1000) feng      (1000)      728 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/vdw.py
--rw-r--r--   0 feng      (1000) feng      (1000)     1241 2023-03-31 04:51:08.000000 irff-1.5.2/irff/tools/zmat_to_atoms.py
--rw-r--r--   0 feng      (1000) feng      (1000)     9972 2023-03-31 04:50:49.000000 irff-1.5.2/irff/trainer.py
--rw-r--r--   0 feng      (1000) feng      (1000)     3798 2023-03-31 04:50:49.000000 irff-1.5.2/irff/zmatrix.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.296149 irff-1.5.2/irff.egg-info/
--rw-r--r--   0 feng      (1000) feng      (1000)      328 2023-03-31 05:01:30.000000 irff-1.5.2/irff.egg-info/PKG-INFO
--rw-r--r--   0 feng      (1000) feng      (1000)     4727 2023-03-31 05:01:30.000000 irff-1.5.2/irff.egg-info/SOURCES.txt
--rw-r--r--   0 feng      (1000) feng      (1000)        1 2023-03-31 05:01:30.000000 irff-1.5.2/irff.egg-info/dependency_links.txt
--rw-r--r--   0 feng      (1000) feng      (1000)        1 2023-03-31 05:01:30.000000 irff-1.5.2/irff.egg-info/not-zip-safe
--rw-r--r--   0 feng      (1000) feng      (1000)        4 2023-03-31 05:01:30.000000 irff-1.5.2/irff.egg-info/requires.txt
--rw-r--r--   0 feng      (1000) feng      (1000)        5 2023-03-31 05:01:30.000000 irff-1.5.2/irff.egg-info/top_level.txt
--rw-r--r--   0 feng      (1000) feng      (1000)       38 2023-03-31 05:01:30.316149 irff-1.5.2/setup.cfg
--rw-r--r--   0 feng      (1000) feng      (1000)     3568 2023-03-31 04:50:46.000000 irff-1.5.2/setup.py
-drwxr-xr-x   0 feng      (1000) feng      (1000)        0 2023-03-31 05:01:30.316149 irff-1.5.2/test/
--rw-r--r--   0 feng      (1000) feng      (1000)      241 2023-03-31 04:50:58.000000 irff-1.5.2/test/test.py
--rw-r--r--   0 feng      (1000) feng      (1000)      956 2023-03-31 04:50:58.000000 irff-1.5.2/test/test_data.py
--rw-r--r--   0 feng      (1000) feng      (1000)      272 2023-03-31 04:50:58.000000 irff-1.5.2/test/test_reax.py
--rw-r--r--   0 feng      (1000) feng      (1000)      806 2023-03-31 04:50:58.000000 irff-1.5.2/test/test_reax_nn.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    35181 2023-06-24 01:41:43.000000 irff-1.5.3/LICENSE
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      288 2023-07-03 14:53:55.000000 irff-1.5.3/PKG-INFO
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1482 2023-06-24 01:41:43.000000 irff-1.5.3/README.md
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    48550 2023-06-24 01:41:43.000000 irff-1.5.3/irff/AtomDance.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    34873 2023-06-24 01:41:43.000000 irff-1.5.3/irff/LearningMachine.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2861 2023-06-24 01:41:43.000000 irff-1.5.3/irff/RadiusCutOff.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)        4 2023-06-24 01:41:43.000000 irff-1.5.3/irff/__init__.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/data/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2268 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/ColData.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      439 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/dpdata.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    20949 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/mdtodata.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3005 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/prep_data.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      726 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/qeout_to_traj.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/deb/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7652 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/compare_energies.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    28016 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/deb_bde.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3746 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/hbdeb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2338 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/ird.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3542 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/irdeb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    27553 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/irffdeb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      696 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/irnan.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4126 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/mpdeb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    30455 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/reax_debug.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    28582 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/reax_gulp.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2712 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/theta.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/dft/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1764 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/CheckEmol.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4168 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/SinglePointEnergy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    16923 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/cpmd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    16974 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/dftb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     9604 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/nwchem.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    32584 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/qe.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    34877 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/siesta.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    22010 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/siesta_zmatix_constrain.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4145 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/smd_server.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1712 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dingtalk.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    32101 2023-06-24 01:41:43.000000 irff-1.5.3/irff/emdk.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    44033 2023-06-24 01:41:43.000000 irff-1.5.3/irff/fitbo.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)   230745 2023-07-03 14:53:54.000000 irff-1.5.3/irff/getNeighbor.c
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1822 2023-06-24 01:41:43.000000 irff-1.5.3/irff/getNeighbors.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6453 2023-06-24 01:41:43.000000 irff-1.5.3/irff/intCheck.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    56628 2023-06-24 01:41:43.000000 irff-1.5.3/irff/irff.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    58276 2023-06-24 01:41:43.000000 irff-1.5.3/irff/irff_np.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    16472 2023-06-24 01:41:43.000000 irff-1.5.3/irff/link.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/md/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4042 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/ReactionCapture.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3104 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2360 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/gofr.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    16896 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/gulp.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4704 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/hugoniot.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    18130 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/irmd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    19211 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/lammps.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/ml/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)        3 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6999 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/data.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7349 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/evaluate_data.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7764 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/evolution.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6427 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/ffield.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    10950 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/fit.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4110 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/fluctuation.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6011 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/gaqeq.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     9327 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/genetic.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    11038 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/gpfit_tfv2.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6406 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/harmonic.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    10769 2023-06-24 14:27:05.000000 irff-1.5.3/irff/ml/train.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    20150 2023-06-24 01:41:43.000000 irff-1.5.3/irff/mlqeq.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    14721 2023-06-24 01:41:43.000000 irff-1.5.3/irff/molecule.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    67947 2023-06-24 01:41:43.000000 irff-1.5.3/irff/mpnn.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)   908572 2023-07-03 14:53:54.000000 irff-1.5.3/irff/neighbor.c
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2987 2023-06-24 01:41:43.000000 irff-1.5.3/irff/neighbors.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/irff/plot/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1557 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/BondEnergy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2152 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/CheckAng.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1608 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/LearningResults.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3477 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/LearningResultsAng.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     5896 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/MessagePassing.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      185 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1782 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/abc.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2811 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/angel_to_bond.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4040 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/bde.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7652 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/compare_energies.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1766 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/fingerprint.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2360 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/gofr.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    18668 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/irnn_plot.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3899 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/label_md.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3813 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/labels.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     5155 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/morse.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     8837 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/morse_taper.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     8460 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/mpbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3813 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/mpnn_plbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3165 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/nx.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1853 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/pdf.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1120 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7085 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plbo.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1831 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/ple.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3406 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plea.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1522 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/pleb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2451 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/pleo.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1697 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plev.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1401 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plevdw.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4559 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plf.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3707 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_atoms.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2110 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_atoms_matplot.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2391 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_atoms_momenta.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1701 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_bond_energy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1632 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_charge.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2454 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_energy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2183 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_eover.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4129 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_eover_atom.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2696 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_functions.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1358 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_morse.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2543 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_pes.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3304 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_pressure.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2752 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_zmat_pes.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1917 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plotenergy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1900 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plotenergy_bond.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2240 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/pltp.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4694 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/reax_plbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1821 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/reax_pldd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    18380 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/reax_plot.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4402 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/reax_plov.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    24951 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/rffbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1199 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/sigmoid.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     8207 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/vdw_taper.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3108 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/view.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/irff/prop/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/prop/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2362 2023-06-24 01:41:43.000000 irff-1.5.3/irff/prop/gofr.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6059 2023-06-24 01:41:43.000000 irff-1.5.3/irff/qeq.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)   103280 2023-06-24 01:41:43.000000 irff-1.5.3/irff/reax.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    34168 2023-06-24 01:41:43.000000 irff-1.5.3/irff/reax_data.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    87075 2023-06-24 01:41:43.000000 irff-1.5.3/irff/reax_nn.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    27071 2023-06-24 01:41:43.000000 irff-1.5.3/irff/reaxfflib.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    11293 2023-06-24 01:41:43.000000 irff-1.5.3/irff/spectra.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/irff/structures/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      607 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/Al.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      767 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/C2C4.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2495 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/HMX_MOL.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2495 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/NM.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      434 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2469 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/ball.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2776 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/ball_bulk.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      844 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/diamond.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2749 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/fox7.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1949 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/nm3.gen
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/irff/tools/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1189 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/eos_opt.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      203 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/epstopdf.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1518 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/ffield_to_json.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1422 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/ffieldtolib.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1470 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/fingerprint.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6093 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/fit_hugoniot_state.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     9738 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/fitnn.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1259 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/json_to_ffield.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     8741 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/morse_taper.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1626 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/pre_opt.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6657 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/prepare_ffield.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1351 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/pressure.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3953 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/pseudo_gen.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3567 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/rsetff.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3328 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/setwb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      728 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/vdw.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1241 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/zmat_to_atoms.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     9800 2023-06-24 01:41:43.000000 irff-1.5.3/irff/trainer.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3798 2023-06-24 01:41:43.000000 irff-1.5.3/irff/zmatrix.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      288 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/PKG-INFO
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3493 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/SOURCES.txt
+-rwxrwxrwx   0 feng      (1000) feng      (1000)        1 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/dependency_links.txt
+-rwxrwxrwx   0 feng      (1000) feng      (1000)        5 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/top_level.txt
+-rwxrwxrwx   0 feng      (1000) feng      (1000)       38 2023-07-03 14:53:55.000000 irff-1.5.3/setup.cfg
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      857 2023-06-24 01:41:43.000000 irff-1.5.3/setup.py
```

### Comparing `irff-1.5.2/irff/AtomDance.py` & `irff-1.5.3/irff/AtomDance.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     if len(score)>=1:
        m = np.argmax(score)
        zv,zvlo,zvhi = zvs[m],zvlo_[m],zvhi_[m] 
     return Df_,zmatrix,zv,zvlo,zvhi
 
 
 class AtomDance(object):
-  def __init__(self,atoms=None,poscar=None,nn=True,ffield='ffield.json',
+  def __init__(self,atoms=None,poscar=None,nn=True,nomb=False,ffield='ffield.json',
                rotAng=40.0,angmax=30.0,freeatoms=None,FirstAtom=None,
                rmin=0.4,rmax=1.25,botol=0.0):
       self.rmin          = rmin
       self.rmax          = rmax
       self.botol         = botol
       self.BondDistrubed = []
       self.rotAng        = rotAng
@@ -241,14 +241,15 @@
             atoms  = read('poscar.gen')
          else:
             atoms  = read(poscar)
 
       self.ir = IRFF_NP(atoms=atoms,
                         libfile=ffield,
                         rcut=None,
+                        nomb=nomb,
                         nn=nn)
       self.natom     = self.ir.natom
       self.atom_name = self.ir.atom_name
       spec           = self.ir.spec
       self.atoms     = self.ir.atoms
       self.mass      = atoms.get_masses()
       if freeatoms is None:
```

### Comparing `irff-1.5.2/irff/LearningMachine.py` & `irff-1.5.3/irff/LearningMachine.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,37 +53,38 @@
   ''' recursive learning machine constructed by I-ReaxFF and siesta '''
   def __init__(self,initConfig='poscar.gen',
                dataset=None,ncpu=40,
                maxiter=100,
                dt_mlmd=0.1, dt_aimd=0.3,dft_step=5,
                batch=50,max_batch=100,
                step=20000,md_step=20,MaxMDstep=200,MinMDstep=50,
-               colFrame=50,colmin=3,
+               col_frame=50,col_min_interval=3,
                mom_step=100,
                mpopt=[1,1,1,1], messages=1,
                optword='nocoul',cons=None,clip={},
                T=300,# Tmax=1000,
                label=None,
                convergence=0.01,nconvergence=3,
                accCriteria=0.9,lossCriteria=10.0,lossTole=1.0,accTole=0.05,
                accMax=0.9,accInc=1.0001,mdInc=1.2,resetAcc=2,
-               learnWay=5,FreePairs=None,beta=None,
-               FreeAtoms=None,FirstAtom=None,
+               learn_method=3,FreePairs=None,beta=None,
+               free_atoms=None,first_atom=None,
                rodic=None,
                rmin=0.88,rmax=1.33,angmax=25.0,
-               CheckZmat=True,
+               CheckZmat=True,uncertainty=0.96,period=30,
                EngTole=0.05,dEtole=0.2,dEstop=2.0,
                nn=True,vdwnn=False,
                bo_layer=None,mf_layer=[9,1],be_layer=[9,1],vdw_layer=None,#[6,1],
-               be_universal_nn=None,bo_universal_nn=None,mf_universal_nn=None,vdw_universal_nn=None,
+               be_universal_nn=None,bo_universal_nn=None,
+               mf_universal_nn=None,vdw_universal_nn=None,
                BOFunction=0,EnergyFunction=1,MessageFunction=3,VdwFunction=1,
                spv_be=False,beup={},belo={},
                spv_bo=False,
                spv_vdw=False,vup={},vlo={},
-               spv_ang=False,lambda_ang=0.02,
+               spv_pi=False,# lambda_ang=0.02,
                weight={'others':2.0},
                lambda_bd=10000.0,lambda_reg=0.0001, # regularize=True,
                lambda_me=0.1,learning_rate=0.0001,
                writelib=5000,ffield='ffield.json',
                dft='siesta',kpts=(1,1,1),xcf='VDW',xca='DRSLL',basistype='DZP',
                **kwargs):
       ''' max_batch: max number of batch 
@@ -100,18 +101,20 @@
       self.accMax         = accMax 
       self.accInc         = accInc       # accuracy inrease factor
       self.resetAcc       = resetAcc     # reset accuracy criteria after this train cycle
       self.rmin           = rmin         # minimum bond length used to supervise ML-MD simulation
       self.rmax           = rmax
       self.angmax         = angmax
       self.CheckZmat      = CheckZmat
+      self.uncertainty    = uncertainty
+      self.period         = period
       self.convergence    = convergence
       self.cons           = cons
       self.nconvergence   = nconvergence
-      self.learnWay       = learnWay    # the way of learing
+      self.learn_method   = learn_method     # the way of learing
       self.ncpu           = ncpu
       self.step           = step
       self.batch          = batch
       self.dataset        = dataset
       self.maxiter        = maxiter
       self.max_batch      = max_batch   # max number in dataset to train
       self.dft            = dft
@@ -123,16 +126,16 @@
       self.dt_mlmd        = dt_mlmd
       self.dt_aimd        = dt_aimd
       self.T              = T
       # self.Tmax         = Tmax
       self.md_step        = md_step
       self.mom_step       = mom_step
       self.beta           = beta
-      self.colFrame       = colFrame
-      self.colmin         = colmin
+      self.col_frame       = col_frame
+      self.col_min_interval = col_min_interval
       self.EngTole        = EngTole
       self.dEtole         = dEtole
       self.dEstop         = dEstop
       self.MaxMDstep      = MaxMDstep
       self.MinMDstep      = MinMDstep
       self.mpopt          = mpopt
       self.optword        = optword
@@ -151,39 +154,36 @@
       self.vdw_layer      = vdw_layer
       self.bo_universal_nn = bo_universal_nn
       self.be_universal_nn = be_universal_nn
       self.mf_universal_nn = mf_universal_nn
       self.vdw_universal_nn= vdw_universal_nn
       self.beup           = beup
       self.belo           = belo
-      #self.boc            = boc
-      #self.bolo          = bolo
       self.vup            = vup
       self.vlo            = vlo
       self.spv_bo         = spv_bo
       self.spv_vdw        = spv_vdw
       self.spv_be         = spv_be
-      self.spv_ang        = spv_ang
+      self.spv_pi         = spv_pi
       self.lambda_me      = lambda_me
       self.weight         = weight
       self.lambda_bd      = lambda_bd
       # self.regularize   = regularize
       self.lambda_reg     = lambda_reg
-      self.lambda_ang     = lambda_ang
       self.learning_rate  = learning_rate
       self.BOFunction     = BOFunction
       self.EnergyFunction = EnergyFunction
       self.MessageFunction= MessageFunction
       self.writelib       = writelib
-      self.freeatoms      = FreeAtoms
+      self.freeatoms      = free_atoms
       self.freepairs      = FreePairs
       self.a              = AtomDance(poscar=self.initConfig,nn=self.nn,
                                     ffield=ffield,
                                     rmin=self.rmin-0.05,rmax=self.rmax,
-                                    FirstAtom=FirstAtom,freeatoms=self.freeatoms)
+                                    FirstAtom=first_atom,freeatoms=self.freeatoms)
       if self.freepairs is None:
          self.a.get_freebond(freeatoms=self.freeatoms)
       else:
          self.a.freebonds = self.freepairs
  
       self.natom        = self.a.natom
       self.atom_name    = self.a.atom_name
@@ -235,15 +235,15 @@
       iter_        = 0
       step         = 0
       mdsteps      = self.md_step
       momsteps     = self.mom_step
       data_dir     = {}
       running      = True
       Deformed     = 0
-      if self.learnWay==5:
+      if self.learn_method==5:
          if self.freeatoms is None:
             self.freeatoms = []
          ms        = len(self.freeatoms)
       else:
          ms        = 0
 
       self.learnpair = None
@@ -253,50 +253,51 @@
       nconvergence   = 0
       uncertainty_zv = None
       zmat_variable  = None
       zmatopt        = None
       images         = None
       zvlo,zvhi      = 0.0,0.0
       u_zvlo,u_zvhi  = 0.0,0.0
-      relax_step     = 5*self.colmin
+      relax_step     = 5*self.col_min_interval
 
       while running:
           optlog   = None
           relaxlog = None
-          learnWay = self.learnWay
-          mom_step = self.mom_step*(ms+1) if learnWay==5 else self.mom_step
+          learn_method = self.learn_method
+          mom_step = self.mom_step*(ms+1) if learn_method==5 else self.mom_step
           run_dir  = self.aidir+'/'+self.label+'-'+str(iter_)
           data_dir[self.label+'-'+str(iter_)] = cwd+'/'+run_dir+'/'+self.label+'.traj'
 
           if exists(run_dir):
              iter_ += 1
              continue
           if images is not None:
-             atoms = images[-1]   
+             atoms = images[-1] 
           elif isfile('md.traj'): 
-             atoms = read('md.traj',index=-1)
+             atoms = read('md.traj',index=-1) 
              consistance = self.check_atoms(atoms)
              assert consistance,'-  The species or cell parameter in md.traj is not consistant with initial configuration!'
              # print('-  atomic structure from MD trajectories.')
           else:
-             print('-  cannot find MD trajectory, use learnWay=1 in the first iter.')
+             print('-  cannot find MD trajectory, use learn_method=1 in the first iter.')
              atoms = read(self.initConfig)
-             learnWay = 1
+             learn_method = 4 if self.learn_method==4 else 1
           if not self.freeatoms is None:
              atoms = self.a.check_momenta(atoms,freeatoms=self.freeatoms)
              
-          if learnWay in [4,5,6]:
+          if learn_method in [4,5,6]:
              momsteps += mdsteps
              if momsteps >= mom_step:
                 momsteps  = 0
-                if learnWay == 4:
-                   atoms,self.learnpair,groupi,groupj = self.a.bond_momenta(atoms)
-                   if self.learnpair is None:
-                      learnWay = 3
-                elif learnWay == 5:
+                if learn_method == 4:
+                   # atoms,self.learnpair,groupi,groupj = self.a.bond_momenta(atoms)
+                   # if self.learnpair is None:
+                   #    learn_method = 3
+                   self.CheckZmat=False
+                elif learn_method == 5:
                    if ms<self.natom:
                       i = self.a.zmat_id[ms]
                       if i not in self.freeatoms: 
                          self.freeatoms.append(i)
                          for i_ in self.a.neighbors[i]:
                              if len(self.a.neighbors[i_])==1:
                                 if i_ not in self.freeatoms: 
@@ -309,32 +310,33 @@
                       #              self.freeatoms.append(j_)
                       self.save_config()
                       if ms+1<self.natom:
                          j = self.a.zmat_id[ms+1]
                          # self.learnpair = [i,j]
                          atoms,_,_ = self.a.set_bond_momenta(i,j,atoms)
                       else:
-                         learnWay = 3
+                         learn_method = 3
                          self.learnpair = None
-                   if learnWay ==5: learnWay = 4
-                # learnWay  = 2
+                   if learn_method ==5: learn_method = 3 # 4
+                # learn_method  = 2
                 ms       += 1
 
           # self.get_fixatom()
           # atoms.set_constraint(self.fixatoms)
           # atoms.write('poscar.gen')                                    # for aimd
 
-          if learnWay==1: 
+          if learn_method==1: 
              dft_step = self.dft_step
           elif Deformed>=1.0 or uncertainty_zv is not None:
              dft_step = relax_step
           else:
-             dft_step = int(mdsteps/self.colFrame)+1
-          
-          e_aimd,eml_,dEmax_,d2Emax_,LabelDataLog = self.aimd(atoms,cwd,run_dir,dft_step,learnWay)
+             dft_step = self.col_frame # int(mdsteps/self.col_frame)+1
+
+          ### aimd: DO ab init calculations
+          e_aimd,eml_,dEmax_,d2Emax_,LabelDataLog = self.aimd(atoms,cwd,run_dir,dft_step,learn_method) 
           e_siesta.append(e_aimd[0])                                   # get siesta results              
                                                                        # start training  
           trajs_ = prep_data(label=self.label,direcs=data_dir,
                              split_batch=self.batch,max_batch=self.max_batch,
                              frame=1000,dft=self.dft)                  # get trajs for training
           with open('training.log','w') as fe:                         # 
                fe.write('## training loss and accuries\n')             #
@@ -369,17 +371,16 @@
                                                      mf_universal_nn=self.mf_universal_nn,
                                                      vdw_universal_nn=self.vdw_universal_nn,
                                                      BOFunction=self.BOFunction,
                                                      EnergyFunction=self.EnergyFunction,
                                                      MessageFunction=self.MessageFunction,
                                                      # bore=self.bore, # bom=self.bom,
                                                      spv_be=self.spv_be,belo=self.belo,beup=self.beup,
-                                                     spv_bo=self.spv_bo,#boc=self.boc,#boup=self.boup,
+                                                     spv_bo=self.spv_bo,spv_pi=self.spv_pi,
                                                      spv_vdw=self.spv_vdw,vlo=self.vlo,vup=self.vup,
-                                                     spv_ang=self.spv_ang,lambda_ang=self.lambda_ang,
                                                      lambda_me=self.lambda_me,weight=self.weight,
                                                      lambda_reg=self.lambda_reg,
                                                      lambda_bd=self.lambda_bd,
                                                      learning_rate=self.learning_rate)
                 self.load_config()
                 if tIter>=self.resetAcc and tstep>=self.step:
                    if loss<self.lossCriteria+self.lossTole:   # accu>self.accCriteria-self.accTole and
@@ -400,33 +401,37 @@
              # if not zmatopt is None:
              #    optlog,_ = self.a.get_optimal_zv(atoms,zmatopt,optgen=self.initConfig)
              if mdsteps>10:
                 uncertainty_zv,u_zvlo,u_zvhi,optlog = self.a.get_zmat_uncertainty(atoms,optgen=self.initConfig)
 
           if mdsteps<10: mdsteps = 10
           # zmats    = None
-          images     = None
+          images     = None if learn_method!=4 else [atoms]
           # zmatopt  = zmat_vairable # if Deformed>=1.0 else uncertainty_zv
 
-          if learnWay==6:
+          if learn_method==6:
              if ms<len(self.freeatoms):
                 i = self.freeatoms[ms]
                 self.a.pes(i,atoms,nbin=dft_step,dr=0.1,traj='md.traj')
              if ms == len(self.freeatoms) -1:
-                self.learnWay=3
+                self.learn_method=3
+          elif learn_method==4:
+             e_gmd,mdsteps,Deformed,zmat_variable,zvlo,zvhi = self.mlmd(atoms, 10000,
+                                      iter_,learn_method,beta=self.beta,learnpair=self.learnpair,
+                                      groupi=groupi,groupj=groupj) 
           else:
              if Deformed>=1.0:
                 images,relaxlog = self.a.zmat_relax(atoms=atoms,zmat_variable=zmat_variable,nbin=relax_step,
                                                     zvlo=zvlo,zvhi=zvhi,traj='md.traj')
              elif uncertainty_zv is not None:
                 images,relaxlog = self.a.zmat_relax(atoms=atoms,zmat_variable=uncertainty_zv,nbin=relax_step,
                                                     zmatrix=self.a.zmatrix,zvlo=u_zvlo,zvhi=u_zvhi,traj='md.traj') # ,reset=True
              else:
                 e_gmd,mdsteps,Deformed,zmat_variable,zvlo,zvhi = self.mlmd(atoms, 10000,
-                                                iter_,learnWay,beta=self.beta,learnpair=self.learnpair,
+                                                iter_,learn_method,beta=self.beta,learnpair=self.learnpair,
                                                 groupi=groupi,groupj=groupj) 
                 if self.CheckZmat and mdsteps<=3:
                    mdsteps= 10
                    images,relaxlog = self.a.continous(atoms,nbin=mdsteps,traj='md.traj')
              if images is not None:
                 Deformed,zmat,zmat_variable,zvlo,zvhi = check_zmat(atoms=images[-1],rmin=self.rmin,
                                        rmax=self.rmax,angmax=self.angmax,zmat_id=self.a.zmat_id,
@@ -443,22 +448,22 @@
                 self.accCriteria = min(self.accCriteria*self.accInc,self.accMax)  
           elif accu < self.accCriteria:                                 # adjust MD steps according 
              if self.md_step>self.MinMDstep:                                        # training results
                 self.md_step  = int(self.md_step/self.mdInc)            #                 
 
           self.save_config()
 
-          e_gmd = eml_ if learnWay in [3,4,5] else 0.0
+          e_gmd = eml_ if learn_method in [3,4,5] else 0.0
           e_gulp.append(e_gmd[0])
           diff  = abs(e_gmd[0]-e_aimd[0])
           it.append(iter_)
 
           plot_energies(it,e_siesta,e_gulp)                             # plot learning status                                   
           self.learninglog(iter_,loss,accu,mdsteps,e_gulp[-1],e_siesta[-1],dEmax_,d2Emax_,LabelDataLog,
-          	               learnWay,Deformed,
+          	               learn_method,Deformed,
                            self.a.InitZmat,uncertainty_zv,zvlo,zvhi,optlog,relaxlog)
           converg_ = converg
           if diff<=self.convergence: 
              converg = True
           else:
              converg = False
 
@@ -477,15 +482,15 @@
              return diff
           elif loss==-1:
              send_msg('-  Some error occurred!')
              return diff
           iter_ += 1
 
   def learninglog(self,i,loss,accu,mdsteps,eirff,edft,dEmax,d2Emax,LabelDataLog,
-                  learnWay,Deformed,
+                  learn_method,Deformed,
                   InitZmat,uz,uzlo,uzhi,optlog,relaxlog):
       with open('learning.log','a') as l:
          l.write('                  ------------------------------------                  \n')
          l.write('                       Learning iteration:  {:4d}                        \n'.format(i))
          l.write('                  ------------------------------------                  \n')
          l.write(' \n')
          l.write('                     I&II  Labeling and Calling DFT \n')
@@ -505,26 +510,26 @@
          l.write('\n')
          l.write('                           IV Exploring \n')
          l.write('      Exploring the atomic configuration space by MD simulations \n')
          l.write('\n')
          l.write('MD Steps:  {:d}  \n'.format(mdsteps))
          l.write('Energy from ML and DFT:  {:f}  .vs.  {:f} \n'.format(eirff,edft))
          l.write('The max first derivative and second derivative:  {:f}  {:f} \n'.format(dEmax,d2Emax))
-         l.write('The learning method of this iter:  {:d} \n'.format(learnWay))
+         l.write('The learning method of this iter:  {:d} \n'.format(learn_method))
          if not relaxlog is None:
             if Deformed>=1:
                l.write('Molecule structure is deformed, using zmatmix relax\n' )
             elif not uz is None:
                l.write('Zmatrix variable:\n')
             l.write(relaxlog)
          if not optlog is None:
             l.write(optlog)
          l.write(' \n')
 
-  def aimd(self,atoms,cwd,run_dir,tstep,learnWay):
+  def aimd(self,atoms,cwd,run_dir,tstep,learn_method):
       mkdir(run_dir)
       chdir(cwd+'/'+run_dir)
       
       if self.dft=='siesta':
          system('cp ../../*.psf ./')
       elif self.dft=='qe':
          system('cp ../../*.UPF ./')
@@ -532,15 +537,15 @@
       system('cp ../../md.traj ./')
       
       emlmd  = []
       ind_   = ' '
       dEmax  = 0.0
       d2Emax = 0.0
       
-      if learnWay==1:
+      if learn_method==1:
          if self.dft=='siesta':
             images = siesta_md(label=self.label,ncpu=self.ncpu,T=self.T,dt=self.dt_aimd,us='F',tstep=tstep,
                                atoms=atoms,FreeAtoms=self.freeatoms,
                                xcf=self.xcf,xca=self.xca,basistype=self.basistype,**self.kwargs)
             # images = siesta_opt(atoms=atoms,label=self.label,ncpu=self.ncpu,VariableCell=False,us='F',
             #                     tstep=tstep,gen=cwd+'/'+gen,
             #                     xcf=self.xcf,xca=self.xca,basistype=self.basistype)
@@ -552,42 +557,46 @@
             #                gen=cwd+'/'+gen,
             #                kpts=self.kpts,**self.kwargs) ## geomentry optimize
             ind_   = 'Geomentry Optimization'
          else:
             raise RuntimeError('-  This method not implimented!')
          eaimd = [images[0].get_potential_energy()]
          system('cp %s ../../md.traj' %(self.label+'.traj'))
-      elif learnWay>=2:
+      elif learn_method>=2:
          # print('-  files in this dir \n',cwd+'/'+run_dir,'\n',listdir())
          E,E_,dEmax,d2Emax,ind_ = SinglePointEnergies(traj='md.traj',label=self.label,EngTole=self.EngTole,
                                                  frame=tstep,select=True,
-                                                 dE=self.dEtole,colmin=self.colmin,
+                                                 dE=self.dEtole,colmin=self.col_min_interval,
                                                  dft=self.dft,kpts=self.kpts,
                                                  xcf=self.xcf,xca=self.xca,basistype=self.basistype,
                                                  cpu=self.ncpu,**self.kwargs)
          eaimd = E
          emlmd = E_
       else:
          raise RuntimeError('-  learn way not supported yet!')
       chdir(cwd)
       return eaimd,emlmd,dEmax,d2Emax,ind_
 
-  def mlmd(self,atoms,Tmax,Iter,learnWay,learnpair=None,beta=None,
+  def mlmd(self,atoms,Tmax,Iter,learn_method,learnpair=None,beta=None,
            groupi=None,groupj=None):        
       ''' run classic MD to test training results '''
-      mdstep = max(int(self.md_step/5),2) if learnWay==2 else self.md_step
+      mdstep = max(int(self.md_step/5),2) if learn_method==2 else self.md_step
       zmats  = None
+      nomb = False if self.optword.find('nomb')<0 and learn_method!=4 else True
+      active = True if learn_method==4 else False
       irmd = IRMD(atoms=atoms,label=self.label,Iter=Iter,initT=self.T,
                   time_step=self.dt_mlmd,totstep=mdstep,Tmax=Tmax,
                   ro=self.ro,rmin=self.rmin,rmax=self.rmax,angmax=self.angmax,
                   CheckZmat=self.CheckZmat,InitZmat=self.a.InitZmat,
                   zmat_id=self.a.zmat_id,zmat_index=self.a.zmat_index,
                   dEstop=self.dEstop,dEtole=self.dEtole,nn=self.nn,vdwnn=self.vdwnn,
-                  learnpair=learnpair,beta=beta,groupi=groupi,groupj=groupj,freeatoms=self.freeatoms)
-      if learnWay==2:
+                  learnpair=learnpair,beta=beta,groupi=groupi,groupj=groupj,
+                  nomb=nomb,active=active,uncertainty=self.uncertainty,period=self.period,
+                  freeatoms=self.freeatoms)
+      if learn_method==2:
          Deformed,zmats,zv,zvlo,zvhi = irmd.opt()
       else:
          Deformed,zmats,zv,zvlo,zvhi = irmd.run()
       mdsteps= irmd.step
       Emd    = irmd.Epot
       irmd.close()
       return Emd,mdsteps,Deformed,zv,zvlo,zvhi
@@ -650,98 +659,66 @@
       #            consistance = False
       return consistance
 
   def save_config(self):
       with open('options.json','w') as fj:
            options = {'accCriteria':self.accCriteria,
                     'lossCriteria':self.lossCriteria,
-                    # 'lossTole':self.lossTole,
-                    # 'rmax':self.rmax,
-                    # 'angmax':self.angmax,
-                    # 'accTole':self.accTole,
-                    # 'accMax':self.accMax,
-                    # 'accInc':self.accInc,
-                    # 'resetAcc':self.resetAcc,
                     'step':self.step,
                     'md_step':self.md_step,
                     # 'mom_step':self.mom_step,
                     'MaxMDstep':self.MaxMDstep,
                     'MinMDstep':self.MinMDstep,
                     'EngTole':self.EngTole,
                     'dEtole':self.dEtole,
                     'dEstop':self.dEstop,
                     'beta':self.beta,
-                    # 'mpopt':self.mpopt,
-                    # 'regularize':self.regularize,
                     'lambda_reg':self.lambda_reg,
                     'lambda_bd':self.lambda_bd,
                     'lambda_me':self.lambda_me,
-                    'lambda_ang':self.lambda_ang,
                     'learning_rate':self.learning_rate,
-                    # 'rmin':self.rmin,
                     'T':self.T,
                     'maxiter':self.maxiter,
-                    # 'max_batch':self.max_batch,
-                    #'optword':self.optword,
-                    'learnWay':self.learnWay,
-                    'colFrame':self.colFrame,
+                    'learn_method':self.learn_method,
+                    'col_frame':self.col_frame,
                     'CheckZmat':self.CheckZmat,
                     'freeatoms':self.freeatoms}
-                    # 'freepairs':self.freepairs
-                    # 'bore':self.bore,
-                    # 'writelib':self.writelib
 
-           if self.learnWay==1:
+           if self.learn_method==1:
               options['dft_step'] = self.dft_step
            js.dump(options,fj,sort_keys=True,indent=2) 
 
   def load_config(self):
       with open('options.json','r') as fj:
            options = js.load(fj)
            self.accCriteria  = options['accCriteria']
            self.lossCriteria = options['lossCriteria']
-           # self.lossTole     = options['lossTole']
-           # self.rmax         = options['rmax']
-           # self.angmax       = options['angmax']
-           # self.accTole      = options['accTole']
-           # self.accMax     = options['accMax']
-           # self.accInc     = options['accInc']
-           # self.resetAcc   = options['resetAcc']
            self.step         = options['step'] 
-           if self.learnWay==1:
+           if self.learn_method==1:
               self.dft_step     = options['dft_step'] 
            self.md_step      = options['md_step'] 
            
            if 'mom_step' in options: self.mom_step  = options['mom_step'] 
-           if 'colmin'   in options: self.colmin = options['colmin'] 
+           if 'col_min_interval'   in options: self.col_min_interval = options['col_min_interval'] 
 
            self.MaxMDstep    = options['MaxMDstep'] 
            self.MinMDstep    = options['MinMDstep'] 
            self.EngTole      = options['EngTole'] 
            self.dEtole       = options['dEtole'] 
            self.dEstop       = options['dEstop'] 
            self.beta         = options['beta'] 
-           # self.mpopt        = options['mpopt'] 
-           # self.regularize   = options['regularize'] 
            self.lambda_reg   = options['lambda_reg'] 
            self.lambda_bd    = options['lambda_bd']
            self.lambda_me    = options['lambda_me']
-           self.lambda_ang   = options['lambda_ang']
-           # self.rmin       = options['rmin'] 
            self.T            = options['T'] 
            self.maxiter      = options['maxiter']
-           # self.max_batch  = options['max_batch']
-           #self.optword      = options['optword']
-           self.learnWay     = options['learnWay']
+           self.learn_method     = options['learn_method']
            self.learning_rate= options['learning_rate']
-           self.colFrame     = options['colFrame']
+           self.col_frame     = options['col_frame']
            self.CheckZmat    = options['CheckZmat']
-           # self.bore       = options['bore']
-           # self.writelib   = options['writelib']
-           # self.freepairs    = options['freepairs']
            if self.freeatoms!= options['freeatoms']:
               self.freeatoms = options['freeatoms']
               self.a.get_freebond(self.freeatoms)
            
   def close(self):
       print('-  LM compeleted.')
       self.atom_name = None
@@ -751,31 +728,30 @@
 if __name__ == '__main__':
    dataset = {'nm6_5':'/home/feng/siesta/nm6_5',
               'nm6_14':'/home/feng/siesta/nm6_14' }
 
    lm = LearningMachine(initConfig='c14.gen',
                      dataset=dataset,ncpu=8,
                      maxiter=1,
-                     step=50000,md_step=100,MaxMDstep=1000,mom_step=50,colFrame=100,
+                     step=50000,md_step=100,MaxMDstep=1000,mom_step=50,col_frame=100,
                      T=500,
                      angmax=20.0,
                      lossCriteria=20.0,lossTole=1.0,
                      CheckZmat=False,
                      # regularize=True,
                      lambda_reg=0.001,lambda_bd=1000.0,lambda_me=0.001,lambda_ang=0.01,
-                     learnWay=1,dft_step=50,
-                     beta=0.77,# FirstAtom=4,FreeAtoms=[4,5,8], 
+                     learn_method=1,dft_step=50,
+                     beta=0.77,# first_atom=4,FreeAtoms=[4,5,8], 
                      EngTole=0.01,dEtole=0.05,dEstop=2.0,
                      EnergyFunction=1,
                      bo_layer=[4,1],mf_layer=[9,2],be_layer=[6,1],vdw_layer=[6,1],
                      bo_universal_nn=None,#['O-O'],
                      be_universal_nn=None,#['O-O'],
                      mf_universal_nn=None,#['C'],
                      spv_be=False,bore={'others':0.22},
-                     spv_ang=False,
                      vdw_universal_nn=None,vdwnn=True,
                      weight={# 'no2-l':20.0,
                              'others':2.0},
                      optword='nocoul-nolone-nounder-noover', 
                      writelib=1000,convergence=0.04,
                      # xcf='GGA',xca='PBE',basistype='split'
                      dft='qe')
```

### Comparing `irff-1.5.2/irff/RadiusCutOff.py` & `irff-1.5.3/irff/RadiusCutOff.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/data/ColData.py` & `irff-1.5.3/irff/data/ColData.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,31 @@
       cwd         = getcwd()
       gen         = self.label+'.gen'
       self.direcs = {}
       i           = startstep
       data_dir    = {}
       running     = True
 
-      while running:
-          run_dir = 'aimd_'+self.label+'/'+self.label+'-'+str(i)
-          if exists(run_dir):
-             i += increase
-             data_dir[self.label+'-'+str(i)] = cwd+'/'+run_dir+'/'+self.label+'.traj'
-          else:
-             running = False
-          if not endstep is None:
-             if increase>0:
-                if i>endstep: running = False
-             else:
-                if i<endstep: running = False
+      traj        = self.label+'.traj'
+      if isfile(traj):
+         data_dir[self.label] = traj
+      else:
+         while running:
+            run_dir = 'aimd_'+self.label+'/'+self.label+'-'+str(i)
+            if exists(run_dir):
+                i += increase
+                data_dir[self.label+'-'+str(i)] = cwd+'/'+run_dir+'/'+self.label+'.traj'
+            else:
+                running = False
+            if not endstep is None:
+                if increase>0:
+                    if i>endstep: running = False
+                else:
+                    if i<endstep: running = False
+                    
       trajs_ = prep_data(label=self.label,direcs=data_dir,
                          split_batch=batch,max_batch=self.max_batch,
                          frame=100000,dft=dft)              # get trajs for training
       return trajs_
 
 class ColRawData(object):
   def __init__(self,max_batch=1000):
```

### Comparing `irff-1.5.2/irff/data/__init__.py` & `irff-1.5.3/irff/data/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/data/mdtodata.py` & `irff-1.5.3/irff/data/mdtodata.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,17 @@
 
     for i in range(batch):
         md.energy_nw[i]
         x = np.mod(md.x[i],box)  
         A = Atoms(md.atom_name,x,cell=md.cell,pbc=[True,True,True])
 
         e = float(md.energy_nw[i]) 
-        calc = SinglePointCalculator(A,energy=e,
+        A.calc = SinglePointCalculator(A,energy=e,
                                      free_energy=float(md.max_e),
                                      forces=md.forces[i])
-
-        # A.set_calculator(calc)
-        A.calc = calc
         his.write(atoms=A)
         del A
     his.close()
 
 def get_lattice(inp='inp-nve'):
     ''' get cpmd lattice constance '''
     finp = open(inp,'r')
@@ -277,17 +274,16 @@
              c = self.qs[i]
           A   = Atoms(self.atom_name,self.x[ii],
                       charges=c,
                       cell=self.cells[ii],pbc=[True,True,True])
           if self.checkMol:
              A =  press_mol(A)
 
-          calc = SinglePointCalculator(A,energy=float(self.energy_nw[ii]),
+          A.calc = SinglePointCalculator(A,energy=float(self.energy_nw[ii]),
                                          forces=self.forces[ii])
-          A.set_calculator(calc)
           his.write(atoms=A)
           images.append(A)
       his.close()
       return images
 
   def get_images(self):
       images = []
@@ -306,17 +302,16 @@
              c = None
           else:
              c = self.qs[i]
 
           A    = Atoms(self.atom_name,self.x[ii],
                         charges=c,
                         cell=self.cells[ii],pbc=[True,True,True])
-          calc = SinglePointCalculator(A,energy=float(self.energy_nw[ii]),
+          A.calc = SinglePointCalculator(A,energy=float(self.energy_nw[ii]),
                                          forces=self.forces[ii])
-          A.set_calculator(calc)
           images.append(A)
       return images
 
   def get_ase_energy(self,direc):
       images = Trajectory(direc)
       self.nframe = len(images)
       # print(images)
```

### Comparing `irff-1.5.2/irff/data/prep_data.py` & `irff-1.5.3/irff/data/prep_data.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/data/qeout_to_traj.py` & `irff-1.5.3/irff/data/qeout_to_traj.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/__init__.py` & `irff-1.5.3/irff/deb/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/compare_energies.py` & `irff-1.5.3/irff/deb/compare_energies.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/deb_bde.py` & `irff-1.5.3/irff/deb/deb_bde.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         e.append(ir.E)
         
     emin_ = np.min(Eb)
     eb    =  np.array(Eb) - emin_# )/emin_
     vmin_ =  np.min(Ev)
     ev    =  np.array(EV) - vmin_# )/emin_
 
-    plt.figure(figsize=figsize)     
+    plt.figure()     
     # plt.plot(bopsi,alpha=0.8,linewidth=2,linestyle=':',color='k',label=r'$BO_p^{\sigma}$')
     # plt.plot(boppi,alpha=0.8,linewidth=2,linestyle='-.',color='k',label=r'$BO_p^{\pi}$')
     # plt.plot(boppp,alpha=0.8,linewidth=2,linestyle='--',color='k',label=r'$BO_p^{\pi\pi}$')
     # plt.plot(bo0,alpha=0.8,linewidth=2,linestyle='-',color='g',label=r'$BO^{t=0}$')
     
     plt.plot(ev,alpha=0.8,linewidth=2,linestyle='-',color='y',label=r'$E_{vdw}$')
     plt.plot(eb,alpha=0.8,linewidth=2,linestyle='-',color='r',label=r'$E_{bond}$')
@@ -352,16 +352,15 @@
       print('ID: {:4d} Delta\': {:6.4f}'.format(i,ir.Deltap[i]))   
 
 def deb_eang(images,ang=[0,1,2],figsize=(8,6),show=False,print_=False,frame=[0]):
     i,j,k = ang
     a     = 0
     
     eang,ecoa,epen = [],[],[]
-    
-    ir = IRFF_NP(atoms=images[frame],
+    ir = IRFF_NP(atoms=images[frame[0]],
                  libfile='ffield.json',
                  nn=True)
     for f_ in frame:
         ir.calculate(images[f_])
       
         if print_:
            print('\n All angle: \n')
@@ -378,17 +377,17 @@
                a = na
                found = True
         if not found:
            # print('Warning: no angle found for {:s} in this trajector frame!'.format(ang))   
            continue 
         ir.calculate(atoms)
 
-        eang.append(ir.Eang)    
-        ecoa.append(ir.Etcon)
-        epen.append(ir.Epen)
+        eang.append(ir.eang[a])    
+        # ecoa.append(ir.Etcon)
+        # epen.append(ir.Epen)
         if print_:
            print('{:3d}  {:6.4f}  {:6.4f} Dpi: {:6.4f} pbo: {:6.4f} N: {:6.4f} SBO3: {:6.4f} eang: {:6.4f}'.format(i_,
                      ir.thet0[a],ir.theta[a],ir.sbo[a],ir.pbo[a],
                      ir.nlp[j],ir.SBO3[a],ir.eang[a])) # self.thet0-self.theta
          
     plt.figure(figsize=figsize)     
     plt.plot(eang,alpha=0.8,linewidth=2,linestyle='-',color='r',label=r'$E_{ang}$')# ($-E_{ang}/{:4.2f}$)'.format(ang_m))
@@ -631,14 +630,128 @@
     # plt.plot(ecoa,alpha=0.8,linewidth=2,linestyle='-',color='indigo',label=r'$E_{coa}$') # ($E_{coa}/%4.2f$)' %emx)
     # plt.plot(epen,alpha=0.8,linewidth=2,linestyle='-',color='b',label=r'$E_{pen}$') # ($E_{pen}/%4.2f$)' %eox)
     plt.legend(loc='best',edgecolor='yellowgreen')
     plt.savefig('deb_ang.pdf')
     if show: plt.show()
     plt.close()
 
+def get_changed_fourboday(images=None,traj='md.traj'):
+    if images is None:
+       images = Trajectory(traj)
+    Eb,Ea,Etor,E = [],[],[],[]
+    ir = IRFF_NP(atoms=images[0],
+                 libfile='ffield.json',
+                 nn='True')
+    ir.calculate(images[0])
+
+    tor_min = {}
+    tor_max = {}
+    for i,tor in enumerate(ir.tors):
+        t = tuple(tor)
+        tor_min[t] = ir.etor[i]
+        tor_max[t] = ir.etor[i]
+    # print(tor_min)
+
+    for i_,atoms in enumerate(images):       
+        ir.calculate(images[i_])
+        # print('%d Energies: ' %i_,'%12.4f ' %ir.E )
+
+        Eb.append(ir.Ebond)
+        Ea.append(ir.Eang)
+        Etor.append(ir.Etor)
+        E.append(ir.E)
+
+        for i,tor in enumerate(ir.tors):
+            t  = tuple(tor)
+            t_ = (tor[3],tor[2],tor[1],tor[0])
+            if t in tor_min:
+               if tor_min[t]>ir.etor[i]:
+                  tor_min[t] = ir.etor[i]
+               if tor_max[t]<ir.etor[i]:
+                  tor_max[t] = ir.etor[i]
+            elif t_ in tor_min:
+               if tor_min[t_]>ir.etor[i]:
+                  tor_min[t_] = ir.etor[i]
+               if tor_max[t_]<ir.etor[i]:
+                  tor_max[t_] = ir.etor[i]
+            else:
+              tor_min[t] = ir.etor[i]
+              tor_max[t] = ir.etor[i]
+    tor_change = []
+    tor_name   = []
+    m_ = 0.0
+    mi = 0
+    for i,t in enumerate(tor_min):
+        m = tor_max[t] - tor_min[t]
+        if m>m_:
+           mi = i
+           m_ = m
+        tor_change.append(m)
+        tor_name.append(t)
+    tor  = tor_name[mi]
+    tor_ = '{:s}-{:s}-{:s}-{:s}'.format(ir.atom_name[tor[0]],ir.atom_name[tor[1]],
+                                        ir.atom_name[tor[2]],ir.atom_name[tor[3]])
+    print(tor_,tor,tor_change[mi])
+
+def get_changed_threeboday(images=None,traj='md.traj'):
+    if images is None:
+       images = Trajectory(traj)
+    Eb,Ea,Etor,E = [],[],[],[]
+    ir = IRFF_NP(atoms=images[0],
+                 libfile='ffield.json',
+                 nn='True')
+    ir.calculate(images[0])
+
+    ang_min = {}
+    ang_max = {}
+    for i,ang in enumerate(ir.angs):
+        t = tuple(ang)
+        ang_min[t] = ir.eang[i]
+        ang_max[t] = ir.eang[i]
+        
+    for i_,atoms in enumerate(images):       
+        ir.calculate(images[i_])
+        # print('%d Energies: ' %i_,'%12.4f ' %ir.E )
+
+        Eb.append(ir.Ebond)
+        Ea.append(ir.Eang)
+        Etor.append(ir.Etor)
+        E.append(ir.E)
+
+        for i,ang in enumerate(ir.angs):
+            t  = tuple(ang)
+            t_ = (ang[2],ang[1],ang[0])
+            if t in ang_min:
+               if ang_min[t]>ir.eang[i]:
+                  ang_min[t] = ir.eang[i]
+               if ang_max[t]<ir.eang[i]:
+                  ang_max[t] = ir.eang[i]
+            elif t_ in ang_min:
+               if ang_min[t_]>ir.eang[i]:
+                  ang_min[t_] = ir.eang[i]
+               if ang_max[t_]<ir.eang[i]:
+                  ang_max[t_] = ir.eang[i]
+            else:
+              ang_min[t] = ir.eang[i]
+              ang_max[t] = ir.eang[i]
+    ang_change = []
+    ang_name   = []
+    m_ = 0.0
+    mi = 0
+    for i,t in enumerate(ang_min):
+        m = ang_max[t] - ang_min[t]
+        if m>m_:
+           mi = i
+           m_ = m
+        ang_change.append(m)
+        ang_name.append(t)
+    ang  = ang_name[mi]
+    ang_ = '{:s}-{:s}-{:s}'.format(ir.atom_name[ang[0]],ir.atom_name[ang[1]],ir.atom_name[ang[2]])
+    print(ang_,ang,ang_change[mi]) 
+
 ## compare the total energy with DFT energy
 
 # images = Trajectory('md.traj')
 # E = []
 # for atoms in images:
 #     E.append(atoms.get_potential_energy())
```

### Comparing `irff-1.5.2/irff/deb/hbdeb.py` & `irff-1.5.3/irff/deb/hbdeb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/ird.py` & `irff-1.5.3/irff/deb/ird.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/irdeb.py` & `irff-1.5.3/irff/deb/irdeb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/irffdeb.py` & `irff-1.5.3/irff/deb/irffdeb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/irnan.py` & `irff-1.5.3/irff/deb/irnan.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/mpdeb.py` & `irff-1.5.3/irff/deb/mpdeb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/reax_debug.py` & `irff-1.5.3/irff/deb/reax_debug.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/reax_gulp.py` & `irff-1.5.3/irff/deb/reax_gulp.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/deb/theta.py` & `irff-1.5.3/irff/deb/theta.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,47 +9,48 @@
                 libfile='ffield.json',
                 nn=True)
     ir.calculate(atoms)
 
     for a,ang in enumerate(ir.angs):
         i_,j_,k_ = ang
         if ir.eang[a]>0.00000001:
-           print('{:3d} {:2d}-{:2d}-{:2d}  {:s}-{:s}-{:s}  {:8.4f}'.format(a,i_,j_,k_,
-                 ir.atom_name[i_],ir.atom_name[j_],ir.atom_name[k_],ir.eang[a]))
+           print('{:3d} {:2d}-{:2d}-{:2d}  {:s}-{:s}-{:s}  {:8.4f} fijk {:8.4f} f7 {:8.4f} f8 {:8.4f}'.format(a,i_,j_,k_,
+                 ir.atom_name[i_],ir.atom_name[j_],ir.atom_name[k_],ir.eang[a],
+                 ir.fijk[a],ir.f_7[a],ir.f_8[a]))
         elif ir.eang[a]<0.0:
-           print('{:3d} {:2d}-{:2d}-{:2d}  {:s}-{:s}-{:s}  {:8.4f} {:8.4f} {:8.4f} {:8.4f}'.format(a,i_,j_,k_,
+           print('{:3d} {:2d}-{:2d}-{:2d}  {:s}-{:s}-{:s}  {:8.4f} fijk {:8.4f} f7 {:8.4f} f8 {:8.4f}'.format(a,i_,j_,k_,
                  ir.atom_name[i_],ir.atom_name[j_],ir.atom_name[k_],ir.eang[a],
                  ir.fijk[a],ir.f_7[a],ir.f_8[a]))
             
 
     a_ = int(input('please input the id of the  angle to output(-1 to exit): '))
     i,j,k = ir.angs[a_]
     ang_ =  '{:s}-{:s}-{:s}'.format(ir.atom_name[i],ir.atom_name[j],ir.atom_name[k])
 
     theta_ = []
     Eang   = []
 
     if a_>=0:
-        for atoms in images:
+        for t,atoms in enumerate(images):
             ir.calculate(atoms)
             a = np.where(np.logical_and(np.logical_and(ir.angs[:,0]==i,ir.angs[:,1]==j),ir.angs[:,2]==k))
             a = np.squeeze(a)
              
             if len(ir.angs)==1:
-               print('{:3d}  theta0: {:6.4f} theta {:6.4f} Dang: {:6.2f} rnlp: {:6.2f} '
-                        'SBO: {:6.2f} sbo: {:6.2f} pbo: {:6.2f} SBO3: {:6.2f} Eang: {:6.4f}'.format(a,
-                        ir.thet0[a],ir.theta,ir.dang,ir.rnlp,ir.SBO,ir.sbo,ir.pbo,
+               print('{:3d} theta0: {:6.4f} theta: {:6.4f} Dang: {:4.2f} D: {:5.2f} L: {:4.2f} '
+                        'S: {:4.2f} s: {:4.2f} p: {:4.2f} S3: {:4.2f} E: {:6.4f}'.format(t,
+                        ir.thet0[a],ir.theta,ir.dang,ir.Deltap[j],ir.rnlp,ir.SBO,ir.sbo,ir.pbo,
                         ir.SBO3,ir.eang[a])) # self.thet0-self.theta
                theta_.append(ir.theta)
                Eang.append(ir.eang[a])
             else:
-               print('{:3d}  theta0: {:6.4f} theta {:6.4f} Dang: {:6.2f} rnlp: {:6.2f} '
-                        'SBO: {:6.2f} sbo: {:6.2f} pbo: {:6.2f} SBO3: {:6.2f} Eang: {:6.4f}'.format(a,
-                        ir.thet0[a],ir.theta[a],ir.dang[a],ir.rnlp[a],ir.SBO[a],ir.sbo[a],ir.pbo[a],
-                        ir.SBO3[a],ir.eang[a])) # self.thet0-self.theta
+               print('{:3d} t0: {:6.4f} t: {:6.4f} Dang: {:4.2f} D: {:5.2f} L: {:4.2f} '
+                     'S: {:4.2f} s: {:4.2f} p: {:4.2f} S3:{:4.2f} E: {:6.4f}'.format(t,
+                     ir.thet0[a],ir.theta[a],ir.dang[a],ir.Deltap[j],ir.rnlp[a],ir.SBO[a],ir.sbo[a],ir.pbo[a],
+                     ir.SBO3[a],ir.eang[a])) # self.thet0-self.theta
                theta_.append(ir.theta[a])
                Eang.append(ir.eang[a])
                # else:
                #    print(a)
 
         plt.figure()     
         # plt.plot(theta_,Eang,alpha=0.8,linewidth=2,linestyle='-',color='b',label=r'$Eangle({:s})$'.format(ang_))
```

### Comparing `irff-1.5.2/irff/dft/CheckEmol.py` & `irff-1.5.3/irff/dft/CheckEmol.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/dft/SinglePointEnergy.py` & `irff-1.5.3/irff/dft/SinglePointEnergy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/dft/__init__.py` & `irff-1.5.3/irff/dft/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/dft/cpmd.py` & `irff-1.5.3/irff/dft/cpmd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/dft/dftb.py` & `irff-1.5.3/irff/dft/dftb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/dft/nwchem.py` & `irff-1.5.3/irff/dft/nwchem.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/dft/qe.py` & `irff-1.5.3/irff/dft/qe.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,16 +278,16 @@
        pwi.append('  ion_dynamics    = \'bfgs\' \n')
        pwi.append('/\n')  # terminate section
        pwi.append('\n')
        pwi.append('&CELL\n')
        pwi.append('  cell_dynamics    = \'bfgs\' \n')
        pwi.append('/\n')  # terminate section
        pwi.append('\n')
-    else:
-       raise RuntimeError('-  This type of run of QE is not supported yet!')
+    #else:
+    #   raise RuntimeError('-  This type of run of QE is not supported yet!')
     
     if kspacing is not None:
        kgrid = kspacing_to_grid(atoms, kspacing)
     elif kpts is not None:
        if isinstance(kpts, dict) and 'path' not in kpts:
           kgrid, shift = kpts2sizeandoffsets(atoms=atoms, **kpts)
           koffset = []
@@ -324,16 +324,15 @@
        pwi.append('ATOMIC_POSITIONS angstrom\n')
        pwi.extend(atomic_positions_str)
     pwi.append('\n')
 
     # BandPath object or bandpath-as-dictionary:
     if 'K_POINTS' in kwargs:
        pwi.append('K_POINTS automatic\n')
-       pwi.append('{0[0]} {0[1]} {0[2]}  {1[0]:d} {1[1]:d} {1[2]:d}\n'
-                  ''.format(kwargs['K_POINTS'], koffset))
+       pwi.append('{:s} \n'.format(kwargs['K_POINTS']))
     else:
        pwi.append('K_POINTS automatic\n')
        pwi.append('{0[0]} {0[1]} {0[2]}  {1[0]:d} {1[1]:d} {1[2]:d}\n'
                   ''.format(kgrid, koffset))
     pwi.append('\n')
 
     with open('pw.in','w') as fd:
```

### Comparing `irff-1.5.2/irff/dft/siesta.py` & `irff-1.5.3/irff/dft/siesta.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/dft/siesta_zmatix_constrain.py` & `irff-1.5.3/irff/dft/siesta_zmatix_constrain.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/dft/smd_server.py` & `irff-1.5.3/irff/dft/smd_server.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/dingtalk.py` & `irff-1.5.3/irff/dingtalk.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/emdk.py` & `irff-1.5.3/irff/emdk.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/fitbo.py` & `irff-1.5.3/irff/fitbo.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/getNeighbor.c` & `irff-1.5.3/irff/getNeighbor.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-/* Generated by Cython 0.29.13 */
+/* Generated by Cython 0.29.32 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "irff.getNeighbor",
         "sources": [
             "irff/getNeighbor.pyx"
         ]
     },
     "module_name": "irff.getNeighbor"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_13"
-#define CYTHON_HEX_VERSION 0x001D0DF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -55,14 +57,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -91,18 +94,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -132,18 +139,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -163,53 +219,64 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -318,17 +385,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -434,24 +560,36 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
+  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
+  #else
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
+  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #endif
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -492,26 +630,35 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -537,21 +684,21 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -565,16 +712,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -584,19 +733,18 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -697,14 +845,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -908,15 +1057,15 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
@@ -938,21 +1087,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -1083,15 +1240,15 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
@@ -1197,23 +1354,28 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
@@ -1378,14 +1540,17 @@
 /* Python wrapper */
 static PyObject *__pyx_pw_4irff_11getNeighbor_1find_mole(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4irff_11getNeighbor_1find_mole = {"find_mole", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4irff_11getNeighbor_1find_mole, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_4irff_11getNeighbor_1find_mole(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_ID = 0;
   PyObject *__pyx_v_mol_index = 0;
   PyObject *__pyx_v_table = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("find_mole (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ID,&__pyx_n_s_mol_index,&__pyx_n_s_table,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -1459,14 +1624,17 @@
   PyObject *(*__pyx_t_5)(PyObject *);
   int __pyx_t_6;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find_mole", 0);
   __Pyx_INCREF(__pyx_v_mol_index);
 
   /* "irff/getNeighbor.pyx":7
  * 
  * def find_mole(ID,mol_index,table):
  *     mol_index.append(ID)             # <<<<<<<<<<<<<<
@@ -1667,14 +1835,17 @@
 static PyMethodDef __pyx_mdef_4irff_11getNeighbor_3get_neighbors = {"get_neighbors", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4irff_11getNeighbor_3get_neighbors, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_4irff_11getNeighbor_3get_neighbors(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_Atoms = 0;
   PyObject *__pyx_v_r_cut = 0;
   PyObject *__pyx_v_cell = 0;
   PyObject *__pyx_v_exception = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_neighbors (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_filename,&__pyx_n_s_Atoms,&__pyx_n_s_r_cut,&__pyx_n_s_cell,&__pyx_n_s_exception,0};
     PyObject* values[5] = {0,0,0,0,0};
     values[0] = ((PyObject *)Py_None);
@@ -1812,14 +1983,17 @@
   long __pyx_t_14;
   int __pyx_t_15;
   int __pyx_t_16;
   long __pyx_t_17;
   PyObject *__pyx_t_18 = NULL;
   int __pyx_t_19;
   int __pyx_t_20;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_neighbors", 0);
   __Pyx_INCREF(__pyx_v_r_cut);
   __Pyx_INCREF(__pyx_v_cell);
 
   /* "irff/getNeighbor.pyx":16
  * def get_neighbors(filename=None,Atoms=None,r_cut=None,cell=None,exception=[]):
  *     cdef int i,j
@@ -3053,25 +3227,27 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
+#else
+#define __Pyx_PyMODINIT_FUNC void
 #endif
 #else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initgetNeighbor(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initgetNeighbor(void)
@@ -3146,14 +3322,17 @@
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_getNeighbor(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'getNeighbor' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -3193,19 +3372,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("getNeighbor", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -3234,17 +3411,17 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "irff.getNeighbor")) {
       if (unlikely(PyDict_SetItemString(modules, "irff.getNeighbor", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
@@ -3454,15 +3631,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -3481,15 +3658,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -3497,15 +3674,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -3680,15 +3857,15 @@
 #endif
 #endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -3767,15 +3944,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
+        } else if (__Pyx_PyFastCFunction_Check(func)) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -4428,15 +4605,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -4503,15 +4680,15 @@
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* CLineInTraceback */
     #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -4533,15 +4710,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -4607,15 +4784,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
@@ -4627,41 +4804,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
     #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -4672,34 +4856,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -4708,45 +4907,14 @@
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
-/* CIntToPy */
-    static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPyVerify */
     #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
@@ -4762,47 +4930,61 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntToPy */
-    static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+    static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
+        if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(int) <= sizeof(long)) {
+        if (sizeof(long) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
+        return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
     static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -4981,17 +5163,62 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntToPy */
+    static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
     static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -5272,19 +5499,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
     static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -5534,14 +5783,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `irff-1.5.2/irff/getNeighbors.py` & `irff-1.5.3/irff/getNeighbors.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/intCheck.py` & `irff-1.5.3/irff/intCheck.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/irff.py` & `irff-1.5.3/irff/irff.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,27 +88,29 @@
                libfile='ffield',
                vdwcut=10.0,
                atol=0.001,
                hbtol=0.001,
                nn=False,# vdwnn=False,
                messages=1,
                hbshort=6.75,hblong=7.5,
+               nomb=False,  # this option is used when deal with metal system
                autograd=True,
                CalStress=False,
                label="IRFF", **kwargs):
       Calculator.__init__(self,label=label, **kwargs)
       self.atoms        = atoms
       self.cell         = atoms.get_cell()
       self.atom_name    = self.atoms.get_chemical_symbols()
       self.natom        = len(self.atom_name)
       self.spec         = []
       self.nn           = nn
       # self.vdwnn      = vdwnn
       self.EnergyFunction = 0
       self.autograd     = autograd
+      self.nomb         = nomb # without angle, torsion and hbond manybody term
       self.messages     = messages 
       self.safety_value = 0.000000001
       self.GPa          = 1.60217662*1.0e2
       self.CalStress    = CalStress
 
       if libfile.endswith('.json'):
          lf                  = open(libfile,'r')
@@ -188,52 +190,52 @@
       vr    = xj-xi
       
       vrf   = np.dot(vr,rcell)
       vrf   = np.where(vrf-0.5>0,vrf-1.0,vrf)
       vrf   = np.where(vrf+0.5<0,vrf+1.0,vrf)  
       vr    = np.dot(vrf,cell)
       r     = np.sqrt(np.sum(vr*vr,axis=2))
-
-      angs,tors,hbs = get_neighbors(self.natom,self.atom_name,self.r_cuta,r)
+      
+      if self.nomb:
+         angs,tors,hbs = [],[],[]
+      else:
+         angs,tors,hbs = get_neighbors(self.natom,self.atom_name,self.r_cuta,r)
 
       self.angs  = np.array(angs)
       self.tors  = np.array(tors)
       self.hbs   = np.array(hbs)
 
       self.nang  = len(self.angs)
       self.ntor  = len(self.tors)
       self.nhb   = len(self.hbs)
     
       if self.nang>0:
          self.angj  = self.angs[:,1]
          self.angi  = self.angs[:,0]
          self.angk  = self.angs[:,2]
+         P_ = get_pangle(self.p,self.atom_name,len(self.p_ang),self.p_ang,self.nang,angs)
+         for key in P_:
+             self.P[key] = torch.from_numpy(P_[key])
 
       if self.ntor>0:
          self.tori  = self.tors[:,0]
          self.torj  = self.tors[:,1]
          self.tork  = self.tors[:,2]
          self.torl  = self.tors[:,3]
+         P_ = get_ptorsion(self.p,self.atom_name,len(self.p_tor),self.p_tor,self.ntor,tors)
+         for key in P_:
+             self.P[key] = torch.from_numpy(P_[key])
 
       if self.nhb>0:
          self.hbi     = self.hbs[:,0]
          self.hbj     = self.hbs[:,1]
          self.hbk     = self.hbs[:,2]
-
-      P_ = get_pangle(self.p,self.atom_name,len(self.p_ang),self.p_ang,self.nang,angs)
-      for key in P_:
-          self.P[key] = torch.from_numpy(P_[key])
-
-      P_ = get_ptorsion(self.p,self.atom_name,len(self.p_tor),self.p_tor,self.ntor,tors)
-      for key in P_:
-          self.P[key] = torch.from_numpy(P_[key])
-
-      P_ = get_phb(self.p,self.atom_name,len(self.p_hb),self.p_hb,self.nhb,hbs)
-      for key in P_:
-          self.P[key] = torch.from_numpy(P_[key])
+         P_ = get_phb(self.p,self.atom_name,len(self.p_hb),self.p_hb,self.nhb,hbs)
+         for key in P_:
+             self.P[key] = torch.from_numpy(P_[key])
 
   def set_rcut(self,rcut,rcuta,re): 
       rcut_,rcuta_,re_ = setRcut(self.bonds,rcut,rcuta,re)
       self.rcut  = rcut_    ## bond order compute cutoff
       self.rcuta = rcuta_   ## angle term cutoff
 
       # self.r_cut = np.zeros([self.natom,self.natom],dtype=np.float32)
@@ -422,16 +424,17 @@
              Fpp = F[:,:,2]
              self.Hsi.append(self.Hsi[t-1]*Fsi)
              self.Hpi.append(self.Hpi[t-1]*Fpi)
              self.Hpp.append(self.Hpp[t-1]*Fpp)
           elif self.MessageFunction==2:
              Dbi = Di - self.H[t-1]
              Dbj = Dj - self.H[t-1]
-             Fi  = self.f_nn('fm',[Dbj,Dbi,self.Hsi[t-1],self.Hpi[t-1],self.Hpp[t-1]], # +str(t)
-                             layer=self.mf_layer[1])
+             #Fi  = self.f_nn('fm',[Dbj,Dbi,self.Hsi[t-1],self.Hpi[t-1],self.Hpp[t-1]], # +str(t)
+             #                layer=self.mf_layer[1])
+             Fi  = self.f_nn('fm',[Dbj,self.H[t-1],Dbi],layer=self.mf_layer[1])
              Fj  = torch.transpose(Fi,1,0)
              F   = Fi*Fj
              Fsi = F[:,:,0]
              Fpi = F[:,:,1]
              Fpp = F[:,:,2]
              self.Hsi.append(self.Hsi[t-1]*Fsi)
              self.Hpi.append(self.Hpi[t-1]*Fpi)
```

### Comparing `irff-1.5.2/irff/irff_np.py` & `irff-1.5.3/irff/irff_np.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,24 +68,26 @@
   implemented_properties = ["energy", "forces"] # , "stress"]
   def __init__(self,atoms=None,
                libfile='ffield',
                vdwcut=10.0,
                nn=False,# vdwnn=False,
                messages=1,
                hbshort=6.75,hblong=7.5,
+               nomb=False,  # this option is used when dealing with metal system
                mol=None,label="IRFF", **kwargs):
       # Calculator.__init__(self,label=label, **kwargs)
       self.atoms        = atoms
       self.cell         = atoms.get_cell()
       self.atom_name    = self.atoms.get_chemical_symbols()
       self.natom        = len(self.atom_name)
       self.spec         = []
       self.nn           = nn
       # self.vdwnn      = vdwnn
       self.EnergyFunction = 0
+      self.nomb         = nomb # without angle, torsion and hbond manybody term
       self.messages     = messages
       self.safety_value = 0.000000001
       self.label        = label
 
       self.p_ang  = ['theta0','val1','val2','coa1','val7','val4','pen1'] 
       self.p_hb   = ['rohb','Dehb','hb1','hb2']
       self.p_tor  = ['V1','V2','V3','tor1','cot1']  
@@ -159,79 +161,66 @@
       self.d2        = np.triu(d,k=1)
       self.eye       = 1.0 - np.eye(self.natom,dtype=np.float32)
       self.check_offd()
       self.check_hb()
       self.get_rcbo()
       self.set_p(m,self.bo_layer)
       self.Qe= qeq(p=self.p,atoms=self.atoms)
-    
 
   def get_charge(self,cell,positions):
       self.Qe.calc(cell,positions)
       self.q   = self.Qe.q[:-1]
       qij      = np.expand_dims(self.q,axis=0)*np.expand_dims(self.q,axis=1)
       self.qij = qij*14.39975840 
 
-
   def get_neighbor(self,cell,rcell,positions):
       xi    = np.expand_dims(positions,axis=0)
       xj    = np.expand_dims(positions,axis=1)
       vr    = xj-xi
       
       vrf   = np.dot(vr,rcell)
       vrf   = np.where(vrf-0.5>0,vrf-1.0,vrf)
       vrf   = np.where(vrf+0.5<0,vrf+1.0,vrf)  
       vr    = np.dot(vrf,cell)
       r     = np.sqrt(np.sum(vr*vr,axis=2))
 
-      angs,tors,hbs = get_neighbors(self.natom,self.atom_name,self.r_cuta,r)
+      if self.nomb:
+         angs,tors,hbs = [],[],[]
+      else:
+         angs,tors,hbs = get_neighbors(self.natom,self.atom_name,self.r_cuta,r)
 
       self.angs  = np.array(angs)
       self.tors  = np.array(tors)
       self.hbs   = np.array(hbs)
 
       self.nang  = len(self.angs)
       self.ntor  = len(self.tors)
       self.nhb   = len(self.hbs)
     
       if self.nang>0:
          self.angi  = self.angs[:,0] # np.expand_dims(self.angs[:,0],axis=1)
          self.angj  = self.angs[:,1] # np.expand_dims(self.angs[:,1],axis=1)
          self.angk  = self.angs[:,2] # np.expand_dims(self.angs[:,2],axis=1)
-
-         # self.angij = np.transpose([self.angs[:,0],self.angs[:,1]])
-         # self.angjk = np.transpose([self.angs[:,1],self.angs[:,2]])
-         # self.angik = np.transpose([self.angs[:,0],self.angs[:,2]])
+         P_ = get_pangle(self.p,self.atom_name,len(self.p_ang),self.p_ang,self.nang,angs)
+         self.P.update(P_)
 
       if self.ntor>0:
          self.tori  = self.tors[:,0] # np.expand_dims(self.tors[:,0],axis=1)
          self.torj  = self.tors[:,1] # np.expand_dims(self.tors[:,1],axis=1)
          self.tork  = self.tors[:,2] # np.expand_dims(self.tors[:,2],axis=1)
          self.torl  = self.tors[:,3] # np.expand_dims(self.tors[:,3],axis=1)
-
-         # self.torij = np.transpose([self.tors[:,0],self.tors[:,1]])
-         # self.torjk = np.transpose([self.tors[:,1],self.tors[:,2]])
-         # self.torkl = np.transpose([self.tors[:,2],self.tors[:,3]])
+         P_ = get_ptorsion(self.p,self.atom_name,len(self.p_tor),self.p_tor,self.ntor,tors)
+         self.P.update(P_)
 
       if self.nhb>0:
          self.hbi     = self.hbs[:,0] # np.expand_dims(self.hbs[:,0],axis=1)
          self.hbj     = self.hbs[:,1] # np.expand_dims(self.hbs[:,1],axis=1)
          self.hbk     = self.hbs[:,2] # np.expand_dims(self.hbs[:,2],axis=1)
-         # self.hbij  = np.transpose([self.hbs[:,0],self.hbs[:,1]])
-         # self.hbjk  = np.transpose([self.hbs[:,1],self.hbs[:,2]])
-
-      P_ = get_pangle(self.p,self.atom_name,len(self.p_ang),self.p_ang,self.nang,angs)
-      self.P.update(P_)
-
-      P_ = get_ptorsion(self.p,self.atom_name,len(self.p_tor),self.p_tor,self.ntor,tors)
-      self.P.update(P_)
-
-      P_ = get_phb(self.p,self.atom_name,len(self.p_hb),self.p_hb,self.nhb,hbs)
-      self.P.update(P_)
-
+         P_ = get_phb(self.p,self.atom_name,len(self.p_hb),self.p_hb,self.nhb,hbs)
+         self.P.update(P_)
 
   def set_rcut(self,rcut,rcuta,re): 
       rcut_,rcuta_,re_ = setRcut(self.bonds,rcut,rcuta,re)
       self.rcut  = rcut_    ## bond order compute cutoff
       self.rcuta = rcuta_  ## angle term cutoff
 
       self.r_cut = np.zeros([self.natom,self.natom],dtype=np.float32)
@@ -301,38 +290,34 @@
 
       self.Deltap= np.sum(self.bop,axis=1)  
       if self.MessageFunction==1:
          self.D_si = [np.sum(self.bop_si,axis=1)] 
          self.D_pi = [np.sum(self.bop_pi,axis=1)] 
          self.D_pp = [np.sum(self.bop_pp,axis=1)] 
 
-
   def f1(self):
       Dv  = np.expand_dims(self.Deltap - self.P['val'],axis=0)
       self.f2(Dv)
       self.f3(Dv)
       VAL      = np.expand_dims(self.P['val'],axis=1)
       VALt     = np.expand_dims(self.P['val'],axis=0)
       self.f_1 = 0.5*(np.divide(VAL+self.f_2,  VAL+self.f_2+self.f_3)  + 
                       np.divide(VALt+self.f_2, VALt+self.f_2+self.f_3))
 
-
   def f2(self,Dv):
       self.dexpf2  = np.exp(-self.P['boc1']*Dv)
       self.f_2     = self.dexpf2 + np.transpose(self.dexpf2,[1,0])
 
-
   def f3(self,Dv):
       self.dexpf3 = np.exp(-self.P['boc2']*Dv)
       delta_exp   = self.dexpf3 + np.transpose(self.dexpf3,[1,0])
 
       self.f3log  = np.log(0.5*delta_exp )
       self.f_3    = (-1.0/self.P['boc2'])*self.f3log
 
-
   def f45(self):
       self.D_boc = self.Deltap - self.P['valboc'] # + self.p['val_'+atomi]
       
       self.DELTA  = np.expand_dims(self.D_boc,axis=1)
       self.DELTAt = np.transpose(self.DELTA,[1,0])
       
       self.df4 = self.P['boc4']*np.square(self.bop)-self.DELTA
@@ -340,15 +325,14 @@
 
       self.df5 = self.P['boc4']*np.square(self.bop)-self.DELTAt
       self.f5r = np.exp(-self.P['boc3']*(self.df5)+self.P['boc5'])
 
       self.f_4 = 1.0/(1.0+self.f4r)
       self.f_5 = 1.0/(1.0+self.f5r)
 
-
   def get_bondorder(self):
       self.f1()
       self.f45()
 
       f11    = np.where(self.P['ovcorr']>=0.0001,self.f_1,1.0)
       f12    = np.where(np.logical_and(self.P['ovcorr']>=0.0001,self.P['corr13']>=0.0001),
                          self.f_1,1.0)
@@ -396,15 +380,14 @@
       self.F         = []
       self.H.append(self.bop)                   # 
       self.Hsi.append(self.bop_si)              #
       self.Hpi.append(self.bop_pi)              #
       self.Hpp.append(self.bop_pp)              # 
       self.D.append(self.Deltap)                # get the initial hidden state H[0]
 
-
       for t in range(1,self.messages+1):
           Di        = np.expand_dims(self.D[t-1],axis=0)*self.eye
           Dj        = np.expand_dims(self.D[t-1],axis=1)*self.eye
 
           if self.MessageFunction==1:
              Dsi_i = np.expand_dims(self.D_si[t-1],axis=0)*self.eye - self.Hsi[t-1]
              Dsi_j = np.expand_dims(self.D_si[t-1],axis=1)*self.eye - self.Hsi[t-1]
@@ -429,16 +412,17 @@
              self.F.append(F)
              self.Hsi.append(self.Hsi[t-1]*Fsi)
              self.Hpi.append(self.Hpi[t-1]*Fpi)
              self.Hpp.append(self.Hpp[t-1]*Fpp)
           elif self.MessageFunction==2:
              Dbi   = Di  - self.H[t-1]
              Dbj   = Dj  - self.H[t-1]
-             Fi    = self.f_nn('fm',[Dbj,Dbi,self.Hsi[t-1],self.Hpi[t-1],self.Hpp[t-1]], # +str(t)
-                               layer=self.mf_layer[1])
+             #Fi    = self.f_nn('fm',[Dbj,Dbi,self.Hsi[t-1],self.Hpi[t-1],self.Hpp[t-1]], # +str(t)
+             #                  layer=self.mf_layer[1])
+             Fi    = self.f_nn('fm',[Dbj,self.H[t-1],Dbi],layer=self.mf_layer[1])
              Fj    = np.transpose(Fi,[1,0,2])
              F     = Fi*Fj
              Fsi = F[:,:,0]
              Fpi = F[:,:,1]
              Fpp = F[:,:,2]
              self.F.append(F)
              self.Hsi.append(self.Hsi[t-1]*Fsi)
```

### Comparing `irff-1.5.2/irff/link.py` & `irff-1.5.3/irff/link.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/md/ReactionCapture.py` & `irff-1.5.3/irff/md/ReactionCapture.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/md/__init__.py` & `irff-1.5.3/irff/md/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from ..plot import view
 from ase.io.trajectory import Trajectory
 import numpy as np
 
 
 def opt(atoms=None,gen='poscar.gen',fmax=0.3,step=100,
         optimizer=BFGS,
-        vdwnn=False,nn=True):
+        nomb=False,vdwnn=False,nn=True):
     if atoms is None:
        atoms = read(gen)
     atoms.calc = IRFF(atoms=atoms,libfile='ffield.json',rcut=None,
-                      nn=nn,vdwnn=vdwnn)
+                      nomb=nomb,nn=nn,vdwnn=vdwnn)
 
     def check(atoms=atoms):
         epot_      = atoms.get_potential_energy()
         r          = atoms.calc.r.detach().numpy()
         i_         = np.where(np.logical_and(r<0.5,r>0.0001))
         n          = len(i_[0])
 
@@ -37,19 +37,19 @@
     images     = Trajectory('opt.traj')
     # view(images[-1])
     return images
 
 
 def bhopt(atoms=None,gen='poscar.gen',fmax=0.3,step=100,dr=0.5,temperature=100,
           optimizer=BFGS,
-          vdwnn=False,nn=True,v=False):
+          nomb=False,vdwnn=False,nn=True,v=False):
     if atoms is None:
        atoms = read(gen)
     atoms.calc = IRFF(atoms=atoms,libfile='ffield.json',rcut=None,
-                      nn=nn,vdwnn=vdwnn)
+                      nomb=nomb,nn=nn,vdwnn=vdwnn)
 
     optimizer = BasinHopping(atoms=atoms,              # the system to optimize
                       temperature=temperature * kB,    # 'temperature' to overcome barriers
                       dr=dr,                           # maximal stepwidth
                       optimizer=optimizer,
                       fmax=fmax,                       # maximal force for the optimizer
                       trajectory="opt.traj")
@@ -73,18 +73,18 @@
 
     # Write jmol file if requested
     # if write_jmol:
     frequencies.write_jmol()
 
 
 def md(atoms=None,gen='poscar.gen',step=100,nn=True,ffield='ffield.json',initT=300,timeStep=0.1,
-       vdwnn=False,print_interval=1):
+       nomb=False,vdwnn=False,print_interval=1):
     irmd = IRMD(time_step=timeStep,totstep=step,atoms=atoms,gen=gen,Tmax=10000,
                 ro=0.8,rmin=0.5,initT=initT,vdwnn=vdwnn,print_interval=print_interval,
-                nn=nn,ffield=ffield)
+                nomb=nome,nn=nn,ffield=ffield)
     irmd.run()
 
     irmd.close()
     del irmd
     images = Trajectory('md.traj')
    #  if v:
    #     view(images[-1]) # ,viewer='x3d'
```

### Comparing `irff-1.5.2/irff/md/gofr.py` & `irff-1.5.3/irff/md/gofr.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/md/gulp.py` & `irff-1.5.3/irff/md/gulp.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 library reax;
 output movie xyz his.xyz;
 dump 100 restart.grs;
 
 '''
 
 def write_gulp_in(A, runword='gradient qiterative nosymmetry conv verb debu',
-                  T=298.0,
                   time_step=0.1,
                   tot_step=10.0,
                   maxcyc=2000,
                   output=None,
                   restart=100,
                   lib='reax',movieFrequency=10,**kwargs):
     ''' runword = keyword in gulp input
@@ -63,32 +62,34 @@
         #     print('tau_barostat       0.1 ps',file=finp)
         #     print('tau_thermostat     0.1 ps',file=finp)
         if 'ensemble' in kwargs:
             print('ensemble   =  {:s} '.format(kwargs['ensemble']), file=finp)
         if 'tau_thermostat' in kwargs:
             print('tau_thermostat   =  {:f} ps'.format(kwargs['tau_thermostat']), file=finp)
 
-        print('temperature        %f K' % T, file=finp)
+        # print('temperature        %f K' % T, file=finp)
         print('timestep           %f fs' % time_step, file=finp)
         print('production         %f ps' %
               float(tot_step*time_step/1000.0), file=finp)
         print('equilibration      0.0 ps', file=finp)
         print('write              1', file=finp)
         print('sample             1', file=finp)
-
+        
+    if 'T' in kwargs: 
+       print('temperature          {:f} K'.format(kwargs['T']),file=finp)
     if 'pressure' in kwargs:
        print('pressure          {:f} GPa'.format(kwargs['pressure']),file=finp)
 
     print('#', file=finp)
     print('title', file=finp)
     print('GULP calculation', file=finp)
     print('end', file=finp)
     print('#', file=finp)
     if lib == 'brenner':
-        print('%s' % lib, file=finp)
+        print('{:s}'.format(lib), file=finp)
     else:
         print('library %s' % lib, file=finp)
 
     if output is None:
         print('output movie {:d} xyz his.xyz'.format(
             movieFrequency), file=finp)
     else:
@@ -130,16 +131,30 @@
     for i in range(natom):
         line = lines[i+5+charge_line]
         l = line.split()
         q.append(float(l[2]))
     return q, ecoul, eself, evdw
 
 
-def get_reax_energy(fo='out'):
+def get_reax_energy(fo='out',e_kw='ReaxFF force field'):
     fout = open(fo, 'r')
+    e=0.0
+    ebond=0.0
+    elp=0.0
+    eover=0.0
+    eunder=0.0 
+    eang=0.0 
+    epen=0.0 
+    tconj=0.0 
+    etor=0.0 
+    fconj=0.0 
+    evdw=0.0 
+    ehb=0.0 
+    ecl=0.0 
+    esl = 0.0
     for line in fout.readlines():
         if line.find('E(bond)') >= 0:
             ebond = float(line.split()[2])
         elif line.find('E(lonepair)') >= 0:
             elp = float(line.split()[2])
         elif line.find('E(over)') >= 0:
             eover = float(line.split()[2])
@@ -159,16 +174,16 @@
             evdw = float(line.split()[2])
         elif line.find('E(hb)') >= 0:
             ehb = float(line.split()[2])
         elif line.find('E(coulomb)') >= 0:
             ecl = float(line.split()[2])
         elif line.find('E(self)') >= 0:
             esl = float(line.split()[2])
-        elif line.find('ReaxFF force field') >= 0:
-            e = float(line.split()[4])
+        elif line.find(e_kw) >= 0:
+            e = float(line.split()[-2])
     fout.close()
     return e, ebond, elp, eover, eunder, eang, epen, tconj, etor, fconj, evdw, ehb, ecl, esl
 
 def get_md_results(out='gulp.out'):
     ''' get the result from the  gulp MD simulation '''
     flog = open(out, 'r')
     E, Epot, T, P = [], [], [], []
@@ -495,27 +510,25 @@
             for i, f in enumerate(forces):
                 print('{:4d} {:12.8f} {:12.8f} {:12.8f}'.format(
                     i+1, f[0], f[1], f[2]), file=fsiesta)  # Why?
                 # print('{:4d} {:12.8f} {:12.8f} {:12.8f}'.format(i+1,f[0],f[1],f[2]),file=fsiesta)
     return np.array(forces)
 
 
-def get_gulp_forces(images, traj='gulp_force.traj', ffield='reaxff_nn', wforce=False):
+def get_gulp_forces(images, traj='gulp_force.traj', ffield='reaxff_nn',e_kw='ReaxFF force field', wforce=False):
     ''' calculate the force by GULP '''
     his = TrajectoryWriter(traj, mode='w')
     for atoms in images:
         write_gulp_in(atoms, runword='gradient nosymmetry conv qite verb',
                       output='drv gulp', restart=1,
                       lib=ffield)
         system('gulp<inp-gulp>out')
         forces = get_gulp_force_from_drv('gulp.drv', wforce=wforce)
         #atoms.forces = forces
         (e, eb_, el_, eo_, eu_, ea_, ep_,
-         etc_, et_, ef_, ev_, ehb_, ecl_, esl_) = get_reax_energy(fo='out')
+         etc_, et_, ef_, ev_, ehb_, ecl_, esl_) = get_reax_energy(fo='out',e_kw=e_kw)
         #e = atoms.get_potential_energy()
-        calc = SinglePointCalculator(atoms, energy=e,
-                                     forces=forces)
-
-        atoms.set_calculator(calc)
+        atoms.calc = SinglePointCalculator(atoms, energy=e,forces=forces)
+        # atoms.set_calculator(calc)
         his.write(atoms=atoms)
     his.close()
     return atoms
```

### Comparing `irff-1.5.2/irff/md/hugoniot.py` & `irff-1.5.3/irff/md/hugoniot.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/md/irmd.py` & `irff-1.5.3/irff/md/irmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from ..irff import IRFF
 from ..AtomDance import get_zmat_variable,get_zmat_angle,get_zmatrix,check_zmat
 from ase.io import read,write
 import numpy as np
 from ase.optimize import BFGS
 from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
 from ase.md.verlet import VelocityVerlet
-from ase.io.trajectory import Trajectory
+from ase.io.trajectory import Trajectory,TrajectoryWriter
 from ase import units
 
 
-
 def get_pressure(atoms):           
     ir = IRFF(atoms=atoms_md[-1],
             libfile='ffield.json',
             rcut=None,
             nn=True,
             CalStress=True)
     p = []
@@ -59,15 +58,16 @@
                bonds.append((i,j))
     return bonds
 
 
 class IRMD(object):
   ''' Intelligent Reactive Molecular Dynamics '''
   def __init__(self,label=None,atoms=None,gen='poscar.gen',ffield='ffield.json',
-               index=-1,totstep=100,vdwnn=False,nn=True,
+               index=-1,totstep=100,vdwnn=False,nn=True,nomb=False,
+               active=False,period=30,uncertainty=0.96,
                initT=300,Tmax=10000,time_step=0.1,Iter=0,
                ro=None,rmin=0.6,rmax=1.3,angmax=20.0,
                CheckZmat=False,zmat_id=None,zmat_index=None,InitZmat=None,
                learnpair=None,groupi=[],groupj=[],beta=None,freeatoms=None,
                dEstop=1000,dEtole=1.0,print_interval=1):
       self.Epot      = []
       self.epot      = 0.0
@@ -93,20 +93,24 @@
       self.dEtole    = dEtole
       self.learnpair = learnpair
       self.groupi    = groupi
       self.groupj    = groupj
       self.beta      = beta
       self.freeatoms = freeatoms
       self.print_interval = print_interval
+      self.active    = active        # an active leaning protocal for metal
+      self.uncertainty= uncertainty  # the limit of the uncertainty of bond length dirtribution
+      self.images    = []
+      self.rs        = []
 
       if self.atoms is None:
          self.atoms  = read(gen,index=index)
       
       self.atoms.calc= IRFF(atoms=self.atoms, mol=label,libfile=ffield,
-                            rcut=None,nn=nn,vdwnn=vdwnn)
+                            nomb=nomb,rcut=None,nn=nn,vdwnn=vdwnn)
       self.natom     = len(self.atoms)
       self.re        = self.atoms.calc.re
       self.dyn       = None
       self.atoms.calc.calculate(atoms=self.atoms)
       self.InitBonds = getBonds(self.natom,self.atoms.calc.r,self.rmax*self.re)
 
       if (self.atoms is None) and gen.endswith('.gen'):
@@ -119,15 +123,18 @@
             p    = scale * p
             self.atoms.set_momenta(p)
          else:
             MaxwellBoltzmannDistribution(self.atoms, self.initT*units.kB)
 
   def run(self):
       self.zv,self.zvlo,self.zvhi = None,0.0,0.0
-      self.dyn = VelocityVerlet(self.atoms, self.time_step*units.fs,trajectory='md.traj') 
+      if self.active:
+         self.dyn = VelocityVerlet(self.atoms, self.time_step*units.fs)
+      else:
+         self.dyn = VelocityVerlet(self.atoms, self.time_step*units.fs,trajectory='md.traj') 
       if (not self.learnpair is None) and (not self.beta is None):
          vij = self.atoms.positions[self.learnpair[1]] - self.atoms.positions[self.learnpair[0]]
          rij = np.sqrt(np.sum(np.square(vij)))
          vij = vij/rij
 
       self.dEstop_ = 0.0
 
@@ -203,14 +210,39 @@
                          bonds      = getBonds(self.natom,self.atoms.calc.r,1.19*self.re)
                          newbond    = self.checkBond(bonds)
                          if newbond: 
                             self.Deformed += 0.2
                             bonds      = getBonds(self.natom,self.atoms.calc.r,1.17*self.re)
                             newbond    = self.checkBond(bonds)
              self.zmats.append(zmat)
+          elif self.active:
+             self.images.append(a.copy())
+             bo0   =  a.calc.bo0.detach().numpy()
+             r     = a.calc.r.detach().numpy()
+             mask  = np.where(bo0>=0.0001,1,0)     # 掩码，用于过虑掉非成键键长
+            
+             
+             r_ = self.r*mask
+             r_ = r_[r_!=0]
+             self.rs.append(np.var(r_))
+             
+             if self.step%self.period==0:
+                self.rs.append(np.mean(r_))
+                try:
+                   assert self.uncertainty <= self.rs[-1], 'The varience is bigger than limit.'
+                except:
+                   print('The varience is bigger than limit, stop at %d.' %self.step)
+                   self.dyn.max_steps = self.dyn.nsteps-1
+               # n           = np.sum(mask)
+               # if np.mean(self.rs) > 0.01:
+               #    print(self.images)
+               #    break
+                r_          = []
+                self.images = []
+                self.rs     = []
           else:
              r    = a.calc.r.detach().numpy()
              i_   = np.where(np.logical_and(r<self.rmin*self.ro,r>0.0001))
              n    = len(i_[0])
 
           if len(self.Epot)==0:
              dE_ = 0.0
@@ -312,14 +344,19 @@
                  print('potential energy is NAN, stop at %d.' %self.step)
              else:
                  print('unknown reason, stop at %d.' %self.step)
              self.dyn.max_steps = self.dyn.nsteps-1
   
       self.dyn.attach(check,interval=1)
       self.dyn.run(0.00001,self.totstep)
+      if active:
+         traj  = TrajectoryWriter('md.traj',mode='w')
+         for atoms in self.images:
+             traj.write(atoms=atoms)
+         traj.close()
       return self.Deformed,self.zmats,self.zv,self.zvlo,self.zvhi
 
   def checkBond(self,bonds):
       newbond = False
       for bd in bonds:
           bd_ = (bd[1],bd[0])
           if (bd not in self.InitBonds) and (bd_ not in self.InitBonds):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `irff-1.5.2/irff/md/lammps.py` & `irff-1.5.3/irff/md/lammps.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/ml/data.py` & `irff-1.5.3/irff/ml/data.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/ml/evaluate_data.py` & `irff-1.5.3/irff/ml/evaluate_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-# import csv
 import pandas as pd
+import random
 from os.path import isfile
 from os import listdir,getcwd
 import numpy as np
+from sklearn.cluster import KMeans
 from .ffield import ffield_to_csv,update_ffield #,get_csv_data
 from ..data.ColData import ColData
 from ..reax import ReaxFF 
-#from ..dft.CheckEmol import check_emol
 
-# parameters = ['boc1','boc2','boc3','boc4','boc5',
-#               'rosi','ropi','ropp','Desi','Depi','Depp',
-#               'be1','be2','bo1','bo2','bo3','bo4','bo5','bo6',
-#               'valboc','val3','val5','val6','val8','val9','val10',
-#               'ovun1','ovun2','ovun3','ovun4','ovun5','ovun6','ovun7','ovun8',
-#               'lp1','lp2','coa2','coa3','coa4','pen2','pen3','pen4',
-#               'tor2','tor3','tor4','cot2',
-#               'rvdw','gammaw','Devdw','alfa','vdw1',
-#               'rohb','Dehb','hb1','hb2']
 
 def init_ffield_csv(fcsv,parameters=['boc1','boc2','boc3','boc4','boc5',
                     'rosi','ropi','ropp','Desi','Depi','Depp',
                     'be1','be2','bo1','bo2','bo3','bo4','bo5','bo6',
                     'valboc','val3','val5','val6','val8','val9','val10',
                     'ovun1','ovun2','ovun3','ovun4','ovun5','ovun6','ovun7','ovun8',
                     'lp1','lp2','coa2','coa3','coa4','pen2','pen3','pen4',
@@ -37,15 +28,15 @@
                     'rosi','ropi','ropp','Desi','Depi','Depp',
                     'be1','be2','bo1','bo2','bo3','bo4','bo5','bo6',
                     'valboc','val3','val5','val6','val8','val9','val10',
                     'ovun1','ovun2','ovun3','ovun4','ovun5','ovun6','ovun7','ovun8',
                     'lp1','lp2','coa2','coa3','coa4','pen2','pen3','pen4',
                     'tor2','tor3','tor4','cot2',
                     'rvdw','gammaw','Devdw','alfa','vdw1'],
-             evaluate_ffield=True,scale=1.0,pop=20,
+             evaluate_ffield=True,scale=1.0,pop=20,n_clusters=1,
              step=1000,print_step=100,writelib=500):
     ''' evaluate the score of the parameter set in csv file '''
     if not isfile(fcsv):
        # init_ffield_csv(fcsv,parameters=parameters)
        pna,row = ffield_to_csv(ffield='ffield.json',fcsv=fcsv,parameters=parameters) 
        
        scale_  = []                                                 # 创建初始参数分布
@@ -66,27 +57,59 @@
 
        X = np.random.normal(loc=r_, scale=scale_, size=(pop, ndim))  # 初始参数分布
        with open(fcsv,'a') as f:
             for i,x in enumerate(X):
                 print(i+1,end=',',file=f)
                 for x_ in x:
                     print(x_,end=',',file=f)
-                print(-99999999999.9,file=f)                                   # 得分为-999，需要重新评估
-
+                print(-99999999999.9,file=f)                         # 得分<-999，需要重新评估
+    else:
+       if n_clusters>1:
+          d   = pd.read_csv(fcsv)
+          columns        = d.columns
+          for c in columns:                                ### Check Data
+              col_ = c.split()
+              if len(col_)>0:
+                 col = col_[0]
+                 if col == 'Unnamed:':
+                    d.drop(c,axis=1,inplace=True)          ### Delete Unnamed column
+          X   = d.values[:,:-1]
+          #Y  = d.values[:, -1]
+          random.seed()
+          len_ = X.shape[0]
+          n_   = n_clusters if len_>n_clusters else len_
+          kmeans = KMeans(n_clusters=n_, random_state=random.randint(0,10)).fit(X)
+          #print(kmeans.labels_)
+          #print(kmeans.cluster_centers_)
+          clusters = {}            # 取第一次出现的元素为核心，前面的元素分值高，排序好的数据
+          for i,l in enumerate(kmeans.labels_):
+              if l not in clusters:
+                 clusters[l] = i
+              
+          pna,row = ffield_to_csv(ffield='ffield.json',fcsv=fcsv,parameters=parameters,mode='w') 
+          with open(fcsv,'a') as f:
+             for i in clusters:
+                 i_ = clusters[i]
+                 x      = X[i_]
+                 print(i+1,end=',',file=f)
+                 for x_ in x:
+                     print(x_,end=',',file=f)
+                 print(-99999999999.9,file=f)
+                 
     d              = pd.read_csv(fcsv)
     columns        = d.columns
 
     for c in columns:                                                ### Check Data
         col_ = c.split()
         if len(col_)>0:
            col = col_[0]
            if col == 'Unnamed:':
               d.drop(c,axis=1,inplace=True)                          ### Delete Unnamed column
 
-    columns        = d.columns
+    columns = d.columns
     if evaluate_ffield:                                              ### whether evaluate the current ffield
        if not model is None:                                         ### evaluate the score of current ffield
           model.update(p=None,reset_emol=True)
           model.get_zpe()
           model.update(p=None,reset_emol=False)
           model.run(learning_rate=1.0e-4,step=step,print_step=print_step,
                     writelib=writelib,close_session=False)
```

### Comparing `irff-1.5.2/irff/ml/evolution.py` & `irff-1.5.3/irff/ml/evolution.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import random
 import numpy as np
 import types
+from sklearn.cluster import KMeans
 
 
 class Evolution:
     def __init__(self, func, n_dim, F=0.5,
                  size_pop=50, max_iter=200, prob_mut=0.5,
-                 X_input=None,scale=None,
+                 X_input=None,scale=None,n_clusters=1,
                  constraint_eq=tuple(), constraint_ueq=tuple()):
         self.func = func # func_transformer(func)
         assert size_pop % 2 == 0, 'size_pop must be even integer'
         self.size_pop       = size_pop               # size of population
         self.max_iter       = max_iter
         self.prob_mut       = prob_mut               # probability of mutation
         self.n_dim          = n_dim
@@ -37,42 +39,63 @@
         # self.create_ratio = create_ratio
         self.X_input = X_input
         self.F = F
         self.size_pop=size_pop
         self.V, self.U = None, None
         # self.lb, self.ub = np.array(lb) * np.ones(self.n_dim), np.array(ub) * np.ones(self.n_dim)
         self.scale = scale
+        self.n_clusters = n_clusters
         self.crtbp()
 
     def crtbp(self):
         '''
           创建初始                  族群: self.X     
           create the inital population: self.X
         '''
-        len_    = len(self.X_input)
+        len_       = len(self.X_input)
+        n_clusters = self.n_clusters if len_>self.n_clusters else len_
         pop_       = self.size_pop - len_
         self.X     = self.X_input
         Y_         = self.x2y()
         min_y_id   = np.argmin(Y_)
         X_template = self.X_input[min_y_id]          # generate data with Gaussian distribution at X_template 
 
         self.generation_best_X.append(X_template)
         self.generation_best_Y.append(Y_[min_y_id])
 
         if pop_>0:
            # X_    = np.random.uniform(low=self.lb, high=self.ub, size=(pop_, self.n_dim))  
            # Using a Gaussian Distribution instead of uniform distrution 使用高斯分布代替均匀分布
-           X_      = np.random.normal(loc=X_template, scale=self.scale, size=(pop_, self.n_dim))
-           merge_  = np.vstack([self.X_input,X_])
-           self.X  = merge_
+           XS = [self.X_input]
+           size_ = int(pop_/n_clusters)
+
+           if n_clusters>1:
+              random.seed()
+              clusters = {}
+              kmeans = KMeans(n_clusters=n_clusters, random_state=random.randint(0,10)).fit(self.X)
+              for i,l in enumerate(kmeans.labels_):
+                  if l not in clusters:
+                     clusters[l] = i
+              
+              for i,x in enumerate(clusters):
+                  i_ = clusters[x]
+                  size   = size_  if i != (n_clusters-1) else pop_-size_*i
+                  X_     = np.random.normal(loc=self.X[i_], scale=self.scale, size=(size, self.n_dim))
+                  XS.append(X_)
+           else:
+              X_  = np.random.normal(loc=X_template, scale=self.scale, size=(pop_, self.n_dim))
+              XS.append(X_)
+           self.X  = np.vstack(XS)
+
         elif pop_==0:
            self.X = self.X_input
         else:
            raise RuntimeError('The current population is larger than max defination!')
         # print('The length of current population:',len(self.X))
+        assert len(self.X)==self.size_pop,'Error: the length of the population is not equal to it set value!'
         return self.X
 
     def register(self, operator_name, operator, *args, **kwargs):
         '''
         regeister udf to the class
         :param operator_name: string
         :param operator: a function, operator itself
@@ -161,13 +184,13 @@
             self.all_history_Y.append(self.Y)
             # if i%5==0:
             #    print(' ',file=logfile)
             # print(' {:9.6f} '.format(self.generation_best_Y[-1]),end='',file=logfile)
 
         # print('\n----------------------------------------------------------------',file=logfile)
         # print('',file=logfile)
-        global_best_index = np.array(self.generation_best_Y).argmin()
-        global_best_X = self.generation_best_X[global_best_index]
+        self.global_best_index = np.array(self.generation_best_Y).argsort()
+        global_best_X = self.generation_best_X[self.global_best_index[0]]
         global_best_Y = self.func(np.array([global_best_X]))
         return global_best_X, global_best_Y
```

### Comparing `irff-1.5.2/irff/ml/ffield.py` & `irff-1.5.3/irff/ml/ffield.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #from irff.reaxfflib import read_ffield,write_ffield
 import json as js
 import csv
-import pandas as pd
+# import pandas as pd
 from os.path import isfile
 from os import listdir
 
 
 # def init_ffield_csv():
 #     # path='/home/miao/PycharmProjects/scsslh'
 #     files=os.listdir(path)
@@ -41,15 +41,15 @@
         if key in p_:
            p = p_[key]*unit if k in punit else p_[key]
            j['p'][key] = p         
 
     with open('ffield.json','w') as fj:
          js.dump(j,fj,sort_keys=True,indent=2)
 
-def ffield_to_csv(ffield='ffield.json',parameters=None,keys=None,fcsv='ffield.csv'):
+def ffield_to_csv(ffield='ffield.json',parameters=None,keys=None,fcsv='ffield.csv',mode='a'):
     with open(ffield,'r') as lf:
          j  = js.load(lf)
          p_ = j['p']
          try:
             score = j['score']
          except:
             score = -1000
@@ -144,21 +144,21 @@
            if key:               # 过虑空列
               p_name.append(key)
 
     already_exist = False
     if isfile(fcsv):
        already_exist = True
 
-    if already_exist: 
+    if already_exist and mode!='w': 
        fcsv_ = open(fcsv,'a')
     else:
        fcsv_ = open(fcsv,'w')
     csv_write = csv.writer(fcsv_)
 
-    if not already_exist:
+    if not already_exist or mode=='w':
        csv_write.writerow(p_name)
     
     row = ['0'] # if already_exist else []
     for key in p_name:
         if key:
            if key=='score':
               s = '{:.4f}'.format(score)
@@ -166,18 +166,18 @@
               s = '{:.4f}'.format(p_[key])
            row.append(s)
 
     csv_write.writerow(row)
     fcsv_.close()
     return p_name,row
 
-def get_csv_data(fcsv):
-    d = pd.read_csv(fcsv)
-    # print(d['boc1'])
-    return d
+# def get_csv_data(fcsv):
+#     d = pd.read_csv(fcsv)
+#     # print(d['boc1'])
+#     return d
 
 def init_bonds(p_):
     spec,bonds,offd,angs,torp,hbs = [],[],[],[],[],[]
     for key in p_:
         # key = key.encode('raw_unicode_escape')
         # print(key)
         k = key.split('_')
```

### Comparing `irff-1.5.2/irff/ml/fit.py` & `irff-1.5.3/irff/ml/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import pandas as pd
 import matplotlib
 import matplotlib.pyplot as plt
 from scipy.optimize import minimize_scalar
 from irff.ml.data import get_data
 from irff.data.ColData import ColData
-from irff.initCheck import init_bonds
+from irff.intCheck import init_bonds
 tf.compat.v1.disable_eager_execution()
 
 
 def resolve():
     res = minimize_scalar(func,method='brent')
     print(res.x)
     t = sigmoid(0.8813735870089523)
```

### Comparing `irff-1.5.2/irff/ml/fluctuation.py` & `irff-1.5.3/irff/ml/fluctuation.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/ml/gaqeq.py` & `irff-1.5.3/irff/ml/gaqeq.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/ml/genetic.py` & `irff-1.5.3/irff/ml/genetic.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/ml/gpfit_tfv2.py` & `irff-1.5.3/irff/ml/gpfit_tfv2.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/ml/harmonic.py` & `irff-1.5.3/irff/ml/harmonic.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/ml/train.py` & `irff-1.5.3/irff/ml/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,34 @@
                to_evaluate=-998,
            evaluate_ffield=True,
            lossConvergence=30.0,
                max_ml_iter=2000,
             max_generation=500,
                   size_pop=500,
                   init_pop=10,
+                n_clusters=1,
                   prob_mut=0.5,
                  potential=None,
                    trainer=None,
                 parameters=['boc1','boc2'],
                      scale={},
             variable_scale=0,
              max_data_size=1000,
+                regenerate=False,
           end_search_ratio=0.999999,
             end_search_nan=False,
                GAThreshold=0.5):
     ''' Using machine learing model to assis the training of ReaxFF'''
     scoreConvergence = - lossConvergence
 
     d = evaluate(model=potential,trainer=trainer,
                  fcsv=fcsv,to_evaluate=to_evaluate,
                  step=evaluate_step,print_step=print_step,writelib=writelib,
                  evaluate_ffield=evaluate_ffield,pop=init_pop,scale=scale,
-                 parameters=parameters)
+                 n_clusters=n_clusters,parameters=parameters)
     d.sort_values(axis=0,by='score',ascending=False,inplace=True)
 
     X       = d.values[:, : -1]
     Y       = d.values[:, -1]
     columns = d.columns
     new_row = {}
     zrow    = d.index[0]
@@ -76,14 +78,21 @@
          print(new_row,file=galog)
 
     it_       = 0
     score     = scoreConvergence - 0.1
     do_gen    = True
     keep_best = 0
     while score<scoreConvergence and it_< max_ml_iter:
+        if step>0 and it_>0:
+           d = evaluate(model=potential,trainer=trainer,
+                        fcsv=fcsv,to_evaluate=0.0,
+                        step=evaluate_step,
+                        evaluate_ffield=False,
+                        n_clusters=1,parameters=parameters)
+           d.sort_values(axis=0,by='score',ascending=False,inplace=True)
         size_ = d.shape[0]
         zrow  = d.index[0]
         sizepop = int(size_pop/2)
         if size_ > sizepop:
            size_ = sizepop
         X_ = d.values[:size_, : -1]
         X   = d.values[:, : -1]
@@ -91,19 +100,19 @@
 
         ml_model.fit(X,Y)
         score_ = ml_model.score(X,Y) 
         feature_importances = ml_model.feature_importances_
         max_ = max(feature_importances)
 
         if variable_scale==2 and score_>0.98:
-           _scale = scale_*np.random.choice([0.1,1.0,10.0])*feature_importances*feature_importances/(max_*max_)
-        elif variable_scale>=1 and score_>0.94:
-           _scale = scale_*np.random.choice([0.1,1.0,10.0])*feature_importances/max_
+           _scale = scale_*feature_importances*feature_importances/(max_*max_) # *np.random.choice([0.1,1.0,10.0])
+        elif variable_scale>=1 and score_>0.96:
+           _scale = scale_*feature_importances/max_ # *np.random.choice([0.1,1.0,10.0])
         else:
-           _scale = scale_*np.random.choice([0.1,1.0,10.0])
+           _scale = scale_ # *np.random.choice([0.1,1.0,10.0])
 
         galog = open('evolution.log','a')
         print('\n           ----------------------------------',file=galog)
         print('                   Iteration: {:6d} '.format(it_),file=galog)
         print('           ----------------------------------\n',file=galog)
 
         print('\n  The accuraccy of the mathine learning model: {:f}'.format(score_),file=galog)
@@ -117,40 +126,43 @@
         ## PSO DE GMM
         if do_gen:
            print('  Do genetic recommendation ...\n',file=galog)
            # gentic_start_time = time.time()
            # lb=0.9*np.min(X_,axis=0)
            # ub=1.1*np.max(X_,axis=0)
            de = Evolution(func,n_dim=X_.shape[1], F=0.5,size_pop=size_pop,
-                          scale=_scale,max_iter=max_generation, 
+                          scale=_scale,max_iter=max_generation, n_clusters=n_clusters,
                           prob_mut=prob_mut,X_input=X_)    
 
            best_x,best_y = de.run(logfile=galog)                     ###   PSO GMM
            print('  The guessed score of best candidate: {:f} '.format(float(-best_y)),file=galog) 
            print('  The score of last best             : {:f} '.format(d.loc[zrow, 'score']),file=galog) 
            print('\n  The parameter vector: ',file=galog)
            for i_,x_ in enumerate(best_x):
                if i_%3==0:
                   print('\n--------------------------------------------------------------------------------------',file=galog)
                cn = columns[i_]
                best_x[i_] = x_ = float('{:.6f}'.format(x_))
                print('{:16s} {:9.6f} |'.format(cn,x_),end=' ',file=galog)
            print('\n--------------------------------------------------------------------------------------',file=galog)
-           keep_ = True
-           while keep_:
+           keep_ = True if step==0 else False
+           cycle = 0 
+           while keep_ and cycle<10:
                for i,key in enumerate(columns):
                    if key != 'score':
                       if abs(new_row.loc[0,key] - best_x[i])>=0.000001:
                          keep_ = False
                          print('                {:16s} {:9.6f} -> {:9.6f}'.format(key,new_row.loc[0,key],best_x[i]),file=galog)
                if keep_: 
-                  print(' The parameter vector keep best, a random parameter set is chosen ...',file=galog)
-                  i = np.random.choice(de.size_pop)
-                  best_x = de.X[i]
-                  best_y = de.Y[i]
+                  # print(' The parameter vector keep best, a random parameter set is chosen ...',file=galog)
+                  print(' The parameter vector keep best, a second best parameter set is chosen ...',file=galog)
+                  # i = np.random.choice(de.size_pop)
+                  cycle += 1
+                  best_x = de.X[de.global_best_index[cycle]]
+                  best_y = de.Y[de.global_best_index[cycle]]
         else:
            print('  The score of current parameters set looks good, need not do the genetic step.',file=galog)
         print('--------------------------------------------------------------------------------------',file=galog)
         # gentic_end_time = time.time()
         # print('\n  The time usage of genetic recommendation: {:f}'.format(gentic_end_time-gentic_start_time),file=galog)
         if do_gen:
            for i,key in enumerate(columns):
@@ -222,12 +234,13 @@
             
         print('  Saving the data to {:s} ...'.format(fcsv),file=galog)
         if keep_best>4 and ratio>=end_search_ratio:
            print('\n  The current parameter vector keep best for iterations, the search is end.',file=galog)
            break
            
         d.to_csv(fcsv)
-        it_ += 1
         if it_>= max_ml_iter:
            print('\n  The maximum iterations have reached, the search is end.',file=galog)
         galog.close()
 
+        it_ += 1
+
```

### Comparing `irff-1.5.2/irff/mlqeq.py` & `irff-1.5.3/irff/mlqeq.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/molecule.py` & `irff-1.5.3/irff/molecule.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/mpnn.py` & `irff-1.5.3/irff/mpnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,19 +130,19 @@
                batch_size=200,sample='uniform',
                hbshort=6.75,hblong=7.5,
                vdwcut=10.0,
                beup={},                          # e.g. {'C-C':[(1.5,0.5)]} or {'C-C':[(1.5,'si')]}
                belo={},
                vlo={'others':[(0.0,0.0)]},
                vup={'others':[(10.0,0.0)]},
-               pim={'others':10.0},
+               # pim={'others':10.0},
                spv_be=False,                             
-               spv_bo=None,                      # e.g. spv_bo={'C-C':(1.3,0.2,1.0)}
-               spv_pi=False,
-               spv_ang=False,
+               spv_bo=None,                      # e.g. spv_bo={'C-C':[(1.3,7.0,8.0,0,11,0.2,1.0)]}
+               spv_pi=False,                     # e.g. spv_pi={'C-C-C':[(7.5,8.5,0.8,1.8)]}
+               #spv_ang=False,                    
                spv_vdw=False,
                fixrcbo=False,
                weight={'others':1.0},
                ro_scale=0.1,
                clip_op=True,
                clip={},
                InitCheck=True,
@@ -151,20 +151,20 @@
                be_universal_nn=None,be_layer=[9,0],
                bo_universal_nn=None,bo_layer=None,   # [6,0]
                mf_universal_nn=None,mf_layer=[9,0],
                vdw_universal_nn=None,vdw_layer=None, # [9,0]
                vdwnn=False,VdwFunction=1,
                BOFunction=0,
                EnergyFunction=1,
-               MessageFunction=3,
+               MessageFunction=2,
                spec=[],
                lambda_bd=100000.0,
                lambda_pi=1.0,
                lambda_reg=0.01,
-               lambda_ang=1.0,
+               #lambda_ang=1.0,
                fluctuation=0.0,
                regularize_bo=True,
                regularize_be=True,
                regularize_mf=True,
                regularize_vdw=False,
                regularize_bias=False,
                optMethod='ADAM',
@@ -183,21 +183,21 @@
            Intelligence ReaxFF Neual Network: Evoluting the Force Field parameters on-the-fly
            2017-11-01
       '''
       self.messages         = messages
       self.EnergyFunction   = EnergyFunction
       self.MessageFunction  = MessageFunction
       self.BOFunction       = BOFunction
-      self.pim              = pim
+      #self.pim              = pim
       self.spv_bo           = spv_bo
       self.spv_be           = spv_be
       self.beup             = beup
       self.belo             = belo
       self.spv_pi           = spv_pi
-      self.spv_ang          = spv_ang
+      #self.spv_ang         = spv_ang
       self.spv_vdw          = spv_vdw
       self.vup              = vup
       self.vlo              = vlo
       self.fixrcbo          = fixrcbo
       self.regularize_be    = regularize_be
       self.regularize_bo    = regularize_bo
       self.regularize_mf    = regularize_mf
@@ -205,15 +205,15 @@
       self.regularize_bias  = regularize_bias
       if regularize_vdw or regularize_mf or regularize_bo or regularize_be:
          self.regularize    = True
       else:
          self.regularize    = False
       self.lambda_reg       = lambda_reg
       self.lambda_pi        = lambda_pi
-      self.lambda_ang       = lambda_ang
+      #self.lambda_ang      = lambda_ang
       self.fluctuation      = fluctuation
       self.mf_layer         = mf_layer
       self.be_layer         = be_layer
       self.vdw_layer        = vdw_layer if vdwnn else None
 
       self.bo_universal_nn   = bo_universal_nn
       self.be_universal_nn   = be_universal_nn
@@ -276,15 +276,18 @@
           else:
              raise NotImplementedError('-  This function not supported yet!')
 
           sum_edft = tf.reduce_sum(input_tensor=tf.abs(self.dft_energy[mol]-self.max_e[mol]))
           self.accur[mol] = 1.0 - tf.reduce_sum(input_tensor=tf.abs(self.E[mol]-self.dft_energy[mol]))/(sum_edft+0.00000001)
          
           self.Loss     += self.loss[mol]*w_
-          self.accuracy += self.accur[mol]
+          if mol.find('nomb_')<0:
+             self.accuracy += self.accur[mol]
+          else:
+             self.nmol -= 1
 
       self.ME   = 0.0
       for mol in self.mols:
           mols = mol.split('-')[0] 
           self.ME += tf.square(self.MolEnergy[mols])
 
       if self.pseudo_data:
@@ -465,17 +468,21 @@
          Fsi,Fpi,Fpp = tf.unstack(F,axis=2)
          bosi = self.Hsi[t-1][bd]*Fsi
          bopi = self.Hpi[t-1][bd]*Fpi
          bopp = self.Hpp[t-1][bd]*Fpp
       elif self.MessageFunction==2:
          self.Dbi[bd]  = Di-h
          self.Dbj[bd]  = Dj-h
-         Fi   = fmessage(flabel,b[0],self.nbd[bd],[self.Dbi[bd],self.Dbj[bd],self.Hsi[t-1][bd],self.Hpi[t-1][bd],self.Hpp[t-1][bd]],
+         # Fi   = fmessage(flabel,b[0],self.nbd[bd],[self.Dbi[bd],self.Dbj[bd],self.Hsi[t-1][bd],self.Hpi[t-1][bd],self.Hpp[t-1][bd]],
+         #                      self.m,batch=self.batch,layer=self.mf_layer[1])
+         # Fj   = fmessage(flabel,b[1],self.nbd[bd],[self.Dbj[bd],self.Dbi[bd],self.Hsi[t-1][bd],self.Hpi[t-1][bd],self.Hpp[t-1][bd]],
+         #                      self.m,batch=self.batch,layer=self.mf_layer[1])
+         Fi   = fmessage(flabel,b[0],self.nbd[bd],[self.Dbi[bd],h,self.Dbj[bd]],
                               self.m,batch=self.batch,layer=self.mf_layer[1])
-         Fj   = fmessage(flabel,b[1],self.nbd[bd],[self.Dbj[bd],self.Dbi[bd],self.Hsi[t-1][bd],self.Hpi[t-1][bd],self.Hpp[t-1][bd]],
+         Fj   = fmessage(flabel,b[1],self.nbd[bd],[self.Dbj[bd],h,self.Dbi[bd]],
                               self.m,batch=self.batch,layer=self.mf_layer[1])
          F    = Fi*Fj
          Fsi,Fpi,Fpp = tf.unstack(F,axis=2)
 
          bosi = self.Hsi[t-1][bd]*Fsi
          bopi = self.Hpi[t-1][bd]*Fpi
          bopp = self.Hpp[t-1][bd]*Fpp
@@ -821,15 +828,15 @@
              layer['fm'] = self.mf_layer[1]#+str(t)
 
       self.penalty_bop,self.penalty_bo = {},{}
       self.penalty_bo_rcut = {}
       self.penalty_pi,self.penalty_ang = {},{}
       self.penalty_vdw = {} 
       self.penalty_be_cut,self.penalty_be = {},{}
-      self.penalty_s_bo,self.penalty_s = {},{}
+      self.penalty_s = {} #,{}
       self.penalty_rcut = {}
 
       for bd in self.bonds: 
           atomi,atomj = bd.split('-') 
           bdr = atomj + '-' + atomi
           # log_ = tf.math.log((self.botol/(1.0 + self.botol)))
           if self.fixrcbo:
@@ -911,21 +918,30 @@
              if self.spv_bo:
                 #fe_ = tf.where(tf.greater(self.S[bd],0.00001),1.0,0.0) 
                 #self.penalty_s[bd]  = tf.reduce_sum(input_tensor=self.bo0[bd]*fe_)
                 #penalty  = tf.add(self.penalty_s[bd]*self.lambda_bd,penalty)      ## penalty iterm for bond order
                 self.penalty_bo[bd] = tf.constant(0.0)
                 if (bd in self.spv_bo) or (bdr in self.spv_bo):
                    bd_  = bd if bd in self.spv_bo else bdr
-                   r    = self.spv_bo[bd_][0]
-                   bo_l = self.spv_bo[bd_][1]
-                   bo_u = self.spv_bo[bd_][2]
-                   fe   = tf.where(tf.less_equal(self.rbd[bd],r),1.0,0.0) ##### r< r_e that bo > bore_
-                   self.penalty_bo[bd] += tf.reduce_sum(input_tensor=tf.nn.relu((bo_l-self.bop[bd])*fe))
-                   fe   = tf.where(tf.greater_equal(self.rbd[bd],r),1.0,0.0) ##### r< r_e that bo > bore_
-                   self.penalty_bo[bd] += tf.reduce_sum(input_tensor=tf.nn.relu((self.bop[bd]-bo_u)*fe))
+                   for sbo in self.spv_bo[bd_]:
+                       r,dil,diu,djl,dju,bo_l,bo_u = sbo
+                       fe   = tf.where(tf.logical_and(tf.less_equal(self.rbd[bd],r),
+                                                      tf.logical_and(tf.logical_and(tf.greater_equal(self.Dbi[bd],dil),
+                                                                                    tf.greater_equal(self.Dbj[bd],djl)), 
+                                                                     tf.logical_and(tf.less_equal(self.Dbi[bd],diu),
+                                                                                    tf.less_equal(self.Dbj[bd],dju))  ) ),
+                                       1.0,0.0)   ##### r< r_e that bo > bore_
+                       self.penalty_bo[bd] += tf.reduce_sum(input_tensor=tf.nn.relu((bo_l-self.bo0[bd])*fe))
+                       fe   = tf.where(tf.logical_and(tf.greater_equal(self.rbd[bd],r),
+                                                      tf.logical_and(tf.logical_and(tf.greater_equal(self.Dbi[bd],dil),
+                                                                                    tf.greater_equal(self.Dbj[bd],djl)), 
+                                                                     tf.logical_and(tf.less_equal(self.Dbi[bd],diu),
+                                                                                    tf.less_equal(self.Dbj[bd],dju))  ) ),
+                                       1.0,0.0)  ##### r> r_e that bo < bore_
+                       self.penalty_bo[bd] += tf.reduce_sum(input_tensor=tf.nn.relu((self.bo0[bd]-bo_u)*fe))
 
                 penalty  = tf.add(self.penalty_bo[bd]*self.lambda_bd,penalty) 
 
              if self.EnergyFunction != 3: # or self.EnergyFunction == 4 or self.EnergyFunction == 2:
                 fesi = tf.where(tf.less_equal(self.bo0[bd],self.botol),1.0,0.0) ##### bo <= 0.0 that e = 0.0
                 self.penalty_be_cut[bd]  = tf.reduce_sum(tf.nn.relu(self.esi[bd]*fesi))
                 penalty  = tf.add(self.penalty_be_cut[bd]*self.lambda_bd,penalty)
@@ -961,32 +977,28 @@
                    for vlo_ in self.vlo[bd_]:
                        r_,ev_l = vlo_
                        fl      = tf.where(tf.greater(self.rv[bd],r_),1.0,0.0) #####
                        pen_v   = tf.reduce_sum(input_tensor=tf.nn.relu((ev_l - self.EVDW[bd])*fl))
                        self.penalty_vdw[bd] = self.penalty_vdw[bd] + pen_v
                 penalty  = tf.add(self.penalty_vdw[bd]*self.lambda_bd,penalty)
 
-          # for sp in self.spec: 
-          #     pi_ = self.pim[sp] if sp in self.pim else self.pim['others']
-          #     if self.nsp[sp]>0:
-          #        self.penalty_pi[sp] = tf.reduce_sum(input_tensor=tf.nn.relu(self.Dpi[sp]-pi_))
-          #        penalty  = tf.add(self.penalty_pi[sp]*self.lambda_pi,penalty)
       if self.optword.find('noang')<0:
-         for ang in self.angs: 
-             if self.nang[ang]>0:
-                if self.spv_pi:
-                   pi_ = self.pim[ang] if ang in self.pim else self.pim['others']
-                   self.penalty_pi[ang] = tf.reduce_sum(input_tensor=tf.nn.relu(self.SBO[ang]-pi_))
+         if self.spv_pi:                        # regularize pi term
+            for ang in self.spv_pi: 
+                if self.nang[ang]>0:
+                   self.penalty_pi[ang] = tf.constant(0.0)
+                   for spi in self.spv_pi[ang]:
+                       Dl,Du,pil,piu = spi
+                       fpi = tf.where(tf.logical_and(tf.less_equal(self.D_p[ang],Du), 
+                                                    tf.greater_equal(self.D_p[ang],Dl)),
+                                       1.0,0.0)  
+                       self.penalty_pi[ang]+= tf.reduce_sum(input_tensor=tf.nn.relu((self.SBO[ang]-piu)*fpi))
+                       self.penalty_pi[ang]+= tf.reduce_sum(input_tensor=tf.nn.relu((pil-self.SBO[ang])*fpi))
                    penalty  = tf.add(self.penalty_pi[ang]*self.lambda_pi,penalty)
-                if self.spv_ang:
-                   self.penalty_ang[ang] = tf.reduce_sum(self.thet2[ang]*self.fijk[ang])
-                   penalty  = tf.add(self.penalty_ang[ang]*self.lambda_ang,penalty)
 
-         # self.penalty_pi = tf.reduce_sum(input_tensor=tf.nn.relu(self.DPI-2.0)) 
-         # penalty  = tf.add(self.penalty_pi*self.lambda_pi,penalty)
       if self.regularize:                              # regularize
          for sp in self.spec:
              for k in wb_message:
                  for k_ in w_n:
                      key     = k + k_ + '_' + sp
                      pen_w  += tf.reduce_sum(tf.square(self.m[key]))
                  if self.regularize_bias:
@@ -1000,19 +1012,19 @@
          penalty = tf.add(self.lambda_reg*pen_w,penalty)
          penalty = tf.add(self.lambda_reg*pen_b,penalty)
       return penalty
 
   def get_pentalty(self):
       (penalty_bop,penalty_bo,penalty_bo_rcut,
           penalty_be_cut,penalty_be,
-          penalty_s,penalty_s_bo,
+          penalty_s,
           penalty_rcut,rc_bo,
           penalty_vdw) = self.sess.run([self.penalty_bop,self.penalty_bo,self.penalty_bo_rcut,
                                          self.penalty_be_cut,self.penalty_be,
-                                         self.penalty_s,self.penalty_s_bo,self.penalty_rcut,self.rc_bo,
+                                         self.penalty_s,self.penalty_rcut,self.rc_bo,
                                          self.penalty_vdw],
                                         feed_dict=self.feed_dict)
       rcut = self.rcut
       print('\n------------------------------------------------------------------------')
       print('-                                                                      -')
       print('-                         Penalty Information                          -')
       print('-                                                                      -')
@@ -1026,16 +1038,16 @@
              print('Differency between rcut-bo and rcut Penalty of    {:5s}: {:6.4f} {:6.4f} {:6.4f}'.format(bd,penalty_bo_rcut[bd],rc_bo[bd],rcut[bd]))
           # if bd in penalty_esi:
           #    print('Differency between bosi and esi Penalty of      {:5s}: {:6.4f}'.format(bd,penalty_esi[bd]))
           if bd in penalty_be_cut: 
              print('Bond-Energy at radius cutoff penalty of           {:5s}: {:6.4f}'.format(bd,penalty_be_cut[bd]))
           if bd in penalty_be: 
              print('Bond-Energy fluctuation penalty of                {:5s}: {:6.4f}'.format(bd,penalty_be[bd]))
-          if bd in penalty_s_bo:
-             print('Penalty of Bond-Order should greater than zero of {:5s}: {:6.4f}'.format(bd,penalty_s_bo[bd]))
+          # if bd in penalty_s_bo:
+          #   print('Penalty of Bond-Order should greater than zero of {:5s}: {:6.4f}'.format(bd,penalty_s_bo[bd]))
           if bd in penalty_s:
              print('Anti-bond penalty of                              {:5s}: {:6.4f}'.format(bd,penalty_s[bd]))
           if bd in penalty_rcut:
              print('Bond-Order at radius cutoff penalty of            {:5s}: {:6.4f}'.format(bd,penalty_rcut[bd]))
           if bd in penalty_vdw:
              print('Vdw fluctuation penalty of                        {:5s}: {:6.4f}'.format(bd,penalty_vdw[bd]))
       print('\n')
@@ -1277,16 +1289,16 @@
         reuse_m = False
 
     nout_ = 3 if MessageFunction!=4 else 1
     if MessageFunction==1:
         nin_  = 5
     elif MessageFunction==5 :
         nin_  = 3 
-    elif MessageFunction==2:
-        nin_  = 5 
+    # elif MessageFunction==2:
+    #     nin_  = 5 
     else:
         nin_  = 3
 
     for t in range(1,messages+1):
         b = 0.881373587 if t>1 else -0.867
         if mf_universal_nn is not None:
            set_universal_wb(m_=m_,pref='fm',bd=mf_universal_nn[0],reuse_m=reuse_m, 
@@ -1366,8 +1378,40 @@
        else:
           universal_bonds = mf_universal_nn
        for sp in universal_bonds:
            # for t in range(1,messages+1):
            universal_nn.append('fm'+'_'+sp) # +str(t)
     return universal_nn
 
-                 
+'''
+Example:
+    rn = MPNN(libfile='ffield.json',
+              dataset=dataset,            
+              spv_bo={'C-H':[(1.8,9.5,11,2,11,0.0,0.0)],
+                      'H-O':[(1.3,2.0,11,2.78,11,0.0,0.0)],
+                      'C-C':[(1.9,7.9,11,7.9,11,0.0,0.0)] },
+              spv_pi={'N-C-N':[(7.8,8.7,1.65,1.8)],
+                      'C-C-C':[(7.8,8.7,1.61,1.8)],
+                      'C-C-H':[(8.0,8.8,1.61,1.8),(10.0,13,0,0.75)],
+                      'H-C-H':[(8.0,8.8,1.61,1.8)]},
+              weight=weight,
+              optword='nocoul',mpopt=mpopt,
+              opt=opt,cons=cons,clip=clip,
+              regularize_mf=1,regularize_be=1,regularize_bias=1,
+              lambda_reg=0.001,lambda_bd=100.0,lambda_me=0.0002,
+              mf_layer=[9,1],be_layer=[9,1],
+              EnergyFunction=1,MessageFunction=2,
+              mf_universal_nn=None,be_universal_nn=['C-H'],
+              messages=1,
+              bdopt=None,    # ['H-N'], 
+              mfopt=None,    # ['N'], 
+              batch_size=batch,
+              fixrcbo=False,
+              losFunc='n2',  # n2, mse, huber,abs
+              convergence=convergence) 
+
+    loss,accu,accMax,i,zpe =rn.run(learning_rate=lr,
+                      step=step,
+                      print_step=print_step,
+                      writelib=writelib,
+                      method='AdamOptimizer')  
+'''
```

### Comparing `irff-1.5.2/irff/neighbor.c` & `irff-1.5.3/irff/neighbor.c`

 * *Files 0% similar despite different names*

```diff
@@ -1947,14 +1947,15 @@
 static const char __pyx_k_an[] = "an";
 static const char __pyx_k_hb[] = "hb";
 static const char __pyx_k_hn[] = "hn";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np_";
 static const char __pyx_k_tn[] = "tn";
 static const char __pyx_k_ang[] = "ang";
+static const char __pyx_k_anr[] = "anr";
 static const char __pyx_k_hbs[] = "hbs";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_nhb[] = "nhb";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_tab[] = "tab_";
 static const char __pyx_k_tor[] = "tor";
@@ -2094,14 +2095,15 @@
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_kp_u__2;
 static PyObject *__pyx_n_s_a;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_an;
 static PyObject *__pyx_n_s_ang;
 static PyObject *__pyx_n_s_angs;
+static PyObject *__pyx_n_s_anr;
 static PyObject *__pyx_n_s_atom_name;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
@@ -2248,14 +2250,15 @@
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_float_0_0;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_112105877;
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple__3;
@@ -3454,14 +3457,15 @@
 static PyObject *__pyx_pf_4irff_8neighbor_2get_pangle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_p, PyObject *__pyx_v_atom_name, int __pyx_v_np_, PyObject *__pyx_v_p_ang, int __pyx_v_nang, PyObject *__pyx_v_angs) {
   PyObject *__pyx_v_an = 0;
   PyObject *__pyx_v_key = 0;
   int __pyx_v_i;
   int __pyx_v_a_;
   PyObject *__pyx_v_ang = 0;
   PyObject *__pyx_v_P = 0;
+  PyObject *__pyx_v_anr = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
@@ -3573,15 +3577,15 @@
       __pyx_v_a_ = __pyx_t_11;
 
       /* "irff/neighbor.pyx":58
  *         P[key] = np.zeros([nang],dtype=np.float32)
  *         for a_ in range(nang):
  *             ang = angs[a_]             # <<<<<<<<<<<<<<
  *             an = key+'_'+atom_name[ang[0]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[2]]
- *             if not an in p:
+ *             anr = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]
  */
       if (unlikely(__pyx_v_angs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
         __PYX_ERR(0, 58, __pyx_L1_error)
       }
       __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_angs, __pyx_v_a_, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 58, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
@@ -3589,16 +3593,16 @@
       __Pyx_XDECREF_SET(__pyx_v_ang, ((PyObject*)__pyx_t_8));
       __pyx_t_8 = 0;
 
       /* "irff/neighbor.pyx":59
  *         for a_ in range(nang):
  *             ang = angs[a_]
  *             an = key+'_'+atom_name[ang[0]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[2]]             # <<<<<<<<<<<<<<
- *             if not an in p:
- *                an = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]
+ *             anr = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]
+ *             if an in p:
  */
       __pyx_t_8 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_key, __pyx_n_u_); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 59, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (unlikely(__pyx_v_atom_name == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
         __PYX_ERR(0, 59, __pyx_L1_error)
       }
@@ -3658,361 +3662,420 @@
       if (!(likely(PyUnicode_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 59, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_an, ((PyObject*)__pyx_t_6));
       __pyx_t_6 = 0;
 
       /* "irff/neighbor.pyx":60
  *             ang = angs[a_]
  *             an = key+'_'+atom_name[ang[0]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[2]]
- *             if not an in p:             # <<<<<<<<<<<<<<
- *                an = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]
- *             P[key][a_] = p[an]
+ *             anr = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]             # <<<<<<<<<<<<<<
+ *             if an in p:
+ *                P[key][a_] = p[an]
+ */
+      __pyx_t_6 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_key, __pyx_n_u_); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      if (unlikely(__pyx_v_atom_name == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+        __PYX_ERR(0, 60, __pyx_L1_error)
+      }
+      if (unlikely(__pyx_v_ang == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+        __PYX_ERR(0, 60, __pyx_L1_error)
+      }
+      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_ang, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_8 = PyNumber_Add(__pyx_t_1, __pyx_kp_u__2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(__pyx_v_atom_name == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+        __PYX_ERR(0, 60, __pyx_L1_error)
+      }
+      if (unlikely(__pyx_v_ang == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+        __PYX_ERR(0, 60, __pyx_L1_error)
+      }
+      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_ang, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PyNumber_Add(__pyx_t_8, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u__2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(__pyx_v_atom_name == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+        __PYX_ERR(0, 60, __pyx_L1_error)
+      }
+      if (unlikely(__pyx_v_ang == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+        __PYX_ERR(0, 60, __pyx_L1_error)
+      }
+      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_ang, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_anr, __pyx_t_1);
+      __pyx_t_1 = 0;
+
+      /* "irff/neighbor.pyx":61
+ *             an = key+'_'+atom_name[ang[0]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[2]]
+ *             anr = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]
+ *             if an in p:             # <<<<<<<<<<<<<<
+ *                P[key][a_] = p[an]
+ *             elif anr in p:
  */
       if (unlikely(__pyx_v_p == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 60, __pyx_L1_error)
+        __PYX_ERR(0, 61, __pyx_L1_error)
       }
-      __pyx_t_12 = (__Pyx_PyDict_ContainsTF(__pyx_v_an, __pyx_v_p, Py_NE)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __pyx_t_12 = (__Pyx_PyDict_ContainsTF(__pyx_v_an, __pyx_v_p, Py_EQ)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 61, __pyx_L1_error)
       __pyx_t_13 = (__pyx_t_12 != 0);
       if (__pyx_t_13) {
 
-        /* "irff/neighbor.pyx":61
- *             an = key+'_'+atom_name[ang[0]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[2]]
- *             if not an in p:
- *                an = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]             # <<<<<<<<<<<<<<
- *             P[key][a_] = p[an]
- * 
+        /* "irff/neighbor.pyx":62
+ *             anr = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]
+ *             if an in p:
+ *                P[key][a_] = p[an]             # <<<<<<<<<<<<<<
+ *             elif anr in p:
+ *                P[key][a_] = p[anr]
  */
-        __pyx_t_6 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_key, __pyx_n_u_); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 61, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        if (unlikely(__pyx_v_atom_name == Py_None)) {
-          PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 61, __pyx_L1_error)
-        }
-        if (unlikely(__pyx_v_ang == Py_None)) {
+        if (unlikely(__pyx_v_p == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 61, __pyx_L1_error)
+          __PYX_ERR(0, 62, __pyx_L1_error)
         }
-        __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_ang, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_an); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 61, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_v_key); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 62, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(__Pyx_SetItemInt(__pyx_t_8, __pyx_v_a_, __pyx_t_1, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 62, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = PyNumber_Add(__pyx_t_1, __pyx_kp_u__2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 61, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(__pyx_v_atom_name == Py_None)) {
-          PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 61, __pyx_L1_error)
-        }
-        if (unlikely(__pyx_v_ang == Py_None)) {
-          PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 61, __pyx_L1_error)
-        }
-        __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_ang, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 61, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_Add(__pyx_t_8, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u__2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 61, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(__pyx_v_atom_name == Py_None)) {
-          PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 61, __pyx_L1_error)
-        }
-        if (unlikely(__pyx_v_ang == Py_None)) {
+
+        /* "irff/neighbor.pyx":61
+ *             an = key+'_'+atom_name[ang[0]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[2]]
+ *             anr = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]
+ *             if an in p:             # <<<<<<<<<<<<<<
+ *                P[key][a_] = p[an]
+ *             elif anr in p:
+ */
+        goto __pyx_L7;
+      }
+
+      /* "irff/neighbor.pyx":63
+ *             if an in p:
+ *                P[key][a_] = p[an]
+ *             elif anr in p:             # <<<<<<<<<<<<<<
+ *                P[key][a_] = p[anr]
+ *             else:
+ */
+      if (unlikely(__pyx_v_p == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+        __PYX_ERR(0, 63, __pyx_L1_error)
+      }
+      __pyx_t_13 = (__Pyx_PyDict_ContainsTF(__pyx_v_anr, __pyx_v_p, Py_EQ)); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 63, __pyx_L1_error)
+      __pyx_t_12 = (__pyx_t_13 != 0);
+      if (__pyx_t_12) {
+
+        /* "irff/neighbor.pyx":64
+ *                P[key][a_] = p[an]
+ *             elif anr in p:
+ *                P[key][a_] = p[anr]             # <<<<<<<<<<<<<<
+ *             else:
+ *                P[key][a_] = 0.0
+ */
+        if (unlikely(__pyx_v_p == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 61, __pyx_L1_error)
+          __PYX_ERR(0, 64, __pyx_L1_error)
         }
-        __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_ang, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_anr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 61, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_v_key); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 64, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(__Pyx_SetItemInt(__pyx_t_8, __pyx_v_a_, __pyx_t_1, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 64, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 61, __pyx_L1_error)
-        __Pyx_DECREF_SET(__pyx_v_an, ((PyObject*)__pyx_t_1));
-        __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "irff/neighbor.pyx":60
- *             ang = angs[a_]
- *             an = key+'_'+atom_name[ang[0]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[2]]
- *             if not an in p:             # <<<<<<<<<<<<<<
- *                an = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]
- *             P[key][a_] = p[an]
+        /* "irff/neighbor.pyx":63
+ *             if an in p:
+ *                P[key][a_] = p[an]
+ *             elif anr in p:             # <<<<<<<<<<<<<<
+ *                P[key][a_] = p[anr]
+ *             else:
  */
+        goto __pyx_L7;
       }
 
-      /* "irff/neighbor.pyx":62
- *             if not an in p:
- *                an = key+'_'+atom_name[ang[2]]+'-'+atom_name[ang[1]]+'-'+atom_name[ang[0]]
- *             P[key][a_] = p[an]             # <<<<<<<<<<<<<<
+      /* "irff/neighbor.pyx":66
+ *                P[key][a_] = p[anr]
+ *             else:
+ *                P[key][a_] = 0.0             # <<<<<<<<<<<<<<
  * 
  *     P['val3'] = np.zeros([nang],dtype=np.float32)
  */
-      if (unlikely(__pyx_v_p == Py_None)) {
-        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 62, __pyx_L1_error)
+      /*else*/ {
+        __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        if (unlikely(__Pyx_SetItemInt(__pyx_t_1, __pyx_v_a_, __pyx_float_0_0, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 66, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_an); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_v_key); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 62, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_8, __pyx_v_a_, __pyx_t_1, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 62, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_L7:;
     }
   }
 
-  /* "irff/neighbor.pyx":64
- *             P[key][a_] = p[an]
+  /* "irff/neighbor.pyx":68
+ *                P[key][a_] = 0.0
  * 
  *     P['val3'] = np.zeros([nang],dtype=np.float32)             # <<<<<<<<<<<<<<
  *     for a_ in range(nang):
  *         ang = angs[a_]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nang); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nang); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_1);
   PyList_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(PyDict_SetItem(__pyx_v_P, __pyx_n_u_val3, __pyx_t_7) < 0)) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_P, __pyx_n_u_val3, __pyx_t_7) < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "irff/neighbor.pyx":65
+  /* "irff/neighbor.pyx":69
  * 
  *     P['val3'] = np.zeros([nang],dtype=np.float32)
  *     for a_ in range(nang):             # <<<<<<<<<<<<<<
  *         ang = angs[a_]
  *         an = 'val3' + '_' + atom_name[ang[1]]
  */
   __pyx_t_2 = __pyx_v_nang;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_a_ = __pyx_t_4;
 
-    /* "irff/neighbor.pyx":66
+    /* "irff/neighbor.pyx":70
  *     P['val3'] = np.zeros([nang],dtype=np.float32)
  *     for a_ in range(nang):
  *         ang = angs[a_]             # <<<<<<<<<<<<<<
  *         an = 'val3' + '_' + atom_name[ang[1]]
  *         P['val3'][a_] = p[an]
  */
     if (unlikely(__pyx_v_angs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 66, __pyx_L1_error)
+      __PYX_ERR(0, 70, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_GetItemInt_List(__pyx_v_angs, __pyx_v_a_, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_GetItemInt_List(__pyx_v_angs, __pyx_v_a_, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (!(likely(PyList_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_7)->tp_name), 0))) __PYX_ERR(0, 66, __pyx_L1_error)
+    if (!(likely(PyList_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_7)->tp_name), 0))) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_ang, ((PyObject*)__pyx_t_7));
     __pyx_t_7 = 0;
 
-    /* "irff/neighbor.pyx":67
+    /* "irff/neighbor.pyx":71
  *     for a_ in range(nang):
  *         ang = angs[a_]
  *         an = 'val3' + '_' + atom_name[ang[1]]             # <<<<<<<<<<<<<<
  *         P['val3'][a_] = p[an]
  * 
  */
     if (unlikely(__pyx_v_atom_name == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 67, __pyx_L1_error)
+      __PYX_ERR(0, 71, __pyx_L1_error)
     }
     if (unlikely(__pyx_v_ang == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 67, __pyx_L1_error)
+      __PYX_ERR(0, 71, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_GetItemInt_List(__pyx_v_ang, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_GetItemInt_List(__pyx_v_ang, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyNumber_Add(__pyx_n_u_val3_2, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_7 = PyNumber_Add(__pyx_n_u_val3_2, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_7)->tp_name), 0))) __PYX_ERR(0, 67, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_7)->tp_name), 0))) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_an, ((PyObject*)__pyx_t_7));
     __pyx_t_7 = 0;
 
-    /* "irff/neighbor.pyx":68
+    /* "irff/neighbor.pyx":72
  *         ang = angs[a_]
  *         an = 'val3' + '_' + atom_name[ang[1]]
  *         P['val3'][a_] = p[an]             # <<<<<<<<<<<<<<
  * 
  *     P['val5'] = np.zeros([nang],dtype=np.float32)
  */
     if (unlikely(__pyx_v_p == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 68, __pyx_L1_error)
+      __PYX_ERR(0, 72, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_an); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_an); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_n_u_val3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_n_u_val3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_6, __pyx_v_a_, __pyx_t_7, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_6, __pyx_v_a_, __pyx_t_7, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
 
-  /* "irff/neighbor.pyx":70
+  /* "irff/neighbor.pyx":74
  *         P['val3'][a_] = p[an]
  * 
  *     P['val5'] = np.zeros([nang],dtype=np.float32)             # <<<<<<<<<<<<<<
  *     for a_ in range(nang):
  *         ang = angs[a_]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_nang); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_nang); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_7);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_float32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_float32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(PyDict_SetItem(__pyx_v_P, __pyx_n_u_val5, __pyx_t_5) < 0)) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_P, __pyx_n_u_val5, __pyx_t_5) < 0)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "irff/neighbor.pyx":71
+  /* "irff/neighbor.pyx":75
  * 
  *     P['val5'] = np.zeros([nang],dtype=np.float32)
  *     for a_ in range(nang):             # <<<<<<<<<<<<<<
  *         ang = angs[a_]
  *         an = 'val5' + '_' + atom_name[ang[1]]
  */
   __pyx_t_2 = __pyx_v_nang;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_a_ = __pyx_t_4;
 
-    /* "irff/neighbor.pyx":72
+    /* "irff/neighbor.pyx":76
  *     P['val5'] = np.zeros([nang],dtype=np.float32)
  *     for a_ in range(nang):
  *         ang = angs[a_]             # <<<<<<<<<<<<<<
  *         an = 'val5' + '_' + atom_name[ang[1]]
  *         P['val5'][a_] = p[an]
  */
     if (unlikely(__pyx_v_angs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 72, __pyx_L1_error)
+      __PYX_ERR(0, 76, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_angs, __pyx_v_a_, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_angs, __pyx_v_a_, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (!(likely(PyList_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 72, __pyx_L1_error)
+    if (!(likely(PyList_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_ang, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "irff/neighbor.pyx":73
+    /* "irff/neighbor.pyx":77
  *     for a_ in range(nang):
  *         ang = angs[a_]
  *         an = 'val5' + '_' + atom_name[ang[1]]             # <<<<<<<<<<<<<<
  *         P['val5'][a_] = p[an]
  *     return P
  */
     if (unlikely(__pyx_v_atom_name == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 73, __pyx_L1_error)
+      __PYX_ERR(0, 77, __pyx_L1_error)
     }
     if (unlikely(__pyx_v_ang == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 73, __pyx_L1_error)
+      __PYX_ERR(0, 77, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_ang, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_ang, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyNumber_Add(__pyx_n_u_val5_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_Add(__pyx_n_u_val5_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 73, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_an, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "irff/neighbor.pyx":74
+    /* "irff/neighbor.pyx":78
  *         ang = angs[a_]
  *         an = 'val5' + '_' + atom_name[ang[1]]
  *         P['val5'][a_] = p[an]             # <<<<<<<<<<<<<<
  *     return P
  * 
  */
     if (unlikely(__pyx_v_p == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 74, __pyx_L1_error)
+      __PYX_ERR(0, 78, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_an); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_an); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_n_u_val5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_n_u_val5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_1, __pyx_v_a_, __pyx_t_5, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 74, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_1, __pyx_v_a_, __pyx_t_5, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
 
-  /* "irff/neighbor.pyx":75
+  /* "irff/neighbor.pyx":79
  *         an = 'val5' + '_' + atom_name[ang[1]]
  *         P['val5'][a_] = p[an]
  *     return P             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
@@ -4038,20 +4101,21 @@
   __Pyx_AddTraceback("irff.neighbor.get_pangle", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_an);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_ang);
   __Pyx_XDECREF(__pyx_v_P);
+  __Pyx_XDECREF(__pyx_v_anr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "irff/neighbor.pyx":78
+/* "irff/neighbor.pyx":82
  * 
  * 
  * def get_ptorsion(dict p,list atom_name,int np_,list p_tor,int ntor,list tors):             # <<<<<<<<<<<<<<
  *     cdef str tn,key
  *     cdef int i,t_
  */
 
@@ -4098,73 +4162,73 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_atom_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 1); __PYX_ERR(0, 78, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 1); __PYX_ERR(0, 82, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_np)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 2); __PYX_ERR(0, 78, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 2); __PYX_ERR(0, 82, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p_tor)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 3); __PYX_ERR(0, 78, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 3); __PYX_ERR(0, 82, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ntor)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 4); __PYX_ERR(0, 78, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 4); __PYX_ERR(0, 82, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tors)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 5); __PYX_ERR(0, 78, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, 5); __PYX_ERR(0, 82, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_ptorsion") < 0)) __PYX_ERR(0, 78, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_ptorsion") < 0)) __PYX_ERR(0, 82, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
     }
     __pyx_v_p = ((PyObject*)values[0]);
     __pyx_v_atom_name = ((PyObject*)values[1]);
-    __pyx_v_np_ = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_np_ == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L3_error)
+    __pyx_v_np_ = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_np_ == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 82, __pyx_L3_error)
     __pyx_v_p_tor = ((PyObject*)values[3]);
-    __pyx_v_ntor = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_ntor == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L3_error)
+    __pyx_v_ntor = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_ntor == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 82, __pyx_L3_error)
     __pyx_v_tors = ((PyObject*)values[5]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 78, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_ptorsion", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 82, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("irff.neighbor.get_ptorsion", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p), (&PyDict_Type), 1, "p", 1))) __PYX_ERR(0, 78, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_atom_name), (&PyList_Type), 1, "atom_name", 1))) __PYX_ERR(0, 78, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p_tor), (&PyList_Type), 1, "p_tor", 1))) __PYX_ERR(0, 78, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_tors), (&PyList_Type), 1, "tors", 1))) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p), (&PyDict_Type), 1, "p", 1))) __PYX_ERR(0, 82, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_atom_name), (&PyList_Type), 1, "atom_name", 1))) __PYX_ERR(0, 82, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p_tor), (&PyList_Type), 1, "p_tor", 1))) __PYX_ERR(0, 82, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_tors), (&PyList_Type), 1, "tors", 1))) __PYX_ERR(0, 82, __pyx_L1_error)
   __pyx_r = __pyx_pf_4irff_8neighbor_4get_ptorsion(__pyx_self, __pyx_v_p, __pyx_v_atom_name, __pyx_v_np_, __pyx_v_p_tor, __pyx_v_ntor, __pyx_v_tors);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4195,363 +4259,363 @@
   int __pyx_t_12;
   int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_ptorsion", 0);
 
-  /* "irff/neighbor.pyx":82
+  /* "irff/neighbor.pyx":86
  *     cdef int i,t_
  *     cdef list tor
  *     cdef dict P = {}             # <<<<<<<<<<<<<<
  *     # cdef double[:,:] P = np.zeros([np_,ntor])
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_P = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "irff/neighbor.pyx":85
+  /* "irff/neighbor.pyx":89
  *     # cdef double[:,:] P = np.zeros([np_,ntor])
  * 
  *     for i in range(np_):             # <<<<<<<<<<<<<<
  *         key = p_tor[i]
  *         P[key] = np.zeros([ntor],dtype=np.float32)
  */
   __pyx_t_2 = __pyx_v_np_;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "irff/neighbor.pyx":86
+    /* "irff/neighbor.pyx":90
  * 
  *     for i in range(np_):
  *         key = p_tor[i]             # <<<<<<<<<<<<<<
  *         P[key] = np.zeros([ntor],dtype=np.float32)
  *         for t_ in range(ntor):
  */
     if (unlikely(__pyx_v_p_tor == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 86, __pyx_L1_error)
+      __PYX_ERR(0, 90, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_p_tor, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_p_tor, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 86, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "irff/neighbor.pyx":87
+    /* "irff/neighbor.pyx":91
  *     for i in range(np_):
  *         key = p_tor[i]
  *         P[key] = np.zeros([ntor],dtype=np.float32)             # <<<<<<<<<<<<<<
  *         for t_ in range(ntor):
  *             tor = tors[t_]
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_ntor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_ntor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_1);
     PyList_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_6);
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(PyDict_SetItem(__pyx_v_P, __pyx_v_key, __pyx_t_8) < 0)) __PYX_ERR(0, 87, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_P, __pyx_v_key, __pyx_t_8) < 0)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "irff/neighbor.pyx":88
+    /* "irff/neighbor.pyx":92
  *         key = p_tor[i]
  *         P[key] = np.zeros([ntor],dtype=np.float32)
  *         for t_ in range(ntor):             # <<<<<<<<<<<<<<
  *             tor = tors[t_]
  *             tn = key+'_'+atom_name[tor[0]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[3]]
  */
     __pyx_t_9 = __pyx_v_ntor;
     __pyx_t_10 = __pyx_t_9;
     for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
       __pyx_v_t_ = __pyx_t_11;
 
-      /* "irff/neighbor.pyx":89
+      /* "irff/neighbor.pyx":93
  *         P[key] = np.zeros([ntor],dtype=np.float32)
  *         for t_ in range(ntor):
  *             tor = tors[t_]             # <<<<<<<<<<<<<<
  *             tn = key+'_'+atom_name[tor[0]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[3]]
  *             if tn not in p:
  */
       if (unlikely(__pyx_v_tors == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 89, __pyx_L1_error)
+        __PYX_ERR(0, 93, __pyx_L1_error)
       }
-      __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tors, __pyx_v_t_, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 89, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tors, __pyx_v_t_, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 93, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      if (!(likely(PyList_CheckExact(__pyx_t_8))||((__pyx_t_8) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_8)->tp_name), 0))) __PYX_ERR(0, 89, __pyx_L1_error)
+      if (!(likely(PyList_CheckExact(__pyx_t_8))||((__pyx_t_8) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_8)->tp_name), 0))) __PYX_ERR(0, 93, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_tor, ((PyObject*)__pyx_t_8));
       __pyx_t_8 = 0;
 
-      /* "irff/neighbor.pyx":90
+      /* "irff/neighbor.pyx":94
  *         for t_ in range(ntor):
  *             tor = tors[t_]
  *             tn = key+'_'+atom_name[tor[0]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[3]]             # <<<<<<<<<<<<<<
  *             if tn not in p:
  *                tn = key+'_'+atom_name[tor[3]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[0]]
  */
-      __pyx_t_8 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_key, __pyx_n_u_); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_key, __pyx_n_u_); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (unlikely(__pyx_v_atom_name == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 90, __pyx_L1_error)
+        __PYX_ERR(0, 94, __pyx_L1_error)
       }
       if (unlikely(__pyx_v_tor == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 90, __pyx_L1_error)
+        __PYX_ERR(0, 94, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_tor, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_tor, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(__pyx_v_atom_name == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 90, __pyx_L1_error)
+        __PYX_ERR(0, 94, __pyx_L1_error)
       }
       if (unlikely(__pyx_v_tor == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 90, __pyx_L1_error)
+        __PYX_ERR(0, 94, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_tor, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_tor, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_8 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(__pyx_v_atom_name == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 90, __pyx_L1_error)
+        __PYX_ERR(0, 94, __pyx_L1_error)
       }
       if (unlikely(__pyx_v_tor == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 90, __pyx_L1_error)
+        __PYX_ERR(0, 94, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_tor, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_tor, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(__pyx_v_atom_name == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 90, __pyx_L1_error)
+        __PYX_ERR(0, 94, __pyx_L1_error)
       }
       if (unlikely(__pyx_v_tor == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 90, __pyx_L1_error)
+        __PYX_ERR(0, 94, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_tor, 3, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_tor, 3, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (!(likely(PyUnicode_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 90, __pyx_L1_error)
+      if (!(likely(PyUnicode_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_tn, ((PyObject*)__pyx_t_6));
       __pyx_t_6 = 0;
 
-      /* "irff/neighbor.pyx":91
+      /* "irff/neighbor.pyx":95
  *             tor = tors[t_]
  *             tn = key+'_'+atom_name[tor[0]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[3]]
  *             if tn not in p:             # <<<<<<<<<<<<<<
  *                tn = key+'_'+atom_name[tor[3]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[0]]
  *             P[key][t_] = p[tn]
  */
       if (unlikely(__pyx_v_p == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 91, __pyx_L1_error)
+        __PYX_ERR(0, 95, __pyx_L1_error)
       }
-      __pyx_t_12 = (__Pyx_PyDict_ContainsTF(__pyx_v_tn, __pyx_v_p, Py_NE)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_12 = (__Pyx_PyDict_ContainsTF(__pyx_v_tn, __pyx_v_p, Py_NE)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
       __pyx_t_13 = (__pyx_t_12 != 0);
       if (__pyx_t_13) {
 
-        /* "irff/neighbor.pyx":92
+        /* "irff/neighbor.pyx":96
  *             tn = key+'_'+atom_name[tor[0]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[3]]
  *             if tn not in p:
  *                tn = key+'_'+atom_name[tor[3]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[0]]             # <<<<<<<<<<<<<<
  *             P[key][t_] = p[tn]
  *     return P
  */
-        __pyx_t_6 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_key, __pyx_n_u_); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_key, __pyx_n_u_); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         if (unlikely(__pyx_v_atom_name == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 92, __pyx_L1_error)
+          __PYX_ERR(0, 96, __pyx_L1_error)
         }
         if (unlikely(__pyx_v_tor == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 92, __pyx_L1_error)
+          __PYX_ERR(0, 96, __pyx_L1_error)
         }
-        __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tor, 3, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tor, 3, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = PyNumber_Add(__pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_8 = PyNumber_Add(__pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_Add(__pyx_t_8, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_1 = PyNumber_Add(__pyx_t_8, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         if (unlikely(__pyx_v_atom_name == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 92, __pyx_L1_error)
+          __PYX_ERR(0, 96, __pyx_L1_error)
         }
         if (unlikely(__pyx_v_tor == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 92, __pyx_L1_error)
+          __PYX_ERR(0, 96, __pyx_L1_error)
         }
-        __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tor, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tor, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = PyNumber_Add(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_8 = PyNumber_Add(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_kp_u__2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_kp_u__2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         if (unlikely(__pyx_v_atom_name == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 92, __pyx_L1_error)
+          __PYX_ERR(0, 96, __pyx_L1_error)
         }
         if (unlikely(__pyx_v_tor == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 92, __pyx_L1_error)
+          __PYX_ERR(0, 96, __pyx_L1_error)
         }
-        __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tor, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tor, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = PyNumber_Add(__pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_8 = PyNumber_Add(__pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_Add(__pyx_t_8, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_1 = PyNumber_Add(__pyx_t_8, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         if (unlikely(__pyx_v_atom_name == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 92, __pyx_L1_error)
+          __PYX_ERR(0, 96, __pyx_L1_error)
         }
         if (unlikely(__pyx_v_tor == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 92, __pyx_L1_error)
+          __PYX_ERR(0, 96, __pyx_L1_error)
         }
-        __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tor, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_tor, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = PyNumber_Add(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __pyx_t_8 = PyNumber_Add(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (!(likely(PyUnicode_CheckExact(__pyx_t_8))||((__pyx_t_8) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_8)->tp_name), 0))) __PYX_ERR(0, 92, __pyx_L1_error)
+        if (!(likely(PyUnicode_CheckExact(__pyx_t_8))||((__pyx_t_8) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_8)->tp_name), 0))) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_DECREF_SET(__pyx_v_tn, ((PyObject*)__pyx_t_8));
         __pyx_t_8 = 0;
 
-        /* "irff/neighbor.pyx":91
+        /* "irff/neighbor.pyx":95
  *             tor = tors[t_]
  *             tn = key+'_'+atom_name[tor[0]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[3]]
  *             if tn not in p:             # <<<<<<<<<<<<<<
  *                tn = key+'_'+atom_name[tor[3]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[0]]
  *             P[key][t_] = p[tn]
  */
       }
 
-      /* "irff/neighbor.pyx":93
+      /* "irff/neighbor.pyx":97
  *             if tn not in p:
  *                tn = key+'_'+atom_name[tor[3]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[0]]
  *             P[key][t_] = p[tn]             # <<<<<<<<<<<<<<
  *     return P
  * 
  */
       if (unlikely(__pyx_v_p == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 93, __pyx_L1_error)
+        __PYX_ERR(0, 97, __pyx_L1_error)
       }
-      __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_tn); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 93, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_tn); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_6, __pyx_v_t_, __pyx_t_8, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 93, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_6, __pyx_v_t_, __pyx_t_8, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
   }
 
-  /* "irff/neighbor.pyx":94
+  /* "irff/neighbor.pyx":98
  *                tn = key+'_'+atom_name[tor[3]]+'-'+atom_name[tor[2]]+'-'+atom_name[tor[1]]+'-'+atom_name[tor[0]]
  *             P[key][t_] = p[tn]
  *     return P             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_P);
   __pyx_r = __pyx_v_P;
   goto __pyx_L0;
 
-  /* "irff/neighbor.pyx":78
+  /* "irff/neighbor.pyx":82
  * 
  * 
  * def get_ptorsion(dict p,list atom_name,int np_,list p_tor,int ntor,list tors):             # <<<<<<<<<<<<<<
  *     cdef str tn,key
  *     cdef int i,t_
  */
 
@@ -4570,15 +4634,15 @@
   __Pyx_XDECREF(__pyx_v_tor);
   __Pyx_XDECREF(__pyx_v_P);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "irff/neighbor.pyx":97
+/* "irff/neighbor.pyx":101
  * 
  * 
  * def get_phb(dict p,list atom_name,int np_,list p_hb,int nhb,list hbs):             # <<<<<<<<<<<<<<
  *     cdef str tn,key
  *     cdef int i,t_
  */
 
@@ -4625,73 +4689,73 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_atom_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 1); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 1); __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_np)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 2); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 2); __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p_hb)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 3); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 3); __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_nhb)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 4); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 4); __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hbs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 5); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, 5); __PYX_ERR(0, 101, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_phb") < 0)) __PYX_ERR(0, 97, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_phb") < 0)) __PYX_ERR(0, 101, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
     }
     __pyx_v_p = ((PyObject*)values[0]);
     __pyx_v_atom_name = ((PyObject*)values[1]);
-    __pyx_v_np_ = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_np_ == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 97, __pyx_L3_error)
+    __pyx_v_np_ = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_np_ == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
     __pyx_v_p_hb = ((PyObject*)values[3]);
-    __pyx_v_nhb = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_nhb == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 97, __pyx_L3_error)
+    __pyx_v_nhb = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_nhb == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
     __pyx_v_hbs = ((PyObject*)values[5]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 97, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_phb", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 101, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("irff.neighbor.get_phb", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p), (&PyDict_Type), 1, "p", 1))) __PYX_ERR(0, 97, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_atom_name), (&PyList_Type), 1, "atom_name", 1))) __PYX_ERR(0, 97, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p_hb), (&PyList_Type), 1, "p_hb", 1))) __PYX_ERR(0, 97, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_hbs), (&PyList_Type), 1, "hbs", 1))) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p), (&PyDict_Type), 1, "p", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_atom_name), (&PyList_Type), 1, "atom_name", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p_hb), (&PyList_Type), 1, "p_hb", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_hbs), (&PyList_Type), 1, "hbs", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
   __pyx_r = __pyx_pf_4irff_8neighbor_6get_phb(__pyx_self, __pyx_v_p, __pyx_v_atom_name, __pyx_v_np_, __pyx_v_p_hb, __pyx_v_nhb, __pyx_v_hbs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4720,228 +4784,228 @@
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_phb", 0);
 
-  /* "irff/neighbor.pyx":101
+  /* "irff/neighbor.pyx":105
  *     cdef int i,t_
  *     cdef list hb
  *     cdef dict P = {}             # <<<<<<<<<<<<<<
  * 
  *     for i in range(np_):
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_P = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "irff/neighbor.pyx":103
+  /* "irff/neighbor.pyx":107
  *     cdef dict P = {}
  * 
  *     for i in range(np_):             # <<<<<<<<<<<<<<
  *         key = p_hb[i]
  *         P[key] = np.zeros([nhb],dtype=np.float32)
  */
   __pyx_t_2 = __pyx_v_np_;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "irff/neighbor.pyx":104
+    /* "irff/neighbor.pyx":108
  * 
  *     for i in range(np_):
  *         key = p_hb[i]             # <<<<<<<<<<<<<<
  *         P[key] = np.zeros([nhb],dtype=np.float32)
  *         for t_ in range(nhb):
  */
     if (unlikely(__pyx_v_p_hb == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 104, __pyx_L1_error)
+      __PYX_ERR(0, 108, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_p_hb, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_p_hb, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 104, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "irff/neighbor.pyx":105
+    /* "irff/neighbor.pyx":109
  *     for i in range(np_):
  *         key = p_hb[i]
  *         P[key] = np.zeros([nhb],dtype=np.float32)             # <<<<<<<<<<<<<<
  *         for t_ in range(nhb):
  *             hb = hbs[t_]
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nhb); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nhb); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_1);
     PyList_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_6);
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(PyDict_SetItem(__pyx_v_P, __pyx_v_key, __pyx_t_8) < 0)) __PYX_ERR(0, 105, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_P, __pyx_v_key, __pyx_t_8) < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "irff/neighbor.pyx":106
+    /* "irff/neighbor.pyx":110
  *         key = p_hb[i]
  *         P[key] = np.zeros([nhb],dtype=np.float32)
  *         for t_ in range(nhb):             # <<<<<<<<<<<<<<
  *             hb = hbs[t_]
  *             hn = key+'_'+atom_name[hb[0]]+'-'+atom_name[hb[1]]+'-'+atom_name[hb[2]]
  */
     __pyx_t_9 = __pyx_v_nhb;
     __pyx_t_10 = __pyx_t_9;
     for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
       __pyx_v_t_ = __pyx_t_11;
 
-      /* "irff/neighbor.pyx":107
+      /* "irff/neighbor.pyx":111
  *         P[key] = np.zeros([nhb],dtype=np.float32)
  *         for t_ in range(nhb):
  *             hb = hbs[t_]             # <<<<<<<<<<<<<<
  *             hn = key+'_'+atom_name[hb[0]]+'-'+atom_name[hb[1]]+'-'+atom_name[hb[2]]
  *             P[key][t_] = p[hn]
  */
       if (unlikely(__pyx_v_hbs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 107, __pyx_L1_error)
+        __PYX_ERR(0, 111, __pyx_L1_error)
       }
-      __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_hbs, __pyx_v_t_, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_GetItemInt_List(__pyx_v_hbs, __pyx_v_t_, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 111, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      if (!(likely(PyList_CheckExact(__pyx_t_8))||((__pyx_t_8) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_8)->tp_name), 0))) __PYX_ERR(0, 107, __pyx_L1_error)
+      if (!(likely(PyList_CheckExact(__pyx_t_8))||((__pyx_t_8) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_8)->tp_name), 0))) __PYX_ERR(0, 111, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_hb, ((PyObject*)__pyx_t_8));
       __pyx_t_8 = 0;
 
-      /* "irff/neighbor.pyx":108
+      /* "irff/neighbor.pyx":112
  *         for t_ in range(nhb):
  *             hb = hbs[t_]
  *             hn = key+'_'+atom_name[hb[0]]+'-'+atom_name[hb[1]]+'-'+atom_name[hb[2]]             # <<<<<<<<<<<<<<
  *             P[key][t_] = p[hn]
  *     return P
  */
-      __pyx_t_8 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_key, __pyx_n_u_); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_key, __pyx_n_u_); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (unlikely(__pyx_v_atom_name == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 108, __pyx_L1_error)
+        __PYX_ERR(0, 112, __pyx_L1_error)
       }
       if (unlikely(__pyx_v_hb == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 108, __pyx_L1_error)
+        __PYX_ERR(0, 112, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_hb, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_hb, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(__pyx_v_atom_name == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 108, __pyx_L1_error)
+        __PYX_ERR(0, 112, __pyx_L1_error)
       }
       if (unlikely(__pyx_v_hb == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 108, __pyx_L1_error)
+        __PYX_ERR(0, 112, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_hb, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_hb, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_8 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(__pyx_v_atom_name == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 108, __pyx_L1_error)
+        __PYX_ERR(0, 112, __pyx_L1_error)
       }
       if (unlikely(__pyx_v_hb == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 108, __pyx_L1_error)
+        __PYX_ERR(0, 112, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_hb, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_hb, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_atom_name, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_Add(__pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF_SET(__pyx_v_hn, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "irff/neighbor.pyx":109
+      /* "irff/neighbor.pyx":113
  *             hb = hbs[t_]
  *             hn = key+'_'+atom_name[hb[0]]+'-'+atom_name[hb[1]]+'-'+atom_name[hb[2]]
  *             P[key][t_] = p[hn]             # <<<<<<<<<<<<<<
  *     return P
  * 
  */
       if (unlikely(__pyx_v_p == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 109, __pyx_L1_error)
+        __PYX_ERR(0, 113, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_hn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_p, __pyx_v_hn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_P, __pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_1, __pyx_v_t_, __pyx_t_6, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_1, __pyx_v_t_, __pyx_t_6, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   }
 
-  /* "irff/neighbor.pyx":110
+  /* "irff/neighbor.pyx":114
  *             hn = key+'_'+atom_name[hb[0]]+'-'+atom_name[hb[1]]+'-'+atom_name[hb[2]]
  *             P[key][t_] = p[hn]
  *     return P             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_P);
   __pyx_r = __pyx_v_P;
   goto __pyx_L0;
 
-  /* "irff/neighbor.pyx":97
+  /* "irff/neighbor.pyx":101
  * 
  * 
  * def get_phb(dict p,list atom_name,int np_,list p_hb,int nhb,list hbs):             # <<<<<<<<<<<<<<
  *     cdef str tn,key
  *     cdef int i,t_
  */
 
@@ -18807,14 +18871,15 @@
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_an, __pyx_k_an, sizeof(__pyx_k_an), 0, 0, 1, 1},
   {&__pyx_n_s_ang, __pyx_k_ang, sizeof(__pyx_k_ang), 0, 0, 1, 1},
   {&__pyx_n_s_angs, __pyx_k_angs, sizeof(__pyx_k_angs), 0, 0, 1, 1},
+  {&__pyx_n_s_anr, __pyx_k_anr, sizeof(__pyx_k_anr), 0, 0, 1, 1},
   {&__pyx_n_s_atom_name, __pyx_k_atom_name, sizeof(__pyx_k_atom_name), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
@@ -19145,42 +19210,42 @@
   /* "irff/neighbor.pyx":47
  * 
  * 
  * def get_pangle(dict p,list atom_name,int np_,list p_ang,int nang,list angs):             # <<<<<<<<<<<<<<
  *     cdef str an,key
  *     cdef int i,a_
  */
-  __pyx_tuple__24 = PyTuple_Pack(12, __pyx_n_s_p, __pyx_n_s_atom_name, __pyx_n_s_np, __pyx_n_s_p_ang, __pyx_n_s_nang, __pyx_n_s_angs, __pyx_n_s_an, __pyx_n_s_key, __pyx_n_s_i, __pyx_n_s_a, __pyx_n_s_ang, __pyx_n_s_P); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(13, __pyx_n_s_p, __pyx_n_s_atom_name, __pyx_n_s_np, __pyx_n_s_p_ang, __pyx_n_s_nang, __pyx_n_s_angs, __pyx_n_s_an, __pyx_n_s_key, __pyx_n_s_i, __pyx_n_s_a, __pyx_n_s_ang, __pyx_n_s_P, __pyx_n_s_anr); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(6, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_irff_neighbor_pyx, __pyx_n_s_get_pangle, 47, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(6, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_irff_neighbor_pyx, __pyx_n_s_get_pangle, 47, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "irff/neighbor.pyx":78
+  /* "irff/neighbor.pyx":82
  * 
  * 
  * def get_ptorsion(dict p,list atom_name,int np_,list p_tor,int ntor,list tors):             # <<<<<<<<<<<<<<
  *     cdef str tn,key
  *     cdef int i,t_
  */
-  __pyx_tuple__26 = PyTuple_Pack(12, __pyx_n_s_p, __pyx_n_s_atom_name, __pyx_n_s_np, __pyx_n_s_p_tor, __pyx_n_s_ntor, __pyx_n_s_tors, __pyx_n_s_tn, __pyx_n_s_key, __pyx_n_s_i, __pyx_n_s_t, __pyx_n_s_tor, __pyx_n_s_P); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(12, __pyx_n_s_p, __pyx_n_s_atom_name, __pyx_n_s_np, __pyx_n_s_p_tor, __pyx_n_s_ntor, __pyx_n_s_tors, __pyx_n_s_tn, __pyx_n_s_key, __pyx_n_s_i, __pyx_n_s_t, __pyx_n_s_tor, __pyx_n_s_P); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(6, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_irff_neighbor_pyx, __pyx_n_s_get_ptorsion, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(6, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_irff_neighbor_pyx, __pyx_n_s_get_ptorsion, 82, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 82, __pyx_L1_error)
 
-  /* "irff/neighbor.pyx":97
+  /* "irff/neighbor.pyx":101
  * 
  * 
  * def get_phb(dict p,list atom_name,int np_,list p_hb,int nhb,list hbs):             # <<<<<<<<<<<<<<
  *     cdef str tn,key
  *     cdef int i,t_
  */
-  __pyx_tuple__28 = PyTuple_Pack(13, __pyx_n_s_p, __pyx_n_s_atom_name, __pyx_n_s_np, __pyx_n_s_p_hb, __pyx_n_s_nhb, __pyx_n_s_hbs, __pyx_n_s_tn, __pyx_n_s_key, __pyx_n_s_i, __pyx_n_s_t, __pyx_n_s_hb, __pyx_n_s_P, __pyx_n_s_hn); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(13, __pyx_n_s_p, __pyx_n_s_atom_name, __pyx_n_s_np, __pyx_n_s_p_hb, __pyx_n_s_nhb, __pyx_n_s_hbs, __pyx_n_s_tn, __pyx_n_s_key, __pyx_n_s_i, __pyx_n_s_t, __pyx_n_s_hb, __pyx_n_s_P, __pyx_n_s_hn); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(6, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_irff_neighbor_pyx, __pyx_n_s_get_phb, 97, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(6, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_irff_neighbor_pyx, __pyx_n_s_get_phb, 101, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 101, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -19247,14 +19312,15 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_float_0_0 = PyFloat_FromDouble(0.0); if (unlikely(!__pyx_float_0_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -19620,36 +19686,36 @@
  *     cdef int i,a_
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4irff_8neighbor_3get_pangle, NULL, __pyx_n_s_irff_neighbor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_pangle, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "irff/neighbor.pyx":78
+  /* "irff/neighbor.pyx":82
  * 
  * 
  * def get_ptorsion(dict p,list atom_name,int np_,list p_tor,int ntor,list tors):             # <<<<<<<<<<<<<<
  *     cdef str tn,key
  *     cdef int i,t_
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4irff_8neighbor_5get_ptorsion, NULL, __pyx_n_s_irff_neighbor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4irff_8neighbor_5get_ptorsion, NULL, __pyx_n_s_irff_neighbor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_ptorsion, __pyx_t_1) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_ptorsion, __pyx_t_1) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "irff/neighbor.pyx":97
+  /* "irff/neighbor.pyx":101
  * 
  * 
  * def get_phb(dict p,list atom_name,int np_,list p_hb,int nhb,list hbs):             # <<<<<<<<<<<<<<
  *     cdef str tn,key
  *     cdef int i,t_
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4irff_8neighbor_7get_phb, NULL, __pyx_n_s_irff_neighbor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4irff_8neighbor_7get_phb, NULL, __pyx_n_s_irff_neighbor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_phb, __pyx_t_1) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_phb, __pyx_t_1) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "irff/neighbor.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * import numpy as np
  * 
  */
```

### Comparing `irff-1.5.2/irff/neighbors.py` & `irff-1.5.3/irff/neighbors.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/BondEnergy.py` & `irff-1.5.3/irff/plot/BondEnergy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/CheckAng.py` & `irff-1.5.3/irff/plot/CheckAng.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/LearningResults.py` & `irff-1.5.3/irff/plot/LearningResults.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/LearningResultsAng.py` & `irff-1.5.3/irff/plot/LearningResultsAng.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/MessagePassing.py` & `irff-1.5.3/irff/plot/MessagePassing.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/abc.py` & `irff-1.5.3/irff/plot/abc.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/angel_to_bond.py` & `irff-1.5.3/irff/plot/angel_to_bond.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/bde.py` & `irff-1.5.3/irff/plot/bde.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/compare_energies.py` & `irff-1.5.3/irff/plot/compare_energies.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/fingerprint.py` & `irff-1.5.3/irff/plot/fingerprint.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/gofr.py` & `irff-1.5.3/irff/plot/gofr.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/irnn_plot.py` & `irff-1.5.3/irff/plot/irnn_plot.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/label_md.py` & `irff-1.5.3/irff/plot/label_md.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/labels.py` & `irff-1.5.3/irff/plot/labels.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/morse.py` & `irff-1.5.3/irff/plot/morse.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/morse_taper.py` & `irff-1.5.3/irff/plot/morse_taper.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/mpbd.py` & `irff-1.5.3/irff/plot/mpbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/mpnn_plbd.py` & `irff-1.5.3/irff/plot/mpnn_plbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/nx.py` & `irff-1.5.3/irff/plot/nx.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/pdf.py` & `irff-1.5.3/irff/plot/pdf.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plbd.py` & `irff-1.5.3/irff/plot/plbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plbo.py` & `irff-1.5.3/irff/plot/plbo.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/ple.py` & `irff-1.5.3/irff/plot/ple.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plea.py` & `irff-1.5.3/irff/plot/plea.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/pleb.py` & `irff-1.5.3/irff/plot/pleb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/pleo.py` & `irff-1.5.3/irff/plot/pleo.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plev.py` & `irff-1.5.3/irff/plot/plev.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plevdw.py` & `irff-1.5.3/irff/plot/plevdw.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plf.py` & `irff-1.5.3/irff/plot/plf.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_atoms.py` & `irff-1.5.3/irff/plot/plot_atoms.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_atoms_matplot.py` & `irff-1.5.3/irff/plot/plot_atoms_matplot.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_atoms_momenta.py` & `irff-1.5.3/irff/plot/plot_atoms_momenta.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_bond_energy.py` & `irff-1.5.3/irff/plot/plot_bond_energy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_charge.py` & `irff-1.5.3/irff/plot/plot_charge.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_energy.py` & `irff-1.5.3/irff/plot/plot_energy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_eover.py` & `irff-1.5.3/irff/plot/plot_eover.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_eover_atom.py` & `irff-1.5.3/irff/plot/plot_eover_atom.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_functions.py` & `irff-1.5.3/irff/plot/plot_functions.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_morse.py` & `irff-1.5.3/irff/plot/plot_morse.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_pes.py` & `irff-1.5.3/irff/plot/plot_pes.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_pressure.py` & `irff-1.5.3/irff/plot/plot_pressure.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plot_zmat_pes.py` & `irff-1.5.3/irff/plot/plot_zmat_pes.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plotenergy.py` & `irff-1.5.3/irff/plot/plotenergy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/plotenergy_bond.py` & `irff-1.5.3/irff/plot/plotenergy_bond.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/pltp.py` & `irff-1.5.3/irff/plot/pltp.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/reax_plbd.py` & `irff-1.5.3/irff/plot/reax_plbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/reax_pldd.py` & `irff-1.5.3/irff/plot/reax_pldd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/reax_plot.py` & `irff-1.5.3/irff/plot/reax_plot.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/reax_plov.py` & `irff-1.5.3/irff/plot/reax_plov.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/rffbd.py` & `irff-1.5.3/irff/plot/rffbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/sigmoid.py` & `irff-1.5.3/irff/plot/sigmoid.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/vdw_taper.py` & `irff-1.5.3/irff/plot/vdw_taper.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/plot/view.py` & `irff-1.5.3/irff/plot/view.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/prop/__init__.py` & `irff-1.5.3/irff/prop/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/prop/gofr.py` & `irff-1.5.3/irff/prop/gofr.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/qeq.py` & `irff-1.5.3/irff/qeq.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/reax.py` & `irff-1.5.3/irff/reax.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,15 +378,15 @@
       self.f4r,self.f5r,self.f_4,self.f_5,self.df4,self.df5={},{},{},{},{},{}
       self.F,self.F_11,self.F_12,self.F_45={},{},{},{}
       self.fbot = {}
       self.powb,self.expb,self.EBD,self.ebond,self.ebda = {},{},{},{},{}
       self.sieng,self.pieng,self.ppeng = {},{},{}
 
       self.Delta_e,self.DE,self.nlp,self.Delta_lp,self.Dlp = {},{},{},{},{}
-      self.Dpi,self.BSO,self.BOPI,self.Delta_lpcorr,self.NLP = {},{},{},{},{}
+      self.D_p,self.Dpi,self.BSO,self.BOPI,self.Delta_lpcorr,self.NLP = {},{},{},{},{},{}
       self.explp,self.EL,self.elone,self.Elone,self.ELONE = {},{},{},{},{}
       self.EOV,self.Eover,self.eover,self.otrm1,self.otrm2 =  {},{},{},{},{}
 
       self.expeu1,self.expeu2,self.eu1,self.expeu3,self.eu2,self.EUN = {},{},{},{},{},{}
       self.eunder,self.Eunder = {},{}
 
       self.EANG,self.Eang,self.eang,self.theta0,self.fijk = {},{},{},{},{}
@@ -537,16 +537,17 @@
 
           if mol in self.weight:
              self.Loss     += self.loss[mol]*self.weight[mol]
           elif mol_ in self.weight:
              self.Loss     += self.loss[mol]*self.weight[mol_]
           else:
              self.Loss     += self.loss[mol]
-
-          self.accuracy += self.accur[mol]
+             
+          if mol.find('nomb_')<0:
+             self.accuracy += self.accur[mol]
 
       self.ME   = 0.0
       for mol in self.mols:
           mols = mol.split('-')[0] 
           self.ME += tf.square(self.MolEnergy[mols])
 
       self.loss_penalty = self.supervise()
@@ -630,32 +631,35 @@
   def get_atom_energy(self):
       i = 0
       for sp in self.spec:
           if self.nsp[sp]==0:
              continue
           self.eatom[sp] = -tf.ones([self.nsp[sp]])*self.p['atomic_'+sp]
           self.delta[sp] = tf.gather_nd(self.Delta,self.atomlist[sp])
+          dp             = tf.gather_nd(self.Deltap,self.atomlist[sp])
           self.dang[sp]  = self.delta[sp] - self.p['valang_'+sp]
 
           self.get_elone(sp,self.delta[sp]) 
           self.ELONE  = self.EL[sp] if i==0 else tf.concat((self.ELONE,self.EL[sp]),0)
           self.Dlp[sp]= self.delta[sp] - self.p['val_'+sp] - self.Delta_lp[sp]
           DLP_        = self.Dlp[sp] if i==0 else tf.concat((DLP_,self.Dlp[sp]),0)
 
           NLP_    = self.nlp[sp]  if i==0 else tf.concat((NLP_,self.nlp[sp]),0)
           DANG_   = self.dang[sp] if i==0 else tf.concat((DANG_,self.dang[sp]),0)
+          Dp_     = dp if i==0 else tf.concat((Dp_,dp),0)
           i      += 1
 
-      self.Dang= tf.gather_nd(DANG_,self.dalink)   
-      self.NLP = tf.gather_nd(NLP_,self.dalink) 
-
-      DLPL     = tf.gather_nd(DLP_,self.dalink)     
-      self.DLP = tf.gather_nd(DLPL,self.dalist)  # warning: zero pitfal for dalist
-      self.DPIL= tf.reduce_sum(input_tensor=self.BPI*self.DLP,axis=1,name='DPI') # 
-      self.DPI = tf.reduce_sum(input_tensor=self.BPI,axis=1,name='DPI') # *self.DLP
+      self.Dang   = tf.gather_nd(DANG_,self.dalink)   
+      self.Dang_p = tf.gather_nd(Dp_,self.dalink) 
+      self.NLP    = tf.gather_nd(NLP_,self.dalink) 
+
+      DLPL        = tf.gather_nd(DLP_,self.dalink)     
+      self.DLP    = tf.gather_nd(DLPL,self.dalist)  # warning: zero pitfal for dalist
+      self.DPIL   = tf.reduce_sum(input_tensor=self.BPI*self.DLP,axis=1,name='DPI') # 
+      self.DPI    = tf.reduce_sum(input_tensor=self.BPI,axis=1,name='DPI') # *self.DLP
     
       i = 0
       for sp in self.spec:
           if self.nsp[sp]==0:
              continue
           self.Dpi[sp]   = tf.gather_nd(self.DPIL,self.atomlist[sp])
 
@@ -826,14 +830,15 @@
       for ang in self.angs:
           if self.nang[ang]>0:
              atomj = ang.split('-')[1]    
              D     = tf.gather_nd(self.Delta,self.dglist[ang])
              Di    = tf.gather_nd(self.Delta,self.dgilist[ang])
              Dk    = tf.gather_nd(self.Delta,self.dgklist[ang])
              self.D_ang[ang] = tf.gather_nd(self.Dang,self.dglist[ang])
+             self.D_p[ang]   = tf.gather_nd(self.Dang_p,self.dglist[ang])
              # self.D_ang[ang] = D - self.p['valang_'+atomj]
 
              self.get_eangle(ang,atomj,D)
              self.get_epenalty(ang,atomj,D)
              self.get_three_conj(ang,atomj,D,Di,Dk)
 
       for mol in self.mols:
@@ -1531,24 +1536,30 @@
       if not self.sess_build:
          self.session(learning_rate=learning_rate,method=method)  
 
       accs_={}
       libfile = self.libfile.split('.')[0]
 
       for i in range(step+1):
-          loss,lpenalty,ME_,accu,accs,_ = self.sess.run([self.Loss,
+          if i==0:
+             loss,lpenalty,ME_,accu,accs = self.sess.run([self.Loss,
                                                       self.loss_penalty,
                                                       self.ME,
                                                       self.accuracy,
-                                                      self.accur,
-                                                      self.train_step],
+                                                      self.accur],
                                                   feed_dict=self.feed_dict)
-          if i==0:
              accMax = accu
           else:
+             loss,lpenalty,ME_,accu,accs,_ = self.sess.run([self.Loss,
+                                                      self.loss_penalty,
+                                                      self.ME,
+                                                      self.accuracy,
+                                                      self.accur,
+                                                      self.train_step],
+                                                  feed_dict=self.feed_dict)
              if accu>accMax:
                 accMax = accu
 
           if np.isnan(loss):
              if close_session:
                 self.logger.info('NAN error encountered at step %d loss is %f.' %(i,loss/self.nframe))
                 # send_msg('NAN error encountered at step %d loss is %f.' %(i,loss/self.nframe))
@@ -1569,15 +1580,16 @@
 
           if i%print_step==0:
              current = time.time()
              elapsed_time = current - self.time
 
              acc = ''
              for key in accs:
-                 acc += key+': %6.4f ' %accs[key]
+                 if key.find('nomb_')<0:
+                    acc += key+': %6.4f ' %accs[key]
 
              self.logger.info('-  step: %d loss: %6.4f accs: %f %s spv: %6.4f me: %6.4f time: %6.4f' %(i,
                              loss_,accu,acc,lpenalty,ME_,elapsed_time))
              self.time = current
 
           if i%writelib==0 or i==step:
              self.lib_bk = libfile+'_'+str(i)
@@ -1956,15 +1968,15 @@
       self.f4r,self.f5r,self.f_4,self.f_5,self.df4,self.df5=None,None,None,None,None,None
       self.F,self.F_11,self.F_12,self.F_45=None,None,None,None
       self.fbot = None
       self.powb,self.expb,self.EBD,self.ebond,self.ebda = None,None,None,None,None
       self.sieng,self.pieng,self.ppeng = None,None,None
 
       self.D,self.Delta_e,self.DE,self.nlp,self.Delta_lp,self.Dlp = None,None,None,None,None,None
-      self.Dpi,self.BSO,self.BOPI,self.Delta_lpcorr = None,None,None,None
+      self.D_p,self.Dpi,self.BSO,self.BOPI,self.Delta_lpcorr = None,None,None,None,None
       self.explp,self.EL,self.elone,self.Elone,self.ELONE = None,None,None,None,None
       self.EOV,self.Eover,self.eover,self.otrm1,self.otrm2 =  None,None,None,None,None
 
       self.expeu1,self.expeu2,self.eu1,self.expeu3,self.eu2,self.EUN = None,None,None,None,None,None
       self.eunder,self.Eunder = None,None
 
       self.EANG,self.Eang,self.eang,self.theta0,self.fijk = None,None,None,None,None
@@ -2221,15 +2233,15 @@
         elif key=='val9':
            p[k] = tf.clip_by_value(v[k],0.0,6.0)
         elif key=='val':
            sp = vn[1]
            p[k] = tf.clip_by_value(v[k],0.0,8.0)
         elif key=='vale':
            sp = vn[1]
-           p[k] = tf.clip_by_value(v[k],v['val_'+sp],16.0)
+           p[k] = tf.clip_by_value(v[k],v['valang_'+sp],16.0)
         elif key=='valboc':
            sp = vn[1]
            p[k] = tf.clip_by_value(v[k],0.0,100.0)
         elif key=='valang':
            sp = vn[1]
            p[k] = tf.clip_by_value(v[k],0.0,2.0*p_['val_'+sp])
         else:
```

### Comparing `irff-1.5.2/irff/reax_data.py` & `irff-1.5.3/irff/reax_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,18 +190,32 @@
              
       self.R,self.vr = self.compute_bond(self.x)
       image_rs = self.compute_image(self.vr)                            # vdw interaction images
 
       self.get_table()
       self.get_bonds(self.R)
 
-      self.compute_angle(self.R,self.vr)
-      self.compute_torsion(self.R,self.vr)
-
-      self.compute_hbond(image_rs)
+      if self.structure.find('nomb')>=0:
+         self.nhb  = 0
+         self.nang = 0
+         self.ntor = 0
+         self.hb_i,self.hb_j,self.hb_k = [],[],[]
+         self.abij,self.abjk = [],[]
+         self.ang_i,self.ang_j,self.ang_k = [],[],[]
+         self.tij,self.tjk,self.tkl = [],[],[]
+         self.tor_i,self.tor_j,self.tor_k,self.tor_l = [],[],[],[]
+         self.A,self.T,self.H,self.hij={},{},{},{}
+         self.na,self.nt={},{}
+         self.theta,self.s_ijk,self.s_jkl,self.w,self.rhb = None,None,None,None,None
+         self.frhb,self.hbthe = None,None
+      else:
+         self.compute_angle(self.R,self.vr)
+         self.compute_torsion(self.R,self.vr)
+         self.compute_hbond(image_rs)
+         
       self.compute_vdw(image_rs)
 
       # self.get_gulp_energy()
       self.get_charge()
       self.get_ecoul(image_rs)
       self.get_eself()
```

### Comparing `irff-1.5.2/irff/reax_nn.py` & `irff-1.5.3/irff/reax_nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,26 +37,27 @@
                hbshort=6.75,hblong=7.5,
                vdwcut=10.0,
                atol=0.001,
                hbtol=0.001,
                bore={'others':0.0},
                weight={'others':1.0},
                spv_vdw=False,vlo={'others':[(0.0,0.0)]},vup={'others':[(10.0,0.0)]},
+               spv_bo=None,                 # e.g. spv_bo={'C-C':(1.3,8.5,8.5,0.0,0.0)}
                interactive=False,
                ro_scale=0.1,
                clip_op=True,
                clip={'others':(0.4,1.0)},   # parameter range
                InitCheck=True,
                resetDeadNeuron=False,
                optmol=True,
                lambda_me=0.1,
                nnopt=True,
                be_universal_nn=None,be_layer=[9,0],
                mf_universal_nn=None,mf_layer=[9,0],
-               messages=1,
+               messages=1,MessageFunction=2,
                bo_layer=None,
                spec=[],
                board=False,
                lambda_bd=100000.0,
                lambda_pi=1.0,
                lambda_reg=0.01,
                lambda_ang=1.0,
@@ -116,19 +117,21 @@
       else:
          self.regularize = False
       self.lambda_reg    = lambda_reg
       self.lambda_pi     = lambda_pi
       self.lambda_ang    = lambda_ang
       self.mf_layer      = mf_layer
       self.be_layer      = be_layer
-      self.be_universal_nn= be_universal_nn
-      self.mf_universal_nn= mf_universal_nn
-      self.messages      = messages
+      self.be_universal_nn = be_universal_nn
+      self.mf_universal_nn = mf_universal_nn
+      self.messages        = messages
+      self.MessageFunction = MessageFunction
       self.spv_vdw       = spv_vdw
       self.spv_ang       = spv_ang
+      self.spv_bo        = spv_bo
       self.vlo           = vlo
       self.vup           = vup
       self.bo_layer      = bo_layer
       self.weight        = weight
       self.spec          = spec
       self.time          = time.time()
       self.interactive   = interactive
@@ -147,23 +150,23 @@
       #self.hbtol        = hbtol    # hydrogen-bond bond-order tolerence
       self.fixrcbo       = fixrcbo
       self.m_,self.m     = None,None
 
       self.rcut,self.rcuta,self.re = self.read_lib()
       self.set_rcut(self.rcut,self.rcuta,self.re)
 
+      self.set_variable_list()
       self.ic = Intelligent_Check(re=self.re,clip=clip,spec=self.spec,bonds=self.bonds,
-                                  offd=self.offd,angs=self.angs,tors=self.torp)
+                                  offd=self.offd,angs=self.angs,tors=self.torp,ptor=self.p_tor)
       self.p_,self.m_ = self.ic.check(self.p_,self.m_,resetDeadNeuron=self.resetDeadNeuron)
 
       if not self.libfile.endswith('.json'):
          self.p_['acut']    = atol
          self.p_['hbtol']   = hbtol
 
-      self.set_neurons()
       self.torp          = self.checkTors(self.torp)
       
       self.lambda_bd     = lambda_bd
       self.logger        = logger('training.log')
       self.initialized   = False
       self.sess_build    = False
 
@@ -327,30 +330,35 @@
       self.frc = {}
       self.bop_si,self.bop_pi,self.bop_pp,self.bop = {},{},{},{}
       self.bosi,self.bosi_pen = {},{}
       self.bopi,self.bopp,self.bo0,self.bo,self.bso = {},{},{},{},{}
 
       self.Deltap,self.Delta,self.Bp = {},{},{}
       self.delta,self.Di,self.Dj,self.Di_boc,self.Dj_boc={},{},{},{},{}
-      self.D,self.H,self.Hsi,self.Hpi,self.Hpp = {},{},{},{},{}
+      self.D,self.D_si,self.D_pi,self.D_pp = {},{},{},{}
+      self.H,self.Hsi,self.Hpi,self.Hpp = {},{},{},{}
 
       self.SO,self.fbot,self.fhb = {},{},{}
       self.EBD,self.E = {},{}
       self.powb,self.expb,self.ebond = {},{},{}
 
       self.esi   = {}
       self.ebd   = {}
       self.rbd   = {}
       self.rbd_  = {}
+      self.Dbi   = {}
+      self.Dbj   = {}
       #self.bop_ = {}
       #self.bo0_ = {}
       for mol in self.mols:
           self.esi[mol]   = {}
           self.ebd[mol]   = {}
           self.rbd_[mol]  = {}
+          self.Dbi[mol]   = {}
+          self.Dbj[mol]   = {}
           #self.bop_[mol]  = {}
           #self.bo0_[mol]  = {}
 
       self.Delta_e,self.DE,self.Delta_lp,self.Dlp,self.Dang  = {},{},{},{},{}
       self.Bpi,self.Dpi,self.BSO,self.BOpi,self.Delta_lpcorr = {},{},{},{},{}
       self.eover,self.eunder,self.elone,self.Elone= {},{},{},{}
       self.EOV,self.EUN = {},{}
@@ -458,20 +466,30 @@
                            self.ecoul[mol] +
                            self.ehb[mol]   +
                            self.eself[mol], 
                            self.zpe[mol],name='E_%s' %mol)   
 
   def get_delta(self,mol):
       ''' compute the uncorrected Delta: the sum of BO '''
-      BOP = tf.zeros([1,self.batch[mol]])   # for ghost atom, the value is zero
+      BOP    = tf.zeros([1,self.batch[mol]])   # for ghost atom, the value is zero
+      BOP_si = tf.zeros([1,self.batch[mol]])   # for ghost atom, the value is zero
+      BOP_pi = tf.zeros([1,self.batch[mol]])   # for ghost atom, the value is zero
+      BOP_pp = tf.zeros([1,self.batch[mol]])   # for ghost atom, the value is zero
       self.get_bondorder_uc(mol)
+
       BOP              = tf.concat([BOP,self.bop[mol]],0)
-      # BOP            = tf.transpose(BOP,perm=[0,1])
+      BOP_si           = tf.concat([BOP,self.bop_si[mol]],0)
+      BOP_pi           = tf.concat([BOP,self.bop_pi[mol]],0)
+      BOP_pp           = tf.concat([BOP,self.bop_pp[mol]],0)
+
       self.Bp[mol]     = tf.gather_nd(BOP,self.blist[mol])
       self.Deltap[mol] = tf.reduce_sum(input_tensor=self.Bp[mol],axis=1,name='Deltap')
+      self.D_si[mol]   = [tf.reduce_sum(tf.gather_nd(BOP_si,self.blist[mol]),axis=1,name='Deltap_si')]
+      self.D_pi[mol]   = [tf.reduce_sum(tf.gather_nd(BOP_pi,self.blist[mol]),axis=1,name='Deltap_pi')]
+      self.D_pp[mol]   = [tf.reduce_sum(tf.gather_nd(BOP_pp,self.blist[mol]),axis=1,name='Deltap_pp')]
 
   def get_bond_energy(self,mol):
       self.get_delta(mol)
       self.message_passing(mol)
       self.get_final_sate(mol)
       self.get_ebond(mol)
       self.ebond[mol]= tf.reduce_sum(input_tensor=self.EBD[mol],axis=0,name='bondenergy')
@@ -548,21 +566,38 @@
 
           h    = tf.slice(self.H[mol][t-1],[b_[0],0],[b_[1],self.batch[mol]],name=bd+'_h_slice')
           hsi  = tf.slice(self.Hsi[mol][t-1],[b_[0],0],[b_[1],self.batch[mol]],name=bd+'_hsi_slice')
           hpi  = tf.slice(self.Hpi[mol][t-1],[b_[0],0],[b_[1],self.batch[mol]],name=bd+'_hpi_slice')
           hpp  = tf.slice(self.Hpp[mol][t-1],[b_[0],0],[b_[1],self.batch[mol]],name=bd+'_hpp_slice')
 
           b    = bd.split('-')
-          Dbi  = Di - h   
-          Dbj  = Dj - h   
-          
-          Fi   = fmessage(flabel,b[0],self.nbd[mol][bd],[Dbi,h,Dbj],self.m,
-                          batch=self.batch[mol],layer=self.mf_layer[1])
-          Fj   = fmessage(flabel,b[1],self.nbd[mol][bd],[Dbj,h,Dbi],self.m,
-                          batch=self.batch[mol],layer=self.mf_layer[1])
+
+          if self.MessageFunction==1:
+             Dsi_i = tf.gather_nd(self.D_si[mol][t-1],self.dilink[mol][bd]) - hsi
+             Dpi_i = tf.gather_nd(self.D_pi[mol][t-1],self.dilink[mol][bd]) - hpi
+             Dpp_i = tf.gather_nd(self.D_pp[mol][t-1],self.dilink[mol][bd]) - hpp 
+             
+             Dsi_j = tf.gather_nd(self.D_si[mol][t-1],self.djlink[mol][bd]) - hsi
+             Dpi_j = tf.gather_nd(self.D_pi[mol][t-1],self.djlink[mol][bd]) - hpi
+             Dpp_j = tf.gather_nd(self.D_pp[mol][t-1],self.djlink[mol][bd]) - hpp
+
+             Dpii  = Dpi_i + Dpp_i
+             Dpij  = Dpi_j + Dpp_j
+            
+             Fi    = fmessage(flabel,b[0],nbd_,[Dsi_i,Dpii,h,Dpij,Dsi_j],
+                              self.m,batch=self.batch[mol],layer=self.mf_layer[1])
+             Fj    = fmessage(flabel,b[1],nbd_,[Dsi_j,Dpij,h,Dpii,Dsi_i],
+                              self.m,batch=self.batch[mol],layer=self.mf_layer[1])
+          elif self.MessageFunction==2:
+             self.Dbi[mol][bd]  = Di - h   
+             self.Dbj[mol][bd]  = Dj - h   
+             Fi   = fmessage(flabel,b[0],nbd_,[self.Dbi[mol][bd],h,self.Dbj[mol][bd]],self.m,
+                             batch=self.batch[mol],layer=self.mf_layer[1])
+             Fj   = fmessage(flabel,b[1],nbd_,[self.Dbj[mol][bd],h,self.Dbi[mol][bd]],self.m,
+                             batch=self.batch[mol],layer=self.mf_layer[1])
           F    = Fi*Fj
           Fsi,Fpi,Fpp = tf.unstack(F,axis=2)
 
           bosi_.append(hsi*Fsi)
           bopi_.append(hpi*Fpi)
           bopp_.append(hpp*Fpp)
 
@@ -570,33 +605,46 @@
       bopi = tf.concat(bopi_,0)
       bopp = tf.concat(bopp_,0)
       bo   = bosi+bopi+bopp
       return bo,bosi,bopi,bopp
 
   def message_passing(self,mol):
       ''' finding the final Bond-order with a message passing '''
-      self.H[mol]   = [self.bop[mol]]                     # 
-      self.Hsi[mol] = [self.bop_si[mol]]                  #
-      self.Hpi[mol] = [self.bop_pi[mol]]                  #
-      self.Hpp[mol] = [self.bop_pp[mol]]                  # 
-      self.D[mol]   = [self.Deltap[mol]]                  # get the initial hidden state H[0]
+      self.H[mol]    = [self.bop[mol]]                     # 
+      self.Hsi[mol]  = [self.bop_si[mol]]                  #
+      self.Hpi[mol]  = [self.bop_pi[mol]]                  #
+      self.Hpp[mol]  = [self.bop_pp[mol]]                  # 
+      self.D[mol]    = [self.Deltap[mol]]                  # get the initial hidden state H[0]
 
       for t in range(1,self.messages+1):
           print('-  message passing for {:s} t={:d} ...'.format(mol,t))           
           BO    = tf.zeros([1,self.batch[mol]])           # for ghost atom, the value is zero
+          BOsi  = tf.zeros([1,self.batch[mol]])           # for ghost atom, the value is zero
+          BOpi  = tf.zeros([1,self.batch[mol]])           # for ghost atom, the value is zero
+          BOpp  = tf.zeros([1,self.batch[mol]])           # for ghost atom, the value is zero
           bo,bosi,bopi,bopp = self.get_bondorder(mol,t)
           self.H[mol].append(bo)                      # get the hidden state H[t]
           self.Hsi[mol].append(bosi)
           self.Hpi[mol].append(bopi)
           self.Hpp[mol].append(bopp)
 
           BO      = tf.concat([BO,bo],0)
-          D       = tf.gather_nd(BO,self.blist[mol])  
-          Delta   = tf.reduce_sum(input_tensor=D,axis=1)
+          BOsi    = tf.concat([BOsi,bosi],0)
+          BOpi    = tf.concat([BOpi,bopi],0)
+          BOpp    = tf.concat([BOpp,bopp],0)
+
+          Delta   = tf.reduce_sum(tf.gather_nd(BO,self.blist[mol]),axis=1) 
+          Dsi     = tf.reduce_sum(tf.gather_nd(BOsi,self.blist[mol]),axis=1) 
+          Dpi     = tf.reduce_sum(tf.gather_nd(BOpi,self.blist[mol]),axis=1) 
+          Dpp     = tf.reduce_sum(tf.gather_nd(BOpp,self.blist[mol]),axis=1)  
+
           self.D[mol].append(Delta)                  # degree matrix
+          self.D_si[mol].append(Dsi)
+          self.D_pi[mol].append(Dpi)
+          self.D_pp[mol].append(Dpp)
 
   def get_final_sate(self,mol):     
       self.Delta[mol]  = self.D[mol][-1]
       self.bo0[mol]    = self.H[mol][-1]                 # fetch the final state 
       self.bosi[mol]   = self.Hsi[mol][-1]
       self.bopi[mol]   = self.Hpi[mol][-1]
       self.bopp[mol]   = self.Hpp[mol][-1]
@@ -1002,29 +1050,32 @@
           else:
              raise NotImplementedError('-  This function not supported yet!')
 
           sum_edft = tf.reduce_sum(input_tensor=tf.abs(self.dft_energy[mol]-self.max_e[mol]))
           self.accur[mol] = 1.0 - tf.reduce_sum(input_tensor=tf.abs(self.E[mol]-self.dft_energy[mol]))/(sum_edft+0.00000001)
          
           self.Loss     += self.loss[mol]*w_
-          self.accuracy += self.accur[mol]
+          if mol.find('nomb_')<0:
+             self.accuracy += self.accur[mol]
+          else:
+             self.nmol -= 1
 
       self.ME   = 0.0
       for mol in self.mols:
           mol_     = mol.split('-')[0] 
           self.ME += tf.square(self.MolEnergy[mol_])
 
       self.loss_penalty = self.supervise()
       self.Loss        += self.loss_penalty
 
       if self.optmol:
          self.Loss  += self.ME*self.lambda_me
       self.accuracy  = self.accuracy/self.nmol
 
-  def set_neurons(self):
+  def set_variable_list(self):
       self.unit = 4.3364432032e-2
       self.p_g  = ['boc1','boc2','coa2','ovun6','lp1',#'lp3',
                    'ovun7','ovun8','val6','tor2',
                    'tor3','tor4','cot2','coa4','ovun4',               # 
                    'ovun3','val8','val9','val10',
                    'coa3','pen2','pen3','pen4','vdw1',
                    'cutoff','hbtol','acut'] # # 
@@ -1161,16 +1212,16 @@
              self.p[k] = self.var[k]
              
       self.botol       = 0.01*self.p['cutoff']
       self.checkp()
       self.get_rcbo()
       self.m = set_matrix(self.m_,self.spec,self.bonds,
                           self.mfopt,self.mpopt,self.bdopt,self.messages,
-                          self.bo_layer,self.bo_layer_,0,0,
-                          self.mf_layer,self.mf_layer_,3,3,
+                          (6,0),(6,0),0,0,
+                          self.mf_layer,self.mf_layer_,self.MessageFunction_,self.MessageFunction,
                           self.be_layer,self.be_layer_,1,1,
                           (9,0),(9,0),1,1,
                           None,self.be_universal_nn,self.mf_universal_nn,None)
 
   def set_parameters(self,libfile=None):
       if not libfile is None:
          self.p_,zpe,spec,bonds,offd,angs,torp,hbs = read_ffield(libfile=libfile)
@@ -1196,15 +1247,15 @@
       self.atol        = self.p['acut']
       self.hbtol       = self.p['hbtol']
       self.checkp()
       self.get_rcbo()
       self.m = set_matrix(self.m_,self.spec,self.bonds,
                           self.mfopt,self.mpopt,self.bdopt,self.messages,
                           (6,0),(6,0),0,0,
-                          self.mf_layer,self.mf_layer_,3,3,
+                          self.mf_layer,self.mf_layer_,self.MessageFunction_,self.MessageFunction,
                           self.be_layer,self.be_layer_,1,1,
                           (9,0),(9,0),1,1,
                           None,self.be_universal_nn,self.mf_universal_nn,None)
 
   def stack_threebody_parameters(self,mol):
       val_,val1_,val2_,val3_,val4_,val5_,val7_= [],[],[],[],[],[],[]
       valboc_,valang_,theta0_,pen1_,coa1_ = [],[],[],[],[]
@@ -1660,15 +1711,15 @@
                 self.m_[key] = self.m_[key].tolist()  # covert ndarray to list
          # print(' * save parameters to file ...')
          fj = open(libfile+'.json','w')
          j = {'p':self.p_,'m':self.m_,
               'score':score,
               'BOFunction':0,#self.BOFunction,
               'EnergyFunction':1,# self.EnergyFunction,
-              'MessageFunction':3,# self.MessageFunction, 
+              'MessageFunction': self.MessageFunction, 
               'VdwFunction':1,#self.VdwFunction,
               'messages':self.messages,
               'bo_layer':self.bo_layer,
               'mf_layer':self.mf_layer,
               'be_layer':self.be_layer,
               'vdw_layer':None,#self.vdw_layer,
               'rcut':self.rcut,
@@ -1691,15 +1742,15 @@
       if self.libfile.endswith('.json'):
          with open(self.libfile,'r') as lf:
               j = js.load(lf)
          self.p_  = j['p']
          self.m_  = j['m']
          # self.BOFunction_      = j['BOFunction']
          # self.EnergyFunction_  = j['EnergyFunction'] 
-         # self.MessageFunction_ = j['MessageFunction']
+         self.MessageFunction_ = j['MessageFunction']
          # self.VdwFunction_     = j['VdwFunction']
          self.MolEnergy_         = j['MolEnergy']
          # self.bo_layer_        = j['bo_layer']
          self.mf_layer_          = j['mf_layer']
          self.be_layer_          = j['be_layer']
          # self.vdw_layer_       = j['vdw_layer']
          rcut                    = j['rcut']
@@ -1713,16 +1764,14 @@
          rcut,rcuta,re = None,None,None
       return rcut,rcuta,re
 
   def supervise(self):
       ''' adding some penalty term to accelerate the training '''
       log_    = -9.21044036697651
       penalty = 0.0
-      pen_w   = 0.0
-      pen_b   = 0.0
       wb_p    = []
       if self.regularize_be:
          wb_p.append('fe')
       # if self.vdwnn and self.regularize_vdw:
       #    wb_p.append('fv')
       w_n     = ['wi','wo',]
       b_n     = ['bi','bo']
@@ -1732,19 +1781,22 @@
 
       wb_message = []
       if self.regularize_mf:
          for t in range(1,self.messages+1):
              wb_message.append('fm')          
              layer['fm'] = self.mf_layer[1]  
 
-      self.penalty_bop = {}
+      self.penalty_bop     = {}
+      self.penalty_bo      = {}
       self.penalty_bo_rcut = {}
-      self.penalty_be_cut = {}
-      self.penalty_rcut = {}
-      self.penalty_ang  = {}
+      self.penalty_be_cut  = {}
+      self.penalty_rcut    = {}
+      self.penalty_ang     = {}
+      self.penalty_w       = tf.constant(0.0)
+      self.penalty_b       = tf.constant(0.0)
 
       for bd in self.bonds: 
           atomi,atomj = bd.split('-') 
           bdr = atomj + '-' + atomi
           # log_ = tf.math.log((self.botol/(1.0 + self.botol)))
           if self.fixrcbo:
              rcut_si = tf.square(self.rc_bo[bd]-self.rcut[bd])
@@ -1759,96 +1811,119 @@
 
           self.penalty_rcut[bd] = rcut_si + rcut_pi + rcut_pp
           penalty = tf.add(self.penalty_rcut[bd]*self.lambda_bd,penalty)
  
           self.penalty_bop[bd]     = tf.constant(0.0)
           self.penalty_be_cut[bd]  = tf.constant(0.0)
           self.penalty_bo_rcut[bd] = tf.constant(0.0)
+          self.penalty_bo[bd]      = tf.constant(0.0)
+
           for mol in self.mols:
               if self.nbd[mol][bd]>0:       
                  b_   = self.b[mol][bd]
                  #rbd_= tf.slice(self.rbd[mol],[b_[0],0],[b_[1],self.batch[mol]])        
                  bop_ = tf.slice(self.bop[mol],[b_[0],0],[b_[1],self.batch[mol]]) 
                  bo0_ = tf.slice(self.bo0[mol],[b_[0],0],[b_[1],self.batch[mol]]) 
 
                  fbo  = tf.where(tf.less(self.rbd_[mol][bd],self.rc_bo[bd]),0.0,1.0)     # bop should be zero if r>rcut_bo
                  self.penalty_bop[bd]  +=  tf.reduce_sum(bop_*fbo)                       #####  
 
                  fao  = tf.where(tf.greater(self.rbd_[mol][bd],self.rcuta[bd]),1.0,0.0)  ##### r> rcuta that bo = 0.0
                  self.penalty_bo_rcut[bd] += tf.reduce_sum(bo0_*fao)
 
-                 fesi = tf.where(tf.less_equal(bop_,self.botol),1.0,0.0)                 ##### bo <= 0.0 that e = 0.0
+                 fesi = tf.where(tf.less_equal(bo0_,self.botol),1.0,0.0)                 ##### bo <= 0.0 that e = 0.0
                  self.penalty_be_cut[bd]  += tf.reduce_sum(tf.nn.relu(self.esi[mol][bd]*fesi))
+                 
+                 if self.spv_bo:
+                     if (bd in self.spv_bo) or (bdr in self.spv_bo):
+                        bd_  = bd if bd in self.spv_bo else bdr
+                     for sbo in self.spv_bo[bd_]:
+                         r,d_i,d_j,bo_l,bo_u = sbo
+                         fe   = tf.where(tf.logical_and(tf.less_equal(self.rbd[bd],r),
+                                                         tf.logical_and(tf.greater_equal(self.Dbi[bd],d_i),
+                                                                        tf.greater_equal(self.Dbj[bd],d_j))),
+                                          1.0,0.0)   ##### r< r_e that bo > bore_
+                         self.penalty_bo[bd] += tf.reduce_sum(input_tensor=tf.nn.relu((bo_l-self.bo0[bd])*fe))
+                         fe   = tf.where(tf.logical_and(tf.greater_equal(self.rbd[bd],r),
+                                                         tf.logical_and(tf.greater_equal(self.Dbi[bd],d_i),
+                                                                        tf.greater_equal(self.Dbj[bd],d_j))),
+                                          1.0,0.0)  ##### r> r_e that bo < bore_
+                         self.penalty_bo[bd] += tf.reduce_sum(input_tensor=tf.nn.relu((self.bo0[bd]-bo_u)*fe))
 
               if self.spv_ang:
                  self.penalty_ang[mol] = tf.reduce_sum(self.thet2[mol]*self.fijk[mol])
           
           penalty  = tf.add(self.penalty_be_cut[bd]*self.lambda_bd,penalty)
           penalty  = tf.add(self.penalty_bop[bd]*self.lambda_bd,penalty)        
           penalty  = tf.add(self.penalty_bo_rcut[bd]*self.lambda_bd,penalty)
+          penalty  = tf.add(self.penalty_bo[bd]*self.lambda_bd,penalty)   
 
           # penalize term for regularization of the neural networs
           if self.regularize:                             # regularize to avoid overfit
              for k in wb_p:
                  for k_ in w_n:
                      key     = k + k_ + '_' + bd
-                     pen_w  += tf.reduce_sum(tf.square(self.m[key]))
+                     self.penalty_w  += tf.reduce_sum(tf.square(self.m[key]))
                  if self.regularize_bias:
                     for k_ in b_n:
                         key     = k + k_ + '_' + bd
-                        pen_b  += tf.reduce_sum(tf.square(self.m[key]))
+                        self.penalty_b  += tf.reduce_sum(tf.square(self.m[key]))
                  for l in range(layer[k]):                                               
-                     pen_w += tf.reduce_sum(tf.square(self.m[k+'w_'+bd][l]))
+                     self.penalty_w += tf.reduce_sum(tf.square(self.m[k+'w_'+bd][l]))
                      if self.regularize_bias:
-                        pen_b += tf.reduce_sum(tf.square(self.m[k+'b_'+bd][l]))
+                        self.penalty_b += tf.reduce_sum(tf.square(self.m[k+'b_'+bd][l]))
 
       if self.regularize:                              # regularize
          for sp in self.spec:
              for k in wb_message:
                  for k_ in w_n:
                      key     = k + k_ + '_' + sp
-                     pen_w  += tf.reduce_sum(tf.square(self.m[key]))
+                     self.penalty_w  += tf.reduce_sum(tf.square(self.m[key]))
                  if self.regularize_bias:
                     for k_ in b_n:
                         key     = k + k_ + '_' + sp
-                        pen_b  += tf.reduce_sum(tf.square(self.m[key]))
+                        self.penalty_b  += tf.reduce_sum(tf.square(self.m[key]))
                  for l in range(layer[k]):                                               
-                     pen_w += tf.reduce_sum(tf.square(self.m[k+'w_'+sp][l]))
+                     self.penalty_w += tf.reduce_sum(tf.square(self.m[k+'w_'+sp][l]))
                      if self.regularize_bias:
-                        pen_b += tf.reduce_sum(tf.square(self.m[k+'b_'+sp][l]))
-         penalty = tf.add(self.lambda_reg*pen_w,penalty)
-         penalty = tf.add(self.lambda_reg*pen_b,penalty)
+                        self.penalty_b += tf.reduce_sum(tf.square(self.m[k+'b_'+sp][l]))
+         penalty = tf.add(self.lambda_reg*self.penalty_w,penalty)
+         penalty = tf.add(self.lambda_reg*self.penalty_b,penalty)
       return penalty
 
   def get_pentalty(self):
       (penalty_bop,penalty_bo_rcut,
-          penalty_be_cut,
-          penalty_rcut,rc_bo) = self.sess.run([self.penalty_bop,self.penalty_bo_rcut,
-                                         self.penalty_be_cut,
-                                         self.penalty_rcut,self.rc_bo],
+          penalty_bo,penalty_be_cut,
+          penalty_rcut,rc_bo,
+          penalty_w,penalty_b) = self.sess.run([self.penalty_bop,self.penalty_bo_rcut,
+                                         self.penalty_bo,self.penalty_be_cut,
+                                         self.penalty_rcut,self.rc_bo,
+                                         self.penalty_w,self.penalty_b],
                                          feed_dict=self.feed_dict)
       rcut = self.rcut
       print('\n------------------------------------------------------------------------')
       print('-                                                                      -')
       print('-                         Penalty Information                          -')
       print('-                                                                      -')
       print('------------------------------------------------------------------------\n')
       for bd in self.bonds:
           if bd in penalty_bop:
              print('bop cutoff penalty of                             {:5s}: {:6.4f}'.format(bd,penalty_bop[bd]))
-         #  if bd in penalty_bo:
-         #     print('BO state penalty of                             {:5s}: {:6.4f}'.format(bd,penalty_bo[bd]))
+          if bd in penalty_bo:
+             print('BO state penalty of                               {:5s}: {:6.4f}'.format(bd,penalty_bo[bd]))
           if bd in penalty_bo_rcut:
              print('Differency between rcut-bo and rcut Penalty of    {:5s}: {:6.4f} {:6.4f} {:6.4f}'.format(bd,penalty_bo_rcut[bd],rc_bo[bd],rcut[bd]))
           # if bd in penalty_esi:
           #    print('Differency between bosi and esi Penalty of      {:5s}: {:6.4f}'.format(bd,penalty_esi[bd]))
           if bd in penalty_be_cut: 
              print('Bond-Energy at radius cutoff penalty of           {:5s}: {:6.4f}'.format(bd,penalty_be_cut[bd]))
           if bd in penalty_rcut:
              print('Bond-Order at radius cutoff penalty of            {:5s}: {:6.4f}'.format(bd,penalty_rcut[bd]))
+      print('Sum of square of weight:                          {:6.4f}'.format(penalty_w))
+      print('Sum of square of bias:                            {:6.4f}'.format(penalty_b))
       print('\n')
      
       # print('\n------------------------------------------------------------------------')
       # print('-                 -  Energy Components Information  -                  -')
       # print('------------------------------------------------------------------------\n')
       # for mol in self.mols:
       #     print('Max Bond-Order of {:s} {:f}'.format(mol,np.max(bo[mol])))
```

### Comparing `irff-1.5.2/irff/reaxfflib.py` & `irff-1.5.3/irff/reaxfflib.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/spectra.py` & `irff-1.5.3/irff/spectra.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/structures/Al.gen` & `irff-1.5.3/irff/structures/Al.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/structures/C2C4.gen` & `irff-1.5.3/irff/structures/C2C4.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/structures/FAlF.gen` & `irff-1.5.3/irff/structures/nm3.gen`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-20  S    
-C    F    Al   
-1      1      1.330629400693213      2.588795568854290      1.811583572787756
-2      1      2.331968960777784      1.663621050464333      1.098474046886208
-3      2      1.898875443190682      3.156258731006313      2.925917003492592
-4      2      0.916574432998905      3.596638668943495      0.975241675397568
-5      2      1.762903787150570      1.095670504770712     -0.015556924770741
-6      2      2.745204797342348      0.655290566833531      1.935118403324282
-7      2      3.417839916859951      2.015229520997601      0.398613387582728
-8      2      0.186988294972021      2.160126131879196      2.052207241518524
-9      3      0.672955705040224      1.002125284888239      5.277265655464948
-10     3      0.672955705040224      3.027125284888238      7.302265655464947
-11     3      2.697955705040223      1.002125284888239      7.302265655464947
-12     3      2.697955705040223      3.027125284888238      5.277265655464948
-13     1      1.389863721217992      2.626924368738866     11.406362575759186
-14     1      2.391203281302563      1.701749850348911     10.693253049857635
-15     2      1.958109763715461      3.194387530890889     12.520696006464021
-16     2      0.975808753523685      3.634767468828071     10.570020678368996
-17     2      1.822138107675349      1.133799304655290      9.579222078200686
-18     2      2.804439117867127      0.693419366718109     11.529897406295710
-19     2      3.477074237384730      2.053358320882177      9.993392390554156
-20     2      0.246222615496801      2.198254931763772     11.646986244489952
+21  S    
+C    N    O    H    
+1      1      6.176825186867148      1.849305573098204      2.632977730913833
+2      2      5.524048840000000      3.346482360000000      1.836397456000000
+3      3      4.488014080000000      3.835091968000000      1.206684984000000
+4      3      6.456092472000000      3.843426304000000      2.548136920000000
+5      4      2.053670347836237      1.650928887868471      3.256710983250413
+6      4      5.555666930867148      2.079496965098204      3.594848738913833
+7      4      6.059737642867148      0.753225485098204      2.390797786913833
+8      1      2.457641435836234      0.904176223868471      3.987813559250413
+9      2      3.572801571836245      1.668797855868471      4.641173695250414
+10     3      4.163038312970526      2.644291522110522      4.417496977909530
+11     3      4.522011451718785      0.873975221042620      5.289671422062201
+12     4      2.778914371836232     -0.122961472131533      3.667475175250413
+13     4      7.422050106867149      1.904981181098204      2.933404154913833
+14     4      1.612996555836242      0.896594783868471      4.688164295250414
+15     1      3.400593072000000      5.690966656000000      3.609735000000000
+16     2      4.373822688000000      5.567081168000000      4.706918128000000
+17     3      3.837353248000000      5.814201976000000      5.784274344000000
+18     3      5.465852648000000      5.089990760000000      4.632640128000000
+19     4      3.955645032000000      5.935428360000000      2.723515992000000
+20     4      2.837771168000000      4.764140208000000      3.423837952000000
+21     4      2.790227480000000      6.501172048000000      3.922247888000000
      0.000000000000000      0.000000000000000      0.000000000000000 
-     4.050000000000000      0.000000000000000      0.000000000000000 
-     0.000000000000000      4.050000000000000      0.000000000000000 
-     0.000000000000000      0.000000000000000     13.000000000000000 
+     8.000000000000000      0.000000000000000      0.000000000000000 
+     0.000000000000000      8.000000000000000      0.000000000000000 
+     0.000000000000000      0.000000000000000      8.000000000000000
```

### Comparing `irff-1.5.2/irff/structures/HMX_MOL.gen` & `irff-1.5.3/irff/structures/HMX_MOL.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/structures/NM.gen` & `irff-1.5.3/irff/structures/NM.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/structures/ball.py` & `irff-1.5.3/irff/structures/ball.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/structures/ball_bulk.py` & `irff-1.5.3/irff/structures/ball_bulk.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/structures/cl20.gen` & `irff-1.5.3/irff/structures/fox7.gen`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,62 @@
-36  S    
-C    H    N    O    
-1      1      5.817991306000000      7.302328837999999      5.958274491999999
-2      2      5.302913295000000      8.453501278999999      5.423650868999999
-3      1      7.703157563000000      5.916653171000000      5.943459916000000
-4      2      8.960501476999999      5.786990587000000      5.417273574000000
-5      1      6.720529951999999      5.090003405999999      7.845088939000000
-6      2      7.070117287000000      4.535168484000000      9.046917384000000
-7      1      6.695061994000000      4.566898655000000      5.613226957000000
-8      2      7.353062956999999      3.598914446000000      4.901797280000000
-9      1      4.809589626000000      5.949916994000000      5.648437741000000
-10     2      3.698013809000000      6.330417894000000      4.944970370000000
-11     1      5.368488880000000      6.117717038000000      7.868472404000000
-12     2      4.833762003000000      6.247143252999999      9.122152882000000
-13     3      7.680650310999999      7.890947997999999      4.517085116000000
-14     3      6.984084119000000      6.920827766000000      5.359831742000000
-15     3      8.173327028999999      7.030578234000000      8.109721308999999
-16     3      7.712744148000000      5.888340593000000      7.326419051999999
-17     3      5.324214623000000      3.201517793000000      7.146181371999999
-18     3      6.414082252000000      4.141164759000000      6.898016082000000
-19     3      5.198443457000000      4.558817398000000      3.684266976000000
-20     3      5.664354797000000      5.157098402000000      4.934130940000000
-21     3      3.125091129999999      5.302537924000000      7.287811779000000
-22     3      4.524537393999999      5.547354867000000      6.941418627000000
-23     3      5.266588847000000      8.533464454000001      7.934537965999999
-24     3      5.813582579000000      7.311324169999999      7.343151373999999
-25     4      7.653479861000000      9.102089132000000      4.813431570000000
-26     4      8.245420617000001      7.488356517000000      3.482504260000000
-27     4      8.963288081999998      7.856905290999999      7.612793701999999
-28     4      7.833679201999999      7.100639900000000      9.306496554000001
-29     4      5.028586922000000      2.937370941000000      8.325404693999999
-30     4      4.741201966000000      2.637858094000000      6.200982079999999
-31     4      4.146508121000000      4.963365565000000      3.165169666000000
-32     4      5.902635252000000      3.709767353000000      3.116436362000000
-33     4      2.296169478000000      5.106738242999999      6.383770176999999
-34     4      2.766806075000000      5.348618235000000      8.475749598000000
-35     4      4.048822389000000      8.566315154000000      8.191481980000001
-36     4      5.972326991000000      9.558374161000000      8.023418635000001
-     0.000000000000000      0.000000000000000      0.000000000000000 
-    12.000000000000000      0.000000000000000      0.000000000000000 
-     0.000000000000000     12.000000000000000      0.000000000000000 
-     0.000000000000000      0.000000000000000     12.000000000000000 
+          56 S
+ C H O N 
+     1  3    5.62104    2.12265    8.31118
+     2  3    4.83996    4.55235    2.47468
+     3  3    2.13404    1.21485    3.36182
+     4  3    1.35296    5.46015    9.19832
+     5  3    5.78145    3.38422    6.58357
+     6  3    4.67955    3.29078    0.74707
+     7  3    2.29445   -0.04673    5.08943
+     8  3    1.19255    6.72173   10.92593
+     9  3    1.82021    2.42970    8.55631
+    10  3    8.64079    4.24530    2.71981
+    11  3   -1.66679    0.90780    3.11669
+    12  3    5.15379    5.76720    8.95319
+    13  3    3.60556    2.83020    9.66524
+    14  3    6.85544    3.84480    3.82874
+    15  3    0.11856    0.50730    2.00776
+    16  3    3.36844    6.16770    7.84426
+    17  4    5.11194    2.81018    7.44737
+    18  4    5.34906    3.86483    1.61087
+    19  4    1.62494    0.52733    4.22563
+    20  4    1.86206    6.14768   10.06213
+    21  4    3.02672    2.71005    8.57965
+    22  4    7.43428    3.96495    2.74316
+    23  4   -0.46028    0.62745    3.09335
+    24  4    3.94728    6.04755    8.92984
+    25  1    3.71714    2.92365    7.37734
+    26  1    6.74386    3.75135    1.54084
+    27  1    0.23014    0.41385    4.29566
+    28  1    3.25686    6.26115   10.13216
+    29  1    3.01974    3.26408    6.15167
+    30  1    7.44126    3.41092    0.31517
+    31  1   -0.46726    0.07343    5.52133
+    32  1    3.95426    6.60157   11.35783
+    33  4    3.67530    3.56445    5.06608
+    34  4    6.78570    3.11055   -0.77042
+    35  4    0.18830   -0.22695    6.60692
+    36  4    3.29870    6.90195   12.44342
+    37  4    1.70863    3.27075    6.11665
+    38  4    8.75237    3.40425    0.28015
+    39  4   -1.77837    0.06675    5.55635
+    40  4    5.26537    6.60825   11.39285
+    41  2    5.74366    5.61755   10.93914
+    42  2    5.48131    6.35424   12.48301
+    43  2    3.87389    6.69837   13.32240
+    44  2    2.27137    6.46784   12.54612
+    45  2   -2.39735    0.30272    4.71606
+    46  2   -2.27098   -0.18735    6.48326
+    47  2   -0.43753   -0.46589    7.46677
+    48  2    1.24840   -0.18728    6.46723
+    49  2    1.30120    3.26177    7.05170
+    50  2    1.33151    3.60594    5.11673
+    51  2    4.64672    3.02993    5.01382
+    52  2    3.10414    3.46513    4.21472
+    53  2    5.68882    3.11948   -0.68816
+    54  2    7.41200    2.86795   -1.60336
+    55  2    9.22016    3.14097   -0.67998
+    56  2    9.16810    3.66143    1.19810
+  -2.3973479270935059      -0.46588900685310364       -1.6033619642257690     
+   6.9739999771118164        0.0000000000000000        0.0000000000000000     
+   0.0000000000000000        6.6750001907348633        0.0000000000000000     
+   0.0000000000000000        0.0000000000000000        11.673000335693359
```

### Comparing `irff-1.5.2/irff/structures/diamond.py` & `irff-1.5.3/irff/structures/diamond.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/__init__.py` & `irff-1.5.3/irff/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/eos_opt.py` & `irff-1.5.3/irff/tools/eos_opt.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/ffield_to_json.py` & `irff-1.5.3/irff/tools/ffield_to_json.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/ffieldtolib.py` & `irff-1.5.3/irff/tools/ffieldtolib.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/fingerprint.py` & `irff-1.5.3/irff/tools/fingerprint.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/fit_hugoniot_state.py` & `irff-1.5.3/irff/tools/fit_hugoniot_state.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/fitnn.py` & `irff-1.5.3/irff/tools/fitnn.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/json_to_ffield.py` & `irff-1.5.3/irff/tools/json_to_ffield.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/morse_taper.py` & `irff-1.5.3/irff/tools/morse_taper.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/pre_opt.py` & `irff-1.5.3/irff/tools/pre_opt.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/prepare_ffield.py` & `irff-1.5.3/irff/tools/prepare_ffield.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/pressure.py` & `irff-1.5.3/irff/tools/pressure.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/pseudo_gen.py` & `irff-1.5.3/irff/tools/pseudo_gen.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/rsetff.py` & `irff-1.5.3/irff/tools/rsetff.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/setwb.py` & `irff-1.5.3/irff/tools/setwb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/vdw.py` & `irff-1.5.3/irff/tools/vdw.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/tools/zmat_to_atoms.py` & `irff-1.5.3/irff/tools/zmat_to_atoms.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.2/irff/trainer.py` & `irff-1.5.3/irff/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os.path import isfile # exists
 import argh
 import argparse
 import numpy as np
 from .reax import ReaxFF
 from .reax_nn import ReaxFF_nn
 from .mpnn import MPNN
-from .initCheck import Init_Check
+# from .intCheck import Intelligent_Check 
 from .dingtalk import send_msg
 import json as js
 
 
 # dataset ={'ethw':'/home/gfeng/siesta/train/case1',
 #           'ethw1':'/home/gfeng/siesta/train/case1/run_1'}
 # batch = 50
@@ -34,19 +34,19 @@
           be_universal_nn='all',
           bo_universal_nn='all',
           mf_universal_nn='all',
           vdw_universal_nn='all',
           spv_bo=False,#boc={},#boup={},
           spv_be=False,belo={},beup={},
           spv_vdw=False,vlo={},vup={},
-          spv_ang=False,
+          spv_pi=False,
           bore={'others':0.45},
-          bom={'others':1.20},
+          #bom={'others':1.20},
           weight={'others':10.0},
-          lambda_bd=10000.0,lambda_reg=0.0001,lambda_ang=0.02,
+          lambda_bd=10000.0,lambda_reg=0.0001,
           learning_rate=1.0e-4,
           ffield='ffield.json',**kwargs):
     ''' training the force field '''
     rn = ReaxFF(libfile=ffield,
                 dataset=dataset, 
                 dft='siesta',
                 spec=spec,
@@ -90,20 +90,19 @@
                spec=[],
                writelib=1000,nn=True,vdwnn=True,VdwFunction=1,
                bo_layer=[4,1],mf_layer=[9,2],be_layer=[6,1],vdw_layer=[6,1],
                be_universal_nn='all',bo_universal_nn='all',mf_universal_nn='all',
                vdw_universal_nn='all',
                BOFunction=0,EnergyFunction=3,MessageFunction=2,
                messages=1,mpopt=[1,1,1,1],
-               spv_bo=False,#boc={},#boup={},
+               spv_bo=False,spv_pi=False,
                spv_be=False,belo={},beup={},
                spv_vdw=False,vlo={},vup={},
-               lambda_me=0.1,lambda_ang=0.02,lambda_bd=1000.0,
+               lambda_me=0.1,lambda_bd=1000.0,
                weight={'others':10.0},
-               spv_ang=False,
                lambda_reg=0.0001, # regularize=True,
                learning_rate=1.0e-4,
                ffield = 'ffield.json',**kwargs):
     ''' train the massage passing model '''
     regularize =True if lambda_reg>0.0001 else False
     cons_=['val','vale',
            'ovun1','ovun2','ovun3','ovun4',
@@ -139,17 +138,16 @@
               messages=messages,
               mpopt=mpopt,
               batch_size=batch,
               losFunc='n2',
               regularize_be=regularize,regularize_bo=regularize,regularize_mf=regularize,
               lambda_reg=lambda_reg,lambda_bd=lambda_bd,
               spv_be=spv_be,belo=belo,beup=beup,
-              spv_bo=spv_bo,#boup=boup,
+              spv_bo=spv_bo,spv_pi=spv_pi, 
               spv_vdw=spv_vdw,vlo=vlo,vup=vup,
-              spv_ang=spv_ang,lambda_ang=lambda_ang,
               weight=weight,lambda_me=lambda_me,
               convergence=convergence,
               lossConvergence=lossConvergence) # Loss Functon can be n2,abs,mse,huber
 
     loss,accu,accMax,i,zpe =rn.run(learning_rate=learning_rate,
                                    step=step,
                                    print_step=10,
@@ -186,17 +184,17 @@
                be_universal_nn='all',bo_universal_nn='all',mf_universal_nn='all',
                vdw_universal_nn='all',
                BOFunction=0,EnergyFunction=3,MessageFunction=2,
                messages=1,mpopt=[1,1,1,1],
                spv_bo=False,#boc={},#boup={},
                spv_be=False,belo={},beup={},
                spv_vdw=False,vlo={},vup={},
-               lambda_me=0.1,lambda_ang=0.02,lambda_bd=1000.0,
+               lambda_me=0.1,lambda_bd=1000.0,
                weight={'others':10.0},
-               spv_ang=False,
+               spv_pi=False,
                lambda_reg=0.0001, # regularize=True,
                learning_rate=1.0e-4,
                ffield = 'ffield.json',**kwargs):
     ''' train the massage passing model '''
     regularize =True if lambda_reg>0.0001 else False
     cons_=['val','vale',
            'ovun1','ovun2','ovun3','ovun4',
@@ -232,17 +230,16 @@
               messages=messages,
               mpopt=mpopt,
               batch_size=batch,
               losFunc='n2',
               regularize_be=regularize,regularize_bo=regularize,regularize_mf=regularize,
               lambda_reg=lambda_reg,lambda_bd=lambda_bd,
               spv_be=spv_be,belo=belo,beup=beup,
-              spv_bo=spv_bo,#boup=boup,
+              spv_bo=spv_bo,#spv_pi=spv_pi,
               spv_vdw=spv_vdw,vlo=vlo,vup=vup,
-              spv_ang=spv_ang,lambda_ang=lambda_ang,
               weight=weight,lambda_me=lambda_me,
               convergence=convergence,
               lossConvergence=lossConvergence) # Loss Functon can be n2,abs,mse,huber
 
     loss,accu,accMax,i,zpe =rn.run(learning_rate=learning_rate,
                                    step=step,
                                    print_step=10,
```

### Comparing `irff-1.5.2/irff/zmatrix.py` & `irff-1.5.3/irff/zmatrix.py`

 * *Files identical despite different names*

