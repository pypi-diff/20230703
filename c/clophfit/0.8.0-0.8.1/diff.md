# Comparing `tmp/clophfit-0.8.0.tar.gz` & `tmp/clophfit-0.8.1.tar.gz`

## Comparing `clophfit-0.8.0.tar` & `clophfit-0.8.1.tar`

### file list

```diff
@@ -1,235 +1,188 @@
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.8.0/.codespellrc
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.8.0/.darglint
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 clophfit-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.8.0/.python-version
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.8.0/.readthedocs.yml
--rw-r--r--   0        0        0    16409 2020-02-02 00:00:00.000000 clophfit-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 clophfit-0.8.0/TODO.org
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.8.0/bandit.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.8.0/cz_customize_info.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 clophfit-0.8.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.8.0/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.8.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/Makefile
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/click.rst
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/conf.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f1.png
--rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f2.png
--rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f3.png
--rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f4.png
--rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f5.png
--rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f6.png
--rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/bs_pd_f7.png
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/csvtable.png
--rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/emcee-01.png
--rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/emcee-02.png
--rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/emcee-11.png
--rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/emcee-12.png
--rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/f01.png
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/file.png
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit1.png
--rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit2.png
--rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit3.png
--rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit4.png
--rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit5.png
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit6.png
--rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/gR_fit7.png
--rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit0.png
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit1.png
--rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit2.png
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit3.png
--rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/glmfit_np.r_.png
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit1.png
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit2.png
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit3.png
--rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit4.png
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmfit5.png
--rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel1.png
--rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel2.png
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel3.png
--rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel4.png
--rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel5.png
--rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel6.png
--rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/lmodel_H04.png
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/note_file.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/r_bs.png
--rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P-lmodel1.png
--rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P-lmodel2.png
--rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R1.png
--rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R2.png
--rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R3.png
--rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R4.png
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R5.png
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/ratio2P_R6.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/_static/rpy_bs.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/api/api.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/api/binding.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/api/prenspire.rst
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/api/prtecan.rst
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/contributing.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/description.rst
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/development.rst
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/older.rst
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/prenspire.rst
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/prenspire.uml.rst
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/prtecan.rst
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/prtecan.uml.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/references/references.rst
--rw-r--r--   0        0        0  1158929 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/prenspire.ipynb
--rw-r--r--   0        0        0  1959014 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/prtecan.ipynb
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/usage.org
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/usage.rst
--rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/usage2.org
--rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.8.0/docs/tutorials/usage2.rst
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/__init__.py
--rw-r--r--   0        0        0    12856 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/py.typed
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/binding/__init__.py
--rw-r--r--   0        0        0    22246 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/binding/fitting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/__init__.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/dil_buffer.py
--rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/dil_correction.py
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/fit_rpy.py
--rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/fit_titration.py
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/fit_titration_global.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/merge.py
--rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/plot_tecan.py
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/fit.tecan
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/fit.tecan.cl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/new_sort_K.sh
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_all
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_e2
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_lib
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_lib2
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_s202n
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/sum_v224q
--rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/old/bash/w_ave.sh
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/prenspire/__init__.py
--rw-r--r--   0        0        0    22071 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/prenspire/prenspire.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/prtecan/__init__.py
--rw-r--r--   0        0        0    54541 2020-02-02 00:00:00.000000 clophfit-0.8.0/src/clophfit/prtecan/prtecan.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_binding.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_cli.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_oldscripts.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_prenspire.py
--rw-r--r--   0        0        0    26719 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/test_prtecan.py
--rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/24well_clop0_95.csv
--rw-r--r--   0        0        0   679291 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/G10.csv
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/NTT-G10_note.csv
--rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/e2-T-without_sample_column.csv
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota-Err
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota.csv
--rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/h148g-spettroC.csv
--rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/NTT_37C_pKa.csv
--rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv
--rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png
--rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv
--rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv
--rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv
--rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv
--rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv
--rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv
--rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_100.xls
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_150.xls
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_20.xls
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_5.78.xls
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_50.xls
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_6.38.xls
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_6.83.xls
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_7.24.xls
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_7.67.xls
--rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_8.23.xls
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_8.82.xls
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290212_9.31.xls
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290513_5.5.xls
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290513_5.5_bad.xls
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290513_7.2.xls
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/290513_8.8.xls
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/list.cl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/list.cl20
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/list.pH
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/list.pH2
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/200214 pH data.ods
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl1_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl2_200214.xls
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl3_200214.xls
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl4_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl5_200214.xls
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl6_200214.xls
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl7_200214.xls
--rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/NaCl8_200214.xls
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/additions.cl
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/additions.pH
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/fit0-1.csv
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/fit0.csv
--rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/fit1-1.csv
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/fit1.csv
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/list.cl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/list.pH
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH5.0_200214.xls
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH5.8_200214.xls
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH6.5_200214.xls
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH7.1_200214.xls
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH7.6_200214.xls
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH8.3_200214.xls
--rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/pH9.1_200214.xls
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/scheme.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/140220/scheme0.txt
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
--rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/exceptions/84wells_290212_20.xlsx
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/Tecan/exceptions/88wells_290212_20.xlsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/A01-20140311a.dat
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/A01.dat
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/A11.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/B01.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/H04.dat
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/NTT-A04-Cl_note
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/copyIP.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/ratio2P.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/w.txt
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_A.csv
--rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_A.png
--rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_B.csv
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_B.png
--rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_C.csv
--rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_C.png
--rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_D.csv
--rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_D.png
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_E.csv
--rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_E.png
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_F.csv
--rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/Meas/A04 Cl_F.png
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/Cl/A11-failed.dat
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/Cl/B05-20130628-cor.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/pH/B01-failed.dat
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/pH/D05.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/global/pH/H04-with_nan.dat
--rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/k/D05.dat-bs.png
--rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/k/D05.dat.png
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png
--rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/output/global/pH/D05.dat.png
--rw-r--r--   0        0        0   530592 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/tmp/A04 Cl.csv
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 clophfit-0.8.0/tests/data/tmp/NTT-A04-Cl_note.csv
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.8.0/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 clophfit-0.8.0/README.md
--rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 clophfit-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 clophfit-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.8.1/.codespellrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.8.1/.darglint
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 clophfit-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.8.1/.python-version
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 clophfit-0.8.1/.readthedocs.yml
+-rw-r--r--   0        0        0    17499 2020-02-02 00:00:00.000000 clophfit-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 clophfit-0.8.1/TODO.org
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.8.1/bandit.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.8.1/cz_customize_info.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.8.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 clophfit-0.8.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.8.1/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.8.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/Makefile
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/click.rst
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/conf.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/_static/csvtable.png
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/_static/file.png
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/_static/note_file.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/api/api.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/api/binding.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/api/prenspire.rst
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/api/prtecan.rst
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/references/contributing.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/references/description.rst
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/references/development.rst
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/references/older.rst
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/references/prenspire.rst
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/references/prenspire.uml.rst
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/references/prtecan.rst
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/references/prtecan.uml.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/references/references.rst
+-rw-r--r--   0        0        0  2146653 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/tutorials/LMfit.ipynb
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/tutorials/oldscripts_TODO.org
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/tutorials/oldscripts_TODO.rst
+-rw-r--r--   0        0        0  1158929 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/tutorials/prenspire.ipynb
+-rw-r--r--   0        0        0  1959014 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/tutorials/prtecan.ipynb
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 clophfit-0.8.1/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/__init__.py
+-rw-r--r--   0        0        0    12856 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/py.typed
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/binding/__init__.py
+-rw-r--r--   0        0        0    22272 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/binding/fitting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/__init__.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/dil_buffer.py
+-rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/dil_correction.py
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/fit_rpy.py
+-rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/fit_titration.py
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/fit_titration_global.py
+-rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/merge.py
+-rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/plot_tecan.py
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/fit.tecan
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/fit.tecan.cl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/new_sort_K.sh
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/sum_all
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/sum_e2
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/sum_lib
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/sum_lib2
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/sum_s202n
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/sum_v224q
+-rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/old/bash/w_ave.sh
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/prenspire/__init__.py
+-rw-r--r--   0        0        0    22071 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/prenspire/prenspire.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/prtecan/__init__.py
+-rw-r--r--   0        0        0    54541 2020-02-02 00:00:00.000000 clophfit-0.8.1/src/clophfit/prtecan/prtecan.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/conftest.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/test_binding.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/test_cli.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/test_oldscripts.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/test_prenspire.py
+-rw-r--r--   0        0        0    28622 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/test_prtecan.py
+-rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/24well_clop0_95.csv
+-rw-r--r--   0        0        0   679291 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/G10.csv
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/NTT-G10_note.csv
+-rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/e2-T-without_sample_column.csv
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/h148g-spettroC-nota
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/h148g-spettroC-nota-Err
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/h148g-spettroC-nota.csv
+-rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/h148g-spettroC.csv
+-rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/cli/NTT_37C_pKa.csv
+-rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv
+-rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.png
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv
+-rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.png
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv
+-rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/exceptions/e2dan-emwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/exceptions/e2dan-exwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/exceptions/e2dan-exwavelength2.csv
+-rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv
+-rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv
+-rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv
+-rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_100.xls
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_150.xls
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_20.xls
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_5.78.xls
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_50.xls
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_6.38.xls
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_6.83.xls
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_7.24.xls
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_7.67.xls
+-rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_8.23.xls
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_8.82.xls
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290212_9.31.xls
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290513_5.5.xls
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290513_5.5_bad.xls
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290513_7.2.xls
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/290513_8.8.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/list.cl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/list.cl20
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/list.pH
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/list.pH2
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/200214 pH data.ods
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/NaCl1_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/NaCl2_200214.xls
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/NaCl3_200214.xls
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/NaCl4_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/NaCl5_200214.xls
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/NaCl6_200214.xls
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/NaCl7_200214.xls
+-rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/NaCl8_200214.xls
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/additions.cl
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/additions.pH
+-rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/fit0-1.csv
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/fit0.csv
+-rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/fit1-1.csv
+-rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/fit1.csv
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/list.cl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/list.pH
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/pH5.0_200214.xls
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/pH5.8_200214.xls
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/pH6.5_200214.xls
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/pH7.1_200214.xls
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/pH7.6_200214.xls
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/pH8.3_200214.xls
+-rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/pH9.1_200214.xls
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/scheme.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/140220/scheme0.txt
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/exceptions/84wells_290212_20.xlsx
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/Tecan/exceptions/88wells_290212_20.xlsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/A01-20140311a.dat
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/A01.dat
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/A11.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/B01.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/H04.dat
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/NTT-A04-Cl_note
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/copyIP.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/ratio2P.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/w.txt
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_A.csv
+-rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_A.png
+-rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_B.csv
+-rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_B.png
+-rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_C.csv
+-rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_C.png
+-rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_D.csv
+-rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_D.png
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_E.csv
+-rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_E.png
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_F.csv
+-rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/Meas/A04 Cl_F.png
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/global/Cl/A11-failed.dat
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/global/Cl/B05-20130628-cor.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/global/pH/B01-failed.dat
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/global/pH/D05.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/global/pH/H04-with_nan.dat
+-rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/k/D05.dat-bs.png
+-rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/k/D05.dat.png
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/output/global/Cl/B05-20130628-cor.dat.png
+-rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/output/global/pH/D05.dat.png
+-rw-r--r--   0        0        0   530592 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/tmp/A04 Cl.csv
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 clophfit-0.8.1/tests/data/tmp/NTT-A04-Cl_note.csv
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.8.1/LICENSE.txt
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 clophfit-0.8.1/README.md
+-rw-r--r--   0        0        0    11381 2020-02-02 00:00:00.000000 clophfit-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 clophfit-0.8.1/PKG-INFO
```

