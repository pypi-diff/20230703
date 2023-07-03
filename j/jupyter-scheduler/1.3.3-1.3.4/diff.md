# Comparing `tmp/jupyter_scheduler-1.3.3.tar.gz` & `tmp/jupyter_scheduler-1.3.4.tar.gz`

## Comparing `jupyter_scheduler-1.3.3.tar` & `jupyter_scheduler-1.3.4.tar`

### file list

```diff
@@ -1,168 +1,168 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.eslintrc.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.prettierrc
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.stylelintrc
--rw-r--r--   0        0        0    32953 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/CHANGELOG.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/MANIFEST.in
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/babel.config.js
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/conftest.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/install.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jest.config.js
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/setup.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/tsconfig.json
--rw-r--r--   0        0        0   473708 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/yarn.lock
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/binder/environment.yml
--rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/binder/postBuild
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/dev/seed.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/dev/templates/1.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/dev/templates/2.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/dev/templates/3.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/Makefile
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/conf.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/make.bat
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/requirements.txt
--rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/_static/jupyter_logo.png
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/contributors/index.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/developers/index.md
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/operators/index.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/index.md
--rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/actions_definition_details.png
--rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/actions_job_details.png
--rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/actions_list.png
--rw-r--r--   0        0        0   102590 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/create_job_form.png
--rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/create_job_from_filebrowser.png
--rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/create_job_from_notebook.png
--rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/custom_schedule.png
--rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/download_button.png
--rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/downloaded_files.png
--rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/headers.png
--rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/item_name.png
--rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/launcher.png
--rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/run_on_schedule.png
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter-config/nb-config/jupyter_scheduler.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter-config/server-config/jupyter_scheduler.json
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/_version.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/environments.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/exceptions.py
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/executors.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/extension.py
--rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/handlers.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/job_files_manager.py
--rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/models.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/orm.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/parameterize.py
--rw-r--r--   0        0        0    30914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/scheduler.py
--rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/task_runner.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/utils.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/package.json
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js
--rw-r--r--   0        0        0   347357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js
--rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js
--rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
--rw-r--r--   0        0        0   121687 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js.LICENSE.txt
--rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js.LICENSE.txt
--rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
--rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js.LICENSE.txt
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js
--rw-r--r--   0        0        0    80414 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/810.e798ed21e01eb5bbedc6.js
--rw-r--r--   0        0        0    25917 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js
--rw-r--r--   0        0        0    10072 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/remoteEntry.4716e9b91831e140cc89.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/style.js
--rw-r--r--   0        0        0    40850 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/mocks.py
--rw-r--r--   0        0        0    27273 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_handlers.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_job_files_manager.py
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_scheduler.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/utils.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.html
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/schema/plugin.json
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/advanced-options.tsx
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/context.ts
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/handler.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/hooks.ts
--rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/index.tsx
--rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/model.ts
--rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/notebook-jobs-panel.tsx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/size.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/svg.d.ts
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/theme-provider.ts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/tokens.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/__tests__/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/box.tsx
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/button-bar.tsx
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/button.tsx
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/cluster.tsx
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/collapsible-panel.tsx
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/compute-type-picker.tsx
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/confirm-buttons.tsx
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/confirm-dialog-buttons.tsx
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/create-schedule-options.tsx
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/environment-picker.tsx
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/error-boundary.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/heading.tsx
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/icon-buttons.tsx
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/icons.ts
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/input-file-snapshot.tsx
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/job-definition-row.tsx
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/job-file-link.tsx
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/job-row.tsx
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/labeled-value.tsx
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/output-format-picker.tsx
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/parameters-picker.tsx
--rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/schedule-inputs.tsx
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/stack.tsx
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/advanced-table/advanced-table-header.tsx
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/advanced-table/advanced-table.tsx
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/advanced-table/index.tsx
--rw-r--r--   0        0        0     8298 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/create-job-from-definition.tsx
--rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/create-job.tsx
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/edit-job-definition.tsx
--rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/list-jobs.tsx
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/detail-view/detail-view.tsx
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/detail-view/index.tsx
--rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/detail-view/job-definition.tsx
--rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/detail-view/job-detail.tsx
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/util/errors.tsx
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/util/job-name-validation.tsx
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/base.css
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/box.css
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/button.css
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/cluster.css
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/collapsible-panel.css
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/edit-job-definitions.css
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/heading.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/index.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/labeled-value.css
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/stack.css
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/variables.css
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/icons/calendar-add-on.svg
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/icons/calendar-month.svg
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/icons/event-note.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/tests/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/LICENSE
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/README.md
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/.eslintrc.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/.prettierrc
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/.stylelintrc
+-rw-r--r--   0        0        0    33780 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/CHANGELOG.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/MANIFEST.in
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/babel.config.js
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/conftest.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/install.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jest.config.js
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/setup.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/tsconfig.json
+-rw-r--r--   0        0        0   473708 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/yarn.lock
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/binder/environment.yml
+-rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/binder/postBuild
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/dev/seed.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/dev/templates/1.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/dev/templates/2.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/dev/templates/3.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/Makefile
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/conf.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/make.bat
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/requirements.txt
+-rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/_static/jupyter_logo.png
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/contributors/index.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/developers/index.md
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/operators/index.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/index.md
+-rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/actions_definition_details.png
+-rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/actions_job_details.png
+-rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/actions_list.png
+-rw-r--r--   0        0        0   102590 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/create_job_form.png
+-rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/create_job_from_filebrowser.png
+-rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/create_job_from_notebook.png
+-rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/custom_schedule.png
+-rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/download_button.png
+-rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/downloaded_files.png
+-rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/headers.png
+-rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/item_name.png
+-rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/launcher.png
+-rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/docs/users/images/run_on_schedule.png
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter-config/nb-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter-config/server-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/_version.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/environments.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/exceptions.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/executors.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/extension.py
+-rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/handlers.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/job_files_manager.py
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/models.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/orm.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/parameterize.py
+-rw-r--r--   0        0        0    30914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/scheduler.py
+-rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/task_runner.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/utils.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/package.json
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js
+-rw-r--r--   0        0        0   347357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js
+-rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js
+-rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
+-rw-r--r--   0        0        0   121687 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js.LICENSE.txt
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js.LICENSE.txt
+-rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
+-rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js.LICENSE.txt
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js
+-rw-r--r--   0        0        0    80414 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/810.e798ed21e01eb5bbedc6.js
+-rw-r--r--   0        0        0    25917 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js
+-rw-r--r--   0        0        0    10072 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/remoteEntry.86f5f4106f0214d0e3fd.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/style.js
+-rw-r--r--   0        0        0    40850 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/mocks.py
+-rw-r--r--   0        0        0    27273 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_handlers.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_job_files_manager.py
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_scheduler.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/utils.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.html
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/schema/plugin.json
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/advanced-options.tsx
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/context.ts
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/handler.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/hooks.ts
+-rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/index.tsx
+-rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/model.ts
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/notebook-jobs-panel.tsx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/size.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/svg.d.ts
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/theme-provider.ts
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/tokens.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/__tests__/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/box.tsx
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/button-bar.tsx
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/button.tsx
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/cluster.tsx
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/collapsible-panel.tsx
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/compute-type-picker.tsx
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/confirm-buttons.tsx
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/confirm-dialog-buttons.tsx
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/create-schedule-options.tsx
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/environment-picker.tsx
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/error-boundary.tsx
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/heading.tsx
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/icon-buttons.tsx
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/icons.ts
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/input-file-snapshot.tsx
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/job-definition-row.tsx
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/job-file-link.tsx
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/job-row.tsx
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/labeled-value.tsx
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/output-format-picker.tsx
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/parameters-picker.tsx
+-rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/schedule-inputs.tsx
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/stack.tsx
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/advanced-table/advanced-table-header.tsx
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/advanced-table/advanced-table.tsx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/components/advanced-table/index.tsx
+-rw-r--r--   0        0        0     8298 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/mainviews/create-job-from-definition.tsx
+-rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/mainviews/create-job.tsx
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/mainviews/edit-job-definition.tsx
+-rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/mainviews/list-jobs.tsx
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/mainviews/detail-view/detail-view.tsx
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/mainviews/detail-view/index.tsx
+-rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/mainviews/detail-view/job-definition.tsx
+-rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/mainviews/detail-view/job-detail.tsx
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/util/errors.tsx
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/src/util/job-name-validation.tsx
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/base.css
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/box.css
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/button.css
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/cluster.css
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/collapsible-panel.css
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/edit-job-definitions.css
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/heading.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/index.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/labeled-value.css
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/stack.css
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/variables.css
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/icons/calendar-add-on.svg
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/icons/calendar-month.svg
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/style/icons/event-note.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/ui-tests/tests/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/LICENSE
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/README.md
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.4/PKG-INFO
```

