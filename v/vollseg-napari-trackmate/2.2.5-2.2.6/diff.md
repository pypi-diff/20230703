# Comparing `tmp/vollseg-napari-trackmate-2.2.5.tar.gz` & `tmp/vollseg-napari-trackmate-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vollseg-napari-trackmate-2.2.5.tar", last modified: Mon Jul  3 09:16:25 2023, max compression
+gzip compressed data, was "vollseg-napari-trackmate-2.2.6.tar", last modified: Mon Jul  3 09:26:41 2023, max compression
```

## Comparing `vollseg-napari-trackmate-2.2.5.tar` & `vollseg-napari-trackmate-2.2.6.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:25.441593 vollseg-napari-trackmate-2.2.5/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:12.829609 vollseg-napari-trackmate-2.2.5/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.893830 vollseg-napari-trackmate-2.2.5/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/.gitignore
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.962162 vollseg-napari-trackmate-2.2.5/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1532 2023-07-03 09:15:00.000000 vollseg-napari-trackmate-2.2.5/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      664 2023-07-01 10:58:54.000000 vollseg-napari-trackmate-2.2.5/.napari-hub/config.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1126 2023-07-03 08:35:47.000000 vollseg-napari-trackmate-2.2.5/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4241 2023-07-01 10:25:08.000000 vollseg-napari-trackmate-2.2.5/ALGORITHM.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4552 2023-07-03 09:16:25.444314 vollseg-napari-trackmate-2.2.5/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3129 2023-07-03 09:10:54.000000 vollseg-napari-trackmate-2.2.5/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:12.864332 vollseg-napari-trackmate-2.2.5/_build/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:15.095739 vollseg-napari-trackmate-2.2.5/_build/.doctrees/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:15.144206 vollseg-napari-trackmate-2.2.5/_build/.doctrees/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3648 2023-07-01 10:30:53.000000 vollseg-napari-trackmate-2.2.5/_build/.doctrees/.napari-hub/DESCRIPTION.doctree
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16944 2023-07-01 10:30:54.000000 vollseg-napari-trackmate-2.2.5/_build/.doctrees/ALGORITHM.doctree
--rwxrwxrwx   0 debian    (1000) debian    (1000)    12332 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/.doctrees/README.doctree
--rwxrwxrwx   0 debian    (1000) debian    (1000)    28014 2023-07-01 10:30:54.000000 vollseg-napari-trackmate-2.2.5/_build/.doctrees/environment.pickle
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:15.502832 vollseg-napari-trackmate-2.2.5/_build/html/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      230 2023-07-01 10:31:00.000000 vollseg-napari-trackmate-2.2.5/_build/html/.buildinfo
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:15.556958 vollseg-napari-trackmate-2.2.5/_build/html/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13482 2023-07-01 10:31:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/.napari-hub/DESCRIPTION.html
--rwxrwxrwx   0 debian    (1000) debian    (1000)    20268 2023-07-01 10:31:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/ALGORITHM.html
--rwxrwxrwx   0 debian    (1000) debian    (1000)    18199 2023-07-01 10:31:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/README.html
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:12.913043 vollseg-napari-trackmate-2.2.5/_build/html/_downloads/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:15.624772 vollseg-napari-trackmate-2.2.5/_build/html/_downloads/7304322522eb33b4c1d6fcd9b8dac0af/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2316 2023-07-01 10:25:41.000000 vollseg-napari-trackmate-2.2.5/_build/html/_downloads/7304322522eb33b4c1d6fcd9b8dac0af/apply_autoencoder.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:15.688398 vollseg-napari-trackmate-2.2.5/_build/html/_downloads/c74da13609f81dcb94d74f88327c6b07/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2320 2023-06-30 17:25:15.000000 vollseg-napari-trackmate-2.2.5/_build/html/_downloads/c74da13609f81dcb94d74f88327c6b07/visualize_point_clouds.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:15.739737 vollseg-napari-trackmate-2.2.5/_build/html/_images/
--rwxrwxrwx   0 debian    (1000) debian    (1000)   403746 2023-06-30 17:11:11.000000 vollseg-napari-trackmate-2.2.5/_build/html/_images/point_clouds_compared.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:15.856064 vollseg-napari-trackmate-2.2.5/_build/html/_sources/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:15.920884 vollseg-napari-trackmate-2.2.5/_build/html/_sources/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      461 2023-07-01 10:31:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_sources/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4241 2023-07-01 10:25:08.000000 vollseg-napari-trackmate-2.2.5/_build/html/_sources/ALGORITHM.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/_build/html/_sources/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:16.025685 vollseg-napari-trackmate-2.2.5/_build/html/_sphinx_design_static/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    48417 2023-06-30 17:20:26.000000 vollseg-napari-trackmate-2.2.5/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)      770 2023-06-30 17:20:26.000000 vollseg-napari-trackmate-2.2.5/_build/html/_sphinx_design_static/design-tabs.js
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:17.412245 vollseg-napari-trackmate-2.2.5/_build/html/_static/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14693 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/basic.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)      313 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/check-solid.svg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     9032 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/clipboard.min.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)      411 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/copy-button.svg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2060 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/copybutton.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)     8468 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/copybutton.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2698 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/copybutton_funcs.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)    48417 2023-06-30 17:20:26.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)      770 2023-06-30 17:20:26.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/design-tabs.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10766 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/doctools.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)      413 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/documentation_options.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)      286 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/file.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:17.647526 vollseg-napari-trackmate-2.2.5/_build/html/_static/images/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1186 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/images/logo_binder.svg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7601 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/images/logo_colab.png
--rwxrwxrwx   0 debian    (1000) debian    (1000)      681 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/images/logo_deepnote.svg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1758 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/images/logo_jupyterhub.svg
--rwxrwxrwx   0 debian    (1000) debian    (1000)   287630 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/jquery-3.5.1.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)    89476 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/jquery.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10852 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/language_data.js
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.427960 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.030511 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ar/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:17.730122 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ar/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1459 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.061402 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/bg/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:17.808810 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/bg/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1626 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.091480 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/bn/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:17.888585 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/bn/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1564 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.118945 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ca/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:17.971454 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ca/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1166 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.151388 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/cs/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.053951 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/cs/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1323 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.184716 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/da/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.132108 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/da/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1222 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.215224 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/de/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.227039 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/de/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1306 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.249067 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/el/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.317757 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/el/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1640 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.281659 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/eo/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.413646 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/eo/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1255 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.313552 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/es/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.511825 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/es/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1314 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.344484 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/et/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.618052 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/et/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1259 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.375846 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/fi/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.719564 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/fi/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1286 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.415579 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/fr/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.833394 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/fr/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1330 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.452313 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/hr/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:18.944957 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/hr/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1320 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.486334 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/id/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:19.049185 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/id/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.517220 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/it/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:19.167519 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/it/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1321 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.553048 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/iw/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:19.267315 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/iw/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1363 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.583828 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ja/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:19.371063 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ja/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1389 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.614564 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ko/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:19.472848 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ko/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1293 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.644199 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/lt/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:19.574783 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/lt/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1331 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.675634 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/lv/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:19.680076 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/lv/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1322 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.708922 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ml/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:19.790171 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ml/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1803 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.736539 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/mr/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:19.901629 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/mr/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1594 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.768900 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ms/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.015306 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ms/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1133 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.798195 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/nl/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.119576 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/nl/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1274 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.829564 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/no/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.219134 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/no/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1235 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.861876 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/pl/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.332329 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/pl/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1289 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.893160 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/pt/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.448243 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/pt/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1282 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.924470 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ro/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.558033 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ro/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1308 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.955203 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ru/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.661303 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ru/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1640 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:13.985744 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sk/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.761062 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sk/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1311 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.018128 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sl/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.860382 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sl/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.053221 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sr/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:20.951774 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sr/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1597 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.083625 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sv/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.051712 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sv/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1267 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.112579 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ta/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.158628 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ta/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1848 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.144937 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/te/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.269928 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/te/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1726 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.178610 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tg/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.368382 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tg/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1546 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.211956 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/th/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.467110 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/th/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1684 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.243666 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tl/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.570337 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tl/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1193 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.274789 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tr/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.674237 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tr/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1291 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.305284 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/uk/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.780521 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/uk/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1601 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.334468 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ur/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.886612 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ur/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1382 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.369764 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/vi/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:21.991576 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/vi/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1349 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.403154 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/zh_CN/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:22.114270 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/zh_CN/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1228 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.436366 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/zh_TW/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:22.246660 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/zh_TW/LC_MESSAGES/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1259 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rwxrwxrwx   0 debian    (1000) debian    (1000)       90 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/minus.png
--rwxrwxrwx   0 debian    (1000) debian    (1000)    39364 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)       90 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/plus.png
--rwxrwxrwx   0 debian    (1000) debian    (1000)    12758 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/pygments.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)      419 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/sbt-webpack-macros.html
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:22.854231 vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    80814 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/bootstrap.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)      237 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)   335758 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/bootstrap.js.map
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4457 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/pydata-sphinx-theme.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)    19649 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/pydata-sphinx-theme.js.map
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3076 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/sphinx-book-theme.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13067 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/sphinx-book-theme.js.map
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16634 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/searchtools.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2234 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/sphinx-thebe.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3986 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/sphinx-thebe.js
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:23.147538 vollseg-napari-trackmate-2.2.5/_build/html/_static/styles/
--rwxrwxrwx   0 debian    (1000) debian    (1000)   176655 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/styles/bootstrap.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)    63342 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/styles/pydata-sphinx-theme.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13842 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/styles/sphinx-book-theme.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)      106 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/styles/theme.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3728 2023-07-01 10:31:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/togglebutton.css
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7334 2023-07-01 10:31:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/togglebutton.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)    68420 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/underscore-1.13.1.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)    19531 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/underscore.js
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.496967 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.503962 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:23.228175 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7427 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:23.338907 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/css/
--rwxrwxrwx   0 debian    (1000) debian    (1000)   101692 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:24.191866 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rwxrwxrwx   0 debian    (1000) debian    (1000)   181264 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rwxrwxrwx   0 debian    (1000) debian    (1000)   105112 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rwxrwxrwx   0 debian    (1000) debian    (1000)    60236 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rwxrwxrwx   0 debian    (1000) debian    (1000)    24028 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rwxrwxrwx   0 debian    (1000) debian    (1000)   389948 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rwxrwxrwx   0 debian    (1000) debian    (1000)   154840 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10084 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4776 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1864 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/_static/webpack-macros.html
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10554 2023-07-01 10:31:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/genindex.html
--rwxrwxrwx   0 debian    (1000) debian    (1000)       59 2023-06-30 17:20:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/index.html
--rwxrwxrwx   0 debian    (1000) debian    (1000)      297 2023-07-01 10:31:00.000000 vollseg-napari-trackmate-2.2.5/_build/html/objects.inv
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11437 2023-07-01 10:31:35.000000 vollseg-napari-trackmate-2.2.5/_build/html/search.html
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2745 2023-07-01 10:31:32.000000 vollseg-napari-trackmate-2.2.5/_build/html/searchindex.js
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1089 2023-06-30 17:31:08.000000 vollseg-napari-trackmate-2.2.5/_config.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      150 2023-07-01 10:32:10.000000 vollseg-napari-trackmate-2.2.5/_toc.yml
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:24.285317 vollseg-napari-trackmate-2.2.5/examples/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2316 2023-07-01 10:25:41.000000 vollseg-napari-trackmate-2.2.5/examples/apply_autoencoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2320 2023-06-30 17:25:15.000000 vollseg-napari-trackmate-2.2.5/examples/visualize_point_clouds.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:24.356588 vollseg-napari-trackmate-2.2.5/images/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2023-06-30 17:14:02.000000 vollseg-napari-trackmate-2.2.5/images/kapoorlogo.png
--rwxrwxrwx   0 debian    (1000) debian    (1000)   403746 2023-06-30 17:11:11.000000 vollseg-napari-trackmate-2.2.5/images/point_clouds_compared.png
--rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1896 2023-07-03 09:16:25.454145 vollseg-napari-trackmate-2.2.5/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:14.585901 vollseg-napari-trackmate-2.2.5/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:24.753956 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_data_model.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:25.330900 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_tests/test_reader.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_tests/test_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_tests/test_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-07-03 09:15:59.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    82705 2023-07-03 09:13:06.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/launch.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/napari.yaml
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:25.391570 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/resources/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:16:25.029107 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4552 2023-07-03 09:16:00.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7223 2023-07-03 09:16:12.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-03 09:16:00.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-07-03 09:16:00.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       93 2023-07-03 09:16:00.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-03 09:16:00.000000 vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.5/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:41.646148 vollseg-napari-trackmate-2.2.6/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.390399 vollseg-napari-trackmate-2.2.6/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.895997 vollseg-napari-trackmate-2.2.6/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.983237 vollseg-napari-trackmate-2.2.6/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1532 2023-07-03 09:15:00.000000 vollseg-napari-trackmate-2.2.6/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      664 2023-07-01 10:58:54.000000 vollseg-napari-trackmate-2.2.6/.napari-hub/config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1126 2023-07-03 08:35:47.000000 vollseg-napari-trackmate-2.2.6/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4241 2023-07-01 10:25:08.000000 vollseg-napari-trackmate-2.2.6/ALGORITHM.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4552 2023-07-03 09:26:41.648581 vollseg-napari-trackmate-2.2.6/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3129 2023-07-03 09:10:54.000000 vollseg-napari-trackmate-2.2.6/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.431645 vollseg-napari-trackmate-2.2.6/_build/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:30.128256 vollseg-napari-trackmate-2.2.6/_build/.doctrees/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:30.184781 vollseg-napari-trackmate-2.2.6/_build/.doctrees/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     8139 2023-07-03 09:20:27.000000 vollseg-napari-trackmate-2.2.6/_build/.doctrees/.napari-hub/DESCRIPTION.doctree
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16944 2023-07-03 09:20:27.000000 vollseg-napari-trackmate-2.2.6/_build/.doctrees/ALGORITHM.doctree
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    12814 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/.doctrees/README.doctree
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    29911 2023-07-03 09:20:27.000000 vollseg-napari-trackmate-2.2.6/_build/.doctrees/environment.pickle
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:30.621683 vollseg-napari-trackmate-2.2.6/_build/html/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      230 2023-07-03 09:20:33.000000 vollseg-napari-trackmate-2.2.6/_build/html/.buildinfo
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:30.674462 vollseg-napari-trackmate-2.2.6/_build/html/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16783 2023-07-03 09:24:56.000000 vollseg-napari-trackmate-2.2.6/_build/html/.napari-hub/DESCRIPTION.html
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    20268 2023-07-03 09:24:56.000000 vollseg-napari-trackmate-2.2.6/_build/html/ALGORITHM.html
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    18410 2023-07-03 09:24:56.000000 vollseg-napari-trackmate-2.2.6/_build/html/README.html
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.476530 vollseg-napari-trackmate-2.2.6/_build/html/_downloads/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:30.736662 vollseg-napari-trackmate-2.2.6/_build/html/_downloads/7304322522eb33b4c1d6fcd9b8dac0af/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2316 2023-07-01 10:25:41.000000 vollseg-napari-trackmate-2.2.6/_build/html/_downloads/7304322522eb33b4c1d6fcd9b8dac0af/apply_autoencoder.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:30.801779 vollseg-napari-trackmate-2.2.6/_build/html/_downloads/c74da13609f81dcb94d74f88327c6b07/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2320 2023-06-30 17:25:15.000000 vollseg-napari-trackmate-2.2.6/_build/html/_downloads/c74da13609f81dcb94d74f88327c6b07/visualize_point_clouds.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:30.863488 vollseg-napari-trackmate-2.2.6/_build/html/_images/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   403746 2023-06-30 17:11:11.000000 vollseg-napari-trackmate-2.2.6/_build/html/_images/point_clouds_compared.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:30.984194 vollseg-napari-trackmate-2.2.6/_build/html/_sources/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:31.044036 vollseg-napari-trackmate-2.2.6/_build/html/_sources/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1530 2023-07-03 09:24:56.000000 vollseg-napari-trackmate-2.2.6/_build/html/_sources/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4241 2023-07-01 10:25:08.000000 vollseg-napari-trackmate-2.2.6/_build/html/_sources/ALGORITHM.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3129 2023-07-03 09:10:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_sources/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:31.131984 vollseg-napari-trackmate-2.2.6/_build/html/_sphinx_design_static/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    48417 2023-06-30 17:20:26.000000 vollseg-napari-trackmate-2.2.6/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      770 2023-06-30 17:20:26.000000 vollseg-napari-trackmate-2.2.6/_build/html/_sphinx_design_static/design-tabs.js
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:32.716023 vollseg-napari-trackmate-2.2.6/_build/html/_static/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    14693 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/basic.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      313 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/check-solid.svg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     9032 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/clipboard.min.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      411 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/copy-button.svg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2060 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/copybutton.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     8468 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/copybutton.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2698 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/copybutton_funcs.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    48417 2023-06-30 17:20:26.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      770 2023-06-30 17:20:26.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/design-tabs.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10766 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/doctools.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      413 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/documentation_options.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      286 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/file.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:33.077405 vollseg-napari-trackmate-2.2.6/_build/html/_static/images/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1186 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/images/logo_binder.svg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7601 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/images/logo_colab.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      681 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/images/logo_deepnote.svg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1758 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/images/logo_jupyterhub.svg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   287630 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/jquery-3.5.1.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    89476 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/jquery.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10852 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/language_data.js
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.250894 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.597085 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ar/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:33.195846 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ar/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1459 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.629513 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/bg/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:33.318218 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/bg/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1626 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.656295 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/bn/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:33.452984 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/bn/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1564 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.691309 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ca/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:33.594237 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ca/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1166 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.730815 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/cs/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:33.739100 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/cs/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1323 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.772127 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/da/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:33.873204 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/da/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1222 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.808931 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/de/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:34.012123 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/de/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1306 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.848195 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/el/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:34.152994 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/el/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1640 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.896542 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/eo/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:34.266625 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/eo/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1255 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.943228 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/es/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:34.379621 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/es/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1314 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:27.998727 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/et/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:34.490954 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/et/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1259 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.035269 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/fi/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:34.614258 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/fi/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1286 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.079227 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/fr/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:34.732907 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/fr/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1330 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.117459 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/hr/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:34.842507 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/hr/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1320 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.157278 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/id/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:34.949298 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/id/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.190824 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/it/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:35.065453 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/it/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1321 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.223832 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/iw/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:35.186115 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/iw/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1363 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.258783 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ja/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:35.310448 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ja/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1389 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.292400 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ko/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:35.428758 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ko/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1293 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.324044 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/lt/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:35.544931 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/lt/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1331 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.354358 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/lv/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:35.657067 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/lv/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1322 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.387468 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ml/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:35.778771 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ml/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1803 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.421757 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/mr/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:35.902651 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/mr/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1594 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.454214 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ms/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:36.017682 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ms/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1133 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.488705 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/nl/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:36.184545 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/nl/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1274 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.537826 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/no/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:36.298642 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/no/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1235 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.575576 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/pl/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:36.420330 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/pl/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1289 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.611341 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/pt/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:36.544849 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/pt/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1282 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.647247 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ro/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:36.679881 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ro/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1308 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.703004 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ru/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:36.819895 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ru/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1640 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.737602 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sk/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:36.954882 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sk/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1311 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.780512 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sl/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:37.074962 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sl/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.819681 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sr/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:37.197587 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sr/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1597 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.851586 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sv/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:37.323959 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sv/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1267 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.886659 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ta/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:37.451976 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ta/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1848 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.927543 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/te/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:37.569043 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/te/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1726 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:28.983690 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tg/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:37.684265 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tg/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1546 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.022110 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/th/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:37.794082 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/th/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1684 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.057973 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tl/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:37.902711 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tl/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1193 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.091983 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tr/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:38.007890 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tr/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1291 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.122655 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/uk/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:38.111414 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/uk/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1601 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.151853 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ur/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:38.211247 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ur/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1382 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.185893 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/vi/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:38.302822 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/vi/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1349 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.220155 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/zh_CN/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:38.398562 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/zh_CN/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1228 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.262113 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/zh_TW/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:38.498511 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/zh_TW/LC_MESSAGES/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1259 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       90 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/minus.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    39364 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       90 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/plus.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    12758 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/pygments.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      419 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/sbt-webpack-macros.html
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:39.039456 vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    80814 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/bootstrap.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      237 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   335758 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/bootstrap.js.map
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4457 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/pydata-sphinx-theme.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    19649 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3076 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/sphinx-book-theme.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13067 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/sphinx-book-theme.js.map
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16634 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/searchtools.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2234 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/sphinx-thebe.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3986 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/sphinx-thebe.js
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:39.333907 vollseg-napari-trackmate-2.2.6/_build/html/_static/styles/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   176655 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/styles/bootstrap.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    63342 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/styles/pydata-sphinx-theme.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13842 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/styles/sphinx-book-theme.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      106 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/styles/theme.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3728 2023-07-03 09:24:56.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/togglebutton.css
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7334 2023-07-03 09:24:56.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/togglebutton.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    68420 2023-06-17 19:46:55.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/underscore-1.13.1.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    19531 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/underscore.js
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.331717 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.340575 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:39.410150 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7427 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:39.499907 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/css/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   101692 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:40.279190 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   181264 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   105112 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    60236 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    24028 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   389948 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   154840 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10084 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4776 2023-06-30 17:17:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1864 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/_static/webpack-macros.html
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10554 2023-07-03 09:24:56.000000 vollseg-napari-trackmate-2.2.6/_build/html/genindex.html
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       59 2023-06-30 17:20:35.000000 vollseg-napari-trackmate-2.2.6/_build/html/index.html
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      297 2023-07-03 09:20:33.000000 vollseg-napari-trackmate-2.2.6/_build/html/objects.inv
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11437 2023-07-03 09:24:56.000000 vollseg-napari-trackmate-2.2.6/_build/html/search.html
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3269 2023-07-03 09:24:54.000000 vollseg-napari-trackmate-2.2.6/_build/html/searchindex.js
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1089 2023-06-30 17:31:08.000000 vollseg-napari-trackmate-2.2.6/_config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      150 2023-07-01 10:32:10.000000 vollseg-napari-trackmate-2.2.6/_toc.yml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:40.364303 vollseg-napari-trackmate-2.2.6/examples/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2316 2023-07-01 10:25:41.000000 vollseg-napari-trackmate-2.2.6/examples/apply_autoencoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2320 2023-06-30 17:25:15.000000 vollseg-napari-trackmate-2.2.6/examples/visualize_point_clouds.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:40.431942 vollseg-napari-trackmate-2.2.6/images/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2023-06-30 17:14:02.000000 vollseg-napari-trackmate-2.2.6/images/kapoorlogo.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   403746 2023-06-30 17:11:11.000000 vollseg-napari-trackmate-2.2.6/images/point_clouds_compared.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1896 2023-07-03 09:26:41.660199 vollseg-napari-trackmate-2.2.6/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:29.439996 vollseg-napari-trackmate-2.2.6/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:40.862053 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_data_model.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:41.513914 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-07-03 09:26:13.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    82702 2023-07-03 09:24:15.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/launch.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:41.583790 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 09:26:41.181533 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4552 2023-07-03 09:26:14.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7223 2023-07-03 09:26:27.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-03 09:26:14.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-07-03 09:26:14.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       93 2023-07-03 09:26:14.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-03 09:26:14.000000 vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.2.6/tox.ini
```

### Comparing `vollseg-napari-trackmate-2.2.5/.github/workflows/test_and_deploy.yml` & `vollseg-napari-trackmate-2.2.6/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/.gitignore` & `vollseg-napari-trackmate-2.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/.napari-hub/DESCRIPTION.md` & `vollseg-napari-trackmate-2.2.6/.napari-hub/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/.napari-hub/config.yml` & `vollseg-napari-trackmate-2.2.6/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/.pre-commit-config.yaml` & `vollseg-napari-trackmate-2.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/ALGORITHM.md` & `vollseg-napari-trackmate-2.2.6/ALGORITHM.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/LICENSE` & `vollseg-napari-trackmate-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/PKG-INFO` & `vollseg-napari-trackmate-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.2.5
+Version: 2.2.6
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.2.5/README.md` & `vollseg-napari-trackmate-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/.doctrees/ALGORITHM.doctree` & `vollseg-napari-trackmate-2.2.6/_build/.doctrees/ALGORITHM.doctree`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/.doctrees/README.doctree` & `vollseg-napari-trackmate-2.2.6/_build/.doctrees/README.doctree`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9520 3000 0000 0000 008c 0f73 7068  ... 0........sph
+00000000: 8005 9502 3200 0000 0000 008c 0f73 7068  ....2........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
 00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
 00000060: 7365 6374 696f 6e94 9394 2981 947d 9428  section...)..}.(
 00000070: 6805 6806 6807 5d94 2868 098c 0574 6974  h.h.h.].(h...tit
@@ -236,536 +236,566 @@
 00000eb0: 7568 2b68 2d68 1e4b 0a68 1d68 2c68 1b68  uh+h-h.K.h.h,h.h
 00000ec0: 0c68 1c68 0375 6268 098c 0a74 7261 6e73  .h.h.ubh...trans
 00000ed0: 6974 696f 6e94 9394 2981 947d 9428 6805  ition...)..}.(h.
 00000ee0: 6806 6807 5d94 681f 7d94 2868 215d 9468  h.h.].h.}.(h!].h
 00000ef0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
 00000f00: 682b 68e8 681e 4b0c 681d 682c 681b 680c  h+h.h.K.h.h,h.h.
 00000f10: 681c 6803 7562 682e 2981 947d 9428 6805  h.h.ubh.)..}.(h.
-00000f20: 8c6f 5468 6973 205b 6e61 7061 7269 5d20  .oThis [napari] 
-00000f30: 706c 7567 696e 2077 6173 2067 656e 6572  plugin was gener
-00000f40: 6174 6564 2077 6974 6820 5b43 6f6f 6b69  ated with [Cooki
-00000f50: 6563 7574 7465 725d 2075 7369 6e67 205b  ecutter] using [
-00000f60: 406e 6170 6172 695d 2773 205b 636f 6f6b  @napari]'s [cook
-00000f70: 6965 6375 7474 6572 2d6e 6170 6172 692d  iecutter-napari-
-00000f80: 706c 7567 696e 5d20 7465 6d70 6c61 7465  plugin] template
-00000f90: 2e94 6807 5d94 2868 168c 0554 6869 7320  ..h.].(h...This 
-00000fa0: 9485 9481 947d 9428 6805 6806 681b 68f3  .....}.(h.h.h.h.
-00000fb0: 681c 6803 681d 4e68 1e4e 7562 6834 2981  h.h.h.Nh.Nubh4).
-00000fc0: 947d 9428 6805 8c06 6e61 7061 7269 9468  .}.(h...napari.h
-00000fd0: 075d 9468 168c 066e 6170 6172 6994 8594  .].h...napari...
-00000fe0: 8194 7d94 2868 0568 0668 1b68 fb68 1c68  ..}.(h.h.h.h.h.h
-00000ff0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00001000: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00001010: 295d 9468 508c 2068 7474 7073 3a2f 2f67  )].hP. https://g
-00001020: 6974 6875 622e 636f 6d2f 6e61 7061 7269  ithub.com/napari
-00001030: 2f6e 6170 6172 6994 7568 2b68 3368 1e4b  /napari.uh+h3h.K
-00001040: 0e68 1d68 2c68 1b68 f368 1c68 0375 6268  .h.h,h.h.h.h.ubh
-00001050: 168c 1b20 706c 7567 696e 2077 6173 2067  ... plugin was g
-00001060: 656e 6572 6174 6564 2077 6974 6820 9485  enerated with ..
-00001070: 9481 947d 9428 6805 6806 681b 68f3 681c  ...}.(h.h.h.h.h.
-00001080: 6803 681d 4e68 1e4e 7562 6834 2981 947d  h.h.Nh.Nubh4)..}
-00001090: 9428 6805 8c0c 436f 6f6b 6965 6375 7474  .(h...Cookiecutt
-000010a0: 6572 9468 075d 9468 168c 0c43 6f6f 6b69  er.h.].h...Cooki
-000010b0: 6563 7574 7465 7294 8594 8194 7d94 2868  ecutter.....}.(h
-000010c0: 0568 0668 1b6a 0e01 0000 681c 6803 681d  .h.h.j....h.h.h.
-000010d0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-000010e0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000010f0: 6850 8c27 6874 7470 733a 2f2f 6769 7468  hP.'https://gith
-00001100: 7562 2e63 6f6d 2f61 7564 7265 7972 2f63  ub.com/audreyr/c
-00001110: 6f6f 6b69 6563 7574 7465 7294 7568 2b68  ookiecutter.uh+h
-00001120: 3368 1e4b 0e68 1d68 2c68 1b68 f368 1c68  3h.K.h.h,h.h.h.h
-00001130: 0375 6268 168c 0720 7573 696e 6720 9485  .ubh... using ..
-00001140: 9481 947d 9428 6805 6806 681b 68f3 681c  ...}.(h.h.h.h.h.
-00001150: 6803 681d 4e68 1e4e 7562 6834 2981 947d  h.h.Nh.Nubh4)..}
-00001160: 9428 6805 8c07 406e 6170 6172 6994 6807  .(h...@napari.h.
-00001170: 5d94 6816 8c07 406e 6170 6172 6994 8594  ].h...@napari...
-00001180: 8194 7d94 2868 0568 0668 1b6a 2101 0000  ..}.(h.h.h.j!...
-00001190: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-000011a0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000011b0: 5d94 6829 5d94 6850 8c19 6874 7470 733a  ].h)].hP..https:
-000011c0: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6170  //github.com/nap
-000011d0: 6172 6994 7568 2b68 3368 1e4b 0e68 1d68  ari.uh+h3h.K.h.h
-000011e0: 2c68 1b68 f368 1c68 0375 6268 168c 05e2  ,h.h.h.h.ubh....
-000011f0: 8099 7320 9485 9481 947d 9428 6805 6806  ..s .....}.(h.h.
-00001200: 681b 68f3 681c 6803 681d 4e68 1e4e 7562  h.h.h.h.h.Nh.Nub
-00001210: 6834 2981 947d 9428 6805 8c1a 636f 6f6b  h4)..}.(h...cook
-00001220: 6965 6375 7474 6572 2d6e 6170 6172 692d  iecutter-napari-
-00001230: 706c 7567 696e 9468 075d 9468 168c 1a63  plugin.h.].h...c
-00001240: 6f6f 6b69 6563 7574 7465 722d 6e61 7061  ookiecutter-napa
-00001250: 7269 2d70 6c75 6769 6e94 8594 8194 7d94  ri-plugin.....}.
-00001260: 2868 0568 0668 1b6a 3401 0000 681c 6803  (h.h.h.j4...h.h.
-00001270: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00001280: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00001290: 5d94 6850 8c34 6874 7470 733a 2f2f 6769  ].hP.4https://gi
-000012a0: 7468 7562 2e63 6f6d 2f6e 6170 6172 692f  thub.com/napari/
-000012b0: 636f 6f6b 6965 6375 7474 6572 2d6e 6170  cookiecutter-nap
-000012c0: 6172 692d 706c 7567 696e 9475 682b 6833  ari-plugin.uh+h3
-000012d0: 681e 4b0e 681d 682c 681b 68f3 681c 6803  h.K.h.h,h.h.h.h.
-000012e0: 7562 6816 8c0a 2074 656d 706c 6174 652e  ubh... template.
-000012f0: 9485 9481 947d 9428 6805 6806 681b 68f3  .....}.(h.h.h.h.
-00001300: 681c 6803 681d 4e68 1e4e 7562 6568 1f7d  h.h.h.Nh.Nubeh.}
-00001310: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00001320: 5d94 6829 5d94 7568 2b68 2d68 1e4b 0e68  ].h)].uh+h-h.K.h
-00001330: 1d68 2c68 1b68 0c68 1c68 0375 6268 098c  .h,h.h.h.h.ubh..
-00001340: 0372 6177 9493 9429 8194 7d94 2868 058c  .raw...)..}.(h..
-00001350: f43c 212d 2d0a 446f 6e27 7420 6d69 7373  .<!--.Don't miss
-00001360: 2074 6865 2066 756c 6c20 6765 7474 696e   the full gettin
-00001370: 6720 7374 6172 7465 6420 6775 6964 6520  g started guide 
-00001380: 746f 2073 6574 2075 7020 796f 7572 206e  to set up your n
-00001390: 6577 2070 6163 6b61 6765 3a0a 6874 7470  ew package:.http
-000013a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
-000013b0: 6170 6172 692f 636f 6f6b 6965 6375 7474  apari/cookiecutt
-000013c0: 6572 2d6e 6170 6172 692d 706c 7567 696e  er-napari-plugin
-000013d0: 2367 6574 7469 6e67 2d73 7461 7274 6564  #getting-started
-000013e0: 0a0a 616e 6420 7265 7669 6577 2074 6865  ..and review the
-000013f0: 206e 6170 6172 6920 646f 6373 2066 6f72   napari docs for
-00001400: 2070 6c75 6769 6e20 6465 7665 6c6f 7065   plugin develope
-00001410: 7273 3a0a 6874 7470 733a 2f2f 6e61 7061  rs:.https://napa
-00001420: 7269 2e6f 7267 2f73 7461 626c 652f 706c  ri.org/stable/pl
-00001430: 7567 696e 732f 696e 6465 782e 6874 6d6c  ugins/index.html
-00001440: 0a2d 2d3e 0a94 6807 5d94 6816 8cf4 3c21  .-->..h.].h...<!
-00001450: 2d2d 0a44 6f6e 2774 206d 6973 7320 7468  --.Don't miss th
-00001460: 6520 6675 6c6c 2067 6574 7469 6e67 2073  e full getting s
-00001470: 7461 7274 6564 2067 7569 6465 2074 6f20  tarted guide to 
-00001480: 7365 7420 7570 2079 6f75 7220 6e65 7720  set up your new 
-00001490: 7061 636b 6167 653a 0a68 7474 7073 3a2f  package:.https:/
-000014a0: 2f67 6974 6875 622e 636f 6d2f 6e61 7061  /github.com/napa
-000014b0: 7269 2f63 6f6f 6b69 6563 7574 7465 722d  ri/cookiecutter-
-000014c0: 6e61 7061 7269 2d70 6c75 6769 6e23 6765  napari-plugin#ge
-000014d0: 7474 696e 672d 7374 6172 7465 640a 0a61  tting-started..a
-000014e0: 6e64 2072 6576 6965 7720 7468 6520 6e61  nd review the na
-000014f0: 7061 7269 2064 6f63 7320 666f 7220 706c  pari docs for pl
-00001500: 7567 696e 2064 6576 656c 6f70 6572 733a  ugin developers:
-00001510: 0a68 7474 7073 3a2f 2f6e 6170 6172 692e  .https://napari.
-00001520: 6f72 672f 7374 6162 6c65 2f70 6c75 6769  org/stable/plugi
-00001530: 6e73 2f69 6e64 6578 2e68 746d 6c0a 2d2d  ns/index.html.--
-00001540: 3e0a 9485 9481 947d 9428 6805 6806 681b  >......}.(h.h.h.
-00001550: 6a4f 0100 0075 6261 681f 7d94 2868 215d  jO...ubah.}.(h!]
-00001560: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001570: 948c 0666 6f72 6d61 7494 8c04 6874 6d6c  ...format...html
-00001580: 948c 0978 6d6c 3a73 7061 6365 948c 0870  ...xml:space...p
-00001590: 7265 7365 7276 6594 7568 2b6a 4d01 0000  reserve.uh+jM...
-000015a0: 681d 682c 681e 4b10 681b 680c 681c 6803  h.h,h.K.h.h.h.h.
-000015b0: 7562 680b 2981 947d 9428 6805 6806 6807  ubh.)..}.(h.h.h.
-000015c0: 5d94 2868 1029 8194 7d94 2868 058c 0c49  ].(h.)..}.(h...I
-000015d0: 6e73 7461 6c6c 6174 696f 6e94 6807 5d94  nstallation.h.].
-000015e0: 6816 8c0c 496e 7374 616c 6c61 7469 6f6e  h...Installation
-000015f0: 9485 9481 947d 9428 6805 6806 681b 6a64  .....}.(h.h.h.jd
-00001600: 0100 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00001610: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00001620: 9468 275d 9468 295d 9475 682b 680f 681e  .h'].h)].uh+h.h.
-00001630: 4b18 681d 682c 681b 6a61 0100 0068 1c68  K.h.h,h.ja...h.h
-00001640: 0375 6268 2e29 8194 7d94 2868 058c 3559  .ubh.)..}.(h..5Y
-00001650: 6f75 2063 616e 2069 6e73 7461 6c6c 2060  ou can install `
-00001660: 766f 6c6c 7365 672d 6e61 7061 7269 2d74  vollseg-napari-t
-00001670: 7261 636b 6d61 7465 6020 7669 6120 5b70  rackmate` via [p
-00001680: 6970 5d3a 9468 075d 9428 6816 8c10 596f  ip]:.h.].(h...Yo
-00001690: 7520 6361 6e20 696e 7374 616c 6c20 9485  u can install ..
-000016a0: 9481 947d 9428 6805 6806 681b 6a72 0100  ...}.(h.h.h.jr..
-000016b0: 0068 1c68 0368 1d4e 681e 4e75 6268 098c  .h.h.h.Nh.Nubh..
-000016c0: 076c 6974 6572 616c 9493 9429 8194 7d94  .literal...)..}.
-000016d0: 2868 058c 1876 6f6c 6c73 6567 2d6e 6170  (h...vollseg-nap
-000016e0: 6172 692d 7472 6163 6b6d 6174 6594 6807  ari-trackmate.h.
-000016f0: 5d94 6816 8c18 766f 6c6c 7365 672d 6e61  ].h...vollseg-na
-00001700: 7061 7269 2d74 7261 636b 6d61 7465 9485  pari-trackmate..
-00001710: 9481 947d 9428 6805 6806 681b 6a7c 0100  ...}.(h.h.h.j|..
-00001720: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00001730: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00001740: 275d 9468 295d 9475 682b 6a7a 0100 0068  '].h)].uh+jz...h
-00001750: 1e4b 1a68 1d68 2c68 1b6a 7201 0000 681c  .K.h.h,h.jr...h.
-00001760: 6803 7562 6816 8c05 2076 6961 2094 8594  h.ubh... via ...
-00001770: 8194 7d94 2868 0568 0668 1b6a 7201 0000  ..}.(h.h.h.jr...
-00001780: 681c 6803 681d 4e68 1e4e 7562 6834 2981  h.h.h.Nh.Nubh4).
-00001790: 947d 9428 6805 8c03 7069 7094 6807 5d94  .}.(h...pip.h.].
-000017a0: 6816 8c03 7069 7094 8594 8194 7d94 2868  h...pip.....}.(h
-000017b0: 0568 0668 1b6a 8e01 0000 681c 6803 681d  .h.h.j....h.h.h.
-000017c0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-000017d0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000017e0: 6850 8c1d 6874 7470 733a 2f2f 7079 7069  hP..https://pypi
-000017f0: 2e6f 7267 2f70 726f 6a65 6374 2f70 6970  .org/project/pip
-00001800: 2f94 7568 2b68 3368 1e4b 1a68 1d68 2c68  /.uh+h3h.K.h.h,h
-00001810: 1b6a 7201 0000 681c 6803 7562 6816 8c01  .jr...h.h.ubh...
-00001820: 3a94 8594 8194 7d94 2868 0568 0668 1b6a  :.....}.(h.h.h.j
-00001830: 7201 0000 681c 6803 681d 4e68 1e4e 7562  r...h.h.h.Nh.Nub
-00001840: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00001850: 5d94 6827 5d94 6829 5d94 7568 2b68 2d68  ].h'].h)].uh+h-h
-00001860: 1e4b 1a68 1d68 2c68 1b6a 6101 0000 681c  .K.h.h,h.ja...h.
-00001870: 6803 7562 6809 8c0d 6c69 7465 7261 6c5f  h.ubh...literal_
-00001880: 626c 6f63 6b94 9394 2981 947d 9428 6805  block...)..}.(h.
-00001890: 8c25 7069 7020 696e 7374 616c 6c20 766f  .%pip install vo
-000018a0: 6c6c 7365 672d 6e61 7061 7269 2d74 7261  llseg-napari-tra
-000018b0: 636b 6d61 7465 0a94 6807 5d94 6816 8c25  ckmate..h.].h..%
-000018c0: 7069 7020 696e 7374 616c 6c20 766f 6c6c  pip install voll
-000018d0: 7365 672d 6e61 7061 7269 2d74 7261 636b  seg-napari-track
-000018e0: 6d61 7465 0a94 8594 8194 7d94 2868 0568  mate......}.(h.h
-000018f0: 0668 1b6a a901 0000 7562 6168 1f7d 9428  .h.j....ubah.}.(
-00001900: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00001910: 6829 5d94 8c08 6c61 6e67 7561 6765 948c  h)]...language..
-00001920: 046e 6f6e 6594 6a5f 0100 006a 6001 0000  .none.j_...j`...
-00001930: 7568 2b6a a701 0000 681d 682c 681e 4b1c  uh+j....h.h,h.K.
-00001940: 681b 6a61 0100 0068 1c68 0375 6268 2e29  h.ja...h.h.ubh.)
-00001950: 8194 7d94 2868 058c 2754 6f20 696e 7374  ..}.(h..'To inst
-00001960: 616c 6c20 6c61 7465 7374 2064 6576 656c  all latest devel
-00001970: 6f70 6d65 6e74 2076 6572 7369 6f6e 203a  opment version :
-00001980: 9468 075d 9468 168c 2754 6f20 696e 7374  .h.].h..'To inst
-00001990: 616c 6c20 6c61 7465 7374 2064 6576 656c  all latest devel
-000019a0: 6f70 6d65 6e74 2076 6572 7369 6f6e 203a  opment version :
-000019b0: 9485 9481 947d 9428 6805 6806 681b 6ab9  .....}.(h.h.h.j.
-000019c0: 0100 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-000019d0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-000019e0: 9468 275d 9468 295d 9475 682b 682d 681e  .h'].h)].uh+h-h.
-000019f0: 4b20 681d 682c 681b 6a61 0100 0068 1c68  K h.h,h.ja...h.h
-00001a00: 0375 626a a801 0000 2981 947d 9428 6805  .ubj....)..}.(h.
-00001a10: 8c51 7069 7020 696e 7374 616c 6c20 6769  .Qpip install gi
-00001a20: 742b 6874 7470 733a 2f2f 6769 7468 7562  t+https://github
-00001a30: 2e63 6f6d 2f4b 6170 6f6f 726c 6162 732d  .com/Kapoorlabs-
-00001a40: 4341 5045 442f 766f 6c6c 7365 672d 6e61  CAPED/vollseg-na
-00001a50: 7061 7269 2d74 7261 636b 6d61 7465 2e67  pari-trackmate.g
-00001a60: 6974 0a94 6807 5d94 6816 8c51 7069 7020  it..h.].h..Qpip 
-00001a70: 696e 7374 616c 6c20 6769 742b 6874 7470  install git+http
-00001a80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4b  s://github.com/K
-00001a90: 6170 6f6f 726c 6162 732d 4341 5045 442f  apoorlabs-CAPED/
-00001aa0: 766f 6c6c 7365 672d 6e61 7061 7269 2d74  vollseg-napari-t
-00001ab0: 7261 636b 6d61 7465 2e67 6974 0a94 8594  rackmate.git....
-00001ac0: 8194 7d94 2868 0568 0668 1b6a c701 0000  ..}.(h.h.h.j....
-00001ad0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00001ae0: 6825 5d94 6827 5d94 6829 5d94 8c08 6c61  h%].h'].h)]...la
-00001af0: 6e67 7561 6765 946a b801 0000 6a5f 0100  nguage.j....j_..
-00001b00: 006a 6001 0000 7568 2b6a a701 0000 681d  .j`...uh+j....h.
-00001b10: 682c 681e 4b22 681b 6a61 0100 0068 1c68  h,h.K"h.ja...h.h
-00001b20: 0375 6265 681f 7d94 2868 215d 948c 0c69  .ubeh.}.(h!]...i
-00001b30: 6e73 7461 6c6c 6174 696f 6e94 6168 235d  nstallation.ah#]
-00001b40: 9468 255d 948c 0c69 6e73 7461 6c6c 6174  .h%]...installat
-00001b50: 696f 6e94 6168 275d 9468 295d 948c 0764  ion.ah'].h)]...d
-00001b60: 6f63 6e61 6d65 948c 0652 4541 444d 4594  ocname...README.
-00001b70: 8c0c 6865 6164 6572 5f6c 6576 656c 944b  ..header_level.K
-00001b80: 0275 682b 680a 681e 4b18 681d 682c 681b  .uh+h.h.K.h.h,h.
-00001b90: 680c 681c 6803 7562 680b 2981 947d 9428  h.h.h.ubh.)..}.(
-00001ba0: 6805 6806 6807 5d94 2868 1029 8194 7d94  h.h.h.].(h.)..}.
-00001bb0: 2868 058c 0c43 6f6e 7472 6962 7574 696e  (h...Contributin
-00001bc0: 6794 6807 5d94 6816 8c0c 436f 6e74 7269  g.h.].h...Contri
-00001bd0: 6275 7469 6e67 9485 9481 947d 9428 6805  buting.....}.(h.
-00001be0: 6806 681b 6ae4 0100 0068 1c68 0368 1d4e  h.h.j....h.h.h.N
-00001bf0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00001c00: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00001c10: 682b 680f 681e 4b25 681d 682c 681b 6ae1  h+h.h.K%h.h,h.j.
-00001c20: 0100 0068 1c68 0375 6268 2e29 8194 7d94  ...h.h.ubh.)..}.
-00001c30: 2868 058c 9143 6f6e 7472 6962 7574 696f  (h...Contributio
-00001c40: 6e73 2061 7265 2076 6572 7920 7765 6c63  ns are very welc
-00001c50: 6f6d 652e 2054 6573 7473 2063 616e 2062  ome. Tests can b
-00001c60: 6520 7275 6e20 7769 7468 205b 746f 785d  e run with [tox]
-00001c70: 2c20 706c 6561 7365 2065 6e73 7572 650a  , please ensure.
-00001c80: 7468 6520 636f 7665 7261 6765 2061 7420  the coverage at 
-00001c90: 6c65 6173 7420 7374 6179 7320 7468 6520  least stays the 
-00001ca0: 7361 6d65 2062 6566 6f72 6520 796f 7520  same before you 
-00001cb0: 7375 626d 6974 2061 2070 756c 6c20 7265  submit a pull re
-00001cc0: 7175 6573 742e 9468 075d 9428 6816 8c36  quest..h.].(h..6
-00001cd0: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
-00001ce0: 6520 7665 7279 2077 656c 636f 6d65 2e20  e very welcome. 
-00001cf0: 5465 7374 7320 6361 6e20 6265 2072 756e  Tests can be run
-00001d00: 2077 6974 6820 9485 9481 947d 9428 6805   with .....}.(h.
-00001d10: 6806 681b 6af2 0100 0068 1c68 0368 1d4e  h.h.j....h.h.h.N
-00001d20: 681e 4e75 6268 3429 8194 7d94 2868 058c  h.Nubh4)..}.(h..
-00001d30: 0374 6f78 9468 075d 9468 168c 0374 6f78  .tox.h.].h...tox
-00001d40: 9485 9481 947d 9428 6805 6806 681b 6afa  .....}.(h.h.h.j.
-00001d50: 0100 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00001d60: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00001d70: 9468 275d 9468 295d 9468 508c 2568 7474  .h'].h)].hP.%htt
-00001d80: 7073 3a2f 2f74 6f78 2e72 6561 6474 6865  ps://tox.readthe
-00001d90: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00001da0: 742f 9475 682b 6833 681e 4b27 681d 682c  t/.uh+h3h.K'h.h,
-00001db0: 681b 6af2 0100 0068 1c68 0375 6268 168c  h.j....h.h.ubh..
-00001dc0: 0f2c 2070 6c65 6173 6520 656e 7375 7265  ., please ensure
-00001dd0: 9485 9481 947d 9428 6805 6806 681b 6af2  .....}.(h.h.h.j.
-00001de0: 0100 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
-00001df0: 168c 010a 9485 9481 947d 9428 6805 6806  .........}.(h.h.
-00001e00: 681b 6af2 0100 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00001e10: 4e75 6268 168c 4674 6865 2063 6f76 6572  Nubh..Fthe cover
-00001e20: 6167 6520 6174 206c 6561 7374 2073 7461  age at least sta
-00001e30: 7973 2074 6865 2073 616d 6520 6265 666f  ys the same befo
-00001e40: 7265 2079 6f75 2073 7562 6d69 7420 6120  re you submit a 
-00001e50: 7075 6c6c 2072 6571 7565 7374 2e94 8594  pull request....
-00001e60: 8194 7d94 2868 0568 0668 1b6a f201 0000  ..}.(h.h.h.j....
-00001e70: 681c 6803 681d 4e68 1e4e 7562 6568 1f7d  h.h.h.Nh.Nubeh.}
-00001e80: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00001e90: 5d94 6829 5d94 7568 2b68 2d68 1e4b 2768  ].h)].uh+h-h.K'h
-00001ea0: 1d68 2c68 1b6a e101 0000 681c 6803 7562  .h,h.j....h.h.ub
-00001eb0: 6568 1f7d 9428 6821 5d94 8c0c 636f 6e74  eh.}.(h!]...cont
-00001ec0: 7269 6275 7469 6e67 9461 6823 5d94 6825  ributing.ah#].h%
-00001ed0: 5d94 8c0c 636f 6e74 7269 6275 7469 6e67  ]...contributing
-00001ee0: 9461 6827 5d94 6829 5d94 6ade 0100 006a  .ah'].h)].j....j
-00001ef0: df01 0000 6ae0 0100 004b 0375 682b 680a  ....j....K.uh+h.
-00001f00: 681e 4b25 681d 682c 681b 680c 681c 6803  h.K%h.h,h.h.h.h.
-00001f10: 7562 680b 2981 947d 9428 6805 6806 6807  ubh.)..}.(h.h.h.
-00001f20: 5d94 2868 1029 8194 7d94 2868 058c 074c  ].(h.)..}.(h...L
-00001f30: 6963 656e 7365 9468 075d 9468 168c 074c  icense.h.].h...L
-00001f40: 6963 656e 7365 9485 9481 947d 9428 6805  icense.....}.(h.
-00001f50: 6806 681b 6a26 0200 0068 1c68 0368 1d4e  h.h.j&...h.h.h.N
-00001f60: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00001f70: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00001f80: 682b 680f 681e 4b2a 681d 682c 681b 6a23  h+h.h.K*h.h,h.j#
-00001f90: 0200 0068 1c68 0375 6268 2e29 8194 7d94  ...h.h.ubh.)..}.
-00001fa0: 2868 058c 6f44 6973 7472 6962 7574 6564  (h..oDistributed
-00001fb0: 2075 6e64 6572 2074 6865 2074 6572 6d73   under the terms
-00001fc0: 206f 6620 7468 6520 5b42 5344 2d33 5d20   of the [BSD-3] 
-00001fd0: 6c69 6365 6e73 652c 0a22 766f 6c6c 7365  license,."vollse
-00001fe0: 672d 6e61 7061 7269 2d74 7261 636b 6d61  g-napari-trackma
-00001ff0: 7465 2220 6973 2066 7265 6520 616e 6420  te" is free and 
-00002000: 6f70 656e 2073 6f75 7263 6520 736f 6674  open source soft
-00002010: 7761 7265 9468 075d 9428 6816 8c23 4469  ware.h.].(h..#Di
-00002020: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
-00002030: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
-00002040: 2094 8594 8194 7d94 2868 0568 0668 1b6a   .....}.(h.h.h.j
-00002050: 3402 0000 681c 6803 681d 4e68 1e4e 7562  4...h.h.h.Nh.Nub
-00002060: 6834 2981 947d 9428 6805 8c05 4253 442d  h4)..}.(h...BSD-
-00002070: 3394 6807 5d94 6816 8c05 4253 442d 3394  3.h.].h...BSD-3.
-00002080: 8594 8194 7d94 2868 0568 0668 1b6a 3c02  ....}.(h.h.h.j<.
-00002090: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-000020a0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-000020b0: 6827 5d94 6829 5d94 6850 8c2b 6874 7470  h'].h)].hP.+http
-000020c0: 3a2f 2f6f 7065 6e73 6f75 7263 652e 6f72  ://opensource.or
-000020d0: 672f 6c69 6365 6e73 6573 2f42 5344 2d33  g/licenses/BSD-3
-000020e0: 2d43 6c61 7573 6594 7568 2b68 3368 1e4b  -Clause.uh+h3h.K
-000020f0: 2c68 1d68 2c68 1b6a 3402 0000 681c 6803  ,h.h,h.j4...h.h.
-00002100: 7562 6816 8c09 206c 6963 656e 7365 2c94  ubh... license,.
-00002110: 8594 8194 7d94 2868 0568 0668 1b6a 3402  ....}.(h.h.h.j4.
-00002120: 0000 681c 6803 681d 4e68 1e4e 7562 6816  ..h.h.h.Nh.Nubh.
-00002130: 8c01 0a94 8594 8194 7d94 2868 0568 0668  ........}.(h.h.h
-00002140: 1b6a 3402 0000 681c 6803 681d 4e68 1e4e  .j4...h.h.h.Nh.N
-00002150: 7562 6816 8c3f e280 9c76 6f6c 6c73 6567  ubh..?...vollseg
-00002160: 2d6e 6170 6172 692d 7472 6163 6b6d 6174  -napari-trackmat
-00002170: 65e2 809d 2069 7320 6672 6565 2061 6e64  e... is free and
-00002180: 206f 7065 6e20 736f 7572 6365 2073 6f66   open source sof
-00002190: 7477 6172 6594 8594 8194 7d94 2868 0568  tware.....}.(h.h
-000021a0: 0668 1b6a 3402 0000 681c 6803 681d 4e68  .h.j4...h.h.h.Nh
-000021b0: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
-000021c0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-000021d0: 2b68 2d68 1e4b 2c68 1d68 2c68 1b6a 2302  +h-h.K,h.h,h.j#.
-000021e0: 0000 681c 6803 7562 6568 1f7d 9428 6821  ..h.h.ubeh.}.(h!
-000021f0: 5d94 8c07 6c69 6365 6e73 6594 6168 235d  ]...license.ah#]
-00002200: 9468 255d 948c 076c 6963 656e 7365 9461  .h%]...license.a
-00002210: 6827 5d94 6829 5d94 6ade 0100 006a df01  h'].h)].j....j..
-00002220: 0000 6ae0 0100 004b 0475 682b 680a 681e  ..j....K.uh+h.h.
-00002230: 4b2a 681d 682c 681b 680c 681c 6803 7562  K*h.h,h.h.h.h.ub
-00002240: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
-00002250: 2868 1029 8194 7d94 2868 058c 0649 7373  (h.)..}.(h...Iss
-00002260: 7565 7394 6807 5d94 6816 8c06 4973 7375  ues.h.].h...Issu
-00002270: 6573 9485 9481 947d 9428 6805 6806 681b  es.....}.(h.h.h.
-00002280: 6a68 0200 0068 1c68 0368 1d4e 681e 4e75  jh...h.h.h.Nh.Nu
-00002290: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-000022a0: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
-000022b0: 681e 4b2f 681d 682c 681b 6a65 0200 0068  h.K/h.h,h.je...h
-000022c0: 1c68 0375 6268 2e29 8194 7d94 2868 058c  .h.ubh.)..}.(h..
-000022d0: 5849 6620 796f 7520 656e 636f 756e 7465  XIf you encounte
-000022e0: 7220 616e 7920 7072 6f62 6c65 6d73 2c20  r any problems, 
-000022f0: 706c 6561 7365 205b 6669 6c65 2061 6e20  please [file an 
-00002300: 6973 7375 655d 2061 6c6f 6e67 2077 6974  issue] along wit
-00002310: 6820 6120 6465 7461 696c 6564 2064 6573  h a detailed des
-00002320: 6372 6970 7469 6f6e 2e94 6807 5d94 2868  cription..h.].(h
-00002330: 168c 2649 6620 796f 7520 656e 636f 756e  ..&If you encoun
-00002340: 7465 7220 616e 7920 7072 6f62 6c65 6d73  ter any problems
-00002350: 2c20 706c 6561 7365 2094 8594 8194 7d94  , please .....}.
-00002360: 2868 0568 0668 1b6a 7602 0000 681c 6803  (h.h.h.jv...h.h.
-00002370: 681d 4e68 1e4e 7562 6834 2981 947d 9428  h.Nh.Nubh4)..}.(
-00002380: 6805 8c0d 6669 6c65 2061 6e20 6973 7375  h...file an issu
-00002390: 6594 6807 5d94 6816 8c0d 6669 6c65 2061  e.h.].h...file a
-000023a0: 6e20 6973 7375 6594 8594 8194 7d94 2868  n issue.....}.(h
-000023b0: 0568 0668 1b6a 7e02 0000 681c 6803 681d  .h.h.j~...h.h.h.
-000023c0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-000023d0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000023e0: 6850 8c43 6874 7470 733a 2f2f 6769 7468  hP.Chttps://gith
-000023f0: 7562 2e63 6f6d 2f4b 6170 6f6f 726c 6162  ub.com/Kapoorlab
-00002400: 732d 4341 5045 442f 766f 6c6c 7365 672d  s-CAPED/vollseg-
-00002410: 6e61 7061 7269 2d74 7261 636b 6d61 7465  napari-trackmate
-00002420: 2f69 7373 7565 7394 7568 2b68 3368 1e4b  /issues.uh+h3h.K
-00002430: 3168 1d68 2c68 1b6a 7602 0000 681c 6803  1h.h,h.jv...h.h.
-00002440: 7562 6816 8c23 2061 6c6f 6e67 2077 6974  ubh..# along wit
-00002450: 6820 6120 6465 7461 696c 6564 2064 6573  h a detailed des
-00002460: 6372 6970 7469 6f6e 2e94 8594 8194 7d94  cription......}.
-00002470: 2868 0568 0668 1b6a 7602 0000 681c 6803  (h.h.h.jv...h.h.
-00002480: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
-00002490: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-000024a0: 5d94 7568 2b68 2d68 1e4b 3168 1d68 2c68  ].uh+h-h.K1h.h,h
-000024b0: 1b6a 6502 0000 681c 6803 7562 6568 1f7d  .je...h.h.ubeh.}
-000024c0: 9428 6821 5d94 8c06 6973 7375 6573 9461  .(h!]...issues.a
-000024d0: 6823 5d94 6825 5d94 8c06 6973 7375 6573  h#].h%]...issues
-000024e0: 9461 6827 5d94 6829 5d94 6ade 0100 006a  .ah'].h)].j....j
-000024f0: df01 0000 6ae0 0100 004b 0575 682b 680a  ....j....K.uh+h.
-00002500: 681e 4b2f 681d 682c 681b 680c 681c 6803  h.K/h.h,h.h.h.h.
-00002510: 7562 6568 1f7d 9428 6821 5d94 8c18 766f  ubeh.}.(h!]...vo
-00002520: 6c6c 7365 672d 6e61 7061 7269 2d74 7261  llseg-napari-tra
-00002530: 636b 6d61 7465 9461 6823 5d94 288c 0e74  ckmate.ah#].(..t
-00002540: 6578 326a 6178 5f69 676e 6f72 6594 8c0e  ex2jax_ignore...
-00002550: 6d61 7468 6a61 785f 6967 6e6f 7265 9465  mathjax_ignore.e
-00002560: 6825 5d94 8c18 766f 6c6c 7365 672d 6e61  h%]...vollseg-na
-00002570: 7061 7269 2d74 7261 636b 6d61 7465 9461  pari-trackmate.a
-00002580: 6827 5d94 6829 5d94 6ade 0100 006a df01  h'].h)].j....j..
-00002590: 0000 6ae0 0100 004b 0175 682b 680a 681e  ..j....K.uh+h.h.
-000025a0: 4b01 681d 682c 681b 6803 681c 6803 7562  K.h.h,h.h.h.h.ub
-000025b0: 6809 8c08 636f 6d70 6f75 6e64 9493 9429  h...compound...)
-000025c0: 8194 7d94 2868 0568 0668 075d 9468 008c  ..}.(h.h.h.].h..
-000025d0: 0774 6f63 7472 6565 9493 9429 8194 7d94  .toctree...)..}.
-000025e0: 2868 0568 0668 075d 9468 1f7d 9428 6821  (h.h.h.].h.}.(h!
-000025f0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00002600: 5d94 681b 6adf 0100 008c 0765 6e74 7269  ].h.j......entri
-00002610: 6573 945d 944e 8c09 414c 474f 5249 5448  es.].N..ALGORITH
-00002620: 4d94 8694 618c 0c69 6e63 6c75 6465 6669  M...a..includefi
-00002630: 6c65 7394 5d94 6abb 0200 0061 8c08 6d61  les.].j....a..ma
-00002640: 7864 6570 7468 944a ffff ffff 8c07 6361  xdepth.J......ca
-00002650: 7074 696f 6e94 4e8c 0a72 6177 6361 7074  ption.N..rawcapt
-00002660: 696f 6e94 6806 8c04 676c 6f62 9489 8c06  ion.h...glob....
-00002670: 6869 6464 656e 9488 8c0d 696e 636c 7564  hidden....includ
-00002680: 6568 6964 6465 6e94 898c 086e 756d 6265  ehidden....numbe
-00002690: 7265 6494 4b00 8c0a 7469 746c 6573 6f6e  red.K...titleson
-000026a0: 6c79 9488 7568 2b6a ae02 0000 681d 682c  ly..uh+j....h.h,
-000026b0: 681e 4b01 681b 6aab 0200 0075 6261 681f  h.K.h.j....ubah.
-000026c0: 7d94 2868 215d 9468 235d 948c 0f74 6f63  }.(h!].h#]...toc
-000026d0: 7472 6565 2d77 7261 7070 6572 9461 6825  tree-wrapper.ah%
-000026e0: 5d94 6827 5d94 6829 5d94 6ade 0100 006a  ].h'].h)].j....j
-000026f0: df01 0000 6ac0 0200 004e 7568 2b6a a902  ....j....Nuh+j..
-00002700: 0000 7562 6568 1f7d 9428 6821 5d94 6823  ..ubeh.}.(h!].h#
-00002710: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
-00002720: 736f 7572 6365 9468 2c75 682b 6801 8c0e  source.h,uh+h...
-00002730: 6375 7272 656e 745f 736f 7572 6365 944e  current_source.N
-00002740: 8c0c 6375 7272 656e 745f 6c69 6e65 944e  ..current_line.N
-00002750: 8c08 7365 7474 696e 6773 948c 1164 6f63  ..settings...doc
-00002760: 7574 696c 732e 6672 6f6e 7465 6e64 948c  utils.frontend..
-00002770: 0656 616c 7565 7394 9394 2981 947d 9428  .Values...)..}.(
-00002780: 680f 4e8c 0967 656e 6572 6174 6f72 944e  h.N..generator.N
-00002790: 8c09 6461 7465 7374 616d 7094 4e8c 0b73  ..datestamp.N..s
-000027a0: 6f75 7263 655f 6c69 6e6b 944e 8c0a 736f  ource_link.N..so
-000027b0: 7572 6365 5f75 726c 944e 8c0d 746f 635f  urce_url.N..toc_
-000027c0: 6261 636b 6c69 6e6b 7394 8c05 656e 7472  backlinks...entr
-000027d0: 7994 8c12 666f 6f74 6e6f 7465 5f62 6163  y...footnote_bac
-000027e0: 6b6c 696e 6b73 944b 018c 0d73 6563 746e  klinks.K...sectn
-000027f0: 756d 5f78 666f 726d 944b 018c 0e73 7472  um_xform.K...str
-00002800: 6970 5f63 6f6d 6d65 6e74 7394 4e8c 1b73  ip_comments.N..s
-00002810: 7472 6970 5f65 6c65 6d65 6e74 735f 7769  trip_elements_wi
-00002820: 7468 5f63 6c61 7373 6573 944e 8c0d 7374  th_classes.N..st
-00002830: 7269 705f 636c 6173 7365 7394 4e8c 0c72  rip_classes.N..r
-00002840: 6570 6f72 745f 6c65 7665 6c94 4b02 8c0a  eport_level.K...
-00002850: 6861 6c74 5f6c 6576 656c 944b 058c 1165  halt_level.K...e
-00002860: 7869 745f 7374 6174 7573 5f6c 6576 656c  xit_status_level
-00002870: 944b 058c 0564 6562 7567 944e 8c0e 7761  .K...debug.N..wa
-00002880: 726e 696e 675f 7374 7265 616d 944e 8c09  rning_stream.N..
-00002890: 7472 6163 6562 6163 6b94 888c 0e69 6e70  traceback....inp
-000028a0: 7574 5f65 6e63 6f64 696e 6794 8c09 7574  ut_encoding...ut
-000028b0: 662d 382d 7369 6794 8c1c 696e 7075 745f  f-8-sig...input_
-000028c0: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
-000028d0: 616e 646c 6572 948c 0673 7472 6963 7494  andler...strict.
-000028e0: 8c0f 6f75 7470 7574 5f65 6e63 6f64 696e  ..output_encodin
-000028f0: 6794 8c05 7574 662d 3894 8c1d 6f75 7470  g...utf-8...outp
-00002900: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
-00002910: 725f 6861 6e64 6c65 7294 6af1 0200 008c  r_handler.j.....
-00002920: 0e65 7272 6f72 5f65 6e63 6f64 696e 6794  .error_encoding.
-00002930: 8c05 7574 662d 3894 8c1c 6572 726f 725f  ..utf-8...error_
-00002940: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
-00002950: 616e 646c 6572 948c 1062 6163 6b73 6c61  andler...backsla
-00002960: 7368 7265 706c 6163 6594 8c0d 6c61 6e67  shreplace...lang
-00002970: 7561 6765 5f63 6f64 6594 8c02 656e 948c  uage_code...en..
-00002980: 1372 6563 6f72 645f 6465 7065 6e64 656e  .record_dependen
-00002990: 6369 6573 944e 8c06 636f 6e66 6967 944e  cies.N..config.N
-000029a0: 8c09 6964 5f70 7265 6669 7894 6806 8c0e  ..id_prefix.h...
-000029b0: 6175 746f 5f69 645f 7072 6566 6978 948c  auto_id_prefix..
-000029c0: 0269 6494 8c0d 6475 6d70 5f73 6574 7469  .id...dump_setti
-000029d0: 6e67 7394 4e8c 0e64 756d 705f 696e 7465  ngs.N..dump_inte
-000029e0: 726e 616c 7394 4e8c 0f64 756d 705f 7472  rnals.N..dump_tr
-000029f0: 616e 7366 6f72 6d73 944e 8c0f 6475 6d70  ansforms.N..dump
-00002a00: 5f70 7365 7564 6f5f 786d 6c94 4e8c 1065  _pseudo_xml.N..e
-00002a10: 7870 6f73 655f 696e 7465 726e 616c 7394  xpose_internals.
-00002a20: 4e8c 0e73 7472 6963 745f 7669 7369 746f  N..strict_visito
-00002a30: 7294 4e8c 0f5f 6469 7361 626c 655f 636f  r.N.._disable_co
-00002a40: 6e66 6967 944e 8c07 5f73 6f75 7263 6594  nfig.N.._source.
-00002a50: 682c 8c0c 5f64 6573 7469 6e61 7469 6f6e  h,.._destination
-00002a60: 944e 8c0d 5f63 6f6e 6669 675f 6669 6c65  .N.._config_file
-00002a70: 7394 5d94 8c16 6669 6c65 5f69 6e73 6572  s.]...file_inser
-00002a80: 7469 6f6e 5f65 6e61 626c 6564 9488 8c0b  tion_enabled....
-00002a90: 7261 775f 656e 6162 6c65 6494 4b01 8c11  raw_enabled.K...
-00002aa0: 6c69 6e65 5f6c 656e 6774 685f 6c69 6d69  line_length_limi
-00002ab0: 7494 4d10 278c 0e70 6570 5f72 6566 6572  t.M.'..pep_refer
-00002ac0: 656e 6365 7394 4e8c 0c70 6570 5f62 6173  ences.N..pep_bas
-00002ad0: 655f 7572 6c94 8c18 6874 7470 733a 2f2f  e_url...https://
-00002ae0: 7065 7073 2e70 7974 686f 6e2e 6f72 672f  peps.python.org/
-00002af0: 948c 1570 6570 5f66 696c 655f 7572 6c5f  ...pep_file_url_
-00002b00: 7465 6d70 6c61 7465 948c 0870 6570 2d25  template...pep-%
-00002b10: 3034 6494 8c0e 7266 635f 7265 6665 7265  04d...rfc_refere
-00002b20: 6e63 6573 944e 8c0c 7266 635f 6261 7365  nces.N..rfc_base
-00002b30: 5f75 726c 948c 2668 7474 7073 3a2f 2f64  _url..&https://d
-00002b40: 6174 6174 7261 636b 6572 2e69 6574 662e  atatracker.ietf.
-00002b50: 6f72 672f 646f 632f 6874 6d6c 2f94 8c09  org/doc/html/...
-00002b60: 7461 625f 7769 6474 6894 4b08 8c1d 7472  tab_width.K...tr
-00002b70: 696d 5f66 6f6f 746e 6f74 655f 7265 6665  im_footnote_refe
-00002b80: 7265 6e63 655f 7370 6163 6594 898c 1073  rence_space....s
-00002b90: 796e 7461 785f 6869 6768 6c69 6768 7494  yntax_highlight.
-00002ba0: 8c04 6c6f 6e67 948c 0c73 6d61 7274 5f71  ..long...smart_q
-00002bb0: 756f 7465 7394 888c 1373 6d61 7274 7175  uotes....smartqu
-00002bc0: 6f74 6573 5f6c 6f63 616c 6573 945d 948c  otes_locales.]..
-00002bd0: 1d63 6861 7261 6374 6572 5f6c 6576 656c  .character_level
-00002be0: 5f69 6e6c 696e 655f 6d61 726b 7570 9489  _inline_markup..
-00002bf0: 8c0e 646f 6374 6974 6c65 5f78 666f 726d  ..doctitle_xform
-00002c00: 9489 8c0d 646f 6369 6e66 6f5f 7866 6f72  ....docinfo_xfor
-00002c10: 6d94 4b01 8c12 7365 6374 7375 6274 6974  m.K...sectsubtit
-00002c20: 6c65 5f78 666f 726d 9489 8c0c 656d 6265  le_xform....embe
-00002c30: 645f 696d 6167 6573 9489 8c10 656d 6265  d_images....embe
-00002c40: 645f 7374 796c 6573 6865 6574 9489 8c15  d_stylesheet....
-00002c50: 636c 6f61 6b5f 656d 6169 6c5f 6164 6472  cloak_email_addr
-00002c60: 6573 7365 7394 888c 1173 6563 7469 6f6e  esses....section
-00002c70: 5f73 656c 665f 6c69 6e6b 9489 8c03 656e  _self_link....en
-00002c80: 7694 4e75 628c 0872 6570 6f72 7465 7294  v.Nub..reporter.
-00002c90: 4e8c 1069 6e64 6972 6563 745f 7461 7267  N..indirect_targ
-00002ca0: 6574 7394 5d94 8c11 7375 6273 7469 7475  ets.]...substitu
-00002cb0: 7469 6f6e 5f64 6566 7394 7d94 288c 0f77  tion_defs.}.(..w
-00002cc0: 6f72 6463 6f75 6e74 2d77 6f72 6473 9468  ordcount-words.h
-00002cd0: 098c 1773 7562 7374 6974 7574 696f 6e5f  ...substitution_
-00002ce0: 6465 6669 6e69 7469 6f6e 9493 9429 8194  definition...)..
-00002cf0: 7d94 2868 058c 0239 3294 6807 5d94 6816  }.(h...92.h.].h.
-00002d00: 8c02 3932 9485 9481 947d 9428 6805 6806  ..92.....}.(h.h.
-00002d10: 681b 6a2e 0300 0075 6261 681f 7d94 2868  h.j....ubah.}.(h
-00002d20: 215d 9468 235d 9468 255d 948c 0f77 6f72  !].h#].h%]...wor
-00002d30: 6463 6f75 6e74 2d77 6f72 6473 9461 6827  dcount-words.ah'
-00002d40: 5d94 6829 5d94 7568 2b6a 2c03 0000 681d  ].h)].uh+j,...h.
-00002d50: 682c 7562 8c11 776f 7264 636f 756e 742d  h,ub..wordcount-
-00002d60: 6d69 6e75 7465 7394 6a2d 0300 0029 8194  minutes.j-...)..
-00002d70: 7d94 2868 058c 0130 9468 075d 9468 168c  }.(h...0.h.].h..
-00002d80: 0130 9485 9481 947d 9428 6805 6806 681b  .0.....}.(h.h.h.
-00002d90: 6a3e 0300 0075 6261 681f 7d94 2868 215d  j>...ubah.}.(h!]
-00002da0: 9468 235d 9468 255d 948c 1177 6f72 6463  .h#].h%]...wordc
-00002db0: 6f75 6e74 2d6d 696e 7574 6573 9461 6827  ount-minutes.ah'
-00002dc0: 5d94 6829 5d94 7568 2b6a 2c03 0000 681d  ].h)].uh+j,...h.
-00002dd0: 682c 7562 758c 1273 7562 7374 6974 7574  h,ubu..substitut
-00002de0: 696f 6e5f 6e61 6d65 7394 7d94 288c 0f77  ion_names.}.(..w
-00002df0: 6f72 6463 6f75 6e74 2d77 6f72 6473 946a  ordcount-words.j
-00002e00: 2b03 0000 8c11 776f 7264 636f 756e 742d  +.....wordcount-
-00002e10: 6d69 6e75 7465 7394 6a3d 0300 0075 8c08  minutes.j=...u..
-00002e20: 7265 666e 616d 6573 947d 948c 0672 6566  refnames.}...ref
-00002e30: 6964 7394 7d94 8c07 6e61 6d65 6964 7394  ids.}...nameids.
-00002e40: 7d94 286a a602 0000 6aa1 0200 006a db01  }.(j....j....j..
-00002e50: 0000 6ad8 0100 006a 2002 0000 6a1d 0200  ..j....j ...j...
-00002e60: 006a 6202 0000 6a5f 0200 006a 9c02 0000  .jb...j_...j....
-00002e70: 6a99 0200 0075 8c09 6e61 6d65 7479 7065  j....u..nametype
-00002e80: 7394 7d94 286a a602 0000 4e6a db01 0000  s.}.(j....Nj....
-00002e90: 4e6a 2002 0000 4e6a 6202 0000 4e6a 9c02  Nj ...Njb...Nj..
-00002ea0: 0000 4e75 6821 7d94 286a a102 0000 680c  ..Nuh!}.(j....h.
-00002eb0: 6ad8 0100 006a 6101 0000 6a1d 0200 006a  j....ja...j....j
-00002ec0: e101 0000 6a5f 0200 006a 2302 0000 6a99  ....j_...j#...j.
-00002ed0: 0200 006a 6502 0000 758c 0d66 6f6f 746e  ...je...u..footn
-00002ee0: 6f74 655f 7265 6673 947d 948c 0d63 6974  ote_refs.}...cit
-00002ef0: 6174 696f 6e5f 7265 6673 947d 948c 0d61  ation_refs.}...a
-00002f00: 7574 6f66 6f6f 746e 6f74 6573 945d 948c  utofootnotes.]..
-00002f10: 1161 7574 6f66 6f6f 746e 6f74 655f 7265  .autofootnote_re
-00002f20: 6673 945d 948c 1073 796d 626f 6c5f 666f  fs.]...symbol_fo
-00002f30: 6f74 6e6f 7465 7394 5d94 8c14 7379 6d62  otnotes.]...symb
-00002f40: 6f6c 5f66 6f6f 746e 6f74 655f 7265 6673  ol_footnote_refs
-00002f50: 945d 948c 0966 6f6f 746e 6f74 6573 945d  .]...footnotes.]
-00002f60: 948c 0963 6974 6174 696f 6e73 945d 948c  ...citations.]..
-00002f70: 1261 7574 6f66 6f6f 746e 6f74 655f 7374  .autofootnote_st
-00002f80: 6172 7494 4b01 8c15 7379 6d62 6f6c 5f66  art.K...symbol_f
-00002f90: 6f6f 746e 6f74 655f 7374 6172 7494 4b00  ootnote_start.K.
-00002fa0: 8c0a 6964 5f63 6f75 6e74 6572 948c 0b63  ..id_counter...c
-00002fb0: 6f6c 6c65 6374 696f 6e73 948c 0743 6f75  ollections...Cou
-00002fc0: 6e74 6572 9493 947d 9485 9452 948c 0e70  nter...}...R...p
-00002fd0: 6172 7365 5f6d 6573 7361 6765 7394 5d94  arse_messages.].
-00002fe0: 8c12 7472 616e 7366 6f72 6d5f 6d65 7373  ..transform_mess
-00002ff0: 6167 6573 945d 948c 0b74 7261 6e73 666f  ages.]...transfo
-00003000: 726d 6572 944e 8c0b 696e 636c 7564 655f  rmer.N..include_
-00003010: 6c6f 6794 5d94 8c0a 6465 636f 7261 7469  log.]...decorati
-00003020: 6f6e 944e 681c 6803 7562 2e0a            on.Nh.h.ub..
+00000f20: 8c4c 456c 6162 6f72 6174 6520 646f 6375  .LElaborate docu
+00000f30: 6d65 6e74 6174 696f 6e20 666f 7220 7573  mentation for us
+00000f40: 6572 7320 6f66 2074 6869 7320 7265 706f  ers of this repo
+00000f50: 7369 746f 7279 2061 7420 7468 6973 205b  sitory at this [
+00000f60: 646f 6375 6d65 6e74 6174 696f 6e5d 9468  documentation].h
+00000f70: 075d 9428 6816 8c3d 456c 6162 6f72 6174  .].(h..=Elaborat
+00000f80: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
+00000f90: 666f 7220 7573 6572 7320 6f66 2074 6869  for users of thi
+00000fa0: 7320 7265 706f 7369 746f 7279 2061 7420  s repository at 
+00000fb0: 7468 6973 2094 8594 8194 7d94 2868 0568  this .....}.(h.h
+00000fc0: 0668 1b68 f368 1c68 0368 1d4e 681e 4e75  .h.h.h.h.h.Nh.Nu
+00000fd0: 6268 3429 8194 7d94 2868 058c 0d64 6f63  bh4)..}.(h...doc
+00000fe0: 756d 656e 7461 7469 6f6e 9468 075d 9468  umentation.h.].h
+00000ff0: 168c 0d64 6f63 756d 656e 7461 7469 6f6e  ...documentation
+00001000: 9485 9481 947d 9428 6805 6806 681b 68fb  .....}.(h.h.h.h.
+00001010: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00001020: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00001030: 5d94 6829 5d94 6850 8c3b 6874 7470 733a  ].h)].hP.;https:
+00001040: 2f2f 6b61 706f 6f72 6c61 6273 2d63 6170  //kapoorlabs-cap
+00001050: 6564 2e67 6974 6875 622e 696f 2f76 6f6c  ed.github.io/vol
+00001060: 6c73 6567 2d6e 6170 6172 692d 7472 6163  lseg-napari-trac
+00001070: 6b6d 6174 6594 7568 2b68 3368 1e4b 0e68  kmate.uh+h3h.K.h
+00001080: 1d68 2c68 1b68 f368 1c68 0375 6265 681f  .h,h.h.h.h.ubeh.
+00001090: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+000010a0: 275d 9468 295d 9475 682b 682d 681e 4b0e  '].h)].uh+h-h.K.
+000010b0: 681d 682c 681b 680c 681c 6803 7562 682e  h.h,h.h.h.h.ubh.
+000010c0: 2981 947d 9428 6805 8c6e 5468 6973 205b  )..}.(h..nThis [
+000010d0: 6e61 7061 7269 5d20 706c 7567 696e 2077  napari] plugin w
+000010e0: 6173 2067 656e 6572 6174 6564 2077 6974  as generated wit
+000010f0: 6820 5b43 6f6f 6b69 6563 7574 7465 725d  h [Cookiecutter]
+00001100: 2075 7369 6e67 205b 4063 6170 6564 5d27   using [@caped]'
+00001110: 7320 5b63 6f6f 6b69 6563 7574 7465 722d  s [cookiecutter-
+00001120: 6e61 7061 7269 2d70 6c75 6769 6e5d 2074  napari-plugin] t
+00001130: 656d 706c 6174 652e 9468 075d 9428 6816  emplate..h.].(h.
+00001140: 8c05 5468 6973 2094 8594 8194 7d94 2868  ..This .....}.(h
+00001150: 0568 0668 1b6a 1001 0000 681c 6803 681d  .h.h.j....h.h.h.
+00001160: 4e68 1e4e 7562 6834 2981 947d 9428 6805  Nh.Nubh4)..}.(h.
+00001170: 8c06 6e61 7061 7269 9468 075d 9468 168c  ..napari.h.].h..
+00001180: 066e 6170 6172 6994 8594 8194 7d94 2868  .napari.....}.(h
+00001190: 0568 0668 1b6a 1801 0000 681c 6803 681d  .h.h.j....h.h.h.
+000011a0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+000011b0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000011c0: 6850 8c20 6874 7470 733a 2f2f 6769 7468  hP. https://gith
+000011d0: 7562 2e63 6f6d 2f6e 6170 6172 692f 6e61  ub.com/napari/na
+000011e0: 7061 7269 9475 682b 6833 681e 4b10 681d  pari.uh+h3h.K.h.
+000011f0: 682c 681b 6a10 0100 0068 1c68 0375 6268  h,h.j....h.h.ubh
+00001200: 168c 1b20 706c 7567 696e 2077 6173 2067  ... plugin was g
+00001210: 656e 6572 6174 6564 2077 6974 6820 9485  enerated with ..
+00001220: 9481 947d 9428 6805 6806 681b 6a10 0100  ...}.(h.h.h.j...
+00001230: 0068 1c68 0368 1d4e 681e 4e75 6268 3429  .h.h.h.Nh.Nubh4)
+00001240: 8194 7d94 2868 058c 0c43 6f6f 6b69 6563  ..}.(h...Cookiec
+00001250: 7574 7465 7294 6807 5d94 6816 8c0c 436f  utter.h.].h...Co
+00001260: 6f6b 6965 6375 7474 6572 9485 9481 947d  okiecutter.....}
+00001270: 9428 6805 6806 681b 6a2b 0100 0068 1c68  .(h.h.h.j+...h.h
+00001280: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00001290: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000012a0: 295d 9468 508c 2768 7474 7073 3a2f 2f67  )].hP.'https://g
+000012b0: 6974 6875 622e 636f 6d2f 6175 6472 6579  ithub.com/audrey
+000012c0: 722f 636f 6f6b 6965 6375 7474 6572 9475  r/cookiecutter.u
+000012d0: 682b 6833 681e 4b10 681d 682c 681b 6a10  h+h3h.K.h.h,h.j.
+000012e0: 0100 0068 1c68 0375 6268 168c 0720 7573  ...h.h.ubh... us
+000012f0: 696e 6720 9485 9481 947d 9428 6805 6806  ing .....}.(h.h.
+00001300: 681b 6a10 0100 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00001310: 4e75 6268 3429 8194 7d94 2868 058c 0640  Nubh4)..}.(h...@
+00001320: 6361 7065 6494 6807 5d94 6816 8c06 4063  caped.h.].h...@c
+00001330: 6170 6564 9485 9481 947d 9428 6805 6806  aped.....}.(h.h.
+00001340: 681b 6a3e 0100 0068 1c68 0368 1d4e 681e  h.j>...h.h.h.Nh.
+00001350: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00001360: 9468 255d 9468 275d 9468 295d 9468 508c  .h%].h'].h)].hP.
+00001370: 2468 7474 7073 3a2f 2f67 6974 6875 622e  $https://github.
+00001380: 636f 6d2f 4b61 706f 6f72 6c61 6273 2d43  com/Kapoorlabs-C
+00001390: 4150 4544 2f94 7568 2b68 3368 1e4b 1068  APED/.uh+h3h.K.h
+000013a0: 1d68 2c68 1b6a 1001 0000 681c 6803 7562  .h,h.j....h.h.ub
+000013b0: 6816 8c05 e280 9973 2094 8594 8194 7d94  h......s .....}.
+000013c0: 2868 0568 0668 1b6a 1001 0000 681c 6803  (h.h.h.j....h.h.
+000013d0: 681d 4e68 1e4e 7562 6834 2981 947d 9428  h.Nh.Nubh4)..}.(
+000013e0: 6805 8c1a 636f 6f6b 6965 6375 7474 6572  h...cookiecutter
+000013f0: 2d6e 6170 6172 692d 706c 7567 696e 9468  -napari-plugin.h
+00001400: 075d 9468 168c 1a63 6f6f 6b69 6563 7574  .].h...cookiecut
+00001410: 7465 722d 6e61 7061 7269 2d70 6c75 6769  ter-napari-plugi
+00001420: 6e94 8594 8194 7d94 2868 0568 0668 1b6a  n.....}.(h.h.h.j
+00001430: 5101 0000 681c 6803 681d 4e68 1e4e 7562  Q...h.h.h.Nh.Nub
+00001440: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00001450: 5d94 6827 5d94 6829 5d94 6850 8c49 6874  ].h'].h)].hP.Iht
+00001460: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001470: 2f4b 6170 6f6f 726c 6162 732d 4341 5045  /Kapoorlabs-CAPE
+00001480: 442f 636f 6f6b 6965 6375 7474 6572 2d6b  D/cookiecutter-k
+00001490: 6170 6f6f 726c 6162 732d 6e61 7061 7269  apoorlabs-napari
+000014a0: 2d70 6c75 6769 6e94 7568 2b68 3368 1e4b  -plugin.uh+h3h.K
+000014b0: 1068 1d68 2c68 1b6a 1001 0000 681c 6803  .h.h,h.j....h.h.
+000014c0: 7562 6816 8c0a 2074 656d 706c 6174 652e  ubh... template.
+000014d0: 9485 9481 947d 9428 6805 6806 681b 6a10  .....}.(h.h.h.j.
+000014e0: 0100 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
+000014f0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00001500: 9468 275d 9468 295d 9475 682b 682d 681e  .h'].h)].uh+h-h.
+00001510: 4b10 681d 682c 681b 680c 681c 6803 7562  K.h.h,h.h.h.h.ub
+00001520: 6809 8c03 7261 7794 9394 2981 947d 9428  h...raw...)..}.(
+00001530: 6805 8cf4 3c21 2d2d 0a44 6f6e 2774 206d  h...<!--.Don't m
+00001540: 6973 7320 7468 6520 6675 6c6c 2067 6574  iss the full get
+00001550: 7469 6e67 2073 7461 7274 6564 2067 7569  ting started gui
+00001560: 6465 2074 6f20 7365 7420 7570 2079 6f75  de to set up you
+00001570: 7220 6e65 7720 7061 636b 6167 653a 0a68  r new package:.h
+00001580: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001590: 6d2f 6e61 7061 7269 2f63 6f6f 6b69 6563  m/napari/cookiec
+000015a0: 7574 7465 722d 6e61 7061 7269 2d70 6c75  utter-napari-plu
+000015b0: 6769 6e23 6765 7474 696e 672d 7374 6172  gin#getting-star
+000015c0: 7465 640a 0a61 6e64 2072 6576 6965 7720  ted..and review 
+000015d0: 7468 6520 6e61 7061 7269 2064 6f63 7320  the napari docs 
+000015e0: 666f 7220 706c 7567 696e 2064 6576 656c  for plugin devel
+000015f0: 6f70 6572 733a 0a68 7474 7073 3a2f 2f6e  opers:.https://n
+00001600: 6170 6172 692e 6f72 672f 7374 6162 6c65  apari.org/stable
+00001610: 2f70 6c75 6769 6e73 2f69 6e64 6578 2e68  /plugins/index.h
+00001620: 746d 6c0a 2d2d 3e0a 9468 075d 9468 168c  tml.-->..h.].h..
+00001630: f43c 212d 2d0a 446f 6e27 7420 6d69 7373  .<!--.Don't miss
+00001640: 2074 6865 2066 756c 6c20 6765 7474 696e   the full gettin
+00001650: 6720 7374 6172 7465 6420 6775 6964 6520  g started guide 
+00001660: 746f 2073 6574 2075 7020 796f 7572 206e  to set up your n
+00001670: 6577 2070 6163 6b61 6765 3a0a 6874 7470  ew package:.http
+00001680: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
+00001690: 6170 6172 692f 636f 6f6b 6965 6375 7474  apari/cookiecutt
+000016a0: 6572 2d6e 6170 6172 692d 706c 7567 696e  er-napari-plugin
+000016b0: 2367 6574 7469 6e67 2d73 7461 7274 6564  #getting-started
+000016c0: 0a0a 616e 6420 7265 7669 6577 2074 6865  ..and review the
+000016d0: 206e 6170 6172 6920 646f 6373 2066 6f72   napari docs for
+000016e0: 2070 6c75 6769 6e20 6465 7665 6c6f 7065   plugin develope
+000016f0: 7273 3a0a 6874 7470 733a 2f2f 6e61 7061  rs:.https://napa
+00001700: 7269 2e6f 7267 2f73 7461 626c 652f 706c  ri.org/stable/pl
+00001710: 7567 696e 732f 696e 6465 782e 6874 6d6c  ugins/index.html
+00001720: 0a2d 2d3e 0a94 8594 8194 7d94 2868 0568  .-->......}.(h.h
+00001730: 0668 1b6a 6c01 0000 7562 6168 1f7d 9428  .h.jl...ubah.}.(
+00001740: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00001750: 6829 5d94 8c06 666f 726d 6174 948c 0468  h)]...format...h
+00001760: 746d 6c94 8c09 786d 6c3a 7370 6163 6594  tml...xml:space.
+00001770: 8c08 7072 6573 6572 7665 9475 682b 6a6a  ..preserve.uh+jj
+00001780: 0100 0068 1d68 2c68 1e4b 1268 1b68 0c68  ...h.h,h.K.h.h.h
+00001790: 1c68 0375 6268 0b29 8194 7d94 2868 0568  .h.ubh.)..}.(h.h
+000017a0: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
+000017b0: 8c0c 496e 7374 616c 6c61 7469 6f6e 9468  ..Installation.h
+000017c0: 075d 9468 168c 0c49 6e73 7461 6c6c 6174  .].h...Installat
+000017d0: 696f 6e94 8594 8194 7d94 2868 0568 0668  ion.....}.(h.h.h
+000017e0: 1b6a 8101 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+000017f0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001800: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00001810: 0f68 1e4b 1a68 1d68 2c68 1b6a 7e01 0000  .h.K.h.h,h.j~...
+00001820: 681c 6803 7562 682e 2981 947d 9428 6805  h.h.ubh.)..}.(h.
+00001830: 8c35 596f 7520 6361 6e20 696e 7374 616c  .5You can instal
+00001840: 6c20 6076 6f6c 6c73 6567 2d6e 6170 6172  l `vollseg-napar
+00001850: 692d 7472 6163 6b6d 6174 6560 2076 6961  i-trackmate` via
+00001860: 205b 7069 705d 3a94 6807 5d94 2868 168c   [pip]:.h.].(h..
+00001870: 1059 6f75 2063 616e 2069 6e73 7461 6c6c  .You can install
+00001880: 2094 8594 8194 7d94 2868 0568 0668 1b6a   .....}.(h.h.h.j
+00001890: 8f01 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+000018a0: 6809 8c07 6c69 7465 7261 6c94 9394 2981  h...literal...).
+000018b0: 947d 9428 6805 8c18 766f 6c6c 7365 672d  .}.(h...vollseg-
+000018c0: 6e61 7061 7269 2d74 7261 636b 6d61 7465  napari-trackmate
+000018d0: 9468 075d 9468 168c 1876 6f6c 6c73 6567  .h.].h...vollseg
+000018e0: 2d6e 6170 6172 692d 7472 6163 6b6d 6174  -napari-trackmat
+000018f0: 6594 8594 8194 7d94 2868 0568 0668 1b6a  e.....}.(h.h.h.j
+00001900: 9901 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00001910: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00001920: 5d94 6827 5d94 6829 5d94 7568 2b6a 9701  ].h'].h)].uh+j..
+00001930: 0000 681e 4b1c 681d 682c 681b 6a8f 0100  ..h.K.h.h,h.j...
+00001940: 0068 1c68 0375 6268 168c 0520 7669 6120  .h.h.ubh... via 
+00001950: 9485 9481 947d 9428 6805 6806 681b 6a8f  .....}.(h.h.h.j.
+00001960: 0100 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
+00001970: 3429 8194 7d94 2868 058c 0370 6970 9468  4)..}.(h...pip.h
+00001980: 075d 9468 168c 0370 6970 9485 9481 947d  .].h...pip.....}
+00001990: 9428 6805 6806 681b 6aab 0100 0068 1c68  .(h.h.h.j....h.h
+000019a0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+000019b0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000019c0: 295d 9468 508c 1d68 7474 7073 3a2f 2f70  )].hP..https://p
+000019d0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000019e0: 7069 702f 9475 682b 6833 681e 4b1c 681d  pip/.uh+h3h.K.h.
+000019f0: 682c 681b 6a8f 0100 0068 1c68 0375 6268  h,h.j....h.h.ubh
+00001a00: 168c 013a 9485 9481 947d 9428 6805 6806  ...:.....}.(h.h.
+00001a10: 681b 6a8f 0100 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00001a20: 4e75 6265 681f 7d94 2868 215d 9468 235d  Nubeh.}.(h!].h#]
+00001a30: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00001a40: 682d 681e 4b1c 681d 682c 681b 6a7e 0100  h-h.K.h.h,h.j~..
+00001a50: 0068 1c68 0375 6268 098c 0d6c 6974 6572  .h.h.ubh...liter
+00001a60: 616c 5f62 6c6f 636b 9493 9429 8194 7d94  al_block...)..}.
+00001a70: 2868 058c 2570 6970 2069 6e73 7461 6c6c  (h..%pip install
+00001a80: 2076 6f6c 6c73 6567 2d6e 6170 6172 692d   vollseg-napari-
+00001a90: 7472 6163 6b6d 6174 650a 9468 075d 9468  trackmate..h.].h
+00001aa0: 168c 2570 6970 2069 6e73 7461 6c6c 2076  ..%pip install v
+00001ab0: 6f6c 6c73 6567 2d6e 6170 6172 692d 7472  ollseg-napari-tr
+00001ac0: 6163 6b6d 6174 650a 9485 9481 947d 9428  ackmate......}.(
+00001ad0: 6805 6806 681b 6ac6 0100 0075 6261 681f  h.h.h.j....ubah.
+00001ae0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00001af0: 275d 9468 295d 948c 086c 616e 6775 6167  '].h)]...languag
+00001b00: 6594 8c04 6e6f 6e65 946a 7c01 0000 6a7d  e...none.j|...j}
+00001b10: 0100 0075 682b 6ac4 0100 0068 1d68 2c68  ...uh+j....h.h,h
+00001b20: 1e4b 1e68 1b6a 7e01 0000 681c 6803 7562  .K.h.j~...h.h.ub
+00001b30: 682e 2981 947d 9428 6805 8c27 546f 2069  h.)..}.(h..'To i
+00001b40: 6e73 7461 6c6c 206c 6174 6573 7420 6465  nstall latest de
+00001b50: 7665 6c6f 706d 656e 7420 7665 7273 696f  velopment versio
+00001b60: 6e20 3a94 6807 5d94 6816 8c27 546f 2069  n :.h.].h..'To i
+00001b70: 6e73 7461 6c6c 206c 6174 6573 7420 6465  nstall latest de
+00001b80: 7665 6c6f 706d 656e 7420 7665 7273 696f  velopment versio
+00001b90: 6e20 3a94 8594 8194 7d94 2868 0568 0668  n :.....}.(h.h.h
+00001ba0: 1b6a d601 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00001bb0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001bc0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00001bd0: 2d68 1e4b 2268 1d68 2c68 1b6a 7e01 0000  -h.K"h.h,h.j~...
+00001be0: 681c 6803 7562 6ac5 0100 0029 8194 7d94  h.h.ubj....)..}.
+00001bf0: 2868 058c 5170 6970 2069 6e73 7461 6c6c  (h..Qpip install
+00001c00: 2067 6974 2b68 7474 7073 3a2f 2f67 6974   git+https://git
+00001c10: 6875 622e 636f 6d2f 4b61 706f 6f72 6c61  hub.com/Kapoorla
+00001c20: 6273 2d43 4150 4544 2f76 6f6c 6c73 6567  bs-CAPED/vollseg
+00001c30: 2d6e 6170 6172 692d 7472 6163 6b6d 6174  -napari-trackmat
+00001c40: 652e 6769 740a 9468 075d 9468 168c 5170  e.git..h.].h..Qp
+00001c50: 6970 2069 6e73 7461 6c6c 2067 6974 2b68  ip install git+h
+00001c60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001c70: 6d2f 4b61 706f 6f72 6c61 6273 2d43 4150  m/Kapoorlabs-CAP
+00001c80: 4544 2f76 6f6c 6c73 6567 2d6e 6170 6172  ED/vollseg-napar
+00001c90: 692d 7472 6163 6b6d 6174 652e 6769 740a  i-trackmate.git.
+00001ca0: 9485 9481 947d 9428 6805 6806 681b 6ae4  .....}.(h.h.h.j.
+00001cb0: 0100 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
+00001cc0: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00001cd0: 086c 616e 6775 6167 6594 6ad5 0100 006a  .language.j....j
+00001ce0: 7c01 0000 6a7d 0100 0075 682b 6ac4 0100  |...j}...uh+j...
+00001cf0: 0068 1d68 2c68 1e4b 2468 1b6a 7e01 0000  .h.h,h.K$h.j~...
+00001d00: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
+00001d10: 8c0c 696e 7374 616c 6c61 7469 6f6e 9461  ..installation.a
+00001d20: 6823 5d94 6825 5d94 8c0c 696e 7374 616c  h#].h%]...instal
+00001d30: 6c61 7469 6f6e 9461 6827 5d94 6829 5d94  lation.ah'].h)].
+00001d40: 8c07 646f 636e 616d 6594 8c06 5245 4144  ..docname...READ
+00001d50: 4d45 948c 0c68 6561 6465 725f 6c65 7665  ME...header_leve
+00001d60: 6c94 4b02 7568 2b68 0a68 1e4b 1a68 1d68  l.K.uh+h.h.K.h.h
+00001d70: 2c68 1b68 0c68 1c68 0375 6268 0b29 8194  ,h.h.h.h.ubh.)..
+00001d80: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
+00001d90: 947d 9428 6805 8c0c 436f 6e74 7269 6275  .}.(h...Contribu
+00001da0: 7469 6e67 9468 075d 9468 168c 0c43 6f6e  ting.h.].h...Con
+00001db0: 7472 6962 7574 696e 6794 8594 8194 7d94  tributing.....}.
+00001dc0: 2868 0568 0668 1b6a 0102 0000 681c 6803  (h.h.h.j....h.h.
+00001dd0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00001de0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00001df0: 5d94 7568 2b68 0f68 1e4b 2768 1d68 2c68  ].uh+h.h.K'h.h,h
+00001e00: 1b6a fe01 0000 681c 6803 7562 682e 2981  .j....h.h.ubh.).
+00001e10: 947d 9428 6805 8c91 436f 6e74 7269 6275  .}.(h...Contribu
+00001e20: 7469 6f6e 7320 6172 6520 7665 7279 2077  tions are very w
+00001e30: 656c 636f 6d65 2e20 5465 7374 7320 6361  elcome. Tests ca
+00001e40: 6e20 6265 2072 756e 2077 6974 6820 5b74  n be run with [t
+00001e50: 6f78 5d2c 2070 6c65 6173 6520 656e 7375  ox], please ensu
+00001e60: 7265 0a74 6865 2063 6f76 6572 6167 6520  re.the coverage 
+00001e70: 6174 206c 6561 7374 2073 7461 7973 2074  at least stays t
+00001e80: 6865 2073 616d 6520 6265 666f 7265 2079  he same before y
+00001e90: 6f75 2073 7562 6d69 7420 6120 7075 6c6c  ou submit a pull
+00001ea0: 2072 6571 7565 7374 2e94 6807 5d94 2868   request..h.].(h
+00001eb0: 168c 3643 6f6e 7472 6962 7574 696f 6e73  ..6Contributions
+00001ec0: 2061 7265 2076 6572 7920 7765 6c63 6f6d   are very welcom
+00001ed0: 652e 2054 6573 7473 2063 616e 2062 6520  e. Tests can be 
+00001ee0: 7275 6e20 7769 7468 2094 8594 8194 7d94  run with .....}.
+00001ef0: 2868 0568 0668 1b6a 0f02 0000 681c 6803  (h.h.h.j....h.h.
+00001f00: 681d 4e68 1e4e 7562 6834 2981 947d 9428  h.Nh.Nubh4)..}.(
+00001f10: 6805 8c03 746f 7894 6807 5d94 6816 8c03  h...tox.h.].h...
+00001f20: 746f 7894 8594 8194 7d94 2868 0568 0668  tox.....}.(h.h.h
+00001f30: 1b6a 1702 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00001f40: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001f50: 6825 5d94 6827 5d94 6829 5d94 6850 8c25  h%].h'].h)].hP.%
+00001f60: 6874 7470 733a 2f2f 746f 782e 7265 6164  https://tox.read
+00001f70: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00001f80: 7465 7374 2f94 7568 2b68 3368 1e4b 2968  test/.uh+h3h.K)h
+00001f90: 1d68 2c68 1b6a 0f02 0000 681c 6803 7562  .h,h.j....h.h.ub
+00001fa0: 6816 8c0f 2c20 706c 6561 7365 2065 6e73  h..., please ens
+00001fb0: 7572 6594 8594 8194 7d94 2868 0568 0668  ure.....}.(h.h.h
+00001fc0: 1b6a 0f02 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00001fd0: 7562 6816 8c01 0a94 8594 8194 7d94 2868  ubh.........}.(h
+00001fe0: 0568 0668 1b6a 0f02 0000 681c 6803 681d  .h.h.j....h.h.h.
+00001ff0: 4e68 1e4e 7562 6816 8c46 7468 6520 636f  Nh.Nubh..Fthe co
+00002000: 7665 7261 6765 2061 7420 6c65 6173 7420  verage at least 
+00002010: 7374 6179 7320 7468 6520 7361 6d65 2062  stays the same b
+00002020: 6566 6f72 6520 796f 7520 7375 626d 6974  efore you submit
+00002030: 2061 2070 756c 6c20 7265 7175 6573 742e   a pull request.
+00002040: 9485 9481 947d 9428 6805 6806 681b 6a0f  .....}.(h.h.h.j.
+00002050: 0200 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
+00002060: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00002070: 9468 275d 9468 295d 9475 682b 682d 681e  .h'].h)].uh+h-h.
+00002080: 4b29 681d 682c 681b 6afe 0100 0068 1c68  K)h.h,h.j....h.h
+00002090: 0375 6265 681f 7d94 2868 215d 948c 0c63  .ubeh.}.(h!]...c
+000020a0: 6f6e 7472 6962 7574 696e 6794 6168 235d  ontributing.ah#]
+000020b0: 9468 255d 948c 0c63 6f6e 7472 6962 7574  .h%]...contribut
+000020c0: 696e 6794 6168 275d 9468 295d 946a fb01  ing.ah'].h)].j..
+000020d0: 0000 6afc 0100 006a fd01 0000 4b03 7568  ..j....j....K.uh
+000020e0: 2b68 0a68 1e4b 2768 1d68 2c68 1b68 0c68  +h.h.K'h.h,h.h.h
+000020f0: 1c68 0375 6268 0b29 8194 7d94 2868 0568  .h.ubh.)..}.(h.h
+00002100: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
+00002110: 8c07 4c69 6365 6e73 6594 6807 5d94 6816  ..License.h.].h.
+00002120: 8c07 4c69 6365 6e73 6594 8594 8194 7d94  ..License.....}.
+00002130: 2868 0568 0668 1b6a 4302 0000 681c 6803  (h.h.h.jC...h.h.
+00002140: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00002150: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002160: 5d94 7568 2b68 0f68 1e4b 2c68 1d68 2c68  ].uh+h.h.K,h.h,h
+00002170: 1b6a 4002 0000 681c 6803 7562 682e 2981  .j@...h.h.ubh.).
+00002180: 947d 9428 6805 8c6f 4469 7374 7269 6275  .}.(h..oDistribu
+00002190: 7465 6420 756e 6465 7220 7468 6520 7465  ted under the te
+000021a0: 726d 7320 6f66 2074 6865 205b 4253 442d  rms of the [BSD-
+000021b0: 335d 206c 6963 656e 7365 2c0a 2276 6f6c  3] license,."vol
+000021c0: 6c73 6567 2d6e 6170 6172 692d 7472 6163  lseg-napari-trac
+000021d0: 6b6d 6174 6522 2069 7320 6672 6565 2061  kmate" is free a
+000021e0: 6e64 206f 7065 6e20 736f 7572 6365 2073  nd open source s
+000021f0: 6f66 7477 6172 6594 6807 5d94 2868 168c  oftware.h.].(h..
+00002200: 2344 6973 7472 6962 7574 6564 2075 6e64  #Distributed und
+00002210: 6572 2074 6865 2074 6572 6d73 206f 6620  er the terms of 
+00002220: 7468 6520 9485 9481 947d 9428 6805 6806  the .....}.(h.h.
+00002230: 681b 6a51 0200 0068 1c68 0368 1d4e 681e  h.jQ...h.h.h.Nh.
+00002240: 4e75 6268 3429 8194 7d94 2868 058c 0542  Nubh4)..}.(h...B
+00002250: 5344 2d33 9468 075d 9468 168c 0542 5344  SD-3.h.].h...BSD
+00002260: 2d33 9485 9481 947d 9428 6805 6806 681b  -3.....}.(h.h.h.
+00002270: 6a59 0200 0068 1c68 0368 1d4e 681e 4e75  jY...h.h.h.Nh.Nu
+00002280: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00002290: 255d 9468 275d 9468 295d 9468 508c 2b68  %].h'].h)].hP.+h
+000022a0: 7474 703a 2f2f 6f70 656e 736f 7572 6365  ttp://opensource
+000022b0: 2e6f 7267 2f6c 6963 656e 7365 732f 4253  .org/licenses/BS
+000022c0: 442d 332d 436c 6175 7365 9475 682b 6833  D-3-Clause.uh+h3
+000022d0: 681e 4b2e 681d 682c 681b 6a51 0200 0068  h.K.h.h,h.jQ...h
+000022e0: 1c68 0375 6268 168c 0920 6c69 6365 6e73  .h.ubh... licens
+000022f0: 652c 9485 9481 947d 9428 6805 6806 681b  e,.....}.(h.h.h.
+00002300: 6a51 0200 0068 1c68 0368 1d4e 681e 4e75  jQ...h.h.h.Nh.Nu
+00002310: 6268 168c 010a 9485 9481 947d 9428 6805  bh.........}.(h.
+00002320: 6806 681b 6a51 0200 0068 1c68 0368 1d4e  h.h.jQ...h.h.h.N
+00002330: 681e 4e75 6268 168c 3fe2 809c 766f 6c6c  h.Nubh..?...voll
+00002340: 7365 672d 6e61 7061 7269 2d74 7261 636b  seg-napari-track
+00002350: 6d61 7465 e280 9d20 6973 2066 7265 6520  mate... is free 
+00002360: 616e 6420 6f70 656e 2073 6f75 7263 6520  and open source 
+00002370: 736f 6674 7761 7265 9485 9481 947d 9428  software.....}.(
+00002380: 6805 6806 681b 6a51 0200 0068 1c68 0368  h.h.h.jQ...h.h.h
+00002390: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
+000023a0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000023b0: 9475 682b 682d 681e 4b2e 681d 682c 681b  .uh+h-h.K.h.h,h.
+000023c0: 6a40 0200 0068 1c68 0375 6265 681f 7d94  j@...h.h.ubeh.}.
+000023d0: 2868 215d 948c 076c 6963 656e 7365 9461  (h!]...license.a
+000023e0: 6823 5d94 6825 5d94 8c07 6c69 6365 6e73  h#].h%]...licens
+000023f0: 6594 6168 275d 9468 295d 946a fb01 0000  e.ah'].h)].j....
+00002400: 6afc 0100 006a fd01 0000 4b04 7568 2b68  j....j....K.uh+h
+00002410: 0a68 1e4b 2c68 1d68 2c68 1b68 0c68 1c68  .h.K,h.h,h.h.h.h
+00002420: 0375 6268 0b29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
+00002430: 075d 9428 6810 2981 947d 9428 6805 8c06  .].(h.)..}.(h...
+00002440: 4973 7375 6573 9468 075d 9468 168c 0649  Issues.h.].h...I
+00002450: 7373 7565 7394 8594 8194 7d94 2868 0568  ssues.....}.(h.h
+00002460: 0668 1b6a 8502 0000 681c 6803 681d 4e68  .h.j....h.h.h.Nh
+00002470: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00002480: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00002490: 2b68 0f68 1e4b 3168 1d68 2c68 1b6a 8202  +h.h.K1h.h,h.j..
+000024a0: 0000 681c 6803 7562 682e 2981 947d 9428  ..h.h.ubh.)..}.(
+000024b0: 6805 8c58 4966 2079 6f75 2065 6e63 6f75  h..XIf you encou
+000024c0: 6e74 6572 2061 6e79 2070 726f 626c 656d  nter any problem
+000024d0: 732c 2070 6c65 6173 6520 5b66 696c 6520  s, please [file 
+000024e0: 616e 2069 7373 7565 5d20 616c 6f6e 6720  an issue] along 
+000024f0: 7769 7468 2061 2064 6574 6169 6c65 6420  with a detailed 
+00002500: 6465 7363 7269 7074 696f 6e2e 9468 075d  description..h.]
+00002510: 9428 6816 8c26 4966 2079 6f75 2065 6e63  .(h..&If you enc
+00002520: 6f75 6e74 6572 2061 6e79 2070 726f 626c  ounter any probl
+00002530: 656d 732c 2070 6c65 6173 6520 9485 9481  ems, please ....
+00002540: 947d 9428 6805 6806 681b 6a93 0200 0068  .}.(h.h.h.j....h
+00002550: 1c68 0368 1d4e 681e 4e75 6268 3429 8194  .h.h.Nh.Nubh4)..
+00002560: 7d94 2868 058c 0d66 696c 6520 616e 2069  }.(h...file an i
+00002570: 7373 7565 9468 075d 9468 168c 0d66 696c  ssue.h.].h...fil
+00002580: 6520 616e 2069 7373 7565 9485 9481 947d  e an issue.....}
+00002590: 9428 6805 6806 681b 6a9b 0200 0068 1c68  .(h.h.h.j....h.h
+000025a0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+000025b0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000025c0: 295d 9468 508c 4068 7474 7073 3a2f 2f67  )].hP.@https://g
+000025d0: 6974 6875 622e 636f 6d2f 4b61 706f 6f72  ithub.com/Kapoor
+000025e0: 6c61 6273 2d43 4150 4544 2f76 6f6c 6c73  labs-CAPED/volls
+000025f0: 6567 2d6e 6170 6172 692d 6d74 7261 636b  eg-napari-mtrack
+00002600: 2f69 7373 7565 7394 7568 2b68 3368 1e4b  /issues.uh+h3h.K
+00002610: 3368 1d68 2c68 1b6a 9302 0000 681c 6803  3h.h,h.j....h.h.
+00002620: 7562 6816 8c23 2061 6c6f 6e67 2077 6974  ubh..# along wit
+00002630: 6820 6120 6465 7461 696c 6564 2064 6573  h a detailed des
+00002640: 6372 6970 7469 6f6e 2e94 8594 8194 7d94  cription......}.
+00002650: 2868 0568 0668 1b6a 9302 0000 681c 6803  (h.h.h.j....h.h.
+00002660: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
+00002670: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002680: 5d94 7568 2b68 2d68 1e4b 3368 1d68 2c68  ].uh+h-h.K3h.h,h
+00002690: 1b6a 8202 0000 681c 6803 7562 6568 1f7d  .j....h.h.ubeh.}
+000026a0: 9428 6821 5d94 8c06 6973 7375 6573 9461  .(h!]...issues.a
+000026b0: 6823 5d94 6825 5d94 8c06 6973 7375 6573  h#].h%]...issues
+000026c0: 9461 6827 5d94 6829 5d94 6afb 0100 006a  .ah'].h)].j....j
+000026d0: fc01 0000 6afd 0100 004b 0575 682b 680a  ....j....K.uh+h.
+000026e0: 681e 4b31 681d 682c 681b 680c 681c 6803  h.K1h.h,h.h.h.h.
+000026f0: 7562 6568 1f7d 9428 6821 5d94 8c18 766f  ubeh.}.(h!]...vo
+00002700: 6c6c 7365 672d 6e61 7061 7269 2d74 7261  llseg-napari-tra
+00002710: 636b 6d61 7465 9461 6823 5d94 288c 0e74  ckmate.ah#].(..t
+00002720: 6578 326a 6178 5f69 676e 6f72 6594 8c0e  ex2jax_ignore...
+00002730: 6d61 7468 6a61 785f 6967 6e6f 7265 9465  mathjax_ignore.e
+00002740: 6825 5d94 8c18 766f 6c6c 7365 672d 6e61  h%]...vollseg-na
+00002750: 7061 7269 2d74 7261 636b 6d61 7465 9461  pari-trackmate.a
+00002760: 6827 5d94 6829 5d94 6afb 0100 006a fc01  h'].h)].j....j..
+00002770: 0000 6afd 0100 004b 0175 682b 680a 681e  ..j....K.uh+h.h.
+00002780: 4b01 681d 682c 681b 6803 681c 6803 7562  K.h.h,h.h.h.h.ub
+00002790: 6809 8c08 636f 6d70 6f75 6e64 9493 9429  h...compound...)
+000027a0: 8194 7d94 2868 0568 0668 075d 9468 008c  ..}.(h.h.h.].h..
+000027b0: 0774 6f63 7472 6565 9493 9429 8194 7d94  .toctree...)..}.
+000027c0: 2868 0568 0668 075d 9468 1f7d 9428 6821  (h.h.h.].h.}.(h!
+000027d0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000027e0: 5d94 681b 6afc 0100 008c 0765 6e74 7269  ].h.j......entri
+000027f0: 6573 945d 944e 8c09 414c 474f 5249 5448  es.].N..ALGORITH
+00002800: 4d94 8694 618c 0c69 6e63 6c75 6465 6669  M...a..includefi
+00002810: 6c65 7394 5d94 6ad8 0200 0061 8c08 6d61  les.].j....a..ma
+00002820: 7864 6570 7468 944a ffff ffff 8c07 6361  xdepth.J......ca
+00002830: 7074 696f 6e94 4e8c 0a72 6177 6361 7074  ption.N..rawcapt
+00002840: 696f 6e94 6806 8c04 676c 6f62 9489 8c06  ion.h...glob....
+00002850: 6869 6464 656e 9488 8c0d 696e 636c 7564  hidden....includ
+00002860: 6568 6964 6465 6e94 898c 086e 756d 6265  ehidden....numbe
+00002870: 7265 6494 4b00 8c0a 7469 746c 6573 6f6e  red.K...titleson
+00002880: 6c79 9488 7568 2b6a cb02 0000 681d 682c  ly..uh+j....h.h,
+00002890: 681e 4b01 681b 6ac8 0200 0075 6261 681f  h.K.h.j....ubah.
+000028a0: 7d94 2868 215d 9468 235d 948c 0f74 6f63  }.(h!].h#]...toc
+000028b0: 7472 6565 2d77 7261 7070 6572 9461 6825  tree-wrapper.ah%
+000028c0: 5d94 6827 5d94 6829 5d94 6afb 0100 006a  ].h'].h)].j....j
+000028d0: fc01 0000 6add 0200 004e 7568 2b6a c602  ....j....Nuh+j..
+000028e0: 0000 7562 6568 1f7d 9428 6821 5d94 6823  ..ubeh.}.(h!].h#
+000028f0: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
+00002900: 736f 7572 6365 9468 2c75 682b 6801 8c0e  source.h,uh+h...
+00002910: 6375 7272 656e 745f 736f 7572 6365 944e  current_source.N
+00002920: 8c0c 6375 7272 656e 745f 6c69 6e65 944e  ..current_line.N
+00002930: 8c08 7365 7474 696e 6773 948c 1164 6f63  ..settings...doc
+00002940: 7574 696c 732e 6672 6f6e 7465 6e64 948c  utils.frontend..
+00002950: 0656 616c 7565 7394 9394 2981 947d 9428  .Values...)..}.(
+00002960: 680f 4e8c 0967 656e 6572 6174 6f72 944e  h.N..generator.N
+00002970: 8c09 6461 7465 7374 616d 7094 4e8c 0b73  ..datestamp.N..s
+00002980: 6f75 7263 655f 6c69 6e6b 944e 8c0a 736f  ource_link.N..so
+00002990: 7572 6365 5f75 726c 944e 8c0d 746f 635f  urce_url.N..toc_
+000029a0: 6261 636b 6c69 6e6b 7394 8c05 656e 7472  backlinks...entr
+000029b0: 7994 8c12 666f 6f74 6e6f 7465 5f62 6163  y...footnote_bac
+000029c0: 6b6c 696e 6b73 944b 018c 0d73 6563 746e  klinks.K...sectn
+000029d0: 756d 5f78 666f 726d 944b 018c 0e73 7472  um_xform.K...str
+000029e0: 6970 5f63 6f6d 6d65 6e74 7394 4e8c 1b73  ip_comments.N..s
+000029f0: 7472 6970 5f65 6c65 6d65 6e74 735f 7769  trip_elements_wi
+00002a00: 7468 5f63 6c61 7373 6573 944e 8c0d 7374  th_classes.N..st
+00002a10: 7269 705f 636c 6173 7365 7394 4e8c 0c72  rip_classes.N..r
+00002a20: 6570 6f72 745f 6c65 7665 6c94 4b02 8c0a  eport_level.K...
+00002a30: 6861 6c74 5f6c 6576 656c 944b 058c 1165  halt_level.K...e
+00002a40: 7869 745f 7374 6174 7573 5f6c 6576 656c  xit_status_level
+00002a50: 944b 058c 0564 6562 7567 944e 8c0e 7761  .K...debug.N..wa
+00002a60: 726e 696e 675f 7374 7265 616d 944e 8c09  rning_stream.N..
+00002a70: 7472 6163 6562 6163 6b94 888c 0e69 6e70  traceback....inp
+00002a80: 7574 5f65 6e63 6f64 696e 6794 8c09 7574  ut_encoding...ut
+00002a90: 662d 382d 7369 6794 8c1c 696e 7075 745f  f-8-sig...input_
+00002aa0: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
+00002ab0: 616e 646c 6572 948c 0673 7472 6963 7494  andler...strict.
+00002ac0: 8c0f 6f75 7470 7574 5f65 6e63 6f64 696e  ..output_encodin
+00002ad0: 6794 8c05 7574 662d 3894 8c1d 6f75 7470  g...utf-8...outp
+00002ae0: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
+00002af0: 725f 6861 6e64 6c65 7294 6a0e 0300 008c  r_handler.j.....
+00002b00: 0e65 7272 6f72 5f65 6e63 6f64 696e 6794  .error_encoding.
+00002b10: 8c05 7574 662d 3894 8c1c 6572 726f 725f  ..utf-8...error_
+00002b20: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
+00002b30: 616e 646c 6572 948c 1062 6163 6b73 6c61  andler...backsla
+00002b40: 7368 7265 706c 6163 6594 8c0d 6c61 6e67  shreplace...lang
+00002b50: 7561 6765 5f63 6f64 6594 8c02 656e 948c  uage_code...en..
+00002b60: 1372 6563 6f72 645f 6465 7065 6e64 656e  .record_dependen
+00002b70: 6369 6573 944e 8c06 636f 6e66 6967 944e  cies.N..config.N
+00002b80: 8c09 6964 5f70 7265 6669 7894 6806 8c0e  ..id_prefix.h...
+00002b90: 6175 746f 5f69 645f 7072 6566 6978 948c  auto_id_prefix..
+00002ba0: 0269 6494 8c0d 6475 6d70 5f73 6574 7469  .id...dump_setti
+00002bb0: 6e67 7394 4e8c 0e64 756d 705f 696e 7465  ngs.N..dump_inte
+00002bc0: 726e 616c 7394 4e8c 0f64 756d 705f 7472  rnals.N..dump_tr
+00002bd0: 616e 7366 6f72 6d73 944e 8c0f 6475 6d70  ansforms.N..dump
+00002be0: 5f70 7365 7564 6f5f 786d 6c94 4e8c 1065  _pseudo_xml.N..e
+00002bf0: 7870 6f73 655f 696e 7465 726e 616c 7394  xpose_internals.
+00002c00: 4e8c 0e73 7472 6963 745f 7669 7369 746f  N..strict_visito
+00002c10: 7294 4e8c 0f5f 6469 7361 626c 655f 636f  r.N.._disable_co
+00002c20: 6e66 6967 944e 8c07 5f73 6f75 7263 6594  nfig.N.._source.
+00002c30: 682c 8c0c 5f64 6573 7469 6e61 7469 6f6e  h,.._destination
+00002c40: 944e 8c0d 5f63 6f6e 6669 675f 6669 6c65  .N.._config_file
+00002c50: 7394 5d94 8c16 6669 6c65 5f69 6e73 6572  s.]...file_inser
+00002c60: 7469 6f6e 5f65 6e61 626c 6564 9488 8c0b  tion_enabled....
+00002c70: 7261 775f 656e 6162 6c65 6494 4b01 8c11  raw_enabled.K...
+00002c80: 6c69 6e65 5f6c 656e 6774 685f 6c69 6d69  line_length_limi
+00002c90: 7494 4d10 278c 0e70 6570 5f72 6566 6572  t.M.'..pep_refer
+00002ca0: 656e 6365 7394 4e8c 0c70 6570 5f62 6173  ences.N..pep_bas
+00002cb0: 655f 7572 6c94 8c18 6874 7470 733a 2f2f  e_url...https://
+00002cc0: 7065 7073 2e70 7974 686f 6e2e 6f72 672f  peps.python.org/
+00002cd0: 948c 1570 6570 5f66 696c 655f 7572 6c5f  ...pep_file_url_
+00002ce0: 7465 6d70 6c61 7465 948c 0870 6570 2d25  template...pep-%
+00002cf0: 3034 6494 8c0e 7266 635f 7265 6665 7265  04d...rfc_refere
+00002d00: 6e63 6573 944e 8c0c 7266 635f 6261 7365  nces.N..rfc_base
+00002d10: 5f75 726c 948c 2668 7474 7073 3a2f 2f64  _url..&https://d
+00002d20: 6174 6174 7261 636b 6572 2e69 6574 662e  atatracker.ietf.
+00002d30: 6f72 672f 646f 632f 6874 6d6c 2f94 8c09  org/doc/html/...
+00002d40: 7461 625f 7769 6474 6894 4b08 8c1d 7472  tab_width.K...tr
+00002d50: 696d 5f66 6f6f 746e 6f74 655f 7265 6665  im_footnote_refe
+00002d60: 7265 6e63 655f 7370 6163 6594 898c 1073  rence_space....s
+00002d70: 796e 7461 785f 6869 6768 6c69 6768 7494  yntax_highlight.
+00002d80: 8c04 6c6f 6e67 948c 0c73 6d61 7274 5f71  ..long...smart_q
+00002d90: 756f 7465 7394 888c 1373 6d61 7274 7175  uotes....smartqu
+00002da0: 6f74 6573 5f6c 6f63 616c 6573 945d 948c  otes_locales.]..
+00002db0: 1d63 6861 7261 6374 6572 5f6c 6576 656c  .character_level
+00002dc0: 5f69 6e6c 696e 655f 6d61 726b 7570 9489  _inline_markup..
+00002dd0: 8c0e 646f 6374 6974 6c65 5f78 666f 726d  ..doctitle_xform
+00002de0: 9489 8c0d 646f 6369 6e66 6f5f 7866 6f72  ....docinfo_xfor
+00002df0: 6d94 4b01 8c12 7365 6374 7375 6274 6974  m.K...sectsubtit
+00002e00: 6c65 5f78 666f 726d 9489 8c0c 656d 6265  le_xform....embe
+00002e10: 645f 696d 6167 6573 9489 8c10 656d 6265  d_images....embe
+00002e20: 645f 7374 796c 6573 6865 6574 9489 8c15  d_stylesheet....
+00002e30: 636c 6f61 6b5f 656d 6169 6c5f 6164 6472  cloak_email_addr
+00002e40: 6573 7365 7394 888c 1173 6563 7469 6f6e  esses....section
+00002e50: 5f73 656c 665f 6c69 6e6b 9489 8c03 656e  _self_link....en
+00002e60: 7694 4e75 628c 0872 6570 6f72 7465 7294  v.Nub..reporter.
+00002e70: 4e8c 1069 6e64 6972 6563 745f 7461 7267  N..indirect_targ
+00002e80: 6574 7394 5d94 8c11 7375 6273 7469 7475  ets.]...substitu
+00002e90: 7469 6f6e 5f64 6566 7394 7d94 288c 0f77  tion_defs.}.(..w
+00002ea0: 6f72 6463 6f75 6e74 2d77 6f72 6473 9468  ordcount-words.h
+00002eb0: 098c 1773 7562 7374 6974 7574 696f 6e5f  ...substitution_
+00002ec0: 6465 6669 6e69 7469 6f6e 9493 9429 8194  definition...)..
+00002ed0: 7d94 2868 058c 0331 3032 9468 075d 9468  }.(h...102.h.].h
+00002ee0: 168c 0331 3032 9485 9481 947d 9428 6805  ...102.....}.(h.
+00002ef0: 6806 681b 6a4b 0300 0075 6261 681f 7d94  h.h.jK...ubah.}.
+00002f00: 2868 215d 9468 235d 9468 255d 948c 0f77  (h!].h#].h%]...w
+00002f10: 6f72 6463 6f75 6e74 2d77 6f72 6473 9461  ordcount-words.a
+00002f20: 6827 5d94 6829 5d94 7568 2b6a 4903 0000  h'].h)].uh+jI...
+00002f30: 681d 682c 7562 8c11 776f 7264 636f 756e  h.h,ub..wordcoun
+00002f40: 742d 6d69 6e75 7465 7394 6a4a 0300 0029  t-minutes.jJ...)
+00002f50: 8194 7d94 2868 058c 0131 9468 075d 9468  ..}.(h...1.h.].h
+00002f60: 168c 0131 9485 9481 947d 9428 6805 6806  ...1.....}.(h.h.
+00002f70: 681b 6a5b 0300 0075 6261 681f 7d94 2868  h.j[...ubah.}.(h
+00002f80: 215d 9468 235d 9468 255d 948c 1177 6f72  !].h#].h%]...wor
+00002f90: 6463 6f75 6e74 2d6d 696e 7574 6573 9461  dcount-minutes.a
+00002fa0: 6827 5d94 6829 5d94 7568 2b6a 4903 0000  h'].h)].uh+jI...
+00002fb0: 681d 682c 7562 758c 1273 7562 7374 6974  h.h,ubu..substit
+00002fc0: 7574 696f 6e5f 6e61 6d65 7394 7d94 288c  ution_names.}.(.
+00002fd0: 0f77 6f72 6463 6f75 6e74 2d77 6f72 6473  .wordcount-words
+00002fe0: 946a 4803 0000 8c11 776f 7264 636f 756e  .jH.....wordcoun
+00002ff0: 742d 6d69 6e75 7465 7394 6a5a 0300 0075  t-minutes.jZ...u
+00003000: 8c08 7265 666e 616d 6573 947d 948c 0672  ..refnames.}...r
+00003010: 6566 6964 7394 7d94 8c07 6e61 6d65 6964  efids.}...nameid
+00003020: 7394 7d94 286a c302 0000 6abe 0200 006a  s.}.(j....j....j
+00003030: f801 0000 6af5 0100 006a 3d02 0000 6a3a  ....j....j=...j:
+00003040: 0200 006a 7f02 0000 6a7c 0200 006a b902  ...j....j|...j..
+00003050: 0000 6ab6 0200 0075 8c09 6e61 6d65 7479  ..j....u..namety
+00003060: 7065 7394 7d94 286a c302 0000 4e6a f801  pes.}.(j....Nj..
+00003070: 0000 4e6a 3d02 0000 4e6a 7f02 0000 4e6a  ..Nj=...Nj....Nj
+00003080: b902 0000 4e75 6821 7d94 286a be02 0000  ....Nuh!}.(j....
+00003090: 680c 6af5 0100 006a 7e01 0000 6a3a 0200  h.j....j~...j:..
+000030a0: 006a fe01 0000 6a7c 0200 006a 4002 0000  .j....j|...j@...
+000030b0: 6ab6 0200 006a 8202 0000 758c 0d66 6f6f  j....j....u..foo
+000030c0: 746e 6f74 655f 7265 6673 947d 948c 0d63  tnote_refs.}...c
+000030d0: 6974 6174 696f 6e5f 7265 6673 947d 948c  itation_refs.}..
+000030e0: 0d61 7574 6f66 6f6f 746e 6f74 6573 945d  .autofootnotes.]
+000030f0: 948c 1161 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+00003100: 7265 6673 945d 948c 1073 796d 626f 6c5f  refs.]...symbol_
+00003110: 666f 6f74 6e6f 7465 7394 5d94 8c14 7379  footnotes.]...sy
+00003120: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7265  mbol_footnote_re
+00003130: 6673 945d 948c 0966 6f6f 746e 6f74 6573  fs.]...footnotes
+00003140: 945d 948c 0963 6974 6174 696f 6e73 945d  .]...citations.]
+00003150: 948c 1261 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+00003160: 7374 6172 7494 4b01 8c15 7379 6d62 6f6c  start.K...symbol
+00003170: 5f66 6f6f 746e 6f74 655f 7374 6172 7494  _footnote_start.
+00003180: 4b00 8c0a 6964 5f63 6f75 6e74 6572 948c  K...id_counter..
+00003190: 0b63 6f6c 6c65 6374 696f 6e73 948c 0743  .collections...C
+000031a0: 6f75 6e74 6572 9493 947d 9485 9452 948c  ounter...}...R..
+000031b0: 0e70 6172 7365 5f6d 6573 7361 6765 7394  .parse_messages.
+000031c0: 5d94 8c12 7472 616e 7366 6f72 6d5f 6d65  ]...transform_me
+000031d0: 7373 6167 6573 945d 948c 0b74 7261 6e73  ssages.]...trans
+000031e0: 666f 726d 6572 944e 8c0b 696e 636c 7564  former.N..includ
+000031f0: 655f 6c6f 6794 5d94 8c0a 6465 636f 7261  e_log.]...decora
+00003200: 7469 6f6e 944e 681c 6803 7562 2e0a       tion.Nh.h.ub..
```

### Comparing `vollseg-napari-trackmate-2.2.5/_build/.doctrees/environment.pickle` & `vollseg-napari-trackmate-2.2.6/_build/.doctrees/environment.pickle`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9563 6d00 0000 0000 008c 1273 7068  ...cm........sph
+00000000: 8005 95cc 7400 0000 0000 008c 1273 7068  ....t........sph
 00000010: 696e 782e 656e 7669 726f 6e6d 656e 7494  inx.environment.
 00000020: 8c10 4275 696c 6445 6e76 6972 6f6e 6d65  ..BuildEnvironme
 00000030: 6e74 9493 9429 8194 7d94 288c 0361 7070  nt...)..}.(..app
 00000040: 944e 8c0a 646f 6374 7265 6564 6972 948c  .N..doctreedir..
 00000050: 572f 6d6e 742f 632f 5573 6572 732f 7261  W/mnt/c/Users/ra
 00000060: 6e64 6f2f 446f 776e 6c6f 6164 732f 5079  ndo/Downloads/Py
 00000070: 7468 6f6e 5f57 6f72 6b73 7061 6365 2f76  thon_Workspace/v
@@ -154,1598 +154,1717 @@
 00000990: 636f 6465 2d62 6c6f 636b 948c 0a4c 6973  code-block...Lis
 000009a0: 7469 6e67 2025 7394 758c 1165 7874 6572  ting %s.u..exter
 000009b0: 6e61 6c5f 7369 7465 5f6d 6170 948c 1773  nal_site_map...s
 000009c0: 7068 696e 785f 6578 7465 726e 616c 5f74  phinx_external_t
 000009d0: 6f63 2e61 7069 948c 0753 6974 654d 6170  oc.api...SiteMap
 000009e0: 9493 9429 8194 7d94 288c 055f 646f 6373  ...)..}.(.._docs
 000009f0: 947d 9428 8c06 5245 4144 4d45 9468 998c  .}.(..README.h..
-00000a00: 0844 6f63 756d 656e 7494 9394 2981 947d  .Document...)..}
-00000a10: 9428 8c07 646f 636e 616d 6594 68a0 8c08  .(..docname.h...
-00000a20: 7375 6274 7265 6573 945d 9468 998c 0754  subtrees.].h...T
-00000a30: 6f63 5472 6565 9493 9429 8194 7d94 288c  ocTree...)..}.(.
-00000a40: 0569 7465 6d73 945d 9468 998c 0846 696c  .items.].h...Fil
-00000a50: 6549 7465 6d94 9394 8c09 414c 474f 5249  eItem.....ALGORI
-00000a60: 5448 4d94 8594 8194 618c 0763 6170 7469  THM.....a..capti
-00000a70: 6f6e 944e 8c06 6869 6464 656e 9488 8c08  on.N..hidden....
-00000a80: 6d61 7864 6570 7468 944a ffff ffff 8c08  maxdepth.J......
-00000a90: 6e75 6d62 6572 6564 9489 8c08 7265 7665  numbered....reve
-00000aa0: 7273 6564 9489 8c0a 7469 746c 6573 6f6e  rsed....titleson
-00000ab0: 6c79 9488 7562 618c 0574 6974 6c65 944e  ly..uba..title.N
-00000ac0: 7562 8c09 414c 474f 5249 5448 4d94 68a2  ub..ALGORITHM.h.
-00000ad0: 2981 947d 9428 68a5 68ba 68a6 5d94 68b9  )..}.(h.h.h.].h.
-00000ae0: 4e75 6275 8c05 5f72 6f6f 7494 68a3 8c05  Nubu.._root.h...
-00000af0: 5f6d 6574 6194 7d94 8c0c 5f66 696c 655f  _meta.}..._file_
-00000b00: 666f 726d 6174 948c 076a 622d 626f 6f6b  format...jb-book
-00000b10: 9475 628c 0a6d 6173 7465 725f 646f 6394  .ub..master_doc.
-00000b20: 68a0 8c0f 6d61 7468 6a61 7833 5f63 6f6e  h...mathjax3_con
-00000b30: 6669 6794 7d94 8c07 6f70 7469 6f6e 7394  fig.}...options.
-00000b40: 7d94 8c10 7072 6f63 6573 7348 746d 6c43  }...processHtmlC
-00000b50: 6c61 7373 948c 3074 6578 326a 6178 5f70  lass..0tex2jax_p
-00000b60: 726f 6365 7373 7c6d 6174 686a 6178 5f70  rocess|mathjax_p
-00000b70: 726f 6365 7373 7c6d 6174 687c 6f75 7470  rocess|math|outp
-00000b80: 7574 5f61 7265 6194 7373 8c14 6874 6d6c  ut_area.ss..html
-00000b90: 5f70 6572 6d61 6c69 6e6b 735f 6963 6f6e  _permalinks_icon
-00000ba0: 948c 0123 948c 0f6c 6174 6578 5f64 6f63  ...#...latex_doc
-00000bb0: 756d 656e 7473 945d 9428 68a0 8c1c 766f  uments.].(h...vo
-00000bc0: 6c6c 7365 672d 6e61 7061 7269 2d74 7261  llseg-napari-tra
-00000bd0: 636b 6d61 7465 2e74 6578 9468 388c 0c56  ckmate.tex.h8..V
-00000be0: 6172 756e 204b 6170 6f6f 7294 687b 7494  arun Kapoor.h{t.
-00000bf0: 618c 0676 616c 7565 7394 7d94 288c 0770  a..values.}.(..p
-00000c00: 726f 6a65 6374 948c 0650 7974 686f 6e94  roject...Python.
-00000c10: 8c03 656e 7694 4e87 9468 3968 3a68 d54e  ..env.N..h9h:h.N
-00000c20: 8794 8c11 7072 6f6a 6563 745f 636f 7079  ....project_copy
-00000c30: 7269 6768 7494 681f 8c04 6874 6d6c 944e  right.h...html.N
-00000c40: 8794 683b 683c 68d9 4e87 948c 0776 6572  ..h;h<h.N....ver
-00000c50: 7369 6f6e 9468 1f68 d54e 8794 8c07 7265  sion.h.h.N....re
-00000c60: 6c65 6173 6594 681f 68d5 4e87 948c 0574  lease.h.h.N....t
-00000c70: 6f64 6179 9468 1f68 d54e 8794 8c09 746f  oday.h.h.N....to
-00000c80: 6461 795f 666d 7494 4e68 d54e 8794 8c08  day_fmt.Nh.N....
-00000c90: 6c61 6e67 7561 6765 944e 68d5 4e87 948c  language.Nh.N...
-00000ca0: 0b6c 6f63 616c 655f 6469 7273 945d 948c  .locale_dirs.]..
-00000cb0: 076c 6f63 616c 6573 9461 68d5 4e87 948c  .locales.ah.N...
-00000cc0: 1866 6967 7572 655f 6c61 6e67 7561 6765  .figure_language
-00000cd0: 5f66 696c 656e 616d 6594 8c16 7b72 6f6f  _filename...{roo
-00000ce0: 747d 2e7b 6c61 6e67 7561 6765 7d7b 6578  t}.{language}{ex
-00000cf0: 747d 9468 d54e 8794 8c20 6765 7474 6578  t}.h.N... gettex
-00000d00: 745f 616c 6c6f 775f 6675 7a7a 795f 7472  t_allow_fuzzy_tr
-00000d10: 616e 736c 6174 696f 6e73 9489 8c07 6765  anslations....ge
-00000d20: 7474 6578 7494 4e87 9468 c368 a068 d54e  ttext.N..h.h.h.N
-00000d30: 8794 8c08 726f 6f74 5f64 6f63 9468 a068  ....root_doc.h.h
-00000d40: d54e 8794 6884 6888 68d5 4e87 948c 0f73  .N..h.h.h.N....s
-00000d50: 6f75 7263 655f 656e 636f 6469 6e67 948c  ource_encoding..
-00000d60: 0975 7466 2d38 2d73 6967 9468 d54e 8794  .utf-8-sig.h.N..
-00000d70: 683f 6840 68d5 4e87 948c 0c64 6566 6175  h?h@h.N....defau
-00000d80: 6c74 5f72 6f6c 6594 4e68 d54e 8794 8c18  lt_role.Nh.N....
-00000d90: 6164 645f 6675 6e63 7469 6f6e 5f70 6172  add_function_par
-00000da0: 656e 7468 6573 6573 9488 68d5 4e87 948c  entheses..h.N...
-00000db0: 1061 6464 5f6d 6f64 756c 655f 6e61 6d65  .add_module_name
-00000dc0: 7394 8868 d54e 8794 8c1d 7472 696d 5f66  s..h.N....trim_f
-00000dd0: 6f6f 746e 6f74 655f 7265 6665 7265 6e63  ootnote_referenc
-00000de0: 655f 7370 6163 6594 8968 d54e 8794 8c0c  e_space..h.N....
-00000df0: 7368 6f77 5f61 7574 686f 7273 9489 68d5  show_authors..h.
-00000e00: 4e87 9468 1268 1368 d94e 8794 8c12 6869  N..h.h.h.N....hi
-00000e10: 6768 6c69 6768 745f 6c61 6e67 7561 6765  ghlight_language
-00000e20: 948c 0764 6566 6175 6c74 9468 d54e 8794  ...default.h.N..
-00000e30: 8c11 6869 6768 6c69 6768 745f 6f70 7469  ..highlight_opti
-00000e40: 6f6e 7394 7d94 68d5 4e87 948c 0e74 656d  ons.}.h.N....tem
-00000e50: 706c 6174 6573 5f70 6174 6894 5d94 288c  plates_path.].(.
-00000e60: 7b2f 686f 6d65 2f76 6172 756e 6b61 706f  {/home/varunkapo
-00000e70: 6f72 2f61 6e61 636f 6e64 6133 2f65 6e76  or/anaconda3/env
-00000e80: 732f 6e61 7061 7269 656e 762f 6c69 622f  s/naparienv/lib/
-00000e90: 7079 7468 6f6e 332e 392f 7369 7465 2d70  python3.9/site-p
-00000ea0: 6163 6b61 6765 732f 7370 6869 6e78 5f62  ackages/sphinx_b
-00000eb0: 6f6f 6b5f 7468 656d 652f 7468 656d 652f  ook_theme/theme/
-00000ec0: 7370 6869 6e78 5f62 6f6f 6b5f 7468 656d  sphinx_book_them
-00000ed0: 652f 636f 6d70 6f6e 656e 7473 948c 7f2f  e/components.../
-00000ee0: 686f 6d65 2f76 6172 756e 6b61 706f 6f72  home/varunkapoor
-00000ef0: 2f61 6e61 636f 6e64 6133 2f65 6e76 732f  /anaconda3/envs/
-00000f00: 6e61 7061 7269 656e 762f 6c69 622f 7079  naparienv/lib/py
-00000f10: 7468 6f6e 332e 392f 7369 7465 2d70 6163  thon3.9/site-pac
-00000f20: 6b61 6765 732f 7079 6461 7461 5f73 7068  kages/pydata_sph
-00000f30: 696e 785f 7468 656d 652f 7468 656d 652f  inx_theme/theme/
-00000f40: 7079 6461 7461 5f73 7068 696e 785f 7468  pydata_sphinx_th
-00000f50: 656d 652f 636f 6d70 6f6e 656e 7473 948c  eme/components..
-00000f60: 7b2f 686f 6d65 2f76 6172 756e 6b61 706f  {/home/varunkapo
-00000f70: 6f72 2f61 6e61 636f 6e64 6133 2f65 6e76  or/anaconda3/env
-00000f80: 732f 6e61 7061 7269 656e 762f 6c69 622f  s/naparienv/lib/
-00000f90: 7079 7468 6f6e 332e 392f 7369 7465 2d70  python3.9/site-p
-00000fa0: 6163 6b61 6765 732f 7370 6869 6e78 5f62  ackages/sphinx_b
-00000fb0: 6f6f 6b5f 7468 656d 652f 7468 656d 652f  ook_theme/theme/
-00000fc0: 7370 6869 6e78 5f62 6f6f 6b5f 7468 656d  sphinx_book_them
-00000fd0: 652f 636f 6d70 6f6e 656e 7473 9465 68d9  e/components.eh.
-00000fe0: 4e87 948c 0f74 656d 706c 6174 655f 6272  N....template_br
-00000ff0: 6964 6765 944e 68d9 4e87 948c 0d6b 6565  idge.Nh.N....kee
-00001000: 705f 7761 726e 696e 6773 9489 68d5 4e87  p_warnings..h.N.
-00001010: 9468 3468 3568 d54e 8794 8c16 6d6f 6469  .h4h5h.N....modi
-00001020: 6e64 6578 5f63 6f6d 6d6f 6e5f 7072 6566  ndex_common_pref
-00001030: 6978 945d 9468 d94e 8794 8c0a 7273 745f  ix.].h.N....rst_
-00001040: 6570 696c 6f67 944e 68d5 4e87 948c 0a72  epilog.Nh.N....r
-00001050: 7374 5f70 726f 6c6f 6794 4e68 d54e 8794  st_prolog.Nh.N..
-00001060: 8c12 7472 696d 5f64 6f63 7465 7374 5f66  ..trim_doctest_f
-00001070: 6c61 6773 9488 68d5 4e87 948c 0e70 7269  lags..h.N....pri
-00001080: 6d61 7279 5f64 6f6d 6169 6e94 8c02 7079  mary_domain...py
-00001090: 9468 d54e 8794 8c0c 6e65 6564 735f 7370  .h.N....needs_sp
-000010a0: 6869 6e78 944e 4e4e 8794 8c10 6e65 6564  hinx.NNN....need
-000010b0: 735f 6578 7465 6e73 696f 6e73 947d 944e  s_extensions.}.N
-000010c0: 4e87 948c 0c6d 616e 7061 6765 735f 7572  N....manpages_ur
-000010d0: 6c94 4e68 d54e 8794 8c08 6e69 7470 6963  l.Nh.N....nitpic
-000010e0: 6b79 9489 4e4e 8794 8c0e 6e69 7470 6963  ky..NN....nitpic
-000010f0: 6b5f 6967 6e6f 7265 945d 944e 4e87 948c  k_ignore.].NN...
-00001100: 146e 6974 7069 636b 5f69 676e 6f72 655f  .nitpick_ignore_
-00001110: 7265 6765 7894 5d94 4e4e 8794 6833 8868  regex.].NN..h3.h
-00001120: d54e 8794 8c13 6e75 6d66 6967 5f73 6563  .N....numfig_sec
-00001130: 6e75 6d5f 6465 7074 6894 4b01 68d5 4e87  num_depth.K.h.N.
-00001140: 9468 8e68 8f68 d54e 8794 8c0f 6d61 7468  .h.h.h.N....math
-00001150: 5f6e 756d 6265 725f 616c 6c94 8968 d54e  _number_all..h.N
-00001160: 8794 8c11 6d61 7468 5f65 7172 6566 5f66  ....math_eqref_f
-00001170: 6f72 6d61 7494 4e68 d54e 8794 8c0b 6d61  ormat.Nh.N....ma
-00001180: 7468 5f6e 756d 6669 6794 8868 d54e 8794  th_numfig..h.N..
-00001190: 8c0a 746c 735f 7665 7269 6679 9488 68d5  ..tls_verify..h.
-000011a0: 4e87 948c 0b74 6c73 5f63 6163 6572 7473  N....tls_cacerts
-000011b0: 944e 68d5 4e87 948c 0a75 7365 725f 6167  .Nh.N....user_ag
-000011c0: 656e 7494 4e68 d54e 8794 8c0b 736d 6172  ent.Nh.N....smar
-000011d0: 7471 756f 7465 7394 8868 d54e 8794 8c12  tquotes..h.N....
-000011e0: 736d 6172 7471 756f 7465 735f 6163 7469  smartquotes_acti
-000011f0: 6f6e 948c 0371 4465 9468 d54e 8794 8c14  on...qDe.h.N....
-00001200: 736d 6172 7471 756f 7465 735f 6578 636c  smartquotes_excl
-00001210: 7564 6573 947d 9428 8c09 6c61 6e67 7561  udes.}.(..langua
-00001220: 6765 7394 5d94 8c02 6a61 9461 8c08 6275  ges.]...ja.a..bu
-00001230: 696c 6465 7273 945d 9428 8c03 6d61 6e94  ilders.].(..man.
-00001240: 8c04 7465 7874 9465 7568 d54e 8794 8c0d  ..text.euh.N....
-00001250: 6570 7562 5f62 6173 656e 616d 6594 68d4  epub_basename.h.
-00001260: 4e4e 8794 8c0c 6570 7562 5f76 6572 7369  NN....epub_versi
-00001270: 6f6e 9447 4008 0000 0000 0000 8c04 6570  on.G@.........ep
-00001280: 7562 944e 8794 8c0a 6570 7562 5f74 6865  ub.N....epub_the
-00001290: 6d65 946a 5101 0000 6a51 0100 004e 8794  me.jQ...jQ...N..
-000012a0: 8c12 6570 7562 5f74 6865 6d65 5f6f 7074  ..epub_theme_opt
-000012b0: 696f 6e73 947d 946a 5101 0000 4e87 948c  ions.}.jQ...N...
-000012c0: 0a65 7075 625f 7469 746c 6594 68d4 6a51  .epub_title.h.jQ
-000012d0: 0100 004e 8794 8c0b 6570 7562 5f61 7574  ...N....epub_aut
-000012e0: 686f 7294 683a 6a51 0100 004e 8794 8c0d  hor.h:jQ...N....
-000012f0: 6570 7562 5f6c 616e 6775 6167 6594 8c02  epub_language...
-00001300: 656e 946a 5101 0000 4e87 948c 0e65 7075  en.jQ...N....epu
-00001310: 625f 7075 626c 6973 6865 7294 683a 6a51  b_publisher.h:jQ
-00001320: 0100 004e 8794 8c0e 6570 7562 5f63 6f70  ...N....epub_cop
-00001330: 7972 6967 6874 9468 3c6a 5101 0000 4e87  yright.h<jQ...N.
-00001340: 948c 0f65 7075 625f 6964 656e 7469 6669  ...epub_identifi
-00001350: 6572 948c 0775 6e6b 6e6f 776e 946a 5101  er...unknown.jQ.
-00001360: 0000 4e87 948c 0b65 7075 625f 7363 6865  ..N....epub_sche
-00001370: 6d65 946a 6401 0000 6a51 0100 004e 8794  me.jd...jQ...N..
-00001380: 8c08 6570 7562 5f75 6964 946a 6401 0000  ..epub_uid.jd...
-00001390: 68d5 4e87 948c 0a65 7075 625f 636f 7665  h.N....epub_cove
-000013a0: 7294 2968 d54e 8794 8c0a 6570 7562 5f67  r.)h.N....epub_g
-000013b0: 7569 6465 9429 68d5 4e87 948c 0e65 7075  uide.)h.N....epu
-000013c0: 625f 7072 655f 6669 6c65 7394 5d94 68d5  b_pre_files.].h.
-000013d0: 4e87 948c 0f65 7075 625f 706f 7374 5f66  N....epub_post_f
-000013e0: 696c 6573 945d 9468 d54e 8794 687e 687f  iles.].h.N..h~h.
-000013f0: 6a51 0100 004e 8794 8c12 6570 7562 5f65  jQ...N....epub_e
-00001400: 7863 6c75 6465 5f66 696c 6573 945d 9468  xclude_files.].h
-00001410: d54e 8794 8c0d 6570 7562 5f74 6f63 6465  .N....epub_tocde
-00001420: 7074 6894 4b03 68d5 4e87 948c 0b65 7075  pth.K.h.N....epu
-00001430: 625f 746f 6364 7570 9488 68d5 4e87 948c  b_tocdup..h.N...
-00001440: 0d65 7075 625f 746f 6373 636f 7065 946a  .epub_tocscope.j
-00001450: 0401 0000 68d5 4e87 948c 0f65 7075 625f  ....h.N....epub_
-00001460: 6669 785f 696d 6167 6573 9489 68d5 4e87  fix_images..h.N.
-00001470: 948c 1465 7075 625f 6d61 785f 696d 6167  ...epub_max_imag
-00001480: 655f 7769 6474 6894 4b00 68d5 4e87 948c  e_width.K.h.N...
-00001490: 0e65 7075 625f 7368 6f77 5f75 726c 7394  .epub_show_urls.
-000014a0: 8c06 696e 6c69 6e65 946a 5101 0000 4e87  ..inline.jQ...N.
-000014b0: 948c 0e65 7075 625f 7573 655f 696e 6465  ...epub_use_inde
-000014c0: 7894 886a 5101 0000 4e87 948c 1065 7075  x..jQ...N....epu
-000014d0: 625f 6465 7363 7269 7074 696f 6e94 6a64  b_description.jd
-000014e0: 0100 006a 5101 0000 4e87 948c 1065 7075  ...jQ...N....epu
-000014f0: 625f 636f 6e74 7269 6275 746f 7294 6a64  b_contributor.jd
-00001500: 0100 006a 5101 0000 4e87 948c 1165 7075  ...jQ...N....epu
-00001510: 625f 7772 6974 696e 675f 6d6f 6465 948c  b_writing_mode..
-00001520: 0a68 6f72 697a 6f6e 7461 6c94 6a51 0100  .horizontal.jQ..
-00001530: 004e 8794 6814 6815 68d9 4e87 948c 0f68  .N..h.h.h.N....h
-00001540: 746d 6c5f 7468 656d 655f 7061 7468 945d  tml_theme_path.]
-00001550: 9468 d94e 8794 6816 6817 68d9 4e87 9468  .h.N..h.h.h.N..h
-00001560: 3768 3868 d94e 8794 8c10 6874 6d6c 5f73  7h8h.N....html_s
-00001570: 686f 7274 5f74 6974 6c65 9468 3868 d94e  hort_title.h8h.N
-00001580: 8794 8c0a 6874 6d6c 5f73 7479 6c65 944e  ....html_style.N
-00001590: 68d9 4e87 9468 3d4e 68d9 4e87 9468 4668  h.N..h=Nh.N..hFh
-000015a0: 1f68 d94e 8794 6880 6881 68d9 4e87 9468  .h.N..h.h.h.N..h
-000015b0: 8268 8368 d94e 8794 8c10 6874 6d6c 5f73  .h.h.N....html_s
-000015c0: 7461 7469 635f 7061 7468 945d 9428 8c62  tatic_path.].(.b
-000015d0: 2f68 6f6d 652f 7661 7275 6e6b 6170 6f6f  /home/varunkapoo
-000015e0: 722f 616e 6163 6f6e 6461 332f 656e 7673  r/anaconda3/envs
-000015f0: 2f6e 6170 6172 6965 6e76 2f6c 6962 2f70  /naparienv/lib/p
-00001600: 7974 686f 6e33 2e39 2f73 6974 652d 7061  ython3.9/site-pa
-00001610: 636b 6167 6573 2f73 7068 696e 785f 746f  ckages/sphinx_to
-00001620: 6767 6c65 6275 7474 6f6e 2f5f 7374 6174  gglebutton/_stat
-00001630: 6963 948c 602f 686f 6d65 2f76 6172 756e  ic..`/home/varun
-00001640: 6b61 706f 6f72 2f61 6e61 636f 6e64 6133  kapoor/anaconda3
-00001650: 2f65 6e76 732f 6e61 7061 7269 656e 762f  /envs/naparienv/
-00001660: 6c69 622f 7079 7468 6f6e 332e 392f 7369  lib/python3.9/si
-00001670: 7465 2d70 6163 6b61 6765 732f 7370 6869  te-packages/sphi
-00001680: 6e78 5f63 6f70 7962 7574 746f 6e2f 5f73  nx_copybutton/_s
-00001690: 7461 7469 6394 8c5b 2f68 6f6d 652f 7661  tatic..[/home/va
-000016a0: 7275 6e6b 6170 6f6f 722f 616e 6163 6f6e  runkapoor/anacon
-000016b0: 6461 332f 656e 7673 2f6e 6170 6172 6965  da3/envs/naparie
-000016c0: 6e76 2f6c 6962 2f70 7974 686f 6e33 2e39  nv/lib/python3.9
-000016d0: 2f73 6974 652d 7061 636b 6167 6573 2f73  /site-packages/s
-000016e0: 7068 696e 785f 7468 6562 652f 5f73 7461  phinx_thebe/_sta
-000016f0: 7469 6394 8c5e 2f68 6f6d 652f 7661 7275  tic..^/home/varu
-00001700: 6e6b 6170 6f6f 722f 616e 6163 6f6e 6461  nkapoor/anaconda
-00001710: 332f 656e 7673 2f6e 6170 6172 6965 6e76  3/envs/naparienv
-00001720: 2f6c 6962 2f70 7974 686f 6e33 2e39 2f73  /lib/python3.9/s
-00001730: 6974 652d 7061 636b 6167 6573 2f73 7068  ite-packages/sph
-00001740: 696e 785f 636f 6d6d 656e 7473 2f5f 7374  inx_comments/_st
-00001750: 6174 6963 948c 682f 6d6e 742f 632f 5573  atic..h/mnt/c/Us
-00001760: 6572 732f 7261 6e64 6f2f 446f 776e 6c6f  ers/rando/Downlo
-00001770: 6164 732f 5079 7468 6f6e 5f57 6f72 6b73  ads/Python_Works
-00001780: 7061 6365 2f76 6f6c 6c73 6567 2d6e 6170  pace/vollseg-nap
-00001790: 6172 692d 7472 6163 6b6d 6174 652f 5f62  ari-trackmate/_b
-000017a0: 7569 6c64 2f68 746d 6c2f 5f73 7068 696e  uild/html/_sphin
-000017b0: 785f 6465 7369 676e 5f73 7461 7469 6394  x_design_static.
-000017c0: 6568 d94e 8794 8c0f 6874 6d6c 5f65 7874  eh.N....html_ext
-000017d0: 7261 5f70 6174 6894 5d94 68d9 4e87 948c  ra_path.].h.N...
-000017e0: 1568 746d 6c5f 6c61 7374 5f75 7064 6174  .html_last_updat
-000017f0: 6564 5f66 6d74 944e 68d9 4e87 948c 0d68  ed_fmt.Nh.N....h
-00001800: 746d 6c5f 7369 6465 6261 7273 947d 9468  tml_sidebars.}.h
-00001810: d94e 8794 8c15 6874 6d6c 5f61 6464 6974  .N....html_addit
-00001820: 696f 6e61 6c5f 7061 6765 7394 7d94 68d9  ional_pages.}.h.
-00001830: 4e87 948c 1368 746d 6c5f 646f 6d61 696e  N....html_domain
-00001840: 5f69 6e64 6963 6573 9488 68d9 4e87 948c  _indices..h.N...
-00001850: 1368 746d 6c5f 6164 645f 7065 726d 616c  .html_add_permal
-00001860: 696e 6b73 948c 1473 7068 696e 782e 6275  inks...sphinx.bu
-00001870: 696c 6465 7273 2e68 746d 6c94 8c13 5f73  ilders.html..._s
-00001880: 7461 626c 655f 7265 7072 5f6f 626a 6563  table_repr_objec
-00001890: 7494 9394 2981 9468 d94e 8794 8c0f 6874  t...)..h.N....ht
-000018a0: 6d6c 5f70 6572 6d61 6c69 6e6b 7394 8868  ml_permalinks..h
-000018b0: d94e 8794 68ca 68cb 68d9 4e87 948c 0e68  .N..h.h.h.N....h
-000018c0: 746d 6c5f 7573 655f 696e 6465 7894 8868  tml_use_index..h
-000018d0: d94e 8794 8c10 6874 6d6c 5f73 706c 6974  .N....html_split
-000018e0: 5f69 6e64 6578 9489 68d9 4e87 948c 1068  _index..h.N....h
-000018f0: 746d 6c5f 636f 7079 5f73 6f75 7263 6594  tml_copy_source.
-00001900: 8868 d94e 8794 8c14 6874 6d6c 5f73 686f  .h.N....html_sho
-00001910: 775f 736f 7572 6365 6c69 6e6b 9488 68d9  w_sourcelink..h.
-00001920: 4e87 9468 3268 1f68 d94e 8794 8c13 6874  N..h2h.h.N....ht
-00001930: 6d6c 5f75 7365 5f6f 7065 6e73 6561 7263  ml_use_opensearc
-00001940: 6894 681f 68d9 4e87 948c 1068 746d 6c5f  h.h.h.N....html_
-00001950: 6669 6c65 5f73 7566 6669 7894 4e68 d94e  file_suffix.Nh.N
-00001960: 8794 8c10 6874 6d6c 5f6c 696e 6b5f 7375  ....html_link_su
-00001970: 6666 6978 944e 68d9 4e87 948c 1368 746d  ffix.Nh.N....htm
-00001980: 6c5f 7368 6f77 5f63 6f70 7972 6967 6874  l_show_copyright
-00001990: 9488 68d9 4e87 948c 1868 746d 6c5f 7368  ..h.N....html_sh
-000019a0: 6f77 5f73 6561 7263 685f 7375 6d6d 6172  ow_search_summar
-000019b0: 7994 8868 d94e 8794 8c10 6874 6d6c 5f73  y..h.N....html_s
-000019c0: 686f 775f 7370 6869 6e78 9488 68d9 4e87  how_sphinx..h.N.
-000019d0: 948c 0c68 746d 6c5f 636f 6e74 6578 7494  ...html_context.
-000019e0: 7d94 288c 1663 6f70 7962 7574 746f 6e5f  }.(..copybutton_
-000019f0: 7072 6f6d 7074 5f74 6578 7494 681f 8c1b  prompt_text.h...
-00001a00: 636f 7079 6275 7474 6f6e 5f70 726f 6d70  copybutton_promp
-00001a10: 745f 6973 5f72 6567 6578 7094 898c 2163  t_is_regexp...!c
-00001a20: 6f70 7962 7574 746f 6e5f 6f6e 6c79 5f63  opybutton_only_c
-00001a30: 6f70 795f 7072 6f6d 7074 5f6c 696e 6573  opy_prompt_lines
-00001a40: 9488 8c19 636f 7079 6275 7474 6f6e 5f72  ....copybutton_r
-00001a50: 656d 6f76 655f 7072 6f6d 7074 7394 888c  emove_prompts...
-00001a60: 1b63 6f70 7962 7574 746f 6e5f 636f 7079  .copybutton_copy
-00001a70: 5f65 6d70 7479 5f6c 696e 6573 9488 8c26  _empty_lines...&
-00001a80: 636f 7079 6275 7474 6f6e 5f6c 696e 655f  copybutton_line_
-00001a90: 636f 6e74 696e 7561 7469 6f6e 5f63 6861  continuation_cha
-00001aa0: 7261 6374 6572 9468 1f8c 1d63 6f70 7962  racter.h...copyb
-00001ab0: 7574 746f 6e5f 6865 7265 5f64 6f63 5f64  utton_here_doc_d
-00001ac0: 656c 696d 6974 6572 9468 1f8c 1463 6f70  elimiter.h...cop
-00001ad0: 7962 7574 746f 6e5f 696d 6167 655f 7376  ybutton_image_sv
-00001ae0: 6794 681f 8c13 636f 7079 6275 7474 6f6e  g.h...copybutton
-00001af0: 5f73 656c 6563 746f 7294 8c11 6469 762e  _selector...div.
-00001b00: 6869 6768 6c69 6768 7420 7072 6594 8c16  highlight pre...
-00001b10: 636f 7079 6275 7474 6f6e 5f66 6f72 6d61  copybutton_forma
-00001b20: 745f 6675 6e63 9458 7c0a 0000 6675 6e63  t_func.X|...func
-00001b30: 7469 6f6e 2065 7363 6170 6552 6567 4578  tion escapeRegEx
-00001b40: 7028 7374 7269 6e67 2920 7b0a 2020 2020  p(string) {.    
-00001b50: 7265 7475 726e 2073 7472 696e 672e 7265  return string.re
-00001b60: 706c 6163 6528 2f5b 2e2a 2b3f 5e24 7b7d  place(/[.*+?^${}
-00001b70: 2829 7c5b 5c5d 5c5c 5d2f 672c 2027 5c5c  ()|[\]\\]/g, '\\
-00001b80: 2426 2729 3b20 2f2f 2024 2620 6d65 616e  $&'); // $& mean
-00001b90: 7320 7468 6520 7768 6f6c 6520 6d61 7463  s the whole matc
-00001ba0: 6865 6420 7374 7269 6e67 0a7d 0a0a 2f2a  hed string.}../*
-00001bb0: 2a0a 202a 2052 656d 6f76 6573 2065 7863  *. * Removes exc
-00001bc0: 6c75 6465 6420 7465 7874 2066 726f 6d20  luded text from 
-00001bd0: 6120 4e6f 6465 2e0a 202a 0a20 2a20 4070  a Node.. *. * @p
-00001be0: 6172 616d 207b 4e6f 6465 7d20 7461 7267  aram {Node} targ
-00001bf0: 6574 204e 6f64 6520 746f 2066 696c 7465  et Node to filte
-00001c00: 722e 0a20 2a20 4070 6172 616d 207b 7374  r.. * @param {st
-00001c10: 7269 6e67 7d20 6578 636c 7564 6520 4353  ring} exclude CS
-00001c20: 5320 7365 6c65 6374 6f72 206f 6620 6e6f  S selector of no
-00001c30: 6465 7320 746f 2065 7863 6c75 6465 2e0a  des to exclude..
-00001c40: 202a 2040 7265 7475 726e 7320 7b44 4f4d   * @returns {DOM
-00001c50: 5374 7269 6e67 7d20 5465 7874 2066 726f  String} Text fro
-00001c60: 6d20 6074 6172 6765 7460 2077 6974 6820  m `target` with 
-00001c70: 7465 7874 2072 656d 6f76 6564 2e0a 202a  text removed.. *
-00001c80: 2f0a 6675 6e63 7469 6f6e 2066 696c 7465  /.function filte
-00001c90: 7254 6578 7428 7461 7267 6574 2c20 6578  rText(target, ex
-00001ca0: 636c 7564 6529 207b 0a20 2020 2063 6f6e  clude) {.    con
-00001cb0: 7374 2063 6c6f 6e65 203d 2074 6172 6765  st clone = targe
-00001cc0: 742e 636c 6f6e 654e 6f64 6528 7472 7565  t.cloneNode(true
-00001cd0: 293b 2020 2f2f 2063 6c6f 6e65 2061 7320  );  // clone as 
-00001ce0: 746f 206e 6f74 206d 6f64 6966 7920 7468  to not modify th
-00001cf0: 6520 6c69 7665 2044 4f4d 0a20 2020 2069  e live DOM.    i
-00001d00: 6620 2865 7863 6c75 6465 2920 7b0a 2020  f (exclude) {.  
-00001d10: 2020 2020 2020 2f2f 2072 656d 6f76 6520        // remove 
-00001d20: 6578 636c 7564 6564 206e 6f64 6573 0a20  excluded nodes. 
-00001d30: 2020 2020 2020 2063 6c6f 6e65 2e71 7565         clone.que
-00001d40: 7279 5365 6c65 6374 6f72 416c 6c28 6578  rySelectorAll(ex
-00001d50: 636c 7564 6529 2e66 6f72 4561 6368 286e  clude).forEach(n
-00001d60: 6f64 6520 3d3e 206e 6f64 652e 7265 6d6f  ode => node.remo
-00001d70: 7665 2829 293b 0a20 2020 207d 0a20 2020  ve());.    }.   
-00001d80: 2072 6574 7572 6e20 636c 6f6e 652e 696e   return clone.in
-00001d90: 6e65 7254 6578 743b 0a7d 0a0a 2f2f 2043  nerText;.}..// C
-00001da0: 616c 6c62 6163 6b20 7768 656e 2061 2063  allback when a c
-00001db0: 6f70 7920 6275 7474 6f6e 2069 7320 636c  opy button is cl
-00001dc0: 6963 6b65 642e 2057 696c 6c20 6265 2070  icked. Will be p
-00001dd0: 6173 7365 6420 7468 6520 6e6f 6465 2074  assed the node t
-00001de0: 6861 7420 7761 7320 636c 6963 6b65 640a  hat was clicked.
-00001df0: 2f2f 2073 686f 756c 6420 7468 656e 2067  // should then g
-00001e00: 7261 6220 7468 6520 7465 7874 2061 6e64  rab the text and
-00001e10: 2072 6570 6c61 6365 2070 6965 6365 7320   replace pieces 
-00001e20: 6f66 2074 6578 7420 7468 6174 2073 686f  of text that sho
-00001e30: 756c 646e 2774 2062 6520 7573 6564 2069  uldn't be used i
-00001e40: 6e20 6f75 7470 7574 0a66 756e 6374 696f  n output.functio
-00001e50: 6e20 666f 726d 6174 436f 7079 5465 7874  n formatCopyText
-00001e60: 2874 6578 7443 6f6e 7465 6e74 2c20 636f  (textContent, co
-00001e70: 7079 6275 7474 6f6e 5072 6f6d 7074 5465  pybuttonPromptTe
-00001e80: 7874 2c20 6973 5265 6765 7870 203d 2066  xt, isRegexp = f
-00001e90: 616c 7365 2c20 6f6e 6c79 436f 7079 5072  alse, onlyCopyPr
-00001ea0: 6f6d 7074 4c69 6e65 7320 3d20 7472 7565  omptLines = true
-00001eb0: 2c20 7265 6d6f 7665 5072 6f6d 7074 7320  , removePrompts 
-00001ec0: 3d20 7472 7565 2c20 636f 7079 456d 7074  = true, copyEmpt
-00001ed0: 794c 696e 6573 203d 2074 7275 652c 206c  yLines = true, l
-00001ee0: 696e 6543 6f6e 7469 6e75 6174 696f 6e43  ineContinuationC
-00001ef0: 6861 7220 3d20 2222 2c20 6865 7265 446f  har = "", hereDo
-00001f00: 6344 656c 696d 203d 2022 2229 207b 0a20  cDelim = "") {. 
-00001f10: 2020 2076 6172 2072 6567 6578 703b 0a20     var regexp;. 
-00001f20: 2020 2076 6172 206d 6174 6368 3b0a 0a20     var match;.. 
-00001f30: 2020 202f 2f20 446f 2077 6520 6368 6563     // Do we chec
-00001f40: 6b20 666f 7220 6c69 6e65 2063 6f6e 7469  k for line conti
-00001f50: 6e75 6174 696f 6e20 6368 6172 6163 7465  nuation characte
-00001f60: 7273 2061 6e64 2022 4845 5245 2d64 6f63  rs and "HERE-doc
-00001f70: 756d 656e 7473 223f 0a20 2020 2076 6172  uments"?.    var
-00001f80: 2075 7365 4c69 6e65 436f 6e74 203d 2021   useLineCont = !
-00001f90: 216c 696e 6543 6f6e 7469 6e75 6174 696f  !lineContinuatio
-00001fa0: 6e43 6861 720a 2020 2020 7661 7220 7573  nChar.    var us
-00001fb0: 6548 6572 6544 6f63 203d 2021 2168 6572  eHereDoc = !!her
-00001fc0: 6544 6f63 4465 6c69 6d0a 0a20 2020 202f  eDocDelim..    /
-00001fd0: 2f20 6372 6561 7465 2072 6567 6578 7020  / create regexp 
-00001fe0: 746f 2063 6170 7475 7265 2070 726f 6d70  to capture promp
-00001ff0: 7420 616e 6420 7265 6d61 696e 696e 6720  t and remaining 
-00002000: 6c69 6e65 0a20 2020 2069 6620 2869 7352  line.    if (isR
-00002010: 6567 6578 7029 207b 0a20 2020 2020 2020  egexp) {.       
-00002020: 2072 6567 6578 7020 3d20 6e65 7720 5265   regexp = new Re
-00002030: 6745 7870 2827 5e28 2720 2b20 636f 7079  gExp('^(' + copy
-00002040: 6275 7474 6f6e 5072 6f6d 7074 5465 7874  buttonPromptText
-00002050: 202b 2027 2928 2e2a 2927 290a 2020 2020   + ')(.*)').    
-00002060: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
-00002070: 2072 6567 6578 7020 3d20 6e65 7720 5265   regexp = new Re
-00002080: 6745 7870 2827 5e28 2720 2b20 6573 6361  gExp('^(' + esca
-00002090: 7065 5265 6745 7870 2863 6f70 7962 7574  peRegExp(copybut
-000020a0: 746f 6e50 726f 6d70 7454 6578 7429 202b  tonPromptText) +
-000020b0: 2027 2928 2e2a 2927 290a 2020 2020 7d0a   ')(.*)').    }.
-000020c0: 0a20 2020 2063 6f6e 7374 206f 7574 7075  .    const outpu
-000020d0: 744c 696e 6573 203d 205b 5d3b 0a20 2020  tLines = [];.   
-000020e0: 2076 6172 2070 726f 6d70 7446 6f75 6e64   var promptFound
-000020f0: 203d 2066 616c 7365 3b0a 2020 2020 7661   = false;.    va
-00002100: 7220 676f 744c 696e 6543 6f6e 7420 3d20  r gotLineCont = 
-00002110: 6661 6c73 653b 0a20 2020 2076 6172 2067  false;.    var g
-00002120: 6f74 4865 7265 446f 6320 3d20 6661 6c73  otHereDoc = fals
-00002130: 653b 0a20 2020 2063 6f6e 7374 206c 696e  e;.    const lin
-00002140: 6547 6f74 5072 6f6d 7074 203d 205b 5d3b  eGotPrompt = [];
-00002150: 0a20 2020 2066 6f72 2028 636f 6e73 7420  .    for (const 
-00002160: 6c69 6e65 206f 6620 7465 7874 436f 6e74  line of textCont
-00002170: 656e 742e 7370 6c69 7428 275c 6e27 2929  ent.split('\n'))
-00002180: 207b 0a20 2020 2020 2020 206d 6174 6368   {.        match
-00002190: 203d 206c 696e 652e 6d61 7463 6828 7265   = line.match(re
-000021a0: 6765 7870 290a 2020 2020 2020 2020 6966  gexp).        if
-000021b0: 2028 6d61 7463 6820 7c7c 2067 6f74 4c69   (match || gotLi
-000021c0: 6e65 436f 6e74 207c 7c20 676f 7448 6572  neCont || gotHer
-000021d0: 6544 6f63 2920 7b0a 2020 2020 2020 2020  eDoc) {.        
-000021e0: 2020 2020 7072 6f6d 7074 466f 756e 6420      promptFound 
-000021f0: 3d20 7265 6765 7870 2e74 6573 7428 6c69  = regexp.test(li
-00002200: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-00002210: 6c69 6e65 476f 7450 726f 6d70 742e 7075  lineGotPrompt.pu
-00002220: 7368 2870 726f 6d70 7446 6f75 6e64 290a  sh(promptFound).
-00002230: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00002240: 7265 6d6f 7665 5072 6f6d 7074 7320 2626  removePrompts &&
-00002250: 2070 726f 6d70 7446 6f75 6e64 2920 7b0a   promptFound) {.
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 6f75 7470 7574 4c69 6e65 732e 7075 7368  outputLines.push
-00002280: 286d 6174 6368 5b32 5d29 0a20 2020 2020  (match[2]).     
-00002290: 2020 2020 2020 207d 2065 6c73 6520 7b0a         } else {.
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022b0: 6f75 7470 7574 4c69 6e65 732e 7075 7368  outputLines.push
-000022c0: 286c 696e 6529 0a20 2020 2020 2020 2020  (line).         
-000022d0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-000022e0: 2067 6f74 4c69 6e65 436f 6e74 203d 206c   gotLineCont = l
-000022f0: 696e 652e 656e 6473 5769 7468 286c 696e  ine.endsWith(lin
-00002300: 6543 6f6e 7469 6e75 6174 696f 6e43 6861  eContinuationCha
-00002310: 7229 2026 2075 7365 4c69 6e65 436f 6e74  r) & useLineCont
-00002320: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002330: 286c 696e 652e 696e 636c 7564 6573 2868  (line.includes(h
-00002340: 6572 6544 6f63 4465 6c69 6d29 2026 2075  ereDocDelim) & u
-00002350: 7365 4865 7265 446f 6329 0a20 2020 2020  seHereDoc).     
-00002360: 2020 2020 2020 2020 2020 2067 6f74 4865             gotHe
-00002370: 7265 446f 6320 3d20 2167 6f74 4865 7265  reDoc = !gotHere
-00002380: 446f 630a 2020 2020 2020 2020 7d20 656c  Doc.        } el
-00002390: 7365 2069 6620 2821 6f6e 6c79 436f 7079  se if (!onlyCopy
-000023a0: 5072 6f6d 7074 4c69 6e65 7329 207b 0a20  PromptLines) {. 
-000023b0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-000023c0: 744c 696e 6573 2e70 7573 6828 6c69 6e65  tLines.push(line
-000023d0: 290a 2020 2020 2020 2020 7d20 656c 7365  ).        } else
-000023e0: 2069 6620 2863 6f70 7945 6d70 7479 4c69   if (copyEmptyLi
-000023f0: 6e65 7320 2626 206c 696e 652e 7472 696d  nes && line.trim
-00002400: 2829 203d 3d3d 2027 2729 207b 0a20 2020  () === '') {.   
-00002410: 2020 2020 2020 2020 206f 7574 7075 744c           outputL
-00002420: 696e 6573 2e70 7573 6828 6c69 6e65 290a  ines.push(line).
-00002430: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
-00002440: 0a20 2020 202f 2f20 4966 206e 6f20 6c69  .    // If no li
-00002450: 6e65 7320 7769 7468 2074 6865 2070 726f  nes with the pro
-00002460: 6d70 7420 7765 7265 2066 6f75 6e64 2074  mpt were found t
-00002470: 6865 6e20 6a75 7374 2075 7365 206f 7269  hen just use ori
-00002480: 6769 6e61 6c20 6c69 6e65 730a 2020 2020  ginal lines.    
-00002490: 6966 2028 6c69 6e65 476f 7450 726f 6d70  if (lineGotPromp
-000024a0: 742e 736f 6d65 2876 203d 3e20 7620 3d3d  t.some(v => v ==
-000024b0: 3d20 7472 7565 2929 207b 0a20 2020 2020  = true)) {.     
-000024c0: 2020 2074 6578 7443 6f6e 7465 6e74 203d     textContent =
-000024d0: 206f 7574 7075 744c 696e 6573 2e6a 6f69   outputLines.joi
-000024e0: 6e28 275c 6e27 293b 0a20 2020 207d 0a0a  n('\n');.    }..
-000024f0: 2020 2020 2f2f 2052 656d 6f76 6520 6120      // Remove a 
-00002500: 7472 6169 6c69 6e67 206e 6577 6c69 6e65  trailing newline
-00002510: 2074 6f20 6176 6f69 6420 6175 746f 2d72   to avoid auto-r
-00002520: 756e 6e69 6e67 2077 6865 6e20 7061 7374  unning when past
-00002530: 696e 670a 2020 2020 6966 2028 7465 7874  ing.    if (text
-00002540: 436f 6e74 656e 742e 656e 6473 5769 7468  Content.endsWith
-00002550: 2822 5c6e 2229 2920 7b0a 2020 2020 2020  ("\n")) {.      
-00002560: 2020 7465 7874 436f 6e74 656e 7420 3d20    textContent = 
-00002570: 7465 7874 436f 6e74 656e 742e 736c 6963  textContent.slic
-00002580: 6528 302c 202d 3129 0a20 2020 207d 0a20  e(0, -1).    }. 
-00002590: 2020 2072 6574 7572 6e20 7465 7874 436f     return textCo
-000025a0: 6e74 656e 740a 7d0a 948c 1263 6f70 7962  ntent.}....copyb
-000025b0: 7574 746f 6e5f 6578 636c 7564 6594 8c08  utton_exclude...
-000025c0: 2e6c 696e 656e 6f73 948c 0b67 6974 6875  .linenos...githu
-000025d0: 625f 7573 6572 948c 104b 6170 6f6f 726c  b_user...Kapoorl
-000025e0: 6162 732d 4341 5045 4494 8c0b 6769 7468  abs-CAPED...gith
-000025f0: 7562 5f72 6570 6f94 8c18 766f 6c6c 7365  ub_repo...vollse
-00002600: 672d 6e61 7061 7269 2d74 7261 636b 6d61  g-napari-trackma
-00002610: 7465 948c 0e67 6974 6875 625f 7665 7273  te...github_vers
-00002620: 696f 6e94 6828 8c0a 6769 7468 7562 5f75  ion.h(..github_u
-00002630: 726c 948c 1268 7474 7073 3a2f 2f67 6974  rl...https://git
-00002640: 6875 622e 636f 6d94 8c08 646f 635f 7061  hub.com...doc_pa
-00002650: 7468 9468 2475 68d9 4e87 948c 1468 746d  th.h$uh.N....htm
-00002660: 6c5f 6f75 7470 7574 5f65 6e63 6f64 696e  l_output_encodin
-00002670: 6794 8c05 7574 662d 3894 68d9 4e87 948c  g...utf-8.h.N...
-00002680: 1268 746d 6c5f 636f 6d70 6163 745f 6c69  .html_compact_li
-00002690: 7374 7394 8868 d94e 8794 8c15 6874 6d6c  sts..h.N....html
-000026a0: 5f73 6563 6e75 6d62 6572 5f73 7566 6669  _secnumber_suffi
-000026b0: 7894 8c02 2e20 9468 d94e 8794 8c14 6874  x.... .h.N....ht
-000026c0: 6d6c 5f73 6561 7263 685f 6c61 6e67 7561  ml_search_langua
-000026d0: 6765 944e 68d9 4e87 948c 1368 746d 6c5f  ge.Nh.N....html_
-000026e0: 7365 6172 6368 5f6f 7074 696f 6e73 947d  search_options.}
-000026f0: 9468 d94e 8794 8c12 6874 6d6c 5f73 6561  .h.N....html_sea
-00002700: 7263 685f 7363 6f72 6572 9468 1f4e 4e87  rch_scorer.h.NN.
-00002710: 948c 1668 746d 6c5f 7363 616c 6564 5f69  ...html_scaled_i
-00002720: 6d61 6765 5f6c 696e 6b94 8868 d94e 8794  mage_link..h.N..
-00002730: 6847 681f 68d9 4e87 948c 1c68 746d 6c5f  hGh.h.N....html_
-00002740: 636f 6465 626c 6f63 6b5f 6c69 6e65 6e6f  codeblock_lineno
-00002750: 735f 7374 796c 6594 6a83 0100 0068 d94e  s_style.j....h.N
-00002760: 8794 8c12 6874 6d6c 5f6d 6174 685f 7265  ....html_math_re
-00002770: 6e64 6572 6572 944e 68d5 4e87 948c 0c68  nderer.Nh.N....h
-00002780: 746d 6c34 5f77 7269 7465 7294 8968 d94e  tml4_writer..h.N
-00002790: 8794 8c0c 6d61 7468 6a61 785f 7061 7468  ....mathjax_path
-000027a0: 948c 3b68 7474 7073 3a2f 2f63 646e 2e6a  ..;https://cdn.j
-000027b0: 7364 656c 6976 722e 6e65 742f 6e70 6d2f  sdelivr.net/npm/
-000027c0: 6d61 7468 6a61 7840 332f 6573 352f 7465  mathjax@3/es5/te
-000027d0: 782d 6d6d 6c2d 6368 746d 6c2e 6a73 9468  x-mml-chtml.js.h
-000027e0: d94e 8794 8c0f 6d61 7468 6a61 785f 6f70  .N....mathjax_op
-000027f0: 7469 6f6e 7394 7d94 68d9 4e87 948c 0e6d  tions.}.h.N....m
-00002800: 6174 686a 6178 5f69 6e6c 696e 6594 5d94  athjax_inline.].
-00002810: 288c 025c 2894 8c02 5c29 9465 68d9 4e87  (..\(...\).eh.N.
-00002820: 948c 0f6d 6174 686a 6178 5f64 6973 706c  ...mathjax_displ
-00002830: 6179 945d 9428 8c02 5c5b 948c 025c 5d94  ay.].(..\[...\].
-00002840: 6568 d94e 8794 8c0e 6d61 7468 6a61 785f  eh.N....mathjax_
-00002850: 636f 6e66 6967 944e 68d9 4e87 948c 0f6d  config.Nh.N....m
-00002860: 6174 686a 6178 325f 636f 6e66 6967 944e  athjax2_config.N
-00002870: 68d9 4e87 9468 c468 c568 d94e 8794 8c0f  h.N..h.h.h.N....
-00002880: 6765 7474 6578 745f 636f 6d70 6163 7494  gettext_compact.
-00002890: 8868 ee4e 8794 8c10 6765 7474 6578 745f  .h.N....gettext_
-000028a0: 6c6f 6361 7469 6f6e 9488 68ee 4e87 948c  location..h.N...
-000028b0: 0c67 6574 7465 7874 5f75 7569 6494 8968  .gettext_uuid..h
-000028c0: ee4e 8794 8c12 6765 7474 6578 745f 6175  .N....gettext_au
-000028d0: 746f 5f62 7569 6c64 9488 68d5 4e87 948c  to_build..h.N...
-000028e0: 1a67 6574 7465 7874 5f61 6464 6974 696f  .gettext_additio
-000028f0: 6e61 6c5f 7461 7267 6574 7394 5d94 68d5  nal_targets.].h.
-00002900: 4e87 948c 1767 6574 7465 7874 5f6c 6173  N....gettext_las
-00002910: 745f 7472 616e 736c 6174 6f72 948c 1946  t_translator...F
-00002920: 554c 4c20 4e41 4d45 203c 454d 4149 4c40  ULL NAME <EMAIL@
-00002930: 4144 4452 4553 533e 9468 ee4e 8794 8c15  ADDRESS>.h.N....
-00002940: 6765 7474 6578 745f 6c61 6e67 7561 6765  gettext_language
-00002950: 5f74 6561 6d94 8c14 4c41 4e47 5541 4745  _team...LANGUAGE
-00002960: 203c 4c4c 406c 692e 6f72 673e 9468 ee4e   <LL@li.org>.h.N
-00002970: 8794 6863 6879 4e4e 8794 68cc 68cd 4e4e  ..hchyNN..h.h.NN
-00002980: 8794 8c0a 6c61 7465 785f 6c6f 676f 944e  ....latex_logo.N
-00002990: 4e4e 8794 8c10 6c61 7465 785f 6170 7065  NN....latex_appe
-000029a0: 6e64 6963 6573 945d 944e 4e87 948c 1b6c  ndices.].NN....l
-000029b0: 6174 6578 5f75 7365 5f6c 6174 6578 5f6d  atex_use_latex_m
-000029c0: 756c 7469 636f 6c75 6d6e 9489 4e4e 8794  ulticolumn..NN..
-000029d0: 8c0f 6c61 7465 785f 7573 655f 7869 6e64  ..latex_use_xind
-000029e0: 7994 884e 4e87 948c 196c 6174 6578 5f74  y..NN....latex_t
-000029f0: 6f70 6c65 7665 6c5f 7365 6374 696f 6e69  oplevel_sectioni
-00002a00: 6e67 944e 4e4e 8794 8c14 6c61 7465 785f  ng.NNN....latex_
-00002a10: 646f 6d61 696e 5f69 6e64 6963 6573 9488  domain_indices..
-00002a20: 4e4e 8794 8c0f 6c61 7465 785f 7368 6f77  NN....latex_show
-00002a30: 5f75 726c 7394 8c02 6e6f 944e 4e87 948c  _urls...no.NN...
-00002a40: 136c 6174 6578 5f73 686f 775f 7061 6765  .latex_show_page
-00002a50: 7265 6673 9489 4e4e 8794 8c0e 6c61 7465  refs..NN....late
-00002a60: 785f 656c 656d 656e 7473 947d 948c 0870  x_elements.}...p
-00002a70: 7265 616d 626c 6594 5898 0100 000a 2020  reamble.X.....  
-00002a80: 2020 2020 2020 2520 5374 6172 7420 6f66        % Start of
-00002a90: 2070 7265 616d 626c 6520 6465 6669 6e65   preamble define
-00002aa0: 6420 696e 2073 7068 696e 782d 6a75 7079  d in sphinx-jupy
-00002ab0: 7465 7262 6f6f 6b2d 6c61 7465 7820 250a  terbook-latex %.
-00002ac0: 2020 2020 2020 2020 205c 7573 6570 6163           \usepac
-00002ad0: 6b61 6765 5b4c 6174 696e 2c47 7265 656b  kage[Latin,Greek
-00002ae0: 5d7b 7563 6861 7263 6c61 7373 6573 7d0a  ]{ucharclasses}.
-00002af0: 2020 2020 2020 2020 5c75 7365 7061 636b          \usepack
-00002b00: 6167 657b 756e 6963 6f64 652d 6d61 7468  age{unicode-math
-00002b10: 7d0a 2020 2020 2020 2020 2520 6669 7869  }.        % fixi
-00002b20: 6e67 2074 6974 6c65 206f 6620 7468 6520  ng title of the 
-00002b30: 746f 630a 2020 2020 2020 2020 5c61 6464  toc.        \add
-00002b40: 746f 5c63 6170 7469 6f6e 7365 6e67 6c69  to\captionsengli
-00002b50: 7368 7b5c 7265 6e65 7763 6f6d 6d61 6e64  sh{\renewcommand
-00002b60: 7b5c 636f 6e74 656e 7473 6e61 6d65 7d7b  {\contentsname}{
-00002b70: 436f 6e74 656e 7473 7d7d 0a20 2020 2020  Contents}}.     
-00002b80: 2020 205c 6879 7065 7273 6574 7570 7b0a     \hypersetup{.
-00002b90: 2020 2020 2020 2020 2020 2020 7064 6665              pdfe
-00002ba0: 6e63 6f64 696e 673d 6175 746f 2c0a 2020  ncoding=auto,.  
-00002bb0: 2020 2020 2020 2020 2020 7073 6465 7874            psdext
-00002bc0: 7261 0a20 2020 2020 2020 207d 0a20 2020  ra.        }.   
-00002bd0: 2020 2020 2025 2045 6e64 206f 6620 7072       % End of pr
-00002be0: 6561 6d62 6c65 2064 6566 696e 6564 2069  eamble defined i
-00002bf0: 6e20 7370 6869 6e78 2d6a 7570 7974 6572  n sphinx-jupyter
-00002c00: 626f 6f6b 2d6c 6174 6578 2025 0a20 2020  book-latex %.   
-00002c10: 2020 2020 2094 734e 4e87 948c 166c 6174       .sNN....lat
-00002c20: 6578 5f61 6464 6974 696f 6e61 6c5f 6669  ex_additional_fi
-00002c30: 6c65 7394 5d94 4e4e 8794 687a 687b 4e4e  les.].NN..hzh{NN
-00002c40: 8794 8c13 6c61 7465 785f 7468 656d 655f  ....latex_theme_
-00002c50: 6f70 7469 6f6e 7394 7d94 4e4e 8794 8c10  options.}.NN....
-00002c60: 6c61 7465 785f 7468 656d 655f 7061 7468  latex_theme_path
-00002c70: 945d 944e 4e87 948c 0e6c 6174 6578 5f64  .].NN....latex_d
-00002c80: 6f63 636c 6173 7394 7d94 4e4e 8794 8c10  occlass.}.NN....
-00002c90: 6c69 6e6b 6368 6563 6b5f 6967 6e6f 7265  linkcheck_ignore
-00002ca0: 945d 944e 4e87 948c 1b6c 696e 6b63 6865  .].NN....linkche
-00002cb0: 636b 5f65 7863 6c75 6465 5f64 6f63 756d  ck_exclude_docum
-00002cc0: 656e 7473 945d 944e 4e87 948c 1b6c 696e  ents.].NN....lin
-00002cd0: 6b63 6865 636b 5f61 6c6c 6f77 6564 5f72  kcheck_allowed_r
-00002ce0: 6564 6972 6563 7473 947d 944e 4e87 948c  edirects.}.NN...
-00002cf0: 0e6c 696e 6b63 6865 636b 5f61 7574 6894  .linkcheck_auth.
-00002d00: 5d94 4e4e 8794 8c19 6c69 6e6b 6368 6563  ].NN....linkchec
-00002d10: 6b5f 7265 7175 6573 745f 6865 6164 6572  k_request_header
-00002d20: 7394 7d94 4e4e 8794 8c11 6c69 6e6b 6368  s.}.NN....linkch
-00002d30: 6563 6b5f 7265 7472 6965 7394 4b01 4e4e  eck_retries.K.NN
-00002d40: 8794 8c11 6c69 6e6b 6368 6563 6b5f 7469  ....linkcheck_ti
-00002d50: 6d65 6f75 7494 4e4e 4e87 948c 116c 696e  meout.NNN....lin
-00002d60: 6b63 6865 636b 5f77 6f72 6b65 7273 944b  kcheck_workers.K
-00002d70: 054e 4e87 948c 116c 696e 6b63 6865 636b  .NN....linkcheck
-00002d80: 5f61 6e63 686f 7273 9488 4e4e 8794 8c18  _anchors..NN....
-00002d90: 6c69 6e6b 6368 6563 6b5f 616e 6368 6f72  linkcheck_anchor
-00002da0: 735f 6967 6e6f 7265 945d 948c 025e 2194  s_ignore.]...^!.
-00002db0: 614e 4e87 948c 1c6c 696e 6b63 6865 636b  aNN....linkcheck
-00002dc0: 5f72 6174 655f 6c69 6d69 745f 7469 6d65  _rate_limit_time
-00002dd0: 6f75 7494 4740 72c0 0000 0000 004e 4e87  out.G@r......NN.
-00002de0: 948c 096d 616e 5f70 6167 6573 945d 9428  ...man_pages.].(
-00002df0: 68a0 8c06 7079 7468 6f6e 948c 0750 7974  h...python...Pyt
-00002e00: 686f 6e20 945d 9468 3a61 4b01 7494 614e  hon .].h:aK.t.aN
-00002e10: 4e87 948c 0d6d 616e 5f73 686f 775f 7572  N....man_show_ur
-00002e20: 6c73 9489 4e4e 8794 8c1a 6d61 6e5f 6d61  ls..NN....man_ma
-00002e30: 6b65 5f73 6563 7469 6f6e 5f64 6972 6563  ke_section_direc
-00002e40: 746f 7279 9489 4e4e 8794 8c13 7369 6e67  tory..NN....sing
-00002e50: 6c65 6874 6d6c 5f73 6964 6562 6172 7394  lehtml_sidebars.
-00002e60: 6aaa 0100 0068 d94e 8794 8c11 7465 7869  j....h.N....texi
-00002e70: 6e66 6f5f 646f 6375 6d65 6e74 7394 5d94  nfo_documents.].
-00002e80: 2868 a08c 0670 7974 686f 6e94 68d4 683a  (h...python.h.h:
-00002e90: 6a78 0200 008c 1f4f 6e65 206c 696e 6520  jx.....One line 
-00002ea0: 6465 7363 7269 7074 696f 6e20 6f66 2070  description of p
-00002eb0: 726f 6a65 6374 948c 0d4d 6973 6365 6c6c  roject...Miscell
-00002ec0: 616e 656f 7573 9474 9461 4e4e 8794 8c12  aneous.t.aNN....
-00002ed0: 7465 7869 6e66 6f5f 6170 7065 6e64 6963  texinfo_appendic
-00002ee0: 6573 945d 944e 4e87 948c 1074 6578 696e  es.].NN....texin
-00002ef0: 666f 5f65 6c65 6d65 6e74 7394 7d94 4e4e  fo_elements.}.NN
-00002f00: 8794 8c16 7465 7869 6e66 6f5f 646f 6d61  ....texinfo_doma
-00002f10: 696e 5f69 6e64 6963 6573 9488 4e4e 8794  in_indices..NN..
-00002f20: 8c11 7465 7869 6e66 6f5f 7368 6f77 5f75  ..texinfo_show_u
-00002f30: 726c 7394 8c08 666f 6f74 6e6f 7465 944e  rls...footnote.N
-00002f40: 4e87 948c 1574 6578 696e 666f 5f6e 6f5f  N....texinfo_no_
-00002f50: 6465 7461 696c 6d65 6e75 9489 4e4e 8794  detailmenu..NN..
-00002f60: 8c18 7465 7869 6e66 6f5f 6372 6f73 735f  ..texinfo_cross_
-00002f70: 7265 6665 7265 6e63 6573 9488 4e4e 8794  references..NN..
-00002f80: 8c11 7465 7874 5f73 6563 7469 6f6e 6368  ..text_sectionch
-00002f90: 6172 7394 8c07 2a3d 2d7e 222b 6094 68d5  ars...*=-~"+`.h.
-00002fa0: 4e87 948c 0d74 6578 745f 6e65 776c 696e  N....text_newlin
-00002fb0: 6573 948c 0475 6e69 7894 68d5 4e87 948c  es...unix.h.N...
-00002fc0: 1374 6578 745f 6164 645f 7365 636e 756d  .text_add_secnum
-00002fd0: 6265 7273 9488 68d5 4e87 948c 1574 6578  bers..h.N....tex
-00002fe0: 745f 7365 636e 756d 6265 725f 7375 6666  t_secnumber_suff
-00002ff0: 6978 948c 022e 2094 68d5 4e87 948c 0a78  ix.... .h.N....x
-00003000: 6d6c 5f70 7265 7474 7994 8868 d54e 8794  ml_pretty..h.N..
-00003010: 8c0f 635f 6964 5f61 7474 7269 6275 7465  ..c_id_attribute
-00003020: 7394 5d94 68d5 4e87 948c 1263 5f70 6172  s.].h.N....c_par
-00003030: 656e 5f61 7474 7269 6275 7465 7394 5d94  en_attributes.].
-00003040: 68d5 4e87 948c 1063 5f65 7874 7261 5f6b  h.N....c_extra_k
-00003050: 6579 776f 7264 7394 5d94 288c 0761 6c69  eywords.].(..ali
-00003060: 676e 6173 948c 0761 6c69 676e 6f66 948c  gnas...alignof..
-00003070: 0462 6f6f 6c94 8c07 636f 6d70 6c65 7894  .bool...complex.
-00003080: 8c09 696d 6167 696e 6172 7994 8c08 6e6f  ..imaginary...no
-00003090: 7265 7475 726e 948c 0d73 7461 7469 635f  return...static_
-000030a0: 6173 7365 7274 948c 0c74 6872 6561 645f  assert...thread_
-000030b0: 6c6f 6361 6c94 6568 d54e 8794 8c0e 635f  local.eh.N....c_
-000030c0: 616c 6c6f 775f 7072 655f 7633 9489 68d5  allow_pre_v3..h.
-000030d0: 4e87 948c 1863 5f77 6172 6e5f 6f6e 5f61  N....c_warn_on_a
-000030e0: 6c6c 6f77 6564 5f70 7265 5f76 3394 8868  llowed_pre_v3..h
-000030f0: d54e 8794 8c17 6370 705f 696e 6465 785f  .N....cpp_index_
-00003100: 636f 6d6d 6f6e 5f70 7265 6669 7894 5d94  common_prefix.].
-00003110: 68d5 4e87 948c 1163 7070 5f69 645f 6174  h.N....cpp_id_at
-00003120: 7472 6962 7574 6573 945d 9468 d54e 8794  tributes.].h.N..
-00003130: 8c14 6370 705f 7061 7265 6e5f 6174 7472  ..cpp_paren_attr
-00003140: 6962 7574 6573 945d 9468 d54e 8794 8c10  ibutes.].h.N....
-00003150: 6370 705f 6465 6275 675f 6c6f 6f6b 7570  cpp_debug_lookup
-00003160: 9489 681f 4e87 948c 1363 7070 5f64 6562  ..h.N....cpp_deb
-00003170: 7567 5f73 686f 775f 7472 6565 9489 681f  ug_show_tree..h.
-00003180: 4e87 948c 1973 7472 6970 5f73 6967 6e61  N....strip_signa
-00003190: 7475 7265 5f62 6163 6b73 6c61 7368 9489  ture_backslash..
-000031a0: 68d5 4e87 948c 2170 7974 686f 6e5f 7573  h.N...!python_us
-000031b0: 655f 756e 7175 616c 6966 6965 645f 7479  e_unqualified_ty
-000031c0: 7065 5f6e 616d 6573 9489 68d5 4e87 948c  pe_names..h.N...
-000031d0: 1561 7070 6c65 6865 6c70 5f62 756e 646c  .applehelp_bundl
-000031e0: 655f 6e61 6d65 9468 d48c 0961 7070 6c65  e_name.h...apple
-000031f0: 6865 6c70 944e 8794 8c13 6170 706c 6568  help.N....appleh
-00003200: 656c 705f 6275 6e64 6c65 5f69 6494 4e6a  elp_bundle_id.Nj
-00003210: c002 0000 4e87 948c 1461 7070 6c65 6865  ....N....applehe
-00003220: 6c70 5f64 6576 5f72 6567 696f 6e94 8c05  lp_dev_region...
-00003230: 656e 2d75 7394 6ac0 0200 004e 8794 8c18  en-us.j....N....
-00003240: 6170 706c 6568 656c 705f 6275 6e64 6c65  applehelp_bundle
-00003250: 5f76 6572 7369 6f6e 948c 0131 946a c002  _version...1.j..
-00003260: 0000 4e87 948c 0e61 7070 6c65 6865 6c70  ..N....applehelp
-00003270: 5f69 636f 6e94 4e6a c002 0000 4e87 948c  _icon.Nj....N...
-00003280: 1461 7070 6c65 6865 6c70 5f6b 625f 7072  .applehelp_kb_pr
-00003290: 6f64 7563 7494 8c07 5079 7468 6f6e 2d94  oduct...Python-.
-000032a0: 6ac0 0200 004e 8794 8c10 6170 706c 6568  j....N....appleh
-000032b0: 656c 705f 6b62 5f75 726c 944e 6ac0 0200  elp_kb_url.Nj...
-000032c0: 004e 8794 8c14 6170 706c 6568 656c 705f  .N....applehelp_
-000032d0: 7265 6d6f 7465 5f75 726c 944e 6ac0 0200  remote_url.Nj...
-000032e0: 004e 8794 8c17 6170 706c 6568 656c 705f  .N....applehelp_
-000032f0: 696e 6465 785f 616e 6368 6f72 7394 896a  index_anchors..j
-00003300: c002 0000 4e87 948c 1961 7070 6c65 6865  ....N....applehe
-00003310: 6c70 5f6d 696e 5f74 6572 6d5f 6c65 6e67  lp_min_term_leng
-00003320: 7468 944e 6ac0 0200 004e 8794 8c13 6170  th.Nj....N....ap
-00003330: 706c 6568 656c 705f 7374 6f70 776f 7264  plehelp_stopword
-00003340: 7394 6a5d 0100 006a c002 0000 4e87 948c  s.j]...j....N...
-00003350: 1061 7070 6c65 6865 6c70 5f6c 6f63 616c  .applehelp_local
-00003360: 6594 6a5d 0100 006a c002 0000 4e87 948c  e.j]...j....N...
-00003370: 0f61 7070 6c65 6865 6c70 5f74 6974 6c65  .applehelp_title
-00003380: 948c 0b50 7974 686f 6e20 4865 6c70 946a  ...Python Help.j
-00003390: c002 0000 4e87 948c 1b61 7070 6c65 6865  ....N....applehe
-000033a0: 6c70 5f63 6f64 6573 6967 6e5f 6964 656e  lp_codesign_iden
-000033b0: 7469 7479 944e 6ac0 0200 004e 8794 8c18  tity.Nj....N....
-000033c0: 6170 706c 6568 656c 705f 636f 6465 7369  applehelp_codesi
-000033d0: 676e 5f66 6c61 6773 945d 946a c002 0000  gn_flags.].j....
-000033e0: 4e87 948c 1661 7070 6c65 6865 6c70 5f69  N....applehelp_i
-000033f0: 6e64 6578 6572 5f70 6174 6894 8c0f 2f75  ndexer_path.../u
-00003400: 7372 2f62 696e 2f68 6975 7469 6c94 6ac0  sr/bin/hiutil.j.
-00003410: 0200 004e 8794 8c17 6170 706c 6568 656c  ...N....applehel
-00003420: 705f 636f 6465 7369 676e 5f70 6174 6894  p_codesign_path.
-00003430: 8c11 2f75 7372 2f62 696e 2f63 6f64 6573  ../usr/bin/codes
-00003440: 6967 6e94 6ac0 0200 004e 8794 8c20 6170  ign.j....N... ap
-00003450: 706c 6568 656c 705f 6469 7361 626c 655f  plehelp_disable_
-00003460: 6578 7465 726e 616c 5f74 6f6f 6c73 9489  external_tools..
-00003470: 6ac0 0200 004e 8794 8c10 6465 7668 656c  j....N....devhel
-00003480: 705f 6261 7365 6e61 6d65 9468 d48c 0764  p_basename.h...d
-00003490: 6576 6865 6c70 944e 8794 8c11 6874 6d6c  evhelp.N....html
-000034a0: 6865 6c70 5f62 6173 656e 616d 6594 8c09  help_basename...
-000034b0: 7079 7468 6f6e 646f 6394 681f 4e87 948c  pythondoc.h.N...
-000034c0: 1468 746d 6c68 656c 705f 6669 6c65 5f73  .htmlhelp_file_s
-000034d0: 7566 6669 7894 4e68 d94e 8794 8c14 6874  uffix.Nh.N....ht
-000034e0: 6d6c 6865 6c70 5f6c 696e 6b5f 7375 6666  mlhelp_link_suff
-000034f0: 6978 944e 68d9 4e87 948c 0f71 7468 656c  ix.Nh.N....qthel
-00003500: 705f 6261 7365 6e61 6d65 9468 d468 d94e  p_basename.h.h.N
-00003510: 8794 8c10 7174 6865 6c70 5f6e 616d 6573  ....qthelp_names
-00003520: 7061 6365 944e 68d9 4e87 948c 0c71 7468  pace.Nh.N....qth
-00003530: 656c 705f 7468 656d 6594 8c05 6e6f 6e61  elp_theme...nona
-00003540: 7694 68d9 4e87 948c 1471 7468 656c 705f  v.h.N....qthelp_
-00003550: 7468 656d 655f 6f70 7469 6f6e 7394 7d94  theme_options.}.
-00003560: 68d9 4e87 948c 1574 6f67 676c 6562 7574  h.N....togglebut
-00003570: 746f 6e5f 7365 6c65 6374 6f72 948c 1d2e  ton_selector....
-00003580: 746f 6767 6c65 2c20 2e61 646d 6f6e 6974  toggle, .admonit
-00003590: 696f 6e2e 6472 6f70 646f 776e 9468 d94e  ion.dropdown.h.N
-000035a0: 8794 8c11 746f 6767 6c65 6275 7474 6f6e  ....togglebutton
-000035b0: 5f68 696e 7494 8c0d 436c 6963 6b20 746f  _hint...Click to
-000035c0: 2073 686f 7794 68d9 4e87 948c 1674 6f67   show.h.N....tog
-000035d0: 676c 6562 7574 746f 6e5f 6869 6e74 5f68  glebutton_hint_h
-000035e0: 6964 6594 8c0d 436c 6963 6b20 746f 2068  ide...Click to h
-000035f0: 6964 6594 68d9 4e87 948c 1a74 6f67 676c  ide.h.N....toggl
-00003600: 6562 7574 746f 6e5f 6f70 656e 5f6f 6e5f  ebutton_open_on_
-00003610: 7072 696e 7494 8868 d94e 8794 6ad1 0100  print..h.N..j...
-00003620: 0068 1f68 d94e 8794 6ad2 0100 0089 68d9  .h.h.N..j.....h.
-00003630: 4e87 946a d301 0000 8868 d94e 8794 6ad4  N..j.....h.N..j.
-00003640: 0100 0088 68d9 4e87 946a d501 0000 8868  ....h.N..j.....h
-00003650: d94e 8794 6ad6 0100 0068 1f68 d94e 8794  .N..j....h.h.N..
-00003660: 6ad7 0100 0068 1f68 d94e 8794 6ad8 0100  j....h.h.N..j...
-00003670: 0068 1f68 d94e 8794 6ad9 0100 006a da01  .h.h.N..j....j..
-00003680: 0000 68d9 4e87 946a dd01 0000 6ade 0100  ..h.N..j....j...
-00003690: 0068 d94e 8794 8c15 636f 7079 6275 7474  .h.N....copybutt
-000036a0: 6f6e 5f69 6d61 6765 5f70 6174 6894 681f  on_image_path.h.
-000036b0: 68d9 4e87 948c 146d 7973 745f 636f 6d6d  h.N....myst_comm
-000036c0: 6f6e 6d61 726b 5f6f 6e6c 7994 8968 d54e  onmark_only..h.N
-000036d0: 8794 8c0d 6d79 7374 5f67 666d 5f6f 6e6c  ....myst_gfm_onl
-000036e0: 7994 8968 d54e 8794 8c16 6d79 7374 5f65  y..h.N....myst_e
-000036f0: 6e61 626c 655f 6578 7465 6e73 696f 6e73  nable_extensions
-00003700: 9468 4e68 d54e 8794 8c13 6d79 7374 5f64  .hNh.N....myst_d
-00003710: 6973 6162 6c65 5f73 796e 7461 7894 5d94  isable_syntax.].
-00003720: 68d5 4e87 948c 176d 7973 745f 616c 6c5f  h.N....myst_all_
-00003730: 6c69 6e6b 735f 6578 7465 726e 616c 9489  links_external..
-00003740: 68d5 4e87 948c 106d 7973 745f 7572 6c5f  h.N....myst_url_
-00003750: 7363 6865 6d65 7394 6855 68d5 4e87 948c  schemes.hUh.N...
-00003760: 106d 7973 745f 7265 665f 646f 6d61 696e  .myst_ref_domain
-00003770: 7394 4e68 d54e 8794 8c17 6d79 7374 5f6e  s.Nh.N....myst_n
-00003780: 756d 6265 725f 636f 6465 5f62 6c6f 636b  umber_code_block
-00003790: 7394 5d94 68d5 4e87 948c 146d 7973 745f  s.].h.N....myst_
-000037a0: 7469 746c 655f 746f 5f68 6561 6465 7294  title_to_header.
-000037b0: 8968 d54e 8794 8c14 6d79 7374 5f68 6561  .h.N....myst_hea
-000037c0: 6469 6e67 5f61 6e63 686f 7273 944e 68d5  ding_anchors.Nh.
-000037d0: 4e87 948c 166d 7973 745f 6865 6164 696e  N....myst_headin
-000037e0: 675f 736c 7567 5f66 756e 6394 4e68 d54e  g_slug_func.Nh.N
-000037f0: 8794 8c0e 6d79 7374 5f68 746d 6c5f 6d65  ....myst_html_me
-00003800: 7461 947d 9468 d54e 8794 8c18 6d79 7374  ta.}.h.N....myst
-00003810: 5f66 6f6f 746e 6f74 655f 7472 616e 7369  _footnote_transi
-00003820: 7469 6f6e 9488 68d5 4e87 948c 156d 7973  tion..h.N....mys
-00003830: 745f 776f 7264 735f 7065 725f 6d69 6e75  t_words_per_minu
-00003840: 7465 944b c868 d54e 8794 8c12 6d79 7374  te.K.h.N....myst
-00003850: 5f73 7562 7374 6974 7574 696f 6e73 947d  _substitutions.}
-00003860: 9468 d54e 8794 8c13 6d79 7374 5f73 7562  .h.N....myst_sub
-00003870: 5f64 656c 696d 6974 6572 7394 8c01 7b94  _delimiters...{.
-00003880: 8c01 7d94 8694 68d5 4e87 948c 186d 7973  ..}...h.N....mys
-00003890: 745f 6c69 6e6b 6966 795f 6675 7a7a 795f  t_linkify_fuzzy_
-000038a0: 6c69 6e6b 7394 8868 d54e 8794 8c17 6d79  links..h.N....my
-000038b0: 7374 5f64 6d61 7468 5f61 6c6c 6f77 5f6c  st_dmath_allow_l
-000038c0: 6162 656c 7394 8868 d54e 8794 8c16 6d79  abels..h.N....my
-000038d0: 7374 5f64 6d61 7468 5f61 6c6c 6f77 5f73  st_dmath_allow_s
-000038e0: 7061 6365 9488 68d5 4e87 948c 176d 7973  pace..h.N....mys
-000038f0: 745f 646d 6174 685f 616c 6c6f 775f 6469  t_dmath_allow_di
-00003900: 6769 7473 9488 68d5 4e87 948c 186d 7973  gits..h.N....mys
-00003910: 745f 646d 6174 685f 646f 7562 6c65 5f69  t_dmath_double_i
-00003920: 6e6c 696e 6594 8968 d54e 8794 8c13 6d79  nline..h.N....my
-00003930: 7374 5f75 7064 6174 655f 6d61 7468 6a61  st_update_mathja
-00003940: 7894 8868 d54e 8794 8c14 6d79 7374 5f6d  x..h.N....myst_m
-00003950: 6174 686a 6178 5f63 6c61 7373 6573 9468  athjax_classes.h
-00003960: c968 d54e 8794 8c11 6e62 5f63 7573 746f  .h.N....nb_custo
-00003970: 6d5f 666f 726d 6174 7394 7d94 68d5 4e87  m_formats.}.h.N.
-00003980: 948c 0f6e 625f 6d65 7461 6461 7461 5f6b  ...nb_metadata_k
-00003990: 6579 948c 066d 7973 746e 6294 68d5 4e87  ey...mystnb.h.N.
-000039a0: 948c 146e 625f 6365 6c6c 5f6d 6574 6164  ...nb_cell_metad
-000039b0: 6174 615f 6b65 7994 6a4f 0300 0068 d54e  ata_key.jO...h.N
-000039c0: 8794 8c0d 6e62 5f72 656e 6465 725f 6b65  ....nb_render_ke
-000039d0: 7994 8c09 2d2d 756e 7365 742d 2d94 68d5  y...--unset--.h.
-000039e0: 4e87 948c 156e 625f 6b65 726e 656c 5f72  N....nb_kernel_r
-000039f0: 6778 5f61 6c69 6173 6573 947d 9468 d54e  gx_aliases.}.h.N
-00003a00: 8794 8c11 6e62 5f65 7865 6375 7469 6f6e  ....nb_execution
-00003a10: 5f6d 6f64 6594 6860 68d5 4e87 948c 196a  _mode.h`h.N....j
-00003a20: 7570 7974 6572 5f65 7865 6375 7465 5f6e  upyter_execute_n
-00003a30: 6f74 6562 6f6f 6b73 946a 5403 0000 68d5  otebooks.jT...h.
-00003a40: 4e87 948c 176e 625f 6578 6563 7574 696f  N....nb_executio
-00003a50: 6e5f 6361 6368 655f 7061 7468 9468 1f68  n_cache_path.h.h
-00003a60: d54e 8794 8c0d 6a75 7079 7465 725f 6361  .N....jupyter_ca
-00003a70: 6368 6594 6a54 0300 0068 d54e 8794 8c1c  che.jT...h.N....
-00003a80: 6e62 5f65 7865 6375 7469 6f6e 5f65 7863  nb_execution_exc
-00003a90: 6c75 6465 7061 7474 6572 6e73 9468 6268  ludepatterns.hbh
-00003aa0: d54e 8794 8c19 6578 6563 7574 696f 6e5f  .N....execution_
-00003ab0: 6578 636c 7564 6570 6174 7465 726e 7394  excludepatterns.
-00003ac0: 6a54 0300 0068 d54e 8794 8c14 6e62 5f65  jT...h.N....nb_e
-00003ad0: 7865 6375 7469 6f6e 5f74 696d 656f 7574  xecution_timeout
-00003ae0: 944b 1e68 d54e 8794 8c11 6578 6563 7574  .K.h.N....execut
-00003af0: 696f 6e5f 7469 6d65 6f75 7494 6a54 0300  ion_timeout.jT..
-00003b00: 0068 d54e 8794 8c14 6e62 5f65 7865 6375  .h.N....nb_execu
-00003b10: 7469 6f6e 5f69 6e5f 7465 6d70 9489 68d5  tion_in_temp..h.
-00003b20: 4e87 948c 1165 7865 6375 7469 6f6e 5f69  N....execution_i
-00003b30: 6e5f 7465 6d70 946a 5403 0000 68d5 4e87  n_temp.jT...h.N.
-00003b40: 948c 196e 625f 6578 6563 7574 696f 6e5f  ...nb_execution_
-00003b50: 616c 6c6f 775f 6572 726f 7273 9489 68d5  allow_errors..h.
-00003b60: 4e87 948c 1665 7865 6375 7469 6f6e 5f61  N....execution_a
-00003b70: 6c6c 6f77 5f65 7272 6f72 7394 6a54 0300  llow_errors.jT..
-00003b80: 0068 d54e 8794 8c1b 6e62 5f65 7865 6375  .h.N....nb_execu
-00003b90: 7469 6f6e 5f72 6169 7365 5f6f 6e5f 6572  tion_raise_on_er
-00003ba0: 726f 7294 8968 d54e 8794 8c14 6e62 5f65  ror..h.N....nb_e
-00003bb0: 7865 6375 7469 6f6e 5f73 686f 775f 7462  xecution_show_tb
-00003bc0: 9489 68d5 4e87 948c 1165 7865 6375 7469  ..h.N....executi
-00003bd0: 6f6e 5f73 686f 775f 7462 946a 5403 0000  on_show_tb.jT...
-00003be0: 68d5 4e87 948c 106e 625f 6d65 7267 655f  h.N....nb_merge_
-00003bf0: 7374 7265 616d 7394 8968 d54e 8794 8c10  streams..h.N....
-00003c00: 6e62 5f72 656e 6465 725f 706c 7567 696e  nb_render_plugin
-00003c10: 946a 0401 0000 68d5 4e87 948c 156e 625f  .j....h.N....nb_
-00003c20: 7265 6d6f 7665 5f63 6f64 655f 736f 7572  remove_code_sour
-00003c30: 6365 9489 68d5 4e87 948c 166e 625f 7265  ce..h.N....nb_re
-00003c40: 6d6f 7665 5f63 6f64 655f 6f75 7470 7574  move_code_output
-00003c50: 7394 8968 d54e 8794 8c13 6e62 5f63 6f64  s..h.N....nb_cod
-00003c60: 655f 7072 6f6d 7074 5f73 686f 7794 8c15  e_prompt_show...
-00003c70: 5368 6f77 2063 6f64 6520 6365 6c6c 207b  Show code cell {
-00003c80: 7479 7065 7d94 68d5 4e87 948c 136e 625f  type}.h.N....nb_
-00003c90: 636f 6465 5f70 726f 6d70 745f 6869 6465  code_prompt_hide
-00003ca0: 948c 1548 6964 6520 636f 6465 2063 656c  ...Hide code cel
-00003cb0: 6c20 7b74 7970 657d 9468 d54e 8794 8c16  l {type}.h.N....
-00003cc0: 6e62 5f6e 756d 6265 725f 736f 7572 6365  nb_number_source
-00003cd0: 5f6c 696e 6573 9489 68d5 4e87 948c 1a6e  _lines..h.N....n
-00003ce0: 625f 6d69 6d65 5f70 7269 6f72 6974 795f  b_mime_priority_
-00003cf0: 6f76 6572 7269 6465 7394 2968 d54e 8794  overrides.)h.N..
-00003d00: 8c10 6e62 5f6f 7574 7075 745f 7374 6465  ..nb_output_stde
-00003d10: 7272 9468 5c68 d54e 8794 8c14 6e62 5f72  rr.h\h.N....nb_r
-00003d20: 656e 6465 725f 7465 7874 5f6c 6578 6572  ender_text_lexer
-00003d30: 948c 096d 7973 742d 616e 7369 9468 d54e  ...myst-ansi.h.N
-00003d40: 8794 8c15 6e62 5f72 656e 6465 725f 6572  ....nb_render_er
-00003d50: 726f 725f 6c65 7865 7294 8c09 6970 7974  ror_lexer...ipyt
-00003d60: 686f 6e74 6294 68d5 4e87 948c 176e 625f  hontb.h.N....nb_
-00003d70: 7265 6e64 6572 5f69 6d61 6765 5f6f 7074  render_image_opt
-00003d80: 696f 6e73 947d 9468 d54e 8794 8c18 6e62  ions.}.h.N....nb
-00003d90: 5f72 656e 6465 725f 6669 6775 7265 5f6f  _render_figure_o
-00003da0: 7074 696f 6e73 947d 9468 d54e 8794 8c19  ptions.}.h.N....
-00003db0: 6e62 5f72 656e 6465 725f 6d61 726b 646f  nb_render_markdo
-00003dc0: 776e 5f66 6f72 6d61 7494 8c0a 636f 6d6d  wn_format...comm
-00003dd0: 6f6e 6d61 726b 9468 d54e 8794 8c10 6e62  onmark.h.N....nb
-00003de0: 5f69 7079 7769 6467 6574 735f 6a73 947d  _ipywidgets_js.}
-00003df0: 9428 8c46 6874 7470 733a 2f2f 6364 6e6a  .(.Fhttps://cdnj
-00003e00: 732e 636c 6f75 6466 6c61 7265 2e63 6f6d  s.cloudflare.com
-00003e10: 2f61 6a61 782f 6c69 6273 2f72 6571 7569  /ajax/libs/requi
-00003e20: 7265 2e6a 732f 322e 332e 342f 7265 7175  re.js/2.3.4/requ
-00003e30: 6972 652e 6d69 6e2e 6a73 947d 9428 8c09  ire.min.js.}.(..
-00003e40: 696e 7465 6772 6974 7994 8c33 7368 6132  integrity..3sha2
-00003e50: 3536 2d41 6532 567a 2f34 6550 6449 7536  56-Ae2Vz/4ePdIu6
-00003e60: 5a79 492f 355a 4773 596e 622b 6d30 4a6c  ZyI/5ZGsYnb+m0Jl
-00003e70: 4f6d 4b50 6a74 3658 5a39 4a4a 6b41 3d94  OmKPjt6XZ9JJkA=.
-00003e80: 8c0b 6372 6f73 736f 7269 6769 6e94 8c09  ..crossorigin...
-00003e90: 616e 6f6e 796d 6f75 7394 758c 5268 7474  anonymous.u.Rhtt
-00003ea0: 7073 3a2f 2f63 646e 2e6a 7364 656c 6976  ps://cdn.jsdeliv
-00003eb0: 722e 6e65 742f 6e70 6d2f 406a 7570 7974  r.net/npm/@jupyt
-00003ec0: 6572 2d77 6964 6765 7473 2f68 746d 6c2d  er-widgets/html-
-00003ed0: 6d61 6e61 6765 7240 312e 302e 362f 6469  manager@1.0.6/di
-00003ee0: 7374 2f65 6d62 6564 2d61 6d64 2e6a 7394  st/embed-amd.js.
-00003ef0: 7d94 288c 1864 6174 612d 6a75 7079 7465  }.(..data-jupyte
-00003f00: 722d 7769 6467 6574 732d 6364 6e94 8c1d  r-widgets-cdn...
-00003f10: 6874 7470 733a 2f2f 6364 6e2e 6a73 6465  https://cdn.jsde
-00003f20: 6c69 7672 2e6e 6574 2f6e 706d 2f94 6aa0  livr.net/npm/.j.
-00003f30: 0300 006a a103 0000 7575 68d5 4e87 948c  ...j....uuh.N...
-00003f40: 126e 625f 7265 6e64 6572 5f70 7269 6f72  .nb_render_prior
-00003f50: 6974 7994 6a54 0300 0068 d54e 8794 6865  ity.jT...h.N..he
-00003f60: 8868 d54e 8794 684c 8868 d54e 8794 8c0c  .h.N..hL.h.N....
-00003f70: 7468 6562 655f 636f 6e66 6967 947d 9428  thebe_config.}.(
-00003f80: 8c0b 616c 7761 7973 5f6c 6f61 6494 898c  ..always_load...
-00003f90: 0873 656c 6563 746f 7294 8c0c 2e74 6865  .selector....the
-00003fa0: 6265 2c2e 6365 6c6c 948c 0e73 656c 6563  be,.cell...selec
-00003fb0: 746f 725f 696e 7075 7494 8c03 7072 6594  tor_input...pre.
-00003fc0: 8c0f 7365 6c65 6374 6f72 5f6f 7574 7075  ..selector_outpu
-00003fd0: 7494 8c15 2e6f 7574 7075 742c 202e 6365  t....output, .ce
-00003fe0: 6c6c 5f6f 7574 7075 7494 7568 d94e 8794  ll_output.uh.N..
-00003ff0: 6848 6849 68d9 4e87 9468 6968 6a68 d54e  hHhIh.N..hihjh.N
-00004000: 8794 6845 8968 d54e 8794 8c13 696e 7465  ..hE.h.N....inte
-00004010: 7273 7068 696e 785f 6d61 7070 696e 6794  rsphinx_mapping.
-00004020: 7d94 68d5 4e87 948c 1769 6e74 6572 7370  }.h.N....intersp
-00004030: 6869 6e78 5f63 6163 6865 5f6c 696d 6974  hinx_cache_limit
-00004040: 944b 0568 1f4e 8794 8c13 696e 7465 7273  .K.h.N....inters
-00004050: 7068 696e 785f 7469 6d65 6f75 7494 4e68  phinx_timeout.Nh
-00004060: 1f4e 8794 8c1d 696e 7465 7273 7068 696e  .N....intersphin
-00004070: 785f 6469 7361 626c 6564 5f72 6566 7479  x_disabled_refty
-00004080: 7065 7394 5d94 68d5 4e87 948c 1473 645f  pes.].h.N....sd_
-00004090: 666f 6e74 6177 6573 6f6d 655f 6c61 7465  fontawesome_late
-000040a0: 7894 8968 d54e 8794 8c14 6269 6274 6578  x..h.N....bibtex
-000040b0: 5f64 6566 6175 6c74 5f73 7479 6c65 948c  _default_style..
-000040c0: 0561 6c70 6861 9468 d94e 8794 8c0f 6269  .alpha.h.N....bi
-000040d0: 6274 6578 5f74 6f6f 6c74 6970 7394 8868  btex_tooltips..h
-000040e0: d94e 8794 8c15 6269 6274 6578 5f74 6f6f  .N....bibtex_too
-000040f0: 6c74 6970 735f 7374 796c 6594 681f 68d9  ltips_style.h.h.
-00004100: 4e87 9468 6668 6768 d94e 8794 8c0f 6269  N..hfhgh.N....bi
-00004110: 6274 6578 5f65 6e63 6f64 696e 6794 8c09  btex_encoding...
-00004120: 7574 662d 382d 7369 6794 68d9 4e87 948c  utf-8-sig.h.N...
-00004130: 1a62 6962 7465 785f 6269 626c 696f 6772  .bibtex_bibliogr
-00004140: 6170 6879 5f68 6561 6465 7294 681f 68d9  aphy_header.h.h.
-00004150: 4e87 948c 1e62 6962 7465 785f 666f 6f74  N....bibtex_foot
-00004160: 6269 626c 696f 6772 6170 6879 5f68 6561  bibliography_hea
-00004170: 6465 7294 681f 68d9 4e87 948c 1662 6962  der.h.h.N....bib
-00004180: 7465 785f 7265 6665 7265 6e63 655f 7374  tex_reference_st
-00004190: 796c 6594 8c05 6c61 6265 6c94 68d5 4e87  yle...label.h.N.
-000041a0: 948c 1b62 6962 7465 785f 666f 6f74 5f72  ...bibtex_foot_r
-000041b0: 6566 6572 656e 6365 5f73 7479 6c65 948c  eference_style..
-000041c0: 0466 6f6f 7494 68d5 4e87 948c 0e62 6962  .foot.h.N....bib
-000041d0: 7465 785f 6369 7465 5f69 6494 681f 68d9  tex_cite_id.h.h.
-000041e0: 4e87 948c 1262 6962 7465 785f 666f 6f74  N....bibtex_foot
-000041f0: 6369 7465 5f69 6494 681f 68d9 4e87 948c  cite_id.h.h.N...
-00004200: 1662 6962 7465 785f 6269 626c 696f 6772  .bibtex_bibliogr
-00004210: 6170 6879 5f69 6494 681f 68d9 4e87 948c  aphy_id.h.h.N...
-00004220: 1a62 6962 7465 785f 666f 6f74 6269 626c  .bibtex_footbibl
-00004230: 696f 6772 6170 6879 5f69 6494 681f 68d9  iography_id.h.h.
-00004240: 4e87 948c 196a 626c 6174 6578 5f6c 6f61  N....jblatex_loa
-00004250: 645f 696d 6763 6f6e 7665 7274 6572 9488  d_imgconverter..
-00004260: 68d5 4e87 9468 7c68 7d68 d54e 8794 8c19  h.N..h|h}h.N....
-00004270: 6a62 6c61 7465 785f 6361 7074 696f 6e73  jblatex_captions
-00004280: 5f74 6f5f 7061 7274 7394 4e68 d54e 8794  _to_parts.Nh.N..
-00004290: 7575 628c 0d63 6f6e 6669 675f 7374 6174  uub..config_stat
-000042a0: 7573 944b 018c 1363 6f6e 6669 675f 7374  us.K...config_st
-000042b0: 6174 7573 5f65 7874 7261 9468 1f8c 0665  atus_extra.h...e
-000042c0: 7665 6e74 7394 4e68 d38c 0e73 7068 696e  vents.Nh...sphin
-000042d0: 782e 7072 6f6a 6563 7494 8c07 5072 6f6a  x.project...Proj
-000042e0: 6563 7494 9394 2981 947d 9428 6808 6809  ect...)..}.(h.h.
-000042f0: 6884 6888 8c08 646f 636e 616d 6573 948f  h.h...docnames..
-00004300: 9428 8c06 5245 4144 4d45 948c 172e 6e61  .(..README....na
-00004310: 7061 7269 2d68 7562 2f44 4553 4352 4950  pari-hub/DESCRIP
-00004320: 5449 4f4e 948c 0941 4c47 4f52 4954 484d  TION...ALGORITHM
-00004330: 9490 7562 68dc 7d94 288c 1073 7068 696e  ..ubh.}.(..sphin
-00004340: 782e 646f 6d61 696e 732e 6394 4b02 8c18  x.domains.c.K...
-00004350: 7370 6869 6e78 2e64 6f6d 6169 6e73 2e63  sphinx.domains.c
-00004360: 6861 6e67 6573 6574 944b 018c 1773 7068  hangeset.K...sph
-00004370: 696e 782e 646f 6d61 696e 732e 6369 7461  inx.domains.cita
-00004380: 7469 6f6e 944b 018c 1273 7068 696e 782e  tion.K...sphinx.
-00004390: 646f 6d61 696e 732e 6370 7094 4b05 8c14  domains.cpp.K...
-000043a0: 7370 6869 6e78 2e64 6f6d 6169 6e73 2e69  sphinx.domains.i
-000043b0: 6e64 6578 944b 018c 1973 7068 696e 782e  ndex.K...sphinx.
-000043c0: 646f 6d61 696e 732e 6a61 7661 7363 7269  domains.javascri
-000043d0: 7074 944b 028c 1373 7068 696e 782e 646f  pt.K...sphinx.do
-000043e0: 6d61 696e 732e 6d61 7468 944b 028c 1573  mains.math.K...s
-000043f0: 7068 696e 782e 646f 6d61 696e 732e 7079  phinx.domains.py
-00004400: 7468 6f6e 944b 038c 1273 7068 696e 782e  thon.K...sphinx.
-00004410: 646f 6d61 696e 732e 7273 7494 4b02 8c12  domains.rst.K...
-00004420: 7370 6869 6e78 2e64 6f6d 6169 6e73 2e73  sphinx.domains.s
-00004430: 7464 944b 0268 754b 0168 774b 0968 134b  td.K.huK.hwK.h.K
-00004440: 3875 8c14 7665 7273 696f 6e69 6e67 5f63  8u..versioning_c
-00004450: 6f6e 6469 7469 6f6e 9489 8c12 7665 7273  ondition....vers
-00004460: 696f 6e69 6e67 5f63 6f6d 7061 7265 9489  ioning_compare..
-00004470: 8c07 646f 6d61 696e 7394 7d94 8c08 7365  ..domains.}...se
-00004480: 7474 696e 6773 947d 9428 8c0e 6175 746f  ttings.}.(..auto
-00004490: 5f69 645f 7072 6566 6978 948c 0269 6494  _id_prefix...id.
-000044a0: 8c0c 656d 6265 645f 696d 6167 6573 9489  ..embed_images..
-000044b0: 8c10 656d 6265 645f 7374 796c 6573 6865  ..embed_styleshe
-000044c0: 6574 9489 8c15 636c 6f61 6b5f 656d 6169  et....cloak_emai
-000044d0: 6c5f 6164 6472 6573 7365 7394 888c 0c70  l_addresses....p
-000044e0: 6570 5f62 6173 655f 7572 6c94 8c18 6874  ep_base_url...ht
-000044f0: 7470 733a 2f2f 7065 7073 2e70 7974 686f  tps://peps.pytho
-00004500: 6e2e 6f72 672f 948c 0e70 6570 5f72 6566  n.org/...pep_ref
-00004510: 6572 656e 6365 7394 4e8c 0c72 6663 5f62  erences.N..rfc_b
-00004520: 6173 655f 7572 6c94 8c26 6874 7470 733a  ase_url..&https:
-00004530: 2f2f 6461 7461 7472 6163 6b65 722e 6965  //datatracker.ie
-00004540: 7466 2e6f 7267 2f64 6f63 2f68 746d 6c2f  tf.org/doc/html/
-00004550: 948c 0e72 6663 5f72 6566 6572 656e 6365  ...rfc_reference
-00004560: 7394 4e8c 0e69 6e70 7574 5f65 6e63 6f64  s.N..input_encod
-00004570: 696e 6794 68f5 8c0e 646f 6374 6974 6c65  ing.h...doctitle
-00004580: 5f78 666f 726d 9489 8c12 7365 6374 7375  _xform....sectsu
-00004590: 6274 6974 6c65 5f78 666f 726d 9489 8c11  btitle_xform....
-000045a0: 7365 6374 696f 6e5f 7365 6c66 5f6c 696e  section_self_lin
-000045b0: 6b94 898c 0a68 616c 745f 6c65 7665 6c94  k....halt_level.
-000045c0: 4b05 8c16 6669 6c65 5f69 6e73 6572 7469  K...file_inserti
-000045d0: 6f6e 5f65 6e61 626c 6564 9488 8c13 736d  on_enabled....sm
-000045e0: 6172 7471 756f 7465 735f 6c6f 6361 6c65  artquotes_locale
-000045f0: 7394 5d94 68d5 6803 68fe 898c 0d6c 616e  s.].h.h.h....lan
-00004600: 6775 6167 655f 636f 6465 946a 5d01 0000  guage_code.j]...
-00004610: 8c0c 736d 6172 745f 7175 6f74 6573 9488  ..smart_quotes..
-00004620: 758c 0861 6c6c 5f64 6f63 7394 7d94 286a  u..all_docs.}.(j
-00004630: f103 0000 4741 d928 0017 7c99 d26a f203  ....GA.(..|..j..
-00004640: 0000 4741 d928 0017 8367 426a f003 0000  ..GA.(...gBj....
-00004650: 4741 d928 0017 86d9 6375 8c0c 6465 7065  GA.(....cu..depe
-00004660: 6e64 656e 6369 6573 9468 858c 0b64 6566  ndencies.h...def
-00004670: 6175 6c74 6469 6374 9493 948c 0862 7569  aultdict.....bui
-00004680: 6c74 696e 7394 8c03 7365 7494 9394 8594  ltins...set.....
-00004690: 5294 6af2 0300 008f 9428 8c20 696d 6167  R.j......(. imag
-000046a0: 6573 2f70 6f69 6e74 5f63 6c6f 7564 735f  es/point_clouds_
-000046b0: 636f 6d70 6172 6564 2e70 6e67 948c 1d65  compared.png...e
-000046c0: 7861 6d70 6c65 732f 6170 706c 795f 6175  xamples/apply_au
-000046d0: 746f 656e 636f 6465 722e 7079 948c 2265  toencoder.py.."e
-000046e0: 7861 6d70 6c65 732f 7669 7375 616c 697a  xamples/visualiz
-000046f0: 655f 706f 696e 745f 636c 6f75 6473 2e70  e_point_clouds.p
-00004700: 7994 9073 8c08 696e 636c 7564 6564 946a  y..s..included.j
-00004710: 1d04 0000 6a20 0400 0085 9452 948c 0d72  ....j .....R...r
-00004720: 6572 6561 645f 616c 7761 7973 948f 948c  eread_always....
-00004730: 086d 6574 6164 6174 6194 6a1d 0400 006a  .metadata.j....j
-00004740: 1e04 0000 8c04 6469 6374 9493 9485 9452  ......dict.....R
-00004750: 9428 6af1 0300 007d 948c 0977 6f72 6463  .(j....}...wordc
-00004760: 6f75 6e74 947d 9428 8c05 776f 7264 7394  ount.}.(..words.
-00004770: 4b09 8c07 6d69 6e75 7465 7394 4b00 7573  K...minutes.K.us
-00004780: 6af2 0300 007d 946a 3204 0000 7d94 286a  j....}.j2...}.(j
-00004790: 3404 0000 4d51 026a 3504 0000 4b03 7573  4...MQ.j5...K.us
-000047a0: 6af0 0300 007d 946a 3204 0000 7d94 286a  j....}.j2...}.(j
-000047b0: 3404 0000 4b5c 6a35 0400 004b 0075 7375  4...K\j5...K.usu
-000047c0: 8c06 7469 746c 6573 947d 9428 6af1 0300  ..titles.}.(j...
-000047d0: 008c 0e64 6f63 7574 696c 732e 6e6f 6465  ...docutils.node
-000047e0: 7394 68b9 9394 2981 947d 9428 8c09 7261  s.h...)..}.(..ra
-000047f0: 7773 6f75 7263 6594 681f 8c08 6368 696c  wsource.h...chil
-00004800: 6472 656e 945d 946a 3c04 0000 8c04 5465  dren.].j<.....Te
-00004810: 7874 9493 948c 0a3c 6e6f 2074 6974 6c65  xt.....<no title
-00004820: 3e94 8594 8194 7d94 286a 4004 0000 681f  >.....}.(j@...h.
-00004830: 8c06 7061 7265 6e74 946a 3e04 0000 7562  ..parent.j>...ub
-00004840: 618c 0a61 7474 7269 6275 7465 7394 7d94  a..attributes.}.
-00004850: 288c 0369 6473 945d 948c 0763 6c61 7373  (..ids.]...class
-00004860: 6573 945d 948c 056e 616d 6573 945d 948c  es.]...names.]..
-00004870: 0864 7570 6e61 6d65 7394 5d94 8c08 6261  .dupnames.]...ba
-00004880: 636b 7265 6673 945d 9475 8c07 7461 676e  ckrefs.].u..tagn
-00004890: 616d 6594 68b9 7562 6af2 0300 006a 3d04  ame.h.ubj....j=.
-000048a0: 0000 2981 947d 9428 6a40 0400 0068 1f6a  ..)..}.(j@...h.j
-000048b0: 4104 0000 5d94 6a44 0400 008c 0941 6c67  A...].jD.....Alg
-000048c0: 6f72 6974 686d 9485 9481 947d 9428 6a40  orithm.....}.(j@
-000048d0: 0400 0068 1f6a 4904 0000 6a57 0400 0075  ...h.jI...jW...u
-000048e0: 6261 6a4a 0400 007d 9428 6a4c 0400 005d  bajJ...}.(jL...]
-000048f0: 946a 4e04 0000 5d94 6a50 0400 005d 946a  .jN...].jP...].j
-00004900: 5204 0000 5d94 6a54 0400 005d 9475 6a56  R...].jT...].ujV
-00004910: 0400 0068 b975 626a f003 0000 6a3d 0400  ...h.ubj....j=..
-00004920: 0029 8194 7d94 286a 4004 0000 681f 6a41  .)..}.(j@...h.jA
-00004930: 0400 005d 946a 4404 0000 8c18 766f 6c6c  ...].jD.....voll
-00004940: 7365 672d 6e61 7061 7269 2d74 7261 636b  seg-napari-track
-00004950: 6d61 7465 9485 9481 947d 9428 6a40 0400  mate.....}.(j@..
-00004960: 0068 1f6a 4904 0000 6a64 0400 0075 6261  .h.jI...jd...uba
-00004970: 6a4a 0400 007d 9428 6a4c 0400 005d 946a  jJ...}.(jL...].j
-00004980: 4e04 0000 5d94 6a50 0400 005d 946a 5204  N...].jP...].jR.
-00004990: 0000 5d94 6a54 0400 005d 9475 6a56 0400  ..].jT...].ujV..
-000049a0: 0068 b975 6275 8c0a 6c6f 6e67 7469 746c  .h.ubu..longtitl
-000049b0: 6573 947d 9428 6af1 0300 006a 3e04 0000  es.}.(j....j>...
-000049c0: 6af2 0300 006a 5704 0000 6af0 0300 006a  j....jW...j....j
-000049d0: 6404 0000 758c 0474 6f63 7394 7d94 286a  d...u..tocs.}.(j
-000049e0: f103 0000 6a3c 0400 008c 0b62 756c 6c65  ....j<.....bulle
-000049f0: 745f 6c69 7374 9493 9429 8194 7d94 286a  t_list...)..}.(j
-00004a00: 4004 0000 681f 6a41 0400 005d 946a 4a04  @...h.jA...].jJ.
-00004a10: 0000 7d94 286a 4c04 0000 5d94 6a4e 0400  ..}.(jL...].jN..
-00004a20: 005d 946a 5004 0000 5d94 6a52 0400 005d  .].jP...].jR...]
-00004a30: 946a 5404 0000 5d94 756a 5604 0000 6a75  .jT...].ujV...ju
-00004a40: 0400 0075 626a f203 0000 6a76 0400 0029  ...ubj....jv...)
-00004a50: 8194 7d94 286a 4004 0000 681f 6a41 0400  ..}.(j@...h.jA..
-00004a60: 005d 946a 3c04 0000 8c09 6c69 7374 5f69  .].j<.....list_i
-00004a70: 7465 6d94 9394 2981 947d 9428 6a40 0400  tem...)..}.(j@..
-00004a80: 0068 1f6a 4104 0000 5d94 288c 0f73 7068  .h.jA...].(..sph
-00004a90: 696e 782e 6164 646e 6f64 6573 948c 1163  inx.addnodes...c
-00004aa0: 6f6d 7061 6374 5f70 6172 6167 7261 7068  ompact_paragraph
-00004ab0: 9493 9429 8194 7d94 286a 4004 0000 681f  ...)..}.(j@...h.
-00004ac0: 6a41 0400 005d 946a 3c04 0000 8c09 7265  jA...].j<.....re
-00004ad0: 6665 7265 6e63 6594 9394 2981 947d 9428  ference...)..}.(
-00004ae0: 6a40 0400 0068 1f6a 4104 0000 5d94 6a44  j@...h.jA...].jD
-00004af0: 0400 008c 0941 6c67 6f72 6974 686d 9485  .....Algorithm..
-00004b00: 9481 947d 9428 6a40 0400 0068 1f6a 4904  ...}.(j@...h.jI.
-00004b10: 0000 6a90 0400 0075 6261 6a4a 0400 007d  ..j....ubajJ...}
-00004b20: 9428 6a4c 0400 005d 946a 4e04 0000 5d94  .(jL...].jN...].
-00004b30: 6a50 0400 005d 946a 5204 0000 5d94 6a54  jP...].jR...].jT
-00004b40: 0400 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-00004b50: 888c 0672 6566 7572 6994 6af2 0300 008c  ...refuri.j.....
-00004b60: 0a61 6e63 686f 726e 616d 6594 681f 756a  .anchorname.h.uj
-00004b70: 5604 0000 6a8e 0400 006a 4904 0000 6a8b  V...j....jI...j.
-00004b80: 0400 0075 6261 6a4a 0400 007d 9428 6a4c  ...ubajJ...}.(jL
-00004b90: 0400 005d 946a 4e04 0000 5d94 6a50 0400  ...].jN...].jP..
-00004ba0: 005d 946a 5204 0000 5d94 6a54 0400 005d  .].jR...].jT...]
-00004bb0: 9475 6a56 0400 006a 8904 0000 6a49 0400  .ujV...j....jI..
-00004bc0: 006a 8504 0000 7562 6a76 0400 0029 8194  .j....ubjv...)..
-00004bd0: 7d94 286a 4004 0000 681f 6a41 0400 005d  }.(j@...h.jA...]
-00004be0: 9428 6a84 0400 0029 8194 7d94 286a 4004  .(j....)..}.(j@.
-00004bf0: 0000 681f 6a41 0400 005d 946a 8a04 0000  ..h.jA...].j....
-00004c00: 2981 947d 9428 6a40 0400 0068 1f6a 4104  )..}.(j@...h.jA.
-00004c10: 0000 5d94 6a8f 0400 0029 8194 7d94 286a  ..].j....)..}.(j
-00004c20: 4004 0000 681f 6a41 0400 005d 946a 4404  @...h.jA...].jD.
-00004c30: 0000 8c19 5365 676d 656e 7461 7469 6f6e  ....Segmentation
-00004c40: 2061 6e64 2054 7261 636b 696e 6794 8594   and Tracking...
-00004c50: 8194 7d94 286a 4004 0000 681f 6a49 0400  ..}.(j@...h.jI..
-00004c60: 006a af04 0000 7562 616a 4a04 0000 7d94  .j....ubajJ...}.
-00004c70: 286a 4c04 0000 5d94 6a4e 0400 005d 946a  (jL...].jN...].j
-00004c80: 5004 0000 5d94 6a52 0400 005d 946a 5404  P...].jR...].jT.
-00004c90: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-00004ca0: 8c06 7265 6675 7269 946a f203 0000 8c0a  ..refuri.j......
-00004cb0: 616e 6368 6f72 6e61 6d65 948c 1a23 7365  anchorname...#se
-00004cc0: 676d 656e 7461 7469 6f6e 2d61 6e64 2d74  gmentation-and-t
-00004cd0: 7261 636b 696e 6794 756a 5604 0000 6a8e  racking.ujV...j.
-00004ce0: 0400 006a 4904 0000 6aac 0400 0075 6261  ...jI...j....uba
-00004cf0: 6a4a 0400 007d 9428 6a4c 0400 005d 946a  jJ...}.(jL...].j
-00004d00: 4e04 0000 5d94 6a50 0400 005d 946a 5204  N...].jP...].jR.
-00004d10: 0000 5d94 6a54 0400 005d 9475 6a56 0400  ..].jT...].ujV..
-00004d20: 006a 8904 0000 6a49 0400 006a a904 0000  .j....jI...j....
-00004d30: 7562 616a 4a04 0000 7d94 286a 4c04 0000  ubajJ...}.(jL...
-00004d40: 5d94 6a4e 0400 005d 946a 5004 0000 5d94  ].jN...].jP...].
-00004d50: 6a52 0400 005d 946a 5404 0000 5d94 756a  jR...].jT...].uj
-00004d60: 5604 0000 6a83 0400 006a 4904 0000 6aa6  V...j....jI...j.
-00004d70: 0400 0075 626a 8404 0000 2981 947d 9428  ...ubj....)..}.(
-00004d80: 6a40 0400 0068 1f6a 4104 0000 5d94 6a8a  j@...h.jA...].j.
-00004d90: 0400 0029 8194 7d94 286a 4004 0000 681f  ...)..}.(j@...h.
-00004da0: 6a41 0400 005d 946a 8f04 0000 2981 947d  jA...].j....)..}
-00004db0: 9428 6a40 0400 0068 1f6a 4104 0000 5d94  .(j@...h.jA...].
-00004dc0: 6a44 0400 008c 0c50 6f69 6e74 2043 6c6f  jD.....Point Clo
-00004dd0: 7564 7394 8594 8194 7d94 286a 4004 0000  uds.....}.(j@...
-00004de0: 681f 6a49 0400 006a d204 0000 7562 616a  h.jI...j....ubaj
-00004df0: 4a04 0000 7d94 286a 4c04 0000 5d94 6a4e  J...}.(jL...].jN
-00004e00: 0400 005d 946a 5004 0000 5d94 6a52 0400  ...].jP...].jR..
-00004e10: 005d 946a 5404 0000 5d94 8c08 696e 7465  .].jT...]...inte
-00004e20: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00004e30: f203 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
-00004e40: 948c 0d23 706f 696e 742d 636c 6f75 6473  ...#point-clouds
-00004e50: 9475 6a56 0400 006a 8e04 0000 6a49 0400  .ujV...j....jI..
-00004e60: 006a cf04 0000 7562 616a 4a04 0000 7d94  .j....ubajJ...}.
-00004e70: 286a 4c04 0000 5d94 6a4e 0400 005d 946a  (jL...].jN...].j
-00004e80: 5004 0000 5d94 6a52 0400 005d 946a 5404  P...].jR...].jT.
-00004e90: 0000 5d94 756a 5604 0000 6a89 0400 006a  ..].ujV...j....j
-00004ea0: 4904 0000 6acc 0400 0075 6261 6a4a 0400  I...j....ubajJ..
-00004eb0: 007d 9428 6a4c 0400 005d 946a 4e04 0000  .}.(jL...].jN...
-00004ec0: 5d94 6a50 0400 005d 946a 5204 0000 5d94  ].jP...].jR...].
-00004ed0: 6a54 0400 005d 9475 6a56 0400 006a 8304  jT...].ujV...j..
-00004ee0: 0000 6a49 0400 006a a604 0000 7562 6a84  ..jI...j....ubj.
-00004ef0: 0400 0029 8194 7d94 286a 4004 0000 681f  ...)..}.(j@...h.
-00004f00: 6a41 0400 005d 946a 8a04 0000 2981 947d  jA...].j....)..}
-00004f10: 9428 6a40 0400 0068 1f6a 4104 0000 5d94  .(j@...h.jA...].
-00004f20: 6a8f 0400 0029 8194 7d94 286a 4004 0000  j....)..}.(j@...
-00004f30: 681f 6a41 0400 005d 946a 4404 0000 8c0b  h.jA...].jD.....
-00004f40: 4175 746f 656e 636f 6465 7294 8594 8194  Autoencoder.....
-00004f50: 7d94 286a 4004 0000 681f 6a49 0400 006a  }.(j@...h.jI...j
-00004f60: f504 0000 7562 616a 4a04 0000 7d94 286a  ....ubajJ...}.(j
-00004f70: 4c04 0000 5d94 6a4e 0400 005d 946a 5004  L...].jN...].jP.
-00004f80: 0000 5d94 6a52 0400 005d 946a 5404 0000  ..].jR...].jT...
-00004f90: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
-00004fa0: 7265 6675 7269 946a f203 0000 8c0a 616e  refuri.j......an
-00004fb0: 6368 6f72 6e61 6d65 948c 0c23 6175 746f  chorname...#auto
-00004fc0: 656e 636f 6465 7294 756a 5604 0000 6a8e  encoder.ujV...j.
-00004fd0: 0400 006a 4904 0000 6af2 0400 0075 6261  ...jI...j....uba
-00004fe0: 6a4a 0400 007d 9428 6a4c 0400 005d 946a  jJ...}.(jL...].j
-00004ff0: 4e04 0000 5d94 6a50 0400 005d 946a 5204  N...].jP...].jR.
-00005000: 0000 5d94 6a54 0400 005d 9475 6a56 0400  ..].jT...].ujV..
-00005010: 006a 8904 0000 6a49 0400 006a ef04 0000  .j....jI...j....
-00005020: 7562 616a 4a04 0000 7d94 286a 4c04 0000  ubajJ...}.(jL...
-00005030: 5d94 6a4e 0400 005d 946a 5004 0000 5d94  ].jN...].jP...].
-00005040: 6a52 0400 005d 946a 5404 0000 5d94 756a  jR...].jT...].uj
-00005050: 5604 0000 6a83 0400 006a 4904 0000 6aa6  V...j....jI...j.
-00005060: 0400 0075 626a 8404 0000 2981 947d 9428  ...ubj....)..}.(
-00005070: 6a40 0400 0068 1f6a 4104 0000 5d94 6a8a  j@...h.jA...].j.
-00005080: 0400 0029 8194 7d94 286a 4004 0000 681f  ...)..}.(j@...h.
-00005090: 6a41 0400 005d 946a 8f04 0000 2981 947d  jA...].j....)..}
-000050a0: 9428 6a40 0400 0068 1f6a 4104 0000 5d94  .(j@...h.jA...].
-000050b0: 6a44 0400 008c 0e53 6861 7065 2046 6561  jD.....Shape Fea
-000050c0: 7475 7265 7394 8594 8194 7d94 286a 4004  tures.....}.(j@.
-000050d0: 0000 681f 6a49 0400 006a 1805 0000 7562  ..h.jI...j....ub
-000050e0: 616a 4a04 0000 7d94 286a 4c04 0000 5d94  ajJ...}.(jL...].
-000050f0: 6a4e 0400 005d 946a 5004 0000 5d94 6a52  jN...].jP...].jR
-00005100: 0400 005d 946a 5404 0000 5d94 8c08 696e  ...].jT...]...in
-00005110: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
-00005120: 946a f203 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
-00005130: 6d65 948c 0f23 7368 6170 652d 6665 6174  me...#shape-feat
-00005140: 7572 6573 9475 6a56 0400 006a 8e04 0000  ures.ujV...j....
-00005150: 6a49 0400 006a 1505 0000 7562 616a 4a04  jI...j....ubajJ.
-00005160: 0000 7d94 286a 4c04 0000 5d94 6a4e 0400  ..}.(jL...].jN..
-00005170: 005d 946a 5004 0000 5d94 6a52 0400 005d  .].jP...].jR...]
-00005180: 946a 5404 0000 5d94 756a 5604 0000 6a89  .jT...].ujV...j.
-00005190: 0400 006a 4904 0000 6a12 0500 0075 6261  ...jI...j....uba
-000051a0: 6a4a 0400 007d 9428 6a4c 0400 005d 946a  jJ...}.(jL...].j
-000051b0: 4e04 0000 5d94 6a50 0400 005d 946a 5204  N...].jP...].jR.
-000051c0: 0000 5d94 6a54 0400 005d 9475 6a56 0400  ..].jT...].ujV..
-000051d0: 006a 8304 0000 6a49 0400 006a a604 0000  .j....jI...j....
-000051e0: 7562 6a84 0400 0029 8194 7d94 286a 4004  ubj....)..}.(j@.
-000051f0: 0000 681f 6a41 0400 005d 946a 8a04 0000  ..h.jA...].j....
-00005200: 2981 947d 9428 6a40 0400 0068 1f6a 4104  )..}.(j@...h.jA.
-00005210: 0000 5d94 6a8f 0400 0029 8194 7d94 286a  ..].j....)..}.(j
-00005220: 4004 0000 681f 6a41 0400 005d 946a 4404  @...h.jA...].jD.
-00005230: 0000 8c10 4479 6e61 6d69 6320 4665 6174  ....Dynamic Feat
-00005240: 7572 6573 9485 9481 947d 9428 6a40 0400  ures.....}.(j@..
-00005250: 0068 1f6a 4904 0000 6a3b 0500 0075 6261  .h.jI...j;...uba
-00005260: 6a4a 0400 007d 9428 6a4c 0400 005d 946a  jJ...}.(jL...].j
-00005270: 4e04 0000 5d94 6a50 0400 005d 946a 5204  N...].jP...].jR.
-00005280: 0000 5d94 6a54 0400 005d 948c 0869 6e74  ..].jT...]...int
-00005290: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
-000052a0: 6af2 0300 008c 0a61 6e63 686f 726e 616d  j......anchornam
-000052b0: 6594 8c11 2364 796e 616d 6963 2d66 6561  e...#dynamic-fea
-000052c0: 7475 7265 7394 756a 5604 0000 6a8e 0400  tures.ujV...j...
-000052d0: 006a 4904 0000 6a38 0500 0075 6261 6a4a  .jI...j8...ubajJ
-000052e0: 0400 007d 9428 6a4c 0400 005d 946a 4e04  ...}.(jL...].jN.
-000052f0: 0000 5d94 6a50 0400 005d 946a 5204 0000  ..].jP...].jR...
-00005300: 5d94 6a54 0400 005d 9475 6a56 0400 006a  ].jT...].ujV...j
-00005310: 8904 0000 6a49 0400 006a 3505 0000 7562  ....jI...j5...ub
-00005320: 616a 4a04 0000 7d94 286a 4c04 0000 5d94  ajJ...}.(jL...].
-00005330: 6a4e 0400 005d 946a 5004 0000 5d94 6a52  jN...].jP...].jR
-00005340: 0400 005d 946a 5404 0000 5d94 756a 5604  ...].jT...].ujV.
-00005350: 0000 6a83 0400 006a 4904 0000 6aa6 0400  ..j....jI...j...
-00005360: 0075 6265 6a4a 0400 007d 9428 6a4c 0400  .ubejJ...}.(jL..
-00005370: 005d 946a 4e04 0000 5d94 6a50 0400 005d  .].jN...].jP...]
-00005380: 946a 5204 0000 5d94 6a54 0400 005d 9475  .jR...].jT...].u
-00005390: 6a56 0400 006a 7504 0000 6a49 0400 006a  jV...ju...jI...j
-000053a0: 8504 0000 7562 656a 4a04 0000 7d94 286a  ....ubejJ...}.(j
-000053b0: 4c04 0000 5d94 6a4e 0400 005d 946a 5004  L...].jN...].jP.
-000053c0: 0000 5d94 6a52 0400 005d 946a 5404 0000  ..].jR...].jT...
-000053d0: 5d94 756a 5604 0000 6a83 0400 006a 4904  ].ujV...j....jI.
-000053e0: 0000 6a80 0400 0075 6261 6a4a 0400 007d  ..j....ubajJ...}
-000053f0: 9428 6a4c 0400 005d 946a 4e04 0000 5d94  .(jL...].jN...].
-00005400: 6a50 0400 005d 946a 5204 0000 5d94 6a54  jP...].jR...].jT
-00005410: 0400 005d 9475 6a56 0400 006a 7504 0000  ...].ujV...ju...
-00005420: 7562 6af0 0300 006a 7604 0000 2981 947d  ubj....jv...)..}
-00005430: 9428 6a40 0400 0068 1f6a 4104 0000 5d94  .(j@...h.jA...].
-00005440: 286a 8404 0000 2981 947d 9428 6a40 0400  (j....)..}.(j@..
-00005450: 0068 1f6a 4104 0000 5d94 286a 8a04 0000  .h.jA...].(j....
-00005460: 2981 947d 9428 6a40 0400 0068 1f6a 4104  )..}.(j@...h.jA.
-00005470: 0000 5d94 6a8f 0400 0029 8194 7d94 286a  ..].j....)..}.(j
-00005480: 4004 0000 681f 6a41 0400 005d 946a 4404  @...h.jA...].jD.
-00005490: 0000 8c18 766f 6c6c 7365 672d 6e61 7061  ....vollseg-napa
-000054a0: 7269 2d74 7261 636b 6d61 7465 9485 9481  ri-trackmate....
-000054b0: 947d 9428 6a40 0400 0068 1f6a 4904 0000  .}.(j@...h.jI...
-000054c0: 6a73 0500 0075 6261 6a4a 0400 007d 9428  js...ubajJ...}.(
-000054d0: 6a4c 0400 005d 946a 4e04 0000 5d94 6a50  jL...].jN...].jP
-000054e0: 0400 005d 946a 5204 0000 5d94 6a54 0400  ...].jR...].jT..
-000054f0: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
-00005500: 0672 6566 7572 6994 6af0 0300 008c 0a61  .refuri.j......a
-00005510: 6e63 686f 726e 616d 6594 681f 756a 5604  nchorname.h.ujV.
-00005520: 0000 6a8e 0400 006a 4904 0000 6a70 0500  ..j....jI...jp..
-00005530: 0075 6261 6a4a 0400 007d 9428 6a4c 0400  .ubajJ...}.(jL..
-00005540: 005d 946a 4e04 0000 5d94 6a50 0400 005d  .].jN...].jP...]
-00005550: 946a 5204 0000 5d94 6a54 0400 005d 9475  .jR...].jT...].u
-00005560: 6a56 0400 006a 8904 0000 6a49 0400 006a  jV...j....jI...j
-00005570: 6d05 0000 7562 6a76 0400 0029 8194 7d94  m...ubjv...)..}.
-00005580: 286a 4004 0000 681f 6a41 0400 005d 9428  (j@...h.jA...].(
-00005590: 6a84 0400 0029 8194 7d94 286a 4004 0000  j....)..}.(j@...
-000055a0: 681f 6a41 0400 005d 946a 8a04 0000 2981  h.jA...].j....).
-000055b0: 947d 9428 6a40 0400 0068 1f6a 4104 0000  .}.(j@...h.jA...
-000055c0: 5d94 6a8f 0400 0029 8194 7d94 286a 4004  ].j....)..}.(j@.
-000055d0: 0000 681f 6a41 0400 005d 946a 4404 0000  ..h.jA...].jD...
-000055e0: 8c0c 496e 7374 616c 6c61 7469 6f6e 9485  ..Installation..
-000055f0: 9481 947d 9428 6a40 0400 0068 1f6a 4904  ...}.(j@...h.jI.
-00005600: 0000 6a92 0500 0075 6261 6a4a 0400 007d  ..j....ubajJ...}
-00005610: 9428 6a4c 0400 005d 946a 4e04 0000 5d94  .(jL...].jN...].
-00005620: 6a50 0400 005d 946a 5204 0000 5d94 6a54  jP...].jR...].jT
-00005630: 0400 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-00005640: 888c 0672 6566 7572 6994 6af0 0300 008c  ...refuri.j.....
-00005650: 0a61 6e63 686f 726e 616d 6594 8c0d 2369  .anchorname...#i
-00005660: 6e73 7461 6c6c 6174 696f 6e94 756a 5604  nstallation.ujV.
-00005670: 0000 6a8e 0400 006a 4904 0000 6a8f 0500  ..j....jI...j...
-00005680: 0075 6261 6a4a 0400 007d 9428 6a4c 0400  .ubajJ...}.(jL..
-00005690: 005d 946a 4e04 0000 5d94 6a50 0400 005d  .].jN...].jP...]
-000056a0: 946a 5204 0000 5d94 6a54 0400 005d 9475  .jR...].jT...].u
-000056b0: 6a56 0400 006a 8904 0000 6a49 0400 006a  jV...j....jI...j
-000056c0: 8c05 0000 7562 616a 4a04 0000 7d94 286a  ....ubajJ...}.(j
-000056d0: 4c04 0000 5d94 6a4e 0400 005d 946a 5004  L...].jN...].jP.
-000056e0: 0000 5d94 6a52 0400 005d 946a 5404 0000  ..].jR...].jT...
-000056f0: 5d94 756a 5604 0000 6a83 0400 006a 4904  ].ujV...j....jI.
-00005700: 0000 6a89 0500 0075 626a 8404 0000 2981  ..j....ubj....).
-00005710: 947d 9428 6a40 0400 0068 1f6a 4104 0000  .}.(j@...h.jA...
-00005720: 5d94 6a8a 0400 0029 8194 7d94 286a 4004  ].j....)..}.(j@.
-00005730: 0000 681f 6a41 0400 005d 946a 8f04 0000  ..h.jA...].j....
-00005740: 2981 947d 9428 6a40 0400 0068 1f6a 4104  )..}.(j@...h.jA.
-00005750: 0000 5d94 6a44 0400 008c 0c43 6f6e 7472  ..].jD.....Contr
-00005760: 6962 7574 696e 6794 8594 8194 7d94 286a  ibuting.....}.(j
-00005770: 4004 0000 681f 6a49 0400 006a b505 0000  @...h.jI...j....
-00005780: 7562 616a 4a04 0000 7d94 286a 4c04 0000  ubajJ...}.(jL...
-00005790: 5d94 6a4e 0400 005d 946a 5004 0000 5d94  ].jN...].jP...].
-000057a0: 6a52 0400 005d 946a 5404 0000 5d94 8c08  jR...].jT...]...
-000057b0: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
-000057c0: 7269 946a f003 0000 8c0a 616e 6368 6f72  ri.j......anchor
-000057d0: 6e61 6d65 948c 0d23 636f 6e74 7269 6275  name...#contribu
-000057e0: 7469 6e67 9475 6a56 0400 006a 8e04 0000  ting.ujV...j....
-000057f0: 6a49 0400 006a b205 0000 7562 616a 4a04  jI...j....ubajJ.
-00005800: 0000 7d94 286a 4c04 0000 5d94 6a4e 0400  ..}.(jL...].jN..
-00005810: 005d 946a 5004 0000 5d94 6a52 0400 005d  .].jP...].jR...]
-00005820: 946a 5404 0000 5d94 756a 5604 0000 6a89  .jT...].ujV...j.
-00005830: 0400 006a 4904 0000 6aaf 0500 0075 6261  ...jI...j....uba
-00005840: 6a4a 0400 007d 9428 6a4c 0400 005d 946a  jJ...}.(jL...].j
-00005850: 4e04 0000 5d94 6a50 0400 005d 946a 5204  N...].jP...].jR.
-00005860: 0000 5d94 6a54 0400 005d 9475 6a56 0400  ..].jT...].ujV..
-00005870: 006a 8304 0000 6a49 0400 006a 8905 0000  .j....jI...j....
-00005880: 7562 6a84 0400 0029 8194 7d94 286a 4004  ubj....)..}.(j@.
-00005890: 0000 681f 6a41 0400 005d 946a 8a04 0000  ..h.jA...].j....
-000058a0: 2981 947d 9428 6a40 0400 0068 1f6a 4104  )..}.(j@...h.jA.
-000058b0: 0000 5d94 6a8f 0400 0029 8194 7d94 286a  ..].j....)..}.(j
-000058c0: 4004 0000 681f 6a41 0400 005d 946a 4404  @...h.jA...].jD.
-000058d0: 0000 8c07 4c69 6365 6e73 6594 8594 8194  ....License.....
-000058e0: 7d94 286a 4004 0000 681f 6a49 0400 006a  }.(j@...h.jI...j
-000058f0: d805 0000 7562 616a 4a04 0000 7d94 286a  ....ubajJ...}.(j
-00005900: 4c04 0000 5d94 6a4e 0400 005d 946a 5004  L...].jN...].jP.
-00005910: 0000 5d94 6a52 0400 005d 946a 5404 0000  ..].jR...].jT...
-00005920: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
-00005930: 7265 6675 7269 946a f003 0000 8c0a 616e  refuri.j......an
-00005940: 6368 6f72 6e61 6d65 948c 0823 6c69 6365  chorname...#lice
-00005950: 6e73 6594 756a 5604 0000 6a8e 0400 006a  nse.ujV...j....j
-00005960: 4904 0000 6ad5 0500 0075 6261 6a4a 0400  I...j....ubajJ..
-00005970: 007d 9428 6a4c 0400 005d 946a 4e04 0000  .}.(jL...].jN...
-00005980: 5d94 6a50 0400 005d 946a 5204 0000 5d94  ].jP...].jR...].
-00005990: 6a54 0400 005d 9475 6a56 0400 006a 8904  jT...].ujV...j..
-000059a0: 0000 6a49 0400 006a d205 0000 7562 616a  ..jI...j....ubaj
-000059b0: 4a04 0000 7d94 286a 4c04 0000 5d94 6a4e  J...}.(jL...].jN
-000059c0: 0400 005d 946a 5004 0000 5d94 6a52 0400  ...].jP...].jR..
-000059d0: 005d 946a 5404 0000 5d94 756a 5604 0000  .].jT...].ujV...
-000059e0: 6a83 0400 006a 4904 0000 6a89 0500 0075  j....jI...j....u
-000059f0: 626a 8404 0000 2981 947d 9428 6a40 0400  bj....)..}.(j@..
-00005a00: 0068 1f6a 4104 0000 5d94 6a8a 0400 0029  .h.jA...].j....)
-00005a10: 8194 7d94 286a 4004 0000 681f 6a41 0400  ..}.(j@...h.jA..
-00005a20: 005d 946a 8f04 0000 2981 947d 9428 6a40  .].j....)..}.(j@
-00005a30: 0400 0068 1f6a 4104 0000 5d94 6a44 0400  ...h.jA...].jD..
-00005a40: 008c 0649 7373 7565 7394 8594 8194 7d94  ...Issues.....}.
-00005a50: 286a 4004 0000 681f 6a49 0400 006a fb05  (j@...h.jI...j..
-00005a60: 0000 7562 616a 4a04 0000 7d94 286a 4c04  ..ubajJ...}.(jL.
-00005a70: 0000 5d94 6a4e 0400 005d 946a 5004 0000  ..].jN...].jP...
-00005a80: 5d94 6a52 0400 005d 946a 5404 0000 5d94  ].jR...].jT...].
-00005a90: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-00005aa0: 6675 7269 946a f003 0000 8c0a 616e 6368  furi.j......anch
-00005ab0: 6f72 6e61 6d65 948c 0723 6973 7375 6573  orname...#issues
-00005ac0: 9475 6a56 0400 006a 8e04 0000 6a49 0400  .ujV...j....jI..
-00005ad0: 006a f805 0000 7562 616a 4a04 0000 7d94  .j....ubajJ...}.
-00005ae0: 286a 4c04 0000 5d94 6a4e 0400 005d 946a  (jL...].jN...].j
-00005af0: 5004 0000 5d94 6a52 0400 005d 946a 5404  P...].jR...].jT.
-00005b00: 0000 5d94 756a 5604 0000 6a89 0400 006a  ..].ujV...j....j
-00005b10: 4904 0000 6af5 0500 0075 6261 6a4a 0400  I...j....ubajJ..
-00005b20: 007d 9428 6a4c 0400 005d 946a 4e04 0000  .}.(jL...].jN...
-00005b30: 5d94 6a50 0400 005d 946a 5204 0000 5d94  ].jP...].jR...].
-00005b40: 6a54 0400 005d 9475 6a56 0400 006a 8304  jT...].ujV...j..
-00005b50: 0000 6a49 0400 006a 8905 0000 7562 656a  ..jI...j....ubej
-00005b60: 4a04 0000 7d94 286a 4c04 0000 5d94 6a4e  J...}.(jL...].jN
-00005b70: 0400 005d 946a 5004 0000 5d94 6a52 0400  ...].jP...].jR..
-00005b80: 005d 946a 5404 0000 5d94 756a 5604 0000  .].jT...].ujV...
-00005b90: 6a75 0400 006a 4904 0000 6a6d 0500 0075  ju...jI...jm...u
-00005ba0: 6265 6a4a 0400 007d 9428 6a4c 0400 005d  bejJ...}.(jL...]
-00005bb0: 946a 4e04 0000 5d94 6a50 0400 005d 946a  .jN...].jP...].j
-00005bc0: 5204 0000 5d94 6a54 0400 005d 9475 6a56  R...].jT...].ujV
-00005bd0: 0400 006a 8304 0000 6a49 0400 006a 6a05  ...j....jI...jj.
-00005be0: 0000 7562 6a88 0400 008c 0774 6f63 7472  ..ubj......toctr
-00005bf0: 6565 9493 9429 8194 7d94 286a 4004 0000  ee...)..}.(j@...
-00005c00: 681f 6a41 0400 005d 946a 4a04 0000 7d94  h.jA...].jJ...}.
-00005c10: 286a 4c04 0000 5d94 6a4e 0400 005d 946a  (jL...].jN...].j
-00005c20: 5004 0000 5d94 6a52 0400 005d 946a 5404  P...].jR...].jT.
-00005c30: 0000 5d94 8c06 7061 7265 6e74 946a f003  ..]...parent.j..
-00005c40: 0000 8c07 656e 7472 6965 7394 5d94 4e8c  ....entries.].N.
-00005c50: 0941 4c47 4f52 4954 484d 9486 9461 8c0c  .ALGORITHM...a..
-00005c60: 696e 636c 7564 6566 696c 6573 945d 946a  includefiles.].j
-00005c70: 3206 0000 618c 086d 6178 6465 7074 6894  2...a..maxdepth.
-00005c80: 4aff ffff ff8c 0763 6170 7469 6f6e 944e  J......caption.N
-00005c90: 8c0a 7261 7763 6170 7469 6f6e 9468 1f8c  ..rawcaption.h..
-00005ca0: 0467 6c6f 6294 898c 0668 6964 6465 6e94  .glob....hidden.
-00005cb0: 888c 0d69 6e63 6c75 6465 6869 6464 656e  ...includehidden
-00005cc0: 9489 8c08 6e75 6d62 6572 6564 944b 008c  ....numbered.K..
-00005cd0: 0a74 6974 6c65 736f 6e6c 7994 8875 6a56  .titlesonly..ujV
-00005ce0: 0400 006a 2406 0000 8c06 736f 7572 6365  ...j$.....source
-00005cf0: 948c 502f 6d6e 742f 632f 5573 6572 732f  ..P/mnt/c/Users/
-00005d00: 7261 6e64 6f2f 446f 776e 6c6f 6164 732f  rando/Downloads/
-00005d10: 5079 7468 6f6e 5f57 6f72 6b73 7061 6365  Python_Workspace
-00005d20: 2f76 6f6c 6c73 6567 2d6e 6170 6172 692d  /vollseg-napari-
-00005d30: 7472 6163 6b6d 6174 652f 5245 4144 4d45  trackmate/README
-00005d40: 2e6d 6494 8c04 6c69 6e65 944b 016a 4904  .md...line.K.jI.
-00005d50: 0000 6a6a 0500 0075 6265 6a4a 0400 007d  ..jj...ubejJ...}
-00005d60: 9428 6a4c 0400 005d 946a 4e04 0000 5d94  .(jL...].jN...].
-00005d70: 6a50 0400 005d 946a 5204 0000 5d94 6a54  jP...].jR...].jT
-00005d80: 0400 005d 9475 6a56 0400 006a 7504 0000  ...].ujV...ju...
-00005d90: 7562 758c 0f74 6f63 5f6e 756d 5f65 6e74  ubu..toc_num_ent
-00005da0: 7269 6573 947d 9428 6af1 0300 004b 006a  ries.}.(j....K.j
-00005db0: f203 0000 4b06 6af0 0300 004b 0575 8c0e  ....K.j....K.u..
-00005dc0: 746f 635f 7365 636e 756d 6265 7273 947d  toc_secnumbers.}
-00005dd0: 948c 0e74 6f63 5f66 6967 6e75 6d62 6572  ...toc_fignumber
-00005de0: 7394 7d94 8c10 746f 6374 7265 655f 696e  s.}...toctree_in
-00005df0: 636c 7564 6573 947d 946a f003 0000 5d94  cludes.}.j....].
-00005e00: 6a32 0600 0061 738c 1066 696c 6573 5f74  j2...as..files_t
-00005e10: 6f5f 7265 6275 696c 6494 7d94 6a32 0600  o_rebuild.}.j2..
-00005e20: 008f 9428 6af0 0300 0090 738c 0d67 6c6f  ...(j.....s..glo
-00005e30: 625f 746f 6374 7265 6573 948f 948c 116e  b_toctrees.....n
-00005e40: 756d 6265 7265 645f 746f 6374 7265 6573  umbered_toctrees
-00005e50: 948f 948c 0a64 6f6d 6169 6e64 6174 6194  .....domaindata.
-00005e60: 7d94 288c 0163 947d 9428 8c0b 726f 6f74  }.(..c.}.(..root
-00005e70: 5f73 796d 626f 6c94 6af4 0300 008c 0653  _symbol.j......S
-00005e80: 796d 626f 6c94 9394 2981 947d 9428 6a49  ymbol...)..}.(jI
-00005e90: 0400 004e 8c0c 7369 626c 696e 6741 626f  ...N..siblingAbo
-00005ea0: 7665 944e 8c0c 7369 626c 696e 6742 656c  ve.N..siblingBel
-00005eb0: 6f77 944e 8c05 6964 656e 7494 4e8c 0b64  ow.N..ident.N..d
-00005ec0: 6563 6c61 7261 7469 6f6e 944e 68a5 4e6a  eclaration.Nh.Nj
-00005ed0: 4006 0000 4e8c 0f69 7352 6564 6563 6c61  @...N..isRedecla
-00005ee0: 7261 7469 6f6e 9489 8c09 5f63 6869 6c64  ration...._child
-00005ef0: 7265 6e94 5d94 8c0d 5f61 6e6f 6e43 6869  ren.]..._anonChi
-00005f00: 6c64 7265 6e94 5d94 7562 8c07 6f62 6a65  ldren.].ub..obje
-00005f10: 6374 7394 7d94 68dc 4b00 758c 0963 6861  cts.}.h.K.u..cha
-00005f20: 6e67 6573 6574 947d 9428 8c07 6368 616e  ngeset.}.(..chan
-00005f30: 6765 7394 7d94 68dc 4b00 758c 0863 6974  ges.}.h.K.u..cit
-00005f40: 6174 696f 6e94 7d94 2868 dc4b 008c 0963  ation.}.(h.K...c
-00005f50: 6974 6174 696f 6e73 947d 948c 0d63 6974  itations.}...cit
-00005f60: 6174 696f 6e5f 7265 6673 947d 9475 8c03  ation_refs.}.u..
-00005f70: 6370 7094 7d94 286a 5b06 0000 6af7 0300  cpp.}.(j[...j...
-00005f80: 006a 5c06 0000 9394 2981 947d 9428 6a49  .j\.....)..}.(jI
-00005f90: 0400 004e 6a60 0600 004e 6a61 0600 004e  ...Nj`...Nja...N
-00005fa0: 8c09 6964 656e 744f 724f 7094 4e8c 0e74  ..identOrOp.N..t
-00005fb0: 656d 706c 6174 6550 6172 616d 7394 4e8c  emplateParams.N.
-00005fc0: 0c74 656d 706c 6174 6541 7267 7394 4e6a  .templateArgs.Nj
-00005fd0: 6306 0000 4e68 a54e 6a40 0600 004e 6a64  c...Nh.Nj@...Njd
-00005fe0: 0600 0089 6a65 0600 005d 946a 6706 0000  ....je...].jg...
-00005ff0: 5d94 7562 6a50 0400 007d 9468 dc4b 0075  ].ubjP...}.h.K.u
-00006000: 8c05 696e 6465 7894 7d94 2868 dc4b 008c  ..index.}.(h.K..
-00006010: 0765 6e74 7269 6573 947d 9428 6af1 0300  .entries.}.(j...
-00006020: 005d 946a f203 0000 5d94 6af0 0300 005d  .].j....].j....]
-00006030: 9475 758c 026a 7394 7d94 286a 6906 0000  .uu..js.}.(ji...
-00006040: 7d94 8c07 6d6f 6475 6c65 7394 7d94 68dc  }...modules.}.h.
-00006050: 4b00 758c 046d 6174 6894 7d94 286a 6906  K.u..math.}.(ji.
-00006060: 0000 7d94 8c0d 6861 735f 6571 7561 7469  ..}...has_equati
-00006070: 6f6e 7394 7d94 286a f103 0000 896a f203  ons.}.(j.....j..
-00006080: 0000 896a f003 0000 8975 68dc 4b00 756a  ...j.....uh.K.uj
-00006090: 1e01 0000 7d94 286a 6906 0000 7d94 6a8a  ....}.(ji...}.j.
-000060a0: 0600 007d 9468 dc4b 0075 8c03 7273 7494  ...}.h.K.u..rst.
-000060b0: 7d94 286a 6906 0000 7d94 68dc 4b00 758c  }.(ji...}.h.K.u.
-000060c0: 0373 7464 947d 9428 8c0b 7072 6f67 6f70  .std.}.(..progop
-000060d0: 7469 6f6e 7394 7d94 6a69 0600 007d 948c  tions.}.ji...}..
-000060e0: 066c 6162 656c 7394 7d94 288c 0867 656e  .labels.}.(..gen
-000060f0: 696e 6465 7894 6a9e 0600 0068 1f8c 0d73  index.j....h...s
-00006100: 7068 696e 782e 6c6f 6361 6c65 948c 115f  phinx.locale..._
-00006110: 5472 616e 736c 6174 696f 6e50 726f 7879  TranslationProxy
-00006120: 9493 9428 6a9f 0600 008c 0f5f 6c61 7a79  ...(j......_lazy
-00006130: 5f74 7261 6e73 6c61 7465 9493 9468 138c  _translate...h..
-00006140: 0767 656e 6572 616c 948c 0549 6e64 6578  .general...Index
-00006150: 9474 9481 946a a306 0000 6813 6aa4 0600  .t...j....h.j...
-00006160: 006a a506 0000 8794 8694 6287 948c 086d  .j........b....m
-00006170: 6f64 696e 6465 7894 8c0b 7079 2d6d 6f64  odindex...py-mod
-00006180: 696e 6465 7894 681f 6aa1 0600 0028 6aa3  index.h.j....(j.
-00006190: 0600 0068 136a a406 0000 8c0c 4d6f 6475  ...h.j......Modu
-000061a0: 6c65 2049 6e64 6578 9474 9481 946a a306  le Index.t...j..
-000061b0: 0000 6813 6aa4 0600 006a ad06 0000 8794  ..h.j....j......
-000061c0: 8694 6287 948c 0673 6561 7263 6894 6ab3  ..b....search.j.
-000061d0: 0600 0068 1f6a a106 0000 286a a306 0000  ...h.j....(j....
-000061e0: 6813 6aa4 0600 008c 0b53 6561 7263 6820  h.j......Search 
-000061f0: 5061 6765 9474 9481 946a a306 0000 6813  Page.t...j....h.
-00006200: 6aa4 0600 006a b406 0000 8794 8694 6287  j....j........b.
-00006210: 948c 0b70 792d 6d6f 6469 6e64 6578 946a  ...py-modindex.j
-00006220: ba06 0000 681f 8c13 5079 7468 6f6e 204d  ....h...Python M
-00006230: 6f64 756c 6520 496e 6465 7894 8794 758c  odule Index...u.
-00006240: 0a61 6e6f 6e6c 6162 656c 7394 7d94 286a  .anonlabels.}.(j
-00006250: 9e06 0000 6a9e 0600 0068 1f86 946a ab06  ....j....h...j..
-00006260: 0000 6aac 0600 0068 1f86 946a b306 0000  ..j....h...j....
-00006270: 6ab3 0600 0068 1f86 946a ba06 0000 6aba  j....h...j....j.
-00006280: 0600 0068 1f86 9475 68dc 4b00 8c05 7465  ...h...uh.K...te
-00006290: 726d 7394 7d94 758c 0465 7661 6c94 7d94  rms.}.u..eval.}.
-000062a0: 68dc 4b01 738c 0467 6c75 6594 7d94 68dc  h.K.s..glue.}.h.
-000062b0: 4b01 738c 0463 6974 6594 7d94 288c 0762  K.s..cite.}.(..b
-000062c0: 6962 6461 7461 948c 1c73 7068 696e 7863  ibdata...sphinxc
-000062d0: 6f6e 7472 6962 2e62 6962 7465 782e 6269  ontrib.bibtex.bi
-000062e0: 6266 696c 6594 8c07 4269 6244 6174 6194  bfile...BibData.
-000062f0: 9394 6acd 0300 007d 948c 552f 6d6e 742f  ..j....}..U/mnt/
-00006300: 632f 5573 6572 732f 7261 6e64 6f2f 446f  c/Users/rando/Do
-00006310: 776e 6c6f 6164 732f 5079 7468 6f6e 5f57  wnloads/Python_W
-00006320: 6f72 6b73 7061 6365 2f76 6f6c 6c73 6567  orkspace/vollseg
-00006330: 2d6e 6170 6172 692d 7472 6163 6b6d 6174  -napari-trackmat
-00006340: 652f 7265 6665 7265 6e63 6573 2e62 6962  e/references.bib
-00006350: 946a cc06 0000 8c07 4269 6246 696c 6594  .j......BibFile.
-00006360: 9394 47ff f000 0000 0000 007d 9486 9481  ..G........}....
-00006370: 9473 8c0f 7079 6274 6578 2e64 6174 6162  .s..pybtex.datab
-00006380: 6173 6594 8c10 4269 626c 696f 6772 6170  ase...Bibliograp
-00006390: 6879 4461 7461 9493 9429 8194 7d94 286a  hyData...)..}.(j
-000063a0: 8206 0000 8c0c 7079 6274 6578 2e75 7469  ......pybtex.uti
-000063b0: 6c73 948c 1a4f 7264 6572 6564 4361 7365  ls...OrderedCase
-000063c0: 496e 7365 6e73 6974 6976 6544 6963 7494  InsensitiveDict.
-000063d0: 9394 2981 947d 9428 8c05 5f64 6963 7494  ..)..}.(.._dict.
-000063e0: 7d94 8c05 5f6b 6579 7394 6887 2952 9475  }..._keys.h.)R.u
-000063f0: 628c 0e63 726f 7373 7265 665f 636f 756e  b..crossref_coun
-00006400: 7494 6adb 0600 008c 1a43 6173 6549 6e73  t.j......CaseIns
-00006410: 656e 7369 7469 7665 4465 6661 756c 7444  ensitiveDefaultD
-00006420: 6963 7494 9394 2981 947d 9428 6ae0 0600  ict...)..}.(j...
-00006430: 007d 946a e206 0000 7d94 8c0f 6465 6661  .}.j....}...defa
-00006440: 756c 745f 6661 6374 6f72 7994 6a1e 0400  ult_factory.j...
-00006450: 008c 0369 6e74 9493 9475 628c 0d6d 696e  ...int...ub..min
-00006460: 5f63 726f 7373 7265 6673 944b 028c 095f  _crossrefs.K..._
-00006470: 7072 6561 6d62 6c65 945d 948c 0e77 616e  preamble.]...wan
-00006480: 7465 645f 656e 7472 6965 7394 4e6a 7106  ted_entries.Njq.
-00006490: 0000 6adb 0600 008c 1243 6173 6549 6e73  ..j......CaseIns
-000064a0: 656e 7369 7469 7665 5365 7494 9394 2981  ensitiveSet...).
-000064b0: 947d 9428 8c04 5f73 6574 948f 946a e206  .}.(.._set...j..
-000064c0: 0000 7d94 7562 7562 8794 8194 8c13 6269  ..}.ubub......bi
-000064d0: 626c 696f 6772 6170 6879 5f68 6561 6465  bliography_heade
-000064e0: 7294 6a3c 0400 008c 0963 6f6e 7461 696e  r.j<.....contain
-000064f0: 6572 9493 9429 8194 7d94 286a 4004 0000  er...)..}.(j@...
-00006500: 681f 6a41 0400 005d 946a 4a04 0000 7d94  h.jA...].jJ...}.
-00006510: 286a 4c04 0000 5d94 6a4e 0400 005d 946a  (jL...].jN...].j
-00006520: 5004 0000 5d94 6a52 0400 005d 946a 5404  P...].jR...].jT.
-00006530: 0000 5d94 756a 5604 0000 6afc 0600 0075  ..].ujV...j....u
-00006540: 628c 0e62 6962 6c69 6f67 7261 7068 6965  b..bibliographie
-00006550: 7394 7d94 6a71 0600 005d 946a 7306 0000  s.}.jq...].js...
-00006560: 5d94 68dc 4b04 758c 0866 6f6f 7463 6974  ].h.K.u..footcit
-00006570: 6594 7d94 286a fb06 0000 6afd 0600 0029  e.}.(j....j....)
-00006580: 8194 7d94 286a 4004 0000 681f 6a41 0400  ..}.(j@...h.jA..
-00006590: 005d 946a 4a04 0000 7d94 286a 4c04 0000  .].jJ...}.(jL...
-000065a0: 5d94 6a4e 0400 005d 946a 5004 0000 5d94  ].jN...].jP...].
-000065b0: 6a52 0400 005d 946a 5404 0000 5d94 756a  jR...].jT...].uj
-000065c0: 5604 0000 6afc 0600 0075 6268 dc4b 0075  V...j....ubh.K.u
-000065d0: 758c 0669 6d61 6765 7394 8c0b 7370 6869  u..images...sphi
-000065e0: 6e78 2e75 7469 6c94 8c10 4669 6c65 6e61  nx.util...Filena
-000065f0: 6d65 556e 6971 4469 6374 9493 9429 8194  meUniqDict...)..
-00006600: 6a24 0400 008f 9428 6af2 0300 0090 8c19  j$.....(j.......
-00006610: 706f 696e 745f 636c 6f75 6473 5f63 6f6d  point_clouds_com
-00006620: 7061 7265 642e 706e 6794 8694 738f 9428  pared.png...s..(
-00006630: 6a1c 0700 0090 628c 0764 6c66 696c 6573  j.....b..dlfiles
-00006640: 946a 1707 0000 8c0d 446f 776e 6c6f 6164  .j......Download
-00006650: 4669 6c65 7394 9394 2981 9428 6a26 0400  Files...)..(j&..
-00006660: 008f 9428 6af2 0300 0090 8c3a 6337 3464  ...(j......:c74d
-00006670: 6131 3336 3039 6638 3164 6362 3934 6437  a13609f81dcb94d7
-00006680: 3466 3838 3332 3763 3662 3037 2f76 6973  4f88327c6b07/vis
-00006690: 7561 6c69 7a65 5f70 6f69 6e74 5f63 6c6f  ualize_point_clo
-000066a0: 7564 732e 7079 9486 946a 2504 0000 8f94  uds.py...j%.....
-000066b0: 286a f203 0000 908c 3537 3330 3433 3232  (j......57304322
-000066c0: 3532 3265 6233 3362 3463 3164 3666 6364  522eb33b4c1d6fcd
-000066d0: 3962 3864 6163 3061 662f 6170 706c 795f  9b8dac0af/apply_
-000066e0: 6175 746f 656e 636f 6465 722e 7079 9486  autoencoder.py..
-000066f0: 9475 8c12 6f72 6967 696e 616c 5f69 6d61  .u..original_ima
-00006700: 6765 5f75 7269 947d 948c 0974 656d 705f  ge_uri.}...temp_
-00006710: 6461 7461 947d 948c 0b72 6566 5f63 6f6e  data.}...ref_con
-00006720: 7465 7874 947d 948c 0b6d 7973 745f 636f  text.}...myst_co
-00006730: 6e66 6967 948c 176d 7973 745f 7061 7273  nfig...myst_pars
-00006740: 6572 2e63 6f6e 6669 672e 6d61 696e 948c  er.config.main..
-00006750: 0e4d 6450 6172 7365 7243 6f6e 6669 6794  .MdParserConfig.
-00006760: 9394 2981 947d 9428 8c0f 636f 6d6d 6f6e  ..)..}.(..common
-00006770: 6d61 726b 5f6f 6e6c 7994 898c 0867 666d  mark_only....gfm
-00006780: 5f6f 6e6c 7994 898c 1165 6e61 626c 655f  _only....enable_
-00006790: 6578 7465 6e73 696f 6e73 9468 4e8c 0e64  extensions.hN..d
-000067a0: 6973 6162 6c65 5f73 796e 7461 7894 6a1d  isable_syntax.j.
-000067b0: 0300 008c 1261 6c6c 5f6c 696e 6b73 5f65  .....all_links_e
-000067c0: 7874 6572 6e61 6c94 898c 0b75 726c 5f73  xternal....url_s
-000067d0: 6368 656d 6573 9468 558c 0b72 6566 5f64  chemes.hU..ref_d
-000067e0: 6f6d 6169 6e73 944e 8c15 6869 6768 6c69  omains.N..highli
-000067f0: 6768 745f 636f 6465 5f62 6c6f 636b 7394  ght_code_blocks.
-00006800: 888c 126e 756d 6265 725f 636f 6465 5f62  ...number_code_b
-00006810: 6c6f 636b 7394 6a26 0300 008c 0f74 6974  locks.j&.....tit
-00006820: 6c65 5f74 6f5f 6865 6164 6572 9489 8c0f  le_to_header....
-00006830: 6865 6164 696e 675f 616e 6368 6f72 7394  heading_anchors.
-00006840: 4e8c 1168 6561 6469 6e67 5f73 6c75 675f  N..heading_slug_
-00006850: 6675 6e63 944e 8c09 6874 6d6c 5f6d 6574  func.N..html_met
-00006860: 6194 6a2f 0300 008c 1366 6f6f 746e 6f74  a.j/.....footnot
-00006870: 655f 7472 616e 7369 7469 6f6e 9488 8c10  e_transition....
-00006880: 776f 7264 735f 7065 725f 6d69 6e75 7465  words_per_minute
-00006890: 944b c88c 0d73 7562 7374 6974 7574 696f  .K...substitutio
-000068a0: 6e73 946a 3603 0000 8c0e 7375 625f 6465  ns.j6.....sub_de
-000068b0: 6c69 6d69 7465 7273 946a 3b03 0000 8c13  limiters.j;.....
-000068c0: 6c69 6e6b 6966 795f 6675 7a7a 795f 6c69  linkify_fuzzy_li
-000068d0: 6e6b 7394 888c 1264 6d61 7468 5f61 6c6c  nks....dmath_all
-000068e0: 6f77 5f6c 6162 656c 7394 888c 1164 6d61  ow_labels....dma
-000068f0: 7468 5f61 6c6c 6f77 5f73 7061 6365 9488  th_allow_space..
-00006900: 8c12 646d 6174 685f 616c 6c6f 775f 6469  ..dmath_allow_di
-00006910: 6769 7473 9488 8c13 646d 6174 685f 646f  gits....dmath_do
-00006920: 7562 6c65 5f69 6e6c 696e 6594 898c 0e75  uble_inline....u
-00006930: 7064 6174 655f 6d61 7468 6a61 7894 888c  pdate_mathjax...
-00006940: 0f6d 6174 686a 6178 5f63 6c61 7373 6573  .mathjax_classes
-00006950: 9468 c975 628c 0d6d 7973 746e 625f 636f  .h.ub..mystnb_co
-00006960: 6e66 6967 948c 136d 7973 745f 6e62 2e63  nfig...myst_nb.c
-00006970: 6f72 652e 636f 6e66 6967 948c 0e4e 6250  ore.config...NbP
-00006980: 6172 7365 7243 6f6e 6669 6794 9394 2981  arserConfig...).
-00006990: 947d 9428 8c0e 6375 7374 6f6d 5f66 6f72  .}.(..custom_for
-000069a0: 6d61 7473 947d 948c 0a72 6561 645f 6173  mats.}...read_as
-000069b0: 5f6d 6494 898c 0c6d 6574 6164 6174 615f  _md....metadata_
-000069c0: 6b65 7994 6a4f 0300 008c 1163 656c 6c5f  key.jO.....cell_
-000069d0: 6d65 7461 6461 7461 5f6b 6579 946a 4f03  metadata_key.jO.
-000069e0: 0000 8c12 6b65 726e 656c 5f72 6778 5f61  ....kernel_rgx_a
-000069f0: 6c69 6173 6573 946a 5703 0000 8c0e 6578  liases.jW.....ex
-00006a00: 6563 7574 696f 6e5f 6d6f 6465 9468 608c  ecution_mode.h`.
-00006a10: 1465 7865 6375 7469 6f6e 5f63 6163 6865  .execution_cache
-00006a20: 5f70 6174 6894 8c5c 2f6d 6e74 2f63 2f55  _path..\/mnt/c/U
-00006a30: 7365 7273 2f72 616e 646f 2f44 6f77 6e6c  sers/rando/Downl
-00006a40: 6f61 6473 2f50 7974 686f 6e5f 576f 726b  oads/Python_Work
-00006a50: 7370 6163 652f 766f 6c6c 7365 672d 6e61  space/vollseg-na
-00006a60: 7061 7269 2d74 7261 636b 6d61 7465 2f5f  pari-trackmate/_
-00006a70: 6275 696c 642f 2e6a 7570 7974 6572 5f63  build/.jupyter_c
-00006a80: 6163 6865 946a 6303 0000 6862 6a67 0300  ache.jc...hbjg..
-00006a90: 004b 1e6a 6b03 0000 896a 6f03 0000 898c  .K.jk....jo.....
-00006aa0: 1865 7865 6375 7469 6f6e 5f72 6169 7365  .execution_raise
-00006ab0: 5f6f 6e5f 6572 726f 7294 896a 7503 0000  _on_error..ju...
-00006ac0: 898c 0d6d 6572 6765 5f73 7472 6561 6d73  ...merge_streams
-00006ad0: 9489 8c0d 7265 6e64 6572 5f70 6c75 6769  ....render_plugi
-00006ae0: 6e94 6a04 0100 008c 1272 656d 6f76 655f  n.j......remove_
-00006af0: 636f 6465 5f73 6f75 7263 6594 898c 1372  code_source....r
-00006b00: 656d 6f76 655f 636f 6465 5f6f 7574 7075  emove_code_outpu
-00006b10: 7473 9489 8c10 636f 6465 5f70 726f 6d70  ts....code_promp
-00006b20: 745f 7368 6f77 946a 8003 0000 8c10 636f  t_show.j......co
-00006b30: 6465 5f70 726f 6d70 745f 6869 6465 946a  de_prompt_hide.j
-00006b40: 8303 0000 8c13 6e75 6d62 6572 5f73 6f75  ......number_sou
-00006b50: 7263 655f 6c69 6e65 7394 898c 0c62 7569  rce_lines....bui
-00006b60: 6c64 6572 5f6e 616d 6594 68d9 8c17 6d69  lder_name.h...mi
-00006b70: 6d65 5f70 7269 6f72 6974 795f 6f76 6572  me_priority_over
-00006b80: 7269 6465 7394 298c 0d6f 7574 7075 745f  rides.)..output_
-00006b90: 7374 6465 7272 9468 5c8c 1172 656e 6465  stderr.h\..rende
-00006ba0: 725f 7465 7874 5f6c 6578 6572 946a 8c03  r_text_lexer.j..
-00006bb0: 0000 8c12 7265 6e64 6572 5f65 7272 6f72  ....render_error
-00006bc0: 5f6c 6578 6572 946a 8f03 0000 8c14 7265  _lexer.j......re
-00006bd0: 6e64 6572 5f69 6d61 6765 5f6f 7074 696f  nder_image_optio
-00006be0: 6e73 946a 9203 0000 8c15 7265 6e64 6572  ns.j......render
-00006bf0: 5f66 6967 7572 655f 6f70 7469 6f6e 7394  _figure_options.
-00006c00: 6a95 0300 008c 1672 656e 6465 725f 6d61  j......render_ma
-00006c10: 726b 646f 776e 5f66 6f72 6d61 7494 6a98  rkdown_format.j.
-00006c20: 0300 008c 0d69 7079 7769 6467 6574 735f  .....ipywidgets_
-00006c30: 6a73 946a 9b03 0000 8c0d 6f75 7470 7574  js.j......output
-00006c40: 5f66 6f6c 6465 7294 8c5d 2f6d 6e74 2f63  _folder..]/mnt/c
-00006c50: 2f55 7365 7273 2f72 616e 646f 2f44 6f77  /Users/rando/Dow
-00006c60: 6e6c 6f61 6473 2f50 7974 686f 6e5f 576f  nloads/Python_Wo
-00006c70: 726b 7370 6163 652f 766f 6c6c 7365 672d  rkspace/vollseg-
-00006c80: 6e61 7061 7269 2d74 7261 636b 6d61 7465  napari-trackmate
-00006c90: 2f5f 6275 696c 642f 6a75 7079 7465 725f  /_build/jupyter_
-00006ca0: 6578 6563 7574 6594 8c0a 6170 7065 6e64  execute...append
-00006cb0: 5f63 7373 9488 8c0e 6d65 7461 6461 7461  _css....metadata
-00006cc0: 5f74 6f5f 666d 9489 7562 8c11 696e 7465  _to_fm..ub..inte
-00006cd0: 7273 7068 696e 785f 6361 6368 6594 7d94  rsphinx_cache.}.
-00006ce0: 8c15 696e 7465 7273 7068 696e 785f 696e  ..intersphinx_in
-00006cf0: 7665 6e74 6f72 7994 7d94 8c1b 696e 7465  ventory.}...inte
-00006d00: 7273 7068 696e 785f 6e61 6d65 645f 696e  rsphinx_named_in
-00006d10: 7665 6e74 6f72 7994 7d94 8c19 7370 6869  ventory.}...sphi
-00006d20: 6e78 5f64 6573 6967 6e5f 6373 735f 6368  nx_design_css_ch
-00006d30: 616e 6765 6494 898c 106e 625f 6e65 775f  anged....nb_new_
-00006d40: 6578 6563 5f64 6174 6194 8968 9868 9c8c  exec_data..h.h..
-00006d50: 0b6e 625f 6d65 7461 6461 7461 946a 1d04  .nb_metadata.j..
-00006d60: 0000 6a2e 0400 0085 9452 9475 622e       ..j......R.ub.
+00000a00: 0844 6f63 756d 656e 7494 9394 2981 944e  .Document...)..N
+00000a10: 7d94 288c 0764 6f63 6e61 6d65 9468 a08c  }.(..docname.h..
+00000a20: 0873 7562 7472 6565 7394 5d94 6899 8c07  .subtrees.].h...
+00000a30: 546f 6354 7265 6594 9394 2981 944e 7d94  TocTree...)..N}.
+00000a40: 288c 0569 7465 6d73 945d 9468 998c 0846  (..items.].h...F
+00000a50: 696c 6549 7465 6d94 9394 8c09 414c 474f  ileItem.....ALGO
+00000a60: 5249 5448 4d94 8594 8194 618c 0763 6170  RITHM.....a..cap
+00000a70: 7469 6f6e 944e 8c06 6869 6464 656e 9488  tion.N..hidden..
+00000a80: 8c08 6d61 7864 6570 7468 944a ffff ffff  ..maxdepth.J....
+00000a90: 8c08 6e75 6d62 6572 6564 9489 8c08 7265  ..numbered....re
+00000aa0: 7665 7273 6564 9489 8c0a 7469 746c 6573  versed....titles
+00000ab0: 6f6e 6c79 9488 7586 9462 618c 0574 6974  only..u..ba..tit
+00000ac0: 6c65 944e 7586 9462 8c09 414c 474f 5249  le.Nu..b..ALGORI
+00000ad0: 5448 4d94 68a2 2981 944e 7d94 2868 a568  THM.h.)..N}.(h.h
+00000ae0: bc68 a65d 9468 ba4e 7586 9462 758c 055f  .h.].h.Nu..bu.._
+00000af0: 726f 6f74 9468 a38c 055f 6d65 7461 947d  root.h..._meta.}
+00000b00: 948c 0c5f 6669 6c65 5f66 6f72 6d61 7494  ..._file_format.
+00000b10: 8c07 6a62 2d62 6f6f 6b94 7562 8c0a 6d61  ..jb-book.ub..ma
+00000b20: 7374 6572 5f64 6f63 9468 a08c 0f6d 6174  ster_doc.h...mat
+00000b30: 686a 6178 335f 636f 6e66 6967 947d 948c  hjax3_config.}..
+00000b40: 076f 7074 696f 6e73 947d 948c 1070 726f  .options.}...pro
+00000b50: 6365 7373 4874 6d6c 436c 6173 7394 8c30  cessHtmlClass..0
+00000b60: 7465 7832 6a61 785f 7072 6f63 6573 737c  tex2jax_process|
+00000b70: 6d61 7468 6a61 785f 7072 6f63 6573 737c  mathjax_process|
+00000b80: 6d61 7468 7c6f 7574 7075 745f 6172 6561  math|output_area
+00000b90: 9473 738c 1468 746d 6c5f 7065 726d 616c  .ss..html_permal
+00000ba0: 696e 6b73 5f69 636f 6e94 8c01 2394 8c0f  inks_icon...#...
+00000bb0: 6c61 7465 785f 646f 6375 6d65 6e74 7394  latex_documents.
+00000bc0: 5d94 2868 a08c 1c76 6f6c 6c73 6567 2d6e  ].(h...vollseg-n
+00000bd0: 6170 6172 692d 7472 6163 6b6d 6174 652e  apari-trackmate.
+00000be0: 7465 7894 6838 8c0c 5661 7275 6e20 4b61  tex.h8..Varun Ka
+00000bf0: 706f 6f72 9468 7b74 9461 8c06 7661 6c75  poor.h{t.a..valu
+00000c00: 6573 947d 9428 8c07 7072 6f6a 6563 7494  es.}.(..project.
+00000c10: 8c06 5079 7468 6f6e 948c 0365 6e76 944e  ..Python...env.N
+00000c20: 8794 6839 683a 68d8 4e87 948c 1170 726f  ..h9h:h.N....pro
+00000c30: 6a65 6374 5f63 6f70 7972 6967 6874 9468  ject_copyright.h
+00000c40: 1f8c 0468 746d 6c94 4e87 9468 3b68 3c68  ...html.N..h;h<h
+00000c50: dc4e 8794 8c07 7665 7273 696f 6e94 681f  .N....version.h.
+00000c60: 68d8 4e87 948c 0772 656c 6561 7365 9468  h.N....release.h
+00000c70: 1f68 d84e 8794 8c05 746f 6461 7994 681f  .h.N....today.h.
+00000c80: 68d8 4e87 948c 0974 6f64 6179 5f66 6d74  h.N....today_fmt
+00000c90: 944e 68d8 4e87 948c 086c 616e 6775 6167  .Nh.N....languag
+00000ca0: 6594 4e68 d84e 8794 8c0b 6c6f 6361 6c65  e.Nh.N....locale
+00000cb0: 5f64 6972 7394 5d94 8c07 6c6f 6361 6c65  _dirs.]...locale
+00000cc0: 7394 6168 d84e 8794 8c18 6669 6775 7265  s.ah.N....figure
+00000cd0: 5f6c 616e 6775 6167 655f 6669 6c65 6e61  _language_filena
+00000ce0: 6d65 948c 167b 726f 6f74 7d2e 7b6c 616e  me...{root}.{lan
+00000cf0: 6775 6167 657d 7b65 7874 7d94 68d8 4e87  guage}{ext}.h.N.
+00000d00: 948c 2067 6574 7465 7874 5f61 6c6c 6f77  .. gettext_allow
+00000d10: 5f66 757a 7a79 5f74 7261 6e73 6c61 7469  _fuzzy_translati
+00000d20: 6f6e 7394 898c 0767 6574 7465 7874 944e  ons....gettext.N
+00000d30: 8794 68c6 68a0 68d8 4e87 948c 0872 6f6f  ..h.h.h.N....roo
+00000d40: 745f 646f 6394 68a0 68d8 4e87 9468 8468  t_doc.h.h.N..h.h
+00000d50: 8868 d84e 8794 8c0f 736f 7572 6365 5f65  .h.N....source_e
+00000d60: 6e63 6f64 696e 6794 8c09 7574 662d 382d  ncoding...utf-8-
+00000d70: 7369 6794 68d8 4e87 9468 3f68 4068 d84e  sig.h.N..h?h@h.N
+00000d80: 8794 8c0c 6465 6661 756c 745f 726f 6c65  ....default_role
+00000d90: 944e 68d8 4e87 948c 1861 6464 5f66 756e  .Nh.N....add_fun
+00000da0: 6374 696f 6e5f 7061 7265 6e74 6865 7365  ction_parenthese
+00000db0: 7394 8868 d84e 8794 8c10 6164 645f 6d6f  s..h.N....add_mo
+00000dc0: 6475 6c65 5f6e 616d 6573 9488 68d8 4e87  dule_names..h.N.
+00000dd0: 948c 1d74 7269 6d5f 666f 6f74 6e6f 7465  ...trim_footnote
+00000de0: 5f72 6566 6572 656e 6365 5f73 7061 6365  _reference_space
+00000df0: 9489 68d8 4e87 948c 0c73 686f 775f 6175  ..h.N....show_au
+00000e00: 7468 6f72 7394 8968 d84e 8794 6812 6813  thors..h.N..h.h.
+00000e10: 68dc 4e87 948c 1268 6967 686c 6967 6874  h.N....highlight
+00000e20: 5f6c 616e 6775 6167 6594 8c07 6465 6661  _language...defa
+00000e30: 756c 7494 68d8 4e87 948c 1168 6967 686c  ult.h.N....highl
+00000e40: 6967 6874 5f6f 7074 696f 6e73 947d 9468  ight_options.}.h
+00000e50: d84e 8794 8c0e 7465 6d70 6c61 7465 735f  .N....templates_
+00000e60: 7061 7468 945d 9428 8c7c 2f68 6f6d 652f  path.].(.|/home/
+00000e70: 7661 7275 6e6b 6170 6f6f 722f 616e 6163  varunkapoor/anac
+00000e80: 6f6e 6461 332f 656e 7673 2f6e 6170 6172  onda3/envs/napar
+00000e90: 6965 6e76 2f6c 6962 2f70 7974 686f 6e33  ienv/lib/python3
+00000ea0: 2e31 302f 7369 7465 2d70 6163 6b61 6765  .10/site-package
+00000eb0: 732f 7370 6869 6e78 5f62 6f6f 6b5f 7468  s/sphinx_book_th
+00000ec0: 656d 652f 7468 656d 652f 7370 6869 6e78  eme/theme/sphinx
+00000ed0: 5f62 6f6f 6b5f 7468 656d 652f 636f 6d70  _book_theme/comp
+00000ee0: 6f6e 656e 7473 948c 802f 686f 6d65 2f76  onents.../home/v
+00000ef0: 6172 756e 6b61 706f 6f72 2f61 6e61 636f  arunkapoor/anaco
+00000f00: 6e64 6133 2f65 6e76 732f 6e61 7061 7269  nda3/envs/napari
+00000f10: 656e 762f 6c69 622f 7079 7468 6f6e 332e  env/lib/python3.
+00000f20: 3130 2f73 6974 652d 7061 636b 6167 6573  10/site-packages
+00000f30: 2f70 7964 6174 615f 7370 6869 6e78 5f74  /pydata_sphinx_t
+00000f40: 6865 6d65 2f74 6865 6d65 2f70 7964 6174  heme/theme/pydat
+00000f50: 615f 7370 6869 6e78 5f74 6865 6d65 2f63  a_sphinx_theme/c
+00000f60: 6f6d 706f 6e65 6e74 7394 8c7c 2f68 6f6d  omponents..|/hom
+00000f70: 652f 7661 7275 6e6b 6170 6f6f 722f 616e  e/varunkapoor/an
+00000f80: 6163 6f6e 6461 332f 656e 7673 2f6e 6170  aconda3/envs/nap
+00000f90: 6172 6965 6e76 2f6c 6962 2f70 7974 686f  arienv/lib/pytho
+00000fa0: 6e33 2e31 302f 7369 7465 2d70 6163 6b61  n3.10/site-packa
+00000fb0: 6765 732f 7370 6869 6e78 5f62 6f6f 6b5f  ges/sphinx_book_
+00000fc0: 7468 656d 652f 7468 656d 652f 7370 6869  theme/theme/sphi
+00000fd0: 6e78 5f62 6f6f 6b5f 7468 656d 652f 636f  nx_book_theme/co
+00000fe0: 6d70 6f6e 656e 7473 9465 68dc 4e87 948c  mponents.eh.N...
+00000ff0: 0f74 656d 706c 6174 655f 6272 6964 6765  .template_bridge
+00001000: 944e 68dc 4e87 948c 0d6b 6565 705f 7761  .Nh.N....keep_wa
+00001010: 726e 696e 6773 9489 68d8 4e87 9468 3468  rnings..h.N..h4h
+00001020: 3568 d84e 8794 8c16 6d6f 6469 6e64 6578  5h.N....modindex
+00001030: 5f63 6f6d 6d6f 6e5f 7072 6566 6978 945d  _common_prefix.]
+00001040: 9468 dc4e 8794 8c0a 7273 745f 6570 696c  .h.N....rst_epil
+00001050: 6f67 944e 68d8 4e87 948c 0a72 7374 5f70  og.Nh.N....rst_p
+00001060: 726f 6c6f 6794 4e68 d84e 8794 8c12 7472  rolog.Nh.N....tr
+00001070: 696d 5f64 6f63 7465 7374 5f66 6c61 6773  im_doctest_flags
+00001080: 9488 68d8 4e87 948c 0e70 7269 6d61 7279  ..h.N....primary
+00001090: 5f64 6f6d 6169 6e94 8c02 7079 9468 d84e  _domain...py.h.N
+000010a0: 8794 8c0c 6e65 6564 735f 7370 6869 6e78  ....needs_sphinx
+000010b0: 944e 4e4e 8794 8c10 6e65 6564 735f 6578  .NNN....needs_ex
+000010c0: 7465 6e73 696f 6e73 947d 944e 4e87 948c  tensions.}.NN...
+000010d0: 0c6d 616e 7061 6765 735f 7572 6c94 4e68  .manpages_url.Nh
+000010e0: d84e 8794 8c08 6e69 7470 6963 6b79 9489  .N....nitpicky..
+000010f0: 4e4e 8794 8c0e 6e69 7470 6963 6b5f 6967  NN....nitpick_ig
+00001100: 6e6f 7265 945d 944e 4e87 948c 146e 6974  nore.].NN....nit
+00001110: 7069 636b 5f69 676e 6f72 655f 7265 6765  pick_ignore_rege
+00001120: 7894 5d94 4e4e 8794 6833 8868 d84e 8794  x.].NN..h3.h.N..
+00001130: 8c13 6e75 6d66 6967 5f73 6563 6e75 6d5f  ..numfig_secnum_
+00001140: 6465 7074 6894 4b01 68d8 4e87 9468 8e68  depth.K.h.N..h.h
+00001150: 8f68 d84e 8794 8c0f 6d61 7468 5f6e 756d  .h.N....math_num
+00001160: 6265 725f 616c 6c94 8968 d84e 8794 8c11  ber_all..h.N....
+00001170: 6d61 7468 5f65 7172 6566 5f66 6f72 6d61  math_eqref_forma
+00001180: 7494 4e68 d84e 8794 8c0b 6d61 7468 5f6e  t.Nh.N....math_n
+00001190: 756d 6669 6794 8868 d84e 8794 8c0a 746c  umfig..h.N....tl
+000011a0: 735f 7665 7269 6679 9488 68d8 4e87 948c  s_verify..h.N...
+000011b0: 0b74 6c73 5f63 6163 6572 7473 944e 68d8  .tls_cacerts.Nh.
+000011c0: 4e87 948c 0a75 7365 725f 6167 656e 7494  N....user_agent.
+000011d0: 4e68 d84e 8794 8c0b 736d 6172 7471 756f  Nh.N....smartquo
+000011e0: 7465 7394 8868 d84e 8794 8c12 736d 6172  tes..h.N....smar
+000011f0: 7471 756f 7465 735f 6163 7469 6f6e 948c  tquotes_action..
+00001200: 0371 4465 9468 d84e 8794 8c14 736d 6172  .qDe.h.N....smar
+00001210: 7471 756f 7465 735f 6578 636c 7564 6573  tquotes_excludes
+00001220: 947d 9428 8c09 6c61 6e67 7561 6765 7394  .}.(..languages.
+00001230: 5d94 8c02 6a61 9461 8c08 6275 696c 6465  ]...ja.a..builde
+00001240: 7273 945d 9428 8c03 6d61 6e94 8c04 7465  rs.].(..man...te
+00001250: 7874 9465 7568 d84e 8794 8c0d 6570 7562  xt.euh.N....epub
+00001260: 5f62 6173 656e 616d 6594 68d7 4e4e 8794  _basename.h.NN..
+00001270: 8c0c 6570 7562 5f76 6572 7369 6f6e 9447  ..epub_version.G
+00001280: 4008 0000 0000 0000 8c04 6570 7562 944e  @.........epub.N
+00001290: 8794 8c0a 6570 7562 5f74 6865 6d65 946a  ....epub_theme.j
+000012a0: 5401 0000 6a54 0100 004e 8794 8c12 6570  T...jT...N....ep
+000012b0: 7562 5f74 6865 6d65 5f6f 7074 696f 6e73  ub_theme_options
+000012c0: 947d 946a 5401 0000 4e87 948c 0a65 7075  .}.jT...N....epu
+000012d0: 625f 7469 746c 6594 68d7 6a54 0100 004e  b_title.h.jT...N
+000012e0: 8794 8c0b 6570 7562 5f61 7574 686f 7294  ....epub_author.
+000012f0: 683a 6a54 0100 004e 8794 8c0d 6570 7562  h:jT...N....epub
+00001300: 5f6c 616e 6775 6167 6594 8c02 656e 946a  _language...en.j
+00001310: 5401 0000 4e87 948c 0e65 7075 625f 7075  T...N....epub_pu
+00001320: 626c 6973 6865 7294 683a 6a54 0100 004e  blisher.h:jT...N
+00001330: 8794 8c0e 6570 7562 5f63 6f70 7972 6967  ....epub_copyrig
+00001340: 6874 9468 3c6a 5401 0000 4e87 948c 0f65  ht.h<jT...N....e
+00001350: 7075 625f 6964 656e 7469 6669 6572 948c  pub_identifier..
+00001360: 0775 6e6b 6e6f 776e 946a 5401 0000 4e87  .unknown.jT...N.
+00001370: 948c 0b65 7075 625f 7363 6865 6d65 946a  ...epub_scheme.j
+00001380: 6701 0000 6a54 0100 004e 8794 8c08 6570  g...jT...N....ep
+00001390: 7562 5f75 6964 946a 6701 0000 68d8 4e87  ub_uid.jg...h.N.
+000013a0: 948c 0a65 7075 625f 636f 7665 7294 2968  ...epub_cover.)h
+000013b0: d84e 8794 8c0a 6570 7562 5f67 7569 6465  .N....epub_guide
+000013c0: 9429 68d8 4e87 948c 0e65 7075 625f 7072  .)h.N....epub_pr
+000013d0: 655f 6669 6c65 7394 5d94 68d8 4e87 948c  e_files.].h.N...
+000013e0: 0f65 7075 625f 706f 7374 5f66 696c 6573  .epub_post_files
+000013f0: 945d 9468 d84e 8794 687e 687f 6a54 0100  .].h.N..h~h.jT..
+00001400: 004e 8794 8c12 6570 7562 5f65 7863 6c75  .N....epub_exclu
+00001410: 6465 5f66 696c 6573 945d 9468 d84e 8794  de_files.].h.N..
+00001420: 8c0d 6570 7562 5f74 6f63 6465 7074 6894  ..epub_tocdepth.
+00001430: 4b03 68d8 4e87 948c 0b65 7075 625f 746f  K.h.N....epub_to
+00001440: 6364 7570 9488 68d8 4e87 948c 0d65 7075  cdup..h.N....epu
+00001450: 625f 746f 6373 636f 7065 946a 0701 0000  b_tocscope.j....
+00001460: 68d8 4e87 948c 0f65 7075 625f 6669 785f  h.N....epub_fix_
+00001470: 696d 6167 6573 9489 68d8 4e87 948c 1465  images..h.N....e
+00001480: 7075 625f 6d61 785f 696d 6167 655f 7769  pub_max_image_wi
+00001490: 6474 6894 4b00 68d8 4e87 948c 0e65 7075  dth.K.h.N....epu
+000014a0: 625f 7368 6f77 5f75 726c 7394 8c06 696e  b_show_urls...in
+000014b0: 6c69 6e65 946a 5401 0000 4e87 948c 0e65  line.jT...N....e
+000014c0: 7075 625f 7573 655f 696e 6465 7894 886a  pub_use_index..j
+000014d0: 5401 0000 4e87 948c 1065 7075 625f 6465  T...N....epub_de
+000014e0: 7363 7269 7074 696f 6e94 6a67 0100 006a  scription.jg...j
+000014f0: 5401 0000 4e87 948c 1065 7075 625f 636f  T...N....epub_co
+00001500: 6e74 7269 6275 746f 7294 6a67 0100 006a  ntributor.jg...j
+00001510: 5401 0000 4e87 948c 1165 7075 625f 7772  T...N....epub_wr
+00001520: 6974 696e 675f 6d6f 6465 948c 0a68 6f72  iting_mode...hor
+00001530: 697a 6f6e 7461 6c94 6a54 0100 004e 8794  izontal.jT...N..
+00001540: 6814 6815 68dc 4e87 948c 0f68 746d 6c5f  h.h.h.N....html_
+00001550: 7468 656d 655f 7061 7468 945d 9468 dc4e  theme_path.].h.N
+00001560: 8794 6816 6817 68dc 4e87 9468 3768 3868  ..h.h.h.N..h7h8h
+00001570: dc4e 8794 8c10 6874 6d6c 5f73 686f 7274  .N....html_short
+00001580: 5f74 6974 6c65 9468 3868 dc4e 8794 8c0a  _title.h8h.N....
+00001590: 6874 6d6c 5f73 7479 6c65 944e 68dc 4e87  html_style.Nh.N.
+000015a0: 9468 3d4e 68dc 4e87 9468 4668 1f68 dc4e  .h=Nh.N..hFh.h.N
+000015b0: 8794 6880 6881 68dc 4e87 9468 8268 8368  ..h.h.h.N..h.h.h
+000015c0: dc4e 8794 8c10 6874 6d6c 5f73 7461 7469  .N....html_stati
+000015d0: 635f 7061 7468 945d 9428 8c63 2f68 6f6d  c_path.].(.c/hom
+000015e0: 652f 7661 7275 6e6b 6170 6f6f 722f 616e  e/varunkapoor/an
+000015f0: 6163 6f6e 6461 332f 656e 7673 2f6e 6170  aconda3/envs/nap
+00001600: 6172 6965 6e76 2f6c 6962 2f70 7974 686f  arienv/lib/pytho
+00001610: 6e33 2e31 302f 7369 7465 2d70 6163 6b61  n3.10/site-packa
+00001620: 6765 732f 7370 6869 6e78 5f74 6f67 676c  ges/sphinx_toggl
+00001630: 6562 7574 746f 6e2f 5f73 7461 7469 6394  ebutton/_static.
+00001640: 8c61 2f68 6f6d 652f 7661 7275 6e6b 6170  .a/home/varunkap
+00001650: 6f6f 722f 616e 6163 6f6e 6461 332f 656e  oor/anaconda3/en
+00001660: 7673 2f6e 6170 6172 6965 6e76 2f6c 6962  vs/naparienv/lib
+00001670: 2f70 7974 686f 6e33 2e31 302f 7369 7465  /python3.10/site
+00001680: 2d70 6163 6b61 6765 732f 7370 6869 6e78  -packages/sphinx
+00001690: 5f63 6f70 7962 7574 746f 6e2f 5f73 7461  _copybutton/_sta
+000016a0: 7469 6394 8c5c 2f68 6f6d 652f 7661 7275  tic..\/home/varu
+000016b0: 6e6b 6170 6f6f 722f 616e 6163 6f6e 6461  nkapoor/anaconda
+000016c0: 332f 656e 7673 2f6e 6170 6172 6965 6e76  3/envs/naparienv
+000016d0: 2f6c 6962 2f70 7974 686f 6e33 2e31 302f  /lib/python3.10/
+000016e0: 7369 7465 2d70 6163 6b61 6765 732f 7370  site-packages/sp
+000016f0: 6869 6e78 5f74 6865 6265 2f5f 7374 6174  hinx_thebe/_stat
+00001700: 6963 948c 5f2f 686f 6d65 2f76 6172 756e  ic.._/home/varun
+00001710: 6b61 706f 6f72 2f61 6e61 636f 6e64 6133  kapoor/anaconda3
+00001720: 2f65 6e76 732f 6e61 7061 7269 656e 762f  /envs/naparienv/
+00001730: 6c69 622f 7079 7468 6f6e 332e 3130 2f73  lib/python3.10/s
+00001740: 6974 652d 7061 636b 6167 6573 2f73 7068  ite-packages/sph
+00001750: 696e 785f 636f 6d6d 656e 7473 2f5f 7374  inx_comments/_st
+00001760: 6174 6963 948c 682f 6d6e 742f 632f 5573  atic..h/mnt/c/Us
+00001770: 6572 732f 7261 6e64 6f2f 446f 776e 6c6f  ers/rando/Downlo
+00001780: 6164 732f 5079 7468 6f6e 5f57 6f72 6b73  ads/Python_Works
+00001790: 7061 6365 2f76 6f6c 6c73 6567 2d6e 6170  pace/vollseg-nap
+000017a0: 6172 692d 7472 6163 6b6d 6174 652f 5f62  ari-trackmate/_b
+000017b0: 7569 6c64 2f68 746d 6c2f 5f73 7068 696e  uild/html/_sphin
+000017c0: 785f 6465 7369 676e 5f73 7461 7469 6394  x_design_static.
+000017d0: 6568 dc4e 8794 8c0f 6874 6d6c 5f65 7874  eh.N....html_ext
+000017e0: 7261 5f70 6174 6894 5d94 68dc 4e87 948c  ra_path.].h.N...
+000017f0: 1568 746d 6c5f 6c61 7374 5f75 7064 6174  .html_last_updat
+00001800: 6564 5f66 6d74 944e 68dc 4e87 948c 0d68  ed_fmt.Nh.N....h
+00001810: 746d 6c5f 7369 6465 6261 7273 947d 9468  tml_sidebars.}.h
+00001820: dc4e 8794 8c15 6874 6d6c 5f61 6464 6974  .N....html_addit
+00001830: 696f 6e61 6c5f 7061 6765 7394 7d94 68dc  ional_pages.}.h.
+00001840: 4e87 948c 1368 746d 6c5f 646f 6d61 696e  N....html_domain
+00001850: 5f69 6e64 6963 6573 9488 68dc 4e87 948c  _indices..h.N...
+00001860: 1368 746d 6c5f 6164 645f 7065 726d 616c  .html_add_permal
+00001870: 696e 6b73 948c 1473 7068 696e 782e 6275  inks...sphinx.bu
+00001880: 696c 6465 7273 2e68 746d 6c94 8c13 5f73  ilders.html..._s
+00001890: 7461 626c 655f 7265 7072 5f6f 626a 6563  table_repr_objec
+000018a0: 7494 9394 2981 9468 dc4e 8794 8c0f 6874  t...)..h.N....ht
+000018b0: 6d6c 5f70 6572 6d61 6c69 6e6b 7394 8868  ml_permalinks..h
+000018c0: dc4e 8794 68cd 68ce 68dc 4e87 948c 0e68  .N..h.h.h.N....h
+000018d0: 746d 6c5f 7573 655f 696e 6465 7894 8868  tml_use_index..h
+000018e0: dc4e 8794 8c10 6874 6d6c 5f73 706c 6974  .N....html_split
+000018f0: 5f69 6e64 6578 9489 68dc 4e87 948c 1068  _index..h.N....h
+00001900: 746d 6c5f 636f 7079 5f73 6f75 7263 6594  tml_copy_source.
+00001910: 8868 dc4e 8794 8c14 6874 6d6c 5f73 686f  .h.N....html_sho
+00001920: 775f 736f 7572 6365 6c69 6e6b 9488 68dc  w_sourcelink..h.
+00001930: 4e87 9468 3268 1f68 dc4e 8794 8c13 6874  N..h2h.h.N....ht
+00001940: 6d6c 5f75 7365 5f6f 7065 6e73 6561 7263  ml_use_opensearc
+00001950: 6894 681f 68dc 4e87 948c 1068 746d 6c5f  h.h.h.N....html_
+00001960: 6669 6c65 5f73 7566 6669 7894 4e68 dc4e  file_suffix.Nh.N
+00001970: 8794 8c10 6874 6d6c 5f6c 696e 6b5f 7375  ....html_link_su
+00001980: 6666 6978 944e 68dc 4e87 948c 1368 746d  ffix.Nh.N....htm
+00001990: 6c5f 7368 6f77 5f63 6f70 7972 6967 6874  l_show_copyright
+000019a0: 9488 68dc 4e87 948c 1868 746d 6c5f 7368  ..h.N....html_sh
+000019b0: 6f77 5f73 6561 7263 685f 7375 6d6d 6172  ow_search_summar
+000019c0: 7994 8868 dc4e 8794 8c10 6874 6d6c 5f73  y..h.N....html_s
+000019d0: 686f 775f 7370 6869 6e78 9488 68dc 4e87  how_sphinx..h.N.
+000019e0: 948c 0c68 746d 6c5f 636f 6e74 6578 7494  ...html_context.
+000019f0: 7d94 288c 1663 6f70 7962 7574 746f 6e5f  }.(..copybutton_
+00001a00: 7072 6f6d 7074 5f74 6578 7494 681f 8c1b  prompt_text.h...
+00001a10: 636f 7079 6275 7474 6f6e 5f70 726f 6d70  copybutton_promp
+00001a20: 745f 6973 5f72 6567 6578 7094 898c 2163  t_is_regexp...!c
+00001a30: 6f70 7962 7574 746f 6e5f 6f6e 6c79 5f63  opybutton_only_c
+00001a40: 6f70 795f 7072 6f6d 7074 5f6c 696e 6573  opy_prompt_lines
+00001a50: 9488 8c19 636f 7079 6275 7474 6f6e 5f72  ....copybutton_r
+00001a60: 656d 6f76 655f 7072 6f6d 7074 7394 888c  emove_prompts...
+00001a70: 1b63 6f70 7962 7574 746f 6e5f 636f 7079  .copybutton_copy
+00001a80: 5f65 6d70 7479 5f6c 696e 6573 9488 8c26  _empty_lines...&
+00001a90: 636f 7079 6275 7474 6f6e 5f6c 696e 655f  copybutton_line_
+00001aa0: 636f 6e74 696e 7561 7469 6f6e 5f63 6861  continuation_cha
+00001ab0: 7261 6374 6572 9468 1f8c 1d63 6f70 7962  racter.h...copyb
+00001ac0: 7574 746f 6e5f 6865 7265 5f64 6f63 5f64  utton_here_doc_d
+00001ad0: 656c 696d 6974 6572 9468 1f8c 1463 6f70  elimiter.h...cop
+00001ae0: 7962 7574 746f 6e5f 696d 6167 655f 7376  ybutton_image_sv
+00001af0: 6794 681f 8c13 636f 7079 6275 7474 6f6e  g.h...copybutton
+00001b00: 5f73 656c 6563 746f 7294 8c11 6469 762e  _selector...div.
+00001b10: 6869 6768 6c69 6768 7420 7072 6594 8c16  highlight pre...
+00001b20: 636f 7079 6275 7474 6f6e 5f66 6f72 6d61  copybutton_forma
+00001b30: 745f 6675 6e63 9458 7c0a 0000 6675 6e63  t_func.X|...func
+00001b40: 7469 6f6e 2065 7363 6170 6552 6567 4578  tion escapeRegEx
+00001b50: 7028 7374 7269 6e67 2920 7b0a 2020 2020  p(string) {.    
+00001b60: 7265 7475 726e 2073 7472 696e 672e 7265  return string.re
+00001b70: 706c 6163 6528 2f5b 2e2a 2b3f 5e24 7b7d  place(/[.*+?^${}
+00001b80: 2829 7c5b 5c5d 5c5c 5d2f 672c 2027 5c5c  ()|[\]\\]/g, '\\
+00001b90: 2426 2729 3b20 2f2f 2024 2620 6d65 616e  $&'); // $& mean
+00001ba0: 7320 7468 6520 7768 6f6c 6520 6d61 7463  s the whole matc
+00001bb0: 6865 6420 7374 7269 6e67 0a7d 0a0a 2f2a  hed string.}../*
+00001bc0: 2a0a 202a 2052 656d 6f76 6573 2065 7863  *. * Removes exc
+00001bd0: 6c75 6465 6420 7465 7874 2066 726f 6d20  luded text from 
+00001be0: 6120 4e6f 6465 2e0a 202a 0a20 2a20 4070  a Node.. *. * @p
+00001bf0: 6172 616d 207b 4e6f 6465 7d20 7461 7267  aram {Node} targ
+00001c00: 6574 204e 6f64 6520 746f 2066 696c 7465  et Node to filte
+00001c10: 722e 0a20 2a20 4070 6172 616d 207b 7374  r.. * @param {st
+00001c20: 7269 6e67 7d20 6578 636c 7564 6520 4353  ring} exclude CS
+00001c30: 5320 7365 6c65 6374 6f72 206f 6620 6e6f  S selector of no
+00001c40: 6465 7320 746f 2065 7863 6c75 6465 2e0a  des to exclude..
+00001c50: 202a 2040 7265 7475 726e 7320 7b44 4f4d   * @returns {DOM
+00001c60: 5374 7269 6e67 7d20 5465 7874 2066 726f  String} Text fro
+00001c70: 6d20 6074 6172 6765 7460 2077 6974 6820  m `target` with 
+00001c80: 7465 7874 2072 656d 6f76 6564 2e0a 202a  text removed.. *
+00001c90: 2f0a 6675 6e63 7469 6f6e 2066 696c 7465  /.function filte
+00001ca0: 7254 6578 7428 7461 7267 6574 2c20 6578  rText(target, ex
+00001cb0: 636c 7564 6529 207b 0a20 2020 2063 6f6e  clude) {.    con
+00001cc0: 7374 2063 6c6f 6e65 203d 2074 6172 6765  st clone = targe
+00001cd0: 742e 636c 6f6e 654e 6f64 6528 7472 7565  t.cloneNode(true
+00001ce0: 293b 2020 2f2f 2063 6c6f 6e65 2061 7320  );  // clone as 
+00001cf0: 746f 206e 6f74 206d 6f64 6966 7920 7468  to not modify th
+00001d00: 6520 6c69 7665 2044 4f4d 0a20 2020 2069  e live DOM.    i
+00001d10: 6620 2865 7863 6c75 6465 2920 7b0a 2020  f (exclude) {.  
+00001d20: 2020 2020 2020 2f2f 2072 656d 6f76 6520        // remove 
+00001d30: 6578 636c 7564 6564 206e 6f64 6573 0a20  excluded nodes. 
+00001d40: 2020 2020 2020 2063 6c6f 6e65 2e71 7565         clone.que
+00001d50: 7279 5365 6c65 6374 6f72 416c 6c28 6578  rySelectorAll(ex
+00001d60: 636c 7564 6529 2e66 6f72 4561 6368 286e  clude).forEach(n
+00001d70: 6f64 6520 3d3e 206e 6f64 652e 7265 6d6f  ode => node.remo
+00001d80: 7665 2829 293b 0a20 2020 207d 0a20 2020  ve());.    }.   
+00001d90: 2072 6574 7572 6e20 636c 6f6e 652e 696e   return clone.in
+00001da0: 6e65 7254 6578 743b 0a7d 0a0a 2f2f 2043  nerText;.}..// C
+00001db0: 616c 6c62 6163 6b20 7768 656e 2061 2063  allback when a c
+00001dc0: 6f70 7920 6275 7474 6f6e 2069 7320 636c  opy button is cl
+00001dd0: 6963 6b65 642e 2057 696c 6c20 6265 2070  icked. Will be p
+00001de0: 6173 7365 6420 7468 6520 6e6f 6465 2074  assed the node t
+00001df0: 6861 7420 7761 7320 636c 6963 6b65 640a  hat was clicked.
+00001e00: 2f2f 2073 686f 756c 6420 7468 656e 2067  // should then g
+00001e10: 7261 6220 7468 6520 7465 7874 2061 6e64  rab the text and
+00001e20: 2072 6570 6c61 6365 2070 6965 6365 7320   replace pieces 
+00001e30: 6f66 2074 6578 7420 7468 6174 2073 686f  of text that sho
+00001e40: 756c 646e 2774 2062 6520 7573 6564 2069  uldn't be used i
+00001e50: 6e20 6f75 7470 7574 0a66 756e 6374 696f  n output.functio
+00001e60: 6e20 666f 726d 6174 436f 7079 5465 7874  n formatCopyText
+00001e70: 2874 6578 7443 6f6e 7465 6e74 2c20 636f  (textContent, co
+00001e80: 7079 6275 7474 6f6e 5072 6f6d 7074 5465  pybuttonPromptTe
+00001e90: 7874 2c20 6973 5265 6765 7870 203d 2066  xt, isRegexp = f
+00001ea0: 616c 7365 2c20 6f6e 6c79 436f 7079 5072  alse, onlyCopyPr
+00001eb0: 6f6d 7074 4c69 6e65 7320 3d20 7472 7565  omptLines = true
+00001ec0: 2c20 7265 6d6f 7665 5072 6f6d 7074 7320  , removePrompts 
+00001ed0: 3d20 7472 7565 2c20 636f 7079 456d 7074  = true, copyEmpt
+00001ee0: 794c 696e 6573 203d 2074 7275 652c 206c  yLines = true, l
+00001ef0: 696e 6543 6f6e 7469 6e75 6174 696f 6e43  ineContinuationC
+00001f00: 6861 7220 3d20 2222 2c20 6865 7265 446f  har = "", hereDo
+00001f10: 6344 656c 696d 203d 2022 2229 207b 0a20  cDelim = "") {. 
+00001f20: 2020 2076 6172 2072 6567 6578 703b 0a20     var regexp;. 
+00001f30: 2020 2076 6172 206d 6174 6368 3b0a 0a20     var match;.. 
+00001f40: 2020 202f 2f20 446f 2077 6520 6368 6563     // Do we chec
+00001f50: 6b20 666f 7220 6c69 6e65 2063 6f6e 7469  k for line conti
+00001f60: 6e75 6174 696f 6e20 6368 6172 6163 7465  nuation characte
+00001f70: 7273 2061 6e64 2022 4845 5245 2d64 6f63  rs and "HERE-doc
+00001f80: 756d 656e 7473 223f 0a20 2020 2076 6172  uments"?.    var
+00001f90: 2075 7365 4c69 6e65 436f 6e74 203d 2021   useLineCont = !
+00001fa0: 216c 696e 6543 6f6e 7469 6e75 6174 696f  !lineContinuatio
+00001fb0: 6e43 6861 720a 2020 2020 7661 7220 7573  nChar.    var us
+00001fc0: 6548 6572 6544 6f63 203d 2021 2168 6572  eHereDoc = !!her
+00001fd0: 6544 6f63 4465 6c69 6d0a 0a20 2020 202f  eDocDelim..    /
+00001fe0: 2f20 6372 6561 7465 2072 6567 6578 7020  / create regexp 
+00001ff0: 746f 2063 6170 7475 7265 2070 726f 6d70  to capture promp
+00002000: 7420 616e 6420 7265 6d61 696e 696e 6720  t and remaining 
+00002010: 6c69 6e65 0a20 2020 2069 6620 2869 7352  line.    if (isR
+00002020: 6567 6578 7029 207b 0a20 2020 2020 2020  egexp) {.       
+00002030: 2072 6567 6578 7020 3d20 6e65 7720 5265   regexp = new Re
+00002040: 6745 7870 2827 5e28 2720 2b20 636f 7079  gExp('^(' + copy
+00002050: 6275 7474 6f6e 5072 6f6d 7074 5465 7874  buttonPromptText
+00002060: 202b 2027 2928 2e2a 2927 290a 2020 2020   + ')(.*)').    
+00002070: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
+00002080: 2072 6567 6578 7020 3d20 6e65 7720 5265   regexp = new Re
+00002090: 6745 7870 2827 5e28 2720 2b20 6573 6361  gExp('^(' + esca
+000020a0: 7065 5265 6745 7870 2863 6f70 7962 7574  peRegExp(copybut
+000020b0: 746f 6e50 726f 6d70 7454 6578 7429 202b  tonPromptText) +
+000020c0: 2027 2928 2e2a 2927 290a 2020 2020 7d0a   ')(.*)').    }.
+000020d0: 0a20 2020 2063 6f6e 7374 206f 7574 7075  .    const outpu
+000020e0: 744c 696e 6573 203d 205b 5d3b 0a20 2020  tLines = [];.   
+000020f0: 2076 6172 2070 726f 6d70 7446 6f75 6e64   var promptFound
+00002100: 203d 2066 616c 7365 3b0a 2020 2020 7661   = false;.    va
+00002110: 7220 676f 744c 696e 6543 6f6e 7420 3d20  r gotLineCont = 
+00002120: 6661 6c73 653b 0a20 2020 2076 6172 2067  false;.    var g
+00002130: 6f74 4865 7265 446f 6320 3d20 6661 6c73  otHereDoc = fals
+00002140: 653b 0a20 2020 2063 6f6e 7374 206c 696e  e;.    const lin
+00002150: 6547 6f74 5072 6f6d 7074 203d 205b 5d3b  eGotPrompt = [];
+00002160: 0a20 2020 2066 6f72 2028 636f 6e73 7420  .    for (const 
+00002170: 6c69 6e65 206f 6620 7465 7874 436f 6e74  line of textCont
+00002180: 656e 742e 7370 6c69 7428 275c 6e27 2929  ent.split('\n'))
+00002190: 207b 0a20 2020 2020 2020 206d 6174 6368   {.        match
+000021a0: 203d 206c 696e 652e 6d61 7463 6828 7265   = line.match(re
+000021b0: 6765 7870 290a 2020 2020 2020 2020 6966  gexp).        if
+000021c0: 2028 6d61 7463 6820 7c7c 2067 6f74 4c69   (match || gotLi
+000021d0: 6e65 436f 6e74 207c 7c20 676f 7448 6572  neCont || gotHer
+000021e0: 6544 6f63 2920 7b0a 2020 2020 2020 2020  eDoc) {.        
+000021f0: 2020 2020 7072 6f6d 7074 466f 756e 6420      promptFound 
+00002200: 3d20 7265 6765 7870 2e74 6573 7428 6c69  = regexp.test(li
+00002210: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+00002220: 6c69 6e65 476f 7450 726f 6d70 742e 7075  lineGotPrompt.pu
+00002230: 7368 2870 726f 6d70 7446 6f75 6e64 290a  sh(promptFound).
+00002240: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00002250: 7265 6d6f 7665 5072 6f6d 7074 7320 2626  removePrompts &&
+00002260: 2070 726f 6d70 7446 6f75 6e64 2920 7b0a   promptFound) {.
+00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002280: 6f75 7470 7574 4c69 6e65 732e 7075 7368  outputLines.push
+00002290: 286d 6174 6368 5b32 5d29 0a20 2020 2020  (match[2]).     
+000022a0: 2020 2020 2020 207d 2065 6c73 6520 7b0a         } else {.
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 6f75 7470 7574 4c69 6e65 732e 7075 7368  outputLines.push
+000022d0: 286c 696e 6529 0a20 2020 2020 2020 2020  (line).         
+000022e0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+000022f0: 2067 6f74 4c69 6e65 436f 6e74 203d 206c   gotLineCont = l
+00002300: 696e 652e 656e 6473 5769 7468 286c 696e  ine.endsWith(lin
+00002310: 6543 6f6e 7469 6e75 6174 696f 6e43 6861  eContinuationCha
+00002320: 7229 2026 2075 7365 4c69 6e65 436f 6e74  r) & useLineCont
+00002330: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002340: 286c 696e 652e 696e 636c 7564 6573 2868  (line.includes(h
+00002350: 6572 6544 6f63 4465 6c69 6d29 2026 2075  ereDocDelim) & u
+00002360: 7365 4865 7265 446f 6329 0a20 2020 2020  seHereDoc).     
+00002370: 2020 2020 2020 2020 2020 2067 6f74 4865             gotHe
+00002380: 7265 446f 6320 3d20 2167 6f74 4865 7265  reDoc = !gotHere
+00002390: 446f 630a 2020 2020 2020 2020 7d20 656c  Doc.        } el
+000023a0: 7365 2069 6620 2821 6f6e 6c79 436f 7079  se if (!onlyCopy
+000023b0: 5072 6f6d 7074 4c69 6e65 7329 207b 0a20  PromptLines) {. 
+000023c0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+000023d0: 744c 696e 6573 2e70 7573 6828 6c69 6e65  tLines.push(line
+000023e0: 290a 2020 2020 2020 2020 7d20 656c 7365  ).        } else
+000023f0: 2069 6620 2863 6f70 7945 6d70 7479 4c69   if (copyEmptyLi
+00002400: 6e65 7320 2626 206c 696e 652e 7472 696d  nes && line.trim
+00002410: 2829 203d 3d3d 2027 2729 207b 0a20 2020  () === '') {.   
+00002420: 2020 2020 2020 2020 206f 7574 7075 744c           outputL
+00002430: 696e 6573 2e70 7573 6828 6c69 6e65 290a  ines.push(line).
+00002440: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
+00002450: 0a20 2020 202f 2f20 4966 206e 6f20 6c69  .    // If no li
+00002460: 6e65 7320 7769 7468 2074 6865 2070 726f  nes with the pro
+00002470: 6d70 7420 7765 7265 2066 6f75 6e64 2074  mpt were found t
+00002480: 6865 6e20 6a75 7374 2075 7365 206f 7269  hen just use ori
+00002490: 6769 6e61 6c20 6c69 6e65 730a 2020 2020  ginal lines.    
+000024a0: 6966 2028 6c69 6e65 476f 7450 726f 6d70  if (lineGotPromp
+000024b0: 742e 736f 6d65 2876 203d 3e20 7620 3d3d  t.some(v => v ==
+000024c0: 3d20 7472 7565 2929 207b 0a20 2020 2020  = true)) {.     
+000024d0: 2020 2074 6578 7443 6f6e 7465 6e74 203d     textContent =
+000024e0: 206f 7574 7075 744c 696e 6573 2e6a 6f69   outputLines.joi
+000024f0: 6e28 275c 6e27 293b 0a20 2020 207d 0a0a  n('\n');.    }..
+00002500: 2020 2020 2f2f 2052 656d 6f76 6520 6120      // Remove a 
+00002510: 7472 6169 6c69 6e67 206e 6577 6c69 6e65  trailing newline
+00002520: 2074 6f20 6176 6f69 6420 6175 746f 2d72   to avoid auto-r
+00002530: 756e 6e69 6e67 2077 6865 6e20 7061 7374  unning when past
+00002540: 696e 670a 2020 2020 6966 2028 7465 7874  ing.    if (text
+00002550: 436f 6e74 656e 742e 656e 6473 5769 7468  Content.endsWith
+00002560: 2822 5c6e 2229 2920 7b0a 2020 2020 2020  ("\n")) {.      
+00002570: 2020 7465 7874 436f 6e74 656e 7420 3d20    textContent = 
+00002580: 7465 7874 436f 6e74 656e 742e 736c 6963  textContent.slic
+00002590: 6528 302c 202d 3129 0a20 2020 207d 0a20  e(0, -1).    }. 
+000025a0: 2020 2072 6574 7572 6e20 7465 7874 436f     return textCo
+000025b0: 6e74 656e 740a 7d0a 948c 1263 6f70 7962  ntent.}....copyb
+000025c0: 7574 746f 6e5f 6578 636c 7564 6594 8c08  utton_exclude...
+000025d0: 2e6c 696e 656e 6f73 948c 0b67 6974 6875  .linenos...githu
+000025e0: 625f 7573 6572 948c 104b 6170 6f6f 726c  b_user...Kapoorl
+000025f0: 6162 732d 4341 5045 4494 8c0b 6769 7468  abs-CAPED...gith
+00002600: 7562 5f72 6570 6f94 8c18 766f 6c6c 7365  ub_repo...vollse
+00002610: 672d 6e61 7061 7269 2d74 7261 636b 6d61  g-napari-trackma
+00002620: 7465 948c 0e67 6974 6875 625f 7665 7273  te...github_vers
+00002630: 696f 6e94 6828 8c0a 6769 7468 7562 5f75  ion.h(..github_u
+00002640: 726c 948c 1268 7474 7073 3a2f 2f67 6974  rl...https://git
+00002650: 6875 622e 636f 6d94 8c08 646f 635f 7061  hub.com...doc_pa
+00002660: 7468 9468 2475 68dc 4e87 948c 1468 746d  th.h$uh.N....htm
+00002670: 6c5f 6f75 7470 7574 5f65 6e63 6f64 696e  l_output_encodin
+00002680: 6794 8c05 7574 662d 3894 68dc 4e87 948c  g...utf-8.h.N...
+00002690: 1268 746d 6c5f 636f 6d70 6163 745f 6c69  .html_compact_li
+000026a0: 7374 7394 8868 dc4e 8794 8c15 6874 6d6c  sts..h.N....html
+000026b0: 5f73 6563 6e75 6d62 6572 5f73 7566 6669  _secnumber_suffi
+000026c0: 7894 8c02 2e20 9468 dc4e 8794 8c14 6874  x.... .h.N....ht
+000026d0: 6d6c 5f73 6561 7263 685f 6c61 6e67 7561  ml_search_langua
+000026e0: 6765 944e 68dc 4e87 948c 1368 746d 6c5f  ge.Nh.N....html_
+000026f0: 7365 6172 6368 5f6f 7074 696f 6e73 947d  search_options.}
+00002700: 9468 dc4e 8794 8c12 6874 6d6c 5f73 6561  .h.N....html_sea
+00002710: 7263 685f 7363 6f72 6572 9468 1f4e 4e87  rch_scorer.h.NN.
+00002720: 948c 1668 746d 6c5f 7363 616c 6564 5f69  ...html_scaled_i
+00002730: 6d61 6765 5f6c 696e 6b94 8868 dc4e 8794  mage_link..h.N..
+00002740: 6847 681f 68dc 4e87 948c 1c68 746d 6c5f  hGh.h.N....html_
+00002750: 636f 6465 626c 6f63 6b5f 6c69 6e65 6e6f  codeblock_lineno
+00002760: 735f 7374 796c 6594 6a86 0100 0068 dc4e  s_style.j....h.N
+00002770: 8794 8c12 6874 6d6c 5f6d 6174 685f 7265  ....html_math_re
+00002780: 6e64 6572 6572 944e 68d8 4e87 948c 0c68  nderer.Nh.N....h
+00002790: 746d 6c34 5f77 7269 7465 7294 8968 dc4e  tml4_writer..h.N
+000027a0: 8794 8c0c 6d61 7468 6a61 785f 7061 7468  ....mathjax_path
+000027b0: 948c 3b68 7474 7073 3a2f 2f63 646e 2e6a  ..;https://cdn.j
+000027c0: 7364 656c 6976 722e 6e65 742f 6e70 6d2f  sdelivr.net/npm/
+000027d0: 6d61 7468 6a61 7840 332f 6573 352f 7465  mathjax@3/es5/te
+000027e0: 782d 6d6d 6c2d 6368 746d 6c2e 6a73 9468  x-mml-chtml.js.h
+000027f0: dc4e 8794 8c0f 6d61 7468 6a61 785f 6f70  .N....mathjax_op
+00002800: 7469 6f6e 7394 7d94 68dc 4e87 948c 0e6d  tions.}.h.N....m
+00002810: 6174 686a 6178 5f69 6e6c 696e 6594 5d94  athjax_inline.].
+00002820: 288c 025c 2894 8c02 5c29 9465 68dc 4e87  (..\(...\).eh.N.
+00002830: 948c 0f6d 6174 686a 6178 5f64 6973 706c  ...mathjax_displ
+00002840: 6179 945d 9428 8c02 5c5b 948c 025c 5d94  ay.].(..\[...\].
+00002850: 6568 dc4e 8794 8c0e 6d61 7468 6a61 785f  eh.N....mathjax_
+00002860: 636f 6e66 6967 944e 68dc 4e87 948c 0f6d  config.Nh.N....m
+00002870: 6174 686a 6178 325f 636f 6e66 6967 944e  athjax2_config.N
+00002880: 68dc 4e87 9468 c768 c868 dc4e 8794 8c0f  h.N..h.h.h.N....
+00002890: 6765 7474 6578 745f 636f 6d70 6163 7494  gettext_compact.
+000028a0: 8868 f14e 8794 8c10 6765 7474 6578 745f  .h.N....gettext_
+000028b0: 6c6f 6361 7469 6f6e 9488 68f1 4e87 948c  location..h.N...
+000028c0: 0c67 6574 7465 7874 5f75 7569 6494 8968  .gettext_uuid..h
+000028d0: f14e 8794 8c12 6765 7474 6578 745f 6175  .N....gettext_au
+000028e0: 746f 5f62 7569 6c64 9488 68d8 4e87 948c  to_build..h.N...
+000028f0: 1a67 6574 7465 7874 5f61 6464 6974 696f  .gettext_additio
+00002900: 6e61 6c5f 7461 7267 6574 7394 5d94 68d8  nal_targets.].h.
+00002910: 4e87 948c 1767 6574 7465 7874 5f6c 6173  N....gettext_las
+00002920: 745f 7472 616e 736c 6174 6f72 948c 1946  t_translator...F
+00002930: 554c 4c20 4e41 4d45 203c 454d 4149 4c40  ULL NAME <EMAIL@
+00002940: 4144 4452 4553 533e 9468 f14e 8794 8c15  ADDRESS>.h.N....
+00002950: 6765 7474 6578 745f 6c61 6e67 7561 6765  gettext_language
+00002960: 5f74 6561 6d94 8c14 4c41 4e47 5541 4745  _team...LANGUAGE
+00002970: 203c 4c4c 406c 692e 6f72 673e 9468 f14e   <LL@li.org>.h.N
+00002980: 8794 6863 6879 4e4e 8794 68cf 68d0 4e4e  ..hchyNN..h.h.NN
+00002990: 8794 8c0a 6c61 7465 785f 6c6f 676f 944e  ....latex_logo.N
+000029a0: 4e4e 8794 8c10 6c61 7465 785f 6170 7065  NN....latex_appe
+000029b0: 6e64 6963 6573 945d 944e 4e87 948c 1b6c  ndices.].NN....l
+000029c0: 6174 6578 5f75 7365 5f6c 6174 6578 5f6d  atex_use_latex_m
+000029d0: 756c 7469 636f 6c75 6d6e 9489 4e4e 8794  ulticolumn..NN..
+000029e0: 8c0f 6c61 7465 785f 7573 655f 7869 6e64  ..latex_use_xind
+000029f0: 7994 884e 4e87 948c 196c 6174 6578 5f74  y..NN....latex_t
+00002a00: 6f70 6c65 7665 6c5f 7365 6374 696f 6e69  oplevel_sectioni
+00002a10: 6e67 944e 4e4e 8794 8c14 6c61 7465 785f  ng.NNN....latex_
+00002a20: 646f 6d61 696e 5f69 6e64 6963 6573 9488  domain_indices..
+00002a30: 4e4e 8794 8c0f 6c61 7465 785f 7368 6f77  NN....latex_show
+00002a40: 5f75 726c 7394 8c02 6e6f 944e 4e87 948c  _urls...no.NN...
+00002a50: 136c 6174 6578 5f73 686f 775f 7061 6765  .latex_show_page
+00002a60: 7265 6673 9489 4e4e 8794 8c0e 6c61 7465  refs..NN....late
+00002a70: 785f 656c 656d 656e 7473 947d 948c 0870  x_elements.}...p
+00002a80: 7265 616d 626c 6594 5898 0100 000a 2020  reamble.X.....  
+00002a90: 2020 2020 2020 2520 5374 6172 7420 6f66        % Start of
+00002aa0: 2070 7265 616d 626c 6520 6465 6669 6e65   preamble define
+00002ab0: 6420 696e 2073 7068 696e 782d 6a75 7079  d in sphinx-jupy
+00002ac0: 7465 7262 6f6f 6b2d 6c61 7465 7820 250a  terbook-latex %.
+00002ad0: 2020 2020 2020 2020 205c 7573 6570 6163           \usepac
+00002ae0: 6b61 6765 5b4c 6174 696e 2c47 7265 656b  kage[Latin,Greek
+00002af0: 5d7b 7563 6861 7263 6c61 7373 6573 7d0a  ]{ucharclasses}.
+00002b00: 2020 2020 2020 2020 5c75 7365 7061 636b          \usepack
+00002b10: 6167 657b 756e 6963 6f64 652d 6d61 7468  age{unicode-math
+00002b20: 7d0a 2020 2020 2020 2020 2520 6669 7869  }.        % fixi
+00002b30: 6e67 2074 6974 6c65 206f 6620 7468 6520  ng title of the 
+00002b40: 746f 630a 2020 2020 2020 2020 5c61 6464  toc.        \add
+00002b50: 746f 5c63 6170 7469 6f6e 7365 6e67 6c69  to\captionsengli
+00002b60: 7368 7b5c 7265 6e65 7763 6f6d 6d61 6e64  sh{\renewcommand
+00002b70: 7b5c 636f 6e74 656e 7473 6e61 6d65 7d7b  {\contentsname}{
+00002b80: 436f 6e74 656e 7473 7d7d 0a20 2020 2020  Contents}}.     
+00002b90: 2020 205c 6879 7065 7273 6574 7570 7b0a     \hypersetup{.
+00002ba0: 2020 2020 2020 2020 2020 2020 7064 6665              pdfe
+00002bb0: 6e63 6f64 696e 673d 6175 746f 2c0a 2020  ncoding=auto,.  
+00002bc0: 2020 2020 2020 2020 2020 7073 6465 7874            psdext
+00002bd0: 7261 0a20 2020 2020 2020 207d 0a20 2020  ra.        }.   
+00002be0: 2020 2020 2025 2045 6e64 206f 6620 7072       % End of pr
+00002bf0: 6561 6d62 6c65 2064 6566 696e 6564 2069  eamble defined i
+00002c00: 6e20 7370 6869 6e78 2d6a 7570 7974 6572  n sphinx-jupyter
+00002c10: 626f 6f6b 2d6c 6174 6578 2025 0a20 2020  book-latex %.   
+00002c20: 2020 2020 2094 734e 4e87 948c 166c 6174       .sNN....lat
+00002c30: 6578 5f61 6464 6974 696f 6e61 6c5f 6669  ex_additional_fi
+00002c40: 6c65 7394 5d94 4e4e 8794 687a 687b 4e4e  les.].NN..hzh{NN
+00002c50: 8794 8c13 6c61 7465 785f 7468 656d 655f  ....latex_theme_
+00002c60: 6f70 7469 6f6e 7394 7d94 4e4e 8794 8c10  options.}.NN....
+00002c70: 6c61 7465 785f 7468 656d 655f 7061 7468  latex_theme_path
+00002c80: 945d 944e 4e87 948c 0e6c 6174 6578 5f64  .].NN....latex_d
+00002c90: 6f63 636c 6173 7394 7d94 4e4e 8794 8c10  occlass.}.NN....
+00002ca0: 6c69 6e6b 6368 6563 6b5f 6967 6e6f 7265  linkcheck_ignore
+00002cb0: 945d 944e 4e87 948c 1b6c 696e 6b63 6865  .].NN....linkche
+00002cc0: 636b 5f65 7863 6c75 6465 5f64 6f63 756d  ck_exclude_docum
+00002cd0: 656e 7473 945d 944e 4e87 948c 1b6c 696e  ents.].NN....lin
+00002ce0: 6b63 6865 636b 5f61 6c6c 6f77 6564 5f72  kcheck_allowed_r
+00002cf0: 6564 6972 6563 7473 947d 944e 4e87 948c  edirects.}.NN...
+00002d00: 0e6c 696e 6b63 6865 636b 5f61 7574 6894  .linkcheck_auth.
+00002d10: 5d94 4e4e 8794 8c19 6c69 6e6b 6368 6563  ].NN....linkchec
+00002d20: 6b5f 7265 7175 6573 745f 6865 6164 6572  k_request_header
+00002d30: 7394 7d94 4e4e 8794 8c11 6c69 6e6b 6368  s.}.NN....linkch
+00002d40: 6563 6b5f 7265 7472 6965 7394 4b01 4e4e  eck_retries.K.NN
+00002d50: 8794 8c11 6c69 6e6b 6368 6563 6b5f 7469  ....linkcheck_ti
+00002d60: 6d65 6f75 7494 4e4e 4e87 948c 116c 696e  meout.NNN....lin
+00002d70: 6b63 6865 636b 5f77 6f72 6b65 7273 944b  kcheck_workers.K
+00002d80: 054e 4e87 948c 116c 696e 6b63 6865 636b  .NN....linkcheck
+00002d90: 5f61 6e63 686f 7273 9488 4e4e 8794 8c18  _anchors..NN....
+00002da0: 6c69 6e6b 6368 6563 6b5f 616e 6368 6f72  linkcheck_anchor
+00002db0: 735f 6967 6e6f 7265 945d 948c 025e 2194  s_ignore.]...^!.
+00002dc0: 614e 4e87 948c 1c6c 696e 6b63 6865 636b  aNN....linkcheck
+00002dd0: 5f72 6174 655f 6c69 6d69 745f 7469 6d65  _rate_limit_time
+00002de0: 6f75 7494 4740 72c0 0000 0000 004e 4e87  out.G@r......NN.
+00002df0: 948c 096d 616e 5f70 6167 6573 945d 9428  ...man_pages.].(
+00002e00: 68a0 8c06 7079 7468 6f6e 948c 0750 7974  h...python...Pyt
+00002e10: 686f 6e20 945d 9468 3a61 4b01 7494 614e  hon .].h:aK.t.aN
+00002e20: 4e87 948c 0d6d 616e 5f73 686f 775f 7572  N....man_show_ur
+00002e30: 6c73 9489 4e4e 8794 8c1a 6d61 6e5f 6d61  ls..NN....man_ma
+00002e40: 6b65 5f73 6563 7469 6f6e 5f64 6972 6563  ke_section_direc
+00002e50: 746f 7279 9489 4e4e 8794 8c13 7369 6e67  tory..NN....sing
+00002e60: 6c65 6874 6d6c 5f73 6964 6562 6172 7394  lehtml_sidebars.
+00002e70: 6aad 0100 0068 dc4e 8794 8c11 7465 7869  j....h.N....texi
+00002e80: 6e66 6f5f 646f 6375 6d65 6e74 7394 5d94  nfo_documents.].
+00002e90: 2868 a08c 0670 7974 686f 6e94 68d7 683a  (h...python.h.h:
+00002ea0: 6a7b 0200 008c 1f4f 6e65 206c 696e 6520  j{.....One line 
+00002eb0: 6465 7363 7269 7074 696f 6e20 6f66 2070  description of p
+00002ec0: 726f 6a65 6374 948c 0d4d 6973 6365 6c6c  roject...Miscell
+00002ed0: 616e 656f 7573 9474 9461 4e4e 8794 8c12  aneous.t.aNN....
+00002ee0: 7465 7869 6e66 6f5f 6170 7065 6e64 6963  texinfo_appendic
+00002ef0: 6573 945d 944e 4e87 948c 1074 6578 696e  es.].NN....texin
+00002f00: 666f 5f65 6c65 6d65 6e74 7394 7d94 4e4e  fo_elements.}.NN
+00002f10: 8794 8c16 7465 7869 6e66 6f5f 646f 6d61  ....texinfo_doma
+00002f20: 696e 5f69 6e64 6963 6573 9488 4e4e 8794  in_indices..NN..
+00002f30: 8c11 7465 7869 6e66 6f5f 7368 6f77 5f75  ..texinfo_show_u
+00002f40: 726c 7394 8c08 666f 6f74 6e6f 7465 944e  rls...footnote.N
+00002f50: 4e87 948c 1574 6578 696e 666f 5f6e 6f5f  N....texinfo_no_
+00002f60: 6465 7461 696c 6d65 6e75 9489 4e4e 8794  detailmenu..NN..
+00002f70: 8c18 7465 7869 6e66 6f5f 6372 6f73 735f  ..texinfo_cross_
+00002f80: 7265 6665 7265 6e63 6573 9488 4e4e 8794  references..NN..
+00002f90: 8c11 7465 7874 5f73 6563 7469 6f6e 6368  ..text_sectionch
+00002fa0: 6172 7394 8c07 2a3d 2d7e 222b 6094 68d8  ars...*=-~"+`.h.
+00002fb0: 4e87 948c 0d74 6578 745f 6e65 776c 696e  N....text_newlin
+00002fc0: 6573 948c 0475 6e69 7894 68d8 4e87 948c  es...unix.h.N...
+00002fd0: 1374 6578 745f 6164 645f 7365 636e 756d  .text_add_secnum
+00002fe0: 6265 7273 9488 68d8 4e87 948c 1574 6578  bers..h.N....tex
+00002ff0: 745f 7365 636e 756d 6265 725f 7375 6666  t_secnumber_suff
+00003000: 6978 948c 022e 2094 68d8 4e87 948c 0a78  ix.... .h.N....x
+00003010: 6d6c 5f70 7265 7474 7994 8868 d84e 8794  ml_pretty..h.N..
+00003020: 8c0f 635f 6964 5f61 7474 7269 6275 7465  ..c_id_attribute
+00003030: 7394 5d94 68d8 4e87 948c 1263 5f70 6172  s.].h.N....c_par
+00003040: 656e 5f61 7474 7269 6275 7465 7394 5d94  en_attributes.].
+00003050: 68d8 4e87 948c 1063 5f65 7874 7261 5f6b  h.N....c_extra_k
+00003060: 6579 776f 7264 7394 5d94 288c 0761 6c69  eywords.].(..ali
+00003070: 676e 6173 948c 0761 6c69 676e 6f66 948c  gnas...alignof..
+00003080: 0462 6f6f 6c94 8c07 636f 6d70 6c65 7894  .bool...complex.
+00003090: 8c09 696d 6167 696e 6172 7994 8c08 6e6f  ..imaginary...no
+000030a0: 7265 7475 726e 948c 0d73 7461 7469 635f  return...static_
+000030b0: 6173 7365 7274 948c 0c74 6872 6561 645f  assert...thread_
+000030c0: 6c6f 6361 6c94 6568 d84e 8794 8c0e 635f  local.eh.N....c_
+000030d0: 616c 6c6f 775f 7072 655f 7633 9489 68d8  allow_pre_v3..h.
+000030e0: 4e87 948c 1863 5f77 6172 6e5f 6f6e 5f61  N....c_warn_on_a
+000030f0: 6c6c 6f77 6564 5f70 7265 5f76 3394 8868  llowed_pre_v3..h
+00003100: d84e 8794 8c17 6370 705f 696e 6465 785f  .N....cpp_index_
+00003110: 636f 6d6d 6f6e 5f70 7265 6669 7894 5d94  common_prefix.].
+00003120: 68d8 4e87 948c 1163 7070 5f69 645f 6174  h.N....cpp_id_at
+00003130: 7472 6962 7574 6573 945d 9468 d84e 8794  tributes.].h.N..
+00003140: 8c14 6370 705f 7061 7265 6e5f 6174 7472  ..cpp_paren_attr
+00003150: 6962 7574 6573 945d 9468 d84e 8794 8c10  ibutes.].h.N....
+00003160: 6370 705f 6465 6275 675f 6c6f 6f6b 7570  cpp_debug_lookup
+00003170: 9489 681f 4e87 948c 1363 7070 5f64 6562  ..h.N....cpp_deb
+00003180: 7567 5f73 686f 775f 7472 6565 9489 681f  ug_show_tree..h.
+00003190: 4e87 948c 1973 7472 6970 5f73 6967 6e61  N....strip_signa
+000031a0: 7475 7265 5f62 6163 6b73 6c61 7368 9489  ture_backslash..
+000031b0: 68d8 4e87 948c 2170 7974 686f 6e5f 7573  h.N...!python_us
+000031c0: 655f 756e 7175 616c 6966 6965 645f 7479  e_unqualified_ty
+000031d0: 7065 5f6e 616d 6573 9489 68d8 4e87 948c  pe_names..h.N...
+000031e0: 1561 7070 6c65 6865 6c70 5f62 756e 646c  .applehelp_bundl
+000031f0: 655f 6e61 6d65 9468 d78c 0961 7070 6c65  e_name.h...apple
+00003200: 6865 6c70 944e 8794 8c13 6170 706c 6568  help.N....appleh
+00003210: 656c 705f 6275 6e64 6c65 5f69 6494 4e6a  elp_bundle_id.Nj
+00003220: c302 0000 4e87 948c 1461 7070 6c65 6865  ....N....applehe
+00003230: 6c70 5f64 6576 5f72 6567 696f 6e94 8c05  lp_dev_region...
+00003240: 656e 2d75 7394 6ac3 0200 004e 8794 8c18  en-us.j....N....
+00003250: 6170 706c 6568 656c 705f 6275 6e64 6c65  applehelp_bundle
+00003260: 5f76 6572 7369 6f6e 948c 0131 946a c302  _version...1.j..
+00003270: 0000 4e87 948c 0e61 7070 6c65 6865 6c70  ..N....applehelp
+00003280: 5f69 636f 6e94 4e6a c302 0000 4e87 948c  _icon.Nj....N...
+00003290: 1461 7070 6c65 6865 6c70 5f6b 625f 7072  .applehelp_kb_pr
+000032a0: 6f64 7563 7494 8c07 5079 7468 6f6e 2d94  oduct...Python-.
+000032b0: 6ac3 0200 004e 8794 8c10 6170 706c 6568  j....N....appleh
+000032c0: 656c 705f 6b62 5f75 726c 944e 6ac3 0200  elp_kb_url.Nj...
+000032d0: 004e 8794 8c14 6170 706c 6568 656c 705f  .N....applehelp_
+000032e0: 7265 6d6f 7465 5f75 726c 944e 6ac3 0200  remote_url.Nj...
+000032f0: 004e 8794 8c17 6170 706c 6568 656c 705f  .N....applehelp_
+00003300: 696e 6465 785f 616e 6368 6f72 7394 896a  index_anchors..j
+00003310: c302 0000 4e87 948c 1961 7070 6c65 6865  ....N....applehe
+00003320: 6c70 5f6d 696e 5f74 6572 6d5f 6c65 6e67  lp_min_term_leng
+00003330: 7468 944e 6ac3 0200 004e 8794 8c13 6170  th.Nj....N....ap
+00003340: 706c 6568 656c 705f 7374 6f70 776f 7264  plehelp_stopword
+00003350: 7394 6a60 0100 006a c302 0000 4e87 948c  s.j`...j....N...
+00003360: 1061 7070 6c65 6865 6c70 5f6c 6f63 616c  .applehelp_local
+00003370: 6594 6a60 0100 006a c302 0000 4e87 948c  e.j`...j....N...
+00003380: 0f61 7070 6c65 6865 6c70 5f74 6974 6c65  .applehelp_title
+00003390: 948c 0b50 7974 686f 6e20 4865 6c70 946a  ...Python Help.j
+000033a0: c302 0000 4e87 948c 1b61 7070 6c65 6865  ....N....applehe
+000033b0: 6c70 5f63 6f64 6573 6967 6e5f 6964 656e  lp_codesign_iden
+000033c0: 7469 7479 944e 6ac3 0200 004e 8794 8c18  tity.Nj....N....
+000033d0: 6170 706c 6568 656c 705f 636f 6465 7369  applehelp_codesi
+000033e0: 676e 5f66 6c61 6773 945d 946a c302 0000  gn_flags.].j....
+000033f0: 4e87 948c 1661 7070 6c65 6865 6c70 5f69  N....applehelp_i
+00003400: 6e64 6578 6572 5f70 6174 6894 8c0f 2f75  ndexer_path.../u
+00003410: 7372 2f62 696e 2f68 6975 7469 6c94 6ac3  sr/bin/hiutil.j.
+00003420: 0200 004e 8794 8c17 6170 706c 6568 656c  ...N....applehel
+00003430: 705f 636f 6465 7369 676e 5f70 6174 6894  p_codesign_path.
+00003440: 8c11 2f75 7372 2f62 696e 2f63 6f64 6573  ../usr/bin/codes
+00003450: 6967 6e94 6ac3 0200 004e 8794 8c20 6170  ign.j....N... ap
+00003460: 706c 6568 656c 705f 6469 7361 626c 655f  plehelp_disable_
+00003470: 6578 7465 726e 616c 5f74 6f6f 6c73 9489  external_tools..
+00003480: 6ac3 0200 004e 8794 8c10 6465 7668 656c  j....N....devhel
+00003490: 705f 6261 7365 6e61 6d65 9468 d78c 0764  p_basename.h...d
+000034a0: 6576 6865 6c70 944e 8794 8c11 6874 6d6c  evhelp.N....html
+000034b0: 6865 6c70 5f62 6173 656e 616d 6594 8c09  help_basename...
+000034c0: 7079 7468 6f6e 646f 6394 681f 4e87 948c  pythondoc.h.N...
+000034d0: 1468 746d 6c68 656c 705f 6669 6c65 5f73  .htmlhelp_file_s
+000034e0: 7566 6669 7894 4e68 dc4e 8794 8c14 6874  uffix.Nh.N....ht
+000034f0: 6d6c 6865 6c70 5f6c 696e 6b5f 7375 6666  mlhelp_link_suff
+00003500: 6978 944e 68dc 4e87 948c 0f71 7468 656c  ix.Nh.N....qthel
+00003510: 705f 6261 7365 6e61 6d65 9468 d768 dc4e  p_basename.h.h.N
+00003520: 8794 8c10 7174 6865 6c70 5f6e 616d 6573  ....qthelp_names
+00003530: 7061 6365 944e 68dc 4e87 948c 0c71 7468  pace.Nh.N....qth
+00003540: 656c 705f 7468 656d 6594 8c05 6e6f 6e61  elp_theme...nona
+00003550: 7694 68dc 4e87 948c 1471 7468 656c 705f  v.h.N....qthelp_
+00003560: 7468 656d 655f 6f70 7469 6f6e 7394 7d94  theme_options.}.
+00003570: 68dc 4e87 948c 1574 6f67 676c 6562 7574  h.N....togglebut
+00003580: 746f 6e5f 7365 6c65 6374 6f72 948c 1d2e  ton_selector....
+00003590: 746f 6767 6c65 2c20 2e61 646d 6f6e 6974  toggle, .admonit
+000035a0: 696f 6e2e 6472 6f70 646f 776e 9468 dc4e  ion.dropdown.h.N
+000035b0: 8794 8c11 746f 6767 6c65 6275 7474 6f6e  ....togglebutton
+000035c0: 5f68 696e 7494 8c0d 436c 6963 6b20 746f  _hint...Click to
+000035d0: 2073 686f 7794 68dc 4e87 948c 1674 6f67   show.h.N....tog
+000035e0: 676c 6562 7574 746f 6e5f 6869 6e74 5f68  glebutton_hint_h
+000035f0: 6964 6594 8c0d 436c 6963 6b20 746f 2068  ide...Click to h
+00003600: 6964 6594 68dc 4e87 948c 1a74 6f67 676c  ide.h.N....toggl
+00003610: 6562 7574 746f 6e5f 6f70 656e 5f6f 6e5f  ebutton_open_on_
+00003620: 7072 696e 7494 8868 dc4e 8794 6ad4 0100  print..h.N..j...
+00003630: 0068 1f68 dc4e 8794 6ad5 0100 0089 68dc  .h.h.N..j.....h.
+00003640: 4e87 946a d601 0000 8868 dc4e 8794 6ad7  N..j.....h.N..j.
+00003650: 0100 0088 68dc 4e87 946a d801 0000 8868  ....h.N..j.....h
+00003660: dc4e 8794 6ad9 0100 0068 1f68 dc4e 8794  .N..j....h.h.N..
+00003670: 6ada 0100 0068 1f68 dc4e 8794 6adb 0100  j....h.h.N..j...
+00003680: 0068 1f68 dc4e 8794 6adc 0100 006a dd01  .h.h.N..j....j..
+00003690: 0000 68dc 4e87 946a e001 0000 6ae1 0100  ..h.N..j....j...
+000036a0: 0068 dc4e 8794 8c15 636f 7079 6275 7474  .h.N....copybutt
+000036b0: 6f6e 5f69 6d61 6765 5f70 6174 6894 681f  on_image_path.h.
+000036c0: 68dc 4e87 948c 146d 7973 745f 636f 6d6d  h.N....myst_comm
+000036d0: 6f6e 6d61 726b 5f6f 6e6c 7994 8968 d84e  onmark_only..h.N
+000036e0: 8794 8c0d 6d79 7374 5f67 666d 5f6f 6e6c  ....myst_gfm_onl
+000036f0: 7994 8968 d84e 8794 8c16 6d79 7374 5f65  y..h.N....myst_e
+00003700: 6e61 626c 655f 6578 7465 6e73 696f 6e73  nable_extensions
+00003710: 9468 4e68 d84e 8794 8c13 6d79 7374 5f64  .hNh.N....myst_d
+00003720: 6973 6162 6c65 5f73 796e 7461 7894 5d94  isable_syntax.].
+00003730: 68d8 4e87 948c 176d 7973 745f 616c 6c5f  h.N....myst_all_
+00003740: 6c69 6e6b 735f 6578 7465 726e 616c 9489  links_external..
+00003750: 68d8 4e87 948c 106d 7973 745f 7572 6c5f  h.N....myst_url_
+00003760: 7363 6865 6d65 7394 6855 68d8 4e87 948c  schemes.hUh.N...
+00003770: 106d 7973 745f 7265 665f 646f 6d61 696e  .myst_ref_domain
+00003780: 7394 4e68 d84e 8794 8c17 6d79 7374 5f6e  s.Nh.N....myst_n
+00003790: 756d 6265 725f 636f 6465 5f62 6c6f 636b  umber_code_block
+000037a0: 7394 5d94 68d8 4e87 948c 146d 7973 745f  s.].h.N....myst_
+000037b0: 7469 746c 655f 746f 5f68 6561 6465 7294  title_to_header.
+000037c0: 8968 d84e 8794 8c14 6d79 7374 5f68 6561  .h.N....myst_hea
+000037d0: 6469 6e67 5f61 6e63 686f 7273 944e 68d8  ding_anchors.Nh.
+000037e0: 4e87 948c 166d 7973 745f 6865 6164 696e  N....myst_headin
+000037f0: 675f 736c 7567 5f66 756e 6394 4e68 d84e  g_slug_func.Nh.N
+00003800: 8794 8c0e 6d79 7374 5f68 746d 6c5f 6d65  ....myst_html_me
+00003810: 7461 947d 9468 d84e 8794 8c18 6d79 7374  ta.}.h.N....myst
+00003820: 5f66 6f6f 746e 6f74 655f 7472 616e 7369  _footnote_transi
+00003830: 7469 6f6e 9488 68d8 4e87 948c 156d 7973  tion..h.N....mys
+00003840: 745f 776f 7264 735f 7065 725f 6d69 6e75  t_words_per_minu
+00003850: 7465 944b c868 d84e 8794 8c12 6d79 7374  te.K.h.N....myst
+00003860: 5f73 7562 7374 6974 7574 696f 6e73 947d  _substitutions.}
+00003870: 9468 d84e 8794 8c13 6d79 7374 5f73 7562  .h.N....myst_sub
+00003880: 5f64 656c 696d 6974 6572 7394 8c01 7b94  _delimiters...{.
+00003890: 8c01 7d94 8694 68d8 4e87 948c 186d 7973  ..}...h.N....mys
+000038a0: 745f 6c69 6e6b 6966 795f 6675 7a7a 795f  t_linkify_fuzzy_
+000038b0: 6c69 6e6b 7394 8868 d84e 8794 8c17 6d79  links..h.N....my
+000038c0: 7374 5f64 6d61 7468 5f61 6c6c 6f77 5f6c  st_dmath_allow_l
+000038d0: 6162 656c 7394 8868 d84e 8794 8c16 6d79  abels..h.N....my
+000038e0: 7374 5f64 6d61 7468 5f61 6c6c 6f77 5f73  st_dmath_allow_s
+000038f0: 7061 6365 9488 68d8 4e87 948c 176d 7973  pace..h.N....mys
+00003900: 745f 646d 6174 685f 616c 6c6f 775f 6469  t_dmath_allow_di
+00003910: 6769 7473 9488 68d8 4e87 948c 186d 7973  gits..h.N....mys
+00003920: 745f 646d 6174 685f 646f 7562 6c65 5f69  t_dmath_double_i
+00003930: 6e6c 696e 6594 8968 d84e 8794 8c13 6d79  nline..h.N....my
+00003940: 7374 5f75 7064 6174 655f 6d61 7468 6a61  st_update_mathja
+00003950: 7894 8868 d84e 8794 8c14 6d79 7374 5f6d  x..h.N....myst_m
+00003960: 6174 686a 6178 5f63 6c61 7373 6573 9468  athjax_classes.h
+00003970: cc68 d84e 8794 8c11 6e62 5f63 7573 746f  .h.N....nb_custo
+00003980: 6d5f 666f 726d 6174 7394 7d94 68d8 4e87  m_formats.}.h.N.
+00003990: 948c 0f6e 625f 6d65 7461 6461 7461 5f6b  ...nb_metadata_k
+000039a0: 6579 948c 066d 7973 746e 6294 68d8 4e87  ey...mystnb.h.N.
+000039b0: 948c 146e 625f 6365 6c6c 5f6d 6574 6164  ...nb_cell_metad
+000039c0: 6174 615f 6b65 7994 6a52 0300 0068 d84e  ata_key.jR...h.N
+000039d0: 8794 8c0d 6e62 5f72 656e 6465 725f 6b65  ....nb_render_ke
+000039e0: 7994 8c09 2d2d 756e 7365 742d 2d94 68d8  y...--unset--.h.
+000039f0: 4e87 948c 156e 625f 6b65 726e 656c 5f72  N....nb_kernel_r
+00003a00: 6778 5f61 6c69 6173 6573 947d 9468 d84e  gx_aliases.}.h.N
+00003a10: 8794 8c11 6e62 5f65 7865 6375 7469 6f6e  ....nb_execution
+00003a20: 5f6d 6f64 6594 6860 68d8 4e87 948c 196a  _mode.h`h.N....j
+00003a30: 7570 7974 6572 5f65 7865 6375 7465 5f6e  upyter_execute_n
+00003a40: 6f74 6562 6f6f 6b73 946a 5703 0000 68d8  otebooks.jW...h.
+00003a50: 4e87 948c 176e 625f 6578 6563 7574 696f  N....nb_executio
+00003a60: 6e5f 6361 6368 655f 7061 7468 9468 1f68  n_cache_path.h.h
+00003a70: d84e 8794 8c0d 6a75 7079 7465 725f 6361  .N....jupyter_ca
+00003a80: 6368 6594 6a57 0300 0068 d84e 8794 8c1c  che.jW...h.N....
+00003a90: 6e62 5f65 7865 6375 7469 6f6e 5f65 7863  nb_execution_exc
+00003aa0: 6c75 6465 7061 7474 6572 6e73 9468 6268  ludepatterns.hbh
+00003ab0: d84e 8794 8c19 6578 6563 7574 696f 6e5f  .N....execution_
+00003ac0: 6578 636c 7564 6570 6174 7465 726e 7394  excludepatterns.
+00003ad0: 6a57 0300 0068 d84e 8794 8c14 6e62 5f65  jW...h.N....nb_e
+00003ae0: 7865 6375 7469 6f6e 5f74 696d 656f 7574  xecution_timeout
+00003af0: 944b 1e68 d84e 8794 8c11 6578 6563 7574  .K.h.N....execut
+00003b00: 696f 6e5f 7469 6d65 6f75 7494 6a57 0300  ion_timeout.jW..
+00003b10: 0068 d84e 8794 8c14 6e62 5f65 7865 6375  .h.N....nb_execu
+00003b20: 7469 6f6e 5f69 6e5f 7465 6d70 9489 68d8  tion_in_temp..h.
+00003b30: 4e87 948c 1165 7865 6375 7469 6f6e 5f69  N....execution_i
+00003b40: 6e5f 7465 6d70 946a 5703 0000 68d8 4e87  n_temp.jW...h.N.
+00003b50: 948c 196e 625f 6578 6563 7574 696f 6e5f  ...nb_execution_
+00003b60: 616c 6c6f 775f 6572 726f 7273 9489 68d8  allow_errors..h.
+00003b70: 4e87 948c 1665 7865 6375 7469 6f6e 5f61  N....execution_a
+00003b80: 6c6c 6f77 5f65 7272 6f72 7394 6a57 0300  llow_errors.jW..
+00003b90: 0068 d84e 8794 8c1b 6e62 5f65 7865 6375  .h.N....nb_execu
+00003ba0: 7469 6f6e 5f72 6169 7365 5f6f 6e5f 6572  tion_raise_on_er
+00003bb0: 726f 7294 8968 d84e 8794 8c14 6e62 5f65  ror..h.N....nb_e
+00003bc0: 7865 6375 7469 6f6e 5f73 686f 775f 7462  xecution_show_tb
+00003bd0: 9489 68d8 4e87 948c 1165 7865 6375 7469  ..h.N....executi
+00003be0: 6f6e 5f73 686f 775f 7462 946a 5703 0000  on_show_tb.jW...
+00003bf0: 68d8 4e87 948c 106e 625f 6d65 7267 655f  h.N....nb_merge_
+00003c00: 7374 7265 616d 7394 8968 d84e 8794 8c10  streams..h.N....
+00003c10: 6e62 5f72 656e 6465 725f 706c 7567 696e  nb_render_plugin
+00003c20: 946a 0701 0000 68d8 4e87 948c 156e 625f  .j....h.N....nb_
+00003c30: 7265 6d6f 7665 5f63 6f64 655f 736f 7572  remove_code_sour
+00003c40: 6365 9489 68d8 4e87 948c 166e 625f 7265  ce..h.N....nb_re
+00003c50: 6d6f 7665 5f63 6f64 655f 6f75 7470 7574  move_code_output
+00003c60: 7394 8968 d84e 8794 8c13 6e62 5f63 6f64  s..h.N....nb_cod
+00003c70: 655f 7072 6f6d 7074 5f73 686f 7794 8c15  e_prompt_show...
+00003c80: 5368 6f77 2063 6f64 6520 6365 6c6c 207b  Show code cell {
+00003c90: 7479 7065 7d94 68d8 4e87 948c 136e 625f  type}.h.N....nb_
+00003ca0: 636f 6465 5f70 726f 6d70 745f 6869 6465  code_prompt_hide
+00003cb0: 948c 1548 6964 6520 636f 6465 2063 656c  ...Hide code cel
+00003cc0: 6c20 7b74 7970 657d 9468 d84e 8794 8c16  l {type}.h.N....
+00003cd0: 6e62 5f6e 756d 6265 725f 736f 7572 6365  nb_number_source
+00003ce0: 5f6c 696e 6573 9489 68d8 4e87 948c 1a6e  _lines..h.N....n
+00003cf0: 625f 6d69 6d65 5f70 7269 6f72 6974 795f  b_mime_priority_
+00003d00: 6f76 6572 7269 6465 7394 2968 d84e 8794  overrides.)h.N..
+00003d10: 8c10 6e62 5f6f 7574 7075 745f 7374 6465  ..nb_output_stde
+00003d20: 7272 9468 5c68 d84e 8794 8c14 6e62 5f72  rr.h\h.N....nb_r
+00003d30: 656e 6465 725f 7465 7874 5f6c 6578 6572  ender_text_lexer
+00003d40: 948c 096d 7973 742d 616e 7369 9468 d84e  ...myst-ansi.h.N
+00003d50: 8794 8c15 6e62 5f72 656e 6465 725f 6572  ....nb_render_er
+00003d60: 726f 725f 6c65 7865 7294 8c09 6970 7974  ror_lexer...ipyt
+00003d70: 686f 6e74 6294 68d8 4e87 948c 176e 625f  hontb.h.N....nb_
+00003d80: 7265 6e64 6572 5f69 6d61 6765 5f6f 7074  render_image_opt
+00003d90: 696f 6e73 947d 9468 d84e 8794 8c18 6e62  ions.}.h.N....nb
+00003da0: 5f72 656e 6465 725f 6669 6775 7265 5f6f  _render_figure_o
+00003db0: 7074 696f 6e73 947d 9468 d84e 8794 8c19  ptions.}.h.N....
+00003dc0: 6e62 5f72 656e 6465 725f 6d61 726b 646f  nb_render_markdo
+00003dd0: 776e 5f66 6f72 6d61 7494 8c0a 636f 6d6d  wn_format...comm
+00003de0: 6f6e 6d61 726b 9468 d84e 8794 8c10 6e62  onmark.h.N....nb
+00003df0: 5f69 7079 7769 6467 6574 735f 6a73 947d  _ipywidgets_js.}
+00003e00: 9428 8c46 6874 7470 733a 2f2f 6364 6e6a  .(.Fhttps://cdnj
+00003e10: 732e 636c 6f75 6466 6c61 7265 2e63 6f6d  s.cloudflare.com
+00003e20: 2f61 6a61 782f 6c69 6273 2f72 6571 7569  /ajax/libs/requi
+00003e30: 7265 2e6a 732f 322e 332e 342f 7265 7175  re.js/2.3.4/requ
+00003e40: 6972 652e 6d69 6e2e 6a73 947d 9428 8c09  ire.min.js.}.(..
+00003e50: 696e 7465 6772 6974 7994 8c33 7368 6132  integrity..3sha2
+00003e60: 3536 2d41 6532 567a 2f34 6550 6449 7536  56-Ae2Vz/4ePdIu6
+00003e70: 5a79 492f 355a 4773 596e 622b 6d30 4a6c  ZyI/5ZGsYnb+m0Jl
+00003e80: 4f6d 4b50 6a74 3658 5a39 4a4a 6b41 3d94  OmKPjt6XZ9JJkA=.
+00003e90: 8c0b 6372 6f73 736f 7269 6769 6e94 8c09  ..crossorigin...
+00003ea0: 616e 6f6e 796d 6f75 7394 758c 5268 7474  anonymous.u.Rhtt
+00003eb0: 7073 3a2f 2f63 646e 2e6a 7364 656c 6976  ps://cdn.jsdeliv
+00003ec0: 722e 6e65 742f 6e70 6d2f 406a 7570 7974  r.net/npm/@jupyt
+00003ed0: 6572 2d77 6964 6765 7473 2f68 746d 6c2d  er-widgets/html-
+00003ee0: 6d61 6e61 6765 7240 312e 302e 362f 6469  manager@1.0.6/di
+00003ef0: 7374 2f65 6d62 6564 2d61 6d64 2e6a 7394  st/embed-amd.js.
+00003f00: 7d94 288c 1864 6174 612d 6a75 7079 7465  }.(..data-jupyte
+00003f10: 722d 7769 6467 6574 732d 6364 6e94 8c1d  r-widgets-cdn...
+00003f20: 6874 7470 733a 2f2f 6364 6e2e 6a73 6465  https://cdn.jsde
+00003f30: 6c69 7672 2e6e 6574 2f6e 706d 2f94 6aa3  livr.net/npm/.j.
+00003f40: 0300 006a a403 0000 7575 68d8 4e87 948c  ...j....uuh.N...
+00003f50: 126e 625f 7265 6e64 6572 5f70 7269 6f72  .nb_render_prior
+00003f60: 6974 7994 6a57 0300 0068 d84e 8794 6865  ity.jW...h.N..he
+00003f70: 8868 d84e 8794 684c 8868 d84e 8794 8c0c  .h.N..hL.h.N....
+00003f80: 7468 6562 655f 636f 6e66 6967 947d 9428  thebe_config.}.(
+00003f90: 8c0b 616c 7761 7973 5f6c 6f61 6494 898c  ..always_load...
+00003fa0: 0873 656c 6563 746f 7294 8c0c 2e74 6865  .selector....the
+00003fb0: 6265 2c2e 6365 6c6c 948c 0e73 656c 6563  be,.cell...selec
+00003fc0: 746f 725f 696e 7075 7494 8c03 7072 6594  tor_input...pre.
+00003fd0: 8c0f 7365 6c65 6374 6f72 5f6f 7574 7075  ..selector_outpu
+00003fe0: 7494 8c15 2e6f 7574 7075 742c 202e 6365  t....output, .ce
+00003ff0: 6c6c 5f6f 7574 7075 7494 7568 dc4e 8794  ll_output.uh.N..
+00004000: 6848 6849 68dc 4e87 9468 6968 6a68 d84e  hHhIh.N..hihjh.N
+00004010: 8794 6845 8968 d84e 8794 8c13 696e 7465  ..hE.h.N....inte
+00004020: 7273 7068 696e 785f 6d61 7070 696e 6794  rsphinx_mapping.
+00004030: 7d94 68d8 4e87 948c 1769 6e74 6572 7370  }.h.N....intersp
+00004040: 6869 6e78 5f63 6163 6865 5f6c 696d 6974  hinx_cache_limit
+00004050: 944b 0568 1f4e 8794 8c13 696e 7465 7273  .K.h.N....inters
+00004060: 7068 696e 785f 7469 6d65 6f75 7494 4e68  phinx_timeout.Nh
+00004070: 1f4e 8794 8c1d 696e 7465 7273 7068 696e  .N....intersphin
+00004080: 785f 6469 7361 626c 6564 5f72 6566 7479  x_disabled_refty
+00004090: 7065 7394 5d94 68d8 4e87 948c 1473 645f  pes.].h.N....sd_
+000040a0: 666f 6e74 6177 6573 6f6d 655f 6c61 7465  fontawesome_late
+000040b0: 7894 8968 d84e 8794 8c14 6269 6274 6578  x..h.N....bibtex
+000040c0: 5f64 6566 6175 6c74 5f73 7479 6c65 948c  _default_style..
+000040d0: 0561 6c70 6861 9468 dc4e 8794 8c0f 6269  .alpha.h.N....bi
+000040e0: 6274 6578 5f74 6f6f 6c74 6970 7394 8868  btex_tooltips..h
+000040f0: dc4e 8794 8c15 6269 6274 6578 5f74 6f6f  .N....bibtex_too
+00004100: 6c74 6970 735f 7374 796c 6594 681f 68dc  ltips_style.h.h.
+00004110: 4e87 9468 6668 6768 dc4e 8794 8c0f 6269  N..hfhgh.N....bi
+00004120: 6274 6578 5f65 6e63 6f64 696e 6794 8c09  btex_encoding...
+00004130: 7574 662d 382d 7369 6794 68dc 4e87 948c  utf-8-sig.h.N...
+00004140: 1a62 6962 7465 785f 6269 626c 696f 6772  .bibtex_bibliogr
+00004150: 6170 6879 5f68 6561 6465 7294 681f 68dc  aphy_header.h.h.
+00004160: 4e87 948c 1e62 6962 7465 785f 666f 6f74  N....bibtex_foot
+00004170: 6269 626c 696f 6772 6170 6879 5f68 6561  bibliography_hea
+00004180: 6465 7294 681f 68dc 4e87 948c 1662 6962  der.h.h.N....bib
+00004190: 7465 785f 7265 6665 7265 6e63 655f 7374  tex_reference_st
+000041a0: 796c 6594 8c05 6c61 6265 6c94 68d8 4e87  yle...label.h.N.
+000041b0: 948c 1b62 6962 7465 785f 666f 6f74 5f72  ...bibtex_foot_r
+000041c0: 6566 6572 656e 6365 5f73 7479 6c65 948c  eference_style..
+000041d0: 0466 6f6f 7494 68d8 4e87 948c 0e62 6962  .foot.h.N....bib
+000041e0: 7465 785f 6369 7465 5f69 6494 681f 68dc  tex_cite_id.h.h.
+000041f0: 4e87 948c 1262 6962 7465 785f 666f 6f74  N....bibtex_foot
+00004200: 6369 7465 5f69 6494 681f 68dc 4e87 948c  cite_id.h.h.N...
+00004210: 1662 6962 7465 785f 6269 626c 696f 6772  .bibtex_bibliogr
+00004220: 6170 6879 5f69 6494 681f 68dc 4e87 948c  aphy_id.h.h.N...
+00004230: 1a62 6962 7465 785f 666f 6f74 6269 626c  .bibtex_footbibl
+00004240: 696f 6772 6170 6879 5f69 6494 681f 68dc  iography_id.h.h.
+00004250: 4e87 948c 196a 626c 6174 6578 5f6c 6f61  N....jblatex_loa
+00004260: 645f 696d 6763 6f6e 7665 7274 6572 9488  d_imgconverter..
+00004270: 68d8 4e87 9468 7c68 7d68 d84e 8794 8c19  h.N..h|h}h.N....
+00004280: 6a62 6c61 7465 785f 6361 7074 696f 6e73  jblatex_captions
+00004290: 5f74 6f5f 7061 7274 7394 4e68 d84e 8794  _to_parts.Nh.N..
+000042a0: 7575 628c 0d63 6f6e 6669 675f 7374 6174  uub..config_stat
+000042b0: 7573 944b 018c 1363 6f6e 6669 675f 7374  us.K...config_st
+000042c0: 6174 7573 5f65 7874 7261 9468 1f8c 0665  atus_extra.h...e
+000042d0: 7665 6e74 7394 4e68 d68c 0e73 7068 696e  vents.Nh...sphin
+000042e0: 782e 7072 6f6a 6563 7494 8c07 5072 6f6a  x.project...Proj
+000042f0: 6563 7494 9394 2981 947d 9428 6808 6809  ect...)..}.(h.h.
+00004300: 6884 6888 8c08 646f 636e 616d 6573 948f  h.h...docnames..
+00004310: 9428 8c09 414c 474f 5249 5448 4d94 8c17  .(..ALGORITHM...
+00004320: 2e6e 6170 6172 692d 6875 622f 4445 5343  .napari-hub/DESC
+00004330: 5249 5054 494f 4e94 8c06 5245 4144 4d45  RIPTION...README
+00004340: 9490 7562 68df 7d94 288c 1073 7068 696e  ..ubh.}.(..sphin
+00004350: 782e 646f 6d61 696e 732e 6394 4b02 8c18  x.domains.c.K...
+00004360: 7370 6869 6e78 2e64 6f6d 6169 6e73 2e63  sphinx.domains.c
+00004370: 6861 6e67 6573 6574 944b 018c 1773 7068  hangeset.K...sph
+00004380: 696e 782e 646f 6d61 696e 732e 6369 7461  inx.domains.cita
+00004390: 7469 6f6e 944b 018c 1273 7068 696e 782e  tion.K...sphinx.
+000043a0: 646f 6d61 696e 732e 6370 7094 4b05 8c14  domains.cpp.K...
+000043b0: 7370 6869 6e78 2e64 6f6d 6169 6e73 2e69  sphinx.domains.i
+000043c0: 6e64 6578 944b 018c 1973 7068 696e 782e  ndex.K...sphinx.
+000043d0: 646f 6d61 696e 732e 6a61 7661 7363 7269  domains.javascri
+000043e0: 7074 944b 028c 1373 7068 696e 782e 646f  pt.K...sphinx.do
+000043f0: 6d61 696e 732e 6d61 7468 944b 028c 1573  mains.math.K...s
+00004400: 7068 696e 782e 646f 6d61 696e 732e 7079  phinx.domains.py
+00004410: 7468 6f6e 944b 038c 1273 7068 696e 782e  thon.K...sphinx.
+00004420: 646f 6d61 696e 732e 7273 7494 4b02 8c12  domains.rst.K...
+00004430: 7370 6869 6e78 2e64 6f6d 6169 6e73 2e73  sphinx.domains.s
+00004440: 7464 944b 0268 754b 0168 774b 0968 134b  td.K.huK.hwK.h.K
+00004450: 3875 8c14 7665 7273 696f 6e69 6e67 5f63  8u..versioning_c
+00004460: 6f6e 6469 7469 6f6e 9489 8c12 7665 7273  ondition....vers
+00004470: 696f 6e69 6e67 5f63 6f6d 7061 7265 9489  ioning_compare..
+00004480: 8c07 646f 6d61 696e 7394 7d94 8c08 7365  ..domains.}...se
+00004490: 7474 696e 6773 947d 9428 8c0e 6175 746f  ttings.}.(..auto
+000044a0: 5f69 645f 7072 6566 6978 948c 0269 6494  _id_prefix...id.
+000044b0: 8c0c 656d 6265 645f 696d 6167 6573 9489  ..embed_images..
+000044c0: 8c10 656d 6265 645f 7374 796c 6573 6865  ..embed_styleshe
+000044d0: 6574 9489 8c15 636c 6f61 6b5f 656d 6169  et....cloak_emai
+000044e0: 6c5f 6164 6472 6573 7365 7394 888c 0c70  l_addresses....p
+000044f0: 6570 5f62 6173 655f 7572 6c94 8c18 6874  ep_base_url...ht
+00004500: 7470 733a 2f2f 7065 7073 2e70 7974 686f  tps://peps.pytho
+00004510: 6e2e 6f72 672f 948c 0e70 6570 5f72 6566  n.org/...pep_ref
+00004520: 6572 656e 6365 7394 4e8c 0c72 6663 5f62  erences.N..rfc_b
+00004530: 6173 655f 7572 6c94 8c26 6874 7470 733a  ase_url..&https:
+00004540: 2f2f 6461 7461 7472 6163 6b65 722e 6965  //datatracker.ie
+00004550: 7466 2e6f 7267 2f64 6f63 2f68 746d 6c2f  tf.org/doc/html/
+00004560: 948c 0e72 6663 5f72 6566 6572 656e 6365  ...rfc_reference
+00004570: 7394 4e8c 0e69 6e70 7574 5f65 6e63 6f64  s.N..input_encod
+00004580: 696e 6794 68f8 8c0e 646f 6374 6974 6c65  ing.h...doctitle
+00004590: 5f78 666f 726d 9489 8c12 7365 6374 7375  _xform....sectsu
+000045a0: 6274 6974 6c65 5f78 666f 726d 9489 8c11  btitle_xform....
+000045b0: 7365 6374 696f 6e5f 7365 6c66 5f6c 696e  section_self_lin
+000045c0: 6b94 898c 0a68 616c 745f 6c65 7665 6c94  k....halt_level.
+000045d0: 4b05 8c16 6669 6c65 5f69 6e73 6572 7469  K...file_inserti
+000045e0: 6f6e 5f65 6e61 626c 6564 9488 8c13 736d  on_enabled....sm
+000045f0: 6172 7471 756f 7465 735f 6c6f 6361 6c65  artquotes_locale
+00004600: 7394 5d94 68d8 6803 6a01 0100 0089 8c0d  s.].h.h.j.......
+00004610: 6c61 6e67 7561 6765 5f63 6f64 6594 6a60  language_code.j`
+00004620: 0100 008c 0c73 6d61 7274 5f71 756f 7465  .....smart_quote
+00004630: 7394 8875 8c08 616c 6c5f 646f 6373 947d  s..u..all_docs.}
+00004640: 9428 6af4 0300 0047 41d9 28a4 b6f4 c1f4  .(j....GA.(.....
+00004650: 6af3 0300 0047 41d9 28a4 b6f8 028e 6af5  j....GA.(.....j.
+00004660: 0300 0047 41d9 28a4 b6fa 1f28 758c 0c64  ...GA.(....(u..d
+00004670: 6570 656e 6465 6e63 6965 7394 6885 8c0b  ependencies.h...
+00004680: 6465 6661 756c 7464 6963 7494 9394 8c08  defaultdict.....
+00004690: 6275 696c 7469 6e73 948c 0373 6574 9493  builtins...set..
+000046a0: 9485 9452 946a f303 0000 8f94 288c 2265  ...R.j......(."e
+000046b0: 7861 6d70 6c65 732f 7669 7375 616c 697a  xamples/visualiz
+000046c0: 655f 706f 696e 745f 636c 6f75 6473 2e70  e_point_clouds.p
+000046d0: 7994 8c1d 6578 616d 706c 6573 2f61 7070  y...examples/app
+000046e0: 6c79 5f61 7574 6f65 6e63 6f64 6572 2e70  ly_autoencoder.p
+000046f0: 7994 8c20 696d 6167 6573 2f70 6f69 6e74  y.. images/point
+00004700: 5f63 6c6f 7564 735f 636f 6d70 6172 6564  _clouds_compared
+00004710: 2e70 6e67 9490 738c 0869 6e63 6c75 6465  .png..s..include
+00004720: 6494 6a20 0400 006a 2304 0000 8594 5294  d.j ...j#.....R.
+00004730: 8c0d 7265 7265 6164 5f61 6c77 6179 7394  ..reread_always.
+00004740: 8f94 8c08 6d65 7461 6461 7461 946a 2004  ....metadata.j .
+00004750: 0000 6a21 0400 008c 0464 6963 7494 9394  ..j!.....dict...
+00004760: 8594 5294 286a f403 0000 7d94 8c09 776f  ..R.(j....}...wo
+00004770: 7264 636f 756e 7494 7d94 288c 0577 6f72  rdcount.}.(..wor
+00004780: 6473 944b c98c 076d 696e 7574 6573 944b  ds.K...minutes.K
+00004790: 0175 736a f303 0000 7d94 6a35 0400 007d  .usj....}.j5...}
+000047a0: 9428 6a37 0400 004d 5102 6a38 0400 004b  .(j7...MQ.j8...K
+000047b0: 0375 736a f503 0000 7d94 6a35 0400 007d  .usj....}.j5...}
+000047c0: 9428 6a37 0400 004b 666a 3804 0000 4b01  .(j7...Kfj8...K.
+000047d0: 7573 758c 0674 6974 6c65 7394 7d94 286a  usu..titles.}.(j
+000047e0: f403 0000 8c0e 646f 6375 7469 6c73 2e6e  ......docutils.n
+000047f0: 6f64 6573 9468 ba93 9429 8194 7d94 288c  odes.h...)..}.(.
+00004800: 0972 6177 736f 7572 6365 9468 1f8c 0863  .rawsource.h...c
+00004810: 6869 6c64 7265 6e94 5d94 6a3f 0400 008c  hildren.].j?....
+00004820: 0454 6578 7494 9394 8c0b 4465 7363 7269  .Text.....Descri
+00004830: 7074 696f 6e94 8594 8194 7d94 286a 4304  ption.....}.(jC.
+00004840: 0000 681f 8c06 7061 7265 6e74 946a 4104  ..h...parent.jA.
+00004850: 0000 7562 618c 0a61 7474 7269 6275 7465  ..uba..attribute
+00004860: 7394 7d94 288c 0369 6473 945d 948c 0763  s.}.(..ids.]...c
+00004870: 6c61 7373 6573 945d 948c 056e 616d 6573  lasses.]...names
+00004880: 945d 948c 0864 7570 6e61 6d65 7394 5d94  .]...dupnames.].
+00004890: 8c08 6261 636b 7265 6673 945d 9475 8c07  ..backrefs.].u..
+000048a0: 7461 676e 616d 6594 68ba 7562 6af3 0300  tagname.h.ubj...
+000048b0: 006a 4004 0000 2981 947d 9428 6a43 0400  .j@...)..}.(jC..
+000048c0: 0068 1f6a 4404 0000 5d94 6a47 0400 008c  .h.jD...].jG....
+000048d0: 0941 6c67 6f72 6974 686d 9485 9481 947d  .Algorithm.....}
+000048e0: 9428 6a43 0400 0068 1f6a 4c04 0000 6a5a  .(jC...h.jL...jZ
+000048f0: 0400 0075 6261 6a4d 0400 007d 9428 6a4f  ...ubajM...}.(jO
+00004900: 0400 005d 946a 5104 0000 5d94 6a53 0400  ...].jQ...].jS..
+00004910: 005d 946a 5504 0000 5d94 6a57 0400 005d  .].jU...].jW...]
+00004920: 9475 6a59 0400 0068 ba75 626a f503 0000  .ujY...h.ubj....
+00004930: 6a40 0400 0029 8194 7d94 286a 4304 0000  j@...)..}.(jC...
+00004940: 681f 6a44 0400 005d 946a 4704 0000 8c18  h.jD...].jG.....
+00004950: 766f 6c6c 7365 672d 6e61 7061 7269 2d74  vollseg-napari-t
+00004960: 7261 636b 6d61 7465 9485 9481 947d 9428  rackmate.....}.(
+00004970: 6a43 0400 0068 1f6a 4c04 0000 6a67 0400  jC...h.jL...jg..
+00004980: 0075 6261 6a4d 0400 007d 9428 6a4f 0400  .ubajM...}.(jO..
+00004990: 005d 946a 5104 0000 5d94 6a53 0400 005d  .].jQ...].jS...]
+000049a0: 946a 5504 0000 5d94 6a57 0400 005d 9475  .jU...].jW...].u
+000049b0: 6a59 0400 0068 ba75 6275 8c0a 6c6f 6e67  jY...h.ubu..long
+000049c0: 7469 746c 6573 947d 9428 6af4 0300 006a  titles.}.(j....j
+000049d0: 4104 0000 6af3 0300 006a 5a04 0000 6af5  A...j....jZ...j.
+000049e0: 0300 006a 6704 0000 758c 0474 6f63 7394  ...jg...u..tocs.
+000049f0: 7d94 286a f403 0000 6a3f 0400 008c 0b62  }.(j....j?.....b
+00004a00: 756c 6c65 745f 6c69 7374 9493 9429 8194  ullet_list...)..
+00004a10: 7d94 286a 4304 0000 681f 6a44 0400 005d  }.(jC...h.jD...]
+00004a20: 9428 6a3f 0400 008c 096c 6973 745f 6974  .(j?.....list_it
+00004a30: 656d 9493 9429 8194 7d94 286a 4304 0000  em...)..}.(jC...
+00004a40: 681f 6a44 0400 005d 948c 0f73 7068 696e  h.jD...]...sphin
+00004a50: 782e 6164 646e 6f64 6573 948c 1163 6f6d  x.addnodes...com
+00004a60: 7061 6374 5f70 6172 6167 7261 7068 9493  pact_paragraph..
+00004a70: 9429 8194 7d94 286a 4304 0000 681f 6a44  .)..}.(jC...h.jD
+00004a80: 0400 005d 946a 3f04 0000 8c09 7265 6665  ...].j?.....refe
+00004a90: 7265 6e63 6594 9394 2981 947d 9428 6a43  rence...)..}.(jC
+00004aa0: 0400 0068 1f6a 4404 0000 5d94 6a47 0400  ...h.jD...].jG..
+00004ab0: 008c 0b44 6573 6372 6970 7469 6f6e 9485  ...Description..
+00004ac0: 9481 947d 9428 6a43 0400 0068 1f6a 4c04  ...}.(jC...h.jL.
+00004ad0: 0000 6a8a 0400 0075 6261 6a4d 0400 007d  ..j....ubajM...}
+00004ae0: 9428 6a4f 0400 005d 946a 5104 0000 5d94  .(jO...].jQ...].
+00004af0: 6a53 0400 005d 946a 5504 0000 5d94 6a57  jS...].jU...].jW
+00004b00: 0400 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
+00004b10: 888c 0672 6566 7572 6994 6af4 0300 008c  ...refuri.j.....
+00004b20: 0a61 6e63 686f 726e 616d 6594 681f 756a  .anchorname.h.uj
+00004b30: 5904 0000 6a88 0400 006a 4c04 0000 6a85  Y...j....jL...j.
+00004b40: 0400 0075 6261 6a4d 0400 007d 9428 6a4f  ...ubajM...}.(jO
+00004b50: 0400 005d 946a 5104 0000 5d94 6a53 0400  ...].jQ...].jS..
+00004b60: 005d 946a 5504 0000 5d94 6a57 0400 005d  .].jU...].jW...]
+00004b70: 9475 6a59 0400 006a 8304 0000 6a4c 0400  .ujY...j....jL..
+00004b80: 006a 7f04 0000 7562 616a 4d04 0000 7d94  .j....ubajM...}.
+00004b90: 286a 4f04 0000 5d94 6a51 0400 005d 946a  (jO...].jQ...].j
+00004ba0: 5304 0000 5d94 6a55 0400 005d 946a 5704  S...].jU...].jW.
+00004bb0: 0000 5d94 756a 5904 0000 6a7d 0400 006a  ..].ujY...j}...j
+00004bc0: 4c04 0000 6a7a 0400 0075 626a 7e04 0000  L...jz...ubj~...
+00004bd0: 2981 947d 9428 6a43 0400 0068 1f6a 4404  )..}.(jC...h.jD.
+00004be0: 0000 5d94 6a84 0400 0029 8194 7d94 286a  ..].j....)..}.(j
+00004bf0: 4304 0000 681f 6a44 0400 005d 946a 8904  C...h.jD...].j..
+00004c00: 0000 2981 947d 9428 6a43 0400 0068 1f6a  ..)..}.(jC...h.j
+00004c10: 4404 0000 5d94 6a47 0400 008c 1057 686f  D...].jG.....Who
+00004c20: 2069 7320 5468 6973 2046 6f72 3f94 8594   is This For?...
+00004c30: 8194 7d94 286a 4304 0000 681f 6a4c 0400  ..}.(jC...h.jL..
+00004c40: 006a ac04 0000 7562 616a 4d04 0000 7d94  .j....ubajM...}.
+00004c50: 286a 4f04 0000 5d94 6a51 0400 005d 946a  (jO...].jQ...].j
+00004c60: 5304 0000 5d94 6a55 0400 005d 946a 5704  S...].jU...].jW.
+00004c70: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
+00004c80: 8c06 7265 6675 7269 946a f403 0000 8c0a  ..refuri.j......
+00004c90: 616e 6368 6f72 6e61 6d65 948c 1023 7768  anchorname...#wh
+00004ca0: 6f2d 6973 2d74 6869 732d 666f 7294 756a  o-is-this-for.uj
+00004cb0: 5904 0000 6a88 0400 006a 4c04 0000 6aa9  Y...j....jL...j.
+00004cc0: 0400 0075 6261 6a4d 0400 007d 9428 6a4f  ...ubajM...}.(jO
+00004cd0: 0400 005d 946a 5104 0000 5d94 6a53 0400  ...].jQ...].jS..
+00004ce0: 005d 946a 5504 0000 5d94 6a57 0400 005d  .].jU...].jW...]
+00004cf0: 9475 6a59 0400 006a 8304 0000 6a4c 0400  .ujY...j....jL..
+00004d00: 006a a604 0000 7562 616a 4d04 0000 7d94  .j....ubajM...}.
+00004d10: 286a 4f04 0000 5d94 6a51 0400 005d 946a  (jO...].jQ...].j
+00004d20: 5304 0000 5d94 6a55 0400 005d 946a 5704  S...].jU...].jW.
+00004d30: 0000 5d94 756a 5904 0000 6a7d 0400 006a  ..].ujY...j}...j
+00004d40: 4c04 0000 6a7a 0400 0075 626a 7e04 0000  L...jz...ubj~...
+00004d50: 2981 947d 9428 6a43 0400 0068 1f6a 4404  )..}.(jC...h.jD.
+00004d60: 0000 5d94 6a84 0400 0029 8194 7d94 286a  ..].j....)..}.(j
+00004d70: 4304 0000 681f 6a44 0400 005d 946a 8904  C...h.jD...].j..
+00004d80: 0000 2981 947d 9428 6a43 0400 0068 1f6a  ..)..}.(jC...h.j
+00004d90: 4404 0000 5d94 6a47 0400 008c 0c48 6f77  D...].jG.....How
+00004da0: 2074 6f20 4775 6964 6594 8594 8194 7d94   to Guide.....}.
+00004db0: 286a 4304 0000 681f 6a4c 0400 006a cf04  (jC...h.jL...j..
+00004dc0: 0000 7562 616a 4d04 0000 7d94 286a 4f04  ..ubajM...}.(jO.
+00004dd0: 0000 5d94 6a51 0400 005d 946a 5304 0000  ..].jQ...].jS...
+00004de0: 5d94 6a55 0400 005d 946a 5704 0000 5d94  ].jU...].jW...].
+00004df0: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
+00004e00: 6675 7269 946a f403 0000 8c0a 616e 6368  furi.j......anch
+00004e10: 6f72 6e61 6d65 948c 0d23 686f 772d 746f  orname...#how-to
+00004e20: 2d67 7569 6465 9475 6a59 0400 006a 8804  -guide.ujY...j..
+00004e30: 0000 6a4c 0400 006a cc04 0000 7562 616a  ..jL...j....ubaj
+00004e40: 4d04 0000 7d94 286a 4f04 0000 5d94 6a51  M...}.(jO...].jQ
+00004e50: 0400 005d 946a 5304 0000 5d94 6a55 0400  ...].jS...].jU..
+00004e60: 005d 946a 5704 0000 5d94 756a 5904 0000  .].jW...].ujY...
+00004e70: 6a83 0400 006a 4c04 0000 6ac9 0400 0075  j....jL...j....u
+00004e80: 6261 6a4d 0400 007d 9428 6a4f 0400 005d  bajM...}.(jO...]
+00004e90: 946a 5104 0000 5d94 6a53 0400 005d 946a  .jQ...].jS...].j
+00004ea0: 5504 0000 5d94 6a57 0400 005d 9475 6a59  U...].jW...].ujY
+00004eb0: 0400 006a 7d04 0000 6a4c 0400 006a 7a04  ...j}...jL...jz.
+00004ec0: 0000 7562 6a7e 0400 0029 8194 7d94 286a  ..ubj~...)..}.(j
+00004ed0: 4304 0000 681f 6a44 0400 005d 946a 8404  C...h.jD...].j..
+00004ee0: 0000 2981 947d 9428 6a43 0400 0068 1f6a  ..)..}.(jC...h.j
+00004ef0: 4404 0000 5d94 6a89 0400 0029 8194 7d94  D...].j....)..}.
+00004f00: 286a 4304 0000 681f 6a44 0400 005d 946a  (jC...h.jD...].j
+00004f10: 4704 0000 8c0c 4765 7474 696e 6720 4865  G.....Getting He
+00004f20: 6c70 9485 9481 947d 9428 6a43 0400 0068  lp.....}.(jC...h
+00004f30: 1f6a 4c04 0000 6af2 0400 0075 6261 6a4d  .jL...j....ubajM
+00004f40: 0400 007d 9428 6a4f 0400 005d 946a 5104  ...}.(jO...].jQ.
+00004f50: 0000 5d94 6a53 0400 005d 946a 5504 0000  ..].jS...].jU...
+00004f60: 5d94 6a57 0400 005d 948c 0869 6e74 6572  ].jW...]...inter
+00004f70: 6e61 6c94 888c 0672 6566 7572 6994 6af4  nal....refuri.j.
+00004f80: 0300 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
+00004f90: 8c0d 2367 6574 7469 6e67 2d68 656c 7094  ..#getting-help.
+00004fa0: 756a 5904 0000 6a88 0400 006a 4c04 0000  ujY...j....jL...
+00004fb0: 6aef 0400 0075 6261 6a4d 0400 007d 9428  j....ubajM...}.(
+00004fc0: 6a4f 0400 005d 946a 5104 0000 5d94 6a53  jO...].jQ...].jS
+00004fd0: 0400 005d 946a 5504 0000 5d94 6a57 0400  ...].jU...].jW..
+00004fe0: 005d 9475 6a59 0400 006a 8304 0000 6a4c  .].ujY...j....jL
+00004ff0: 0400 006a ec04 0000 7562 616a 4d04 0000  ...j....ubajM...
+00005000: 7d94 286a 4f04 0000 5d94 6a51 0400 005d  }.(jO...].jQ...]
+00005010: 946a 5304 0000 5d94 6a55 0400 005d 946a  .jS...].jU...].j
+00005020: 5704 0000 5d94 756a 5904 0000 6a7d 0400  W...].ujY...j}..
+00005030: 006a 4c04 0000 6a7a 0400 0075 626a 7e04  .jL...jz...ubj~.
+00005040: 0000 2981 947d 9428 6a43 0400 0068 1f6a  ..)..}.(jC...h.j
+00005050: 4404 0000 5d94 6a84 0400 0029 8194 7d94  D...].j....)..}.
+00005060: 286a 4304 0000 681f 6a44 0400 005d 946a  (jC...h.jD...].j
+00005070: 8904 0000 2981 947d 9428 6a43 0400 0068  ....)..}.(jC...h
+00005080: 1f6a 4404 0000 5d94 6a47 0400 008c 0b48  .jD...].jG.....H
+00005090: 6f77 2074 6f20 4369 7465 9485 9481 947d  ow to Cite.....}
+000050a0: 9428 6a43 0400 0068 1f6a 4c04 0000 6a15  .(jC...h.jL...j.
+000050b0: 0500 0075 6261 6a4d 0400 007d 9428 6a4f  ...ubajM...}.(jO
+000050c0: 0400 005d 946a 5104 0000 5d94 6a53 0400  ...].jQ...].jS..
+000050d0: 005d 946a 5504 0000 5d94 6a57 0400 005d  .].jU...].jW...]
+000050e0: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
+000050f0: 6566 7572 6994 6af4 0300 008c 0a61 6e63  efuri.j......anc
+00005100: 686f 726e 616d 6594 8c0c 2368 6f77 2d74  horname...#how-t
+00005110: 6f2d 6369 7465 9475 6a59 0400 006a 8804  o-cite.ujY...j..
+00005120: 0000 6a4c 0400 006a 1205 0000 7562 616a  ..jL...j....ubaj
+00005130: 4d04 0000 7d94 286a 4f04 0000 5d94 6a51  M...}.(jO...].jQ
+00005140: 0400 005d 946a 5304 0000 5d94 6a55 0400  ...].jS...].jU..
+00005150: 005d 946a 5704 0000 5d94 756a 5904 0000  .].jW...].ujY...
+00005160: 6a83 0400 006a 4c04 0000 6a0f 0500 0075  j....jL...j....u
+00005170: 6261 6a4d 0400 007d 9428 6a4f 0400 005d  bajM...}.(jO...]
+00005180: 946a 5104 0000 5d94 6a53 0400 005d 946a  .jQ...].jS...].j
+00005190: 5504 0000 5d94 6a57 0400 005d 9475 6a59  U...].jW...].ujY
+000051a0: 0400 006a 7d04 0000 6a4c 0400 006a 7a04  ...j}...jL...jz.
+000051b0: 0000 7562 656a 4d04 0000 7d94 286a 4f04  ..ubejM...}.(jO.
+000051c0: 0000 5d94 6a51 0400 005d 946a 5304 0000  ..].jQ...].jS...
+000051d0: 5d94 6a55 0400 005d 946a 5704 0000 5d94  ].jU...].jW...].
+000051e0: 756a 5904 0000 6a78 0400 0075 626a f303  ujY...jx...ubj..
+000051f0: 0000 6a79 0400 0029 8194 7d94 286a 4304  ..jy...)..}.(jC.
+00005200: 0000 681f 6a44 0400 005d 946a 7e04 0000  ..h.jD...].j~...
+00005210: 2981 947d 9428 6a43 0400 0068 1f6a 4404  )..}.(jC...h.jD.
+00005220: 0000 5d94 286a 8404 0000 2981 947d 9428  ..].(j....)..}.(
+00005230: 6a43 0400 0068 1f6a 4404 0000 5d94 6a89  jC...h.jD...].j.
+00005240: 0400 0029 8194 7d94 286a 4304 0000 681f  ...)..}.(jC...h.
+00005250: 6a44 0400 005d 946a 4704 0000 8c09 416c  jD...].jG.....Al
+00005260: 676f 7269 7468 6d94 8594 8194 7d94 286a  gorithm.....}.(j
+00005270: 4304 0000 681f 6a4c 0400 006a 4105 0000  C...h.jL...jA...
+00005280: 7562 616a 4d04 0000 7d94 286a 4f04 0000  ubajM...}.(jO...
+00005290: 5d94 6a51 0400 005d 946a 5304 0000 5d94  ].jQ...].jS...].
+000052a0: 6a55 0400 005d 946a 5704 0000 5d94 8c08  jU...].jW...]...
+000052b0: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
+000052c0: 7269 946a f303 0000 8c0a 616e 6368 6f72  ri.j......anchor
+000052d0: 6e61 6d65 9468 1f75 6a59 0400 006a 8804  name.h.ujY...j..
+000052e0: 0000 6a4c 0400 006a 3e05 0000 7562 616a  ..jL...j>...ubaj
+000052f0: 4d04 0000 7d94 286a 4f04 0000 5d94 6a51  M...}.(jO...].jQ
+00005300: 0400 005d 946a 5304 0000 5d94 6a55 0400  ...].jS...].jU..
+00005310: 005d 946a 5704 0000 5d94 756a 5904 0000  .].jW...].ujY...
+00005320: 6a83 0400 006a 4c04 0000 6a3b 0500 0075  j....jL...j;...u
+00005330: 626a 7904 0000 2981 947d 9428 6a43 0400  bjy...)..}.(jC..
+00005340: 0068 1f6a 4404 0000 5d94 286a 7e04 0000  .h.jD...].(j~...
+00005350: 2981 947d 9428 6a43 0400 0068 1f6a 4404  )..}.(jC...h.jD.
+00005360: 0000 5d94 6a84 0400 0029 8194 7d94 286a  ..].j....)..}.(j
+00005370: 4304 0000 681f 6a44 0400 005d 946a 8904  C...h.jD...].j..
+00005380: 0000 2981 947d 9428 6a43 0400 0068 1f6a  ..)..}.(jC...h.j
+00005390: 4404 0000 5d94 6a47 0400 008c 1953 6567  D...].jG.....Seg
+000053a0: 6d65 6e74 6174 696f 6e20 616e 6420 5472  mentation and Tr
+000053b0: 6163 6b69 6e67 9485 9481 947d 9428 6a43  acking.....}.(jC
+000053c0: 0400 0068 1f6a 4c04 0000 6a60 0500 0075  ...h.jL...j`...u
+000053d0: 6261 6a4d 0400 007d 9428 6a4f 0400 005d  bajM...}.(jO...]
+000053e0: 946a 5104 0000 5d94 6a53 0400 005d 946a  .jQ...].jS...].j
+000053f0: 5504 0000 5d94 6a57 0400 005d 948c 0869  U...].jW...]...i
+00005400: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
+00005410: 6994 6af3 0300 008c 0a61 6e63 686f 726e  i.j......anchorn
+00005420: 616d 6594 8c1a 2373 6567 6d65 6e74 6174  ame...#segmentat
+00005430: 696f 6e2d 616e 642d 7472 6163 6b69 6e67  ion-and-tracking
+00005440: 9475 6a59 0400 006a 8804 0000 6a4c 0400  .ujY...j....jL..
+00005450: 006a 5d05 0000 7562 616a 4d04 0000 7d94  .j]...ubajM...}.
+00005460: 286a 4f04 0000 5d94 6a51 0400 005d 946a  (jO...].jQ...].j
+00005470: 5304 0000 5d94 6a55 0400 005d 946a 5704  S...].jU...].jW.
+00005480: 0000 5d94 756a 5904 0000 6a83 0400 006a  ..].ujY...j....j
+00005490: 4c04 0000 6a5a 0500 0075 6261 6a4d 0400  L...jZ...ubajM..
+000054a0: 007d 9428 6a4f 0400 005d 946a 5104 0000  .}.(jO...].jQ...
+000054b0: 5d94 6a53 0400 005d 946a 5504 0000 5d94  ].jS...].jU...].
+000054c0: 6a57 0400 005d 9475 6a59 0400 006a 7d04  jW...].ujY...j}.
+000054d0: 0000 6a4c 0400 006a 5705 0000 7562 6a7e  ..jL...jW...ubj~
+000054e0: 0400 0029 8194 7d94 286a 4304 0000 681f  ...)..}.(jC...h.
+000054f0: 6a44 0400 005d 946a 8404 0000 2981 947d  jD...].j....)..}
+00005500: 9428 6a43 0400 0068 1f6a 4404 0000 5d94  .(jC...h.jD...].
+00005510: 6a89 0400 0029 8194 7d94 286a 4304 0000  j....)..}.(jC...
+00005520: 681f 6a44 0400 005d 946a 4704 0000 8c0c  h.jD...].jG.....
+00005530: 506f 696e 7420 436c 6f75 6473 9485 9481  Point Clouds....
+00005540: 947d 9428 6a43 0400 0068 1f6a 4c04 0000  .}.(jC...h.jL...
+00005550: 6a83 0500 0075 6261 6a4d 0400 007d 9428  j....ubajM...}.(
+00005560: 6a4f 0400 005d 946a 5104 0000 5d94 6a53  jO...].jQ...].jS
+00005570: 0400 005d 946a 5504 0000 5d94 6a57 0400  ...].jU...].jW..
+00005580: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
+00005590: 0672 6566 7572 6994 6af3 0300 008c 0a61  .refuri.j......a
+000055a0: 6e63 686f 726e 616d 6594 8c0d 2370 6f69  nchorname...#poi
+000055b0: 6e74 2d63 6c6f 7564 7394 756a 5904 0000  nt-clouds.ujY...
+000055c0: 6a88 0400 006a 4c04 0000 6a80 0500 0075  j....jL...j....u
+000055d0: 6261 6a4d 0400 007d 9428 6a4f 0400 005d  bajM...}.(jO...]
+000055e0: 946a 5104 0000 5d94 6a53 0400 005d 946a  .jQ...].jS...].j
+000055f0: 5504 0000 5d94 6a57 0400 005d 9475 6a59  U...].jW...].ujY
+00005600: 0400 006a 8304 0000 6a4c 0400 006a 7d05  ...j....jL...j}.
+00005610: 0000 7562 616a 4d04 0000 7d94 286a 4f04  ..ubajM...}.(jO.
+00005620: 0000 5d94 6a51 0400 005d 946a 5304 0000  ..].jQ...].jS...
+00005630: 5d94 6a55 0400 005d 946a 5704 0000 5d94  ].jU...].jW...].
+00005640: 756a 5904 0000 6a7d 0400 006a 4c04 0000  ujY...j}...jL...
+00005650: 6a57 0500 0075 626a 7e04 0000 2981 947d  jW...ubj~...)..}
+00005660: 9428 6a43 0400 0068 1f6a 4404 0000 5d94  .(jC...h.jD...].
+00005670: 6a84 0400 0029 8194 7d94 286a 4304 0000  j....)..}.(jC...
+00005680: 681f 6a44 0400 005d 946a 8904 0000 2981  h.jD...].j....).
+00005690: 947d 9428 6a43 0400 0068 1f6a 4404 0000  .}.(jC...h.jD...
+000056a0: 5d94 6a47 0400 008c 0b41 7574 6f65 6e63  ].jG.....Autoenc
+000056b0: 6f64 6572 9485 9481 947d 9428 6a43 0400  oder.....}.(jC..
+000056c0: 0068 1f6a 4c04 0000 6aa6 0500 0075 6261  .h.jL...j....uba
+000056d0: 6a4d 0400 007d 9428 6a4f 0400 005d 946a  jM...}.(jO...].j
+000056e0: 5104 0000 5d94 6a53 0400 005d 946a 5504  Q...].jS...].jU.
+000056f0: 0000 5d94 6a57 0400 005d 948c 0869 6e74  ..].jW...]...int
+00005700: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
+00005710: 6af3 0300 008c 0a61 6e63 686f 726e 616d  j......anchornam
+00005720: 6594 8c0c 2361 7574 6f65 6e63 6f64 6572  e...#autoencoder
+00005730: 9475 6a59 0400 006a 8804 0000 6a4c 0400  .ujY...j....jL..
+00005740: 006a a305 0000 7562 616a 4d04 0000 7d94  .j....ubajM...}.
+00005750: 286a 4f04 0000 5d94 6a51 0400 005d 946a  (jO...].jQ...].j
+00005760: 5304 0000 5d94 6a55 0400 005d 946a 5704  S...].jU...].jW.
+00005770: 0000 5d94 756a 5904 0000 6a83 0400 006a  ..].ujY...j....j
+00005780: 4c04 0000 6aa0 0500 0075 6261 6a4d 0400  L...j....ubajM..
+00005790: 007d 9428 6a4f 0400 005d 946a 5104 0000  .}.(jO...].jQ...
+000057a0: 5d94 6a53 0400 005d 946a 5504 0000 5d94  ].jS...].jU...].
+000057b0: 6a57 0400 005d 9475 6a59 0400 006a 7d04  jW...].ujY...j}.
+000057c0: 0000 6a4c 0400 006a 5705 0000 7562 6a7e  ..jL...jW...ubj~
+000057d0: 0400 0029 8194 7d94 286a 4304 0000 681f  ...)..}.(jC...h.
+000057e0: 6a44 0400 005d 946a 8404 0000 2981 947d  jD...].j....)..}
+000057f0: 9428 6a43 0400 0068 1f6a 4404 0000 5d94  .(jC...h.jD...].
+00005800: 6a89 0400 0029 8194 7d94 286a 4304 0000  j....)..}.(jC...
+00005810: 681f 6a44 0400 005d 946a 4704 0000 8c0e  h.jD...].jG.....
+00005820: 5368 6170 6520 4665 6174 7572 6573 9485  Shape Features..
+00005830: 9481 947d 9428 6a43 0400 0068 1f6a 4c04  ...}.(jC...h.jL.
+00005840: 0000 6ac9 0500 0075 6261 6a4d 0400 007d  ..j....ubajM...}
+00005850: 9428 6a4f 0400 005d 946a 5104 0000 5d94  .(jO...].jQ...].
+00005860: 6a53 0400 005d 946a 5504 0000 5d94 6a57  jS...].jU...].jW
+00005870: 0400 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
+00005880: 888c 0672 6566 7572 6994 6af3 0300 008c  ...refuri.j.....
+00005890: 0a61 6e63 686f 726e 616d 6594 8c0f 2373  .anchorname...#s
+000058a0: 6861 7065 2d66 6561 7475 7265 7394 756a  hape-features.uj
+000058b0: 5904 0000 6a88 0400 006a 4c04 0000 6ac6  Y...j....jL...j.
+000058c0: 0500 0075 6261 6a4d 0400 007d 9428 6a4f  ...ubajM...}.(jO
+000058d0: 0400 005d 946a 5104 0000 5d94 6a53 0400  ...].jQ...].jS..
+000058e0: 005d 946a 5504 0000 5d94 6a57 0400 005d  .].jU...].jW...]
+000058f0: 9475 6a59 0400 006a 8304 0000 6a4c 0400  .ujY...j....jL..
+00005900: 006a c305 0000 7562 616a 4d04 0000 7d94  .j....ubajM...}.
+00005910: 286a 4f04 0000 5d94 6a51 0400 005d 946a  (jO...].jQ...].j
+00005920: 5304 0000 5d94 6a55 0400 005d 946a 5704  S...].jU...].jW.
+00005930: 0000 5d94 756a 5904 0000 6a7d 0400 006a  ..].ujY...j}...j
+00005940: 4c04 0000 6a57 0500 0075 626a 7e04 0000  L...jW...ubj~...
+00005950: 2981 947d 9428 6a43 0400 0068 1f6a 4404  )..}.(jC...h.jD.
+00005960: 0000 5d94 6a84 0400 0029 8194 7d94 286a  ..].j....)..}.(j
+00005970: 4304 0000 681f 6a44 0400 005d 946a 8904  C...h.jD...].j..
+00005980: 0000 2981 947d 9428 6a43 0400 0068 1f6a  ..)..}.(jC...h.j
+00005990: 4404 0000 5d94 6a47 0400 008c 1044 796e  D...].jG.....Dyn
+000059a0: 616d 6963 2046 6561 7475 7265 7394 8594  amic Features...
+000059b0: 8194 7d94 286a 4304 0000 681f 6a4c 0400  ..}.(jC...h.jL..
+000059c0: 006a ec05 0000 7562 616a 4d04 0000 7d94  .j....ubajM...}.
+000059d0: 286a 4f04 0000 5d94 6a51 0400 005d 946a  (jO...].jQ...].j
+000059e0: 5304 0000 5d94 6a55 0400 005d 946a 5704  S...].jU...].jW.
+000059f0: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
+00005a00: 8c06 7265 6675 7269 946a f303 0000 8c0a  ..refuri.j......
+00005a10: 616e 6368 6f72 6e61 6d65 948c 1123 6479  anchorname...#dy
+00005a20: 6e61 6d69 632d 6665 6174 7572 6573 9475  namic-features.u
+00005a30: 6a59 0400 006a 8804 0000 6a4c 0400 006a  jY...j....jL...j
+00005a40: e905 0000 7562 616a 4d04 0000 7d94 286a  ....ubajM...}.(j
+00005a50: 4f04 0000 5d94 6a51 0400 005d 946a 5304  O...].jQ...].jS.
+00005a60: 0000 5d94 6a55 0400 005d 946a 5704 0000  ..].jU...].jW...
+00005a70: 5d94 756a 5904 0000 6a83 0400 006a 4c04  ].ujY...j....jL.
+00005a80: 0000 6ae6 0500 0075 6261 6a4d 0400 007d  ..j....ubajM...}
+00005a90: 9428 6a4f 0400 005d 946a 5104 0000 5d94  .(jO...].jQ...].
+00005aa0: 6a53 0400 005d 946a 5504 0000 5d94 6a57  jS...].jU...].jW
+00005ab0: 0400 005d 9475 6a59 0400 006a 7d04 0000  ...].ujY...j}...
+00005ac0: 6a4c 0400 006a 5705 0000 7562 656a 4d04  jL...jW...ubejM.
+00005ad0: 0000 7d94 286a 4f04 0000 5d94 6a51 0400  ..}.(jO...].jQ..
+00005ae0: 005d 946a 5304 0000 5d94 6a55 0400 005d  .].jS...].jU...]
+00005af0: 946a 5704 0000 5d94 756a 5904 0000 6a78  .jW...].ujY...jx
+00005b00: 0400 006a 4c04 0000 6a3b 0500 0075 6265  ...jL...j;...ube
+00005b10: 6a4d 0400 007d 9428 6a4f 0400 005d 946a  jM...}.(jO...].j
+00005b20: 5104 0000 5d94 6a53 0400 005d 946a 5504  Q...].jS...].jU.
+00005b30: 0000 5d94 6a57 0400 005d 9475 6a59 0400  ..].jW...].ujY..
+00005b40: 006a 7d04 0000 6a4c 0400 006a 3805 0000  .j}...jL...j8...
+00005b50: 7562 616a 4d04 0000 7d94 286a 4f04 0000  ubajM...}.(jO...
+00005b60: 5d94 6a51 0400 005d 946a 5304 0000 5d94  ].jQ...].jS...].
+00005b70: 6a55 0400 005d 946a 5704 0000 5d94 756a  jU...].jW...].uj
+00005b80: 5904 0000 6a78 0400 0075 626a f503 0000  Y...jx...ubj....
+00005b90: 6a79 0400 0029 8194 7d94 286a 4304 0000  jy...)..}.(jC...
+00005ba0: 681f 6a44 0400 005d 9428 6a7e 0400 0029  h.jD...].(j~...)
+00005bb0: 8194 7d94 286a 4304 0000 681f 6a44 0400  ..}.(jC...h.jD..
+00005bc0: 005d 9428 6a84 0400 0029 8194 7d94 286a  .].(j....)..}.(j
+00005bd0: 4304 0000 681f 6a44 0400 005d 946a 8904  C...h.jD...].j..
+00005be0: 0000 2981 947d 9428 6a43 0400 0068 1f6a  ..)..}.(jC...h.j
+00005bf0: 4404 0000 5d94 6a47 0400 008c 1876 6f6c  D...].jG.....vol
+00005c00: 6c73 6567 2d6e 6170 6172 692d 7472 6163  lseg-napari-trac
+00005c10: 6b6d 6174 6594 8594 8194 7d94 286a 4304  kmate.....}.(jC.
+00005c20: 0000 681f 6a4c 0400 006a 2406 0000 7562  ..h.jL...j$...ub
+00005c30: 616a 4d04 0000 7d94 286a 4f04 0000 5d94  ajM...}.(jO...].
+00005c40: 6a51 0400 005d 946a 5304 0000 5d94 6a55  jQ...].jS...].jU
+00005c50: 0400 005d 946a 5704 0000 5d94 8c08 696e  ...].jW...]...in
+00005c60: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
+00005c70: 946a f503 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
+00005c80: 6d65 9468 1f75 6a59 0400 006a 8804 0000  me.h.ujY...j....
+00005c90: 6a4c 0400 006a 2106 0000 7562 616a 4d04  jL...j!...ubajM.
+00005ca0: 0000 7d94 286a 4f04 0000 5d94 6a51 0400  ..}.(jO...].jQ..
+00005cb0: 005d 946a 5304 0000 5d94 6a55 0400 005d  .].jS...].jU...]
+00005cc0: 946a 5704 0000 5d94 756a 5904 0000 6a83  .jW...].ujY...j.
+00005cd0: 0400 006a 4c04 0000 6a1e 0600 0075 626a  ...jL...j....ubj
+00005ce0: 7904 0000 2981 947d 9428 6a43 0400 0068  y...)..}.(jC...h
+00005cf0: 1f6a 4404 0000 5d94 286a 7e04 0000 2981  .jD...].(j~...).
+00005d00: 947d 9428 6a43 0400 0068 1f6a 4404 0000  .}.(jC...h.jD...
+00005d10: 5d94 6a84 0400 0029 8194 7d94 286a 4304  ].j....)..}.(jC.
+00005d20: 0000 681f 6a44 0400 005d 946a 8904 0000  ..h.jD...].j....
+00005d30: 2981 947d 9428 6a43 0400 0068 1f6a 4404  )..}.(jC...h.jD.
+00005d40: 0000 5d94 6a47 0400 008c 0c49 6e73 7461  ..].jG.....Insta
+00005d50: 6c6c 6174 696f 6e94 8594 8194 7d94 286a  llation.....}.(j
+00005d60: 4304 0000 681f 6a4c 0400 006a 4306 0000  C...h.jL...jC...
+00005d70: 7562 616a 4d04 0000 7d94 286a 4f04 0000  ubajM...}.(jO...
+00005d80: 5d94 6a51 0400 005d 946a 5304 0000 5d94  ].jQ...].jS...].
+00005d90: 6a55 0400 005d 946a 5704 0000 5d94 8c08  jU...].jW...]...
+00005da0: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
+00005db0: 7269 946a f503 0000 8c0a 616e 6368 6f72  ri.j......anchor
+00005dc0: 6e61 6d65 948c 0d23 696e 7374 616c 6c61  name...#installa
+00005dd0: 7469 6f6e 9475 6a59 0400 006a 8804 0000  tion.ujY...j....
+00005de0: 6a4c 0400 006a 4006 0000 7562 616a 4d04  jL...j@...ubajM.
+00005df0: 0000 7d94 286a 4f04 0000 5d94 6a51 0400  ..}.(jO...].jQ..
+00005e00: 005d 946a 5304 0000 5d94 6a55 0400 005d  .].jS...].jU...]
+00005e10: 946a 5704 0000 5d94 756a 5904 0000 6a83  .jW...].ujY...j.
+00005e20: 0400 006a 4c04 0000 6a3d 0600 0075 6261  ...jL...j=...uba
+00005e30: 6a4d 0400 007d 9428 6a4f 0400 005d 946a  jM...}.(jO...].j
+00005e40: 5104 0000 5d94 6a53 0400 005d 946a 5504  Q...].jS...].jU.
+00005e50: 0000 5d94 6a57 0400 005d 9475 6a59 0400  ..].jW...].ujY..
+00005e60: 006a 7d04 0000 6a4c 0400 006a 3a06 0000  .j}...jL...j:...
+00005e70: 7562 6a7e 0400 0029 8194 7d94 286a 4304  ubj~...)..}.(jC.
+00005e80: 0000 681f 6a44 0400 005d 946a 8404 0000  ..h.jD...].j....
+00005e90: 2981 947d 9428 6a43 0400 0068 1f6a 4404  )..}.(jC...h.jD.
+00005ea0: 0000 5d94 6a89 0400 0029 8194 7d94 286a  ..].j....)..}.(j
+00005eb0: 4304 0000 681f 6a44 0400 005d 946a 4704  C...h.jD...].jG.
+00005ec0: 0000 8c0c 436f 6e74 7269 6275 7469 6e67  ....Contributing
+00005ed0: 9485 9481 947d 9428 6a43 0400 0068 1f6a  .....}.(jC...h.j
+00005ee0: 4c04 0000 6a66 0600 0075 6261 6a4d 0400  L...jf...ubajM..
+00005ef0: 007d 9428 6a4f 0400 005d 946a 5104 0000  .}.(jO...].jQ...
+00005f00: 5d94 6a53 0400 005d 946a 5504 0000 5d94  ].jS...].jU...].
+00005f10: 6a57 0400 005d 948c 0869 6e74 6572 6e61  jW...]...interna
+00005f20: 6c94 888c 0672 6566 7572 6994 6af5 0300  l....refuri.j...
+00005f30: 008c 0a61 6e63 686f 726e 616d 6594 8c0d  ...anchorname...
+00005f40: 2363 6f6e 7472 6962 7574 696e 6794 756a  #contributing.uj
+00005f50: 5904 0000 6a88 0400 006a 4c04 0000 6a63  Y...j....jL...jc
+00005f60: 0600 0075 6261 6a4d 0400 007d 9428 6a4f  ...ubajM...}.(jO
+00005f70: 0400 005d 946a 5104 0000 5d94 6a53 0400  ...].jQ...].jS..
+00005f80: 005d 946a 5504 0000 5d94 6a57 0400 005d  .].jU...].jW...]
+00005f90: 9475 6a59 0400 006a 8304 0000 6a4c 0400  .ujY...j....jL..
+00005fa0: 006a 6006 0000 7562 616a 4d04 0000 7d94  .j`...ubajM...}.
+00005fb0: 286a 4f04 0000 5d94 6a51 0400 005d 946a  (jO...].jQ...].j
+00005fc0: 5304 0000 5d94 6a55 0400 005d 946a 5704  S...].jU...].jW.
+00005fd0: 0000 5d94 756a 5904 0000 6a7d 0400 006a  ..].ujY...j}...j
+00005fe0: 4c04 0000 6a3a 0600 0075 626a 7e04 0000  L...j:...ubj~...
+00005ff0: 2981 947d 9428 6a43 0400 0068 1f6a 4404  )..}.(jC...h.jD.
+00006000: 0000 5d94 6a84 0400 0029 8194 7d94 286a  ..].j....)..}.(j
+00006010: 4304 0000 681f 6a44 0400 005d 946a 8904  C...h.jD...].j..
+00006020: 0000 2981 947d 9428 6a43 0400 0068 1f6a  ..)..}.(jC...h.j
+00006030: 4404 0000 5d94 6a47 0400 008c 074c 6963  D...].jG.....Lic
+00006040: 656e 7365 9485 9481 947d 9428 6a43 0400  ense.....}.(jC..
+00006050: 0068 1f6a 4c04 0000 6a89 0600 0075 6261  .h.jL...j....uba
+00006060: 6a4d 0400 007d 9428 6a4f 0400 005d 946a  jM...}.(jO...].j
+00006070: 5104 0000 5d94 6a53 0400 005d 946a 5504  Q...].jS...].jU.
+00006080: 0000 5d94 6a57 0400 005d 948c 0869 6e74  ..].jW...]...int
+00006090: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
+000060a0: 6af5 0300 008c 0a61 6e63 686f 726e 616d  j......anchornam
+000060b0: 6594 8c08 236c 6963 656e 7365 9475 6a59  e...#license.ujY
+000060c0: 0400 006a 8804 0000 6a4c 0400 006a 8606  ...j....jL...j..
+000060d0: 0000 7562 616a 4d04 0000 7d94 286a 4f04  ..ubajM...}.(jO.
+000060e0: 0000 5d94 6a51 0400 005d 946a 5304 0000  ..].jQ...].jS...
+000060f0: 5d94 6a55 0400 005d 946a 5704 0000 5d94  ].jU...].jW...].
+00006100: 756a 5904 0000 6a83 0400 006a 4c04 0000  ujY...j....jL...
+00006110: 6a83 0600 0075 6261 6a4d 0400 007d 9428  j....ubajM...}.(
+00006120: 6a4f 0400 005d 946a 5104 0000 5d94 6a53  jO...].jQ...].jS
+00006130: 0400 005d 946a 5504 0000 5d94 6a57 0400  ...].jU...].jW..
+00006140: 005d 9475 6a59 0400 006a 7d04 0000 6a4c  .].ujY...j}...jL
+00006150: 0400 006a 3a06 0000 7562 6a7e 0400 0029  ...j:...ubj~...)
+00006160: 8194 7d94 286a 4304 0000 681f 6a44 0400  ..}.(jC...h.jD..
+00006170: 005d 946a 8404 0000 2981 947d 9428 6a43  .].j....)..}.(jC
+00006180: 0400 0068 1f6a 4404 0000 5d94 6a89 0400  ...h.jD...].j...
+00006190: 0029 8194 7d94 286a 4304 0000 681f 6a44  .)..}.(jC...h.jD
+000061a0: 0400 005d 946a 4704 0000 8c06 4973 7375  ...].jG.....Issu
+000061b0: 6573 9485 9481 947d 9428 6a43 0400 0068  es.....}.(jC...h
+000061c0: 1f6a 4c04 0000 6aac 0600 0075 6261 6a4d  .jL...j....ubajM
+000061d0: 0400 007d 9428 6a4f 0400 005d 946a 5104  ...}.(jO...].jQ.
+000061e0: 0000 5d94 6a53 0400 005d 946a 5504 0000  ..].jS...].jU...
+000061f0: 5d94 6a57 0400 005d 948c 0869 6e74 6572  ].jW...]...inter
+00006200: 6e61 6c94 888c 0672 6566 7572 6994 6af5  nal....refuri.j.
+00006210: 0300 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
+00006220: 8c07 2369 7373 7565 7394 756a 5904 0000  ..#issues.ujY...
+00006230: 6a88 0400 006a 4c04 0000 6aa9 0600 0075  j....jL...j....u
+00006240: 6261 6a4d 0400 007d 9428 6a4f 0400 005d  bajM...}.(jO...]
+00006250: 946a 5104 0000 5d94 6a53 0400 005d 946a  .jQ...].jS...].j
+00006260: 5504 0000 5d94 6a57 0400 005d 9475 6a59  U...].jW...].ujY
+00006270: 0400 006a 8304 0000 6a4c 0400 006a a606  ...j....jL...j..
+00006280: 0000 7562 616a 4d04 0000 7d94 286a 4f04  ..ubajM...}.(jO.
+00006290: 0000 5d94 6a51 0400 005d 946a 5304 0000  ..].jQ...].jS...
+000062a0: 5d94 6a55 0400 005d 946a 5704 0000 5d94  ].jU...].jW...].
+000062b0: 756a 5904 0000 6a7d 0400 006a 4c04 0000  ujY...j}...jL...
+000062c0: 6a3a 0600 0075 6265 6a4d 0400 007d 9428  j:...ubejM...}.(
+000062d0: 6a4f 0400 005d 946a 5104 0000 5d94 6a53  jO...].jQ...].jS
+000062e0: 0400 005d 946a 5504 0000 5d94 6a57 0400  ...].jU...].jW..
+000062f0: 005d 9475 6a59 0400 006a 7804 0000 6a4c  .].ujY...jx...jL
+00006300: 0400 006a 1e06 0000 7562 656a 4d04 0000  ...j....ubejM...
+00006310: 7d94 286a 4f04 0000 5d94 6a51 0400 005d  }.(jO...].jQ...]
+00006320: 946a 5304 0000 5d94 6a55 0400 005d 946a  .jS...].jU...].j
+00006330: 5704 0000 5d94 756a 5904 0000 6a7d 0400  W...].ujY...j}..
+00006340: 006a 4c04 0000 6a1b 0600 0075 626a 8204  .jL...j....ubj..
+00006350: 0000 8c07 746f 6374 7265 6594 9394 2981  ....toctree...).
+00006360: 947d 9428 6a43 0400 0068 1f6a 4404 0000  .}.(jC...h.jD...
+00006370: 5d94 6a4d 0400 007d 9428 6a4f 0400 005d  ].jM...}.(jO...]
+00006380: 946a 5104 0000 5d94 6a53 0400 005d 946a  .jQ...].jS...].j
+00006390: 5504 0000 5d94 6a57 0400 005d 948c 0670  U...].jW...]...p
+000063a0: 6172 656e 7494 6af5 0300 008c 0765 6e74  arent.j......ent
+000063b0: 7269 6573 945d 944e 8c09 414c 474f 5249  ries.].N..ALGORI
+000063c0: 5448 4d94 8694 618c 0c69 6e63 6c75 6465  THM...a..include
+000063d0: 6669 6c65 7394 5d94 6ae3 0600 0061 8c08  files.].j....a..
+000063e0: 6d61 7864 6570 7468 944a ffff ffff 8c07  maxdepth.J......
+000063f0: 6361 7074 696f 6e94 4e8c 0a72 6177 6361  caption.N..rawca
+00006400: 7074 696f 6e94 681f 8c04 676c 6f62 9489  ption.h...glob..
+00006410: 8c06 6869 6464 656e 9488 8c0d 696e 636c  ..hidden....incl
+00006420: 7564 6568 6964 6465 6e94 898c 086e 756d  udehidden....num
+00006430: 6265 7265 6494 4b00 8c0a 7469 746c 6573  bered.K...titles
+00006440: 6f6e 6c79 9488 756a 5904 0000 6ad5 0600  only..ujY...j...
+00006450: 008c 0673 6f75 7263 6594 8c50 2f6d 6e74  ...source..P/mnt
+00006460: 2f63 2f55 7365 7273 2f72 616e 646f 2f44  /c/Users/rando/D
+00006470: 6f77 6e6c 6f61 6473 2f50 7974 686f 6e5f  ownloads/Python_
+00006480: 576f 726b 7370 6163 652f 766f 6c6c 7365  Workspace/vollse
+00006490: 672d 6e61 7061 7269 2d74 7261 636b 6d61  g-napari-trackma
+000064a0: 7465 2f52 4541 444d 452e 6d64 948c 046c  te/README.md...l
+000064b0: 696e 6594 4b01 6a4c 0400 006a 1b06 0000  ine.K.jL...j....
+000064c0: 7562 656a 4d04 0000 7d94 286a 4f04 0000  ubejM...}.(jO...
+000064d0: 5d94 6a51 0400 005d 946a 5304 0000 5d94  ].jQ...].jS...].
+000064e0: 6a55 0400 005d 946a 5704 0000 5d94 756a  jU...].jW...].uj
+000064f0: 5904 0000 6a78 0400 0075 6275 8c0f 746f  Y...jx...ubu..to
+00006500: 635f 6e75 6d5f 656e 7472 6965 7394 7d94  c_num_entries.}.
+00006510: 286a f403 0000 4b05 6af3 0300 004b 066a  (j....K.j....K.j
+00006520: f503 0000 4b05 758c 0e74 6f63 5f73 6563  ....K.u..toc_sec
+00006530: 6e75 6d62 6572 7394 7d94 8c0e 746f 635f  numbers.}...toc_
+00006540: 6669 676e 756d 6265 7273 947d 948c 1074  fignumbers.}...t
+00006550: 6f63 7472 6565 5f69 6e63 6c75 6465 7394  octree_includes.
+00006560: 7d94 6af5 0300 005d 946a e306 0000 6173  }.j....].j....as
+00006570: 8c10 6669 6c65 735f 746f 5f72 6562 7569  ..files_to_rebui
+00006580: 6c64 947d 946a e306 0000 8f94 286a f503  ld.}.j......(j..
+00006590: 0000 9073 8c0d 676c 6f62 5f74 6f63 7472  ...s..glob_toctr
+000065a0: 6565 7394 8f94 8c11 6e75 6d62 6572 6564  ees.....numbered
+000065b0: 5f74 6f63 7472 6565 7394 8f94 8c0a 646f  _toctrees.....do
+000065c0: 6d61 696e 6461 7461 947d 9428 8c01 6394  maindata.}.(..c.
+000065d0: 7d94 288c 0b72 6f6f 745f 7379 6d62 6f6c  }.(..root_symbol
+000065e0: 946a f703 0000 8c06 5379 6d62 6f6c 9493  .j......Symbol..
+000065f0: 9429 8194 7d94 286a 4c04 0000 4e8c 0c73  .)..}.(jL...N..s
+00006600: 6962 6c69 6e67 4162 6f76 6594 4e8c 0c73  iblingAbove.N..s
+00006610: 6962 6c69 6e67 4265 6c6f 7794 4e8c 0569  iblingBelow.N..i
+00006620: 6465 6e74 944e 8c0b 6465 636c 6172 6174  dent.N..declarat
+00006630: 696f 6e94 4e68 a54e 6af1 0600 004e 8c0f  ion.Nh.Nj....N..
+00006640: 6973 5265 6465 636c 6172 6174 696f 6e94  isRedeclaration.
+00006650: 898c 095f 6368 696c 6472 656e 945d 948c  ..._children.]..
+00006660: 0d5f 616e 6f6e 4368 696c 6472 656e 945d  ._anonChildren.]
+00006670: 9475 628c 076f 626a 6563 7473 947d 9468  .ub..objects.}.h
+00006680: df4b 0075 8c09 6368 616e 6765 7365 7494  .K.u..changeset.
+00006690: 7d94 288c 0763 6861 6e67 6573 947d 9468  }.(..changes.}.h
+000066a0: df4b 0075 8c08 6369 7461 7469 6f6e 947d  .K.u..citation.}
+000066b0: 9428 68df 4b00 8c09 6369 7461 7469 6f6e  .(h.K...citation
+000066c0: 7394 7d94 8c0d 6369 7461 7469 6f6e 5f72  s.}...citation_r
+000066d0: 6566 7394 7d94 758c 0363 7070 947d 9428  efs.}.u..cpp.}.(
+000066e0: 6a0c 0700 006a fa03 0000 6a0d 0700 0093  j....j....j.....
+000066f0: 9429 8194 7d94 286a 4c04 0000 4e6a 1107  .)..}.(jL...Nj..
+00006700: 0000 4e6a 1207 0000 4e8c 0969 6465 6e74  ..Nj....N..ident
+00006710: 4f72 4f70 944e 8c0e 7465 6d70 6c61 7465  OrOp.N..template
+00006720: 5061 7261 6d73 944e 8c0c 7465 6d70 6c61  Params.N..templa
+00006730: 7465 4172 6773 944e 6a14 0700 004e 68a5  teArgs.Nj....Nh.
+00006740: 4e6a f106 0000 4e6a 1507 0000 896a 1607  Nj....Nj.....j..
+00006750: 0000 5d94 6a18 0700 005d 9475 626a 5304  ..].j....].ubjS.
+00006760: 0000 7d94 68df 4b00 758c 0569 6e64 6578  ..}.h.K.u..index
+00006770: 947d 9428 68df 4b00 8c07 656e 7472 6965  .}.(h.K...entrie
+00006780: 7394 7d94 286a f403 0000 5d94 6af3 0300  s.}.(j....].j...
+00006790: 005d 946a f503 0000 5d94 7575 8c02 6a73  .].j....].uu..js
+000067a0: 947d 9428 6a1a 0700 007d 948c 076d 6f64  .}.(j....}...mod
+000067b0: 756c 6573 947d 9468 df4b 0075 8c04 6d61  ules.}.h.K.u..ma
+000067c0: 7468 947d 9428 6a1a 0700 007d 948c 0d68  th.}.(j....}...h
+000067d0: 6173 5f65 7175 6174 696f 6e73 947d 9428  as_equations.}.(
+000067e0: 6af4 0300 0089 6af3 0300 0089 6af5 0300  j.....j.....j...
+000067f0: 0089 7568 df4b 0075 6a21 0100 007d 9428  ..uh.K.uj!...}.(
+00006800: 6a1a 0700 007d 946a 3b07 0000 7d94 68df  j....}.j;...}.h.
+00006810: 4b00 758c 0372 7374 947d 9428 6a1a 0700  K.u..rst.}.(j...
+00006820: 007d 9468 df4b 0075 8c03 7374 6494 7d94  .}.h.K.u..std.}.
+00006830: 288c 0b70 726f 676f 7074 696f 6e73 947d  (..progoptions.}
+00006840: 946a 1a07 0000 7d94 8c06 6c61 6265 6c73  .j....}...labels
+00006850: 947d 9428 8c08 6765 6e69 6e64 6578 946a  .}.(..genindex.j
+00006860: 4f07 0000 681f 8c0d 7370 6869 6e78 2e6c  O...h...sphinx.l
+00006870: 6f63 616c 6594 8c11 5f54 7261 6e73 6c61  ocale..._Transla
+00006880: 7469 6f6e 5072 6f78 7994 9394 286a 5007  tionProxy...(jP.
+00006890: 0000 8c0f 5f6c 617a 795f 7472 616e 736c  ...._lazy_transl
+000068a0: 6174 6594 9394 6813 8c07 6765 6e65 7261  ate...h...genera
+000068b0: 6c94 8c05 496e 6465 7894 7494 8194 6a54  l...Index.t...jT
+000068c0: 0700 0068 136a 5507 0000 6a56 0700 0087  ...h.jU...jV....
+000068d0: 9486 9462 8794 8c08 6d6f 6469 6e64 6578  ...b....modindex
+000068e0: 948c 0b70 792d 6d6f 6469 6e64 6578 9468  ...py-modindex.h
+000068f0: 1f6a 5207 0000 286a 5407 0000 6813 6a55  .jR...(jT...h.jU
+00006900: 0700 008c 0c4d 6f64 756c 6520 496e 6465  .....Module Inde
+00006910: 7894 7494 8194 6a54 0700 0068 136a 5507  x.t...jT...h.jU.
+00006920: 0000 6a5e 0700 0087 9486 9462 8794 8c06  ..j^.......b....
+00006930: 7365 6172 6368 946a 6407 0000 681f 6a52  search.jd...h.jR
+00006940: 0700 0028 6a54 0700 0068 136a 5507 0000  ...(jT...h.jU...
+00006950: 8c0b 5365 6172 6368 2050 6167 6594 7494  ..Search Page.t.
+00006960: 8194 6a54 0700 0068 136a 5507 0000 6a65  ..jT...h.jU...je
+00006970: 0700 0087 9486 9462 8794 8c0b 7079 2d6d  .......b....py-m
+00006980: 6f64 696e 6465 7894 6a6b 0700 0068 1f8c  odindex.jk...h..
+00006990: 1350 7974 686f 6e20 4d6f 6475 6c65 2049  .Python Module I
+000069a0: 6e64 6578 9487 9475 8c0a 616e 6f6e 6c61  ndex...u..anonla
+000069b0: 6265 6c73 947d 9428 6a4f 0700 006a 4f07  bels.}.(jO...jO.
+000069c0: 0000 681f 8694 6a5c 0700 006a 5d07 0000  ..h...j\...j]...
+000069d0: 681f 8694 6a64 0700 006a 6407 0000 681f  h...jd...jd...h.
+000069e0: 8694 6a6b 0700 006a 6b07 0000 681f 8694  ..jk...jk...h...
+000069f0: 7568 df4b 008c 0574 6572 6d73 947d 9475  uh.K...terms.}.u
+00006a00: 8c04 6576 616c 947d 9468 df4b 0173 8c04  ..eval.}.h.K.s..
+00006a10: 676c 7565 947d 9468 df4b 0173 8c04 6369  glue.}.h.K.s..ci
+00006a20: 7465 947d 9428 8c07 6269 6264 6174 6194  te.}.(..bibdata.
+00006a30: 8c1c 7370 6869 6e78 636f 6e74 7269 622e  ..sphinxcontrib.
+00006a40: 6269 6274 6578 2e62 6962 6669 6c65 948c  bibtex.bibfile..
+00006a50: 0742 6962 4461 7461 9493 946a d003 0000  .BibData...j....
+00006a60: 7d94 8c55 2f6d 6e74 2f63 2f55 7365 7273  }..U/mnt/c/Users
+00006a70: 2f72 616e 646f 2f44 6f77 6e6c 6f61 6473  /rando/Downloads
+00006a80: 2f50 7974 686f 6e5f 576f 726b 7370 6163  /Python_Workspac
+00006a90: 652f 766f 6c6c 7365 672d 6e61 7061 7269  e/vollseg-napari
+00006aa0: 2d74 7261 636b 6d61 7465 2f72 6566 6572  -trackmate/refer
+00006ab0: 656e 6365 732e 6269 6294 6a7d 0700 008c  ences.bib.j}....
+00006ac0: 0742 6962 4669 6c65 9493 9447 fff0 0000  .BibFile...G....
+00006ad0: 0000 0000 7d94 8694 8194 738c 0f70 7962  ....}.....s..pyb
+00006ae0: 7465 782e 6461 7461 6261 7365 948c 1042  tex.database...B
+00006af0: 6962 6c69 6f67 7261 7068 7944 6174 6194  ibliographyData.
+00006b00: 9394 2981 947d 9428 6a33 0700 008c 0c70  ..)..}.(j3.....p
+00006b10: 7962 7465 782e 7574 696c 7394 8c1a 4f72  ybtex.utils...Or
+00006b20: 6465 7265 6443 6173 6549 6e73 656e 7369  deredCaseInsensi
+00006b30: 7469 7665 4469 6374 9493 9429 8194 7d94  tiveDict...)..}.
+00006b40: 288c 055f 6469 6374 947d 948c 055f 6b65  (.._dict.}..._ke
+00006b50: 7973 9468 8729 5294 7562 8c0e 6372 6f73  ys.h.)R.ub..cros
+00006b60: 7372 6566 5f63 6f75 6e74 946a 8c07 0000  sref_count.j....
+00006b70: 8c1a 4361 7365 496e 7365 6e73 6974 6976  ..CaseInsensitiv
+00006b80: 6544 6566 6175 6c74 4469 6374 9493 9429  eDefaultDict...)
+00006b90: 8194 7d94 286a 9107 0000 7d94 6a93 0700  ..}.(j....}.j...
+00006ba0: 007d 948c 0f64 6566 6175 6c74 5f66 6163  .}...default_fac
+00006bb0: 746f 7279 946a 2104 0000 8c03 696e 7494  tory.j!.....int.
+00006bc0: 9394 7562 8c0d 6d69 6e5f 6372 6f73 7372  ..ub..min_crossr
+00006bd0: 6566 7394 4b02 8c09 5f70 7265 616d 626c  efs.K..._preambl
+00006be0: 6594 5d94 8c0e 7761 6e74 6564 5f65 6e74  e.]...wanted_ent
+00006bf0: 7269 6573 944e 6a22 0700 006a 8c07 0000  ries.Nj"...j....
+00006c00: 8c12 4361 7365 496e 7365 6e73 6974 6976  ..CaseInsensitiv
+00006c10: 6553 6574 9493 9429 8194 7d94 288c 045f  eSet...)..}.(.._
+00006c20: 7365 7494 8f94 6a93 0700 007d 9475 6275  set...j....}.ubu
+00006c30: 6287 9481 948c 1362 6962 6c69 6f67 7261  b......bibliogra
+00006c40: 7068 795f 6865 6164 6572 946a 3f04 0000  phy_header.j?...
+00006c50: 8c09 636f 6e74 6169 6e65 7294 9394 2981  ..container...).
+00006c60: 947d 9428 6a43 0400 0068 1f6a 4404 0000  .}.(jC...h.jD...
+00006c70: 5d94 6a4d 0400 007d 9428 6a4f 0400 005d  ].jM...}.(jO...]
+00006c80: 946a 5104 0000 5d94 6a53 0400 005d 946a  .jQ...].jS...].j
+00006c90: 5504 0000 5d94 6a57 0400 005d 9475 6a59  U...].jW...].ujY
+00006ca0: 0400 006a ad07 0000 7562 8c0e 6269 626c  ...j....ub..bibl
+00006cb0: 696f 6772 6170 6869 6573 947d 946a 2207  iographies.}.j".
+00006cc0: 0000 5d94 6a24 0700 005d 9468 df4b 0475  ..].j$...].h.K.u
+00006cd0: 8c08 666f 6f74 6369 7465 947d 9428 6aac  ..footcite.}.(j.
+00006ce0: 0700 006a ae07 0000 2981 947d 9428 6a43  ...j....)..}.(jC
+00006cf0: 0400 0068 1f6a 4404 0000 5d94 6a4d 0400  ...h.jD...].jM..
+00006d00: 007d 9428 6a4f 0400 005d 946a 5104 0000  .}.(jO...].jQ...
+00006d10: 5d94 6a53 0400 005d 946a 5504 0000 5d94  ].jS...].jU...].
+00006d20: 6a57 0400 005d 9475 6a59 0400 006a ad07  jW...].ujY...j..
+00006d30: 0000 7562 68df 4b00 7575 8c06 696d 6167  ..ubh.K.uu..imag
+00006d40: 6573 948c 0b73 7068 696e 782e 7574 696c  es...sphinx.util
+00006d50: 948c 1046 696c 656e 616d 6555 6e69 7144  ...FilenameUniqD
+00006d60: 6963 7494 9394 2981 946a 2904 0000 8f94  ict...)..j).....
+00006d70: 286a f303 0000 908c 1970 6f69 6e74 5f63  (j.......point_c
+00006d80: 6c6f 7564 735f 636f 6d70 6172 6564 2e70  louds_compared.p
+00006d90: 6e67 9486 9473 8f94 286a cd07 0000 9062  ng...s..(j.....b
+00006da0: 8c07 646c 6669 6c65 7394 6ac8 0700 008c  ..dlfiles.j.....
+00006db0: 0d44 6f77 6e6c 6f61 6446 696c 6573 9493  .DownloadFiles..
+00006dc0: 9429 8194 286a 2704 0000 8f94 286a f303  .)..(j'.....(j..
+00006dd0: 0000 908c 3a63 3734 6461 3133 3630 3966  ....:c74da13609f
+00006de0: 3831 6463 6239 3464 3734 6638 3833 3237  81dcb94d74f88327
+00006df0: 6336 6230 372f 7669 7375 616c 697a 655f  c6b07/visualize_
+00006e00: 706f 696e 745f 636c 6f75 6473 2e70 7994  point_clouds.py.
+00006e10: 8694 6a28 0400 008f 9428 6af3 0300 0090  ..j(.....(j.....
+00006e20: 8c35 3733 3034 3332 3235 3232 6562 3333  .57304322522eb33
+00006e30: 6234 6331 6436 6663 6439 6238 6461 6330  b4c1d6fcd9b8dac0
+00006e40: 6166 2f61 7070 6c79 5f61 7574 6f65 6e63  af/apply_autoenc
+00006e50: 6f64 6572 2e70 7994 8694 758c 126f 7269  oder.py...u..ori
+00006e60: 6769 6e61 6c5f 696d 6167 655f 7572 6994  ginal_image_uri.
+00006e70: 7d94 8c09 7465 6d70 5f64 6174 6194 7d94  }...temp_data.}.
+00006e80: 8c0b 7265 665f 636f 6e74 6578 7494 7d94  ..ref_context.}.
+00006e90: 8c0b 6d79 7374 5f63 6f6e 6669 6794 8c17  ..myst_config...
+00006ea0: 6d79 7374 5f70 6172 7365 722e 636f 6e66  myst_parser.conf
+00006eb0: 6967 2e6d 6169 6e94 8c0e 4d64 5061 7273  ig.main...MdPars
+00006ec0: 6572 436f 6e66 6967 9493 9429 8194 7d94  erConfig...)..}.
+00006ed0: 288c 0f63 6f6d 6d6f 6e6d 6172 6b5f 6f6e  (..commonmark_on
+00006ee0: 6c79 9489 8c08 6766 6d5f 6f6e 6c79 9489  ly....gfm_only..
+00006ef0: 8c11 656e 6162 6c65 5f65 7874 656e 7369  ..enable_extensi
+00006f00: 6f6e 7394 684e 8c0e 6469 7361 626c 655f  ons.hN..disable_
+00006f10: 7379 6e74 6178 946a 2003 0000 8c12 616c  syntax.j .....al
+00006f20: 6c5f 6c69 6e6b 735f 6578 7465 726e 616c  l_links_external
+00006f30: 9489 8c0b 7572 6c5f 7363 6865 6d65 7394  ....url_schemes.
+00006f40: 6855 8c0b 7265 665f 646f 6d61 696e 7394  hU..ref_domains.
+00006f50: 4e8c 1568 6967 686c 6967 6874 5f63 6f64  N..highlight_cod
+00006f60: 655f 626c 6f63 6b73 9488 8c12 6e75 6d62  e_blocks....numb
+00006f70: 6572 5f63 6f64 655f 626c 6f63 6b73 946a  er_code_blocks.j
+00006f80: 2903 0000 8c0f 7469 746c 655f 746f 5f68  ).....title_to_h
+00006f90: 6561 6465 7294 898c 0f68 6561 6469 6e67  eader....heading
+00006fa0: 5f61 6e63 686f 7273 944e 8c11 6865 6164  _anchors.N..head
+00006fb0: 696e 675f 736c 7567 5f66 756e 6394 4e8c  ing_slug_func.N.
+00006fc0: 0968 746d 6c5f 6d65 7461 946a 3203 0000  .html_meta.j2...
+00006fd0: 8c13 666f 6f74 6e6f 7465 5f74 7261 6e73  ..footnote_trans
+00006fe0: 6974 696f 6e94 888c 1077 6f72 6473 5f70  ition....words_p
+00006ff0: 6572 5f6d 696e 7574 6594 4bc8 8c0d 7375  er_minute.K...su
+00007000: 6273 7469 7475 7469 6f6e 7394 6a39 0300  bstitutions.j9..
+00007010: 008c 0e73 7562 5f64 656c 696d 6974 6572  ...sub_delimiter
+00007020: 7394 6a3e 0300 008c 136c 696e 6b69 6679  s.j>.....linkify
+00007030: 5f66 757a 7a79 5f6c 696e 6b73 9488 8c12  _fuzzy_links....
+00007040: 646d 6174 685f 616c 6c6f 775f 6c61 6265  dmath_allow_labe
+00007050: 6c73 9488 8c11 646d 6174 685f 616c 6c6f  ls....dmath_allo
+00007060: 775f 7370 6163 6594 888c 1264 6d61 7468  w_space....dmath
+00007070: 5f61 6c6c 6f77 5f64 6967 6974 7394 888c  _allow_digits...
+00007080: 1364 6d61 7468 5f64 6f75 626c 655f 696e  .dmath_double_in
+00007090: 6c69 6e65 9489 8c0e 7570 6461 7465 5f6d  line....update_m
+000070a0: 6174 686a 6178 9488 8c0f 6d61 7468 6a61  athjax....mathja
+000070b0: 785f 636c 6173 7365 7394 68cc 7562 8c0d  x_classes.h.ub..
+000070c0: 6d79 7374 6e62 5f63 6f6e 6669 6794 8c13  mystnb_config...
+000070d0: 6d79 7374 5f6e 622e 636f 7265 2e63 6f6e  myst_nb.core.con
+000070e0: 6669 6794 8c0e 4e62 5061 7273 6572 436f  fig...NbParserCo
+000070f0: 6e66 6967 9493 9429 8194 7d94 288c 0e63  nfig...)..}.(..c
+00007100: 7573 746f 6d5f 666f 726d 6174 7394 7d94  ustom_formats.}.
+00007110: 8c0a 7265 6164 5f61 735f 6d64 9489 8c0c  ..read_as_md....
+00007120: 6d65 7461 6461 7461 5f6b 6579 946a 5203  metadata_key.jR.
+00007130: 0000 8c11 6365 6c6c 5f6d 6574 6164 6174  ....cell_metadat
+00007140: 615f 6b65 7994 6a52 0300 008c 126b 6572  a_key.jR.....ker
+00007150: 6e65 6c5f 7267 785f 616c 6961 7365 7394  nel_rgx_aliases.
+00007160: 6a5a 0300 008c 0e65 7865 6375 7469 6f6e  jZ.....execution
+00007170: 5f6d 6f64 6594 6860 8c14 6578 6563 7574  _mode.h`..execut
+00007180: 696f 6e5f 6361 6368 655f 7061 7468 948c  ion_cache_path..
+00007190: 5c2f 6d6e 742f 632f 5573 6572 732f 7261  \/mnt/c/Users/ra
+000071a0: 6e64 6f2f 446f 776e 6c6f 6164 732f 5079  ndo/Downloads/Py
+000071b0: 7468 6f6e 5f57 6f72 6b73 7061 6365 2f76  thon_Workspace/v
+000071c0: 6f6c 6c73 6567 2d6e 6170 6172 692d 7472  ollseg-napari-tr
+000071d0: 6163 6b6d 6174 652f 5f62 7569 6c64 2f2e  ackmate/_build/.
+000071e0: 6a75 7079 7465 725f 6361 6368 6594 6a66  jupyter_cache.jf
+000071f0: 0300 0068 626a 6a03 0000 4b1e 6a6e 0300  ...hbjj...K.jn..
+00007200: 0089 6a72 0300 0089 8c18 6578 6563 7574  ..jr......execut
+00007210: 696f 6e5f 7261 6973 655f 6f6e 5f65 7272  ion_raise_on_err
+00007220: 6f72 9489 6a78 0300 0089 8c0d 6d65 7267  or..jx......merg
+00007230: 655f 7374 7265 616d 7394 898c 0d72 656e  e_streams....ren
+00007240: 6465 725f 706c 7567 696e 946a 0701 0000  der_plugin.j....
+00007250: 8c12 7265 6d6f 7665 5f63 6f64 655f 736f  ..remove_code_so
+00007260: 7572 6365 9489 8c13 7265 6d6f 7665 5f63  urce....remove_c
+00007270: 6f64 655f 6f75 7470 7574 7394 898c 1063  ode_outputs....c
+00007280: 6f64 655f 7072 6f6d 7074 5f73 686f 7794  ode_prompt_show.
+00007290: 6a83 0300 008c 1063 6f64 655f 7072 6f6d  j......code_prom
+000072a0: 7074 5f68 6964 6594 6a86 0300 008c 136e  pt_hide.j......n
+000072b0: 756d 6265 725f 736f 7572 6365 5f6c 696e  umber_source_lin
+000072c0: 6573 9489 8c0c 6275 696c 6465 725f 6e61  es....builder_na
+000072d0: 6d65 9468 dc8c 176d 696d 655f 7072 696f  me.h...mime_prio
+000072e0: 7269 7479 5f6f 7665 7272 6964 6573 9429  rity_overrides.)
+000072f0: 8c0d 6f75 7470 7574 5f73 7464 6572 7294  ..output_stderr.
+00007300: 685c 8c11 7265 6e64 6572 5f74 6578 745f  h\..render_text_
+00007310: 6c65 7865 7294 6a8f 0300 008c 1272 656e  lexer.j......ren
+00007320: 6465 725f 6572 726f 725f 6c65 7865 7294  der_error_lexer.
+00007330: 6a92 0300 008c 1472 656e 6465 725f 696d  j......render_im
+00007340: 6167 655f 6f70 7469 6f6e 7394 6a95 0300  age_options.j...
+00007350: 008c 1572 656e 6465 725f 6669 6775 7265  ...render_figure
+00007360: 5f6f 7074 696f 6e73 946a 9803 0000 8c16  _options.j......
+00007370: 7265 6e64 6572 5f6d 6172 6b64 6f77 6e5f  render_markdown_
+00007380: 666f 726d 6174 946a 9b03 0000 8c0d 6970  format.j......ip
+00007390: 7977 6964 6765 7473 5f6a 7394 6a9e 0300  ywidgets_js.j...
+000073a0: 008c 0d6f 7574 7075 745f 666f 6c64 6572  ...output_folder
+000073b0: 948c 5d2f 6d6e 742f 632f 5573 6572 732f  ..]/mnt/c/Users/
+000073c0: 7261 6e64 6f2f 446f 776e 6c6f 6164 732f  rando/Downloads/
+000073d0: 5079 7468 6f6e 5f57 6f72 6b73 7061 6365  Python_Workspace
+000073e0: 2f76 6f6c 6c73 6567 2d6e 6170 6172 692d  /vollseg-napari-
+000073f0: 7472 6163 6b6d 6174 652f 5f62 7569 6c64  trackmate/_build
+00007400: 2f6a 7570 7974 6572 5f65 7865 6375 7465  /jupyter_execute
+00007410: 948c 0a61 7070 656e 645f 6373 7394 888c  ...append_css...
+00007420: 0e6d 6574 6164 6174 615f 746f 5f66 6d94  .metadata_to_fm.
+00007430: 8975 628c 1169 6e74 6572 7370 6869 6e78  .ub..intersphinx
+00007440: 5f63 6163 6865 947d 948c 1569 6e74 6572  _cache.}...inter
+00007450: 7370 6869 6e78 5f69 6e76 656e 746f 7279  sphinx_inventory
+00007460: 947d 948c 1b69 6e74 6572 7370 6869 6e78  .}...intersphinx
+00007470: 5f6e 616d 6564 5f69 6e76 656e 746f 7279  _named_inventory
+00007480: 947d 948c 1973 7068 696e 785f 6465 7369  .}...sphinx_desi
+00007490: 676e 5f63 7373 5f63 6861 6e67 6564 9489  gn_css_changed..
+000074a0: 8c10 6e62 5f6e 6577 5f65 7865 635f 6461  ..nb_new_exec_da
+000074b0: 7461 9489 6898 689c 8c0b 6e62 5f6d 6574  ta..h.h...nb_met
+000074c0: 6164 6174 6194 6a20 0400 006a 3104 0000  adata.j ...j1...
+000074d0: 8594 5294 7562 2e                        ..R.ub.
```

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/.napari-hub/DESCRIPTION.html` & `vollseg-napari-trackmate-2.2.6/_build/html/search.html`

 * *Files 18% similar despite different names*

```diff
@@ -3,70 +3,71 @@
 <!DOCTYPE html>
 
 
 <html >
 
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
-
-    <title>&lt;no title&gt; &#8212; VollSeg extension for cell tracking</title>
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><title>Search - VollSeg extension for cell tracking</title>
 
 
 
   <script data-cfasync="false">
     document.documentElement.dataset.mode = localStorage.getItem("mode") || "";
     document.documentElement.dataset.theme = localStorage.getItem("theme") || "light";
   </script>
 
   <!-- Loaded before other Sphinx assets -->
-  <link href="../_static/styles/theme.css?digest=e353d410970836974a52" rel="stylesheet" />
-<link href="../_static/styles/bootstrap.css?digest=e353d410970836974a52" rel="stylesheet" />
-<link href="../_static/styles/pydata-sphinx-theme.css?digest=e353d410970836974a52" rel="stylesheet" />
-
-
-  <link href="../_static/vendor/fontawesome/6.1.2/css/all.min.css?digest=e353d410970836974a52" rel="stylesheet" />
-  <link rel="preload" as="font" type="font/woff2" crossorigin href="../_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2" />
-<link rel="preload" as="font" type="font/woff2" crossorigin href="../_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2" />
-<link rel="preload" as="font" type="font/woff2" crossorigin href="../_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2" />
-
-    <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
-    <link rel="stylesheet" href="../_static/styles/sphinx-book-theme.css?digest=14f4ca6b54d191a8c7657f6c759bf11a5fb86285" type="text/css" />
-    <link rel="stylesheet" type="text/css" href="../_static/togglebutton.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/sphinx-thebe.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/design-style.4045f2051d55cab465a707391d5b2007.min.css" />
+  <link href="_static/styles/theme.css?digest=e353d410970836974a52" rel="stylesheet" />
+<link href="_static/styles/bootstrap.css?digest=e353d410970836974a52" rel="stylesheet" />
+<link href="_static/styles/pydata-sphinx-theme.css?digest=e353d410970836974a52" rel="stylesheet" />
+
+
+  <link href="_static/vendor/fontawesome/6.1.2/css/all.min.css?digest=e353d410970836974a52" rel="stylesheet" />
+  <link rel="preload" as="font" type="font/woff2" crossorigin href="_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2" />
+<link rel="preload" as="font" type="font/woff2" crossorigin href="_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2" />
+<link rel="preload" as="font" type="font/woff2" crossorigin href="_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2" />
+
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <link rel="stylesheet" href="_static/styles/sphinx-book-theme.css?digest=14f4ca6b54d191a8c7657f6c759bf11a5fb86285" type="text/css" />
+    <link rel="stylesheet" type="text/css" href="_static/togglebutton.css" />
+    <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
+    <link rel="stylesheet" type="text/css" href="_static/sphinx-thebe.css" />
+    <link rel="stylesheet" type="text/css" href="_static/design-style.4045f2051d55cab465a707391d5b2007.min.css" />
 
   <!-- Pre-loaded scripts that we'll load fully later -->
-  <link rel="preload" as="script" href="../_static/scripts/bootstrap.js?digest=e353d410970836974a52" />
-<link rel="preload" as="script" href="../_static/scripts/pydata-sphinx-theme.js?digest=e353d410970836974a52" />
+  <link rel="preload" as="script" href="_static/scripts/bootstrap.js?digest=e353d410970836974a52" />
+<link rel="preload" as="script" href="_static/scripts/pydata-sphinx-theme.js?digest=e353d410970836974a52" />
 
-    <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
-    <script src="../_static/jquery.js"></script>
-    <script src="../_static/underscore.js"></script>
-    <script src="../_static/doctools.js"></script>
-    <script src="../_static/clipboard.min.js"></script>
-    <script src="../_static/copybutton.js"></script>
-    <script src="../_static/scripts/sphinx-book-theme.js?digest=5a5c038af52cf7bc1a1ec88eea08e6366ee68824"></script>
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+    <script src="_static/jquery.js"></script>
+    <script src="_static/underscore.js"></script>
+    <script src="_static/doctools.js"></script>
+    <script src="_static/clipboard.min.js"></script>
+    <script src="_static/copybutton.js"></script>
+    <script src="_static/scripts/sphinx-book-theme.js?digest=5a5c038af52cf7bc1a1ec88eea08e6366ee68824"></script>
     <script>let toggleHintShow = 'Click to show';</script>
     <script>let toggleHintHide = 'Click to hide';</script>
     <script>let toggleOpenOnPrint = 'true';</script>
-    <script src="../_static/togglebutton.js"></script>
+    <script src="_static/togglebutton.js"></script>
     <script>var togglebuttonSelector = '.toggle, .admonition.dropdown';</script>
-    <script src="../_static/design-tabs.js"></script>
+    <script src="_static/design-tabs.js"></script>
     <script>const THEBE_JS_URL = "https://unpkg.com/thebe@0.8.2/lib/index.js"
 const thebe_selector = ".thebe,.cell"
 const thebe_selector_input = "pre"
 const thebe_selector_output = ".output, .cell_output"
 </script>
-    <script async="async" src="../_static/sphinx-thebe.js"></script>
-    <script>DOCUMENTATION_OPTIONS.pagename = '.napari-hub/DESCRIPTION';</script>
-    <link rel="index" title="Index" href="../genindex.html" />
-    <link rel="search" title="Search" href="../search.html" />
+    <script async="async" src="_static/sphinx-thebe.js"></script>
+    <script>DOCUMENTATION_OPTIONS.pagename = 'search';</script>
+  <script src="_static/searchtools.js"></script>
+  <script src="_static/language_data.js"></script>
+  <script src="searchindex.js"></script>
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="#" />
   <meta name="viewport" content="width=device-width, initial-scale=1"/>
   <meta name="docsearch:language" content="None"/>
   </head>
 
 
   <body data-bs-spy="scroll" data-bs-target=".bd-toc-nav" data-offset="180" data-bs-root-margin="0px 0px -60%" data-default-mode="">
 
@@ -86,15 +87,15 @@
           id="__secondary"/>
   <label class="overlay overlay-secondary" for="__secondary"></label>
 
   <div class="search-button__wrapper">
     <div class="search-button__overlay"></div>
     <div class="search-button__search-container">
 <form class="bd-search d-flex align-items-center"
-      action="../search.html"
+      action="#"
       method="get">
   <i class="fa-solid fa-magnifying-glass"></i>
   <input type="search"
          class="form-control"
          name="q"
          id="search-input"
          placeholder="Search this book..."
@@ -124,35 +125,35 @@
 
   </div>
 
     <div class="sidebar-primary-items__start sidebar-primary__section">
         <div class="sidebar-primary-item">
 
 
-<a class="navbar-brand logo" href="../README.html">
+<a class="navbar-brand logo" href="README.html">
 
 
 
 
 
     <p class="title logo__title">VollSeg extension for cell tracking</p>
 
 </a></div>
         <div class="sidebar-primary-item"><nav class="bd-links" id="bd-docs-nav" aria-label="Main">
     <div class="bd-toc-item navbar-nav active">
 
         <ul class="nav bd-sidenav bd-sidenav__home-link">
             <li class="toctree-l1">
-                <a class="reference internal" href="../README.html">
+                <a class="reference internal" href="README.html">
                     vollseg-napari-trackmate
                 </a>
             </li>
         </ul>
         <ul class="nav bd-sidenav">
-<li class="toctree-l1"><a class="reference internal" href="../ALGORITHM.html">Algorithm</a></li>
+<li class="toctree-l1"><a class="reference internal" href="ALGORITHM.html">Algorithm</a></li>
 </ul>
 
     </div>
 </nav></div>
     </div>
 
 
@@ -216,15 +217,15 @@
 <span class="btn__text-container">Repository</span>
 </a>
 </li>
 
 
 
 
-      <li><a href="https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues/new?title=Issue%20on%20page%20%2F.napari-hub/DESCRIPTION.html&body=Your%20issue%20content%20here." target="_blank"
+      <li><a href="https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues/new?title=Issue%20on%20page%20%2Fsearch.html&body=Your%20issue%20content%20here." target="_blank"
    class="btn btn-sm btn-source-issues-button dropdown-item"
    title="Open an issue"
    data-bs-placement="left" data-bs-toggle="tooltip"
 >
 
 
 <span class="btn__icon-container">
@@ -236,62 +237,14 @@
 
   </ul>
 </div>
 
 
 
 
-
-
-<div class="dropdown dropdown-download-buttons">
-  <button class="btn dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false" aria-label="Download this page">
-    <i class="fas fa-download"></i>
-  </button>
-  <ul class="dropdown-menu">
-
-
-
-      <li><a href="../_sources/.napari-hub/DESCRIPTION.md" target="_blank"
-   class="btn btn-sm btn-download-source-button dropdown-item"
-   title="Download source file"
-   data-bs-placement="left" data-bs-toggle="tooltip"
->
-
-
-<span class="btn__icon-container">
-  <i class="fas fa-file"></i>
-  </span>
-<span class="btn__text-container">.md</span>
-</a>
-</li>
-
-
-
-
-      <li>
-<button onclick="window.print()"
-  class="btn btn-sm btn-download-pdf-button dropdown-item"
-  title="Print to PDF"
-  data-bs-placement="left" data-bs-toggle="tooltip"
->
-
-
-<span class="btn__icon-container">
-  <i class="fas fa-file-pdf"></i>
-  </span>
-<span class="btn__text-container">.pdf</span>
-</button>
-</li>
-
-  </ul>
-</div>
-
-
-
-
 <button onclick="toggleFullScreen()"
   class="btn btn-sm btn-fullscreen-button"
   title="Fullscreen mode"
   data-bs-placement="bottom" data-bs-toggle="tooltip"
 >
 
 
@@ -315,80 +268,59 @@
 <script>
 document.write(`
   <button class="btn btn-sm navbar-btn search-button search-button__button" title="Search" aria-label="Search" data-bs-placement="bottom" data-bs-toggle="tooltip">
     <i class="fa-solid fa-magnifying-glass"></i>
   </button>
 `);
 </script>
-<label class="sidebar-toggle secondary-toggle btn btn-sm" for="__secondary"title="Toggle secondary sidebar" data-bs-placement="bottom" data-bs-toggle="tooltip">
-    <span class="fa-solid fa-list"></span>
-</label>
+
 </div></div>
 
     </div>
 
 </div>
 </div>
 
 
+  <div class="bd-search-container">
+    <h1>Search</h1>
+    <noscript>
+      <div class="admonition error">
+        <p class="admonition-title">Error</p>
+        <p>Please activate JavaScript to enable the search functionality.</p>
+      </div>
+    </noscript>
 
-<div id="jb-print-docs-body" class="onlyprint">
-    <h1><no title></h1>
-    <!-- Table of contents -->
-    <div id="print-main-content">
-        <div id="jb-print-toc">
-
-            <div>
-                <h2> Contents </h2>
-            </div>
-            <nav aria-label="Page">
-                <ul class="simple visible nav section-nav flex-column">
-</ul>
-
-            </nav>
-        </div>
-    </div>
-</div>
-
-
-
-<div id="searchbox"></div>
-                <article class="bd-article" role="main">
-
-  <!-- This file is a placeholder for customizing description of your plugin
-on the napari hub if you wish. The readme file will be used by default if
-you wish not to do any customization for the napari hub listing.
-
-If you need some help writing a good description, check out our
-[guide](https://github.com/chanzuckerberg/napari-hub/wiki/Writing-the-Perfect-Description-for-your-Plugin)
--->
-<p>The developer has not yet provided a napari-hub specific description.</p>
-
-    <script type="text/x-thebe-config">
-    {
-        requestKernel: true,
-        binderOptions: {
-            repo: "binder-examples/jupyter-stacks-datascience",
-            ref: "master",
-        },
-        codeMirrorConfig: {
-            theme: "abcdef",
-            mode: "python"
-        },
-        kernelOptions: {
-            name: "python3",
-            path: "./.napari-hub"
-        },
-        predefinedOutput: true
+<form class="bd-search d-flex align-items-center"
+      action="#"
+      method="get">
+  <i class="fa-solid fa-magnifying-glass"></i>
+  <input type="search"
+         class="form-control"
+         name="q"
+         id="search-input"
+         placeholder="Search this book..."
+         aria-label="Search this book..."
+         autocomplete="off"
+         autocorrect="off"
+         autocapitalize="off"
+         spellcheck="false"/>
+  <span class="search-button__kbd-shortcut"><kbd class="kbd-shortcut__modifier">Ctrl</kbd>+<kbd>K</kbd></span>
+</form>
+    <div id="search-results"></div>
+  </div>
+  <script>
+    // Activate the search field on page load
+    let searchInput = document.querySelector("form.bd-search input");
+    if (searchInput) {
+        searchInput.focus();
+        searchInput.select();
+        console.log("[PST]: Set focus on search field.");
     }
-    </script>
-    <script>kernelName = 'python3'</script>
-
-                </article>
-
+  </script>
 
 
 
                 <footer class="bd-footer-article">
 
 <div class="footer-article-items footer-article__inner">
 
@@ -400,28 +332,14 @@
 
                 </footer>
 
             </div>
 
 
 
-                <div class="bd-sidebar-secondary bd-toc"><div class="sidebar-secondary-items sidebar-secondary__inner">
-
-  <div class="sidebar-secondary-item">
-  <div class="page-toc tocsection onthispage">
-    <i class="fa-solid fa-list"></i> Contents
-  </div>
-  <nav class="bd-toc-nav page-toc">
-    <ul class="simple visible nav section-nav flex-column">
-</ul>
-
-  </nav></div>
-
-</div></div>
-
 
           </div>
           <footer class="bd-footer-content">
 
 <div class="bd-footer-content__inner container">
 
   <div class="footer-item">
@@ -456,14 +374,14 @@
 
 
       </main>
     </div>
   </div>
 
   <!-- Scripts loaded after <body> so the DOM is not blocked -->
-  <script src="../_static/scripts/bootstrap.js?digest=e353d410970836974a52"></script>
-<script src="../_static/scripts/pydata-sphinx-theme.js?digest=e353d410970836974a52"></script>
+  <script src="_static/scripts/bootstrap.js?digest=e353d410970836974a52"></script>
+<script src="_static/scripts/pydata-sphinx-theme.js?digest=e353d410970836974a52"></script>
 
   <footer class="bd-footer">
   </footer>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -26,20 +26,16 @@
 VollSeg_extension_for_cell_tracking
     * vollseg-napari-trackmate
     * Algorithm
 
     *    Repository
     *    Open_issue
 
-    *    .md
-    *     .pdf
+****** Search ******
+Error
+Please activate JavaScript to enable the search functionality.
+ [Unknown INPUT type] Ctrl+K
 
-
-***** Contents *****
-
-The developer has not yet provided a napari-hub specific description.
-
- Contents
 By Varun Kapoor
 Â© Copyright 2022.
```

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/ALGORITHM.html` & `vollseg-napari-trackmate-2.2.6/_build/html/ALGORITHM.html`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/README.html` & `vollseg-napari-trackmate-2.2.6/_build/html/README.html`

 * *Files 2% similar despite different names*

```diff
@@ -364,15 +364,16 @@
 <a class="reference external" href="https://pypi.org/project/vollseg-napari-trackmate"><img alt="PyPI" src="https://img.shields.io/pypi/v/vollseg-napari-trackmate.svg?color=green" /></a>
 <a class="reference external" href="https://python.org"><img alt="Python Version" src="https://img.shields.io/pypi/pyversions/vollseg-napari-trackmate.svg?color=green" /></a>
 <a class="reference external" href="https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/actions"><img alt="tests" src="https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/workflows/tests/badge.svg" /></a>
 <a class="reference external" href="https://codecov.io/gh/Kapoorlabs-CAPED/vollseg-napari-trackmate"><img alt="codecov" src="https://codecov.io/gh/Kapoorlabs-CAPED/vollseg-napari-trackmate/branch/main/graph/badge.svg" /></a>
 <a class="reference external" href="https://napari-hub.org/plugins/vollseg-napari-trackmate"><img alt="napari hub" src="https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/vollseg-napari-trackmate" /></a></p>
 <p>Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library</p>
 <hr class="docutils" />
-<p>This <a class="reference external" href="https://github.com/napari/napari">napari</a> plugin was generated with <a class="reference external" href="https://github.com/audreyr/cookiecutter">Cookiecutter</a> using <a class="reference external" href="https://github.com/napari">&#64;napari</a>’s <a class="reference external" href="https://github.com/napari/cookiecutter-napari-plugin">cookiecutter-napari-plugin</a> template.</p>
+<p>Elaborate documentation for users of this repository at this <a class="reference external" href="https://kapoorlabs-caped.github.io/vollseg-napari-trackmate">documentation</a></p>
+<p>This <a class="reference external" href="https://github.com/napari/napari">napari</a> plugin was generated with <a class="reference external" href="https://github.com/audreyr/cookiecutter">Cookiecutter</a> using <a class="reference external" href="https://github.com/Kapoorlabs-CAPED/">&#64;caped</a>’s <a class="reference external" href="https://github.com/Kapoorlabs-CAPED/cookiecutter-kapoorlabs-napari-plugin">cookiecutter-napari-plugin</a> template.</p>
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/stable/plugins/index.html
 -->
@@ -395,15 +396,15 @@
 <section id="license">
 <h2>License<a class="headerlink" href="#license" title="Permalink to this headline">#</a></h2>
 <p>Distributed under the terms of the <a class="reference external" href="http://opensource.org/licenses/BSD-3-Clause">BSD-3</a> license,
 “vollseg-napari-trackmate” is free and open source software</p>
 </section>
 <section id="issues">
 <h2>Issues<a class="headerlink" href="#issues" title="Permalink to this headline">#</a></h2>
-<p>If you encounter any problems, please <a class="reference external" href="https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues">file an issue</a> along with a detailed description.</p>
+<p>If you encounter any problems, please <a class="reference external" href="https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack/issues">file an issue</a> along with a detailed description.</p>
 </section>
 </section>
 <div class="toctree-wrapper compound">
 </div>
 
     <script type="text/x-thebe-config">
     {
```

#### html2text {}

```diff
@@ -43,15 +43,16 @@
     * Issues
 
 ****** vollseg-napari-trackmate# ******
 [License_BSD-3] [PyPI] [Python_Version] [tests] [codecov] [napari_hub]
 Track analysis using TrackMate xml and csv generated tracks using
 NapaTrackMater as the base library
 ===============================================================================
-This napari plugin was generated with Cookiecutter using @napariâs
+Elaborate documentation for users of this repository at this documentation
+This napari plugin was generated with Cookiecutter using @capedâs
 cookiecutter-napari-plugin template.
 
 ***** Installation# *****
 You can install vollseg-napari-trackmate via pip:
 pip install vollseg-napari-trackmate
 To install latest development version :
 pip install git+https://github.com/Kapoorlabs-CAPED/vollseg-napari-
```

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_downloads/7304322522eb33b4c1d6fcd9b8dac0af/apply_autoencoder.py` & `vollseg-napari-trackmate-2.2.6/_build/html/_downloads/7304322522eb33b4c1d6fcd9b8dac0af/apply_autoencoder.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_downloads/c74da13609f81dcb94d74f88327c6b07/visualize_point_clouds.py` & `vollseg-napari-trackmate-2.2.6/_build/html/_downloads/c74da13609f81dcb94d74f88327c6b07/visualize_point_clouds.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_images/point_clouds_compared.png` & `vollseg-napari-trackmate-2.2.6/_build/html/_images/point_clouds_compared.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_sources/ALGORITHM.md` & `vollseg-napari-trackmate-2.2.6/_build/html/_sources/ALGORITHM.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_sources/README.md` & `vollseg-napari-trackmate-2.2.6/_build/html/_sources/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 [![codecov](https://codecov.io/gh/Kapoorlabs-CAPED/vollseg-napari-trackmate/branch/main/graph/badge.svg)](https://codecov.io/gh/Kapoorlabs-CAPED/vollseg-napari-trackmate)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/vollseg-napari-trackmate)](https://napari-hub.org/plugins/vollseg-napari-trackmate)
 
 Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 
 ----------------------------------
 
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+Elaborate documentation for users of this repository at this [documentation]
+
+This [napari] plugin was generated with [Cookiecutter] using [@caped]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/stable/plugins/index.html
@@ -47,21 +49,22 @@
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
+[@caped]: https://github.com/Kapoorlabs-CAPED/
 [MIT]: http://opensource.org/licenses/MIT
 [BSD-3]: http://opensource.org/licenses/BSD-3-Clause
 [GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
 [GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
 [Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-
-[file an issue]: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
+[cookiecutter-napari-plugin]: https://github.com/Kapoorlabs-CAPED/cookiecutter-kapoorlabs-napari-plugin
+[documentation]: https://kapoorlabs-caped.github.io/vollseg-napari-trackmate
+[file an issue]: https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
```

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_sphinx_design_static/design-tabs.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_sphinx_design_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/basic.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/clipboard.min.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/copybutton.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/copybutton.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/copybutton_funcs.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/design-tabs.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/doctools.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/images/logo_binder.svg` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/images/logo_colab.png` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/images/logo_deepnote.svg` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/images/logo_jupyterhub.svg` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/jquery-3.5.1.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/jquery.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/language_data.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/pygments.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/bootstrap.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/bootstrap.js.map` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/pydata-sphinx-theme.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/pydata-sphinx-theme.js.map` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/sphinx-book-theme.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/scripts/sphinx-book-theme.js.map` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/searchtools.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/sphinx-thebe.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/sphinx-thebe.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/sphinx-thebe.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/sphinx-thebe.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/styles/bootstrap.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/styles/pydata-sphinx-theme.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/styles/sphinx-book-theme.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/togglebutton.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/togglebutton.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/togglebutton.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/togglebutton.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/underscore-1.13.1.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/underscore.js` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/_static/webpack-macros.html` & `vollseg-napari-trackmate-2.2.6/_build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/genindex.html` & `vollseg-napari-trackmate-2.2.6/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/_build/html/searchindex.js` & `vollseg-napari-trackmate-2.2.6/_build/html/searchindex.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -18,259 +18,301 @@
     filenames: [".napari-hub/DESCRIPTION.md", "ALGORITHM.md", "README.md"],
     objects: {},
     objnames: {},
     objtypes: {},
     terms: {
         "2d": 1,
         "3": 2,
-        "3d": 1,
-        "do": 1,
+        "3d": [0, 1],
+        "do": [0, 1],
         As: 1,
-        If: 2,
+        If: [0, 2],
         In: 1,
-        The: [0, 1],
+        It: 0,
+        The: 1,
         To: 2,
         acceler: 1,
         accur: 1,
         achiev: 1,
         action: 1,
-        addit: 1,
+        addit: [0, 1],
+        affind: 0,
         ai: 1,
         aim: 1,
         akin: 1,
         all: 1,
-        allow: 1,
-        along: [1, 2],
+        allow: [0, 1],
+        along: [0, 1, 2],
         also: 1,
-        an: [1, 2],
-        analysi: [1, 2],
+        an: [0, 1, 2],
+        analysi: [0, 1, 2],
         angl: 1,
         ani: 2,
         append: 1,
-        appli: 1,
+        appli: [0, 1],
         approach: 1,
-        ar: [1, 2],
+        ar: [0, 1, 2],
         area: 1,
         auto: 1,
+        autoencod: 0,
         axi: 1,
-        base: [1, 2],
+        base: [0, 1, 2],
         basic: 1,
         befor: [1, 2],
         below: 1,
         between: 1,
         binari: 1,
         biolog: 1,
         boundari: 1,
         bsd: 2,
-        can: [1, 2],
+        bug: 0,
+        can: [0, 1, 2],
         cape: 2,
         carri: 1,
-        cell: 1,
+        cell: [0, 1],
         center: 1,
         centroid: 1,
         certain: 1,
         choos: 1,
+        citat: 0,
         classic: 1,
+        cloud: 0,
         co: 1,
         com: 2,
         combin: 1,
         come: 1,
         comparis: 1,
-        comput: 1,
-        convert: 1,
+        comput: [0, 1],
+        confer: 0,
+        convert: [0, 1],
         cookiecutt: 2,
         covari: 1,
         coverag: 2,
-        creat: 1,
-        csv: [1, 2],
+        creat: [0, 1],
+        csv: [0, 1, 2],
         cube: 1,
-        data: 1,
+        data: [0, 1],
         dataset: 1,
-        descript: [0, 2],
+        descript: 2,
         detail: [1, 2],
-        develop: [0, 1, 2],
+        develop: [1, 2],
         differ: 1,
         distanc: 1,
         distribut: 2,
+        document: [0, 2],
+        dynam: 0,
         eccentr: 1,
-        edg: 1,
+        edg: [0, 1],
         edit: 1,
         eigenvalu: 1,
         eigenvector: 1,
+        either: 0,
+        elabor: [0, 2],
         encod: 1,
         encount: 2,
         enhanc: 1,
         ensur: 2,
         evit: 1,
         expens: 1,
         far: 1,
-        fate: 1,
+        fate: [0, 1],
+        featur: 0,
         figur: 1,
-        fiji: 1,
-        file: [1, 2],
+        fiji: [0, 1],
+        file: [0, 1, 2],
+        find: 0,
         first: 1,
-        follow: 1,
+        follow: [0, 1],
         found: 1,
         free: 2,
-        from: 1,
+        from: [0, 1],
         further: 1,
-        gener: [1, 2],
+        gener: [0, 1, 2],
         git: 2,
-        github: 2,
+        github: [0, 2],
         give: 1,
         given: 1,
         gpu: 1,
         grant: 1,
-        ha: [0, 1],
-        have: 1,
+        gui: 0,
+        ha: 1,
+        have: [0, 1],
         hpc: 1,
-        http: 2,
-        hub: 0,
-        imag: 1,
+        html: 0,
+        http: [0, 2],
+        imag: [0, 1],
         input: 1,
         instanc: 1,
-        interest: 1,
+        intend: 0,
+        interest: [0, 1],
+        issu: 0,
         its: 1,
         kapoorlab: [1, 2],
-        label: 1,
+        label: [0, 1],
         largest: 1,
         latest: 2,
         least: 2,
         left: 1,
         librari: 2,
-        lightn: 1,
-        like: 1,
+        lightn: [0, 1],
+        like: [0, 1],
         locat: 1,
         made: 1,
         march: 1,
         mask: 1,
-        master: 1,
+        master: [0, 1],
         matrix: 1,
         membran: 1,
         microscopi: 1,
-        model: 1,
+        model: [0, 1],
         more: 1,
         most: 1,
         motion: 1,
         multi: 1,
         multipl: 1,
-        napari: [0, 1],
+        napari: 1,
         napatrackmat: 2,
+        need: 0,
         nuclei: 1,
         obtain: 1,
         open: 2,
         ordin: 1,
+        org: 0,
         origin: 1,
-        our: 1,
+        other: 0,
+        our: [0, 1],
         out: 1,
         output: 1,
         own: 1,
-        perform: 1,
+        packag: 0,
+        perform: [0, 1],
         pip: 2,
-        pleas: 2,
-        plugin: [1, 2],
+        pleas: [0, 2],
+        plugin: [0, 1, 2],
+        point: 0,
         popular: 1,
         pre: 1,
         predict: 1,
         prior: 1,
         problem: 2,
+        proceed: 0,
         produc: 1,
         program: 1,
-        provid: [0, 1],
+        provid: 1,
         pull: 2,
         purpos: 1,
         pytorch: 1,
         quantif: 1,
         radial: 1,
+        rais: 0,
         raw: 1,
         recommend: 1,
-        repositori: 1,
-        represent: 1,
+        relev: 0,
+        repositori: [0, 1, 2],
+        represent: [0, 1],
         request: 2,
-        research: 1,
+        research: [0, 1],
         run: 2,
         s: 2,
         same: [1, 2],
+        scipi: 0,
+        scipy2021: 0,
         script: 1,
+        segment: 0,
         select: 1,
         sentin: 1,
         serv: 1,
+        shape: 0,
         sight: 1,
         simpli: 1,
         softwar: [1, 2],
         solut: 1,
         some: 1,
         sourc: 2,
-        specif: 0,
         speed: 1,
-        spot: 1,
+        spot: [0, 1],
         stai: 2,
         startup: 1,
         step: 1,
         submit: [1, 2],
         success: 1,
         suit: 1,
         superior: 1,
+        support: 0,
         surfac: 1,
-        take: 1,
+        take: [0, 1],
         templat: 2,
         term: 2,
         test: 2,
         thei: 1,
         them: 1,
         therbi: 1,
         thi: [1, 2],
         those: 1,
-        time: 1,
+        time: [0, 1],
         timelaps: 1,
         tissu: 1,
         tool: 1,
         top: 1,
+        torch: 0,
         tox: 2,
-        track: 2,
-        trackmat: 1,
-        train: 1,
+        track: [0, 2],
+        trackmat: [0, 1],
+        train: [0, 1],
         type: 1,
         uk: 1,
         under: 2,
         up: 1,
-        us: [1, 2],
-        user: 1,
+        upload: 0,
+        us: [0, 1, 2],
+        user: [0, 1, 2],
         usual: 1,
+        varun_kapoor: 0,
         vector: 1,
         veri: 2,
-        version: [1, 2],
+        version: [0, 1, 2],
         via: 2,
         victori: 1,
         visual: 1,
-        vollseg: 1,
+        vollseg: [0, 1],
         volum: 1,
         wa: [1, 2],
         we: 1,
         welcom: 2,
         whcih: 1,
         when: 1,
-        which: 1,
-        xml: [1, 2],
-        yet: 0,
-        you: 2
+        which: [0, 1],
+        work: 0,
+        would: 0,
+        xml: [0, 1, 2],
+        you: [0, 2],
+        your: 0
     },
-    titles: ["&lt;no title&gt;", "Algorithm", "vollseg-napari-trackmate"],
+    titles: ["Description", "Algorithm", "vollseg-napari-trackmate"],
     titleterms: {
+        For: 0,
         algorithm: 1,
         autoencod: 1,
+        cite: 0,
         cloud: 1,
         contribut: 2,
+        descript: 0,
         dynam: 1,
         featur: 1,
+        get: 0,
+        guid: 0,
+        help: 0,
+        how: 0,
         instal: 2,
         issu: 2,
         licens: 2,
         napari: 2,
         point: 1,
         segment: 1,
         shape: 1,
+        thi: 0,
         track: 1,
         trackmat: 2,
-        vollseg: 2
+        vollseg: 2,
+        who: 0
     }
 })
```

### Comparing `vollseg-napari-trackmate-2.2.5/_config.yml` & `vollseg-napari-trackmate-2.2.6/_config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/examples/apply_autoencoder.py` & `vollseg-napari-trackmate-2.2.6/examples/apply_autoencoder.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/examples/visualize_point_clouds.py` & `vollseg-napari-trackmate-2.2.6/examples/visualize_point_clouds.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/images/kapoorlogo.png` & `vollseg-napari-trackmate-2.2.6/images/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/images/point_clouds_compared.png` & `vollseg-napari-trackmate-2.2.6/images/point_clouds_compared.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/setup.cfg` & `vollseg-napari-trackmate-2.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_data_model.py` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_sample_data.py` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_widget.py` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
             model_class_cloud_auto_encoder = CloudAutoEncoder
             autoencoder = model_class_cloud_auto_encoder(
                 num_features=config_cloud_auto_encoder["num_features"],
                 k=config_cloud_auto_encoder["k_nearest_neighbours"],
                 encoder_type=config_cloud_auto_encoder["encoder_type"],
                 decoder_type=config_cloud_auto_encoder["decoder_type"],
             )
-            autoencoder_model = AutoLightningModel.load_fvolrom_checkpoint(
+            autoencoder_model = AutoLightningModel.load_from_checkpoint(
                 path_auto,
                 network=autoencoder,
                 loss_func=ChamferLoss(),
                 optim_func=Adam(lr=0.001),
                 scale_z=config_cloud_auto_encoder["scale_z"],
                 scale_xy=config_cloud_auto_encoder["scale_xy"],
             )
```

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/_writer.py` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/napari.yaml` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.2.5
+Version: 2.2.6
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.2.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg-napari-trackmate-2.2.6/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.2.5/tox.ini` & `vollseg-napari-trackmate-2.2.6/tox.ini`

 * *Files identical despite different names*