### Comparing `clophfit-0.8.0/.pre-commit-config.yaml` & `clophfit-0.8.1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
-      - id: check-added-large-files # hyper
-        exclude: "^tests/EnSpire/"
+      - id: check-added-large-files
+        exclude: "^tests/EnSpire/|^docs/tutorials/LMfit.ipynb"
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-shebang-scripts-are-executable
       - id: check-merge-conflict
       - id: check-symlinks
       - id: destroyed-symlinks
@@ -35,28 +35,28 @@
     hooks:
       - id: pretty-format-ini
         args: [--autofix]
       - id: pretty-format-toml
         args: [--autofix]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
+    rev: v0.0.275
     hooks:
       - id: ruff
         # args: [--exclude, "src/clophfit/prenspire/*"]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black-jupyter
       - id: black
         require_serial: true
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black]
         exclude: docs/tutorials/usage.*.rst
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0-alpha.9-for-vscode
@@ -86,23 +86,23 @@
   - repo: https://github.com/terrencepreilly/darglint
     rev: v1.8.1
     hooks:
       - id: darglint
         stages: [manual]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.2
+    rev: v0.9.0.5
     hooks:
       - id: shellcheck
         args: [-x]
 
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: 3.2.2
+    rev: 3.5.2
     hooks:
       - id: commitizen
       - id: commitizen-branch
         stages: [push]
```

### Comparing `clophfit-0.8.0/CHANGELOG.md` & `clophfit-0.8.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,46 @@
 <!-- markdownlint-disable MD024 -->
 <!-- vale write-good.TooWordy = NO -->
 
 # Changelog
 