### Comparing `jupyter_scheduler-1.3.3/.eslintrc.js` & `jupyter_scheduler-1.3.4/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/.pre-commit-config.yaml` & `jupyter_scheduler-1.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/.stylelintrc` & `jupyter_scheduler-1.3.4/.stylelintrc`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/CHANGELOG.md` & `jupyter_scheduler-1.3.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.3.4
+
+([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v1.3.3...aaa3a8922a3021b1158c668e50b17e2bf708b4e6))
+
+### Bugs fixed
+
+- Pins Pydantic to version 1, adds Python 3.11 [#391](https://github.com/jupyter-server/jupyter-scheduler/pull/391) ([@JasonWeill](https://github.com/JasonWeill))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2023-06-27&to=2023-07-03&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Agithub-actions+updated%3A2023-06-27..2023-07-03&type=Issues) | [@JasonWeill](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3AJasonWeill+updated%3A2023-06-27..2023-07-03&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.3.3
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v1.3.2...5cd14b538a656e8fd2318dbbb687f2bf4da8fd37))
 
 ### Bugs fixed
 
 - Fix 'icon' prop typing for ConfirmButton component [#386](https://github.com/jupyter-server/jupyter-scheduler/pull/386) ([@andrii-i](https://github.com/andrii-i))
@@ -15,16 +31,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2023-05-11&to=2023-06-27&type=c))
 
 [@andrii-i](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Aandrii-i+updated%3A2023-05-11..2023-06-27&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Agithub-actions+updated%3A2023-05-11..2023-06-27&type=Issues) | [@JasonWeill](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3AJasonWeill+updated%3A2023-05-11..2023-06-27&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Apre-commit-ci+updated%3A2023-05-11..2023-06-27&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.3.2
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v1.3.1...6e4081a273b6da508942d3fe0b4a8ee75f2eade3))
 
 ### Bugs fixed
 
 - Fixed encoding while reading notebook in some platforms [#354](https://github.com/jupyter-server/jupyter-scheduler/pull/354) ([@3coins](https://github.com/3coins))
```

### Comparing `jupyter_scheduler-1.3.3/MANIFEST.in` & `jupyter_scheduler-1.3.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/conftest.py` & `jupyter_scheduler-1.3.4/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jest.config.js` & `jupyter_scheduler-1.3.4/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/package.json` & `jupyter_scheduler-1.3.4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'1.3.4'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.3"
+    "version": "1.3.4"
 }
