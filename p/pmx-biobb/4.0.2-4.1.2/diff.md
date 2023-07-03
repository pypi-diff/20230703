# Comparing `tmp/pmx_biobb-4.0.2.tar.gz` & `tmp/pmx_biobb-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmx_biobb-4.0.2.tar", last modified: Thu Jun 22 15:07:11 2023, max compression
+gzip compressed data, was "dist/pmx_biobb-4.1.2.tar", last modified: Mon Jul  3 12:12:58 2023, max compression
```

## Comparing `pmx_biobb-4.0.2.tar` & `pmx_biobb-4.1.2.tar`

### file list

```diff
@@ -1,243 +1,330 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/
--rw-r--r--   0 pau        (501) staff       (20)     7651 2023-06-14 14:42:12.000000 pmx_biobb-4.0.2/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)       95 2023-06-19 13:37:17.000000 pmx_biobb-4.0.2/MANIFEST.in
--rw-r--r--   0 pau        (501) staff       (20)     2616 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     2087 2023-06-19 13:29:31.000000 pmx_biobb-4.0.2/README.rst
--rw-r--r--   0 pau        (501) staff       (20)      194 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     2154 2023-06-22 15:03:05.000000 pmx_biobb-4.0.2/setup.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/
--rw-r--r--   0 pau        (501) staff       (20)      459 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/_version.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/
--rw-r--r--   0 pau        (501) staff       (20) 17363760 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/bbdep.pkl
--rw-r--r--   0 pau        (501) staff       (20)     1786 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/blosum62_new.mat
--rw-r--r--   0 pau        (501) staff       (20)   144604 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/bp.pkl
--rw-r--r--   0 pau        (501) staff       (20)   149219 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/bp_amber.pkl
--rw-r--r--   0 pau        (501) staff       (20)   148935 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/bp_charmm.pkl
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9416 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    36132 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      951 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/
--rw-r--r--   0 pau        (501) staff       (20)      661 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.am
--rw-r--r--   0 pau        (501) staff       (20)    12694 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.in
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8884 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     3873 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/atommass.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       84 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2060 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1519 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      181 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)     6253 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)      244 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1660 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9612 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    88617 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    47717 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ffnanonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     1208 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2882 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     1767 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)        0 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/lipids.hdb
--rw-r--r--   0 pau        (501) staff       (20)    48593 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/lipids.rtp
--rw-r--r--   0 pau        (501) staff       (20)       70 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/mutres.arn
--rw-r--r--   0 pau        (501) staff       (20)      164 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1884 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      126 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)     9712 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      910 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      916 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1369 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1419 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1576 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     2237 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)      306 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm36mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       92 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     3940 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/elements.dat
--rw-r--r--   0 pau        (501) staff       (20)    29266 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/spc216.gro
--rw-r--r--   0 pau        (501) staff       (20)      343 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/specbond.dat
--rw-r--r--   0 pau        (501) staff       (20)      447 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45/xlateat.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    21524 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2589 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     5335 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)    36132 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      130 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)    45478 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7972 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      974 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129919 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)     2589 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4978 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)    36132 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)     7476 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      974 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129937 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    82367 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/cmap.itp
--rw-r--r--   0 pau        (501) staff       (20)      435 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2734 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     2079 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)       92 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.arn
--rw-r--r--   0 pau        (501) staff       (20)     1134 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8979 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1397 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      198 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.r2b
--rw-r--r--   0 pau        (501) staff       (20)  1133668 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5220 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.vsd
--rw-r--r--   0 pau        (501) staff       (20)   283035 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   123173 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)     1339 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/nbfix.itp
--rw-r--r--   0 pau        (501) staff       (20)      619 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      625 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1026 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1242 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)      221 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)    70529 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/data/rna.pkl
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/extensions/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/
--rw-r--r--   0 pau        (501) staff       (20)    13896 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/Energy.c
--rw-r--r--   0 pau        (501) staff       (20)    15145 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/Geometry.c
--rw-r--r--   0 pau        (501) staff       (20)    20514 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/Geometry.h
--rw-r--r--   0 pau        (501) staff       (20)     2086 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/cpp_test.cpp
--rw-r--r--   0 pau        (501) staff       (20)     3939 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/init.c
--rw-r--r--   0 pau        (501) staff       (20)     4662 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/pmx.h
--rw-r--r--   0 pau        (501) staff       (20)    17556 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/pmx/wrap_Geometry.c
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/
--rw-r--r--   0 pau        (501) staff       (20)     8847 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/trr2xtc.c
--rw-r--r--   0 pau        (501) staff       (20)    64408 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile.c
--rw-r--r--   0 pau        (501) staff       (20)    23730 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile.h
--rw-r--r--   0 pau        (501) staff       (20)    13474 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_c_test.c
--rw-r--r--   0 pau        (501) staff       (20)    14744 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_trr.c
--rw-r--r--   0 pau        (501) staff       (20)     2364 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_trr.h
--rw-r--r--   0 pau        (501) staff       (20)     3629 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_xtc.c
--rw-r--r--   0 pau        (501) staff       (20)     2255 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_xtc.h
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/scripts/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/
--rwxr-xr-x   0 pau        (501) staff       (20)    68373 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/atoms_to_morph.py
--rwxr-xr-x   0 pau        (501) staff       (20)    79997 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/atoms_to_morph_rdkit2018.py
--rwxr-xr-x   0 pau        (501) staff       (20)    22630 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/build_mst_graph.py
--rwxr-xr-x   0 pau        (501) staff       (20)    50443 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/make_hybrid.py
--rwxr-xr-x   0 pau        (501) staff       (20)     2495 2023-06-19 14:09:16.000000 pmx_biobb-4.0.2/src/pmx/scripts/ligands/one_ff_file.py
--rw-r--r--   0 pau        (501) staff       (20)    19712 2023-06-19 13:29:35.000000 pmx_biobb-4.0.2/src/pmx/scripts/md_setup.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     2616 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)    11807 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)       53 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-06-19 14:00:41.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/not-zip-safe
--rw-r--r--   0 pau        (501) staff       (20)       29 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)        4 2023-06-22 15:07:11.000000 pmx_biobb-4.0.2/src/pmx_biobb.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)    65963 2023-06-22 15:03:05.000000 pmx_biobb-4.0.2/versioneer.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/
+-rw-rw-r--   0 pau        (501) staff       (20)     7651 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/LICENSE
+-rw-rw-r--   0 pau        (501) staff       (20)       95 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/MANIFEST.in
+-rw-r--r--   0 pau        (501) staff       (20)     2616 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/PKG-INFO
+-rw-rw-r--   0 pau        (501) staff       (20)     2087 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/README.rst
+-rw-rw-r--   0 pau        (501) staff       (20)      194 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/setup.cfg
+-rw-rw-r--   0 pau        (501) staff       (20)     2125 2023-07-03 12:09:10.000000 pmx_biobb-4.1.2/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/
+-rwxr-xr-x   0 pau        (501) staff       (20)    31247 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/AbsRestraints.py
+-rw-rw-r--   0 pau        (501) staff       (20)     2261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)      439 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/_version.py
+-rw-rw-r--   0 pau        (501) staff       (20)    81006 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/alchemy.py
+-rw-rw-r--   0 pau        (501) staff       (20)    14501 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/analysis.py
+-rw-rw-r--   0 pau        (501) staff       (20)    15992 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/atom.py
+-rw-rw-r--   0 pau        (501) staff       (20)    14221 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/atomselection.py
+-rw-rw-r--   0 pau        (501) staff       (20)    13429 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/builder.py
+-rw-rw-r--   0 pau        (501) staff       (20)    34519 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/chain.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/
+-rw-rw-r--   0 pau        (501) staff       (20)   233765 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/aminoacids.pkl
+-rw-rw-r--   0 pau        (501) staff       (20) 17363760 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/bbdep.pkl
+-rw-rw-r--   0 pau        (501) staff       (20)     1786 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/blosum62_new.mat
+-rw-rw-r--   0 pau        (501) staff       (20)   144604 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/bp.pkl
+-rw-rw-r--   0 pau        (501) staff       (20)   149219 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/bp_amber.pkl
+-rw-rw-r--   0 pau        (501) staff       (20)   148935 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/bp_charmm.pkl
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)      661 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am
+-rw-rw-r--   0 pau        (501) staff       (20)    12694 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in
+-rw-rw-r--   0 pau        (501) staff       (20)     9997 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     8884 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      849 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    80500 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)     5339 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    66560 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     8192 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)       79 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      947 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1948 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     3882 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  3071584 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1260735 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/urea.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)    21524 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     2589 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     9412 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      903 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)   101863 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)     5335 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)    36227 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  1202088 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
+-rw-rw-r--   0 pau        (501) staff       (20)    36132 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      130 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    10830 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    45478 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     7972 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      722 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      974 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1949 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     3886 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  2805564 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1181333 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)   300774 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)   129919 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    16346 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    18595 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)     2589 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     9412 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      903 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)   101863 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)     4978 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)    36227 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  1202088 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres
+-rw-rw-r--   0 pau        (501) staff       (20)    36132 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    10830 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    36132 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     7476 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      709 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      974 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1949 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     3886 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  2805564 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1181333 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)   300774 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)   129937 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    16346 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    18595 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)     9997 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     9416 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      903 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)   104467 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)     4652 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    36127 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     6772 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      704 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      951 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1948 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     3886 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  3290968 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1389335 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/watermodels.dat
+-rw-rw-r--   0 pau        (501) staff       (20)     3873 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/atommass.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)       84 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     2060 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     8026 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)     1519 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      181 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    44420 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     6253 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)    13027 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)    37937 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      244 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)      261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     1660 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      265 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     9612 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    88617 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    74128 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    47717 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)   144554 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2792 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)     1208 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2882 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1767 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)        0 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/lipids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)    48593 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)       70 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.arn
+-rw-rw-r--   0 pau        (501) staff       (20)  2828420 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1165390 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      164 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)      261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     1884 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      265 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      126 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)     9712 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      910 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      916 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1369 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1419 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1576 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2237 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      915 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      306 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)    24002 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)    82367 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  1123865 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  1614095 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     7941 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      435 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2734 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2079 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)       92 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     1134 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     8979 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)     1397 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      198 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)  1133668 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5220 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)       92 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.arn
+-rw-rw-r--   0 pau        (501) staff       (20)  3015999 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1267062 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)   283035 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)   123173 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     1339 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      619 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      625 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1026 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1242 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      221 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/watermodels.dat
+-rw-rw-r--   0 pau        (501) staff       (20)     3940 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/elements.dat
+-rw-rw-r--   0 pau        (501) staff       (20)    10624 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/residuetypes.dat
+-rw-rw-r--   0 pau        (501) staff       (20)    29266 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/spc216.gro
+-rw-rw-r--   0 pau        (501) staff       (20)      343 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/specbond.dat
+-rw-rw-r--   0 pau        (501) staff       (20)      848 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/vdwradii.dat
+-rw-rw-r--   0 pau        (501) staff       (20)      447 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/xlateat.dat
+-rw-rw-r--   0 pau        (501) staff       (20)    70529 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/rna.pkl
+-rw-rw-r--   0 pau        (501) staff       (20)    37772 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/estimators.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/extensions/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/
+-rw-rw-r--   0 pau        (501) staff       (20)    13896 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/Energy.c
+-rw-rw-r--   0 pau        (501) staff       (20)    15145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/Geometry.c
+-rw-rw-r--   0 pau        (501) staff       (20)    20514 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/Geometry.h
+-rw-rw-r--   0 pau        (501) staff       (20)     2086 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/cpp_test.cpp
+-rw-rw-r--   0 pau        (501) staff       (20)     3939 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/init.c
+-rw-rw-r--   0 pau        (501) staff       (20)     4662 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/pmx.h
+-rw-rw-r--   0 pau        (501) staff       (20)    17556 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/wrap_Geometry.c
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/
+-rw-rw-r--   0 pau        (501) staff       (20)     8847 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/trr2xtc.c
+-rw-rw-r--   0 pau        (501) staff       (20)    64408 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile.c
+-rw-rw-r--   0 pau        (501) staff       (20)    23730 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile.h
+-rw-rw-r--   0 pau        (501) staff       (20)    13474 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_c_test.c
+-rw-rw-r--   0 pau        (501) staff       (20)    14744 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_trr.c
+-rw-rw-r--   0 pau        (501) staff       (20)     2364 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_trr.h
+-rw-rw-r--   0 pau        (501) staff       (20)     3629 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_xtc.c
+-rw-rw-r--   0 pau        (501) staff       (20)     2255 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_xtc.h
+-rw-rw-r--   0 pau        (501) staff       (20)    29075 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/ffparser.py
+-rw-rw-r--   0 pau        (501) staff       (20)    97591 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/forcefield.py
+-rw-rw-r--   0 pau        (501) staff       (20)     7685 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/geometry.py
+-rw-rw-r--   0 pau        (501) staff       (20)     8707 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/gmx.py
+-rw-rw-r--   0 pau        (501) staff       (20)     6179 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/jobscript.py
+-rw-rw-r--   0 pau        (501) staff       (20)   123096 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/library.py
+-rw-rw-r--   0 pau        (501) staff       (20)   117960 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/ligand_alchemy.py
+-rw-rw-r--   0 pau        (501) staff       (20)    46805 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/model.py
+-rw-rw-r--   0 pau        (501) staff       (20)    28167 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/molecule.py
+-rw-rw-r--   0 pau        (501) staff       (20)     7345 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/mutdb.py
+-rw-rw-r--   0 pau        (501) staff       (20)     8874 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/ndx.py
+-rw-rw-r--   0 pau        (501) staff       (20)    16599 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/options.py
+-rw-rw-r--   0 pau        (501) staff       (20)     5036 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/parser.py
+-rw-rw-r--   0 pau        (501) staff       (20)    21628 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/rosetta.py
+-rw-rw-r--   0 pau        (501) staff       (20)    15211 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/rosetta_analyze.py
+-rw-rw-r--   0 pau        (501) staff       (20)    11783 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/rotamer.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/scripts/
+-rw-rw-r--   0 pau        (501) staff       (20)        0 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    33900 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/analyze_dhdl.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    19864 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/atomMapping.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    11939 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/build_cyclic_top.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2988 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/cli.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2955 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/gen_abs_restraints.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    73999 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/generate_hybrid_residue.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     7099 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/generate_hybrid_topology.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/scripts/icolos_entrypoints/
+-rw-rw-r--   0 pau        (501) staff       (20)        0 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/icolos_entrypoints/__init__.py
+-rw-rw-r--   0 pau        (501) staff       (20)     7137 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/icolos_entrypoints/assemble_systems.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    12867 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/ligandHybrid.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2705 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/make_double_box.py
+-rw-rw-r--   0 pau        (501) staff       (20)    19943 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/md_setup.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    23072 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/mutate.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    38647 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/parameterize_ligands.py
+-rw-rw-r--   0 pau        (501) staff       (20)     7795 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/prepare_crooks_runs.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     1475 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/set_gmxlib.py
+-rw-rw-r--   0 pau        (501) staff       (20)    17636 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/setup_abfe.py
+-rw-rw-r--   0 pau        (501) staff       (20)    13784 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/summary.py
+-rw-rw-r--   0 pau        (501) staff       (20)    15258 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/utils.py
+-rw-rw-r--   0 pau        (501) staff       (20)    11331 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/xdrfile.py
+-rw-rw-r--   0 pau        (501) staff       (20)     1784 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/xtc.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     2722 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)    14322 2023-07-03 11:43:22.000000 pmx_biobb-4.1.2/src/pmx.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)       53 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/not-zip-safe
+-rw-r--r--   0 pau        (501) staff       (20)       29 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)        4 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/top_level.txt
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     2616 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)    14582 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)       53 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 11:49:27.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/not-zip-safe
+-rw-r--r--   0 pau        (501) staff       (20)       29 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)        4 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/top_level.txt
+-rw-rw-r--   0 pau        (501) staff       (20)    66226 2023-07-03 12:08:52.000000 pmx_biobb-4.1.2/versioneer.py
```

### Comparing `pmx_biobb-4.0.2/LICENSE` & `pmx_biobb-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/PKG-INFO` & `pmx_biobb-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmx_biobb
-Version: 4.0.2
+Version: 4.1.2
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger, Vytautas Gapsys
 Author-email: d.seeliger@gmx.net, vytautas.gapsys@gmail.com
 License: LGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pmx_biobb-4.0.2/README.rst` & `pmx_biobb-4.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/setup.py` & `pmx_biobb-4.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                   )
 extensions = [pmx, xdrio]
 
 # -----
 # Setup
 # -----
 setup(name='pmx_biobb',
-      version='4.0.2',
+      version=versioneer.get_version(),
       cmdclass=versioneer.get_cmdclass(),
       description='Toolkit for free-energy calculation setup/analysis '
                   'and biomolecular structure handling',
       long_description=readme(),
       classifiers=[
         'Programming Language :: Python',
         'Intended Audience :: Science/Research',
@@ -58,13 +58,9 @@
       package_dir={'': 'src'},
       include_package_data=True,
       zip_safe=False,
       ext_modules=extensions,
       tests_require=['pytest'],
       install_requires=['numpy', 'scipy', 'matplotlib', 'rdkit'],
       python_requires=">=3.7",
-      entry_points={
-          "console_scripts": [
-              "pmx = pmx.scripts.cli:entry_point"
-          ]
-        },
+      entry_points={'console_scripts': ['pmx = pmx.scripts.cli:entry_point']},
       )
```

### Comparing `pmx_biobb-4.0.2/src/pmx/data/bbdep.pkl` & `pmx_biobb-4.1.2/src/pmx/data/bbdep.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/blosum62_new.mat` & `pmx_biobb-4.1.2/src/pmx/data/blosum62_new.mat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/bp.pkl` & `pmx_biobb-4.1.2/src/pmx/data/bp.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/bp_amber.pkl` & `pmx_biobb-4.1.2/src/pmx/data/bp_amber.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/bp_charmm.pkl` & `pmx_biobb-4.1.2/src/pmx/data/bp_charmm.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.r2b` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.vsd` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/backup_mutres` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ffbonded.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/forcefield.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/gbsa.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ions.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.mtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spc.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spce.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip3p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4pew.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip5p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/urea.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.am` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.in` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.vsd` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/dna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/gbsa.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/rna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/spc.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/spce.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip3p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip4p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip4pew.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/tip5p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/amber99sbmut.ff/urea.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/atommass.dat` & `pmx_biobb-4.1.2/src/pmx/data/mutff/atommass.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.c.tdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.n.tdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.vsd` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/dna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ffbonded.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ffnanonbonded.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/forcefield.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/gb.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/ions.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/lipids.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/rna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/spc.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/spce.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip3p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip4p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip4pew.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/charmm22starmut.ff/tip5p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/elements.dat` & `pmx_biobb-4.1.2/src/pmx/data/mutff/elements.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45/spc216.gro` & `pmx_biobb-4.1.2/src/pmx/data/mutff/spc216.gro`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ions.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spc.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spce.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/urea.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.arn` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.r2b` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.vsd` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/atomtypes.atp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/correct_ffbonded.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffberger.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffnonbonded.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/forcefield.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/gbsa.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ions.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.mtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spc.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spce.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip3p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4pew.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip5p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/urea.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/cmap.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/gb.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/ions.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.c.tdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.hdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.n.tdb` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.vsd` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.mtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.rtp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/nbfix.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/spc.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/spce.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip3p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip4p.itp` & `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/data/rna.pkl` & `pmx_biobb-4.1.2/src/pmx/data/rna.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/pmx/Energy.c` & `pmx_biobb-4.1.2/src/pmx/extensions/pmx/Energy.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/pmx/Geometry.c` & `pmx_biobb-4.1.2/src/pmx/extensions/pmx/Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/pmx/Geometry.h` & `pmx_biobb-4.1.2/src/pmx/extensions/pmx/Geometry.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/pmx/cpp_test.cpp` & `pmx_biobb-4.1.2/src/pmx/extensions/pmx/cpp_test.cpp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/pmx/init.c` & `pmx_biobb-4.1.2/src/pmx/extensions/pmx/init.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/pmx/pmx.h` & `pmx_biobb-4.1.2/src/pmx/extensions/pmx/pmx.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/pmx/wrap_Geometry.c` & `pmx_biobb-4.1.2/src/pmx/extensions/pmx/wrap_Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/xdr/trr2xtc.c` & `pmx_biobb-4.1.2/src/pmx/extensions/xdr/trr2xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile.c` & `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile.h` & `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_c_test.c` & `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_c_test.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_trr.c` & `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_trr.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_trr.h` & `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_trr.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_xtc.c` & `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/extensions/xdr/xdrfile_xtc.h` & `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_xtc.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.0.2/src/pmx/scripts/ligands/make_hybrid.py` & `pmx_biobb-4.1.2/src/pmx/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1308 +1,1305 @@
-import sys, os
-from pmx import *
-from pmx.parser import *
-from pmx.forcefield2 import *
-from pmx.ndx import *
-import copy as xcopy
-
-def check_if_vsite2_exists( vsites, xs):
-    for v in vsites:
-        if v[0].id==xs[0].id and v[1].id==xs[1].id and v[2].id==xs[2].id and v[3]==xs[3] and v[4]==xs[4]:
-            return(True)
-        elif v[0].id==xs[0].id and v[1].id==xs[1].id and v[2].id==xs[2].id:
-            print("ERROR: it seems that vsites are to be morphed. Gromacs does not support that")
-            sys.exit(0)
-    return(False)
-
-def check_if_vsite3_exists( vsites, xs):
-    for v in vsites:
-        if v[0].id==xs[0].id and v[1].id==xs[1].id and v[2].id==xs[2].id and v[3].id==xs[3].id and v[4]==xs[4] and v[5]==xs[5]:
-            return(True)
-        elif v[0].id==xs[0].id and v[1].id==xs[1].id and v[2].id==xs[2].id and v[3].id==xs[3].id:
-            print("ERROR: it seems that vsites are to be morphed. Gromacs does not support that")
-            sys.exit(0)
-    return(False)
-
-def check_if_exclusion_valid( exclusions, ex ):
-    # return True, if all fine and ex can be added
-
-    # check if the first atom is dummy. If so, all fine
-    a0 = ex[0]
-    if ('DUM' in a0.atomtype) or ('DUM' in a0.atomtypeB):
-        return(True)
-
-    # check if an exclusion already exists
-    for excl in exclusions:
-        if excl[0]==ex[0]: # some interactions for this atom are already excluded
-            if len(excl)!=len(ex): # the exclusion lists are of different length
-                print('ERROR: Something wrong with exclusions: ',excl,ex)
-                sys.exit(1)
+#!/usr/bin/env python
+
+# pmx  Copyright Notice
+# ============================
+#
+# The pmx source code is copyrighted, but you can freely use and
+# copy it as long as you don't change or remove any of the copyright
+# notices.
+#
+# ----------------------------------------------------------------------
+# pmx is Copyright (C) 2006-2013 by Daniel Seeliger
+#
+#                        All Rights Reserved
+#
+# Permission to use, copy, modify, distribute, and distribute modified
+# versions of this software and its documentation for any purpose and
+# without fee is hereby granted, provided that the above copyright
+# notice appear in all copies and that both the copyright notice and
+# this permission notice appear in supporting documentation, and that
+# the name of Daniel Seeliger not be used in advertising or publicity
+# pertaining to distribution of the software without specific, written
+# prior permission.
+#
+# DANIEL SEELIGER DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS
+# SOFTWARE, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS.  IN NO EVENT SHALL DANIEL SEELIGER BE LIABLE FOR ANY
+# SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
+# RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF
+# CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN
+# CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+# ----------------------------------------------------------------------
+
+"""This module contains the Model class. It can use
+GROMACS routines to read and write structure files. Moreover it
+allows to modify structure files in various ways. E.g.:
+
+1. Rename atoms, residues, chains
+2. Delete or add atoms, residues and chains
+
+By default, all residues are renumbered from 1. This option can be deactivated
+by setting renumber_residues to False.
+
+The Model instance contains:
+
+* model.atoms       -> list of atoms
+* model.residues    -> list of residues
+* model.chains      -> list of chains
+* model.chdic       -> chain dictionary (chdic['A'] returns chain A)
+
+Examples
+--------
+Basic usage:
+
+    >>> model = Model('input.pdb')
+
+Some useful methods:
+
+    >>> # returns all backbone atoms
+    >>> model.fetch_atoms(['CA','N','C'])
+    >>> # returns all carbon atoms
+    >>> model.fetch_atoms('C',how='byelem')
+    >>> # return all atoms except hydrogens
+    >>> model.fetch_atoms('H',how='byelem',inv=True)
+
+    >>> # return all ALA,TRP and CYS residues
+    >>> model.fetch_residues(['ALA','TRP','CYS'])
+
+    >>> # returns the first 10 residues
+    >>> rl = model.residues[:10]
+    >>> # return the last residue from chain A
+    >>> rl = model.chdic['A'].residues[-1]
+    >>> # returns a list with the first residues of each chain
+    >>> rl = map(lamda m: m.residues[0], model.chains)
+    >>> # remove chain A
+    >>> del model['A']
+    >>> # write new structure file
+    >>> model.write('output.pdb')
+
+"""
+
+import sys
+import copy
+import numpy as np
+from . import _pmx as _p
+from . import library
+from . import chain
+from .atomselection import Atomselection
+from .molecule import Molecule
+from .atom import Atom
+from string import digits
+
+
+__all__ = ['Model']
+
+
+class Model(Atomselection):
+    """Model Class.
+
+    Parameters
+    ----------
+    filename : str
+        filename of input structure
+    pdbline : bool(?)
+        what is pdbline?
+    renumber_atoms : bool, optional
+        renumber all atoms from 1. Default is True.
+    renumber_residues : bool, optional
+        renumber all residues from 1. In this way, each residue will have a
+        unique ID, also across chains. Default is True.
+    rename_atoms : bool, optional
+        rename atoms so to conform to Gromacs format. Default is False.
+    scale_coords : A|nm, optional
+        whether to enforce the units of the coordinates to be in A or in nm.
+        By default, PDB coordinates are assumed to be in Angstrom (A) and
+        GRO coordinates in nanometers (nm). If you read a PDB file but would
+        like operate on nm coordinates, then select "nm". Viceversa, if you
+        read a GRO file but would like to work on A coordinates, select "A".
+        Note that if you read a PDB file in A coordinates and select "A",
+        nothing happens (same for GRO and "nm" selection).
+    bPDBTER : bool
+        whether to recognize TER lines and other chain breaks, e.g.
+        discontinuous residue indices(?). Default is True.
+    bNoNewID : bool
+        whether to assign new chain IDs? If True, new chain IDs starting
+        with 'pmx' will be assigned(?). Only relevant if bPDBTER is True.
+        Default is True.
+    bPDBGAP : bool
+        whether search for gaps in the chain to assign new chain IDs.
+    bPDBMASS : bool
+        whether to guess masses from the atom library (will fail for
+        complex atom naming, e.g. ND will not be interpreted as nitrogen)
+
+    Attributes
+    ----------
+    title : str
+        title of model. Default is 'PMX MODEL'.
+    filename : str
+        filename from which the Model was imported, otherwise None.
+    chains : list
+        list of Chain instances
+    chdic : dict
+        dict with chain IDs as keys and Chain instances as values
+    residues : list
+        list of molecules/residues
+    unity : str
+        coordinates unit, either 'A' or 'nm'.
+    box : 2d array
+        3x3 array containing the box vectors. See Gromacs manual, Table 3.1
+    moltype : str
+        Type of system: protein, dna, rna, or unknown if organic molecule or
+        a mix of molecules are in the system.
+    """
+    def __init__(self, filename=None, pdbline=None, renumber_atoms=True,
+                 renumber_residues=True, rename_atoms=False, scale_coords=None,
+                 bPDBTER=True, bNoNewID=True, bPDBGAP=False, bPDBMASS=False,
+                 **kwargs):
+
+        Atomselection.__init__(self)
+        self.title = 'PMX MODEL'
+        self.filename = filename
+        self.chains = []
+        self.chdic = {}
+        self.residues = []
+        self.name = None  # FIXME/QUESTION: self.name not used anywhere? remove?
+        self.id = 0
+        self.have_bonds = 0  # FIXME/QUESTION: same as above: never used -> remove?
+        self.box = [[0, 0, 0], [0, 0, 0], [0, 0, 0]]
+        self.unity = 'A'
+        for key, val in kwargs.items():
+            setattr(self, key, val)
+
+        if filename is not None:
+            self.read(filename=filename, bPDBTER=bPDBTER, bNoNewID=bNoNewID, bPDBGAP=bPDBGAP, bPDBMASS=bPDBMASS)
+        if pdbline is not None:
+            self.__readPDB(pdbline=pdbline)
+        if self.atoms:
+            self.unity = self.atoms[0].unity
+            self.make_chains()
+            self.make_residues()
+        if self.residues and not self.atoms:
+            self.al_from_resl()
+            self.make_chains()
+            self.make_residues()
+        if self.chains and not self.residues:
+            self.resl_from_chains()
+            self.al_from_resl()
+            self.make_chains()
+            self.make_residues()
+        if self.chdic and not self.chains:
+            for key, val in self.chdic.items():
+                self.chains.append(val)
+            if not self.atoms and not self.residues:
+                self.resl_from_chains()
+                self.al_from_resl()
+        if renumber_atoms is True:
+            self.renumber_atoms()
+        if renumber_residues is True:
+            self.renumber_residues()
+        if rename_atoms is True:
+            self.rename_atoms_to_gmx()
+        if scale_coords is not None:
+            if scale_coords == 'A':
+                self.nm2a()
+            elif scale_coords == 'nm':
+                self.a2nm()
             else:
-                for e in excl[1:]:
-                    if e not in ex:
-                        print('ERROR: Something wrong with exclusions: ',excl,ex)
-                        sys.exit(1)
-    return(True)
-
-
-def identify_ring_atoms( fname, num ):
-    import rdkit
-    from rdkit import Chem
-    pdbName,atomNameDict = reformatPDB(fname,num)
-    mol = Chem.MolFromPDBFile(pdbName,removeHs=False,sanitize=False)
-    os.remove(pdbName)
-    out = []
-    for a in mol.GetAtoms():
-        if a.IsInRing()==True:
-            out.append(a.GetIdx()+1)
-    return(out)
-
-def __atoms_morphe( atoms ):
-    for atom in atoms:
-        if atom.atomtypeB is not None and (atom.q!=atom.qB or atom.m != atom.mB): return True
-    return False
-
-def sum_charge_of_states( itp ):
-    qA = 0.0
-    qB = 0.0
-    for a in itp.atoms:
-        qA += a.q
-        if __atoms_morphe([a]):
-            qB+=a.qB
+                raise ValueError('unknown unit %s for coordinates' % scale_coords)
+
+        self.assign_moltype()
+
+
+
+    def __str__(self):
+        s = '< Model: moltype=%s, nchain=%d, nres=%d, natom=%d >' %\
+            (self.moltype, len(self.chains), len(self.residues),
+             len(self.atoms))
+        return s
+
+    def writePIR(self, filename, title=""):
+        """Prints sequence to screen in PIR format"""
+        fp = open(filename, "w")
+        if not title:
+            title = '_'.join(self.title.split())
+        print('>P1;%s' % title, file=fp)
+        print('sequence:::::::::', file=fp)
+        for i in range(len(self.chains) - 1):
+            print('%s/' % self.chains[i].get_sequence(), file=fp)
+        print('%s*' % self.chains[-1].get_sequence(), file=fp)
+        fp.close()
+
+    def writeFASTA(self, filename, title=""):
+        """Prints sequence to screen in FASTA format"""
+        fp = open(filename, "w")
+        if not title:
+            title = '_'.join(self.title.split())
+        if len(self.chains) == 1:
+            print('> %s' % title, file=fp)
+            print(self.chains[0].get_sequence(), file=fp)
+        else:
+            for chain in self.chains:
+                print('> %s_chain_%s' % (title, chain.id), file=fp)
+                print(chain.get_sequence(), file=fp)
+
+    # FIXME/TODO: this function is overwriting the write function inherited from
+    # Atomselection. Should we keep only one of the 2?
+    # writePIR and writeFASTA could be moved to Atomselection so that all
+    # write functions are in one place
+    def write(self, fn, title='', nr=1, bPDBTER=False, bAssignChainIDs=False):
+        """Writes Model to file. The format is deduced from the filename
+        extension given, and available options are '.gro', '.pdb', '.fasta',
+        '.pir'.
+
+        Parameters
+        ----------
+        fn : str
+            filename
+        title : str, optional
+            title of the Model to write in fn
+        nr : int, optional
+            what is nr?
+        bPDBTER : bool, optional
+            whether to separate chains with TER entries. Only relevant when
+            writing PDB files. Default is False.
+        bAssignChainIDs : bool, optional
+            whether to write the chains IDs to file. Only relevant when
+            writing PDB files. Default is False.
+        """
+        ext = fn.split('.')[-1]
+        if ext == 'pdb':
+            self.writePDB(fn, title, nr, bPDBTER, bAssignChainIDs)
+        elif ext == 'gro':
+            self.writeGRO(fn, title)
+        elif ext == 'pir':
+            self.writePIR(fn, title)
+        elif ext == 'fasta':
+            self.writeFASTA(fn, title)
         else:
-            qB+=a.q
-    return [qA], [qB]
+            print('pmx_Error_> Can only write pdb or gro!', file=sys.stderr)
+            sys.exit(1)
 
-def findIDinList(ind,decoupAngles):
-    for i in decoupAngles:
-	if( i==ind ):
-	    return True
-    return False
-
-def adjustCoords(m,mol):
-    conf = mol.GetConformer()
-    for ai in m.atoms:
-	ind = ai.id
-#	print ai.x[0]
-	posj = conf.GetAtomPosition(ind-1)
-	ai.x[0] = posj.x
-	ai.x[1] = posj.y
-        ai.x[2] = posj.z
-
-def reformatPDB(filename,num,bStrict=False):
-#    newname = filename.split(".")[0]+"_tempFormat.pdb"
-    newname = "tempFormat"+str(num)+".pdb"
-    m = Model().read(filename)
-
-    # adjust atom names and remember the changes
-    atomNameDict = {}
-    sigmaHoleCounter = 1
-    for a in m.atoms:
-        newAtomName = a.name
-        if 'EP' in a.name:
-            newAtomName = 'HSH'+str(sigmaHoleCounter)
-            sigmaHoleCounter+=1
-        atomNameDict[newAtomName] = a.name
-        a.name = newAtomName
-
-    writeFormatPDB(newname,m,bStrict=bStrict)
-#    m.write(newname)
-    return(newname,atomNameDict)
-
-def restoreAtomNames(mol,atomNameDict):
-    for atom in mol.GetAtoms():
-        newname = atom.GetMonomerInfo().GetName()
-        if newname in atomNameDict.keys():
-            oldname = atomNameDict[newname]
-            atom.GetMonomerInfo().SetName(oldname)
-
-def writeFormatPDB(fname,m,title="",nr=1,bStrict=False):
-    atNameLen = 4
-    if bStrict:
-        atNameLen = 3
-    fp = open(fname,'w')
-    for atom in m.atoms:
-        foo = xcopy.deepcopy(atom)
-        # chlorine
-        if( 'CL' in atom.name or 'Cl' in atom.name or 'cl' in atom.name ):
-            foo.name = "CL"+"  "
-            print >>fp, foo
-        # bromine
-        elif( 'BR' in atom.name or 'Br' in atom.name or 'br' in atom.name ):
-            foo.name = "BR"+"  "
-            print >>fp, foo
-        elif( len(atom.name) > atNameLen): # too long atom name
-            foo = xcopy.deepcopy(atom)
-            foo.name = foo.name[:atNameLen]
-            print >>fp, foo
+    def make_chains(self):
+        """Initialises the Chain instances from the input"""
+        self.chains = []
+        self.chdic = {}
+        cur_chain = None
+        ch = None
+        for atom in self.atoms:
+            if atom.chain_id == cur_chain:
+                if ch:
+                    atom.chain = ch
+                    ch.atoms.append(atom)
+                else:
+                    ch = chain.Chain()
+                    cur_chain = atom.chain_id
+                    ch.id = atom.chain_id
+                    atom.chain = ch
+                    ch.atoms.append(atom)
+            else:
+                if ch:
+                    self.chains.append(ch)
+                    ch = chain.Chain()
+                    cur_chain = atom.chain_id
+                    ch.id = cur_chain
+                    atom.chain = ch
+                    ch.atoms.append(atom)
+                else:
+                    ch = chain.Chain()
+                    cur_chain = atom.chain_id
+                    ch.id = atom.chain_id
+                    atom.chain = ch
+                    ch.atoms.append(atom)
+
+        self.chains.append(ch)
+        for ch in self.chains:
+            ch.model = self
+            idx = ch.id
+            self.chdic[idx] = ch
+
+    def make_residues(self):
+        """Initialises the Molecule instances from the input"""
+        self.residues = []
+        for ch in self.chains:
+            cur_mol = None
+            mol = None
+            for atom in ch.atoms:
+                if atom.resnr == cur_mol:
+                    if mol:
+                        mol.atoms.append(atom)
+                    else:
+                        mol = Molecule()
+                        cur_mol = atom.resnr
+                        mol.resname = atom.resname
+                        mol.id = cur_mol
+                        mol.atoms.append(atom)
+                else:
+                    if mol:
+                        mol.model = self
+                        mol.chain = ch
+                        ch.residues.append(mol)
+                        self.residues.append(mol)
+                        mol = Molecule()
+                        cur_mol = atom.resnr
+                        mol.resname = atom.resname
+                        mol.id = cur_mol
+                        mol.atoms.append(atom)
+                    else:
+                        mol = Molecule()
+                        cur_mol = atom.resnr
+                        mol.resname = atom.resname
+                        mol.id = cur_mol
+                        mol.atoms.append(atom)
+            self.residues.append(mol)
+            ch.residues.append(mol)
+        for r in self.residues:
+            r.assign_moltype()
+            for atom in r.atoms:
+                atom.molecule = r
+                atom.model = self
+                r.model = self
+        for ch in self.chains:
+            for r in ch.residues:
+                r.chain = ch
+                r.chain_id = ch.id
+
+    def __readPDB(self, fname=None, pdbline=None):
+        """Reads a PDB file"""
+        if pdbline:
+            lines = pdbline.split('\n')
         else:
-            print >>fp, atom
-    print >>fp, 'ENDMDL'
-    fp.close()
-
-
-def do_log(fp, s):
-    l = "make_hybrid__log_> "+s
-    print >>sys.stderr, l
-    print >>fp, l
-
-
-def make_pairs(m1, m2, m3, m4, bFit, bDist, dd, plist = None, grps = None):
-
-    pairs = []
-    if plist:
-        for n1, n2 in plist:
-            a1 = m1.fetch_atoms(n1,how='byid')[0]
-	    #print a1
-            a2 = m2.fetch_atoms(n2,how='byid')[0]
-            pairs.append( (a1, a2))
-            for atom3 in m3.atoms:
-                if a1.id == atom3.id:
-                    atom3.x = a2.x
-		    if(bFit==True):
-            		a4 = m4.fetch_atoms(n2,how='byid')[0]
-			atom3.x = a4.x
-        return pairs
-    if(grps and bDist):
-        lst1 = m1.get_by_id(grps[0])
-        lst2 = m2.get_by_id(grps[1])
-        for atom in lst1:
-            mi = dd # nm
-            keep = None
-            for at in lst2:
-                d = (atom-at)/10.0
-                if d < mi:
-                    keep = at
-                    mi = d
-            if keep is not None:
-                pairs.append( (atom, keep) )
-                for atom3 in m3.atoms:
-                    if atom.id == atom3.id:
-                        atom3.x = keep.x
-        return pairs
+            lines = open(fname, 'r').readlines()
+        for line in lines:
+            if line[:4] == 'ATOM' or line[:6] == 'HETATM':
+                a = Atom().readPDBString(line)
+                self.atoms.append(a)
+            if line[:6] == 'CRYST1':
+                self.box = _p.box_from_cryst1(line)
+        self.make_chains()
+        self.make_residues()
+        self.unity = 'A'
+        return self
+
+    def __check_if_gap( self, atC, atN ):
+        if atC==None:
+            return(False)
+        if atN.name != 'N':
+            return(False)
+        d = atC - atN
+        if d > 1.7: # bond 
+            return(True)
+        return(False)
+
+    def __compareWithoutLastChar(self, str1, str2): 
+        if isinstance(str1,int) and isinstance(str2,int): # e.g. 52, 53
+            return(False)
+ 
+        if isinstance(str1,int): # e.g. 52, 52A
+            if str1==int(str2[0:-1]): # 52, 52A
+                return(True)
+            if str1==int(str2[0:-1])-1: # 52, 53A
+                return(True)
+        elif isinstance(str2,int): # e.g. 52A, 52
+            if int(str1[0:-1])==str2: # 52A, 52
+                return(True)
+            if int(str1[0:-1])==str2-1: # 52A, 53
+                return(True)
+        else: # e.g. 52A, 52B
+            if int(str1[0:-1])==int(str2[0:-1]): # 52A, 52B
+                return(True)
+            if int(str1[0:-1])==int(str2[0:-1])-1: # 52A, 53B
+                return(True)
+        return(False)
+
+    def _getChainIDs( self, lines ):
+        """from the pdb lines extract chain IDs """
+        usedChainIDs = []
+        for line in lines:
+            if (line[:4] == 'ATOM') or (line[:6] == 'HETATM'):
+                a = Atom().readPDBString(line)
+                if( a.chain_id not in usedChainIDs ):
+                    usedChainIDs.append( a.chain_id )
+        return( usedChainIDs )
         
-    if(bDist):
-        for atom in m1.atoms:
-            mi = dd # nm
-            keep = None
-            for at in m2.atoms:
-                d = (atom-at)/10.0
-                if d < mi:
-                    keep = at
-                    mi = d
-            if keep is not None:
-                pairs.append( (atom, keep) )
-                for atom3 in m3.atoms:
-                    if atom.id == atom3.id:
-                        atom3.x = keep.x
-    return pairs
-
-def assign_ff(model, itp):
-    for i, atom in enumerate(model.atoms):
-        at = itp.atoms[i]
-        atom.atomtype = at.atomtype
-        atom.cgnr = at.cgnr
-        atom.q = at.q
-        atom.m = at.m
-        atom.atomtypeB = at.atomtypeB
-        atom.qB = at.qB
-        atom.mB = at.mB
-
-# for forcefield2.py
-def gen_dih_entry2(a1,a2,a3,a4,dihtype,entry=None,entryB=None,scDumA=1.0,scDumB=1.0):
-    dihList = []
-    ids = [a1.id,a2.id,a3.id,a4.id]
-    if entry!=None:
-        entry = entry[0].split()
-        entry = [float(foo) for foo in entry]
-    if entryB!=None:
-        entryB = entryB[0].split()
-        entryB = [float(foo) for foo in entryB]
-    if (dihtype == 3 ):
-	zeroesA = [0,0,0,0,0,0]
-	zeroesB = [0,0,0,0,0,0]
-    elif (dihtype == 2): # improper has no multiplicity
-	angleA = 0
-        angleB = 0
-        if( entry != None ):
-            angleA = entry[0]
-        if( entryB != None ):
-            angleB = entryB[0]
-	zeroesA = [angleA,0]
-	zeroesB = [angleB,0]
-    else: # all the other types are the same
-	multA = 0
-	multB = 0
-	angleA = 0
-	angleB = 0
-	if( entry != None ):
-	    angleA = entry[0]
-	    multA = entry[2]
-	if( entryB != None ):
-	    angleB = entryB[0]
-	    multB = entryB[2]
-        zeroesA = [angleA,0,multA]
-        zeroesB = [angleB,0,multB]
-
-    if( entry != None ):
-	if( dihtype == 3 ):
-	    entry = [float(foo)*scDumA for foo in entry]
+    # TODO: make readPDB and readPDBTER a single function. It seems like
+    # readPDBTER is more general PDB reader?
+    def __readPDBTER(self, fname=None, pdbline=None, bNoNewID=True, bPDBGAP=False, bPDBMASS=False):
+        """Reads a PDB file with more options than __readPDB ?"""
+        if pdbline:
+            lines = pdbline.split('\n')
         else:
-            entry[1] = scDumA*float(entry[1])
-	dih = [a1,a2,a3,a4]+[dihtype]+[[dihtype]+entry]+[[dihtype]+zeroesA]
-        dihList.append(dih)
-    if( entryB != None ):
-        if( dihtype == 3 ):
-	    entryB = [float(foo)*scDumB for foo in entryB]
+            lines = open(fname, 'r').readlines()
+
+        chainIDstringInit = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnoprstuvwxyz123456789'
+        chainIDstring = copy.deepcopy(chainIDstringInit)
+        bNewChain = True
+        chainID = ' '
+        prevID = ' '
+        prevAtomName = ' '
+        prevResID = 0
+        prevResName = ' '
+        usedChainIDs = []
+        atomcount = 1
+        prevCatom = None
+
+        # get already used chain IDs
+        usedChainIDs = self._getChainIDs( lines )
+
+        for line in lines:
+            if 'TER' in line:
+                bNewChain = True
+            if (line[:4] == 'ATOM') or (line[:6] == 'HETATM'):
+                a = Atom().readPDBString(line, origID=atomcount)
+                atomcount += 1
+                # identify chain change by ID (when no TER is there)
+                if (a.chain_id != prevID):
+                    bNewChain = True
+                if (self.__check_if_gap( prevCatom,a )==True and bPDBGAP==True):
+                    bNewChain = True
+                if a.resname=='ACE' and prevResName!='ACE':
+                    bNewChain = True
+                if (a.resnr != prevResID):
+                    try:
+                        if self.__compareWithoutLastChar(prevResID,a.resnr)==True: # there are some special cases where residues are named, e.g. 52, 52A, 52B, ...
+                            bNewChain = False
+                        elif a.resnr != prevResID+1:
+                            bNewChain = True
+                        if (prevAtomName == 'OC2') or (prevAtomName == 'OXT') or (prevAtomName == 'OT2'):
+                            bNewChain = True
+                        if (prevAtomName == 'HH33') and ((prevResName=='NME') or (prevResName=='NAC') or (prevResName=='CT3')): # NME cap
+                            bNewChain = True
+                        # do not assign new chain IDs for waters, ions 
+                        if (a.resname=='WAT') or (a.resname=='SOL') or (a.resname=='TIP3') or (a.resname=='HOH') \
+                           or (a.resname=='NA') or (a.resname=='CL') \
+                           or (a.resname=='NaJ') or (a.resname=='Na') or (a.resname=='Cl') or (a.resname=='K') or (a.resname=='KJ') \
+                           or (a.resname=='MG') or (a.resname=='Mg') or (a.resname=='CA') or (a.resname=='Ca') or (a.resname=='CaJ') \
+                           or (a.resname=='ZN') or (a.resname=='Zn'): # add other ions when needed
+                            bNewChain = False
+                            chainID = ''
+                    except TypeError:
+                        bNewChain = False
+                        chainID = ''
+                # the option below overwrites all the others:
+                # when a non-empty ID of the next chain is the same as the previous, then do no change
+                if (a.chain_id!='') and (a.chain_id!=' ') and (a.chain_id==prevID):
+                    bNewChain = False
+                prevID = a.chain_id
+                prevResID = a.resnr
+                prevAtomName = a.name
+                prevResName = a.resname
+                if a.name == 'C':
+                    prevCatom = a
+                if bNewChain==True:
+                    if ((a.chain_id==' ') or (a.chain_id==chainID) or (a.chain_id in usedChainIDs) and bNoNewID==False):
+                        # find a new chain id
+                        bFound = False
+                        while bFound==False:
+                            if len(chainIDstring)==0: # used up all the IDs
+                                chainIDstring = copy.deepcopy(chainIDstringInit)
+                                chainID = "pmxX"
+                                break
+                            foo = chainIDstring[0]
+                            chainIDstring = chainIDstring.lstrip(chainIDstring[0])
+                            if foo not in usedChainIDs:
+                                bFound=True
+                                chainID = foo
+                                if bNoNewID==True:
+                                    chainID = "pmx"+foo
+                                usedChainIDs.append(chainID)
+                    else:
+                        chainID = a.chain_id
+                        usedChainIDs.append(chainID)
+                a.chain_id = chainID
+                self.atoms.append(a)
+                bNewChain = False
+            if line[:6] == 'CRYST1':
+                self.box = _p.box_from_cryst1(line)
+
+        ##### now fix chain IDs that have been newly created #####
+        newChainDict = {}
+        chainIDstring = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnoprstuvwxyz123456789'
+        for a in self.atoms:
+            # chain with a new ID
+            if 'pmx' in a.chain_id:
+                # this ID has already been encountered
+                if a.chain_id in newChainDict.keys():
+                    a.chain_id = newChainDict[a.chain_id]
+                # ID not yet encountered
+                else:
+                    # find a suitable ID
+                    bFound = False
+                    while bFound==False:
+                        if len(chainIDstring)==0: # used up all the IDs
+                            chainIDstring = copy.deepcopy(chainIDstringInit)
+                            newChainDict[a.chain_id] = "X"
+                            a.chain_id = "X"
+                            break
+                        foo = chainIDstring[0]
+                        chainIDstring = chainIDstring.lstrip(chainIDstring[0])
+                        # found
+                        if foo not in usedChainIDs:
+                            bFound=True
+                            usedChainIDs.append(foo)
+                            newChainDict[a.chain_id] = foo
+                            a.chain_id = foo
+
+        self.make_chains()
+        self.make_residues()
+        self.unity = 'A'
+
+        if bPDBMASS==True:
+            assign_masses_to_model( self )
+
+        return self
+
+    def __readGRO(self, filename):
+        """Reads a GRO file"""
+        l = open(filename).readlines()
+        # first line is name/comment
+        name = l[0].rstrip()
+        self.title = name
+        # next line is number of atoms
+        natoms = int(l[1])
+        atoms_parsed = 0
+        while atoms_parsed != natoms:
+            line = l[atoms_parsed+2]
+            resid = int(line[:5])
+            resname = line[5:9].strip()
+            name = line[10:15].strip()
+            idx = int(line[15:20])
+            rest = line[20:].split()
+            assert len(rest) in [3, 6]
+            x = float(rest[0])
+            y = float(rest[1])
+            z = float(rest[2])
+            coords = [x, y, z]
+            if len(rest) == 6:
+                vx = float(rest[3])
+                vy = float(rest[4])
+                vz = float(rest[5])
+                vel = [vx, vy, vz]
+            else:
+                vel = [0, 0, 0]
+            a = Atom(id=idx, name=name, resname=resname,
+                     resnr=resid, x=coords, v=vel, unity='nm')
+            a.get_symbol()
+            self.atoms.append(a)
+            atoms_parsed += 1
+        box_line = [float(i) for i in l[-1].split()]
+        assert len(box_line) in [3, 9]
+        box = [[0, 0, 0], [0, 0, 0], [0, 0, 0]]
+        box[0][0] = box_line[0]
+        box[1][1] = box_line[1]
+        box[2][2] = box_line[2]
+        if len(box_line) == 3:
+            box[0][1] = 0
+            box[0][2] = 0
+            box[1][0] = 0
+            box[1][2] = 0
+            box[2][0] = 0
+            box[2][1] = 0
         else:
-	    entryB[1] = scDumB*float(entryB[1])
-        dih = [a1,a2,a3,a4]+[dihtype]+[[dihtype]+zeroesB]+[[dihtype]+entryB]
-        dihList.append(dih)
-#    if( entry==None ):
-#        dih = ids+entryB+zeroesB
-#        dihList.append(dih)
-#    if( entryB==None ):
-#	dih = ids+zeroesA+entry
-#	dihList.append(dih)
-    return dihList
-
-# for forcefield.py
-def gen_dih_entry(ids,entry=None,entryB=None,scDumA=1.0,scDumB=1.0):
-    dihList = []
-    if (ids[4] == 3 ):
-	zeroesA = [0,0,0,0,0,0]
-	zeroesB = [0,0,0,0,0,0]
-    elif (ids[4] == 2): # improper has no multiplicity
-	angleA = 0
-        angleB = 0
-        if( entry != None ):
-            angleA = entry[0]
-        if( entryB != None ):
-            angleB = entryB[0]
-	zeroesA = [angleA,0]
-	zeroesB = [angleB,0]
-    else: # all the other types are the same
-	multA = 0
-	multB = 0
-	angleA = 0
-	angleB = 0
-	if( entry != None ):
-	    angleA = entry[0]
-	    multA = entry[2]
-	if( entryB != None ):
-	    angleB = entryB[0]
-	    multB = entryB[2]
-        zeroesA = [angleA,0,multA]
-        zeroesB = [angleB,0,multB]
-
-    if( entry != None ):
-	if( ids[4] == 3 ):
-	    entry = [foo*scDumA for foo in entry]
+            box[0][1] = box_line[3]
+            box[0][2] = box_line[4]
+            box[1][0] = box_line[5]
+            box[1][2] = box_line[6]
+            box[2][0] = box_line[7]
+            box[2][1] = box_line[8]
+        self.box = box
+        self.make_chains()
+        self.make_residues()
+        self.unity = 'nm'
+        return self
+
+    def assign_moltype(self):
+        """Identifies what type of molecule the Model is: protein, dna, or rna.
+        If it is a mix, or if it is an organic molecule, "unknown" is
+        assigned to self.moltype.
+        """
+        residues = set([r.resname for r in self.residues])
+
+        # do not consider water and ions
+        residues -= library._water
+        residues -= library._ions
+
+        # determine type
+        # if 'residues' is not empty AND it's a subset of 'library._protein_residues'
+        if bool(residues) and residues <= library._protein_residues:
+            self.moltype = 'protein'
+        elif bool(residues) and residues <= library._dna_residues:
+            self.moltype = 'dna'
+        elif bool(residues) and residues <= library._rna_residues:
+            self.moltype = 'rna'
         else:
-            entry[1] = scDumA*entry[1]
-	dih = ids+entry+zeroesA
-        dihList.append(dih)
-    if( entryB != None ):
-        if( ids[4] == 3 ):
-	    entryB = [foo*scDumB for foo in entryB]
+            self.moltype = 'unknown'
+
+    def read(self, filename, bPDBTER=False, bNoNewID=True, bPDBGAP=False, bPDBMASS=False):
+        """PDB/GRO file reader.
+
+        Parameters
+        ----------
+        filename : str
+            name of input file
+        bPDBTER : bool, optional
+            whether the file contains TER records?. Default is False.
+        bNoNewID : bool, optional
+            whether to assign new chain IDs. If True, new chain IDs starting
+            with 'pmx' will be assigned(?). Only relevant if bPDBTER is also
+            True. Default is True.
+        bPDBGAP : bool
+            whether search for gaps in the chain to assign new chain IDs.
+        """
+        ext = filename.split('.')[-1]
+        if ext == 'pdb':
+            if bPDBTER is True:
+                return self.__readPDBTER(fname=filename,
+                                         pdbline=None,
+                                         bNoNewID=bNoNewID, bPDBGAP=bPDBGAP, bPDBMASS=bPDBMASS)
+            else:
+                return self.__readPDB(fname=filename)
+        elif ext == 'gro':
+            return self.__readGRO(filename)
         else:
-	    entryB[1] = scDumB*entryB[1]
-        dih = ids+zeroesB+entryB
-        dihList.append(dih)
-#    if( entry==None ):
-#        dih = ids+entryB+zeroesB
-#        dihList.append(dih)
-#    if( entryB==None ):
-#	dih = ids+zeroesA+entry
-#	dihList.append(dih)
-    return dihList
-
-# for the newer forcefield2.py
-def get_ff2_entry(ids, itp, gmx45=True, what = 'bond'):
-    if what == 'bond':
-        for b in itp.bonds:
-            if (b[0].id == ids[0] and b[1].id == ids[1]) or \
-               (b[1].id == ids[0] and b[0].id == ids[1]):
-                out = xcopy.deepcopy(b)
-                return out[3:][0]
-    elif what == 'angle':
-        for b in itp.angles:
-            if (b[0].id == ids[0] and b[1].id == ids[1] and b[2].id == ids[2]) or \
-               (b[2].id == ids[0] and b[1].id == ids[1] and b[0].id == ids[2]):
-                out = xcopy.deepcopy(b)
-                return out[4:][0]
-    elif what == 'dihedral':
-        if (ids[4] == 3):
-            for b in itp.dihedrals:
-                if (b[0].id == ids[0] and b[1].id == ids[1] and b[2].id == ids[2] and b[3].id == ids[3]) or \
-                   (b[3].id == ids[0] and b[2].id == ids[1] and b[1].id == ids[2] and b[0].id == ids[3]):
-		    if( ids[4] == b[4] ):
-		        itp.dihedrals.remove(b)
-                        out = xcopy.deepcopy(b)
-                        return out[5:]
-        elif (ids[4] == 9):
-            for b in itp.dihedrals:
-                if (b[0].id == ids[0] and b[1].id == ids[1] and b[2].id == ids[2] and b[3].id == ids[3]) or \
-                   (b[3].id == ids[0] and b[2].id == ids[1] and b[1].id == ids[2] and b[0].id == ids[3]):
-		    if( ids[4] == b[4] ):
-		        itp.dihedrals.remove(b)
-                        out = xcopy.deepcopy(b)
-                        return out[5:]
-        elif (ids[4]==1 and gmx45==True): 
-            for b in itp.dihedrals:
-                if (b[0].id == ids[0] and b[1].id == ids[1] and b[2].id == ids[2] and b[3].id == ids[3]) or \
-                   (b[3].id == ids[0] and b[2].id == ids[1] and b[1].id == ids[2] and b[0].id == ids[3]):
-		    if( ids[4] == b[4] ):
-		        itp.dihedrals.remove(b)
-                        out = xcopy.deepcopy(b)
-                        return out[5:]
-        elif (ids[4]==2 or ids[4]==4 ): # improper
-            for b in itp.dihedrals:
-                sum = 0
-                for b1 in range(0,4):
-                    for b2 in range(0,4):
-                        if (b[b1].id == ids[b2]):
-                            sum += 1
-                            break
-                if ( (sum ==4) and (b[4]==2 or b[4]==4) ):
-		    itp.dihedrals.remove(b)
-                    out = xcopy.deepcopy(b)
-                    return out[5:]
-        elif (ids[4]==1 and gmx45==False ): # improper as proper in version < gmx45
-            for b in itp.dihedrals:
-                sum = 0
-                for b1 in range(0,4):
-                    for b2 in range(0,4):
-                        if (b[b1].id == ids[b2]):
-                            sum += 1
-                            break
-                if ( (sum == 4) and (b[4]==1) ):
-		    itp.dihedrals.remove(b)
-                    out = xcopy.deepcopy(b)
-                    return out[5:]
-    return None
-
-# for the older forcefield.py
-def get_ff_entry(ids, itp, gmx45=True, what = 'bond'):        
-    if what == 'bond':
-        for b in itp.bonds:
-            if (b[0] == ids[0] and b[1] == ids[1]) or \
-               (b[1] == ids[0] and b[0] == ids[1]):
-                return b[3:]
-    elif what == 'angle':
-        for b in itp.angles:
-            if (b[0] == ids[0] and b[1] == ids[1] and b[2] == ids[2]) or \
-               (b[2] == ids[0] and b[1] == ids[1] and b[0] == ids[2]):
-                return b[4:]
-    elif what == 'dihedral':
-        if (ids[4] == 3):
-            for b in itp.dihedrals:
-                if (b[0] == ids[0] and b[1] == ids[1] and b[2] == ids[2] and b[3] == ids[3]) or \
-                   (b[3] == ids[0] and b[2] == ids[1] and b[1] == ids[2] and b[0] == ids[3]):
-		    if( ids[4] == b[4] ):
-		        itp.dihedrals.remove(b)
-                        return b[5:]
-        elif (ids[4] == 9):
-            for b in itp.dihedrals:
-                if (b[0] == ids[0] and b[1] == ids[1] and b[2] == ids[2] and b[3] == ids[3]) or \
-                   (b[3] == ids[0] and b[2] == ids[1] and b[1] == ids[2] and b[0] == ids[3]):
-		    if( ids[4] == b[4] ):
-		        itp.dihedrals.remove(b)
-                        return b[5:]
-        elif (ids[4]==1 and gmx45==True): 
-            for b in itp.dihedrals:
-                if (b[0] == ids[0] and b[1] == ids[1] and b[2] == ids[2] and b[3] == ids[3]) or \
-                   (b[3] == ids[0] and b[2] == ids[1] and b[1] == ids[2] and b[0] == ids[3]):
-		    if( ids[4] == b[4] ):
-		        itp.dihedrals.remove(b)
-                        return b[5:]
-        elif (ids[4]==2 or ids[4]==4 ): # improper
-            for b in itp.dihedrals:
-                sum = 0
-                for b1 in range(0,4):
-                    for b2 in range(0,4):
-                        if (b[b1] == ids[b2]):
-                            sum += 1
-                            break
-                if ( (sum ==4) and (b[4]==2 or b[4]==4) ):
-		    itp.dihedrals.remove(b)
-                    return b[5:]
-        elif (ids[4]==1 and gmx45==False ): # improper as proper in version < gmx45
-            for b in itp.dihedrals:
-                sum = 0
-                for b1 in range(0,4):
-                    for b2 in range(0,4):
-                        if (b[b1] == ids[b2]):
-                            sum += 1
-                            break
-                if ( (sum == 4) and (b[4]==1) ):
-		    itp.dihedrals.remove(b)
-                    return b[5:]
-    return None
-
-def read_pairs_file(fn):
-    l = open(fn).readlines()
-    plst = []
-    for line in l:
-       plst.append(line.split())
-    return plst
-
-################################################################################33
-
-
-def main(argv):
-
-	version = "1.1"
-
-	# define input/output files
-	files= [
-	   FileOption("-l1", "r",["pdb"],"ligand1.pdb",""),
-	   FileOption("-l2", "r",["pdb"],"ligand2.pdb",""),
-	   FileOption("-itp1", "r",["itp"],"lig1.itp",""),
-	   FileOption("-itp2", "r",["itp"],"lig2.itp",""),
-	   FileOption("-n1", "r/o",["ndx"],"scaffold1" ,""),
-	   FileOption("-n2", "r/o",["ndx"],"scaffold2","" ),
-	   FileOption("-pairs", "r/o",["dat"],"pairs" ,""),
-	   FileOption("-oa", "w",["pdb"],"mergedA.pdb" ,""),
-	   FileOption("-ob", "w",["pdb"],"mergedB.pdb" ,""),
-	   FileOption("-oitp", "w",["itp"],"merged.itp","" ),
-	   FileOption("-ffitp", "w",["itp"],"ffmerged.itp" ,""),
-#	   FileOption("-ffitp1", "w/o",["itp"],"ffitp1.itp" ,""),
-#	   FileOption("-ffitp2", "w/o",["itp"],"ffitp2.itp" ,""),
-	   FileOption("-log", "w",["log"],"hybrid.log" ,""),
-	    ]
-
-	# define options
-	options=[
-#	   Option( "-bDist", "bool", "False", "use distance (no alignment) for the morphes"),
-           Option( "-d", "float", "0.05", "distance (nm) between atoms to consider them morphable"),
-           Option( "-scDUMm", "float", "1.0", "scale dummy masses using the counterpart atoms"),
-           Option( "-scDUMa", "float", "1.0", "scale bonded dummy angle parameters"),
-           Option( "-scDUMd", "float", "1.0", "scale bonded dummy dihedral parameters"),
-           Option( "-deAng", "bool", "false", "decouple angles composed of 1 dummy and 2 non-dummies"),
- #          Option( "-GMX45", "bool", "true", "set to noGMX45 for the topologies of earlier gromacs generations"),
-           Option( "-fit", "bool", "false", "fit mol2 onto mol1, only works if pairs.dat is provided"),
-           Option( "-split", "bool", "false", "split the topology into separate transitions"),
-            ]
-
-	help_text = ()
-
-	# pass options, files and the command line to pymacs
-
-   	cmdl = Commandline( argv, options = options,
-                       fileoptions = files,
-                       program_desc = help_text,
-                       check_for_existing_files = False )
-
-	# deal with flags
-	if cmdl.opt['-pairs'].is_set:
-	    read_pairs_from_file = True
-	else:
-	    read_pairs_from_file = False
-
-	gmx45 = True
-	bFit = False
-	deAng = False
-
-        bScaleMass = False #inverse of mDUM
-#        if mDUM==True:
-#            bScaleMass = False
-	if(cmdl['-fit']==True and read_pairs_from_file==True):
-	    bFit = True
-        if(cmdl['-deAng']==True ):
-            deAng = True
-
-	if cmdl.opt['-n1'].is_set:
-	    read_from_idx = True
-	else:
-	    read_from_idx = False
-        bSplit = cmdl['-split']
-
-	dist = 0.05
-	if( cmdl.opt['-d'].is_set ):
-	    dist = cmdl['-d']
-
-        scDuma = 1.0
-        if( cmdl.opt['-scDUMa'].is_set ):
-            scDuma = cmdl['-scDUMa']
-        scDumd = 1.0
-        if( cmdl.opt['-scDUMd'].is_set ):
-            scDumd = cmdl['-scDUMd']
-        scDUMm = 1.0
-        if( cmdl.opt['-scDUMm'].is_set ):
-            scDUMm = cmdl['-scDUMm']
-
-	logfile = open(cmdl['-log'],'w')
-
-	if read_from_idx and read_pairs_from_file:
-	    do_log(logfile, "Error: Can either read a pair list or scaffold index files!")
-	    do_log(logfile,"Exiting!")
-	    sys.exit(1)
-
-
-	do_log(logfile,'Reading ligand 1 from: "%s"' % cmdl['-l1'])
-	do_log(logfile,'Reading ligand 2 from: "%s"' % cmdl['-l2'])
-
-	m1 = Model().read(cmdl['-l1'])
-	m2 = Model().read(cmdl['-l2'])
-
-	do_log(logfile,'Reading itp file 1 from: "%s"' % cmdl['-itp1'])
-	do_log(logfile,'Reading itp file 2 from: "%s"' % cmdl['-itp2'])
-
-	itp1 = ITPFile(cmdl['-itp1'])
-	itp2 = ITPFile(cmdl['-itp2'])
-
-	do_log(logfile,"Assigning forcefield parameters....")
-	assign_ff(m1,itp1)
-	assign_ff(m2,itp2)
-	do_log(logfile,"Making pairs.....")
-
-	if read_pairs_from_file:
-	    do_log(logfile,'Reading file with atom pairs: "%s"' % cmdl['-pairs'])  
-	    plst = read_pairs_file(cmdl['-pairs'])
-	else:
-	    plst = None
-
-	if read_from_idx:
-	    do_log(logfile,'Reading scaffold index file: "%s"' % cmdl['-n1'])  
-#	    grp1 = IndexFile(args['-n1']['fns']).dic['scaffold']
-	    grp1 = IndexFile(cmdl['-n1']).dic['scaffold']
-	    do_log(logfile,'Reading scaffold index file: "%s"' % cmdl['-n2'])  
-	    grp2 = IndexFile(cmdl['-n2']).dic['scaffold']
-	    # now we add all atoms with bonds to scaffold atoms
-	    for b in itp1.bonds:
-		if b[0] in grp1.ids and b[1] not in grp1.ids:
-		    grp1.ids.append(b[1])
-		    do_log(logfile,'Adding atom %s to scaffold 1' % m1.atoms[b[1]-1].name)  
-		elif b[1] in grp1.ids and b[0] not in grp1.ids:
-		    grp1.ids.append(b[0])
-		    do_log(logfile,'Adding atom %s to scaffold 1' % m1.atoms[b[0]-1].name)  
-	    for b in itp2.bonds:
-		if b[0] in grp2.ids and b[1] not in grp2.ids:
-		    grp2.ids.append(b[1])
-		    do_log(logfile,'Adding atom %s to scaffold 2' % m2.atoms[b[1]-1].name)  
-		elif b[1] in grp2.ids and b[0] not in grp2.ids:
-		    grp2.ids.append(b[0])
-		    do_log(logfile,'Adding atom %s to scaffold 2' % m2.atoms[b[0]-1].name)
-	    grps = [grp1.ids, grp2.ids]
-	else:
-	    grps = None
-
-        m3 = m1.copy() #m3 will contain all the atoms from m1, but with the coordinates of the matching atoms from m2
-        m4 = m2.copy() #need to copy it when fitting
-
-	# fitting 
-	if(bFit==True):
-	    from rdkit import Chem
-	    from rdkit.Chem import AllChem
-	    n1 = []
-	    n2 = []
-	    for p in plst:
-		n1.append(int(p[0])-1)
-		n2.append(int(p[1])-1)
-
-	    do_log(logfile,'Superimposing mol2 on mol1')
-            try:
-      	        pdbName1,atomNameDict1 = reformatPDB(cmdl['-l1'],1)
-      	        pdbName2,atomNameDict2 = reformatPDB(cmdl['-l2'],2)
- 	        mol1 = Chem.MolFromPDBFile(pdbName1,removeHs=False,sanitize=False)
-	        mol2 = Chem.MolFromPDBFile(pdbName2,removeHs=False,sanitize=False)
-      	        os.remove(pdbName1)
-    	        os.remove(pdbName2)
-	        Chem.rdMolAlign.AlignMol(mol2,mol1,atomMap=zip(n2,n1))
-            except:
-      	        pdbName1,atomNameDict1 = reformatPDB(cmdl['-l1'],1,bStrict=True)
-      	        pdbName2,atomNameDict2 = reformatPDB(cmdl['-l2'],2,bStrict=True)
- 	        mol1 = Chem.MolFromPDBFile(pdbName1,removeHs=False,sanitize=False)
-	        mol2 = Chem.MolFromPDBFile(pdbName2,removeHs=False,sanitize=False)
-      	        os.remove(pdbName1)
-    	        os.remove(pdbName2)
-	        Chem.rdMolAlign.AlignMol(mol2,mol1,atomMap=zip(n2,n1))
-	    # adjust coordinates of m2
-	    adjustCoords(m2,mol2)  
-	    restoreAtomNames(mol1,atomNameDict1)
-	    restoreAtomNames(mol2,atomNameDict2)
-
-            do_log(logfile,'Superimposing mol1 on mol2')
-            try:
-                pdbName1,atomNameDict1 = reformatPDB(cmdl['-l1'],1)
-                pdbName2,atomNameDict2 = reformatPDB(cmdl['-l2'],2)
-                mol1 = Chem.MolFromPDBFile(pdbName1,removeHs=False,sanitize=False)
-                mol2 = Chem.MolFromPDBFile(pdbName2,removeHs=False,sanitize=False)
-                os.remove(pdbName1)
-                os.remove(pdbName2)
-                Chem.rdMolAlign.AlignMol(mol1,mol2,atomMap=zip(n1,n2))
-            except:
-                pdbName1,atomNameDict1 = reformatPDB(cmdl['-l1'],1,bStrict=True)
-                pdbName2,atomNameDict2 = reformatPDB(cmdl['-l2'],2,bStrict=True)
-                mol1 = Chem.MolFromPDBFile(pdbName1,removeHs=False,sanitize=False)
-                mol2 = Chem.MolFromPDBFile(pdbName2,removeHs=False,sanitize=False)
-                os.remove(pdbName1)
-                os.remove(pdbName2)
-                Chem.rdMolAlign.AlignMol(mol1,mol2,atomMap=zip(n1,n2))
-            # adjust coordinates of m1
-	    adjustCoords(m3,mol1)  
-	    restoreAtomNames(mol1,atomNameDict1)
-	    restoreAtomNames(mol2,atomNameDict2)
-#	sys.exit(0)
-
-        bDist = True
-        pairs = make_pairs(m1, m2, m3, m4, bFit, bDist,dist, plst, grps)
-
-	morphsA = map(lambda p: p[1], pairs)
-	morphsB = map(lambda p: p[0], pairs)
-	dumsA = []
-	dumsA_nofit = []
-	if(bFit==False):
-	    for atom in m2.atoms:
-	        if atom not in morphsA:
-		    dumsA.append(atom)
-	else:
-	    for (atom,at) in zip(m2.atoms,m4.atoms):
-		if atom not in morphsA:
-		    dumsA.append(atom)
-		    dumsA_nofit.append(at)
-	dumsB = []
-	for atom in m1.atoms:
-	    if atom not in morphsB:
-		dumsB.append(atom)
-	do_log(logfile, "Generated %d atom-atom pairs" % len(pairs))
-	do_log(logfile,"Dummies in state A: %d" % len(dumsA))
-	do_log(logfile,"Dummies in state B: %d" % len(dumsB))
-
-
-
-	do_log(logfile,"Making B-states....")
-	for a1, a2 in pairs:
-	    a1.atomtypeB = a2.atomtype
-	    a2.atomtypeB = a1.atomtype #this is my change to catch the DISAPPEARING dihedrals
-	    a1.nameB = a2.name
-	    a1.qB = a2.q
-	    a1.mB = a2.m
-	    a1.idB = a2.id
-	    a2.idB = a1.id #this is my change to catch the DISAPPEARING dihedrals
-	    a2.mB = a1.m
-	    do_log(logfile, "Atom....: %4d  %12s | %6.2f | %6.2f -> %12s | %6.2f | %6.2f" %\
-		   (a1.id, a1.atomtype, a1.q, a1.m, a1.atomtypeB, a1.qB, a1.mB))
-
-	if( bFit==False):
-	    for atom in dumsA:
-	        atom.id_old = atom.id
-	        atom.nameB = atom.name
-	        atom.name = 'D'+atom.name
-	        atom.atomtypeB = atom.atomtype
-	        atom.atomtype = 'DUM_'+atom.atomtype
-	        atom.qB = atom.q
-	        atom.q = 0
-	        atom.mB = atom.m
-	        atom.m = atom.mB #1.
-                
-                atom.m = atom.m*scDUMm
-                if( atom.m < 1.0 and atom.mB != 0.0): # exception for virtual particles
-                    atom.m = 1.0
-
-	        m1.residues[0].append(atom)
- 	        m3.residues[0].append(atom)
-	        do_log(logfile, "Dummy...: %4d  %12s | %6.2f | %6.2f -> %12s | %6.2f | %6.2f" %\
-		       (atom.id, atom.atomtype, atom.q, atom.m, atom.atomtypeB, atom.qB, atom.mB))
-	else:
-            for (atom,at) in zip(dumsA,dumsA_nofit):
-                atom.id_old = atom.id
-                atom.nameB = atom.name
-                atom.name = 'D'+atom.name
-                atom.atomtypeB = atom.atomtype
-                atom.atomtype = 'DUM_'+atom.atomtype
-                atom.qB = atom.q
-                atom.q = 0
-                atom.mB = atom.m
-                atom.m = atom.mB #1.
-
-                atom.m = atom.m*scDUMm
-                if( atom.m < 1.0 and atom.mB != 0.0): # exception for virtual particles
-                    atom.m = 1.0
-
-                m1.residues[0].append(atom)
-                at.id_old = at.id
-                at.nameB = at.name
-                at.name = 'D'+at.name
-                at.atomtypeB = at.atomtype
-                at.atomtype = 'DUM_'+at.atomtype
-                at.qB = at.q
-                at.q = 0
-                at.mB = at.m
-                at.m = at.mB #1.
-
-                at.m = at.m*scDUMm
-                if( at.m < 1.0 and at.mB != 0.0): # exception for virtual particles
-                    at.m = 1.0
-
-                m3.residues[0].append(at)
-                do_log(logfile, "Dummy...: %4d  %12s | %6.2f | %6.2f -> %12s | %6.2f | %6.2f" %\
-                       (atom.id, atom.atomtype, atom.q, atom.m, atom.atomtypeB, atom.qB, atom.mB))
-
-
-	for atom in dumsB:
-	    atom.atomtypeB = 'DUM_'+atom.atomtype
-	    atom.qB = 0
-	    atom.mB = atom.m #1.
-
-            atom.mB = atom.mB*scDUMm
-            if( atom.mB < 1.0 and atom.m != 0.0): # exception for virtual particles
-                atom.mB = 1.0
-
-	    do_log(logfile, "Dummy...: %4d  %12s | %6.2f | %6.2f -> %12s | %6.2f | %6.2f" %\
-		   (atom.id, atom.atomtype, atom.q, atom.m, atom.atomtypeB, atom.qB, atom.mB))
-
-	id_dicAB = {}
-	id_dicBA = {}
-	for atom in m1.atoms:
-	    if hasattr(atom,"idB"):
-		id_dicAB[atom.id] = atom.idB
-		id_dicBA[atom.idB] = atom.id
-	    if hasattr(atom,"id_old"):
-		id_dicAB[atom.id] = atom.id_old
-		id_dicBA[atom.id_old] = atom.id
-		
-	do_log(logfile, "Generating bonded parameters....")    
-
-
-	# go over bonds
-	newbonds = []
-
-	for b in itp1.bonds:
-	    id1 = b[0].id
-	    id2 = b[1].id
-	    a1 = m1.atoms[id1-1]
-	    a2 = m1.atoms[id2-1]
-	    bOk = False
-	    if hasattr(a1,"idB") and hasattr(a2,"idB"):
-		idB1 = a1.idB
-		idB2 = a2.idB
-		entr = get_ff2_entry([idB1, idB2], itp2, gmx45, what= 'bond')
-		if entr is not None:
-		    newbonds.append ([b[0],b[1],b[2],[b[2]]+b[3],[b[2]]+entr])
-		    bOk = True
-		else:
-		    bOk = False
-	    elif a1.atomtypeB[:3] == 'DUM' or a2.atomtypeB[:3] == 'DUM':
-		entr = get_ff2_entry([a1.id, a2.id], itp1, gmx45, what= 'bond')
-		if entr is not None:
-		    newbonds.append ([b[0],b[1],b[2],[b[2]]+b[3],[b[2]]+entr])
-		    bOk = True
-		else:
-		    bOk = False
-	    else:
-		newbonds.append(b)
-		bOk = True
-
-	    if not bOk:
-		do_log(logfile, "Error: Something went wrong while assigning bonds!")
-		do_log(logfile, "A-> Atom1: %d-%s Atom2: %d-%s" %(a1.id, a1.name, a2.id, a2.name))
-		do_log(logfile, "B-> Atom1: %d-%s Atom2: %d-%s" %(a1.idB, a1.nameB, a2.idB, a2.nameB))
-		do_log(logfile,"Exiting....")
-		sys.exit(1)
-
-	# angles
-	newangles = []
-	decoupAngles = []
-	for b in itp1.angles:
-            angtype = b[3]
-            ####### explanation for angle parameters ############
-            # for angtype 1, entry is [angle,force_const]
-            # for angtype 5, entry is [5,angle,force_const,bond,force_const]
-            # write_angles() in forcefield2.py expects entry [angtype,angle,force_const,...]
-	    id1 = b[0].id
-	    id2 = b[1].id
-	    id3 = b[2].id
-	    a1 = m1.atoms[id1-1]
-	    a2 = m1.atoms[id2-1]
-	    a3 = m1.atoms[id3-1]
-	    bOk = False
-	    if hasattr(a1,"idB") and hasattr(a2,"idB") and hasattr(a3,"idB"):
-		idB1 = a1.idB
-		idB2 = a2.idB
-		idB3 = a3.idB
-		entr = get_ff2_entry([idB1, idB2, idB3], itp2, gmx45, what= 'angle')
-		if entr is not None:
-                    if angtype==1:
-                        newangles.append ([b[0],b[1],b[2],angtype,[angtype]+b[4],[angtype]+entr])
-                    else:
-		        newangles.append ([b[0],b[1],b[2],angtype,b[4],entr])
-		    bOk = True
-		else:
-		    bOk = False
-	    elif a1.atomtypeB[:3] == 'DUM' or \
-		     a2.atomtypeB[:3] == 'DUM' or \
-		     a3.atomtypeB[:3] == 'DUM':
-		entr = get_ff2_entry([a1.id, a2.id, a3.id], itp1, gmx45, what= 'angle')
-                if (angtype!=1) and (entr is not None): # remove the angtype from the entr
-                    entr = entr[1:]
-		if entr is not None:
-		    if( (a1.atomtypeB[:3] != 'DUM' and a2.atomtypeB[:3] != 'DUM') \
-			or (a1.atomtypeB[:3] != 'DUM' and a3.atomtypeB[:3] != 'DUM') \
-			or (a2.atomtypeB[:3] != 'DUM' and a3.atomtypeB[:3] != 'DUM') ):
-#		    if( (a1.atomtypeB[:3] != 'DUM') or (a2.atomtypeB[:3] != 'DUM') or (a3.atomtypeB[:3] != 'DUM') ):
-	                entr[1] = scDuma*entr[1]
-                        if angtype==5:
-                            entr[3] = scDuma*entr[3]
-			if(deAng==True):
-			    if( a1.atomtypeB[:3] == 'DUM' ):
-			        if( findIDinList(id1,decoupAngles)==True ):
-				    entr[1] = 0.0
-                                    if angtype==5:
-                                        entr[3] = 0.0
-				else:
-				    decoupAngles.append(id1)
-			    elif( a2.atomtypeB[:3] == 'DUM' ):
-				if( findIDinList(id2,decoupAngles)==True ):
-                                    entr[1] = 0.0
-                                    if angtype==5:
-                                        entr[3] = 0.0
-                                else:
-                                    decoupAngles.append(id2)
-			    elif( a3.atomtypeB[:3] == 'DUM' ):
-				if( findIDinList(id3,decoupAngles)==True ):
-                                    entr[1] = 0.0
-                                    if angtype==5:
-                                        entr[3] = 0.0
-                                else:
-                                    decoupAngles.append(id3)
-                    if angtype==1:
-  	                newangles.append ([b[0],b[1],b[2],angtype,[angtype]+b[4],[angtype]+entr])
-                    else:
-  	                newangles.append ([b[0],b[1],b[2],angtype,b[4],[angtype]+entr])
-		    bOk = True
-		else:
-		    bOk = False
-	    else:
-		newangles.append(b)
-		bOk = True
-
-	    if not bOk:
-		do_log(logfile, "Error: Something went wrong while assigning angles!")
-		do_log(logfile, "A-> Atom1: %d-%s Atom2: %d-%s Atom3: %d-%s" \
-		       %(a1.id, a1.name, a2.id, a2.name, a3.id, a3.name))
-		do_log(logfile, "B-> Atom1: %d-%s Atom2: %d-%s Atom3: %d-%s" \
-		       %(a1.idB, a1.nameB, a2.idB, a2.nameB, a3.idB, a3.nameB))
-		do_log(logfile,"Exiting....")
-		sys.exit(1)
-
-
-	#############################
-	############ VG #############
-	# COMPLETE DIHEDRAL REWRITE #
-	#############################
-	newdihedrals = []
-	cpItp1 = xcopy.deepcopy(itp1)
-	cpItp2 = xcopy.deepcopy(itp2)
-	for b in itp1.dihedrals:
-	    id1 = b[0].id
-            id2 = b[1].id
-            id3 = b[2].id
-            id4 = b[3].id
-            dih_type = b[4]
-            a1 = m1.atoms[id1-1]
-            a2 = m1.atoms[id2-1]
-            a3 = m1.atoms[id3-1]
-            a4 = m1.atoms[id4-1]
-            entrA = get_ff2_entry([id1, id2, id3, id4, dih_type], cpItp1, gmx45, what= 'dihedral')
-            bOk = False
-            if hasattr(a1,"idB") and hasattr(a2,"idB") and \
-                   hasattr(a3,"idB") and hasattr(a4,"idB"):
-		# switch the A state off
-                dih = gen_dih_entry2(a1, a2, a3, a4, dih_type, entrA,None)
-                newdihedrals.extend(dih)
-		bOk = True
-	    else:
-                # switch the B state on
-                if a1.atomtypeB[:3] == 'DUM' or \
-                         a2.atomtypeB[:3] == 'DUM' or \
-                         a3.atomtypeB[:3] == 'DUM' or \
-                         a4.atomtypeB[:3] == 'DUM':
-                    if entrA is not None:
-                        dih = gen_dih_entry2(a1, a2, a3, a4, dih_type,entrA,None)
-                        newdihedrals.extend(dih)
-#                        if( (a1.atomtypeB[:3] != 'DUM' and a2.atomtypeB[:3] != 'DUM' and a3.atomtypeB[:3] != 'DUM') \
-#                            or (a1.atomtypeB[:3] != 'DUM' and a2.atomtypeB[:3] != 'DUM' and a4.atomtypeB[:3] != 'DUM') \
-#                            or (a2.atomtypeB[:3] != 'DUM' and a3.atomtypeB[:3] != 'DUM' and a4.atomtypeB[:3] != 'DUM') \
-#                            or (a1.atomtypeB[:3] != 'DUM' and a3.atomtypeB[:3] != 'DUM' and a4.atomtypeB[:3] != 'DUM') ):
-			if( a1.atomtypeB[:3] != 'DUM' or a2.atomtypeB[:3] != 'DUM' or a3.atomtypeB[:3] != 'DUM' or a4.atomtypeB[:3] != 'DUM' ):
-#                        if( (a1.atomtypeB[:3] != 'DUM' and a2.atomtypeB[:3] != 'DUM') \
-#			    or (a1.atomtypeB[:3] != 'DUM' and a3.atomtypeB[:3] != 'DUM') \
-#			    or (a1.atomtypeB[:3] != 'DUM' and a4.atomtypeB[:3] != 'DUM') \
-#			    or (a2.atomtypeB[:3] != 'DUM' and a3.atomtypeB[:3] != 'DUM') \
-#			    or (a2.atomtypeB[:3] != 'DUM' and a4.atomtypeB[:3] != 'DUM') \
-#			    or (a3.atomtypeB[:3] != 'DUM' and a4.atomtypeB[:3] != 'DUM') ):
-                            if dih_type==2 or dih_type==4:# or dih_type==1: # disable improper for dummy-nondummy
-                                dih = gen_dih_entry2(a1, a2, a3, a4, dih_type,None,entrA,1.0,0.0)
-                            else:
-                                dih = gen_dih_entry2(a1, a2, a3, a4, dih_type,None,entrA,1.0,scDumd)
-			else:
-                            dih = gen_dih_entry2(a1, a2, a3, a4, dih_type,None,entrA)
-                        newdihedrals.extend(dih)
-                        bOk = True
-                    else:
-                        bOk = False
+            raise IOError('ERROR: Can only read pdb or gro!')
+
+    def renumber_residues(self):
+        """Renumbers all residues from 1."""
+        for i, res in enumerate(self.residues):
+            res.set_orig_resid(res.id)
+            res.set_resid(i+1)
+
+    # TODO/FIXME: should add/remove/append atoms all be only once in
+    # Atomselection? At the moment they are repeated in Molecule, Chain,
+    # and Model
+    def remove_atom(self, atom):
+        """Removes an Atom instance.
+
+        Parameters
+        ----------
+        atom : Atom
+            Atom instance to remove
+        """
+        m = atom.molecule
+        m.remove_atom(atom)
+
+    def remove_residue(self, residue, renumber_atoms=True, renumber_residues=True):
+        """Removes a Molecule/residue instance.
+
+        Parameters
+        ----------
+        residue : Molecule
+            Molecule instance to remove
+        renumber_atoms : bool, optional
+            whether to renumber the atoms of the Model after removing the
+            residue. Default is True.
+        renumber_residues : bool, optional
+            whether to renumber the residues of the Model after removing the
+            residue. Default is True.
+        """
+        ch = residue.chain
+        ch.remove_residue(residue, renumber_atoms=renumber_atoms,
+                          renumber_residues=renumber_residues)
+
+    def remove_chain(self, key):
+        """Removes a Chain instance given the chain ID.
+
+        Parameters
+        ----------
+        key : str
+            ID of the chain to remove
+        """
+        if key not in self.chdic:
+            print('No chain %s to remove....' % key)
+            print('No changes applied.')
+            return
+        for ch in self.chains:
+            if ch.id == key:
+                idx = self.chains.index(ch)
+                del self.chains[idx]
+                del self.chdic[key]
+        self.resl_from_chains()
+        self.al_from_resl()
+        self.renumber_residues()
+        self.renumber_atoms()
+
+    def __delitem__(self, key):
+        self.remove_chain(key)
+
+    def insert_residue(self, pos, res, chain_id):
+        """Inserts a residue in Model.
+
+        Parameters
+        ----------
+        pos : int
+            position/index where to insert the residue
+        res : Molecule
+            Molecule instance to insert containig the residue of interest
+        chain_id : str
+            ID of the chain where to insert the residue
+        """
+        ch = self.chdic[chain_id]
+        ch.insert_residue(pos, res)
+
+    def replace_residue(self, residue, new, bKeepResNum=False):
+        """Replaces a residue.
+
+        Parameters
+        ----------
+        residue : Molecule
+            residue to replace
+        new : Molecule
+            residue to insert
+        bKeepResNum : bool, optional
+            whether to keep residue ID of the residue that is inserted.
+            Default is False
+        """
+        ch = residue.chain
+        ch.replace_residue(residue, new, bKeepResNum)
+
+    def insert_chain(self, pos, new_chain):
+        """Inserts a Chain in Model.
+
+        Parameters
+        ----------
+        pos : int
+            index where to insert the chain within the list of chains
+        new_chain : Chain
+            instance of the Chain to insert in Model
+        """
+        if new_chain.id in self.chdic:
+            print('Chain identifier %s already in use!' % new_chain.id)
+            print('Changing chain identifier to 0')
+            new_chain.set_chain_id('0')
+        self.chains.insert(pos, new_chain)
+        self.resl_from_chains()
+        self.al_from_resl()
+        self.make_chains()
+        self.make_residues()
+        self.renumber_atoms()
+        self.renumber_residues()
+
+    def append(self, new_chain):
+        """ we assume chain is a Chain"""
+        idx = len(self.chains)
+        self.insert_chain(idx, new_chain)
+
+    def fetch_residue(self, idx, chain=None):
+        """Get a residue based on its index, or index and chain.
+
+        Parameters
+        ----------
+        idx : int
+            ID of the residue to fetch.
+        chain : str, optional
+            chain ID of the residue. This is needed when you have multiple
+            chains and you have not renumbered the residues.
+
+        Returns
+        -------
+        residue : Molecule
+            Molecule instance of the residue found.
+        """
+
+        #########################
+        # generate some residue id lists
+        valid_resids = []
+        for r in self.residues:
+            if isinstance(r.id,str):
+                valid_resids.append(r.id.replace(" ",""))
+            else:
+                valid_resids.append(r.id)
+
+        if chain is not None:        
+            valid_chresids = []
+            for r in self.chdic[chain].residues:
+                if isinstance(r.id,str):
+                    valid_chresids.append(r.id.replace(" ",""))
                 else:
-                    newdihedrals.append(b)
-                    bOk = True
+                    valid_chresids.append(r.id)
+        ##########################
 
-            if not bOk:
-                do_log(logfile, "Error: Something went wrong while assigning dihedrals!")
-                do_log(logfile, "A-> Atom1: %d-%s Atom2: %d-%s Atom3: %d-%s Atom3: %d-%s" \
-                       %(a1.id, a1.name, a2.id, a2.name, a3.id, a3.name, a4.id, a4.name))
-                do_log(logfile, "B-> Atom1: %d-%s Atom2: %d-%s Atom3: %d-%s Atom3: %d-%s" \
-                       %(a1.idB, a1.nameB, a2.idB, a2.nameB, a3.idB, a3.nameB, a4.idB, a4.nameB))
-                do_log(logfile,"Exiting....")
-                sys.exit(1)
-        
-	
-	# second molecule dihedrals
-	for b in itp2.dihedrals:
-            id1 = b[0].id
-            id2 = b[1].id
-            id3 = b[2].id
-            id4 = b[3].id
-            aB1 = m2.atoms[id1-1]
-            aB2 = m2.atoms[id2-1]
-            aB3 = m2.atoms[id3-1]
-            aB4 = m2.atoms[id4-1]
-            newid1 = id_dicBA[b[0].id]
-            newid2 = id_dicBA[b[1].id]
-            newid3 = id_dicBA[b[2].id]
-            newid4 = id_dicBA[b[3].id]
-            a1 = m1.atoms[newid1-1]
-            a2 = m1.atoms[newid2-1]
-            a3 = m1.atoms[newid3-1]
-            a4 = m1.atoms[newid4-1]
-            dih_type = b[4]
-	    entrB = get_ff2_entry([b[0].id,b[1].id,b[2].id,b[3].id, dih_type], cpItp2, gmx45, what='dihedral')
-            bOk = False
-            if hasattr(aB1,"idB") and hasattr(aB2,"idB") and \
-                   hasattr(aB3,"idB") and hasattr(aB4,"idB"):
-		# switch the B state off
-                dih = gen_dih_entry2(a1,a2,a3,a4, dih_type,None,entrB)
-                newdihedrals.extend(dih)
-		bOk = True
+
+        # check idx is a valid selection
+        if idx not in valid_resids:#[r.id for r in self.residues]:
+            raise ValueError('resid %s not found in Model residues' % idx)
+
+        if chain is None:
+            # check selection is unique
+            if [r.id for r in self.residues].count(idx) > 1:
+                raise ValueError('idx choice %s results in non-unique selection' % idx)
+        else:
+            # check chain is a valid selection
+            if chain not in [c.id for c in self.chains]:
+                raise ValueError('chain ID "%s" not found in Model chains' % chain)
+            # check idx+chain is a valid selection
+            if idx not in valid_chresids:#[r.id for r in self.chdic[chain].residues]:
+                raise ValueError('resid %s not found in chain "%s"' % (idx, chain))
+            # check selection is unique
+            if [r.id for r in self.chdic[chain].residues].count(idx) > 1:
+                raise ValueError('idx choice %s for chain "%s" results in non-unique selection' % (idx, chain))
+
+        # then find and return the residue
+        if chain is None:
+            for r in self.residues:
+                if isinstance(r.id,int):
+                    if r.id == idx:
+                        return r
+                else:
+                    if r.id.replace(" ","")==idx:
+                        return r
+        elif chain is not None:
+            for r in self.chdic[chain].residues:
+                if isinstance(r.id,int):
+                    if r.id == idx:
+                        return r
+                else:
+                    if r.id.replace(" ","")==idx:
+                        return r
+            
+
+    def fetch_residues(self, key, inv=False):
+        """Gets residues using a list of residue names.
+
+        Parameters
+        ----------
+        key : str or list
+            resname
+        inv : bool
+            invert selection. Default is False. If True, it finds all residues
+            with resnames different from those in key.
+
+        Returns
+        -------
+        residues : list
+            list of Molecule instances with the residues
+        """
+        if not hasattr(key, "append"):
+            key = [key]
+        result = []
+        if not inv:
+            for r in self.residues:
+                if r.resname in key:
+                    result.append(r)
+        else:
+            for r in self.residues:
+                if r.resname not in key:
+                    result.append(r)
+        return result
+
+    def al_from_resl(self):
+        self.atoms = []
+        for r in self.residues:
+            for atom in r.atoms:
+                self.atoms.append(atom)
+
+    def resl_from_chains(self):
+        self.residues = []
+        for ch in self.chains:
+            for r in ch.residues:
+                self.residues.append(r)
+
+    def copy(self):
+        return copy.deepcopy(self)
+
+    def get_mol2_types(self):
+        if self.atoms[0].symbol == '':
+            self.get_symbol()
+        for ch in self.chains:
+            ch.get_mol2_types()
+
+    def get_mol2_resname(self):
+        for ch in self.chains:
+            ch.get_mol2_resname()
+
+    def get_nterms(self):
+        nter = []
+        for ch in self.chains:
+            first = ch.residues[0]      # first residue
+            if first.resname in library._one_letter.keys():
+                nter.append(first)
+        return nter
+
+    def get_cterms(self):
+        cter = []
+        for ch in self.chains:
+            last = ch.residues[-1]      # last residue
+            if last.resname in library._one_letter.keys():
+                cter.append(last)
+        return last
+
+    def rename_atoms(self):
+        for c in self.chains:
+            c.rename_atoms()
+
+    def residue(self, idx):
+        return self.residues[idx-1]
+
+    def chain(self, iden):
+        return self.chdic[iden]
+
+
+# ==============================================================================
+#                                  Functions
+# ==============================================================================
+def merge_models(*args):
+    '''Merges the atoms from all Model objects in the list provided. Atoms will
+    be merged based on the order of models in the list.
+
+    Parameters
+    ----------
+    *args :
+        variable length argument containing Model objects.
+
+    Returns
+    -------
+    m : Model
+        new Model object containing all the Models in the list.
+
+    Examples
+    --------
+    >>> newmodel = merge_models(model1, model2, model3)
+    >>> newmodel = merge_models(protein, ligand, cofactor, ions)
+    '''
+    model = Model()
+
+    if not all(m.unity == args[0].unity for m in args):
+        raise ValueError('the Model objects provided do not have the same '
+                         'units - convert units to that they are compatible')
+
+    for m in args:
+        # operate on a deep copy of the model, otherwise changes in the atoms
+        # of the merged model will be reflected in the parent models too
+        m_ = copy.deepcopy(m)
+        for a in m_.atoms:
+            model.atoms.append(a)
+
+    model.unity = model.atoms[0].unity
+    model.make_chains()
+    model.make_residues()
+    model.assign_moltype()
+    return model
+
+
+def assign_masses_to_model(model, topology=None):
+    '''Assigns masses to the Model atoms given the ones present in the Topology.
+
+    Parameters
+    ----------
+    model : Model
+        Model object of the molecule.
+    topology : Topology
+        Topology object of the same molecule. When no topology provided, standard library masses are used.
+    '''
+    
+    if topology!=None:
+        for ma, ta in zip(model.atoms, topology.atoms):
+            if ma.name != ta.name:
+                raise ValueError('mismatch of atom names between Model and '
+                                 'Topology objects provided')
+            ma.m = ta.m
+    else:
+        for a in model.atoms:
+            aname = a.name
+            aname = aname.upper()
+            aname = aname.translate(str.maketrans('','',digits))
+            if aname not in library._atommass.keys():
+                a.m = 0.0
             else:
-                # switch the A state on
-                if a1.atomtype.startswith('DUM') or \
-                   a2.atomtype.startswith('DUM') or \
-                   a3.atomtype.startswith('DUM') or \
-                   a4.atomtype.startswith('DUM'):
-                    if entrB is not None:
-                        dih = gen_dih_entry2(a1,a2,a3,a4,dih_type,None,entrB)
-                        newdihedrals.extend(dih)
-#                        if( (a1.atomtype.startswith('DUM')==False and a2.atomtype.startswith('DUM')==False and a3.atomtype.startswith('DUM')==False) \
-#                           or (a1.atomtype.startswith('DUM')==False and a3.atomtype.startswith('DUM')==False and a4.atomtype.startswith('DUM')==False) \
-#                           or (a2.atomtype.startswith('DUM')==False and a3.atomtype.startswith('DUM')==False and a4.atomtype.startswith('DUM')==False) \
-#                           or (a1.atomtype.startswith('DUM')==False and a2.atomtype.startswith('DUM')==False and a4.atomtype.startswith('DUM')==False) ):
-			if( a1.atomtype.startswith('DUM')==False or a2.atomtype.startswith('DUM')==False \
-			    or a3.atomtype.startswith('DUM')==False or a4.atomtype.startswith('DUM')==False ):
-#                        if( (a1.atomtype.startswith('DUM')==False and a2.atomtype.startswith('DUM')==False) \
-#			    or (a1.atomtype.startswith('DUM')==False and a3.atomtype.startswith('DUM')==False) \
-#			    or (a1.atomtype.startswith('DUM')==False and a4.atomtype.startswith('DUM')==False) \
-#			    or (a2.atomtype.startswith('DUM')==False and a3.atomtype.startswith('DUM')==False) \
-#			    or (a2.atomtype.startswith('DUM')==False and a4.atomtype.startswith('DUM')==False) \
-#			    or (a3.atomtype.startswith('DUM')==False and a4.atomtype.startswith('DUM')==False) ):
-                            if dih_type==2 or dih_type==4:# or dih_type==1: # disable improper for dummy-nondummy
-                                dih = gen_dih_entry2(a1,a2,a3,a4,dih_type,entrB,None,0.0,1.0)
-                            else:
-                                dih = gen_dih_entry2(a1,a2,a3,a4,dih_type,entrB,None,scDumd,1.0)
-		        else:
-                            dih = gen_dih_entry2(a1,a2,a3,a4,dih_type,entrB,None)
-                        newdihedrals.extend(dih)
-                        bOk = True
-                    else:
-                        bOk = False
-		else:
-                    newdihedrals.append(b)
-                    bOk = True
-
-            if not bOk:
-                do_log(logfile, "Error: Something went wrong while assigning dihedrals!")
-                do_log(logfile, "A-> Atom1: %d-%s Atom2: %d-%s Atom3: %d-%s Atom3: %d-%s" \
-                       %(a1.id, a1.name, a2.id, a2.name, a3.id, a3.name, a4.id, a4.name))
-                do_log(logfile, "B-> Atom1: %d-%s Atom2: %d-%s Atom3: %d-%s Atom3: %d-%s" \
-                       %(a1.idB, a1.nameB, a2.idB, a2.nameB, a3.idB, a3.nameB, a4.idB, a4.nameB))
-                do_log(logfile,"Exiting....")
-                sys.exit(1)
-        #############################
-        # COMPLETE DIHEDRAL REWRITE #
-        #############################
-
-
-        # vsites2: stateA
-        newvsites2 = []
-        has_vsites2 = False
-#        if(itp1.vsites2):
-#            for b in itp1.vsites2:
-        if(itp1.virtual_sites2):
-            has_vsites2 = True
-            for b in itp1.virtual_sites2:
-                id1 = b[0].id
-                id2 = b[1].id
-                id3 = b[2].id
-                a1 = m1.atoms[id1-1]
-                a2 = m1.atoms[id2-1]
-                a3 = m1.atoms[id3-1]
-                newvsites2.append(b)
-
-        # vsites3: stateA
-        newvsites3 = []
-        has_vsites3 = False
-        if(itp1.virtual_sites3):
-            has_vsites3 = True
-            for b in itp1.virtual_sites3:
-                id1 = b[0].id
-                id2 = b[1].id
-                id3 = b[2].id
-                id4 = b[3].id
-                a1 = m1.atoms[id1-1]
-                a2 = m1.atoms[id2-1]
-                a3 = m1.atoms[id3-1]
-                a4 = m1.atoms[id4-1]
-                newvsites3.append(b)
-
-        # exclusions: stateA
-        newexclusions = []
-        has_exclusions = False
-        if(itp1.exclusions):
-            has_exclusions = True
-            for excl in itp1.exclusions:
-                exclToAdd = []
-                for ex in excl:
-                    newid = ex.id
-                    newa = m1.atoms[newid-1]
-                    exclToAdd.append(newa)
-                newexclusions.append( exclToAdd )  
-
-	# now we have all parameter for pairs
-	# let's go for the dummies
-	for b in itp2.bonds:
-	    newid1 = id_dicBA[b[0].id]
-	    newid2 = id_dicBA[b[1].id]
-	    a1 = m1.atoms[newid1-1]
-	    a2 = m1.atoms[newid2-1]
-	    if a1.atomtype.startswith('DUM') or \
-	       a2.atomtype.startswith('DUM'):
-		newbonds.append( [a1, a2, 1, [1]+b[-1], [1]+b[-1]] )
-
-	decoupAngles = []
-	for b in itp2.angles:
-            angtype = b[3]
-            entry = b[-1]
-            # for type 1
-            paramA = [ 1,entry[0],0.0 ]
-            paramAscDum = [ 1,entry[0],scDuma*float(entry[1]) ]
-            paramB = [ 1,entry[0],entry[1] ]
-            # for type 5
-            if angtype==5:
-                paramA = [ 5,entry[1],0.0,entry[3],0.0 ]
-                paramAscDum = [ 5,entry[1],scDuma*float(entry[2]),entry[3],scDuma*float(entry[4]) ]
-                paramB = [ 5,entry[1],entry[2],entry[3],entry[4] ]
-
-	    newid1 = id_dicBA[b[0].id]
-	    newid2 = id_dicBA[b[1].id]
-	    newid3 = id_dicBA[b[2].id]
-	    a1 = m1.atoms[newid1-1]
-	    a2 = m1.atoms[newid2-1]
-	    a3 = m1.atoms[newid3-1]
-	    if a1.atomtype.startswith('DUM') or \
-	       a2.atomtype.startswith('DUM') or \
-	       a3.atomtype.startswith('DUM'):
-                if( (a1.atomtype.startswith('DUM')==False and a2.atomtype.startswith('DUM')==False) \
-                   or (a1.atomtype.startswith('DUM')==False and a3.atomtype.startswith('DUM')==False) \
-                   or (a2.atomtype.startswith('DUM')==False and a3.atomtype.startswith('DUM')==False) ):
-#		if( a1.atomtype.startswith('DUM')==False or a2.atomtype.startswith('DUM')==False or a3.atomtype.startswith('DUM')==False ):
-
-                    if(deAng==True):
-                        if( a1.atomtype.startswith('DUM')==True ):
-                            if( findIDinList(newid1,decoupAngles)==True ):
-                                newangles.append([ a1,a2,a3,angtype, paramA, paramB ])
-                            else:
-                                newangles.append([ a1,a2,a3,angtype, paramAscDum, paramB ])
-                                decoupAngles.append(newid1)
-                        elif( a2.atomtype.startswith('DUM')==True ):
-                            if( findIDinList(newid2,decoupAngles)==True ):
-                                newangles.append([ a1,a2,a3,angtype, paramA, paramB ])
-                            else:
-                                newangles.append([ a1,a2,a3,angtype, paramAscDum, paramB ])
-                                decoupAngles.append(newid2)
-                        elif( a3.atomtype.startswith('DUM')==True ):
-                            if( findIDinList(newid3,decoupAngles)==True ):
-                                newangles.append([ a1,a2,a3,angtype, paramA, paramB ])
-                            else:
-                                newangles.append([ a1,a2,a3,angtype, paramAscDum, paramB ])
-                                decoupAngles.append(newid3)
-		    else:
-                        newangles.append([ a1,a2,a3,angtype, paramAscDum, paramB ])
-		else:
-                    newangles.append([ a1,a2,a3,angtype, paramB, paramB ])
-
-	# dihedrals already accounted for both states
-#	cpcpItp2 = xcopy.deepcopy(cpItp2) # dirty hack
-#	for b in cpcpItp2.dihedrals:
-#	    newid1 = id_dicBA[b[0]]
-#	    newid2 = id_dicBA[b[1]]
-#	    newid3 = id_dicBA[b[2]]
-#	    newid4 = id_dicBA[b[3]]
-#	    a1 = m1.atoms[newid1-1]
-#	    a2 = m1.atoms[newid2-1]
-#	    a3 = m1.atoms[newid3-1]
-#	    a4 = m1.atoms[newid4-1]
-#	    dih_type = b[4]
-#	    entrB = get_ff_entry([b[0],b[1],b[2],b[3], dih_type], cpItp2, gmx45, what='dihedral')
-#	    if a1.atomtype.startswith('DUM') or \
-#	       a2.atomtype.startswith('DUM') or \
-#	       a3.atomtype.startswith('DUM') or \
-#	       a4.atomtype.startswith('DUM'):
-#		newdihedrals.append( [newid1, newid2, newid3, newid4, b[4]] + b[5:] + b[5:] )
-#                dih = gen_dih_entry([newid1, newid2, newid3, newid4, dih_type],None,entrB)
-#		newdihedrals.extend(dih)
-
-        # vsites2: stateB
-        if(itp2.virtual_sites2):
-            has_vsites2 = True
-            for b in itp2.virtual_sites2:
-                newid1 = id_dicBA[b[0].id]
-                newid2 = id_dicBA[b[1].id]
-                newid3 = id_dicBA[b[2].id]
-                #VG: this is not tested, use with caution
-#               print "UNTESTED PART FOR THE NEW PMX %s %s %s" %(newid1,newid2,newid3)
-#                newid1 = id_dicBA[b[0]]
-#                newid2 = id_dicBA[b[1]]
-#                newid3 = id_dicBA[b[2]]
-                a1 = m1.atoms[newid1-1]
-                a2 = m1.atoms[newid2-1]
-                a3 = m1.atoms[newid3-1]
-                vsiteToAdd = [a1,a2,a3,b[3],b[4]]
-                if( check_if_vsite2_exists( newvsites2, vsiteToAdd )==False ):
-                    newvsites2.append( [a1, a2, a3, b[3], b[4]] )
-#                newvsites2.append( [newid1, newid2, newid3, b[3], b[4]] )
-
-        # vsites3: stateB
-        if(itp2.virtual_sites3):
-            has_vsites3 = True
-            for b in itp2.virtual_sites3:
-                newid1 = id_dicBA[b[0].id]
-                newid2 = id_dicBA[b[1].id]
-                newid3 = id_dicBA[b[2].id]
-                newid4 = id_dicBA[b[3].id]
-                a1 = m1.atoms[newid1-1]
-                a2 = m1.atoms[newid2-1]
-                a3 = m1.atoms[newid3-1]
-                a4 = m1.atoms[newid4-1]
-                vsiteToAdd = [a1,a2,a3,a4,b[4],b[5]]
-                if( check_if_vsite3_exists( newvsites3, vsiteToAdd )==False ):
-                    newvsites3.append( [a1, a2, a3, a4, b[4], b[5]] )
-
-        # exclusions: stateB
-        if(itp2.exclusions):
-            has_exclusions = True
-            for excl in itp2.exclusions:
-                exclToAdd = []
-                for ex in excl:
-                    newid = id_dicBA[ex.id]
-                    newa = m1.atoms[newid-1]
-                    exclToAdd.append(newa)
-                if( check_if_exclusion_valid( newexclusions, exclToAdd )==True ):
-                    newexclusions.append( exclToAdd )  
-
-	# make pairs
-	newpairs = []
-	pp = []
-	for p in itp1.pairs:
-	    newpairs.append( p )
-	    pp.append( (p[0].id,p[1].id) )
-	for p in itp2.pairs:
-	    newid1 = id_dicBA[p[0].id]
-	    newid2 = id_dicBA[p[1].id]
-            a1 = m1.atoms[newid1-1]
-            a2 = m1.atoms[newid2-1]
-	    if (newid1, newid2) not in pp and \
-	       (newid2, newid1) not in pp:
-		newpairs.append([ a1, a2, 1] )
-
-	do_log(logfile, "Generating new itp file")    
-		
-	newitp = ITPFile(filename=None)
-	newitp.name = itp1.name
-        newitp.nrexcl = itp1.nrexcl
-	newitp.atoms = m1.atoms
-        newitp.residues = m1.residues
-	for i, atom in enumerate(newitp.atoms):
-	    atom.cgnr = i +1
-	newitp.bonds = newbonds
-	newitp.pairs = newpairs
-	newitp.angles = newangles
-	newitp.dihedrals = newdihedrals
-        newitp.virtual_sites2 = newvsites2
-        newitp.has_vsites2 = has_vsites2
-        newitp.virtual_sites3 = newvsites3
-        newitp.has_vsites3 = has_vsites3
-        newitp.exclusions = newexclusions
-        newitp.has_exclusions = has_exclusions
-        # get charges
-        qA, qB = sum_charge_of_states( newitp )
-        qA_mem = xcopy.deepcopy( qA )
-        qB_mem = xcopy.deepcopy( qB )
-
-	do_log(logfile, 'Writing new itp file: "%s"' % cmdl['-oitp'])    
-	newitp.write(cmdl['-oitp'], target_qB = qB)
-	#do_log(logfile, 'Writing new structure file: "%s"' % args['-o']['fns'])    
-	#m1.write(args['-o'])
-	do_log(logfile, 'Writing dummy forcefield file: "%s"' % cmdl['-ffitp'])    
-
-        if bSplit==True: # write splitted topology
-            root, ext = os.path.splitext(cmdl['-oitp'])
-            out_file_qoff = root+'_qoff'+ext
-            out_file_vdw = root+'_vdw'+ext
-            out_file_qon = root+'_qon'+ext
-
-
-            print '------------------------------------------------------'
-            print 'log_> Creating splitted topologies............'
-            print 'log_> Making "qoff" topology : "%s"' % out_file_qoff
-            contQ = xcopy.deepcopy(qA_mem)
-            newitp.write( out_file_qoff, stateQ = 'AB', stateTypes = 'AA', dummy_qB='off',
-                          scale_mass = bScaleMass, target_qB = qA, stateBonded = 'AA', full_morphe = False )
-            print 'log_> Charge of state A: %g' % newitp.qA
-            print 'log_> Charge of state B: %g' % newitp.qB
-
-            print '------------------------------------------------------'
-            print 'log_> Making "vdw" topology : "%s"' % out_file_vdw
-            contQ = xcopy.deepcopy(qA_mem)
-            newitp.write( out_file_vdw, stateQ = 'BB', stateTypes = 'AB', dummy_qA='off', dummy_qB = 'off',
-                          scale_mass = bScaleMass, target_qB = contQ, stateBonded = 'AB' , full_morphe = False)
-            print 'log_> Charge of state A: %g' % newitp.qA
-            print 'log_> Charge of state B: %g' % newitp.qB
-            print '------------------------------------------------------'
-
-            print 'log_> Making "qon" topology : "%s"' % out_file_qon
-            newitp.write( out_file_qon, stateQ = 'BB', stateTypes = 'BB', dummy_qA='off', dummy_qB = 'on',
-                          scale_mass = bScaleMass, target_qB = qB_mem,  stateBonded = 'BB' , full_morphe = False)
-            print 'log_> Charge of state A: %g' % newitp.qA
-            print 'log_> Charge of state B: %g' % newitp.qB
-            print '------------------------------------------------------'
-
-
-	# write ffitp
-	fp = open(cmdl['-ffitp'],'w')
-	dd = []
-	print >>fp, '[ atomtypes ]'
-	for atom in m1.atoms:
-	    if atom.atomtype.startswith('DUM') and atom.atomtype not in dd:
-		print >>fp, '%8s %12.6f %12.6f %3s %12.6f %12.6f' % \
-		      (atom.atomtype, 0, 0, 'A',0,0)
-		dd.append(atom.atomtype)
-	    elif atom.atomtypeB.startswith('DUM') and atom.atomtypeB not in dd:
-		print >>fp, '%8s %12.6f %12.6f %3s %12.6f %12.6f' % \
-		      (atom.atomtypeB, 0, 0, 'A',0,0)
-		dd.append(atom.atomtypeB)
-
-	# write merged pdb
-	m1.write(cmdl['-oa'])
-	m3.write(cmdl['-ob'])
+                a.m = library._atommass[aname]
+
+def double_box(m1, m2, r=2.5, d=1.5, bLongestAxis=False, verbose=False):
+    '''Places two structures (two Model objects) into a single box.
+    The box is a rectangular cuboid in which the two structures are placed in
+    such a way to minimise the box volume.
+
+    Parameters
+    ----------
+    m1 : Model
+        first structure.
+    m2 : Model
+        first structure.
+    r : float
+        distance between the two structures (nm).
+    d : float
+        distance to the box wall (nm).
+    bLongestAxis : bool
+        whether to just place structures along the
+        longest axis, rather then optimising the placement and minimising
+        the volume.
+    verbose : bool
+        whether to print out information about the new box or not.
+
+    Returns
+    -------
+    mout : Model
+        new Model object where the two input structures are placed within a
+        single box.
+    '''
+
+    def _translate(m, v, fact=1.0):
+        for a in m.atoms:
+            a.x[0] = a.x[0] + fact*v[0]
+            a.x[1] = a.x[1] + fact*v[1]
+            a.x[2] = a.x[2] + fact*v[2]
+
+    def _get_mass(a):
+        aname = ''.join(i for i in a.name if not i.isdigit())
+        if aname.startswith('Br') or aname.startswith('BR'):
+            return(library._atommass['BR'])
+        elif aname.startswith('Cl') or aname.startswith('CL'):
+            return(library._atommass['CL'])
+        elif aname.startswith('D'):
+            return(library._atommass[aname[1]])
+        else:
+            return(library._atommass[aname[0]])
+        return(1.0)
+
+    def _principal_axes(m):
+        tensor = np.matrix([[0.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]])
+        for a in m.atoms:
+            if ('HOH' in a.resname) or ('SOL' in a.resname) or ('WAT' in a.resname):
+                continue
+            mass = _get_mass(a)
+            tensor[0,0] += mass*(np.power(a.x[1], 2) + np.power(a.x[2], 2))
+            tensor[1,1] += mass*(np.power(a.x[0], 2) + np.power(a.x[2], 2))
+            tensor[2,2] += mass*(np.power(a.x[0], 2) + np.power(a.x[1], 2))
+            tensor[0,1] -= mass*a.x[0]*a.x[1]
+            tensor[1,0] = tensor[0, 1]
+            tensor[0,2] -= mass*a.x[0]*a.x[2]
+            tensor[2,0] = tensor[0, 2]
+            tensor[1,2] -= mass*a.x[1]*a.x[2]
+            tensor[2,1] = tensor[1, 2]
+        evals, evecs = np.linalg.eig(tensor)
+        idx = evals.argsort()[::1] # sort descending, because later the rotation matrix will be calculated as transpose
+        evals = evals[idx]
+        evecs = evecs[:, idx]
+        # check if one axis needs to be flipped
+        crossprod = np.cross(np.transpose(evecs[:,0]), np.transpose(evecs[:,1]))
+        dotprod = np.dot(np.transpose(evecs[:,2]), np.transpose(crossprod))
+        if dotprod < 0.0:
+            evecs[:,2] *= -1.0
+        rotmat = np.transpose(evecs)
+        return(rotmat)
+
+    def _rotate(atoms, R):
+        for atom in atoms:
+            x_old = list(map(lambda x: x, atom.x))
+            for i in range(3):
+                atom.x[i] = 0.0
+                for j in range(3):
+                    atom.x[i] += x_old[j]*R[i,j]
+
+    def _get_com_radius(m):
+        com = [0.0, 0.0, 0.0]
+        radius = 0.0
+        mass = 0.0
+
+        # com
+        for a in m.atoms:
+            a.a2nm()
+            if ('HOH' in a.resname) or ('SOL' in a.resname) or ('WAT' in a.resname):
+                continue
+            aname = a.name[0]
+            if aname.isdigit():
+                aname = a.name[1]
+            amass = _get_mass(a)
+
+            com[0] += a.x[0]*amass
+            com[1] += a.x[1]*amass
+            com[2] += a.x[2]*amass
+            mass += amass
+
+        com[0] /= mass
+        com[1] /= mass
+        com[2] /= mass
+
+        # radius
+        for a in m.atoms:
+            if ('HOH' in a.resname) or ('SOL' in a.resname) or ('WAT' in a.resname):
+                continue
+            foo = (a.x[0]-com[0])**2 + (a.x[1]-com[1])**2 + (a.x[2]-com[2])**2
+            if foo > radius:
+                radius = foo
+        radius = np.sqrt(radius)
+
+        return(com, radius)
+
+    def _get_rect_dist(m):
+        minx = 9999.999
+        maxx = -9999.999
+        miny = 9999.999
+        maxy = -9999.999
+        minz = 9999.999
+        maxz = -9999.999
+        for a in m.atoms:
+            if ('HOH' in a.resname) or ('SOL' in a.resname) or ('WAT' in a.resname):
+                continue
+            if a.x[0] < minx:
+                minx = a.x[0]
+            if a.x[0] > maxx:
+                maxx = a.x[0]
+            if a.x[1] < miny:
+                miny = a.x[1]
+            if a.x[1] > maxy:
+                maxy = a.x[1]
+            if a.x[2] < minz:
+                minz = a.x[2]
+            if a.x[2] > maxz:
+                maxz = a.x[2]
+        a = maxx-minx
+        b = maxy-miny
+        c = maxz-minz
+        return (a, b, c)
+
+    def _get_extr(m, i=0):
+        minx = 9999.999
+        maxx = -9999.999
+        for a in m.atoms:
+            if ('HOH' in a.resname) or ('SOL' in a.resname) or ('WAT' in a.resname):
+                continue
+            if a.x[i] < minx:
+                minx = a.x[i]
+            if a.x[i] > maxx:
+                maxx = a.x[i]
+        return(minx, maxx)
+
+    def _translate_sticking_out(m, l, i=0):
+        minx = 0.0
+        maxx = 0.0
+        for a in m.atoms:
+            if ('HOH' in a.resname) or ('SOL' in a.resname) or ('WAT' in a.resname):
+                continue
+            if a.x[i] < minx:
+                minx = a.x[i]
+            if (a.x[i]-l) > maxx:
+                maxx = a.x[i]-l
+        return(-1.0*(minx+maxx))
+
+    # ====
+    # Main
+    # ====
+
+    # com and radii
+    com1, rad1 = _get_com_radius(m1)
+    com2, rad2 = _get_com_radius(m2)
+
+    # remove COM from the systems
+    _translate(m1, com1, fact=-1.0)
+    _translate(m2, com2, fact=-1.0)
+
+    # if needed, calculate principal axes
+    if bLongestAxis:
+        princRot1 = _principal_axes(m1)
+        princRot2 = _principal_axes(m2)
+        _rotate(m1.atoms, princRot1)
+        _rotate(m2.atoms, princRot2)
+        a_rect1, b_rect1, c_rect1 = _get_rect_dist(m1)
+        a_rect2, b_rect2, c_rect2 = _get_rect_dist(m2)
+
+    # estimate cube's edge for the larger structure
+    a_cube = 0.0
+    if rad1 > rad2:
+        a_cube = 2*rad1+2*d
+    else:
+        a_cube = 2*rad2+2*d
+    if bLongestAxis is True:
+        a_rect = a_rect1 + a_rect2 + r + 2.0*d
+        b_rect = b_rect1 + b_rect2 + 2.0*d
+        c_rect = c_rect1 + c_rect2 + 2.0*d
+        if verbose is True:
+            print("Cuboid dimensions (nm): ", np.round(a_rect), np.round(b_rect), np.round(c_rect, 2))
+    else:
+        if verbose is True:
+            print("Cube's edge (nm): ", np.round(a_cube, 2))
+
+    # cube's diagonal
+    if bLongestAxis is True:
+        d_cube = np.sqrt(np.power(a_rect, 2) + np.power(b_rect, 2) + np.power(c_rect, 2))
+        if verbose is True:
+            print("Cuboid's diagonal (nm): ", np.round(d_cube, 2))
+    else:
+        d_cube = a_cube*np.sqrt(3.0)
+        if verbose is True:
+            print("Cube's diagonal (nm): ", np.round(d_cube, 2))
+
+    # check if cube is enough
+    if bLongestAxis is True:
+        a_box = a_rect
+        b_box = b_rect
+        c_box = c_rect
+    else:
+        dist_cube = d_cube - 2.0*rad1 - 2.0*rad2 - r - 2.0*d
+        a_box = a_cube
+        b_box = a_cube
+        c_box = a_cube
+        if dist_cube > 0.0:
+            if verbose is True:
+                print("Having a cube with the diagonal ", np.round(d_cube, 2), "nm is good enough")
+        else:
+            if verbose is True:
+                print("Need to extend the cube")
+            d_rect = 2.0*rad1 + 2.0*rad2 + r + 2.0*d
+            delta_a_cube = -a_cube + np.sqrt(d_rect**2 - 2.0*a_cube**2)
+            a_box = a_cube + delta_a_cube
+            if verbose is True:
+                print("Rectangle's edge (nm): ", np.round(a_box, 2))
+
+    # translate the larger structure to the middle of the box
+    if rad1 > rad2:
+        # translate smaller to (0,b/2,c/2) and larger to (maxx2+dist+abs(minx2),b/2,c/2)
+        if bLongestAxis is True:
+            _translate(m2, [0.0, b_box/2.0, c_box/2.0])
+            minx1, maxx1 = _get_extr(m1, 0)
+            minx2, maxx2 = _get_extr(m2, 0)
+            _translate(m1, [maxx2+r+abs(minx1), b_box/2.0, c_box/2.0])
+        else:
+            _translate(m1, [a_box/2.0, b_box/2.0, c_box/2.0])
+    else:
+        if bLongestAxis is True:
+            _translate(m1, [0.0, b_box/2.0, c_box/2.0])
+            minx1, maxx1 = _get_extr(m1, 0)
+            minx2, maxx2 = _get_extr(m2, 0)
+            _translate(m2, [maxx1 + r + abs(minx2), b_box/2.0, c_box/2.0])
+        else:
+            _translate(m2, [a_box/2.0, b_box/2.0, c_box/2.0])
+
+    # create an output
+    mout = m1
+    chainList = []
+    for ch in m1.chains:
+        if ch.id not in chainList:
+            chainList.append(ch.id)
+    chainIDstring = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
+    chainIDchanges = {}
+    for ch in m2.chains:
+        if ch.id in chainList:
+            # pick a new chain ID
+            bFound = False
+            while bFound is False:
+                foo = chainIDstring[0]
+                chainIDstring = chainIDstring.lstrip(chainIDstring[0])
+                if foo not in chainList:
+                    bFound = True
+            chainList.append(foo)
+            chainIDchanges[ch.id] = foo
+    for a in m2.atoms:
+        chID = a.chain_id
+        if chID in chainIDchanges:
+            a.chain_id = chainIDchanges[chID]
+    mout.atoms.extend(m2.atoms)
+
+    # create the box
+    mout.box = [[a_box,0.0,0.0], [0.0,b_box,0.0], [0.0,0.0,c_box]]
+
+    # determine translation exactly by checking how much the atoms are sticking out
+    xtransl = _translate_sticking_out(mout, a_box, 0)
+    ytransl = _translate_sticking_out(mout, b_box, 1)
+    ztransl = _translate_sticking_out(mout, c_box, 2)
+    # increase translation by a factor 1.01 to move a bit further from walls
+    _translate(mout, [1.01*xtransl, 1.01*ytransl, 1.01*ztransl])
+
+    # volume
+    V = a_box*b_box*c_box
+    if verbose is True:
+        print("Volume: ", np.round(V, 2), "nm^3")
 
-main( sys.argv )
+    return mout
```

### Comparing `pmx_biobb-4.0.2/src/pmx/scripts/md_setup.py` & `pmx_biobb-4.1.2/src/pmx/scripts/md_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,30 +48,30 @@
         print >>sys.stderr, 'Output written to %s'  % os.path.abspath(os.path.join('.',err_file))
         fp = open(err_file,'w')
         print >>fp, s
         print >>fp, out
         fp.close()
         sys.exit(1)
     else:
-        print("%-90s" % s, ': ok')
+        print "%-90s" % s, ': ok'
 
 chain_ids = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
 
 class MD:
 
     def __init__(self, **kwargs):
 
         self.ff = 'amber99sbmut'
-        self.water = 'tip3p'
+        self.water = 'tip3p' 
         self.conc = .15
         self.box_type = 'triclinic'
         self.box_size = 1.2
         self.vsite = False
         self.princ = False
-        self.md_in_conf = 'md_in.pdb'
+        self.md_in_conf = 'md_in.pdb' 
 
         for key, val in kwargs.items():
             setattr(self,key,val)
 
     def setup(self):
         self.generate_topology( self.pdb_in)
         self.renumber_pdb( )
@@ -104,129 +104,129 @@
             if chain.id != ' ':
                 for r in chain.residues:
                     r.old_chain_id = chain.id
                 chain.set_chain_id( chain_ids[i] )
         self.write_residue_map( m )
         m.write('start.pdb')
         self.pdb_in = 'start.pdb'
-
+        
     def __str__(self):
         s = '< MD (%s) > ' % self.pdb_in
         return s
 
     def clean_backups(self):
         files = glob('#*#')
         for f in files:
             os.unlink(f)
-
+    
     def generate_topology(self, pdb_in):
-
+    
         run = 'pdb2gmx -f %s -water %s -ff %s -o gmx.pdb ' % ( pdb_in, self.water, self.ff )
         if self.vsite:
             run+=' -vsite hydrogens'
         run_command( self.generate_topology, run )
 
     def generate_sim_box(self ):
         if self.princ:
             run = 'echo 4 | editconf -f gmx.pdb -o tmp.pdb -c -princ '
             run_command( run_editconf, run)
             run = 'editconf -f tmp.pdb -o ed.pdb -d %g -bt %s ' % (self.box_size, self.box_type)
             run_command( generate_sim_box, run)
         else:
             run = 'editconf -f gmx.pdb -o ed.pdb -d %g -bt %s ' % (self.box_size, self.box_type)
             run_command( self.generate_sim_box, run)
-
+    
     def fill_sim_box(self ):
         if self.water == 'spce': water = 'spc216'
         else: water = self.water
         run = 'genbox -cp ed.pdb -cs %s -p -o box.pdb' % os.path.join(ff_path,water)
         run_command( self.fill_sim_box, run)
-
+    
     def tpr_from_box(self):
         run = 'grompp -f ~/mdp/em.mdp -c box.pdb'
         run_command( self.tpr_from_box, run)
 
     def get_solvent_index(self ):
         run = 'echo q | make_ndx -f topol.tpr -o tmp.ndx'
         run_command( self.get_solvent_index, run)
         ndx = IndexFile("tmp.ndx")
         return ndx.names.index('SOL')
-
+    
     def add_ions(self ):
         idx = self.get_solvent_index()
         run = 'echo %d | genion  -conc %g -neutral -p -o ion.pdb' % (idx, self.conc)
         run_command( self.add_ions, run)
-
+    
     def make_em_tpr(self):
         run = 'grompp -f ~/mdp/em.mdp -c ion.pdb'
         run_command( self.make_em_tpr, run)
-
+    
     def run_em(self):
         run = 'mdrun -v -c em.pdb'
         run_command( self.run_em, run)
-
+    
     def pdb_from_em(self):
-        run = 'echo 0| trjconv -f em.pdb -s topol.tpr -o min.pdb'
+        run = 'echo 0| trjconv -f em.pdb -s topol.tpr -o min.pdb' 
         run_command( self.pdb_from_em, run)
-
+    
     def compact_repr(self, pdb_in, pdb_out ):
         run = 'echo 0 | trjconv -f %s -s topol.tpr -ur compact -pbc mol -o %s' % (pdb_in, pdb_out)
         run_command( self.compact_repr, run)
-
+    
 
 
 class FreeEnergyMD(MD):
 
     def __init__(self, mutation_file, **kwargs):
 
         MD.__init__( self )
-
+        
         for key, val in kwargs.items():
             setattr(self,key,val)
         self.mutation_tags = []
         self.read_mutation_file( mutation_file )
         self.mutations = []
         if self.mutation_tags:
             self.mutations_from_tags()
         self.runs = []
         self.is_single_chain = False
-
+        
     def read_mutation_file(self, mut_file ):
-        print('\n\t\t\tReading mutation file: %s\n' % mut_file)
+        print '\n\t\t\tReading mutation file: %s\n' % mut_file
         l = open(mut_file).readlines()
         count = 1
         for line in l:
             entr = line.strip()
             if entr:
-                print('\t\t\t (%d) ->  %s' % (count, entr))
+                print '\t\t\t (%d) ->  %s' % (count, entr)
                 self.mutation_tags.append( entr )
                 count+=1
-
+        
 
     def setup(self):
         self.read_pdb()
-        print('\n\n')
+        print '\n\n'
         for m in self.mutations:
             self.setup_mutation_run(m)
 
     def read_pdb( self ):
         self.model = Model(self.md_in_conf)
         if len(self.model.chains) == 1:
             self.is_single_chain = True
-
+            
     def mutations_from_tags(self):
         for t in self.mutation_tags:
             mut = t.split()
             new_mut = []
             for m in mut:
                 resid, resn, chain = m.split('|')
                 resid = int(resid)
                 new_mut.append( ( resid, resn, chain ) )
             self.mutations.append( new_mut )
-
+    
     def setup_mutation_run(self, mutation ):
         muts = []
         affected_chains = []
         for m in mutation:
             resid, resn, chain = m
             residue = self.model.residues[resid-1]
             resname = _one_letter[residue.resname]
@@ -234,50 +234,50 @@
             if chain not in affected_chains:
                 affected_chains.append( chain )
         name = '-'.join(muts)
         if str(self.__class__).split('.')[1] == 'DiscreteTI':
             name+='.dti'
         elif str(self.__class__).split('.')[1] == 'CrooksMD':
             name+='.crooks'
-        print('\n\t\t\tPreparing mutation run -> %s \n' % name)
+        print '\n\t\t\tPreparing mutation run -> %s \n' % name
         if os.path.isdir( name ):
             shutil.rmtree(name)
         os.mkdir(name)
         self.runs.append( name )
         shutil.copy(self.md_in_conf, name)
         script_file = os.path.join(name,'mutations.txt')
         fp = open(script_file,'w')
         for m in mutation:
             resid, resn, chain = m
             print >>fp, resid, resn
         fp.close()
         self.make_mutation(name, affected_chains)
 
-
+        
     def make_mutation(self, path, affected_chains ):
         os.chdir(path)
         run = '~/software/pmx/scripts/mutate_beta45.py -f %s -script mutations.txt -o mut.pdb' % self.md_in_conf
         run_command( self.make_mutation, run )
         self.generate_topology( 'mut.pdb')
         if self.is_single_chain:
-            itp_file = 'topol_Protein.itp'
+            itp_file = 'topol_Protein.itp' 
             run = '~/software/pmx/scripts/make_bstate_beta45.py -itp %s' % itp_file
             run_command( self.make_mutation, run )
             shutil.move(itp_file, itp_file+'.save')
             shutil.move('newtop.itp', itp_file)
         else:
             for chain in affected_chains:
-                print('Applying changes to topology of chain %s' % chain)
+                print 'Applying changes to topology of chain %s' % chain
                 itp_file = 'topol_Protein_chain_%s.itp' % chain
                 run = '~/software/pmx/scripts/make_bstate_beta45.py -itp %s' % itp_file
                 run_command( self.make_mutation, run )
                 shutil.move(itp_file, itp_file+'.save')
                 shutil.move('newtop.itp', itp_file)
-        os.chdir('..')
-
+        os.chdir('..')            
+        
 
 class CrooksMD( FreeEnergyMD ):
 
     def __init__(self, mutation_file, **kwargs):
         FreeEnergyMD.__init__(self, mutation_file)
         for key, val in kwargs.items():
             setattr(self,key,val)
@@ -285,34 +285,34 @@
 
     def do_crooks( self, mdp_file, min_mdp_file, time, nruns ):
         mdp = MDP().read( mdp_file)
         min_mdp = MDP().read( min_mdp_file)
         self.prepare_min_mdp_files(min_mdp, time )
         self.prepare_eq_mdp_files(mdp, time )
         for r in self.runs:
-            print('\n\t\t\tSetting up Crooks run -> %s\n' % r)
+            print '\n\t\t\tSetting up Crooks run -> %s\n' % r
 
             self.minimize_states( r )
             self.setup_equilibration_runs( r, nruns )
-
+        
     def minimize_states( self, path ):
 
         os.chdir(path)
         run = 'grompp -f ../crooks_minA.mdp -c gmx.pdb -o minA.tpr'
         run_command( self.minimize_states, run )
         run = 'grompp -f ../crooks_minB.mdp -c gmx.pdb -o minB.tpr'
         run_command( self.minimize_states, run )
-        print('\n\t\t\tRunning energy minimization on %s ( state A ) \n' % ( path ))
+        print '\n\t\t\tRunning energy minimization on %s ( state A ) \n' % ( path )
         run = 'mdrun -v -c emA.pdb -s minA.tpr'
         run_command( self.minimize_states, run )
-        print('\n\t\t\tRunning energy minimization on %s ( state B ) \n' % ( path ))
+        print '\n\t\t\tRunning energy minimization on %s ( state B ) \n' % ( path )
         run = 'mdrun -v -c emB.pdb -s minB.tpr'
         run_command( self.minimize_states, run )
         os.chdir('..')
-
+        
     def prepare_eq_mdp_files( self, mdp, time ):
         nsteps = 1000*time/.002
         mdp['nsteps'] = nsteps
         mdp['init-lambda'] = 0
         fp = open('crooks_eqA.mdp','w')
         print >>fp, mdp
         fp.close()
@@ -327,19 +327,19 @@
         print >>fp, mdp
         fp.close()
         mdp['init-lambda'] = 1
         fp = open('crooks_minB.mdp','w')
         print >>fp, mdp
         fp.close()
 
-
+        
     def setup_equilibration_runs( self, path, nruns ):
         os.chdir(path)
         for i in range(nruns):
-            print('\n\t\t\tPreparing run input file for  %s ( run %d ) \n' % ( path, i ))
+            print '\n\t\t\tPreparing run input file for  %s ( run %d ) \n' % ( path, i )
             os.mkdir('runA.%d' % i)
             os.mkdir('runB.%d' % i)
             run = 'grompp -f ../crooks_eqA.mdp -c emA.pdb -o runA.%d/topol.tpr' % i
             run_command( self.setup_equilibration_runs, run )
             run = 'grompp -f ../crooks_eqB.mdp -c emB.pdb -o runB.%d/topol.tpr' % i
             run_command( self.setup_equilibration_runs, run )
             self.clean_backups()
@@ -348,15 +348,15 @@
 
 class DiscreteTI( FreeEnergyMD ):
 
     def __init__(self, mutation_file, **kwargs):
         FreeEnergyMD.__init__(self, mutation_file)
         for key, val in kwargs.items():
             setattr(self,key,val)
-
+        
     def read_lambda_steps( self, filename ):
         l = open(filename).readlines()
         self.lambda_steps = []
         for line in l:
             entr = line.strip()
             if entr:
                 self.lambda_steps.append( float(entr) )
@@ -382,36 +382,36 @@
     def setup_runs( self, path ):
         os.chdir( path )
         for lda in self.lambda_steps:
             min_mdp = 'dti_min_%4.3f.mdp' % round(lda,3)
             run_mdp = 'dti_%4.3f.mdp' % round(lda,3)
             run_dir = 'run_%4.3f' % round(lda,3)
             os.mkdir( run_dir )
-            print('\n\t\t\tRunning energy minimization on %s/%s \n' % ( path, run_dir ))
+            print '\n\t\t\tRunning energy minimization on %s/%s \n' % ( path, run_dir )
             run = 'grompp -f ../%s -c gmx.pdb -o %s/em.tpr' % (min_mdp, run_dir )
             run_command( self.setup_runs, run )
             os.chdir( run_dir )
             run = 'mdrun -v -c em.pdb -s em.tpr'
             run_command( self.setup_runs, run )
             os.chdir('..')
-            print('\n\t\t\tPreparing run input file for  %s/%s \n' % ( path, run_dir ))
+            print '\n\t\t\tPreparing run input file for  %s/%s \n' % ( path, run_dir )
             run = 'grompp -f ../%s -c %s/em.pdb -o %s/topol.tpr' % (run_mdp, run_dir, run_dir )
             run_command( self.setup_runs, run )
             self.clean_backups()
         os.chdir( '..')
-
+        
     def do_dti( self, mdp, min_mdp, time ):
         self.prepare_dti_min_mdp_files( min_mdp)
         self.prepare_dti_mdp_files( mdp, time)
         for r in self.runs:
-            print('\n\t\t\tSetting up Discrete TI run -> %s\n' % r)
+            print '\n\t\t\tSetting up Discrete TI run -> %s\n' % r
             self.setup_runs( r )
 
 
-
+        
 def main(argv):
 
     version = "1.0"
 
     options = [
         Option( "-water", "string", "tip3p", "water model"),
         Option( "-box_type", "string", "triclinic", "box geometry (triclinic, octahedron, dodecahedron)"),
@@ -421,30 +421,30 @@
         Option( "-fe.dti", "bool", False, "do discrete TI setup"),
         Option( "-dti_run_time", "float", 10., "Simulation time [ns] at each lambda point"),
         Option( "-fe.crooks", "bool", False, "do Crooks setup"),
         Option( "-n_crooks_runs", "int", 1, "setup # crooks runs for each mutation"),
         Option( "-crooks_run_time", "float", 50., "Simulation time [ns] for crooks equilibrium runs"),
         Option( "-skip_md_setup", "bool", False, "skip md setup and use -f as starting configuration for free energy runs"),
         ]
-
+    
     files = [
         FileOption("-f", "r",["pdb"],"protein", "input pdb file"),
         FileOption("-m", "r/o",["txt"],"mutations", "mutations to make"),
         FileOption("-crooks_mdp", "r/o",["mdp"],"template", "template run mdp file for crooks equilibrium runs"),
         FileOption("-dti_mdp", "r/o",["mdp"],"template", "template run mdp file for discrete TI calculations"),
         FileOption("-min_mdp", "r/o",["mdp"],"em", "template minimization mdp file ( for TI or Crooks )"),
         FileOption("-lambda_steps", "r/o",["txt"],"lambda_steps", "text file with lambda steps for DTI runs"),
         ]
-
-
-
+    
+    
+    
     help_text = ("Script for setting up plain MD runs",
                  )
 
-
+    
     cmdl = Commandline( argv, options = options,
                         fileoptions = files,
                         program_desc = help_text,
                         check_for_existing_files = False, version = version)
 
 
     # make some basic checks
@@ -459,36 +459,36 @@
             sys.exit(1)
         if cmdl['-fe.dti']: # require lambda steps
             try:
                 open(cmdl['-lambda_steps']).readlines()
             except:
                 print >>sys.stderr, 'Error: Cannot open %s' % cmdl['-lambda_steps']
                 sys.exit(1)
-
+            
 
 
     pdb_in = cmdl['-f']
     water = cmdl['-water']
     box_type = cmdl['-box_type']
     box_size = cmdl['-box_size']
     conc = cmdl['-conc']
     free_energy_start_pdb = None
     bVsite = cmdl['-vsite']
     if bVsite and bFreeEnergy:
-        print >>sys.stderr, 'Error: Cannot use virtual sites in free energy calculations !'
+        print >>sys.stderr, 'Error: Cannot use virtual sites in free energy calculations !' 
         sys.exit(1)
-
+        
 
     if not cmdl['-skip_md_setup']:
         md = MD( pdb_in = pdb_in, water = water, conc = conc, box_type = box_type, box_size = box_size )
         md.setup()
         free_energy_start_pdb = md.md_in_conf
     else:
         if not bFreeEnergy:
-            print('Nothing to do........... (no MD, no Free Energy)')
+            print 'Nothing to do........... (no MD, no Free Energy)'
             sys.exit()
     if bFreeEnergy:
         if not free_energy_start_pdb:
             free_energy_start_pdb = pdb_in
         if cmdl['-fe.crooks']:
             crooksMD = CrooksMD( mutation_file, md_in_conf = free_energy_start_pdb)
             crooksMD.setup()
@@ -497,50 +497,50 @@
         if cmdl['-fe.dti']:
             dti = DiscreteTI( mutation_file, md_in_conf = free_energy_start_pdb )
             dti.setup()
             dti.read_lambda_steps( cmdl['-lambda_steps'] )
             dti.do_dti(cmdl['-dti_mdp'], cmdl['-min_mdp'], cmdl['-dti_run_time'] )
 
 
-    print('\n\t\t\t ....... DONE .......... \n')
-
+    print '\n\t\t\t ....... DONE .......... \n'
+    
 
 
 ##     n_crooks_runs = cmdl['-n_crooks_runs']
 ##     if cmdl.opt['-m'].is_set:
 ##         mut_file  = cmdl['-m']
 ##     else:
 ##         mutations = []
 
 ##     if cmdl.opt['-mdp'].is_set:
 ##         mdp = MDP().read( cmdl['-mdp'] )
 ##     if cmdl.opt['-min_mdp'].is_set:
 ##         min_mdp = MDP().read( cmdl['-min_mdp'] )
 ##     if cmdl.opt['-lambda_steps'].is_set:
-##         lambda_file = cmdl['-lambda_steps']
-
-
+##         lambda_file = cmdl['-lambda_steps'] 
+    
+        
 ##     md = MD( pdb_in = pdb_in, water = water, conc = conc, box_type = box_type, box_size = box_size )
 ## #    md.setup()
 
 ##     dti = DiscreteTI( mut_file, md_in_conf = md.md_in_conf )
 ##     dti.setup()
 ##     dti.read_lambda_steps( lambda_file )
 ##     dti.do_dti(mdp, min_mdp, 10. )
 
 
-
+    
 ##     crooksMD = CrooksMD( mut_file, md_in_conf = md.md_in_conf)
 ##     crooksMD.setup()
 ##     crooksMD.do_crooks(mdp, 20, cmdl['-n_crooks_runs'])
-
+    
 #    fe_md = FreeEnergyMD( mutations, md_in_conf = md.md_in_conf )
 #    fe_md.setup()
-
-
+    
+    
 ##     generate_topology(pdb_in, water, 'amber99sbmut')
 ##     generate_sim_box( box_type, box_size )
 ##     fill_sim_box( water )
 ##     tpr_from_box()
 ##     add_ions( conc )
 ##     make_em_tpr()
 ##     run_em()
@@ -549,9 +549,9 @@
 ##     compact_repr( 'min.pdb')
 ##     clean_backups()
 
 
 
 if __name__=='__main__':
     main( sys.argv )
-
+
```

### Comparing `pmx_biobb-4.0.2/src/pmx_biobb.egg-info/PKG-INFO` & `pmx_biobb-4.1.2/src/pmx_biobb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmx-biobb
-Version: 4.0.2
+Version: 4.1.2
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger, Vytautas Gapsys
 Author-email: d.seeliger@gmx.net, vytautas.gapsys@gmail.com
 License: LGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pmx_biobb-4.0.2/versioneer.py` & `pmx_biobb-4.1.2/versioneer.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,15 @@
 domain. The `_version.py` that it creates is also in the public domain.
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
+
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -734,26 +735,26 @@
 def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
-    1: no tags. git_describe was just HEX. 4.0.2
+    1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "4.0.2" %% (pieces["distance"],
+        rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
@@ -1235,27 +1236,29 @@
 def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
-    1: no tags. git_describe was just HEX. 4.0.2
+    1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "4.0.2"
-
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
 
     Exceptions:
@@ -1393,18 +1396,21 @@
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
-    """Get the project version from whatever source is available."""
+    """Get the project version from whatever source is available.
+
+    Returns dict with two keys: 'version' and 'full'.
+    """
 
-    return {"version": "4.0.2", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
+    return {"version": "4.1.2", "full-revisionid": "4.1.2",
+            "dirty": None, "error": None,
             "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
```