+## v0.8.1 (2023-07-03)
+
+### Docs
+
+- fix pointer to changelog in project.toml (#274)
+
+### Build
+
+- update pandas requirement from <2.0.3 to <2.0.4 (#297)
+- update scipy requirement from <1.11.1 to <1.11.2 (#296)
+- bump sphinx-autodoc-typehints from 1.23.2 to 1.23.3 (#294)
+- update pytest requirement from <7.3.3 to <7.4.1 (#292)
+- update commitizen requirement from <3.3.1 to <3.5.3 (#291)
+- update scipy requirement from <1.10.2 to <1.11.1 (#293)
+- bump ruff from 0.0.272 to 0.0.275 (#289)
+- update mypy requirement from <1.4 to <1.5 (#286)
+- update numpy requirement from <1.24.4 to <1.25.1 (#284)
+- bump sphinx-autodoc-typehints from 1.23.0 to 1.23.2 (#283)
+- update commitizen requirement from <3.2.3 to <3.3.1 (#281)
+- update pytest requirement from <7.3.2 to <7.3.3 (#279)
+- bump ruff from 0.0.270 to 0.0.272 (#278)
+- bump pandas-stubs from 2.0.1.230501 to 2.0.2.230605 (#276)
+
+### Refactor
+
+- **docs**: Drop rpy; convert into LMfit.ipynb
+
+### chore
+
+- update pre-commit hooks (#295)
+- update pre-commit hooks (#285)
+- update pre-commit hooks (#280)
+- update pre-commit hooks (#275)
+
 ## v0.8.0 (2023-06-05)
 
 ### Feat
 
 - **prenspire**: build and fit single-and-global SVD-or-band titrations
 - **clop**: fit_titration for old note
 - **clop**: `fit titration global old` and `fit titration old` as cli command
```

### Comparing `clophfit-0.8.0/TODO.org` & `clophfit-0.8.1/TODO.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/cz_customize_info.txt` & `clophfit-0.8.1/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/.github/workflows/ci.yml` & `clophfit-0.8.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/.github/workflows/docs.yml` & `clophfit-0.8.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/Makefile` & `clophfit-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/conf.py` & `clophfit-0.8.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 # -- Project information -----------------------------------------------------
 
 project = "ClopHfit"
 copyright = "2023, Daniele Arosio"  # noqa: A001
 author = "Daniele Arosio"
-release = "0.8.0"
+release = "0.8.1"
 html_title = "ClopHfit"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `clophfit-0.8.0/docs/index.rst` & `clophfit-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/make.bat` & `clophfit-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/_static/csvtable.png` & `clophfit-0.8.1/docs/_static/csvtable.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/_static/file.png` & `clophfit-0.8.1/docs/_static/file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/_static/note_file.png` & `clophfit-0.8.1/docs/_static/note_file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/references/contributing.rst` & `clophfit-0.8.1/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/references/development.rst` & `clophfit-0.8.1/docs/references/development.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/references/older.rst` & `clophfit-0.8.1/docs/references/older.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/references/prenspire.uml.rst` & `clophfit-0.8.1/docs/references/prenspire.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/references/prtecan.rst` & `clophfit-0.8.1/docs/references/prtecan.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/references/prtecan.uml.rst` & `clophfit-0.8.1/docs/references/prtecan.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/tutorials/prenspire.ipynb` & `clophfit-0.8.1/docs/tutorials/prenspire.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/docs/tutorials/prtecan.ipynb` & `clophfit-0.8.1/docs/tutorials/prtecan.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/__main__.py` & `clophfit-0.8.1/src/clophfit/__main__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/binding/fitting.py` & `clophfit-0.8.1/src/clophfit/binding/fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,14 +577,15 @@
     Notes
     -----
     For the SVD method, the function plots the original spectra, the principal
     component vectors, the singular values, the first principal component, and
     the fitting results. For the band method, it plots the original spectra and
     the fitting results.
     """
+    y_offset = 1.0
     if kind == "Cl":
         hue_norm = (0.0, 200.0)
         palette = sb.cm.crest.name
         fz = _binding_kd
     else:
         hue_norm = (5.7, 8.7)
         palette = sb.cm.vlag_r.name
@@ -592,15 +593,15 @@
     x = spectra.columns.to_numpy()
     fig = sb.mpl.pyplot.figure(figsize=(12, 8))
     ax1 = fig.add_axes([0.05, 0.65, 0.32, 0.31])
     plot_spectra(spectra, ax1, hue_norm, palette, kind)
     if band is None:  # SVD
         ddf = spectra.sub(spectra.iloc[:, 0], axis=0)
         u, s, v = np.linalg.svd(ddf)
-        y = v[0, :] + 1
+        y = v[0, :] + y_offset
         result = fit_binding(x, y, fz)
         ax2 = fig.add_axes([0.42, 0.65, 0.32, 0.31])
         _plot_autovectors(spectra.index, u, ax2)
         ax3 = fig.add_axes([0.80, 0.65, 0.18, 0.31])
         plot_autovalues(s[:], ax3)  # don't plot last auto-values?
         ax5 = fig.add_axes([0.63, 0.08, 0.35, 0.50])
         plot_pca(v, ax5, x, hue_norm, palette)
```

### Comparing `clophfit-0.8.0/src/clophfit/old/dil_buffer.py` & `clophfit-0.8.1/src/clophfit/old/dil_buffer.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/old/dil_correction.py` & `clophfit-0.8.1/src/clophfit/old/dil_correction.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/old/fit_rpy.py` & `clophfit-0.8.1/src/clophfit/old/fit_rpy.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/old/fit_titration.py` & `clophfit-0.8.1/src/clophfit/old/fit_titration.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/old/fit_titration_global.py` & `clophfit-0.8.1/src/clophfit/old/fit_titration_global.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/old/merge.py` & `clophfit-0.8.1/src/clophfit/old/merge.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/old/plot_tecan.py` & `clophfit-0.8.1/src/clophfit/old/plot_tecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/old/bash/w_ave.sh` & `clophfit-0.8.1/src/clophfit/old/bash/w_ave.sh`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/prenspire/__init__.py` & `clophfit-0.8.1/src/clophfit/prenspire/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/prenspire/prenspire.py` & `clophfit-0.8.1/src/clophfit/prenspire/prenspire.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/prtecan/__init__.py` & `clophfit-0.8.1/src/clophfit/prtecan/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/src/clophfit/prtecan/prtecan.py` & `clophfit-0.8.1/src/clophfit/prtecan/prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/test_binding.py` & `clophfit-0.8.1/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/test_cli.py` & `clophfit-0.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/test_oldscripts.py` & `clophfit-0.8.1/tests/test_oldscripts.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import subprocess  # nosec B404
 import sys
 import typing
 from pathlib import Path
 from typing import Any
+from typing import ClassVar
 from typing import Iterator
 from typing import List
 from typing import Tuple
 
 import matplotlib.testing.compare as mpltc  # type: ignore
 import pytest
 from matplotlib.testing.exceptions import ImageComparisonFailure  # type: ignore
@@ -22,20 +23,20 @@
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="does not run on windows")
 class TestTitrationFit:
     """Test the old ``fit_titration.py`` script."""
 
     note_fp = "./NTT-A04-Cl_note"
-    csv_files = ["./Meas/A04 Cl_A.csv", "./Meas/A04 Cl_B.csv"]
-    res_svd = [
+    csv_files: ClassVar[list[str]] = ["./Meas/A04 Cl_A.csv", "./Meas/A04 Cl_B.csv"]
+    res_svd: ClassVar[list[str]] = [
         "K =  17.035\nsK =  0.666\nSA =  -0.0\nsSA =  0.007\nSB =  -0.275\nsSB =  0.002",
         "K =  14.824\nsK =  0.708\nSA =  0.019\nsSA =  0.004\nSB =  -0.274\nsSB =  0.002",
     ]
-    res_band = [
+    res_band: ClassVar[list[str]] = [
         "K =  15.205\nsK =  0.549\nSA =  205506.748\nsSA =  1862.684\nSB =  1781.387\nsSB =  1249.163",
         "K =  15.015\nsK =  0.701\nSA =  253789.494\nsSA =  3055.602\nSB =  -4381.091\nsSB =  2040.904",
     ]
 
     @pytest.fixture(
         scope="class",
         params=[
@@ -93,19 +94,19 @@
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="does not run on windows")
 @typing.no_type_check
 class TestTitrationFitGlobal:
     """It test the old ``fit_titration_global.py`` script."""
 
-    dat_files = [
+    dat_files: ClassVar[list[str]] = [
         "./global/pH/D05.dat",
         "./global/Cl/B05-20130628-cor.dat",
     ]
-    res = [
+    res: ClassVar[list[str]] = [
         """SA1   683.357   714.804   740.747   767.245   800.925
 SB1   246.164   299.394   338.212   374.611   417.296
 SA2   11.0487   47.6023   76.2874     104.3   138.128
 SB2    491.64   534.936   571.809   611.045   664.602
   K   7.34376   7.51152   7.65166   7.80003   7.99971
 bootstrap:""",
         """SA1   26910.8   27072.2   27216.7   27361.3   27522.7
```

### Comparing `clophfit-0.8.0/tests/test_prenspire.py` & `clophfit-0.8.1/tests/test_prenspire.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/test_prtecan.py` & `clophfit-0.8.1/tests/test_prtecan.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """Test prtecan module."""
 from __future__ import annotations
 
 import re
 import sys
 from pathlib import Path
 from typing import Any
+from typing import ClassVar
 
 import numpy as np
 import pandas as pd
 import pytest
+from numpy.testing import assert_almost_equal
+from numpy.testing import assert_array_equal
 
 from clophfit import prtecan
 from clophfit.prtecan import Labelblock
+from clophfit.prtecan import LabelblocksGroup
+from clophfit.prtecan import Tecanfile
+from clophfit.prtecan import TecanfilesGroup
 from clophfit.prtecan import TitrationAnalysis
 
 # By defining csvl, lb0, and lb1 as class attributes, they are created only once
 # per test session. Use fixture to capture UserWarning "OVER"
 
 data_tests = Path(__file__).parent / "Tecan"
 pytestmark = pytest.mark.filterwarnings("ignore:OVER")
@@ -83,18 +89,16 @@
     assert mmd["Shaking (Linear) Amplitude:"] == prtecan.Metadata(2, ["mm"])
 
 
 def test_calculate_conc() -> None:
     """Calculates concentration values from Cl additions."""
     additions = [112, 2, 2, 2, 2, 2, 2, 6, 4]
     conc = prtecan.calculate_conc(additions, 1000)
-    np.testing.assert_almost_equal(
-        conc,
-        [0.0, 17.544, 34.483, 50.847, 66.667, 81.967, 96.774, 138.462, 164.179],
-        3,
+    assert_almost_equal(
+        conc, [0.0, 17.544, 34.483, 50.847, 66.667, 81.967, 96.774, 138.462, 164.179], 3
     )
 
 
 @pytest.mark.filterwarnings("ignore:OVER")
 class TestLabelblock:
     """Test labelblock class."""
 
@@ -166,15 +170,15 @@
         lb1.buffer_norm = 0.4821
         assert lb0.data_buffersubtracted_norm["F06"] == pytest.approx(1050.13)
         assert lb1.data_buffersubtracted_norm["H12"] == pytest.approx(48.0)
 
     def test_eq(self, labelblocks: tuple[Labelblock, Labelblock]) -> None:
         """Check if a Labelblock is equal to itself and not equal to a different Labelblock."""
         lb0, lb1 = labelblocks
-        assert lb0 == lb0, "Labelblock is not equal to itself"
+        assert id(lb0) == id(lb0), "Labelblock is not equal to itself"
         assert lb0 != lb1, "Different Labelblocks are incorrectly reported as equal"
         assert (
             lb0.__eq__(1) == NotImplemented
         ), "Equality check against non-Labelblock object did not return NotImplemented"
 
     def test_almost_eq(self, labelblocks: tuple[Labelblock, Labelblock]) -> None:
         """Test the __almost_eq__ method of the Labelblock class."""
@@ -275,97 +279,104 @@
         with pytest.raises(ValueError, match="No Labelblock found."):
             prtecan.Tecanfile(data_tests / "exceptions/0_Labelblocks_290513_5.5.xlsx")
 
 
 class TestLabelblocksGroup:
     """Test LabelBlocksGroup class."""
 
-    tfs = [
-        prtecan.Tecanfile(data_tests / "290513_5.5.xls"),
-        prtecan.Tecanfile(data_tests / "290513_7.2.xls"),
-        prtecan.Tecanfile(data_tests / "290513_8.8.xls"),
-    ]
-    lbg0 = prtecan.LabelblocksGroup([tfs[0].labelblocks[0], tfs[1].labelblocks[0]])
-    lbg1 = prtecan.LabelblocksGroup([tfs[1].labelblocks[1], tfs[2].labelblocks[1]])
-    lbg0.buffer_wells = ["C12", "D01", "D12", "E01", "E12", "F01"]
-    lbg1.buffer_wells = ["C12", "D01", "D12", "E01", "E12", "F01"]
+    @pytest.fixture(autouse=True, scope="class")
+    def tfs(self) -> list[Tecanfile]:
+        """Set up list of Tecanfile."""
+        return [
+            Tecanfile(data_tests / "290513_5.5.xls"),
+            Tecanfile(data_tests / "290513_7.2.xls"),
+            Tecanfile(data_tests / "290513_8.8.xls"),
+        ]
 
-    def test_metadata(self) -> None:
+    @pytest.fixture(autouse=True, scope="class")
+    def lbgs(self, tfs: list[Tecanfile]) -> tuple[LabelblocksGroup, LabelblocksGroup]:
+        """Set up LabelblocksGroup 0 and 1."""
+        lbg0 = LabelblocksGroup([tfs[0].labelblocks[0], tfs[1].labelblocks[0]])
+        lbg1 = LabelblocksGroup([tfs[1].labelblocks[1], tfs[2].labelblocks[1]])
+        lbg0.buffer_wells = ["C12", "D01", "D12", "E01", "E12", "F01"]
+        lbg1.buffer_wells = ["C12", "D01", "D12", "E01", "E12", "F01"]
+        return lbg0, lbg1
+
+    def test_metadata(self, lbgs: tuple[LabelblocksGroup, LabelblocksGroup]) -> None:
         """Merge only shared metadata."""
-        assert self.lbg0.metadata.get("Temperature") is None
-        assert self.lbg1.metadata.get("Temperature") is None
-        assert self.lbg1.metadata.get("Gain") is None
-        assert self.lbg1.labelblocks[0].metadata["Gain"].value == 98
-        assert self.lbg1.labelblocks[1].metadata["Gain"].value == 99
+        assert lbgs[0].metadata.get("Temperature") is None
+        assert lbgs[1].metadata.get("Temperature") is None
+        assert lbgs[1].metadata.get("Gain") is None
+        assert lbgs[1].labelblocks[0].metadata["Gain"].value == 98
+        assert lbgs[1].labelblocks[1].metadata["Gain"].value == 99
         # Common metadata.
-        assert self.lbg0.metadata["Gain"].value == 94
-        assert self.lbg0.metadata["Number of Flashes"].value == 10
+        assert lbgs[0].metadata["Gain"].value == 94
+        assert lbgs[0].metadata["Number of Flashes"].value == 10
 
-    def test_data(self) -> None:
+    def test_data(self, lbgs: tuple[LabelblocksGroup, LabelblocksGroup]) -> None:
         """Merge data."""
-        assert self.lbg0.data is not None
-        assert self.lbg0.data["A01"] == [18713, 17088]
-        assert self.lbg0.data["H12"] == [28596, 25771]
-        assert self.lbg1.data is None
+        assert lbgs[0].data is not None
+        assert lbgs[0].data["A01"] == [18713, 17088]
+        assert lbgs[0].data["H12"] == [28596, 25771]
+        assert lbgs[1].data is None
 
-    def test_data_normalized(self) -> None:
+    def test_data_normalized(
+        self, lbgs: tuple[LabelblocksGroup, LabelblocksGroup]
+    ) -> None:
         """Merge data_normalized."""
-        np.testing.assert_almost_equal(
-            self.lbg1.data_norm["H12"], [693.980, 714.495], 3
-        )
-        np.testing.assert_almost_equal(
-            self.lbg0.data_norm["A01"], [995.372, 908.936], 3
-        )
+        assert_almost_equal(lbgs[1].data_norm["H12"], [693.980, 714.495], 3)
+        assert_almost_equal(lbgs[0].data_norm["A01"], [995.372, 908.936], 3)
 
-    def test_data_buffersubtracted(self) -> None:
+    def test_data_buffersubtracted(
+        self, lbgs: tuple[LabelblocksGroup, LabelblocksGroup]
+    ) -> None:
         """Merge data_buffersubtracted."""
-        assert self.lbg0.data_buffersubtracted is not None
-        np.testing.assert_almost_equal(
-            self.lbg0.data_buffersubtracted["B07"], [7069, 5716.7], 1
-        )
-        assert self.lbg1.data_buffersubtracted is None
+        assert lbgs[0].data_buffersubtracted is not None
+        assert_almost_equal(lbgs[0].data_buffersubtracted["B07"], [7069, 5716.7], 1)
+        assert lbgs[1].data_buffersubtracted is None
 
-    def test_data_buffersubtracted_norm(self) -> None:
+    def test_data_buffersubtracted_norm(
+        self, lbgs: tuple[LabelblocksGroup, LabelblocksGroup]
+    ) -> None:
         """Merge data_buffersubtracted."""
-        np.testing.assert_almost_equal(
-            self.lbg0.data_buffersubtracted_norm["B07"], [376.01, 304.08], 2
+        assert_almost_equal(
+            lbgs[0].data_buffersubtracted_norm["B07"], [376.01, 304.08], 2
         )
-        np.testing.assert_almost_equal(
-            self.lbg1.data_buffersubtracted_norm["B07"], [355.16, 348.57], 2
+        assert_almost_equal(
+            lbgs[1].data_buffersubtracted_norm["B07"], [355.16, 348.57], 2
         )
 
-    def test_notequal_labelblocks(self) -> None:
-        """It raises Exception when concatenating unequal labelblocks."""
-        tfs = self.tfs
+    def test_notequal_labelblocks(self, tfs: list[Tecanfile]) -> None:
+        """Raise Exception when concatenating unequal labelblocks."""
         with pytest.raises(ValueError, match="Creation of labelblock group failed."):
             prtecan.LabelblocksGroup([tfs[1].labelblocks[0], tfs[2].labelblocks[1]])
 
 
 class TestTecanfileGroup:
     """Group tecanfiles properly."""
 
     class TestAllEqLbgs:
         """Test TfG with 2 LbG in the same order."""
 
-        filenames = ["290513_5.5.xls", "290513_7.2.xls"]
-        tecanfiles = [prtecan.Tecanfile(data_tests / f) for f in filenames]
-        tfg = prtecan.TecanfilesGroup(tecanfiles)
+        @pytest.fixture(autouse=True, scope="class")
+        def tfg(self) -> TecanfilesGroup:
+            """Set up TecanfilesGroup."""
+            filenames = ["290513_5.5.xls", "290513_7.2.xls"]
+            tecanfiles = [Tecanfile(data_tests / f) for f in filenames]
+            return TecanfilesGroup(tecanfiles)
 
-        def test_metadata(self) -> None:
+        def test_metadata(self, tfg: TecanfilesGroup) -> None:
             """Parse general metadata."""
-            assert (
-                self.tfg.metadata["Plate"].value
-                == "PE 96 Flat Bottom White   [PE.pdfx]"
-            )
-            assert self.tfg.metadata["System"].value == "TECANROBOT"
+            assert tfg.metadata["Plate"].value == "PE 96 Flat Bottom White   [PE.pdfx]"
+            assert tfg.metadata["System"].value == "TECANROBOT"
 
-        def test_labelblocksgroups(self) -> None:
+        def test_labelblocksgroups(self, tfg: TecanfilesGroup) -> None:
             """Generate 2 LbG with .data and .metadata."""
-            lbg0 = self.tfg.labelblocksgroups[0]
-            lbg1 = self.tfg.labelblocksgroups[1]
+            lbg0 = tfg.labelblocksgroups[0]
+            lbg1 = tfg.labelblocksgroups[1]
             # metadata
             assert lbg0.metadata["Number of Flashes"].value == 10.0
             assert lbg1.metadata["Gain"].value == 98.0
             # data normalized ... enough in lbg
             # data
             assert lbg0.data is not None
             assert lbg0.data["A01"] == [18713, 17088]
@@ -373,90 +384,115 @@
             assert lbg1.data is not None
             assert lbg1.data["A01"] == [7878, 8761]
             assert lbg1.data["H12"] == [14226, 13602]
 
     class TestAlmostEqLbgs:
         """Test TfG when 1 LbG equal and a second with almost equal labelblocks."""
 
-        filenames = [
-            "290513_5.5.xls",  # Label1 and Label2
-            "290513_7.2.xls",  # Label1 and Label2
-            "290513_8.8.xls",  # Label1 and Label2 with different metadata
-        ]
-        tecanfiles = [prtecan.Tecanfile(data_tests / f) for f in filenames]
-        with pytest.warns(UserWarning) as record:
-            group = prtecan.TecanfilesGroup(tecanfiles)
-
-        def test_warn(self) -> None:
+        @pytest.fixture(autouse=True, scope="class")
+        def tfg_warn(self) -> tuple[TecanfilesGroup, pytest.WarningsRecorder]:
+            """Set up TecanfilesGroup with Warning."""
+            filenames = [
+                "290513_5.5.xls",  # Label1 and Label2
+                "290513_7.2.xls",  # Label1 and Label2
+                "290513_8.8.xls",  # Label1 and Label2 with different metadata
+            ]
+            tecanfiles = [Tecanfile(data_tests / f) for f in filenames]
+            with pytest.warns(UserWarning) as record:
+                tfg = TecanfilesGroup(tecanfiles)
+            return tfg, record
+
+        @pytest.fixture(autouse=True, scope="class")
+        def tfg(
+            self, tfg_warn: tuple[TecanfilesGroup, pytest.WarningsRecorder]
+        ) -> TecanfilesGroup:
+            """Extract TecanfilesGroup."""
+            return tfg_warn[0]
+
+        def test_warn(
+            self, tfg_warn: tuple[TecanfilesGroup, pytest.WarningsRecorder]
+        ) -> None:
             """Warn about labelblocks anomaly."""
-            assert "Different LabelblocksGroup among filenames:" in str(
-                self.record[0].message
-            )
+            msg_str = str(tfg_warn[1][0].message)
+            assert "Different LabelblocksGroup among filenames" in msg_str
 
-        def test_labelblocksgroups(self) -> None:
+        def test_labelblocksgroups(self, tfg: TecanfilesGroup) -> None:
             """Generate 1 LbG with .data and .metadata."""
-            lbg0 = self.group.labelblocksgroups[0]
+            lbg0 = tfg.labelblocksgroups[0]
             # metadata
             assert lbg0.metadata["Number of Flashes"].value == 10.0
             assert lbg0.metadata["Gain"].value == 94
             # data
             assert lbg0.data is not None
             assert lbg0.data["A01"] == [18713.0, 17088.0, 17123.0]
             assert lbg0.data["H12"] == [28596.0, 25771.0, 28309.0]
 
-        def test_mergeable_labelblocksgroups(self) -> None:
+        def test_mergeable_labelblocksgroups(self, tfg: TecanfilesGroup) -> None:
             """Generate 1 Lbg only with .data_normalized and only common .metadata."""
-            lbg1 = self.group.labelblocksgroups[1]
+            lbg1 = tfg.labelblocksgroups[1]
             # metadata
             assert lbg1.metadata["Number of Flashes"].value == 10.0
             assert lbg1.metadata.get("Gain") is None
             assert lbg1.data is None
             # data_normalized
-            np.testing.assert_almost_equal(
+            assert_almost_equal(
                 lbg1.data_norm["A01"], [401.9387755, 446.9897959, 450.0]
             )
-            np.testing.assert_almost_equal(
+            assert_almost_equal(
                 lbg1.data_norm["H12"], [725.8163265, 693.9795918, 714.4949494]
             )
 
     class TestOnly1commonLbg:
         """Test TfG with different number of labelblocks, but mergeable."""
 
-        filenames = [
-            "290212_5.78.xls",  # Label1 and Label2
-            "290212_20.xls",  # Label2 only
-            "290212_100.xls",  # Label2 only
-        ]
-        tecanfiles = [prtecan.Tecanfile(data_tests / f) for f in filenames]
-        # pylint: disable=W0201
-        with pytest.warns(UserWarning) as record:
-            group = prtecan.TecanfilesGroup(tecanfiles)
-
-        def test_warn(self) -> None:
+        @pytest.fixture(autouse=True, scope="class")
+        def tfg_warn(self) -> tuple[TecanfilesGroup, pytest.WarningsRecorder]:
+            """Set up TecanfilesGroup with Warning."""
+            filenames = [
+                "290212_5.78.xls",  # Label1 and Label2
+                "290212_20.xls",  # Label2 only
+                "290212_100.xls",  # Label2 only
+            ]
+            tecanfiles = [Tecanfile(data_tests / f) for f in filenames]
+            with pytest.warns(UserWarning) as record:
+                tfg = TecanfilesGroup(tecanfiles)
+            return tfg, record
+
+        @pytest.fixture(autouse=True, scope="class")
+        def tfg(
+            self, tfg_warn: tuple[TecanfilesGroup, pytest.WarningsRecorder]
+        ) -> TecanfilesGroup:
+            """Extract TecanfilesGroup."""
+            return tfg_warn[0]
+
+        def test_warn(
+            self, tfg_warn: tuple[TecanfilesGroup, pytest.WarningsRecorder]
+        ) -> None:
             """Warn about labelblocks anomaly."""
-            assert "Different LabelblocksGroup among filenames" in str(
-                self.record[0].message
-            )
+            msg_str = str(tfg_warn[1][0].message)
+            assert "Different LabelblocksGroup among filenames" in msg_str
 
-        def test_labelblocksgroups(self) -> None:
+        def test_labelblocksgroups(self, tfg: TecanfilesGroup) -> None:
             """Generates 1 LbG with .data and .metadata."""
-            lbg = self.group.labelblocksgroups[0]
+            lbg = tfg.labelblocksgroups[0]
             # metadata
             assert lbg.metadata["Number of Flashes"].value == 10.0
             assert lbg.metadata["Gain"].value == 93.0
             # data
             assert lbg.data is not None
             assert lbg.data["A01"] == [6289, 6462, 6465]
             assert lbg.data["H12"] == [4477, 4705, 4918]
 
     class TestFailToMerge:
         """Test TfG without mergeable labelblocks."""
 
-        filenames = ["290513_5.5.xls", "290513_5.5_bad.xls"]
-        tecanfiles = [prtecan.Tecanfile(data_tests / f) for f in filenames]
+        filenames: ClassVar[list[str]] = ["290513_5.5.xls", "290513_5.5_bad.xls"]
+        tecanfiles: ClassVar[list[prtecan.Tecanfile]] = [
+            prtecan.Tecanfile(data_tests / f) for f in filenames
+        ]
 
         def test_raise_exception(self) -> None:
             """Raise Exception when there is no way to build labelblocksGroup."""
             with pytest.raises(
                 ValueError,
                 match=r"No common labelblock in filenames: .*290513_5.5_bad.xls",
             ):
@@ -520,15 +556,15 @@
 
 @pytest.mark.filterwarnings("ignore:OVER")
 class TestTitrationAnalysis:
     """Test TitrationAnalysis class."""
 
     @pytest.fixture(autouse=True, scope="class")
     def titan(self) -> TitrationAnalysis:
-        """Set up test class."""
+        """Set up the TitrationAnalysis."""
         titan = prtecan.TitrationAnalysis.fromlistfile(data_tests / "140220/list.pH")
         titan.load_additions(data_tests / "140220/additions.pH")
         titan.load_scheme(data_tests / "140220/scheme.txt")
         return titan
 
     def test_scheme(self, titan: TitrationAnalysis) -> None:
         """It finds well position for buffer samples."""
@@ -548,50 +584,48 @@
         with pytest.raises(ValueError, match=re.escape(msg)):
             titan.load_scheme(bad_schemefile)
 
     def test_subtract_bg(self, titan: TitrationAnalysis) -> None:
         """It subtracts buffer average values."""
         lbg0 = titan.labelblocksgroups[0]
         lbg1 = titan.labelblocksgroups[1]
-        np.testing.assert_almost_equal(
-            lbg0.data_norm["E01"][::2],
-            [601.72, 641.505, 674.355, 706.774],
-            3,
+        assert_almost_equal(
+            lbg0.data_norm["E01"][::2], [601.72, 641.505, 674.355, 706.774], 3
         )
         assert lbg0.data is not None
         assert lbg0.data["E01"][::2] == [11192.0, 11932.0, 12543.0, 13146.0]
         assert lbg0.data_buffersubtracted is not None
-        np.testing.assert_array_equal(
+        assert_array_equal(
             lbg0.data_buffersubtracted["A12"][::3], [8084.5, 16621.75, 13775.0]
         )
         assert lbg1.data_buffersubtracted is not None
-        np.testing.assert_array_equal(
+        assert_array_equal(
             lbg1.data_buffersubtracted["A12"][::3], [9758.25, 1334.0, 283.5]
         )
 
     def test_dilution_correction(self, titan: TitrationAnalysis) -> None:
         """It applies dilution correction read from file listing additions."""
         assert titan.additions is not None
-        np.testing.assert_array_equal(titan.additions, [100, 2, 2, 2, 2, 2, 2])
+        assert_array_equal(titan.additions, [100, 2, 2, 2, 2, 2, 2])
         assert titan.data_dilutioncorrected is not None
         assert titan.data_dilutioncorrected[1] is not None
-        np.testing.assert_almost_equal(
+        assert_almost_equal(
             titan.data_dilutioncorrected[1]["A12"],
             [9758.25, 7524.795, 3079.18, 1414.04, 641.79, 402.325, 317.52],
         )
 
     def test_data_dilutioncorrected_norma(self, titan: TitrationAnalysis) -> None:
         """It normalizes data."""
         assert titan.data_dilutioncorrected_norm is not None
-        np.testing.assert_almost_equal(
+        assert_almost_equal(
             titan.data_dilutioncorrected_norm[0]["A12"][::2],
             [434.65, 878.73, 975.58, 829.46],
             2,
         )
-        np.testing.assert_almost_equal(
+        assert_almost_equal(
             titan.data_dilutioncorrected_norm[1]["A12"][::2],
             [871.272, 274.927, 57.303, 28.35],
             3,
         )
 
     def test_keys(self, titan: TitrationAnalysis) -> None:
         """It gets well positions for ctrl and unknown samples."""
```

### Comparing `clophfit-0.8.0/tests/EnSpire/24well_clop0_95.csv` & `clophfit-0.8.1/tests/EnSpire/24well_clop0_95.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/G10.csv` & `clophfit-0.8.1/tests/EnSpire/G10.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/NTT-G10_note.csv` & `clophfit-0.8.1/tests/EnSpire/NTT-G10_note.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/e2-T-without_sample_column.csv` & `clophfit-0.8.1/tests/EnSpire/e2-T-without_sample_column.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota` & `clophfit-0.8.1/tests/EnSpire/h148g-spettroC-nota`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota-Err` & `clophfit-0.8.1/tests/EnSpire/h148g-spettroC-nota-Err`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/h148g-spettroC-nota.csv` & `clophfit-0.8.1/tests/EnSpire/h148g-spettroC-nota.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/h148g-spettroC.csv` & `clophfit-0.8.1/tests/EnSpire/h148g-spettroC.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/cli/NTT_37C_pKa.csv` & `clophfit-0.8.1/tests/EnSpire/cli/NTT_37C_pKa.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv` & `clophfit-0.8.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png` & `clophfit-0.8.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv` & `clophfit-0.8.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png` & `clophfit-0.8.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv` & `clophfit-0.8.1/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv` & `clophfit-0.8.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv` & `clophfit-0.8.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv` & `clophfit-0.8.1/tests/EnSpire/exceptions/e2dan-emwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv` & `clophfit-0.8.1/tests/EnSpire/exceptions/e2dan-exwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv` & `clophfit-0.8.1/tests/EnSpire/exceptions/e2dan-exwavelength2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv` & `clophfit-0.8.1/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv` & `clophfit-0.8.1/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv` & `clophfit-0.8.1/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv` & `clophfit-0.8.1/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_100.xls` & `clophfit-0.8.1/tests/Tecan/290212_100.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_150.xls` & `clophfit-0.8.1/tests/Tecan/290212_150.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_20.xls` & `clophfit-0.8.1/tests/Tecan/290212_20.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_5.78.xls` & `clophfit-0.8.1/tests/Tecan/290212_5.78.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_50.xls` & `clophfit-0.8.1/tests/Tecan/290212_50.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_6.38.xls` & `clophfit-0.8.1/tests/Tecan/290212_6.38.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_6.83.xls` & `clophfit-0.8.1/tests/Tecan/290212_6.83.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_7.24.xls` & `clophfit-0.8.1/tests/Tecan/290212_7.24.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_7.67.xls` & `clophfit-0.8.1/tests/Tecan/290212_7.67.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_8.23.xls` & `clophfit-0.8.1/tests/Tecan/290212_8.23.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_8.82.xls` & `clophfit-0.8.1/tests/Tecan/290212_8.82.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290212_9.31.xls` & `clophfit-0.8.1/tests/Tecan/290212_9.31.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290513_5.5.xls` & `clophfit-0.8.1/tests/Tecan/290513_5.5.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290513_5.5_bad.xls` & `clophfit-0.8.1/tests/Tecan/290513_5.5_bad.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290513_7.2.xls` & `clophfit-0.8.1/tests/Tecan/290513_7.2.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/290513_8.8.xls` & `clophfit-0.8.1/tests/Tecan/290513_8.8.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/200214 pH data.ods` & `clophfit-0.8.1/tests/Tecan/140220/200214 pH data.ods`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/NaCl1_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/NaCl1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/NaCl2_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/NaCl2_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/NaCl3_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/NaCl3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/NaCl4_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/NaCl4_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/NaCl5_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/NaCl5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/NaCl6_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/NaCl6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/NaCl7_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/NaCl7_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/NaCl8_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/NaCl8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/fit0-1.csv` & `clophfit-0.8.1/tests/Tecan/140220/fit0-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/fit0.csv` & `clophfit-0.8.1/tests/Tecan/140220/fit0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/fit1-1.csv` & `clophfit-0.8.1/tests/Tecan/140220/fit1-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/fit1.csv` & `clophfit-0.8.1/tests/Tecan/140220/fit1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/pH5.0_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/pH5.0_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/pH5.8_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/pH5.8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/pH6.5_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/pH6.5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/pH7.1_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/pH7.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/pH7.6_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/pH7.6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/pH8.3_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/pH8.3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/140220/pH9.1_200214.xls` & `clophfit-0.8.1/tests/Tecan/140220/pH9.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx` & `clophfit-0.8.1/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls` & `clophfit-0.8.1/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/exceptions/84wells_290212_20.xlsx` & `clophfit-0.8.1/tests/Tecan/exceptions/84wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/Tecan/exceptions/88wells_290212_20.xlsx` & `clophfit-0.8.1/tests/Tecan/exceptions/88wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/A01-20140311a.dat` & `clophfit-0.8.1/tests/data/A01-20140311a.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/A01.dat` & `clophfit-0.8.1/tests/data/A01.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/NTT-A04-Cl_note` & `clophfit-0.8.1/tests/data/NTT-A04-Cl_note`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_A.csv` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_A.png` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_B.csv` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_B.png` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_C.csv` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_C.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_C.png` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_C.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_D.csv` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_D.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_D.png` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_D.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_E.csv` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_E.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_E.png` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_E.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_F.csv` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_F.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/Meas/A04 Cl_F.png` & `clophfit-0.8.1/tests/data/Meas/A04 Cl_F.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/k/D05.dat-bs.png` & `clophfit-0.8.1/tests/data/k/D05.dat-bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/k/D05.dat.png` & `clophfit-0.8.1/tests/data/k/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.8.1/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.8.1/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.8.1/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.8.1/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png` & `clophfit-0.8.1/tests/data/output/global/Cl/B05-20130628-cor.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/output/global/pH/D05.dat.png` & `clophfit-0.8.1/tests/data/output/global/pH/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/tmp/A04 Cl.csv` & `clophfit-0.8.1/tests/data/tmp/A04 Cl.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/tests/data/tmp/NTT-A04-Cl_note.csv` & `clophfit-0.8.1/tests/data/tmp/NTT-A04-Cl_note.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/.gitignore` & `clophfit-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/LICENSE.txt` & `clophfit-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.8.0/README.md` & `clophfit-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.8.0"
+- Version: "0.8.1"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/ClopHfit/)
 using `pip`:
 
     pip install clophfit
```

### Comparing `clophfit-0.8.0/pyproject.toml` & `clophfit-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,18 @@
 ]
 dependencies = [
   'click < 8.1.4',
   'corner < 2.2.3',
   'emcee < 3.1.5',
   'lmfit < 1.2.2',
   'matplotlib < 3.7.2',
-  'numpy < 1.24.4',
+  'numpy < 1.25.1',
   'openpyxl < 3.1.3',
-  'pandas < 2.0.3',
-  'rpy2 < 3.5.13',
-  'scipy < 1.10.2',
+  'pandas < 2.0.4',
+  'scipy < 1.11.2',
   'seaborn < 0.12.3',
   'sympy < 1.13.0',
   'tqdm < 4.65.1',
   'xlrd < 2.0.2'
 ]
 description = "Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra."
 keywords = [
@@ -44,53 +43,53 @@
   "macromolecule binding"
 ]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "clophfit"
 readme = "README.md"
 requires-python = ">=3.8, <3.12"
-version = "0.8.0"
+version = "0.8.1"
 
 [project.optional-dependencies]
 dev = [
-  "commitizen < 3.2.3",
+  "commitizen < 3.5.3",
   "ipykernel",
   "jupyter",
-  "ruff == 0.0.270",
+  "ruff == 0.0.275",
   "pylsp-mypy",
   "python-lsp-ruff"
 ]
 docs = [
   "autodocsumm == 0.2.11",
   # "myst-parser == 1.0.0",
   "nbsphinx == 0.9.2",
   "pydata-sphinx-theme == 0.13.3",
   "Sphinx == 7.0.1",
   "sphinx-click == 4.4.0",
-  "sphinx_autodoc_typehints == 1.23.0",
+  "sphinx_autodoc_typehints == 1.23.3",
   "sphinxcontrib-plantuml == 0.25"
 ]
 tests = [
   "coverage[toml] < 7.2.8",
-  "mypy < 1.4",
-  "pandas-stubs == 2.0.1.230501",
+  "mypy < 1.5",
+  "pandas-stubs == 2.0.2.230605",
   "Pygments < 2.15.2",
-  "pytest < 7.3.2",
+  "pytest < 7.4.1",
   "typeguard == 4.0.0",
   "xdoctest < 1.1.2"
 ]
 
 [project.scripts]
 "clop" = "clophfit.__main__:clop"
 "fit_titration_global_old" = "clophfit.old.fit_titration_global:main"
 "fit_titration_old" = "clophfit.old.fit_titration:main"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/darosio/ClopHfit/issues"
-Changelog = "https://darosio.github.io/ClopHfit/misc/CHANGELOG.html"
+Changelog = "https://github.com/darosio/ClopHfit/blob/main/CHANGELOG.md"
 Discussions = "https://github.com/darosio/ClopHfit/discussions"
 Documentation = "https://clophfit.readthedocs.io"
 "Github releases" = "https://github.com/darosio/ClopHfit/releases"
 Homepage = "https://github.com/darosio/ClopHfit"
 
 [tool.black]
 exclude = '''
@@ -108,15 +107,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.8.0"
+version = "0.8.1"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "README.md:Version"
 ]
 
 [tool.commitizen.customize]
```

### Comparing `clophfit-0.8.0/PKG-INFO` & `clophfit-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: clophfit
-Version: 0.8.0
+Version: 0.8.1
 Summary: Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra.
 Project-URL: Bug Tracker, https://github.com/darosio/ClopHfit/issues
-Project-URL: Changelog, https://darosio.github.io/ClopHfit/misc/CHANGELOG.html
+Project-URL: Changelog, https://github.com/darosio/ClopHfit/blob/main/CHANGELOG.md
 Project-URL: Discussions, https://github.com/darosio/ClopHfit/discussions
 Project-URL: Documentation, https://clophfit.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/ClopHfit/releases
 Project-URL: Homepage, https://github.com/darosio/ClopHfit
 Author-email: daniele arosio <daniele.arosio@cnr.it>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
@@ -25,44 +25,43 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.12,>=3.8
 Requires-Dist: click<8.1.4
 Requires-Dist: corner<2.2.3
 Requires-Dist: emcee<3.1.5
 Requires-Dist: lmfit<1.2.2
 Requires-Dist: matplotlib<3.7.2
-Requires-Dist: numpy<1.24.4
+Requires-Dist: numpy<1.25.1
 Requires-Dist: openpyxl<3.1.3
-Requires-Dist: pandas<2.0.3
-Requires-Dist: rpy2<3.5.13
-Requires-Dist: scipy<1.10.2
+Requires-Dist: pandas<2.0.4
+Requires-Dist: scipy<1.11.2
 Requires-Dist: seaborn<0.12.3
 Requires-Dist: sympy<1.13.0
 Requires-Dist: tqdm<4.65.1
 Requires-Dist: xlrd<2.0.2
 Provides-Extra: dev
-Requires-Dist: commitizen<3.2.3; extra == 'dev'
+Requires-Dist: commitizen<3.5.3; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
 Requires-Dist: python-lsp-ruff; extra == 'dev'
-Requires-Dist: ruff==0.0.270; extra == 'dev'
+Requires-Dist: ruff==0.0.275; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm==0.2.11; extra == 'docs'
 Requires-Dist: nbsphinx==0.9.2; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme==0.13.3; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints==1.23.0; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints==1.23.3; extra == 'docs'
 Requires-Dist: sphinx-click==4.4.0; extra == 'docs'
 Requires-Dist: sphinx==7.0.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-plantuml==0.25; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: coverage[toml]<7.2.8; extra == 'tests'
-Requires-Dist: mypy<1.4; extra == 'tests'
-Requires-Dist: pandas-stubs==2.0.1.230501; extra == 'tests'
+Requires-Dist: mypy<1.5; extra == 'tests'
+Requires-Dist: pandas-stubs==2.0.2.230605; extra == 'tests'
 Requires-Dist: pygments<2.15.2; extra == 'tests'
-Requires-Dist: pytest<7.3.2; extra == 'tests'
+Requires-Dist: pytest<7.4.1; extra == 'tests'
 Requires-Dist: typeguard==4.0.0; extra == 'tests'
 Requires-Dist: xdoctest<1.1.2; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # ClopHfit
 
 [![PyPI](https://img.shields.io/pypi/v/ClopHfit.svg)](https://pypi.org/project/ClopHfit/)
@@ -71,15 +70,15 @@
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.8.0"
+- Version: "0.8.1"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/ClopHfit/)
 using `pip`:
 
     pip install clophfit
```