```

### Comparing `jupyter_scheduler-1.3.3/tsconfig.json` & `jupyter_scheduler-1.3.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/yarn.lock` & `jupyter_scheduler-1.3.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/binder/postBuild` & `jupyter_scheduler-1.3.4/binder/postBuild`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/dev/seed.py` & `jupyter_scheduler-1.3.4/dev/seed.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/dev/templates/1.ipynb` & `jupyter_scheduler-1.3.4/dev/templates/1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/dev/templates/2.ipynb` & `jupyter_scheduler-1.3.4/dev/templates/2.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/dev/templates/3.ipynb` & `jupyter_scheduler-1.3.4/dev/templates/3.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/Makefile` & `jupyter_scheduler-1.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/conf.py` & `jupyter_scheduler-1.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/make.bat` & `jupyter_scheduler-1.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/_static/jupyter_logo.png` & `jupyter_scheduler-1.3.4/docs/_static/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/contributors/index.md` & `jupyter_scheduler-1.3.4/docs/contributors/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/developers/index.md` & `jupyter_scheduler-1.3.4/docs/developers/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/operators/index.md` & `jupyter_scheduler-1.3.4/docs/operators/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/index.md` & `jupyter_scheduler-1.3.4/docs/users/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/actions_definition_details.png` & `jupyter_scheduler-1.3.4/docs/users/images/actions_definition_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/actions_job_details.png` & `jupyter_scheduler-1.3.4/docs/users/images/actions_job_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/actions_list.png` & `jupyter_scheduler-1.3.4/docs/users/images/actions_list.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/create_job_form.png` & `jupyter_scheduler-1.3.4/docs/users/images/create_job_form.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/create_job_from_filebrowser.png` & `jupyter_scheduler-1.3.4/docs/users/images/create_job_from_filebrowser.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/create_job_from_notebook.png` & `jupyter_scheduler-1.3.4/docs/users/images/create_job_from_notebook.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/custom_schedule.png` & `jupyter_scheduler-1.3.4/docs/users/images/custom_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/download_button.png` & `jupyter_scheduler-1.3.4/docs/users/images/download_button.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/downloaded_files.png` & `jupyter_scheduler-1.3.4/docs/users/images/downloaded_files.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/headers.png` & `jupyter_scheduler-1.3.4/docs/users/images/headers.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/item_name.png` & `jupyter_scheduler-1.3.4/docs/users/images/item_name.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/launcher.png` & `jupyter_scheduler-1.3.4/docs/users/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/docs/users/images/run_on_schedule.png` & `jupyter_scheduler-1.3.4/docs/users/images/run_on_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/environments.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/environments.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/exceptions.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/executors.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/executors.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/extension.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/handlers.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/job_files_manager.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/job_files_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/models.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/models.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/orm.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/orm.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/parameterize.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/parameterize.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/scheduler.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/task_runner.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/task_runner.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/utils.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/package.json` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.86f5f4106f0214d0e3fd.js'}}",*

 * * "'version'": "'1.3.4'"}*

