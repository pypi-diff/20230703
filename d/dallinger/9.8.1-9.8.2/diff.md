# Comparing `tmp/dallinger-9.8.1.tar.gz` & `tmp/dallinger-9.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dallinger-9.8.1.tar", last modified: Thu Jun 22 21:05:05 2023, max compression
+gzip compressed data, was "dallinger-9.8.2.tar", last modified: Mon Jul  3 01:42:03 2023, max compression
```

## Comparing `dallinger-9.8.1.tar` & `dallinger-9.8.2.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.717707 dallinger-9.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-22 21:04:27.000000 dallinger-9.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-22 21:04:27.000000 dallinger-9.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-22 21:05:05.717707 dallinger-9.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-22 21:04:27.000000 dallinger-9.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-22 21:05:01.000000 dallinger-9.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-06-22 21:04:27.000000 dallinger-9.8.1/constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/bots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger/command_line/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26878 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/docker_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger/default_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/default_configs/.dallingerconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/default_configs/global_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/default_configs/local_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger/dev_server/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/dev_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/dev_server/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/heroku.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/prepare_docker_image.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/docker/ssh_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/ssh_templates/docker-compose-server.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/wheel_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/experiment_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    58487 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/worker_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.689707 dallinger-9.8.1/dallinger/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/frontend/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/css/dallinger.css
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/css/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/frontend/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/frontend/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/dallinger2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/dallinger2.test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.689707 dallinger-9.8.1/dallinger/frontend/static/scripts/fingerprintjs2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/network-monitor.js
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/reconnecting-websocket.js
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/require.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/reqwest.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/spin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/store+json2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracker.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/load-tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-console.js
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.689707 dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/templates/base/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/ad.html
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/consent.html
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_database.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_develop.html
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_heroku.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_lifecycle.html
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/error-complete.html
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter_prolific.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/launch.html
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.705707 dallinger-9.8.1/dallinger/heroku/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/Procfile
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/Procfile_no_clock
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/rq_gevent_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)    68521 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    20449 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/pytest_dallinger.py
--rw-r--r--   0 runner    (1001) docker     (123)    64022 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/redis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.705707 dallinger-9.8.1/dallinger_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger_scripts/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger_scripts/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger_scripts/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-06-22 21:04:27.000000 dallinger-9.8.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.705707 dallinger-9.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.709707 dallinger-9.8.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.713707 dallinger-9.8.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.eot
--rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.woff
--rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/Dallinger AWS Group.png
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/burst.png
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/chain.png
--rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/class_chart.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/corner.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/delayed.png
--rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/directories.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/empty.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/front_back_layout.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/full.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/grid.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/grid_mini.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/grid_small.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/heroku.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/star.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.713707 dallinger-9.8.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/acknowledgments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/aws_etc_keys.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/build_demo_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/building_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/command_line_utility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/communicating_with_the_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/contributing_to_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/creating_an_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/dallinger_the_scientist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/demo_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/demoing_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/demos_on_heroku.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/developing_dallinger_setup_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/docker_only.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/docker_support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/docker_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/email_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/experiment_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/extra_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/installing_dallinger_for_users.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/javascript_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/learning_to_use_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/monitoring_a_live_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/postico_and_postgres.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/private_repo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/python_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/recruitment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/registration_on_OSF.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/required_experiment_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/rewarding_participants.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/running_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/running_the_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/scheduled_tasks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.713707 dallinger-9.8.1/docs/source/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/info.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/network.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/node.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/notification.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/participant.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/transformation.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/transmission.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/vector.csvs
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/the_experiment_class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/vagrant_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/waiting_rooms.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/web_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/writing_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-06-22 21:04:27.000000 dallinger-9.8.1/incubator.png
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-22 21:04:27.000000 dallinger-9.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 21:05:05.717707 dallinger-9.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-22 21:04:27.000000 dallinger-9.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.717707 dallinger-9.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_bots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    40624 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)    42171 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    77386 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_griduniverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_replay_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.857538 dallinger-9.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-03 01:41:22.000000 dallinger-9.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 01:41:22.000000 dallinger-9.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 01:42:03.857538 dallinger-9.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 01:41:22.000000 dallinger-9.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-03 01:41:55.000000 dallinger-9.8.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-07-03 01:41:22.000000 dallinger-9.8.2/constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.825538 dallinger-9.8.2/dallinger/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/bots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/command_line/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26878 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/docker_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/default_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/default_configs/.dallingerconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/default_configs/global_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/default_configs/local_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/dev_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/dev_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/dev_server/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/heroku.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/prepare_docker_image.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/docker/ssh_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/ssh_templates/docker-compose-server.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/wheel_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/experiment_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58487 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/worker_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.821538 dallinger-9.8.2/dallinger/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/css/dallinger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/css/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/dallinger2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/dallinger2.test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.821538 dallinger-9.8.2/dallinger/frontend/static/scripts/fingerprintjs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/network-monitor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/reconnecting-websocket.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/require.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/reqwest.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/spin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/store+json2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracker.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/load-tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-console.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.821538 dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.837538 dallinger-9.8.2/dallinger/frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.837538 dallinger-9.8.2/dallinger/frontend/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/ad.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/consent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_database.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_develop.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_heroku.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_lifecycle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/error-complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter_prolific.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/launch.html
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.837538 dallinger-9.8.2/dallinger/heroku/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/Procfile
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/Procfile_no_clock
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/rq_gevent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    68521 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20449 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/pytest_dallinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64022 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/redis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.841538 dallinger-9.8.2/dallinger_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger_scripts/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger_scripts/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger_scripts/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-03 01:41:22.000000 dallinger-9.8.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.841538 dallinger-9.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.845538 dallinger-9.8.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.849538 dallinger-9.8.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/Dallinger AWS Group.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/burst.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/chain.png
+-rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/class_chart.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/corner.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/delayed.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/directories.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/empty.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/front_back_layout.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/full.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/grid.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/grid_mini.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/grid_small.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/heroku.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/star.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.849538 dallinger-9.8.2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/acknowledgments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/aws_etc_keys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/build_demo_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/building_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/command_line_utility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/communicating_with_the_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/contributing_to_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/creating_an_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/dallinger_the_scientist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/demo_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/demoing_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/demos_on_heroku.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/developing_dallinger_setup_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/docker_only.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/docker_support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/docker_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/email_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/experiment_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/extra_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/installing_dallinger_for_users.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/javascript_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/learning_to_use_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/monitoring_a_live_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/postico_and_postgres.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/private_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/python_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/recruitment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/registration_on_OSF.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/required_experiment_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/rewarding_participants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/running_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/running_the_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/scheduled_tasks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.853538 dallinger-9.8.2/docs/source/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/info.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/network.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/node.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/notification.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/participant.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/transformation.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/transmission.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/vector.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/the_experiment_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/vagrant_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/waiting_rooms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/web_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/writing_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-07-03 01:41:22.000000 dallinger-9.8.2/incubator.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-03 01:41:22.000000 dallinger-9.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 01:42:03.857538 dallinger-9.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-03 01:41:22.000000 dallinger-9.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.857538 dallinger-9.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_bots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40624 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42171 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77386 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_griduniverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_replay_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_utils.py
```

### Comparing `dallinger-9.8.1/LICENSE` & `dallinger-9.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/PKG-INFO` & `dallinger-9.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.8.1
+Version: 9.8.2
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dallinger-9.8.1/README.md` & `dallinger-9.8.2/README.md`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/README.rst` & `dallinger-9.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/constraints.txt` & `dallinger-9.8.2/constraints.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/__init__.py` & `dallinger-9.8.2/dallinger/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/bots.py` & `dallinger-9.8.2/dallinger/bots.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/command_line/__init__.py` & `dallinger-9.8.2/dallinger/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/command_line/appdirs.py` & `dallinger-9.8.2/dallinger/command_line/appdirs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/command_line/config.py` & `dallinger-9.8.2/dallinger/command_line/config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/command_line/develop.py` & `dallinger-9.8.2/dallinger/command_line/develop.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/command_line/docker.py` & `dallinger-9.8.2/dallinger/command_line/docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/command_line/docker_ssh.py` & `dallinger-9.8.2/dallinger/command_line/docker_ssh.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/command_line/utils.py` & `dallinger-9.8.2/dallinger/command_line/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/config.py` & `dallinger-9.8.2/dallinger/config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/data.py` & `dallinger-9.8.2/dallinger/data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/db.py` & `dallinger-9.8.2/dallinger/db.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/default_configs/global_config_defaults.txt` & `dallinger-9.8.2/dallinger/default_configs/global_config_defaults.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/deployment.py` & `dallinger-9.8.2/dallinger/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/dev_server/app.py` & `dallinger-9.8.2/dallinger/dev_server/app.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/docker/deployment.py` & `dallinger-9.8.2/dallinger/docker/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/docker/docker-compose.yml.j2` & `dallinger-9.8.2/dallinger/docker/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2` & `dallinger-9.8.2/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/docker/ssh_templates/docker-compose-server.yml` & `dallinger-9.8.2/dallinger/docker/ssh_templates/docker-compose-server.yml`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/docker/tools.py` & `dallinger-9.8.2/dallinger/docker/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/docker/wheel_filename.py` & `dallinger-9.8.2/dallinger/docker/wheel_filename.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/experiment.py` & `dallinger-9.8.2/dallinger/experiment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/experiment_server/dashboard.py` & `dallinger-9.8.2/dallinger/experiment_server/dashboard.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/experiment_server/experiment_server.py` & `dallinger-9.8.2/dallinger/experiment_server/experiment_server.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/experiment_server/gunicorn.py` & `dallinger-9.8.2/dallinger/experiment_server/gunicorn.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/experiment_server/replay.py` & `dallinger-9.8.2/dallinger/experiment_server/replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/experiment_server/sockets.py` & `dallinger-9.8.2/dallinger/experiment_server/sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/experiment_server/utils.py` & `dallinger-9.8.2/dallinger/experiment_server/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/experiment_server/worker_events.py` & `dallinger-9.8.2/dallinger/experiment_server/worker_events.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/experiments/__init__.py` & `dallinger-9.8.2/dallinger/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/css/bootstrap.min.css` & `dallinger-9.8.2/dallinger/frontend/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/css/dashboard.css` & `dallinger-9.8.2/dallinger/frontend/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/bootstrap.min.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/clipboard.min.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/dallinger2.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/dallinger2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -432,15 +432,15 @@
             'participant_id': participantId
         }).done(function() {
             deferred.resolve();
             dlgr.allowExit();
 
             let openedFromDashboard;
             try {
-                openedFromDashboard = window.opener && !window.opener.location.pathname.startsWith("/dashboard")
+                openedFromDashboard = window.opener && window.opener.location.pathname.startsWith("/dashboard");
             } catch (error) {
                 // If the parent window was from a different origin (e.g. Prolific) then we see an error like this:
                 // Uncaught DOMException: Blocked a frame with origin XXX from accessing a cross-origin frame.
                 // We catch and ignore this error.
                 openedFromDashboard = false;
             }
```

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/dallinger2.test.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/dallinger2.test.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/jquery-3.6.0.min.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/network-monitor.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/network-monitor.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/popper.min.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/popper.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/reconnecting-websocket.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/reconnecting-websocket.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/require.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/require.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/reqwest.min.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/reqwest.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/spin.min.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/spin.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/store+json2.min.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/store+json2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/tracker.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/tracker.js.map` & `dallinger-9.8.2/dallinger/frontend/static/scripts/tracker.js.map`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/load-tracker.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/load-tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js` & `dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css` & `dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js` & `dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/base/ad.html` & `dallinger-9.8.2/dallinger/frontend/templates/base/ad.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/base/consent.html` & `dallinger-9.8.2/dallinger/frontend/templates/base/consent.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/base/dashboard.html` & `dallinger-9.8.2/dallinger/frontend/templates/base/dashboard.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/base/layout.html` & `dallinger-9.8.2/dallinger/frontend/templates/base/layout.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/base/questionnaire.html` & `dallinger-9.8.2/dallinger/frontend/templates/base/questionnaire.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/dashboard_database.html` & `dallinger-9.8.2/dallinger/frontend/templates/dashboard_database.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/dashboard_develop.html` & `dallinger-9.8.2/dallinger/frontend/templates/dashboard_develop.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/dashboard_home.html` & `dallinger-9.8.2/dallinger/frontend/templates/dashboard_home.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/dashboard_lifecycle.html` & `dallinger-9.8.2/dallinger/frontend/templates/dashboard_lifecycle.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/dashboard_monitor.html` & `dallinger-9.8.2/dallinger/frontend/templates/dashboard_monitor.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/dashboard_mturk.html` & `dallinger-9.8.2/dallinger/frontend/templates/dashboard_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/error-complete.html` & `dallinger-9.8.2/dallinger/frontend/templates/error-complete.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/error.html` & `dallinger-9.8.2/dallinger/frontend/templates/error.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter.html` & `dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter_mturk.html` & `dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter_prolific.html` & `dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter_prolific.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/login.html` & `dallinger-9.8.2/dallinger/frontend/templates/login.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/frontend/templates/waiting.html` & `dallinger-9.8.2/dallinger/frontend/templates/waiting.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/heroku/clock.py` & `dallinger-9.8.2/dallinger/heroku/clock.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/heroku/rq_gevent_worker.py` & `dallinger-9.8.2/dallinger/heroku/rq_gevent_worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/heroku/tools.py` & `dallinger-9.8.2/dallinger/heroku/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/jupyter.py` & `dallinger-9.8.2/dallinger/jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/models.py` & `dallinger-9.8.2/dallinger/models.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/mturk.py` & `dallinger-9.8.2/dallinger/mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/networks.py` & `dallinger-9.8.2/dallinger/networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/nodes.py` & `dallinger-9.8.2/dallinger/nodes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/notifications.py` & `dallinger-9.8.2/dallinger/notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/processes.py` & `dallinger-9.8.2/dallinger/processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/prolific.py` & `dallinger-9.8.2/dallinger/prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/pytest_dallinger.py` & `dallinger-9.8.2/dallinger/pytest_dallinger.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/recruiters.py` & `dallinger-9.8.2/dallinger/recruiters.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/redis_utils.py` & `dallinger-9.8.2/dallinger/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/registration.py` & `dallinger-9.8.2/dallinger/registration.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/transformations.py` & `dallinger-9.8.2/dallinger/transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger/utils.py` & `dallinger-9.8.2/dallinger/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger.egg-info/PKG-INFO` & `dallinger-9.8.2/dallinger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.8.1
+Version: 9.8.2
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dallinger-9.8.1/dallinger.egg-info/SOURCES.txt` & `dallinger-9.8.2/dallinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger.egg-info/requires.txt` & `dallinger-9.8.2/dallinger.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dallinger_scripts/worker.py` & `dallinger-9.8.2/dallinger_scripts/worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/dev-requirements.txt` & `dallinger-9.8.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/Makefile` & `dallinger-9.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/make.bat` & `dallinger-9.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.eot` & `dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.eot`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.svg` & `dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.svg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.ttf` & `dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.ttf`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.woff` & `dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.woff`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/Dallinger AWS Group.png` & `dallinger-9.8.2/docs/source/_static/Dallinger AWS Group.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/barplot.png` & `dallinger-9.8.2/docs/source/_static/barplot.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/burst.png` & `dallinger-9.8.2/docs/source/_static/burst.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/chain.png` & `dallinger-9.8.2/docs/source/_static/chain.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/class_chart.jpg` & `dallinger-9.8.2/docs/source/_static/class_chart.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/corner.jpg` & `dallinger-9.8.2/docs/source/_static/corner.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/custom.css` & `dallinger-9.8.2/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/delayed.png` & `dallinger-9.8.2/docs/source/_static/delayed.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/directories.jpg` & `dallinger-9.8.2/docs/source/_static/directories.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/empty.jpg` & `dallinger-9.8.2/docs/source/_static/empty.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/front_back_layout.jpg` & `dallinger-9.8.2/docs/source/_static/front_back_layout.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/full.png` & `dallinger-9.8.2/docs/source/_static/full.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/grid.png` & `dallinger-9.8.2/docs/source/_static/grid.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/grid_mini.png` & `dallinger-9.8.2/docs/source/_static/grid_mini.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/grid_small.png` & `dallinger-9.8.2/docs/source/_static/grid_small.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/heroku.jpg` & `dallinger-9.8.2/docs/source/_static/heroku.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/_static/star.png` & `dallinger-9.8.2/docs/source/_static/star.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/aws_etc_keys.rst` & `dallinger-9.8.2/docs/source/aws_etc_keys.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/build_demo_docs.py` & `dallinger-9.8.2/docs/source/build_demo_docs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/building_documentation.rst` & `dallinger-9.8.2/docs/source/building_documentation.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/classes.rst` & `dallinger-9.8.2/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/command_line_utility.rst` & `dallinger-9.8.2/docs/source/command_line_utility.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/communicating_with_the_server.rst` & `dallinger-9.8.2/docs/source/communicating_with_the_server.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/conf.py` & `dallinger-9.8.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/configuration.rst` & `dallinger-9.8.2/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/contributing_to_dallinger.rst` & `dallinger-9.8.2/docs/source/contributing_to_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/creating_an_experiment.rst` & `dallinger-9.8.2/docs/source/creating_an_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/demo_index.rst` & `dallinger-9.8.2/docs/source/demo_index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/demoing_dallinger.rst` & `dallinger-9.8.2/docs/source/demoing_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/demos_on_heroku.rst` & `dallinger-9.8.2/docs/source/demos_on_heroku.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/developing_dallinger_setup_guide.rst` & `dallinger-9.8.2/docs/source/developing_dallinger_setup_guide.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/docker_only.rst` & `dallinger-9.8.2/docs/source/docker_only.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/docker_support.rst` & `dallinger-9.8.2/docs/source/docker_support.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/docker_tutorial.rst` & `dallinger-9.8.2/docs/source/docker_tutorial.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/email_setup.rst` & `dallinger-9.8.2/docs/source/email_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/experiment_data.rst` & `dallinger-9.8.2/docs/source/experiment_data.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/extra_configuration.rst` & `dallinger-9.8.2/docs/source/extra_configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/index.rst` & `dallinger-9.8.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/installing_dallinger_for_users.rst` & `dallinger-9.8.2/docs/source/installing_dallinger_for_users.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/javascript_api.rst` & `dallinger-9.8.2/docs/source/javascript_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/learning_to_use_dallinger.rst` & `dallinger-9.8.2/docs/source/learning_to_use_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/monitoring_a_live_experiment.rst` & `dallinger-9.8.2/docs/source/monitoring_a_live_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/networks.rst` & `dallinger-9.8.2/docs/source/networks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/postico_and_postgres.rst` & `dallinger-9.8.2/docs/source/postico_and_postgres.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/private_repo.rst` & `dallinger-9.8.2/docs/source/private_repo.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/python_module.rst` & `dallinger-9.8.2/docs/source/python_module.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/recruitment.rst` & `dallinger-9.8.2/docs/source/recruitment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/required_experiment_files.rst` & `dallinger-9.8.2/docs/source/required_experiment_files.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/rewarding_participants.rst` & `dallinger-9.8.2/docs/source/rewarding_participants.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/running_bots.rst` & `dallinger-9.8.2/docs/source/running_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/running_the_tests.rst` & `dallinger-9.8.2/docs/source/running_the_tests.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/scheduled_tasks.rst` & `dallinger-9.8.2/docs/source/scheduled_tasks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/spelling_wordlist.txt` & `dallinger-9.8.2/docs/source/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/the_experiment_class.rst` & `dallinger-9.8.2/docs/source/the_experiment_class.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/troubleshooting.rst` & `dallinger-9.8.2/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/vagrant_setup.rst` & `dallinger-9.8.2/docs/source/vagrant_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/waiting_rooms.rst` & `dallinger-9.8.2/docs/source/waiting_rooms.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/web_api.rst` & `dallinger-9.8.2/docs/source/web_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/docs/source/writing_bots.rst` & `dallinger-9.8.2/docs/source/writing_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/incubator.png` & `dallinger-9.8.2/incubator.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/requirements.txt` & `dallinger-9.8.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/setup.py` & `dallinger-9.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
 
 setup_args = dict(
     name="dallinger",
     packages=["dallinger", "dallinger_scripts"],
-    version="9.8.1",
+    version="9.8.2",
     description="Laboratory automation for the behavioral and social sciences",
     long_description=README,
     long_description_content_type="text/markdown",
     url="http://github.com/Dallinger/Dallinger",
     maintainer="Jordan Suchow",
     maintainer_email="suchow@berkeley.edu",
     license="MIT",
```

### Comparing `dallinger-9.8.1/tests/test_agents.py` & `dallinger-9.8.2/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_api.py` & `dallinger-9.8.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_bots.py` & `dallinger-9.8.2/tests/test_bots.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_cli_config.py` & `dallinger-9.8.2/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_command_line.py` & `dallinger-9.8.2/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_config.py` & `dallinger-9.8.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_dashboard.py` & `dallinger-9.8.2/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_data.py` & `dallinger-9.8.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_db.py` & `dallinger-9.8.2/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_demos.py` & `dallinger-9.8.2/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_deployment.py` & `dallinger-9.8.2/tests/test_deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_docker.py` & `dallinger-9.8.2/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_environments.py` & `dallinger-9.8.2/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_experiment.py` & `dallinger-9.8.2/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_experiment_server.py` & `dallinger-9.8.2/tests/test_experiment_server.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_griduniverse.py` & `dallinger-9.8.2/tests/test_griduniverse.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_heroku.py` & `dallinger-9.8.2/tests/test_heroku.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_information.py` & `dallinger-9.8.2/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_jupyter.py` & `dallinger-9.8.2/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_models.py` & `dallinger-9.8.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_mturk.py` & `dallinger-9.8.2/tests/test_mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_networks.py` & `dallinger-9.8.2/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_notifications.py` & `dallinger-9.8.2/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_processes.py` & `dallinger-9.8.2/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_prolific.py` & `dallinger-9.8.2/tests/test_prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_recruiters.py` & `dallinger-9.8.2/tests/test_recruiters.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_replay.py` & `dallinger-9.8.2/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_replay_state.py` & `dallinger-9.8.2/tests/test_replay_state.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_sockets.py` & `dallinger-9.8.2/tests/test_sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_sources.py` & `dallinger-9.8.2/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_transformations.py` & `dallinger-9.8.2/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.1/tests/test_utils.py` & `dallinger-9.8.2/tests/test_utils.py`

 * *Files identical despite different names*