```diff
@@ -72,15 +72,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.4716e9b91831e140cc89.js",
+            "load": "static/remoteEntry.86f5f4106f0214d0e3fd.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_scheduler"
                 },
@@ -141,9 +141,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.3"
+    "version": "1.3.4"
 }
```

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'1.3.4'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.3"
+    "version": "1.3.4"
 }
```

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/810.e798ed21e01eb5bbedc6.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/810.e798ed21e01eb5bbedc6.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/remoteEntry.4716e9b91831e140cc89.js` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/remoteEntry.86f5f4106f0214d0e3fd.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -141,15 +141,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : d > l.from)) && (n[r] = {
                             get: t,
                             from: d,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (l("@emotion/react", "11.10.4", (() => Promise.all([P.e(275), P.e(506), P.e(271), P.e(171)]).then((() => () => P(5506))))), l("@emotion/styled", "11.10.4", (() => Promise.all([P.e(378), P.e(271), P.e(211), P.e(799), P.e(122)]).then((() => () => P(4378))))), l("@jupyterlab/scheduler", "1.3.3", (() => Promise.all([P.e(687), P.e(470), P.e(271), P.e(222), P.e(948), P.e(810)]).then((() => () => P(1810))))), l("@mui/material", "5.10.6", (() => Promise.all([P.e(687), P.e(177), P.e(470), P.e(271), P.e(222), P.e(948)]).then((() => () => P(4177))))), l("@mui/system", "5.10.6", (() => Promise.all([P.e(275), P.e(687), P.e(871), P.e(271), P.e(211), P.e(222)]).then((() => () => P(1871))))), l("cronstrue", "2.12.0", (() => P.e(458).then((() => () => P(2458))))), l("tzdata", "1.0.33", (() => P.e(613).then((() => () => P(8613)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@emotion/react", "11.10.4", (() => Promise.all([P.e(275), P.e(506), P.e(271), P.e(171)]).then((() => () => P(5506))))), l("@emotion/styled", "11.10.4", (() => Promise.all([P.e(378), P.e(271), P.e(211), P.e(799), P.e(122)]).then((() => () => P(4378))))), l("@jupyterlab/scheduler", "1.3.4", (() => Promise.all([P.e(687), P.e(470), P.e(271), P.e(222), P.e(948), P.e(810)]).then((() => () => P(1810))))), l("@mui/material", "5.10.6", (() => Promise.all([P.e(687), P.e(177), P.e(470), P.e(271), P.e(222), P.e(948)]).then((() => () => P(4177))))), l("@mui/system", "5.10.6", (() => Promise.all([P.e(275), P.e(687), P.e(871), P.e(271), P.e(211), P.e(222)]).then((() => () => P(1871))))), l("cronstrue", "2.12.0", (() => P.e(458).then((() => () => P(2458))))), l("tzdata", "1.0.33", (() => P.e(613).then((() => () => P(8613)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/third-party-licenses.json` & `jupyter_scheduler-1.3.4/jupyter_scheduler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/mocks.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_handlers.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_job_files_manager.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_job_files_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_scheduler.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/utils.py` & `jupyter_scheduler-1.3.4/jupyter_scheduler/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb` & `jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb` & `jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz` & `jupyter_scheduler-1.3.4/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/schema/plugin.json` & `jupyter_scheduler-1.3.4/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/advanced-options.tsx` & `jupyter_scheduler-1.3.4/src/advanced-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/handler.ts` & `jupyter_scheduler-1.3.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/index.tsx` & `jupyter_scheduler-1.3.4/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/model.ts` & `jupyter_scheduler-1.3.4/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/notebook-jobs-panel.tsx` & `jupyter_scheduler-1.3.4/src/notebook-jobs-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/theme-provider.ts` & `jupyter_scheduler-1.3.4/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/tokens.ts` & `jupyter_scheduler-1.3.4/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/cluster.tsx` & `jupyter_scheduler-1.3.4/src/components/cluster.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/collapsible-panel.tsx` & `jupyter_scheduler-1.3.4/src/components/collapsible-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/compute-type-picker.tsx` & `jupyter_scheduler-1.3.4/src/components/compute-type-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/confirm-buttons.tsx` & `jupyter_scheduler-1.3.4/src/components/confirm-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/confirm-dialog-buttons.tsx` & `jupyter_scheduler-1.3.4/src/components/confirm-dialog-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/create-schedule-options.tsx` & `jupyter_scheduler-1.3.4/src/components/create-schedule-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/environment-picker.tsx` & `jupyter_scheduler-1.3.4/src/components/environment-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/error-boundary.tsx` & `jupyter_scheduler-1.3.4/src/components/error-boundary.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/heading.tsx` & `jupyter_scheduler-1.3.4/src/components/heading.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/icon-buttons.tsx` & `jupyter_scheduler-1.3.4/src/components/icon-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/icons.ts` & `jupyter_scheduler-1.3.4/src/components/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/input-file-snapshot.tsx` & `jupyter_scheduler-1.3.4/src/components/input-file-snapshot.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/job-definition-row.tsx` & `jupyter_scheduler-1.3.4/src/components/job-definition-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/job-file-link.tsx` & `jupyter_scheduler-1.3.4/src/components/job-file-link.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/job-row.tsx` & `jupyter_scheduler-1.3.4/src/components/job-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/labeled-value.tsx` & `jupyter_scheduler-1.3.4/src/components/labeled-value.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/output-format-picker.tsx` & `jupyter_scheduler-1.3.4/src/components/output-format-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/parameters-picker.tsx` & `jupyter_scheduler-1.3.4/src/components/parameters-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/schedule-inputs.tsx` & `jupyter_scheduler-1.3.4/src/components/schedule-inputs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/advanced-table/advanced-table-header.tsx` & `jupyter_scheduler-1.3.4/src/components/advanced-table/advanced-table-header.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/components/advanced-table/advanced-table.tsx` & `jupyter_scheduler-1.3.4/src/components/advanced-table/advanced-table.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/mainviews/create-job-from-definition.tsx` & `jupyter_scheduler-1.3.4/src/mainviews/create-job-from-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/mainviews/create-job.tsx` & `jupyter_scheduler-1.3.4/src/mainviews/create-job.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/mainviews/edit-job-definition.tsx` & `jupyter_scheduler-1.3.4/src/mainviews/edit-job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/mainviews/list-jobs.tsx` & `jupyter_scheduler-1.3.4/src/mainviews/list-jobs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/mainviews/detail-view/detail-view.tsx` & `jupyter_scheduler-1.3.4/src/mainviews/detail-view/detail-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/mainviews/detail-view/job-definition.tsx` & `jupyter_scheduler-1.3.4/src/mainviews/detail-view/job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/mainviews/detail-view/job-detail.tsx` & `jupyter_scheduler-1.3.4/src/mainviews/detail-view/job-detail.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/util/errors.tsx` & `jupyter_scheduler-1.3.4/src/util/errors.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/src/util/job-name-validation.tsx` & `jupyter_scheduler-1.3.4/src/util/job-name-validation.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/style/base.css` & `jupyter_scheduler-1.3.4/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/style/button.css` & `jupyter_scheduler-1.3.4/style/button.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/style/cluster.css` & `jupyter_scheduler-1.3.4/style/cluster.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/style/stack.css` & `jupyter_scheduler-1.3.4/style/stack.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/style/icons/calendar-add-on.svg` & `jupyter_scheduler-1.3.4/style/icons/calendar-add-on.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/style/icons/calendar-month.svg` & `jupyter_scheduler-1.3.4/style/icons/calendar-month.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/ui-tests/README.md` & `jupyter_scheduler-1.3.4/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/ui-tests/jupyter_server_test_config.py` & `jupyter_scheduler-1.3.4/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/.gitignore` & `jupyter_scheduler-1.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/LICENSE` & `jupyter_scheduler-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/README.md` & `jupyter_scheduler-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.3/pyproject.toml` & `jupyter_scheduler-1.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.3.1", "jupyterlab~=3.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_scheduler"
-version = "1.3.3"
+version = "1.3.4"
 description = "A JupyterLab extension for running notebook jobs"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "Project Jupyter" },
 ]
@@ -22,20 +22,21 @@
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "jupyter_server>=1.6,<3",
     "traitlets",
     "nbconvert",
-    "pydantic",
+    "pydantic~=1.10",
     "sqlalchemy<2",
     "croniter",
     "pytz",
     "fsspec",
     "s3fs",
     "psutil"
 ]
@@ -89,15 +90,15 @@
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
 build_cmd = "install:extension"
 npm = ["jlpm"]
 source_dir = "src"
 build_dir = "jupyter_scheduler/labextension"
 
 [tool.tbump.version]
-current = "1.3.3"
+current = "1.3.4"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [[tool.tbump.file]]
 src = "pyproject.toml"
 version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\""
 
 [[tool.tbump.file]]
```

### Comparing `jupyter_scheduler-1.3.3/PKG-INFO` & `jupyter_scheduler-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_scheduler
-Version: 1.3.3
+Version: 1.3.4
 Summary: A JupyterLab extension for running notebook jobs
 Project-URL: Homepage, https://github.com/jupyter-server/jupyter-scheduler
 Author: Project Jupyter
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Project Jupyter
         All rights reserved.
@@ -43,21 +43,22 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: croniter
 Requires-Dist: fsspec
 Requires-Dist: jupyter-server<3,>=1.6
 Requires-Dist: nbconvert
 Requires-Dist: psutil
-Requires-Dist: pydantic
+Requires-Dist: pydantic~=1.10
 Requires-Dist: pytz
 Requires-Dist: s3fs
 Requires-Dist: sqlalchemy<2
 Requires-Dist: traitlets
 Provides-Extra: dev
 Requires-Dist: click; extra == 'dev'
 Provides-Extra: docs
```

