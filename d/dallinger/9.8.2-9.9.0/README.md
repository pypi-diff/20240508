# Comparing `tmp/dallinger-9.8.2.tar.gz` & `tmp/dallinger-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dallinger-9.8.2.tar", last modified: Mon Jul  3 01:42:03 2023, max compression
+gzip compressed data, was "dallinger-9.9.0.tar", last modified: Thu Jul 27 11:37:13 2023, max compression
```

## Comparing `dallinger-9.8.2.tar` & `dallinger-9.9.0.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.857538 dallinger-9.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-03 01:41:22.000000 dallinger-9.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 01:41:22.000000 dallinger-9.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 01:42:03.857538 dallinger-9.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 01:41:22.000000 dallinger-9.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-03 01:41:55.000000 dallinger-9.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-07-03 01:41:22.000000 dallinger-9.8.2/constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.825538 dallinger-9.8.2/dallinger/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/bots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/command_line/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26878 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/docker_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/command_line/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/default_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/default_configs/.dallingerconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/default_configs/global_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/default_configs/local_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/dev_server/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/dev_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/dev_server/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/heroku.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/prepare_docker_image.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/docker/ssh_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/ssh_templates/docker-compose-server.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/docker/wheel_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/experiment_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    58487 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiment_server/worker_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.821538 dallinger-9.8.2/dallinger/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger/frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/css/dallinger.css
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/css/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/dallinger2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/dallinger2.test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.821538 dallinger-9.8.2/dallinger/frontend/static/scripts/fingerprintjs2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/network-monitor.js
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/reconnecting-websocket.js
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/require.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/reqwest.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/spin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/store+json2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracker.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/load-tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-console.js
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.821538 dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.833538 dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.837538 dallinger-9.8.2/dallinger/frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.837538 dallinger-9.8.2/dallinger/frontend/templates/base/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/ad.html
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/consent.html
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/base/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_database.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_develop.html
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_heroku.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_lifecycle.html
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/dashboard_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/error-complete.html
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter_prolific.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/launch.html
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/frontend/templates/waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.837538 dallinger-9.8.2/dallinger/heroku/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/Procfile
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/Procfile_no_clock
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/rq_gevent_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/heroku/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)    68521 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    20449 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/pytest_dallinger.py
--rw-r--r--   0 runner    (1001) docker     (123)    64022 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/redis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.829538 dallinger-9.8.2/dallinger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 01:42:03.000000 dallinger-9.8.2/dallinger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.841538 dallinger-9.8.2/dallinger_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger_scripts/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger_scripts/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-03 01:41:22.000000 dallinger-9.8.2/dallinger_scripts/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-03 01:41:22.000000 dallinger-9.8.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.841538 dallinger-9.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.845538 dallinger-9.8.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.849538 dallinger-9.8.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.eot
--rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.woff
--rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/Dallinger AWS Group.png
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/burst.png
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/chain.png
--rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/class_chart.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/corner.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/delayed.png
--rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/directories.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/empty.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/front_back_layout.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/full.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/grid.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/grid_mini.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/grid_small.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/heroku.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_static/star.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.849538 dallinger-9.8.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/acknowledgments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/aws_etc_keys.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/build_demo_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/building_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/command_line_utility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/communicating_with_the_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/contributing_to_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/creating_an_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/dallinger_the_scientist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/demo_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/demoing_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/demos_on_heroku.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/developing_dallinger_setup_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/docker_only.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/docker_support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/docker_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/email_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/experiment_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/extra_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/installing_dallinger_for_users.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/javascript_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/learning_to_use_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/monitoring_a_live_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/postico_and_postgres.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/private_repo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/python_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/recruitment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/registration_on_OSF.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/required_experiment_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/rewarding_participants.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/running_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/running_the_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/scheduled_tasks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.853538 dallinger-9.8.2/docs/source/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/info.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/network.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/node.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/notification.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/participant.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/transformation.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/transmission.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/schemas/vector.csvs
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/the_experiment_class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/vagrant_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/waiting_rooms.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/web_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-03 01:41:22.000000 dallinger-9.8.2/docs/source/writing_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-07-03 01:41:22.000000 dallinger-9.8.2/incubator.png
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-03 01:41:22.000000 dallinger-9.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 01:42:03.857538 dallinger-9.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-03 01:41:22.000000 dallinger-9.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:42:03.857538 dallinger-9.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_bots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    40624 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)    42171 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    77386 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_griduniverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_replay_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-03 01:41:22.000000 dallinger-9.8.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.948804 dallinger-9.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-27 11:36:39.000000 dallinger-9.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-27 11:36:39.000000 dallinger-9.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-27 11:37:13.948804 dallinger-9.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-27 11:36:39.000000 dallinger-9.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-27 11:37:09.000000 dallinger-9.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-27 11:36:39.000000 dallinger-9.9.0/constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.924804 dallinger-9.9.0/dallinger/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/bots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.924804 dallinger-9.9.0/dallinger/command_line/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/command_line/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/command_line/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/command_line/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/command_line/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30870 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/command_line/docker_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/command_line/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.928804 dallinger-9.9.0/dallinger/default_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/default_configs/.dallingerconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/default_configs/global_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/default_configs/local_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.928804 dallinger-9.9.0/dallinger/dev_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/dev_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/dev_server/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.928804 dallinger-9.9.0/dallinger/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/docker/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/docker/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/docker/heroku.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/docker/prepare_docker_image.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.928804 dallinger-9.9.0/dallinger/docker/ssh_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/docker/ssh_templates/docker-compose-server.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/docker/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/docker/wheel_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62502 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.928804 dallinger-9.9.0/dallinger/experiment_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiment_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiment_server/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58980 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiment_server/experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiment_server/gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiment_server/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiment_server/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiment_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiment_server/worker_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.928804 dallinger-9.9.0/dallinger/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.912804 dallinger-9.9.0/dallinger/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.928804 dallinger-9.9.0/dallinger/frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.928804 dallinger-9.9.0/dallinger/frontend/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/css/dallinger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/css/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.928804 dallinger-9.9.0/dallinger/frontend/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.932804 dallinger-9.9.0/dallinger/frontend/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/dallinger2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/dallinger2.test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.912804 dallinger-9.9.0/dallinger/frontend/static/scripts/fingerprintjs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.932804 dallinger-9.9.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/network-monitor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/reconnecting-websocket.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/require.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/reqwest.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/spin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/store+json2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/tracker.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.932804 dallinger-9.9.0/dallinger/frontend/static/scripts/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/tracking/load-tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/tracking/scribe-console.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.912804 dallinger-9.9.0/dallinger/frontend/static/vis@4.17.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.932804 dallinger-9.9.0/dallinger/frontend/static/vis@4.17.0/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.932804 dallinger-9.9.0/dallinger/frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.936804 dallinger-9.9.0/dallinger/frontend/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/base/ad.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/base/consent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/base/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/base/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/base/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/dashboard_database.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/dashboard_develop.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/dashboard_heroku.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/dashboard_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/dashboard_lifecycle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/dashboard_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/dashboard_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/error-complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/exit_recruiter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/exit_recruiter_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/exit_recruiter_prolific.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/launch.html
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/frontend/templates/waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.936804 dallinger-9.9.0/dallinger/heroku/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/heroku/Procfile
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/heroku/Procfile_no_clock
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/heroku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/heroku/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/heroku/rq_gevent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/heroku/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/heroku/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    68521 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20503 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/pytest_dallinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64067 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/redis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33114 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.924804 dallinger-9.9.0/dallinger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-27 11:37:13.000000 dallinger-9.9.0/dallinger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-27 11:37:13.000000 dallinger-9.9.0/dallinger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:37:13.000000 dallinger-9.9.0/dallinger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-27 11:37:13.000000 dallinger-9.9.0/dallinger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:37:13.000000 dallinger-9.9.0/dallinger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-27 11:37:13.000000 dallinger-9.9.0/dallinger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 11:37:13.000000 dallinger-9.9.0/dallinger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.936804 dallinger-9.9.0/dallinger_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger_scripts/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger_scripts/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-27 11:36:39.000000 dallinger-9.9.0/dallinger_scripts/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-07-27 11:36:39.000000 dallinger-9.9.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.936804 dallinger-9.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.940804 dallinger-9.9.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.944804 dallinger-9.9.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/AvenirLTStd-Book_gdi.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/AvenirLTStd-Book_gdi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/AvenirLTStd-Book_gdi.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/Dallinger AWS Group.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/burst.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/chain.png
+-rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/class_chart.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/corner.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/delayed.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/directories.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/empty.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/front_back_layout.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/full.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/grid.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/grid_mini.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/grid_small.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/heroku.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_static/star.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.944804 dallinger-9.9.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/acknowledgments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/aws_etc_keys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/build_demo_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/building_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/command_line_utility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/communicating_with_the_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/contributing_to_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/creating_an_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/dallinger_the_scientist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/demo_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/demoing_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/demos_on_heroku.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/developing_dallinger_setup_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/docker_only.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/docker_support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/docker_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/email_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/experiment_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/extra_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/installing_dallinger_for_users.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/javascript_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/learning_to_use_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/monitoring_a_live_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/postico_and_postgres.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/private_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/python_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/recruitment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/registration_on_OSF.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/required_experiment_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/rewarding_participants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/running_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/running_the_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/scheduled_tasks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.944804 dallinger-9.9.0/docs/source/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/schemas/info.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/schemas/network.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/schemas/node.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/schemas/notification.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/schemas/participant.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/schemas/transformation.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/schemas/transmission.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/schemas/vector.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/the_experiment_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/vagrant_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/waiting_rooms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/web_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-27 11:36:39.000000 dallinger-9.9.0/docs/source/writing_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-07-27 11:36:39.000000 dallinger-9.9.0/incubator.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-27 11:36:39.000000 dallinger-9.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-27 11:37:13.948804 dallinger-9.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-27 11:36:39.000000 dallinger-9.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:37:13.948804 dallinger-9.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_bots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40624 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42171 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74418 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_griduniverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57547 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_replay_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-27 11:36:39.000000 dallinger-9.9.0/tests/test_utils.py
```

### Comparing `dallinger-9.8.2/LICENSE` & `dallinger-9.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/PKG-INFO` & `dallinger-9.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.8.2
+Version: 9.9.0
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Provides-Extra: data
 Provides-Extra: dev
 Provides-Extra: docker
 License-File: LICENSE
 
 Dallinger
 =======
-[![Build Status](https://github.com/dallinger/Dallinger/workflows/continuous-integration/badge.svg)](https://github.com/Dallinger/Dallinger/actions?query=workflow%3Acontinuous-integration)
+[![Build Status](https://github.com/dallinger/Dallinger/actions/workflows/deploy.yml/badge.svg)](https://github.com/dallinger/Dallinger/actions/workflows/deploy.yml/badge.svg)
 [![Demos](https://img.shields.io/badge/demos-11-edd172.svg)](http://dallinger.readthedocs.io/en/latest/#demos)
 [![codecov](https://codecov.io/gh/Dallinger/Dallinger/branch/master/graph/badge.svg)](https://codecov.io/gh/Dallinger/Dallinger)
 [![Code Climate](https://codeclimate.com/github/Dallinger/Dallinger/badges/gpa.svg)](https://codeclimate.com/github/Dallinger/Dallinger)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://en.wikipedia.org/wiki/MIT_License)
 
 <img src="https://raw.githubusercontent.com/Dallinger/Dallinger/master/incubator.png" width="125" alt="Dallinger's incubator">
```

### Comparing `dallinger-9.8.2/README.md` & `dallinger-9.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Dallinger
 =======
-[![Build Status](https://github.com/dallinger/Dallinger/workflows/continuous-integration/badge.svg)](https://github.com/Dallinger/Dallinger/actions?query=workflow%3Acontinuous-integration)
+[![Build Status](https://github.com/dallinger/Dallinger/actions/workflows/deploy.yml/badge.svg)](https://github.com/dallinger/Dallinger/actions/workflows/deploy.yml/badge.svg)
 [![Demos](https://img.shields.io/badge/demos-11-edd172.svg)](http://dallinger.readthedocs.io/en/latest/#demos)
 [![codecov](https://codecov.io/gh/Dallinger/Dallinger/branch/master/graph/badge.svg)](https://codecov.io/gh/Dallinger/Dallinger)
 [![Code Climate](https://codeclimate.com/github/Dallinger/Dallinger/badges/gpa.svg)](https://codeclimate.com/github/Dallinger/Dallinger)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://en.wikipedia.org/wiki/MIT_License)
 
 <img src="https://raw.githubusercontent.com/Dallinger/Dallinger/master/incubator.png" width="125" alt="Dallinger's incubator">
```

### Comparing `dallinger-9.8.2/README.rst` & `dallinger-9.9.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 group at https://groups.google.com/d/forum/dallinger.
 
 License
 -------
 
 The project is licensed under the MIT license.
 
-.. |Build Status| image:: https://github.com/dallinger/Dallinger/workflows/continuous-integration/badge.svg
-   :target: https://github.com/Dallinger/Dallinger/actions?query=workflow%3Acontinuous-integration
+.. |Build Status| image:: https://github.com/dallinger/Dallinger/actions/workflows/deploy.yml/badge.svg
+   :target: https://github.com/dallinger/Dallinger/actions/workflows/deploy.yml/badge.svg
 .. |Demos| image:: https://img.shields.io/badge/demos-11-edd172.svg
    :target: http://dallinger.readthedocs.io/en/latest/#demos
 .. |codecov| image:: https://codecov.io/gh/Dallinger/Dallinger/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/Dallinger/Dallinger
 .. |Code Climate| image:: https://codeclimate.com/github/Dallinger/Dallinger/badges/gpa.svg
    :target: https://codeclimate.com/github/Dallinger/Dallinger
 .. |License| image:: https://img.shields.io/badge/license-MIT-blue.svg
```

### Comparing `dallinger-9.8.2/constraints.txt` & `dallinger-9.9.0/constraints.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,86 +6,84 @@
 #
 
     # via -r constraints.in
 alabaster==0.7.13
     # via
     #   dallinger
     #   sphinx
-anyio==3.7.0
+anyio==3.7.1
     # via jupyter-server
 apscheduler==3.10.1
     # via dallinger
 argon2-cffi==21.3.0
-    # via
-    #   jupyter-server
-    #   nbclassic
-    #   notebook
+    # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-async-generator==1.10
-    # via trio
+async-lru==2.0.3
+    # via jupyterlab
 async-timeout==4.0.2
     # via redis
 attrs==23.1.0
     # via
     #   jsonschema
     #   outcome
+    #   referencing
     #   trio
 babel==2.12.1
-    # via sphinx
+    # via
+    #   jupyterlab-server
+    #   sphinx
 backcall==0.2.0
     # via ipython
 bcrypt==4.0.1
     # via paramiko
 beautifulsoup4==4.12.2
     # via nbconvert
-black==23.3.0
+black==23.7.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
 blinker==1.6.2
     # via flask
-boto3==1.26.158
+boto3==1.28.11
     # via dallinger
-botocore==1.29.158
+botocore==1.31.11
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
 bump2version==1.0.1
-    # via bumpversion
-bumpversion==0.6.0
     # via dallinger
 cached-property==1.5.2
     # via dallinger
 cachetools==5.3.1
     # via tox
-certifi==2023.5.7
+certifi==2023.7.22
     # via
     #   requests
     #   selenium
 cffi==1.15.1
     # via
     #   argon2-cffi-bindings
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 chardet==5.1.0
     # via tox
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via
     #   black
     #   dallinger
     #   flask
     #   pip-tools
     #   rq
 colorama==0.4.6
@@ -94,48 +92,48 @@
     # via ipykernel
 coverage==7.2.7
     # via
     #   coverage-pth
     #   dallinger
 coverage-pth==0.0.2
     # via dallinger
-cryptography==41.0.1
+cryptography==41.0.2
     # via
     #   paramiko
     #   pyopenssl
 debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via
     #   nbconvert
     #   odfpy
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
 docker==6.1.3
     # via dallinger
 docutils==0.18.1
     # via
     #   myst-parser
     #   sphinx
     #   sphinx-rtd-theme
 et-xmlfile==1.1.0
     # via openpyxl
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via
     #   anyio
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.11.1
+faker==19.2.0
     # via dallinger
-fastjsonschema==2.17.1
+fastjsonschema==2.18.0
     # via nbformat
 filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
@@ -154,64 +152,60 @@
     # via dallinger
 flask-wtf==1.1.1
     # via dallinger
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via dallinger
-gevent==22.10.2
+gevent==23.7.0
     # via
     #   dallinger
     #   flask-sockets
     #   gevent-websocket
 gevent-websocket==0.10.1
     # via flask-sockets
 greenlet==2.0.2
     # via
     #   dallinger
     #   gevent
     #   sqlalchemy
-gunicorn==20.1.0
+gunicorn==21.2.0
     # via dallinger
 h11==0.14.0
     # via wsproto
 heroku3==5.2.1
     # via dallinger
-identify==2.5.24
+identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
     #   trio
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.23.2
+ipykernel==6.25.0
     # via
     #   ipywidgets
     #   jupyter
     #   jupyter-console
-    #   nbclassic
-    #   notebook
+    #   jupyterlab
     #   qtconsole
 ipython==8.12.2
     # via
     #   dallinger
     #   ipykernel
     #   ipywidgets
     #   jupyter-console
 ipython-genutils==0.2.0
-    # via
-    #   nbclassic
-    #   notebook
-    #   qtconsole
-ipywidgets==8.0.6
+    # via qtconsole
+ipywidgets==8.0.7
     # via
     #   dallinger
     #   jupyter
 isoduration==20.11.0
     # via jsonschema
 isort==5.12.0
     # via dallinger
@@ -221,66 +215,79 @@
     #   flask-wtf
 jedi==0.18.2
     # via ipython
 jinja2==3.1.2
     # via
     #   flask
     #   jupyter-server
+    #   jupyterlab
+    #   jupyterlab-server
     #   myst-parser
-    #   nbclassic
     #   nbconvert
-    #   notebook
     #   sphinx
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
+json5==0.9.14
+    # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema==4.17.3
+jsonschema==4.18.4
     # via
     #   jupyter-events
+    #   jupyterlab-server
     #   nbformat
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 jupyter==1.0.0
     # via dallinger
-jupyter-client==8.2.0
+jupyter-client==8.3.0
     # via
     #   ipykernel
     #   jupyter-console
     #   jupyter-server
-    #   nbclassic
     #   nbclient
-    #   notebook
     #   qtconsole
 jupyter-console==6.6.3
     # via jupyter
 jupyter-core==5.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
-    #   nbclassic
+    #   jupyterlab
     #   nbclient
     #   nbconvert
     #   nbformat
-    #   notebook
     #   qtconsole
 jupyter-events==0.6.3
     # via jupyter-server
-jupyter-server==2.6.0
+jupyter-lsp==2.2.0
+    # via jupyterlab
+jupyter-server==2.7.0
     # via
     #   dallinger
-    #   nbclassic
+    #   jupyter-lsp
+    #   jupyterlab
+    #   jupyterlab-server
+    #   notebook
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
+jupyterlab==4.0.3
+    # via notebook
 jupyterlab-pygments==0.2.2
     # via nbconvert
-jupyterlab-widgets==3.0.7
+jupyterlab-server==2.24.0
+    # via
+    #   jupyterlab
+    #   notebook
+jupyterlab-widgets==3.0.8
     # via ipywidgets
 localconfig==1.1.3
     # via dallinger
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
@@ -300,49 +307,42 @@
     # via flake8
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==3.0.1
     # via nbconvert
-mock==5.0.2
+mock==5.1.0
     # via dallinger
 mypy-extensions==1.0.0
     # via black
 myst-parser==2.0.0
     # via dallinger
-nbclassic==1.0.0
-    # via notebook
 nbclient==0.8.0
     # via nbconvert
-nbconvert==7.6.0
+nbconvert==7.7.3
     # via
     #   jupyter
     #   jupyter-server
-    #   nbclassic
-    #   notebook
-nbformat==5.9.0
+nbformat==5.9.1
     # via
     #   jupyter-server
-    #   nbclassic
     #   nbclient
     #   nbconvert
-    #   notebook
 nest-asyncio==1.5.6
-    # via
-    #   ipykernel
-    #   nbclassic
-    #   notebook
+    # via ipykernel
 nodeenv==1.8.0
     # via pre-commit
-notebook==6.5.4
+notebook==7.0.0
     # via jupyter
 notebook-shim==0.2.3
-    # via nbclassic
-numpy==1.24.3
+    # via
+    #   jupyterlab
+    #   notebook
+numpy==1.24.4
     # via
     #   dallinger
     #   pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
@@ -351,25 +351,28 @@
 overrides==7.3.1
     # via jupyter-server
 packaging==23.1
     # via
     #   black
     #   build
     #   docker
+    #   gunicorn
     #   ipykernel
     #   jupyter-server
+    #   jupyterlab
+    #   jupyterlab-server
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   pytest-rerunfailures
     #   qtconsole
     #   qtpy
     #   sphinx
     #   tox
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   dallinger
     #   tablib
 pandocfilters==1.5.0
     # via nbconvert
 paramiko==3.2.0
     # via
@@ -381,34 +384,31 @@
     # via black
 pexpect==4.8.0
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
-pip-tools==6.13.0
+pip-tools==7.1.0
     # via dallinger
-platformdirs==3.7.0
+platformdirs==3.9.1
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
 pluggy==1.2.0
     # via
     #   pytest
     #   tox
 pre-commit==3.3.3
     # via dallinger
-prometheus-client==0.17.0
-    # via
-    #   jupyter-server
-    #   nbclassic
-    #   notebook
-prompt-toolkit==3.0.38
+prometheus-client==0.17.1
+    # via jupyter-server
+prompt-toolkit==3.0.39
     # via
     #   ipython
     #   jupyter-console
 psutil==5.9.5
     # via
     #   dallinger
     #   ipykernel
@@ -441,27 +441,25 @@
     #   sphinx
 pynacl==1.5.0
     # via paramiko
 pyopenssl==23.2.0
     # via dallinger
 pypandoc==1.11
     # via dallinger
-pyproject-api==1.5.2
+pyproject-api==1.5.3
     # via tox
 pyproject-hooks==1.0.0
     # via build
-pyrsistent==0.19.3
-    # via jsonschema
 pysocks==1.7.1
     # via urllib3
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   dallinger
     #   pytest-rerunfailures
-pytest-rerunfailures==11.1.2
+pytest-rerunfailures==12.0
     # via dallinger
 python-dateutil==2.8.2
     # via
     #   arrow
     #   botocore
     #   faker
     #   heroku3
@@ -469,62 +467,66 @@
     #   pandas
 python-json-logger==2.0.7
     # via jupyter-events
 pytz==2023.3
     # via
     #   apscheduler
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   jupyter-events
     #   myst-parser
     #   pre-commit
     #   tablib
 pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
-    #   nbclassic
-    #   notebook
     #   qtconsole
 qtconsole==5.4.3
     # via jupyter
 qtpy==2.3.1
     # via qtconsole
-redis==4.5.5
+redis==4.6.0
     # via
     #   dallinger
     #   rq
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   dallinger
     #   docker
     #   heroku3
+    #   jupyterlab-server
     #   sphinx
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 rq==1.15.1
     # via dallinger
 s3transfer==0.6.1
     # via boto3
 selenium==4.10.0
     # via dallinger
 send2trash==1.8.2
-    # via
-    #   jupyter-server
-    #   nbclassic
-    #   notebook
+    # via jupyter-server
 six==1.16.0
     # via
     #   apscheduler
     #   asttokens
     #   bleach
     #   dallinger
     #   python-dateutil
@@ -561,15 +563,15 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via dallinger
-sqlalchemy==1.4.48
+sqlalchemy==1.4.49
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 sqlalchemy-postgres-copy==0.5.0
     # via dallinger
 sshtunnel==0.4.0
     # via dallinger
@@ -583,115 +585,116 @@
     #   tablib
 tenacity==8.2.2
     # via dallinger
 terminado==0.17.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
-    #   nbclassic
-    #   notebook
 timeago==1.0.16
     # via dallinger
 tinycss2==1.2.1
     # via nbconvert
 tomli==2.0.1
     # via
     #   black
     #   build
+    #   jupyterlab
+    #   pip-tools
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
 tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-    #   nbclassic
+    #   jupyterlab
     #   notebook
     #   terminado
-tox==4.6.3
+tox==4.6.4
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-console
     #   jupyter-core
     #   jupyter-events
     #   jupyter-server
+    #   jupyterlab
     #   matplotlib-inline
-    #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
-    #   notebook
     #   qtconsole
-trio==0.22.0
+trio==0.22.2
     # via
     #   selenium
     #   trio-websocket
 trio-websocket==0.10.3
     # via selenium
+typing-extensions==4.7.1
+    # via async-lru
 tzdata==2023.3
     # via pandas
 tzlocal==5.0.1
     # via
     #   apscheduler
     #   dallinger
-ua-parser==0.16.1
+ua-parser==0.18.0
     # via
     #   dallinger
     #   user-agents
 uri-template==1.3.0
     # via jsonschema
 urllib3==1.26.16
     # via
     #   botocore
     #   docker
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-virtualenv==20.23.1
+virtualenv==20.24.2
     # via
     #   pre-commit
     #   tox
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.6.0
+websocket-client==1.6.1
     # via
     #   docker
     #   jupyter-server
 werkzeug==2.3.6
     # via
     #   flask
     #   flask-login
-wheel==0.40.0
+wheel==0.41.0
     # via pip-tools
-widgetsnbextension==4.0.7
+widgetsnbextension==4.0.8
     # via ipywidgets
 wsproto==1.2.0
     # via trio-websocket
 wtforms==3.0.1
     # via flask-wtf
 xlrd==2.0.1
     # via tablib
 xlwt==1.3.0
     # via tablib
-zope-event==4.6
+zope-event==5.0
     # via gevent
 zope-interface==6.0
     # via gevent
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `dallinger-9.8.2/dallinger/__init__.py` & `dallinger-9.9.0/dallinger/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/bots.py` & `dallinger-9.9.0/dallinger/bots.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/command_line/__init__.py` & `dallinger-9.9.0/dallinger/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/command_line/appdirs.py` & `dallinger-9.9.0/dallinger/command_line/appdirs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/command_line/config.py` & `dallinger-9.9.0/dallinger/command_line/config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/command_line/develop.py` & `dallinger-9.9.0/dallinger/command_line/develop.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/command_line/docker.py` & `dallinger-9.9.0/dallinger/command_line/docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/command_line/docker_ssh.py` & `dallinger-9.9.0/dallinger/command_line/docker_ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,21 @@
 from dallinger.command_line.utils import Output
 from dallinger.config import get_config
 from dallinger.data import bootstrap_db_from_zip, export_db_uri
 from dallinger.db import create_db_engine
 from dallinger.deployment import setup_experiment
 from dallinger.utils import abspath_from_egg, check_output
 
+# A couple of constants to colour console output
+RED = "\033[31m"
+END = "\033[0m"
+GREEN = "\033[32m"
+BLUE = "\033[34m"
+
+
 # Find an identifier for the current user to use as CREATOR of the experiment
 HOSTNAME = gethostname()
 try:
     USER = getuser()
 except KeyError:
     USER = "user"
 
@@ -204,26 +211,26 @@
         config.load()
         image_name = config.get("docker_image_name", None)
         if image_name:
             client = docker.from_env()
             try:
                 check_output(["docker", "manifest", "inspect", image_name])
                 print(f"Image {image_name} found on remote registry")
-                return f(*args, **kwargs)
+                return f(*args, **dict(kwargs, image_name=image_name))
             except CalledProcessError:
                 # The image is not on the registry. Check if it's available locally
                 # and push it if it is. If images.get succeeds it means the image is available locally
                 print(
                     f"Image {image_name} not found on remote registry. Trying to push"
                 )
                 raw_result = client.images.push(image_name)
                 # This is brittle, but it's an edge case not worth more effort
                 if not json.loads(raw_result.split("\r\n")[-2]).get("error"):
                     print(f"Image {image_name} pushed to remote registry")
-                    return f(*args, **kwargs)
+                    return f(*args, **dict(kwargs, image_name=image_name))
                 # The image is not available, neither locally nor on the remote registry
                 print(
                     f"Could not find image {image_name} specified in experiment config as `docker_image_name`"
                 )
                 raise click.Abort
         app_name = kwargs.get("app_name", None)
         _, tmp_dir = setup_experiment(
@@ -235,14 +242,30 @@
         build_image(tmp_dir, config.get("docker_image_base_name"), out=Output())
         image_name = push.callback(use_existing=True, app_name=app_name)
         return f(image_name, *args, **kwargs)
 
     return wrapper
 
 
+def validate_update(f):
+    @wraps(f)
+    def wrapper(*args, **kwargs):
+        if kwargs["update"] and not kwargs.get("app_name"):
+            raise click.UsageError(
+                "Please specify the id of the running app to update with --app-name"
+            )
+        if kwargs["update"] and kwargs.get("archive_path"):
+            raise click.UsageError(
+                "Can't update an existing experiment with an archive: --archive and --update are mutually exclusive"
+            )
+        return f(*args, **kwargs)
+
+    return wrapper
+
+
 @docker_ssh.command()
 @click.option(
     "--sandbox",
     "mode",
     flag_value="sandbox",
     help="Deploy to MTurk sandbox",
     default=True,
@@ -261,17 +284,25 @@
     "--archive",
     "-a",
     "archive_path",
     type=click.Path(exists=True),
     help="Path to a zip archive created with the `export` command to use as initial database state",
 )
 @click.option("--config", "-c", "config_options", nargs=2, multiple=True)
+@click.option(
+    "--update",
+    "-u",
+    flag_value="update",
+    default=False,
+    help="Update an existing experiment",
+)
+@validate_update
 @build_and_push_image
 def deploy(
-    image_name, mode, server, dns_host, app_name, config_options, archive_path
+    image_name, mode, server, dns_host, app_name, config_options, archive_path, update
 ):  # pragma: no cover
     """Deploy a dallinger experiment docker image to a server using ssh."""
     config = get_config()
     config.load()
     server_info = CONFIGURED_HOSTS[server]
     ssh_host = server_info["host"]
     ssh_user = server_info.get("user")
@@ -284,47 +315,88 @@
     email_addr = config.get("contact_email_on_error")
     if HAS_TLS:
         if "@" not in parseaddr(email_addr)[1]:
             print(f"Email address absent or invalid. Value {email_addr} found")
             print("Run `dallinger email-test` to verify your configuration")
             raise click.Abort
     tls = "tls internal" if not HAS_TLS else f"tls {email_addr}"
+
+    experiment_uuid = str(uuid4())
+    if app_name:
+        experiment_id = app_name
+    elif archive_path:
+        experiment_id = get_experiment_id_from_archive(archive_path)
+    else:
+        experiment_id = f"dlgr-{experiment_uuid[:8]}"
+
     if not dns_host:
         dns_host = get_dns_host(ssh_host)
+        print(
+            f"{RED}Using {dns_host} as hostname. This might cause problems:{END} some browsers"
+        )
+        print("might tell users this name is suspicious")
+        print("You can override this by creating a DNS A record pointing to")
+        print(
+            f"{GREEN}{ssh_host}{END} and using option --dns-host to deploy the experiment."
+        )
+        print(
+            f"{BLUE}For instance to use the name experiment1.my-custom-domain.example.com"
+        )
+        print(
+            f"you can pass options --app-name experiment1 --dns-host my-custom-domain.example.com{END}"
+        )
+    else:
+        # Check dns_host: make sure that {experiment_id}.{dns_host} resolves to the remote host
+        dns_ok = ipaddr_experiment = ipaddr_server = True
+        try:
+            ipaddr_server = gethostbyname_ex(f"{ssh_host}")[2][0]
+            ipaddr_experiment = gethostbyname_ex(f"{experiment_id}.{dns_host}")[2][0]
+        except Exception:
+            dns_ok = False
+        if not dns_ok or (ipaddr_experiment != ipaddr_server):
+            print(
+                f"The dns name for the experiment ({experiment_id}.{dns_host}) should resolve to {ipaddr_server}"
+            )
+            print(f"It currently resolves to {ipaddr_experiment}")
+            raise click.Abort
     executor = Executor(ssh_host, user=ssh_user, app=app_name)
     executor.run("mkdir -p ~/dallinger/caddy.d")
 
+    if not update:
+        print("Removing any pre-existing app with the same name.")
+        app_yml = f"~/dallinger/{app_name}/docker-compose.yml"
+        executor.run(
+            f"if [ -f {app_yml} ]; then docker compose -f {app_yml} down --remove-orphans; fi",
+            raise_=False,
+        )
+        print("Removing any pre-existing Redis volumes.")
+        remove_redis_volumes(app_name, executor)
+    else:
+        app_yml = f"~/dallinger/{app_name}/docker-compose.yml"
+        yml_file_exists = executor.run(f"ls -l {app_yml}", raise_=False)
+        if not yml_file_exists:
+            print(
+                f"{app_yml} file not found. App {app_name} does not exist on the server."
+            )
+            raise click.Abort
+
     sftp = get_sftp(ssh_host, user=ssh_user)
     sftp.putfo(BytesIO(DOCKER_COMPOSE_SERVER), "dallinger/docker-compose.yml")
     sftp.putfo(
         BytesIO(CADDYFILE.format(host=dns_host, tls=tls).encode()),
         "dallinger/Caddyfile",
     )
 
-    print("Removing any pre-existing app with the same name.")
-    app_yml = f"~/dallinger/{app_name}/docker-compose.yml"
-    executor.run(
-        f"if [ -f {app_yml} ]; then docker compose -f {app_yml} down --remove-orphans; fi",
-        raise_=False,
-    )
-
-    print("Removing any pre-existing Redis volumes.")
-    remove_redis_volumes(app_name, executor)
-
     print("Launching http and postgresql servers.")
     executor.run("docker compose -f ~/dallinger/docker-compose.yml up -d")
 
-    print("Starting experiment.")
-    experiment_uuid = str(uuid4())
-    if app_name:
-        experiment_id = app_name
-    elif archive_path:
-        experiment_id = get_experiment_id_from_archive(archive_path)
+    if not update:
+        print("Starting experiment.")
     else:
-        experiment_id = f"dlgr-{experiment_uuid[:8]}"
+        print("Restarting experiment.")
 
     dashboard_user = config.get("dashboard_user", "admin")
     dashboard_password = config.get("dashboard_password", secrets.token_urlsafe(8))
 
     cfg = config.as_dict()
     for key in "aws_access_key_id", "aws_secret_access_key":
         # AWS credentials are not included by default in to_dict() result
@@ -363,53 +435,70 @@
     )
     # We invoke the "ls" command in the context of the `web` container.
     # `docker compose` will honour `web`'s dependencies and block
     # until postgresql is ready. This way we can be sure we can start creating the database.
     executor.run(
         f"docker compose -f ~/dallinger/{experiment_id}/docker-compose.yml run --rm web ls"
     )
-    print("Cleaning up db/user")
-    executor.run(
-        rf"""docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c 'DROP DATABASE IF EXISTS "{experiment_id}";'"""
-    )
-    executor.run(
-        rf"""docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c 'DROP USER IF EXISTS "{experiment_id}"; '"""
-    )
-    print(f"Creating database {experiment_id}")
-    executor.run(
-        rf"""docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c 'CREATE DATABASE "{experiment_id}"'"""
-    )
-    create_user_script = f"""CREATE USER "{experiment_id}" with encrypted password '{postgresql_password}'"""
-    executor.run(
-        f"docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c {quote(create_user_script)}"
-    )
     grant_roles_script = (
         f'grant all privileges on database "{experiment_id}" to "{experiment_id}"'
     )
+    if not update:
+        print("Cleaning up db/user")
+        executor.run(
+            rf"""docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c 'DROP DATABASE IF EXISTS "{experiment_id}";'"""
+        )
+        executor.run(
+            rf"""docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c 'DROP USER IF EXISTS "{experiment_id}"; '"""
+        )
+        print(f"Creating database {experiment_id}")
+        executor.run(
+            rf"""docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c 'CREATE DATABASE "{experiment_id}"'"""
+        )
 
-    if archive_path is not None:
-        print(f"Loading database data from {archive_path}")
-        with remote_postgres(server_info, experiment_id) as db_uri:
-            engine = create_db_engine(db_uri)
-            bootstrap_db_from_zip(archive_path, engine)
-            with engine.connect() as conn:
-                conn.execute(grant_roles_script)
-                conn.execute(f'GRANT USAGE ON SCHEMA public TO "{experiment_id}"')
-                conn.execute(
-                    f'GRANT SELECT, INSERT, UPDATE, DELETE ON ALL TABLES IN SCHEMA PUBLIC TO "{experiment_id}"'
-                )
+        if archive_path is not None:
+            print(f"Loading database data from {archive_path}")
+            with remote_postgres(server_info, experiment_id) as db_uri:
+                engine = create_db_engine(db_uri)
+                bootstrap_db_from_zip(archive_path, engine)
+                with engine.connect() as conn:
+                    conn.execute(grant_roles_script)
+                    conn.execute(f'GRANT USAGE ON SCHEMA public TO "{experiment_id}"')
+                    conn.execute(
+                        f'GRANT SELECT, INSERT, UPDATE, DELETE ON ALL TABLES IN SCHEMA PUBLIC TO "{experiment_id}"'
+                    )
+
+    test_user_script = (
+        rf"""SELECT FROM pg_catalog.pg_roles WHERE rolname = '{experiment_id}'"""
+    )
+    query_user_result = executor.run(
+        f"docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c {quote(test_user_script)}",
+        raise_=False,
+    )
+    if "0 rows" in query_user_result:
+        # Create the user: it doesn't exist yet
+        create_user_script = f"""CREATE USER "{experiment_id}" with encrypted password '{postgresql_password}'"""
+        executor.run(
+            f"docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c {quote(create_user_script)}"
+        )
+    else:
+        # Change the password of the existing user
+        change_password_script = f"""ALTER USER "{experiment_id}" WITH ENCRYPTED PASSWORD '{postgresql_password}'"""
+        executor.run(
+            f"docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c {quote(change_password_script)}"
+        )
 
     executor.run(
         f"docker compose -f ~/dallinger/docker-compose.yml exec -T postgresql psql -U dallinger -c {quote(grant_roles_script)}"
     )
 
     executor.run(
         f"docker compose -f ~/dallinger/{experiment_id}/docker-compose.yml up -d"
     )
-    if archive_path is None:
+    if archive_path is None and not update:
         print(f"Experiment {experiment_id} started. Initializing database")
         executor.run(
             f"docker compose -f ~/dallinger/{experiment_id}/docker-compose.yml exec -T web dallinger-housekeeper initdb"
         )
         print("Database initialized")
 
     # We give caddy the alias for the service. If we scale up the service container caddy will
@@ -418,24 +507,27 @@
     sftp.putfo(
         BytesIO(caddy_conf.encode()),
         f"dallinger/caddy.d/{experiment_id}",
     )
     # Tell caddy we changed something in the configuration
     executor.reload_caddy()
 
-    print("Launching experiment")
-    response = get_retrying_http_client().post(
-        f"https://{experiment_id}.{dns_host}/launch", verify=HAS_TLS
-    )
-    print(response.json()["recruitment_msg"])
+    if update:
+        print("Skipping experiment launch logic because we are in update mode.")
+    else:
+        print("Launching experiment")
+        response = get_retrying_http_client().post(
+            f"https://{experiment_id}.{dns_host}/launch", verify=HAS_TLS
+        )
+        print(response.json()["recruitment_msg"])
 
     dashboard_user = cfg["ADMIN_USER"]
     dashboard_password = cfg["dashboard_password"]
     dashboard_link = f"https://{dashboard_user}:{dashboard_password}@{experiment_id}.{dns_host}/dashboard"
-    log_command = f"ssh {ssh_user}@{ssh_host} docker compose -f '~/dallinger/{experiment_id}/docker-compose.yml' logs -f"
+    log_command = f"ssh {ssh_user + '@' if ssh_user else ''}{ssh_host} docker compose -f '~/dallinger/{experiment_id}/docker-compose.yml' logs -f"
 
     deployment_infos = [
         f"Deployed Docker image name: {image_name}",
         "To display the logs for this experiment you can run:",
         log_command,
         f"You can now log in to the console at {dashboard_link} (user = {dashboard_user}, password = {dashboard_password})",
     ]
@@ -562,22 +654,31 @@
 @server_option
 def destroy(server, app):
     """Tear down an experiment run on a server you control via ssh."""
     server_info = CONFIGURED_HOSTS[server]
     ssh_host = server_info["host"]
     ssh_user = server_info.get("user")
     executor = Executor(ssh_host, user=ssh_user, app=app)
+
+    # Check if either the caddy config or the docker compose exist
+    # If not, the app is not deployed
+    caddy_config_exists = executor.run(
+        f"test -f ~/dallinger/caddy.d/{app} && echo Yes", raise_=False
+    )
+    docker_compose_exists = executor.run(
+        f"test -f ~/dallinger/{app}/docker-compose.yml && echo Yes", raise_=False
+    )
+    if not caddy_config_exists and not docker_compose_exists:
+        print(f"App {app} is not deployed")
+        raise click.Abort()
+
     # Remove the caddy configuration file and reload caddy config
-    try:
-        executor.run(f"ls ~/dallinger/caddy.d/{app}")
-    except ExecuteException:
-        print(f"App {app} not found on server {server}")
-        raise click.Abort
-    executor.run(f"rm ~/dallinger/caddy.d/{app}")
+    executor.run(f"rm -f ~/dallinger/caddy.d/{app}")
     executor.reload_caddy()
+
     executor.run(
         f"docker compose -f ~/dallinger/{app}/docker-compose.yml down", raise_=False
     )
     executor.run(f"rm -rf ~/dallinger/{app}/")
     print(f"App {app} removed")
```

### Comparing `dallinger-9.8.2/dallinger/command_line/utils.py` & `dallinger-9.9.0/dallinger/command_line/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/config.py` & `dallinger-9.9.0/dallinger/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     ("heroku_team", six.text_type, ["team"]),
     ("host", six.text_type, []),
     ("id", six.text_type, []),
     ("infrastructure_debug_details", six.text_type, [], False),
     ("keywords", six.text_type, []),
     ("language", six.text_type, []),
     ("lifetime", int, []),
+    ("lock_table_when_creating_participant", bool, []),
     ("logfile", six.text_type, []),
     ("loglevel", int, []),
     ("mode", six.text_type, []),
     ("mturk_qualification_blocklist", six.text_type, ["qualification_blacklist"]),
     ("mturk_qualification_requirements", six.text_type, [], False, [is_valid_json]),
     ("num_dynos_web", int, []),
     ("num_dynos_worker", int, []),
```

### Comparing `dallinger-9.8.2/dallinger/data.py` & `dallinger-9.9.0/dallinger/data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/db.py` & `dallinger-9.9.0/dallinger/db.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/default_configs/global_config_defaults.txt` & `dallinger-9.9.0/dallinger/default_configs/global_config_defaults.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 dallinger_email_address = dallinger@mailinator.com
 
 [Experiment]
 replay = False
 mode = debug
 enable_global_experiment_registry = False
 language = en
+lock_table_when_creating_participant = True
 
 [Recruiter]
 activate_recruiter_on_start = True
 auto_recruit = False
 assign_qualifications = False
 us_only = False
 disable_when_duration_exceeded = True
```

### Comparing `dallinger-9.8.2/dallinger/deployment.py` & `dallinger-9.9.0/dallinger/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/dev_server/app.py` & `dallinger-9.9.0/dallinger/dev_server/app.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/docker/deployment.py` & `dallinger-9.9.0/dallinger/docker/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/docker/docker-compose.yml.j2` & `dallinger-9.9.0/dallinger/docker/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2` & `dallinger-9.9.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/docker/ssh_templates/docker-compose-server.yml` & `dallinger-9.9.0/dallinger/docker/ssh_templates/docker-compose-server.yml`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/docker/tools.py` & `dallinger-9.9.0/dallinger/docker/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/docker/wheel_filename.py` & `dallinger-9.9.0/dallinger/docker/wheel_filename.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/experiment.py` & `dallinger-9.9.0/dallinger/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,14 +552,73 @@
         that they paid attention. This check will run once the *participant*
         completes the experiment. By default performs no checks and returns
         True. See also :func:`~dallinger.experiments.Experiment.data_check`.
 
         """
         return True
 
+    def on_assignment_submitted_to_recruiter(self, participant, event):
+        """Working title. Called when assignment has been submitted
+        to the recruitment platform (may be Dallinger itself) by the
+        participant.
+
+        :param participant (Participant): the ``Participant`` who has
+        submitted a HIT via their recruiter
+        :param event: (dict): Info about the triggering event
+        """
+        eligible_statuses = ("working", "overrecruited", "returned", "abandoned")
+        if participant.status not in eligible_statuses:
+            return
+
+        config = get_config()
+        min_real_bonus = 0.01
+
+        participant.status = "submitted"
+        participant.end_time = event["timestamp"]
+        participant.base_pay = config.get("base_payment")
+        participant.recruiter.approve_hit(participant.assignment_id)
+
+        # Data Check
+        if not self.data_check(participant=participant):
+            participant.status = "bad_data"
+            self.data_check_failed(participant=participant)
+            # NB: if MultiRecruiter is in use, this may not be the same recruiter as
+            # provided the participant we're replacing
+            self.recruiter.recruit(n=1)
+
+            # NOTE EARLY RETURN!!
+            return
+
+        # If they pass the data check, we might pay a bonus
+        bonus = self.bonus(participant=participant)
+        participant.bonus = bonus
+        if bonus >= min_real_bonus:
+            self.log("Bonus = {}: paying bonus".format(bonus))
+            participant.recruiter.reward_bonus(
+                participant,
+                bonus,
+                self.bonus_reason(),
+            )
+        else:
+            self.log("Bonus = {}: NOT paying bonus".format(bonus))
+
+        # Attention Check
+        if self.attention_check(participant=participant):
+            self.log("Attention checks passed.")
+            participant.status = "approved"
+            self.submission_successful(participant=participant)
+            self.recruit()
+        else:
+            self.log("Attention checks failed.")
+            participant.status = "did_not_attend"
+            self.attention_check_failed(participant=participant)
+            # NB: if MultiRecruiter is in use, this may not be the same recruiter
+            # that provided the participant we're replacing:
+            self.recruiter.recruit(n=1)
+
     def participant_task_completed(self, participant):
         """Called when an experiment task is finished and submitted, and prior
         to data and attendance checks.
 
         Assigns the qualifications to the Participant, via their recruiter.
         These will include one Qualification for the experiment
         ID, and others for the configured group_name, if it's been set.
@@ -594,15 +653,14 @@
     def recruit(self):
         """Recruit participants to the experiment as needed.
 
         This method runs whenever a participant successfully completes the
         experiment (participants who fail to finish successfully are
         automatically replaced). By default it recruits 1 participant at a time
         until all networks are full.
-
         """
         if not self.networks(full=False):
             self.log("All networks full: closing recruitment", "-----")
             self.recruiter.close_recruitment()
 
     def log(self, text, key="?????", force=False):
         """Print a string to the logs."""
@@ -618,15 +676,14 @@
         self.log("Status summary: {}".format(str(sorted_counts)))
         return sorted_counts
 
     def save(self, *objects):
         """Add all the objects to the session and commit them.
 
         This only needs to be done for networks and participants.
-
         """
         if len(objects) > 0:
             self.session.add_all(objects)
         self.session.commit()
 
     def node_post_request(self, participant, node):
         """Run when a request to make a node is complete."""
```

### Comparing `dallinger-9.8.2/dallinger/experiment_server/dashboard.py` & `dallinger-9.9.0/dallinger/experiment_server/dashboard.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/experiment_server/experiment_server.py` & `dallinger-9.9.0/dallinger/experiment_server/experiment_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -787,20 +787,30 @@
 def create_participant(worker_id, hit_id, assignment_id, mode, entry_information=None):
     """Create a participant.
 
     This route is hit early on. Any nodes the participant creates will be
     defined in reference to the participant object. You must specify the
     worker_id, hit_id, assignment_id, and mode in the url.
     """
-    # Lock the table, triggering multiple simultaneous accesses to fail
-    try:
-        session.connection().execute("LOCK TABLE participant IN EXCLUSIVE MODE NOWAIT")
-    except exc.OperationalError as e:
-        e.orig = TransactionRollbackError()
-        raise e
+    config = get_config()
+    if not config.ready:
+        config.load()
+
+    if config.get("lock_table_when_creating_participant"):
+        # Historically we have locked the participant table when creating participants
+        # to avoid database inconsistency problems. However some experimenters have experienced
+        # some deadlocking problems associated with this locking, so we have made
+        # it an opt-out behavior.
+        try:
+            session.connection().execute(
+                "LOCK TABLE participant IN EXCLUSIVE MODE NOWAIT"
+            )
+        except exc.OperationalError as e:
+            e.orig = TransactionRollbackError()
+            raise e
 
     missing = [p for p in (worker_id, hit_id, assignment_id) if p == "undefined"]
     if missing:
         msg = "/participant POST: required values were 'undefined'"
         return error_response(error_type=msg, status=403)
 
     fingerprint_hash = request.args.get("fingerprint_hash") or request.form.get(
@@ -1707,15 +1717,16 @@
     # the experiment can request qualification assignment before the
     # worker completes the HIT when using a recruiter like MTurk, where
     # execution of the `worker_events.AssignmentSubmitted` command is
     # deferred until they've submitted the HIT on the MTurk platform.
     exp = Experiment(session)
     exp.participant_task_completed(participant)
 
-    event_type = participant.recruiter.submitted_event()
+    # Does the recruiter want us to execute some command on worker completion?
+    event_type = participant.recruiter.on_completion_event()
 
     if event_type is None:
         return
 
     # Currently we execute this function synchronously, regardless of the
     # event type:
     worker_function(
```

### Comparing `dallinger-9.8.2/dallinger/experiment_server/gunicorn.py` & `dallinger-9.9.0/dallinger/experiment_server/gunicorn.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/experiment_server/replay.py` & `dallinger-9.9.0/dallinger/experiment_server/replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/experiment_server/sockets.py` & `dallinger-9.9.0/dallinger/experiment_server/sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/experiment_server/utils.py` & `dallinger-9.9.0/dallinger/experiment_server/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/experiment_server/worker_events.py` & `dallinger-9.9.0/dallinger/experiment_server/worker_events.py`

 * *Files 16% similar despite different names*

```diff
@@ -124,23 +124,22 @@
                 "Warning: No participants associated with this "
                 "assignment_id. Notification will not be processed.",
                 key,
             )
             return None
 
     elif participant_id is not None:
+        # XXX Why is this not a Participant.get()?
         participant = models.Participant.query.filter_by(id=participant_id).all()[0]
     else:
         raise ValueError(
             "Error: worker_function needs either an assignment_id or a "
             "participant_id, they cannot both be None"
         )
 
-    participant_id = participant.id
-
     runner = runner_cls(
         participant, assignment_id, exp, db.session, _config(), datetime.now()
     )
     runner()
     db.session.commit()
 
 
@@ -167,14 +166,23 @@
         self.participant = participant
         self.assignment_id = assignment_id
         self.experiment = experiment
         self.session = session
         self.config = config
         self.now = now
 
+    @property
+    def data(self):
+        return {
+            "event_type": self.__class__.__name__,
+            "participant_id": self.participant.id,
+            "assignment_id": self.assignment_id,
+            "timestamp": self.now,
+        }
+
     def commit(self):
         self.session.commit()
 
     def log(self, message):
         self.experiment.log(message, self.key)
 
     def update_participant_end_time(self):
@@ -199,88 +207,19 @@
         if self.participant.status == "working":
             self.update_participant_end_time()
             self.participant.status = "returned"
             self.experiment.assignment_returned(participant=self.participant)
 
 
 class AssignmentSubmitted(WorkerEvent):
-    min_real_bonus = 0.01
-
     def __call__(self):
-        if not self.is_eligible(self.participant):
-            return
-
-        self.update_participant_end_time()
-        self.participant.status = "submitted"
-        self.commit()
-
-        self.approve_assignment()
-
-        if not self.data_is_ok():
-            self.fail_data_check()
-            self.experiment.recruiter.recruit(n=1)
-
-            return
-
-        # If their data is ok, pay them a bonus.
-        # Note that the bonus is paid before the attention check.
-        bonus = self.experiment.bonus(participant=self.participant)
-        self.participant.bonus = bonus
-        if bonus >= self.min_real_bonus:
-            self.award_bonus(bonus)
-        else:
-            self.log("Bonus = {}: NOT paying bonus".format(bonus))
-
-        if self.did_attend():
-            self.approve_submission()
-            self.experiment.recruit()
-        else:
-            self.fail_submission()
-            self.experiment.recruiter.recruit(n=1)
-
-    def is_eligible(self, particpant):
-        eligible_statuses = ("working", "overrecruited", "returned", "abandoned")
-        return particpant.status in eligible_statuses
-
-    def data_is_ok(self):
-        """Run a check on our participant's data"""
-        return self.experiment.data_check(participant=self.participant)
-
-    def did_attend(self):
-        return self.experiment.attention_check(participant=self.participant)
-
-    def approve_assignment(self):
-        self.participant.recruiter.approve_hit(self.assignment_id)
-        self.participant.base_pay = self.config.get("base_payment")
-
-    def award_bonus(self, bonus):
-        self.log("Bonus = {}: paying bonus".format(bonus))
-        self.participant.recruiter.reward_bonus(
-            self.participant,
-            bonus,
-            self.experiment.bonus_reason(),
+        self.experiment.on_assignment_submitted_to_recruiter(
+            participant=self.participant, event=self.data
         )
 
-    def fail_data_check(self):
-        self.participant.status = "bad_data"
-        self.experiment.data_check_failed(participant=self.participant)
-        self.commit()
-
-    def approve_submission(self):
-        self.log("All checks passed.")
-        self.participant.status = "approved"
-        self.experiment.submission_successful(participant=self.participant)
-        self.commit()
-
-    def fail_submission(self):
-        self.log("Attention check failed.")
-        self.participant.status = "did_not_attend"
-        self.experiment.attention_check_failed(participant=self.participant)
-        self.commit()
-
 
 class BotAssignmentSubmitted(WorkerEvent):
     def __call__(self):
         self.log("Received bot submission.")
         self.update_participant_end_time()
 
         # No checks for bot submission
```

### Comparing `dallinger-9.8.2/dallinger/experiments/__init__.py` & `dallinger-9.9.0/dallinger/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/css/bootstrap.min.css` & `dallinger-9.9.0/dallinger/frontend/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/css/dashboard.css` & `dallinger-9.9.0/dallinger/frontend/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/bootstrap.min.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/clipboard.min.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/dallinger2.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/dallinger2.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/dallinger2.test.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/dallinger2.test.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/jquery-3.6.0.min.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/network-monitor.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/network-monitor.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/popper.min.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/popper.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/reconnecting-websocket.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/reconnecting-websocket.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/require.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/require.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/reqwest.min.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/reqwest.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/spin.min.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/spin.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/store+json2.min.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/store+json2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/tracker.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/tracker.js.map` & `dallinger-9.9.0/dallinger/frontend/static/scripts/tracker.js.map`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/load-tracker.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/tracking/load-tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js` & `dallinger-9.9.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css` & `dallinger-9.9.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js` & `dallinger-9.9.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/base/ad.html` & `dallinger-9.9.0/dallinger/frontend/templates/base/ad.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/base/consent.html` & `dallinger-9.9.0/dallinger/frontend/templates/base/consent.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/base/dashboard.html` & `dallinger-9.9.0/dallinger/frontend/templates/base/dashboard.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/base/layout.html` & `dallinger-9.9.0/dallinger/frontend/templates/base/layout.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/base/questionnaire.html` & `dallinger-9.9.0/dallinger/frontend/templates/base/questionnaire.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/dashboard_database.html` & `dallinger-9.9.0/dallinger/frontend/templates/dashboard_database.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/dashboard_develop.html` & `dallinger-9.9.0/dallinger/frontend/templates/dashboard_develop.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/dashboard_home.html` & `dallinger-9.9.0/dallinger/frontend/templates/dashboard_home.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/dashboard_lifecycle.html` & `dallinger-9.9.0/dallinger/frontend/templates/dashboard_lifecycle.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/dashboard_monitor.html` & `dallinger-9.9.0/dallinger/frontend/templates/dashboard_monitor.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/dashboard_mturk.html` & `dallinger-9.9.0/dallinger/frontend/templates/dashboard_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/error-complete.html` & `dallinger-9.9.0/dallinger/frontend/templates/error-complete.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/error.html` & `dallinger-9.9.0/dallinger/frontend/templates/error.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter.html` & `dallinger-9.9.0/dallinger/frontend/templates/exit_recruiter.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter_mturk.html` & `dallinger-9.9.0/dallinger/frontend/templates/exit_recruiter_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/exit_recruiter_prolific.html` & `dallinger-9.9.0/dallinger/frontend/templates/exit_recruiter_prolific.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/login.html` & `dallinger-9.9.0/dallinger/frontend/templates/login.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/frontend/templates/waiting.html` & `dallinger-9.9.0/dallinger/frontend/templates/waiting.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/heroku/clock.py` & `dallinger-9.9.0/dallinger/heroku/clock.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/heroku/rq_gevent_worker.py` & `dallinger-9.9.0/dallinger/heroku/rq_gevent_worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/heroku/tools.py` & `dallinger-9.9.0/dallinger/heroku/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/jupyter.py` & `dallinger-9.9.0/dallinger/jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/models.py` & `dallinger-9.9.0/dallinger/models.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/mturk.py` & `dallinger-9.9.0/dallinger/mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/networks.py` & `dallinger-9.9.0/dallinger/networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/nodes.py` & `dallinger-9.9.0/dallinger/nodes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/notifications.py` & `dallinger-9.9.0/dallinger/notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/processes.py` & `dallinger-9.9.0/dallinger/processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/prolific.py` & `dallinger-9.9.0/dallinger/prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/pytest_dallinger.py` & `dallinger-9.9.0/dallinger/pytest_dallinger.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,15 @@
         "heroku_auth_token": "heroku secret",
         "heroku_python_version": "3.9.2",
         "heroku_team": "",
         "host": "0.0.0.0",
         "id": "TEST_EXPERIMENT_UID",  # This is a significant value; change with caution.
         "keywords": "kw1, kw2, kw3",
         "lifetime": 1,
+        "lock_table_when_creating_participant": True,
         "logfile": "-",
         "loglevel": 0,
         "mode": "debug",
         "num_dynos_web": 1,
         "num_dynos_worker": 1,
         "organization_name": "Monsters University",
         "sentry": True,
```

### Comparing `dallinger-9.8.2/dallinger/recruiters.py` & `dallinger-9.9.0/dallinger/recruiters.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,18 +148,19 @@
 
         To reject a questionnaire, this method returns an error string.
 
         By default, they are accepted, so we return None.
         """
         return None
 
-    def submitted_event(self):
-        """Return the appropriate event type to trigger when
-        an assignment is submitted. If no event should be processed,
-        return None.
+    def on_completion_event(self):
+        """Return the name of the appropriate WorkerEvent command to run
+        when a participant completes an experiment.
+
+        If no event should be processed, return None.
         """
         return "AssignmentSubmitted"
 
     def load_service(self, sandbox):
         """Load the appropriate service for this recruiter."""
         raise NotImplementedError
 
@@ -438,15 +439,15 @@
                 study_id=self.current_study_id,
                 worker_id=participant.worker_id,
                 amount=amount,
             )
         except ProlificServiceException as ex:
             logger.exception(str(ex))
 
-    def submitted_event(self):
+    def on_completion_event(self):
         """We cannot perform post-submission actions (approval, bonus payment)
         until after the participant has submitted their study via the Prolific
         UI, which we redirect them to from the exit page. This means that we
         can't do anything when the questionnaire is submitted, so we return None
         to signal this.
         """
         return None
@@ -1198,15 +1199,15 @@
         """
         if participant.status != "working":
             return (
                 "This participant has already sumbitted their HIT "
                 "on MTurk and can no longer submit the questionnaire"
             )
 
-    def submitted_event(self):
+    def on_completion_event(self):
         """MTurk will send its own notification when the worker
         completes the HIT on that service.
         """
         return None
 
     def reward_bonus(self, participant, amount, reason):
         """Reward the Turker for a specified assignment with a bonus."""
@@ -1522,15 +1523,15 @@
             participant.status = "rejected"
             session.commit()
 
     def reward_bonus(self, participant, amount, reason):
         """Logging only. These are bots."""
         logger.info("Bots don't get bonuses. Sorry, bots.")
 
-    def submitted_event(self):
+    def on_completion_event(self):
         return "BotAssignmentSubmitted"
 
     def _get_bot_factory(self):
         # Must be imported at run-time
         from dallinger_experiment.experiment import Bot
 
         return Bot
```

### Comparing `dallinger-9.8.2/dallinger/redis_utils.py` & `dallinger-9.9.0/dallinger/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/registration.py` & `dallinger-9.9.0/dallinger/registration.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/transformations.py` & `dallinger-9.9.0/dallinger/transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger/utils.py` & `dallinger-9.9.0/dallinger/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 from flask import request
 
 from dallinger import db
 from dallinger.compat import is_command
 from dallinger.config import get_config
 from dallinger.version import __version__
 
+try:
+    from pip._vendor import pkg_resources
+except ImportError:
+    pkg_resources = None
+
 fake = Faker()
 
 
 def get_base_url():
     """Returns the base url for the experiment.
     Looks into environment variable HOST first, then in the
     experiment config.
@@ -395,17 +400,20 @@
                 if line[:3] != "-e " and line[0].strip() not in ["#", ""]
             ]
     except (OSError, IOError):
         dependencies = []
 
     for dep in dependencies:
         if find_spec(dep) is None:
-            raise ValueError(
-                f"Please install the '{dep}' package to run this experiment."
-            )
+            try:
+                pkg_resources.get_distribution(dep)
+            except (pkg_resources.DistributionNotFound, AttributeError):
+                raise ValueError(
+                    f"Please install the '{dep}' package to run this experiment."
+                )
 
 
 def develop_target_path(config):
     """Extract the target `dallinger develop` working directory from
     configuration, and return it as a Path.
     """
     develop_path_string = config.get("dallinger_develop_directory", None)
@@ -591,15 +599,14 @@
         compile_info = f"dallinger generate-constraints\n#\n# Compiled from a requirement.txt file with md5sum: {requirements_path_hash}"
         with TemporaryDirectory() as tmpdirname:
             tmpfile = Path(tmpdirname) / "requirements.txt"
             tmpfile.write_text(Path("requirements.txt").read_text() + "\n-c " + url)
             check_output(
                 [
                     "pip-compile",
-                    "--resolver=backtracking",
                     "-v",
                     str(tmpfile),
                     "-o",
                     "constraints.txt",
                 ],
                 env=dict(
                     os.environ,
```

### Comparing `dallinger-9.8.2/dallinger.egg-info/PKG-INFO` & `dallinger-9.9.0/dallinger.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.8.2
+Version: 9.9.0
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Provides-Extra: data
 Provides-Extra: dev
 Provides-Extra: docker
 License-File: LICENSE
 
 Dallinger
 =======
-[![Build Status](https://github.com/dallinger/Dallinger/workflows/continuous-integration/badge.svg)](https://github.com/Dallinger/Dallinger/actions?query=workflow%3Acontinuous-integration)
+[![Build Status](https://github.com/dallinger/Dallinger/actions/workflows/deploy.yml/badge.svg)](https://github.com/dallinger/Dallinger/actions/workflows/deploy.yml/badge.svg)
 [![Demos](https://img.shields.io/badge/demos-11-edd172.svg)](http://dallinger.readthedocs.io/en/latest/#demos)
 [![codecov](https://codecov.io/gh/Dallinger/Dallinger/branch/master/graph/badge.svg)](https://codecov.io/gh/Dallinger/Dallinger)
 [![Code Climate](https://codeclimate.com/github/Dallinger/Dallinger/badges/gpa.svg)](https://codeclimate.com/github/Dallinger/Dallinger)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://en.wikipedia.org/wiki/MIT_License)
 
 <img src="https://raw.githubusercontent.com/Dallinger/Dallinger/master/incubator.png" width="125" alt="Dallinger's incubator">
```

### Comparing `dallinger-9.8.2/dallinger.egg-info/SOURCES.txt` & `dallinger-9.9.0/dallinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dallinger.egg-info/requires.txt` & `dallinger-9.9.0/dallinger.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 [data]
 pandas
 tablib[all]
 
 [dev]
 alabaster
 black
-bumpversion
+bump2version
 coverage
 coverage_pth
 flake8
 isort
 mock
 myst-parser
 pre-commit
```

### Comparing `dallinger-9.8.2/dallinger_scripts/worker.py` & `dallinger-9.9.0/dallinger_scripts/worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/dev-requirements.txt` & `dallinger-9.9.0/dev-requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,86 +6,84 @@
 #
 
     # via -r dev-requirements.in
 alabaster==0.7.13
     # via
     #   dallinger
     #   sphinx
-anyio==3.7.0
+anyio==3.7.1
     # via jupyter-server
 apscheduler==3.10.1
     # via dallinger
 argon2-cffi==21.3.0
-    # via
-    #   jupyter-server
-    #   nbclassic
-    #   notebook
+    # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-async-generator==1.10
-    # via trio
+async-lru==2.0.3
+    # via jupyterlab
 async-timeout==4.0.2
     # via redis
 attrs==23.1.0
     # via
     #   jsonschema
     #   outcome
+    #   referencing
     #   trio
 babel==2.12.1
-    # via sphinx
+    # via
+    #   jupyterlab-server
+    #   sphinx
 backcall==0.2.0
     # via ipython
 bcrypt==4.0.1
     # via paramiko
 beautifulsoup4==4.12.2
     # via nbconvert
-black==23.3.0
+black==23.7.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
 blinker==1.6.2
     # via flask
-boto3==1.26.158
+boto3==1.28.11
     # via dallinger
-botocore==1.29.158
+botocore==1.31.11
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
 bump2version==1.0.1
-    # via bumpversion
-bumpversion==0.6.0
     # via dallinger
 cached-property==1.5.2
     # via dallinger
 cachetools==5.3.1
     # via tox
-certifi==2023.5.7
+certifi==2023.7.22
     # via
     #   requests
     #   selenium
 cffi==1.15.1
     # via
     #   argon2-cffi-bindings
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 chardet==5.1.0
     # via tox
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via
     #   black
     #   dallinger
     #   flask
     #   pip-tools
     #   rq
 colorama==0.4.6
@@ -94,48 +92,48 @@
     # via ipykernel
 coverage==7.2.7
     # via
     #   coverage-pth
     #   dallinger
 coverage-pth==0.0.2
     # via dallinger
-cryptography==41.0.1
+cryptography==41.0.2
     # via
     #   paramiko
     #   pyopenssl
 debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via
     #   nbconvert
     #   odfpy
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
 docker==6.1.3
     # via dallinger
 docutils==0.18.1
     # via
     #   myst-parser
     #   sphinx
     #   sphinx-rtd-theme
 et-xmlfile==1.1.0
     # via openpyxl
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via
     #   anyio
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.11.1
+faker==19.2.0
     # via dallinger
-fastjsonschema==2.17.1
+fastjsonschema==2.18.0
     # via nbformat
 filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
@@ -154,64 +152,60 @@
     # via dallinger
 flask-wtf==1.1.1
     # via dallinger
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via dallinger
-gevent==22.10.2
+gevent==23.7.0
     # via
     #   dallinger
     #   flask-sockets
     #   gevent-websocket
 gevent-websocket==0.10.1
     # via flask-sockets
 greenlet==2.0.2
     # via
     #   dallinger
     #   gevent
     #   sqlalchemy
-gunicorn==20.1.0
+gunicorn==21.2.0
     # via dallinger
 h11==0.14.0
     # via wsproto
 heroku3==5.2.1
     # via dallinger
-identify==2.5.24
+identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
     #   trio
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.23.2
+ipykernel==6.25.0
     # via
     #   ipywidgets
     #   jupyter
     #   jupyter-console
-    #   nbclassic
-    #   notebook
+    #   jupyterlab
     #   qtconsole
 ipython==8.12.2
     # via
     #   dallinger
     #   ipykernel
     #   ipywidgets
     #   jupyter-console
 ipython-genutils==0.2.0
-    # via
-    #   nbclassic
-    #   notebook
-    #   qtconsole
-ipywidgets==8.0.6
+    # via qtconsole
+ipywidgets==8.0.7
     # via
     #   dallinger
     #   jupyter
 isoduration==20.11.0
     # via jsonschema
 isort==5.12.0
     # via dallinger
@@ -221,66 +215,79 @@
     #   flask-wtf
 jedi==0.18.2
     # via ipython
 jinja2==3.1.2
     # via
     #   flask
     #   jupyter-server
+    #   jupyterlab
+    #   jupyterlab-server
     #   myst-parser
-    #   nbclassic
     #   nbconvert
-    #   notebook
     #   sphinx
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
+json5==0.9.14
+    # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema==4.17.3
+jsonschema==4.18.4
     # via
     #   jupyter-events
+    #   jupyterlab-server
     #   nbformat
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 jupyter==1.0.0
     # via dallinger
-jupyter-client==8.2.0
+jupyter-client==8.3.0
     # via
     #   ipykernel
     #   jupyter-console
     #   jupyter-server
-    #   nbclassic
     #   nbclient
-    #   notebook
     #   qtconsole
 jupyter-console==6.6.3
     # via jupyter
 jupyter-core==5.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
-    #   nbclassic
+    #   jupyterlab
     #   nbclient
     #   nbconvert
     #   nbformat
-    #   notebook
     #   qtconsole
 jupyter-events==0.6.3
     # via jupyter-server
-jupyter-server==2.6.0
+jupyter-lsp==2.2.0
+    # via jupyterlab
+jupyter-server==2.7.0
     # via
     #   dallinger
-    #   nbclassic
+    #   jupyter-lsp
+    #   jupyterlab
+    #   jupyterlab-server
+    #   notebook
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
+jupyterlab==4.0.3
+    # via notebook
 jupyterlab-pygments==0.2.2
     # via nbconvert
-jupyterlab-widgets==3.0.7
+jupyterlab-server==2.24.0
+    # via
+    #   jupyterlab
+    #   notebook
+jupyterlab-widgets==3.0.8
     # via ipywidgets
 localconfig==1.1.3
     # via dallinger
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
@@ -300,49 +307,42 @@
     # via flake8
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==3.0.1
     # via nbconvert
-mock==5.0.2
+mock==5.1.0
     # via dallinger
 mypy-extensions==1.0.0
     # via black
 myst-parser==2.0.0
     # via dallinger
-nbclassic==1.0.0
-    # via notebook
 nbclient==0.8.0
     # via nbconvert
-nbconvert==7.6.0
+nbconvert==7.7.3
     # via
     #   jupyter
     #   jupyter-server
-    #   nbclassic
-    #   notebook
-nbformat==5.9.0
+nbformat==5.9.1
     # via
     #   jupyter-server
-    #   nbclassic
     #   nbclient
     #   nbconvert
-    #   notebook
 nest-asyncio==1.5.6
-    # via
-    #   ipykernel
-    #   nbclassic
-    #   notebook
+    # via ipykernel
 nodeenv==1.8.0
     # via pre-commit
-notebook==6.5.4
+notebook==7.0.0
     # via jupyter
 notebook-shim==0.2.3
-    # via nbclassic
-numpy==1.24.3
+    # via
+    #   jupyterlab
+    #   notebook
+numpy==1.24.4
     # via
     #   dallinger
     #   pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
@@ -351,25 +351,28 @@
 overrides==7.3.1
     # via jupyter-server
 packaging==23.1
     # via
     #   black
     #   build
     #   docker
+    #   gunicorn
     #   ipykernel
     #   jupyter-server
+    #   jupyterlab
+    #   jupyterlab-server
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   pytest-rerunfailures
     #   qtconsole
     #   qtpy
     #   sphinx
     #   tox
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   dallinger
     #   tablib
 pandocfilters==1.5.0
     # via nbconvert
 paramiko==3.2.0
     # via
@@ -381,34 +384,31 @@
     # via black
 pexpect==4.8.0
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
-pip-tools==6.13.0
+pip-tools==7.1.0
     # via dallinger
-platformdirs==3.7.0
+platformdirs==3.9.1
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
 pluggy==1.2.0
     # via
     #   pytest
     #   tox
 pre-commit==3.3.3
     # via dallinger
-prometheus-client==0.17.0
-    # via
-    #   jupyter-server
-    #   nbclassic
-    #   notebook
-prompt-toolkit==3.0.38
+prometheus-client==0.17.1
+    # via jupyter-server
+prompt-toolkit==3.0.39
     # via
     #   ipython
     #   jupyter-console
 psutil==5.9.5
     # via
     #   dallinger
     #   ipykernel
@@ -441,27 +441,25 @@
     #   sphinx
 pynacl==1.5.0
     # via paramiko
 pyopenssl==23.2.0
     # via dallinger
 pypandoc==1.11
     # via dallinger
-pyproject-api==1.5.2
+pyproject-api==1.5.3
     # via tox
 pyproject-hooks==1.0.0
     # via build
-pyrsistent==0.19.3
-    # via jsonschema
 pysocks==1.7.1
     # via urllib3
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   dallinger
     #   pytest-rerunfailures
-pytest-rerunfailures==11.1.2
+pytest-rerunfailures==12.0
     # via dallinger
 python-dateutil==2.8.2
     # via
     #   arrow
     #   botocore
     #   faker
     #   heroku3
@@ -469,62 +467,66 @@
     #   pandas
 python-json-logger==2.0.7
     # via jupyter-events
 pytz==2023.3
     # via
     #   apscheduler
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   jupyter-events
     #   myst-parser
     #   pre-commit
     #   tablib
 pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
-    #   nbclassic
-    #   notebook
     #   qtconsole
 qtconsole==5.4.3
     # via jupyter
 qtpy==2.3.1
     # via qtconsole
-redis==4.5.5
+redis==4.6.0
     # via
     #   dallinger
     #   rq
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   dallinger
     #   docker
     #   heroku3
+    #   jupyterlab-server
     #   sphinx
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 rq==1.15.1
     # via dallinger
 s3transfer==0.6.1
     # via boto3
 selenium==4.10.0
     # via dallinger
 send2trash==1.8.2
-    # via
-    #   jupyter-server
-    #   nbclassic
-    #   notebook
+    # via jupyter-server
 six==1.16.0
     # via
     #   apscheduler
     #   asttokens
     #   bleach
     #   dallinger
     #   python-dateutil
@@ -561,15 +563,15 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via dallinger
-sqlalchemy==1.4.48
+sqlalchemy==1.4.49
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 sqlalchemy-postgres-copy==0.5.0
     # via dallinger
 sshtunnel==0.4.0
     # via dallinger
@@ -583,115 +585,116 @@
     #   tablib
 tenacity==8.2.2
     # via dallinger
 terminado==0.17.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
-    #   nbclassic
-    #   notebook
 timeago==1.0.16
     # via dallinger
 tinycss2==1.2.1
     # via nbconvert
 tomli==2.0.1
     # via
     #   black
     #   build
+    #   jupyterlab
+    #   pip-tools
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
 tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-    #   nbclassic
+    #   jupyterlab
     #   notebook
     #   terminado
-tox==4.6.3
+tox==4.6.4
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-console
     #   jupyter-core
     #   jupyter-events
     #   jupyter-server
+    #   jupyterlab
     #   matplotlib-inline
-    #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
-    #   notebook
     #   qtconsole
-trio==0.22.0
+trio==0.22.2
     # via
     #   selenium
     #   trio-websocket
 trio-websocket==0.10.3
     # via selenium
+typing-extensions==4.7.1
+    # via async-lru
 tzdata==2023.3
     # via pandas
 tzlocal==5.0.1
     # via
     #   apscheduler
     #   dallinger
-ua-parser==0.16.1
+ua-parser==0.18.0
     # via
     #   dallinger
     #   user-agents
 uri-template==1.3.0
     # via jsonschema
 urllib3==1.26.16
     # via
     #   botocore
     #   docker
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-virtualenv==20.23.1
+virtualenv==20.24.2
     # via
     #   pre-commit
     #   tox
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.6.0
+websocket-client==1.6.1
     # via
     #   docker
     #   jupyter-server
 werkzeug==2.3.6
     # via
     #   flask
     #   flask-login
-wheel==0.40.0
+wheel==0.41.0
     # via pip-tools
-widgetsnbextension==4.0.7
+widgetsnbextension==4.0.8
     # via ipywidgets
 wsproto==1.2.0
     # via trio-websocket
 wtforms==3.0.1
     # via flask-wtf
 xlrd==2.0.1
     # via tablib
 xlwt==1.3.0
     # via tablib
-zope-event==4.6
+zope-event==5.0
     # via gevent
 zope-interface==6.0
     # via gevent
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `dallinger-9.8.2/docs/Makefile` & `dallinger-9.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/make.bat` & `dallinger-9.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.eot` & `dallinger-9.9.0/docs/source/_static/AvenirLTStd-Book_gdi.eot`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.svg` & `dallinger-9.9.0/docs/source/_static/AvenirLTStd-Book_gdi.svg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.ttf` & `dallinger-9.9.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/AvenirLTStd-Book_gdi.woff` & `dallinger-9.9.0/docs/source/_static/AvenirLTStd-Book_gdi.woff`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/Dallinger AWS Group.png` & `dallinger-9.9.0/docs/source/_static/Dallinger AWS Group.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/barplot.png` & `dallinger-9.9.0/docs/source/_static/barplot.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/burst.png` & `dallinger-9.9.0/docs/source/_static/burst.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/chain.png` & `dallinger-9.9.0/docs/source/_static/chain.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/class_chart.jpg` & `dallinger-9.9.0/docs/source/_static/class_chart.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/corner.jpg` & `dallinger-9.9.0/docs/source/_static/corner.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/custom.css` & `dallinger-9.9.0/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/delayed.png` & `dallinger-9.9.0/docs/source/_static/delayed.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/directories.jpg` & `dallinger-9.9.0/docs/source/_static/directories.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/empty.jpg` & `dallinger-9.9.0/docs/source/_static/empty.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/front_back_layout.jpg` & `dallinger-9.9.0/docs/source/_static/front_back_layout.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/full.png` & `dallinger-9.9.0/docs/source/_static/full.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/grid.png` & `dallinger-9.9.0/docs/source/_static/grid.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/grid_mini.png` & `dallinger-9.9.0/docs/source/_static/grid_mini.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/grid_small.png` & `dallinger-9.9.0/docs/source/_static/grid_small.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/heroku.jpg` & `dallinger-9.9.0/docs/source/_static/heroku.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/_static/star.png` & `dallinger-9.9.0/docs/source/_static/star.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/aws_etc_keys.rst` & `dallinger-9.9.0/docs/source/aws_etc_keys.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/build_demo_docs.py` & `dallinger-9.9.0/docs/source/build_demo_docs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/building_documentation.rst` & `dallinger-9.9.0/docs/source/building_documentation.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/classes.rst` & `dallinger-9.9.0/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/command_line_utility.rst` & `dallinger-9.9.0/docs/source/command_line_utility.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/communicating_with_the_server.rst` & `dallinger-9.9.0/docs/source/communicating_with_the_server.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/conf.py` & `dallinger-9.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/configuration.rst` & `dallinger-9.9.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/contributing_to_dallinger.rst` & `dallinger-9.9.0/docs/source/contributing_to_dallinger.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,66 @@
 Releasing a new version of Dallinger
 ====================================
 
 1. After you've merged the changes you want into `master`, start a new branch on
-which to run the release version upgrade and update the CHANGELOG if that hasn't
+which to run the release version upgrade, e.g. ``release-9.8.1``. Update the CHANGELOG if that hasn't
 been done as part of feature branch work. The entry should link to the new version's
-tree using: `https://github.com/dallinger/dallinger/tree/vX.X.X.`
+tree using: `https://github.com/dallinger/dallinger/tree/vMAJOR.MINOR.PATCH.`
 
 We're using semantic versioning, so there are three parts to the version number.
 when making a release you need to decide which parts should get bumped, which determines
 which command you give to `bumpversion`. `major` is for breaking changes, `minor` for features,
 `patch` for bug fixes.
 
 Under normal circumstances, the ``master`` branch will have a version number
 reflecting a `minor` increment over the previous release, plus a `a1` suffix
-indicating that it includes unreleased ("alpha") changes. If the release you're
+indicating that it includes unreleased ("alpha") changes, e.g. ``9.9.0a1``. If the release you're
 making is indeed a `minor` release, then simply run ``bumpversion release``.
 This will remove the `a1` suffix, leaving the correct minor version increment.
 
 If you have breaking changes and need to switch to a `major` release, then you
 will need to first make that change, commit, and then issue the release increment
 command::
 
     $ bumpversion major
     $ git commit -a -m "Switch to major release"
     $ bumpversion release
     $ git commit -a -m "Update versions for release"
 
 If you need to switch to a `patch` release, you will instead need to
-specify the version explicitly with the ``new-version`` option::
+specify the version explicitly with the ``new-version`` option:, e.g.
 
-    $ bumpversion --new-version 7.7.1
+    $ bumpversion --new-version 9.8.1 patch
     $ git commit -a -m "Switch to patch release"
-    $ bumpverion release
-    $ git commit -a -m "Update versions for release"
 
 2. Run `scripts/update_experiments_constraints.sh` to update the constraints.txt
-files in the demos.
+files in the demos and commit the changes with
+
+    $ git commit -m "Update demos' constraints"
 
 3.  Push your branch and create a PR with the `release` label.
 
-4. Merge this release with the commit "Release version X.X.X."
+4. Merge this release with the commit "Release version MAJOR.MINOR.PATCH."
 
-5. After that's merged, you'll want to tag the merge commit with `git tag vX.X.X` and do `git push origin --tags`. PyPI releases versions based on the tags via `.travis.yml`.
+5. After that's merged, you'll want to tag the merge commit with `git tag vMAJOR.MINOR.PATCH` and do `git push origin --tags`. PyPI releases versions based on the tags via `.travis.yml`.
 
 6. At this point, **WAIT** to make sure the release is successful. If you prematurely
    increment versions again (see next step) and the release has problems, you'll
    find yourself in an unnecessarily confusing situation.
 
-7. Create a new branch (``increment-master-version`` or similar), and bump the
-version to the next `minor` increment::
+7. Create a new branch (``increment-master-version``), and bump the
+version to the next `minor` alpha version::
 
     $ git checkout -b increment-master-version
     $ bumpversion minor
     $ git commit -a -m "Bump version on master branch post-release"
-    $ git push
+    $ git push --set-upstream origin increment-master-version
+
+.. note::
+
+    In case the ``increment-master-version`` branch already exists locally from a previous Dallinger release, you would first need to delete it with
+
+    $ git br -d increment-master-version
+
+You'll then need to open a PR for approval and get the ``increment-master-version`` branch merged as soon as possible, e.g. before merging in new feature branches.
 
-You'll then need to open a PR for approval and get this merged as soon as possible.
+The new Dallinger release should now be published on PyPi (https://pypi.org/project/dallinger/).
```

### Comparing `dallinger-9.8.2/docs/source/creating_an_experiment.rst` & `dallinger-9.9.0/docs/source/creating_an_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/demo_index.rst` & `dallinger-9.9.0/docs/source/demo_index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/demoing_dallinger.rst` & `dallinger-9.9.0/docs/source/demoing_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/demos_on_heroku.rst` & `dallinger-9.9.0/docs/source/demos_on_heroku.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/developing_dallinger_setup_guide.rst` & `dallinger-9.9.0/docs/source/developing_dallinger_setup_guide.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/docker_only.rst` & `dallinger-9.9.0/docs/source/docker_only.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/docker_support.rst` & `dallinger-9.9.0/docs/source/docker_support.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/docker_tutorial.rst` & `dallinger-9.9.0/docs/source/docker_tutorial.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/email_setup.rst` & `dallinger-9.9.0/docs/source/email_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/experiment_data.rst` & `dallinger-9.9.0/docs/source/experiment_data.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/extra_configuration.rst` & `dallinger-9.9.0/docs/source/extra_configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/index.rst` & `dallinger-9.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/installing_dallinger_for_users.rst` & `dallinger-9.9.0/docs/source/installing_dallinger_for_users.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/javascript_api.rst` & `dallinger-9.9.0/docs/source/javascript_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/learning_to_use_dallinger.rst` & `dallinger-9.9.0/docs/source/learning_to_use_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/monitoring_a_live_experiment.rst` & `dallinger-9.9.0/docs/source/monitoring_a_live_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/networks.rst` & `dallinger-9.9.0/docs/source/networks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/postico_and_postgres.rst` & `dallinger-9.9.0/docs/source/postico_and_postgres.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/private_repo.rst` & `dallinger-9.9.0/docs/source/private_repo.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/python_module.rst` & `dallinger-9.9.0/docs/source/python_module.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/recruitment.rst` & `dallinger-9.9.0/docs/source/recruitment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/required_experiment_files.rst` & `dallinger-9.9.0/docs/source/required_experiment_files.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/rewarding_participants.rst` & `dallinger-9.9.0/docs/source/rewarding_participants.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/running_bots.rst` & `dallinger-9.9.0/docs/source/running_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/running_the_tests.rst` & `dallinger-9.9.0/docs/source/running_the_tests.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/scheduled_tasks.rst` & `dallinger-9.9.0/docs/source/scheduled_tasks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/spelling_wordlist.txt` & `dallinger-9.9.0/docs/source/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/the_experiment_class.rst` & `dallinger-9.9.0/docs/source/the_experiment_class.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/troubleshooting.rst` & `dallinger-9.9.0/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/vagrant_setup.rst` & `dallinger-9.9.0/docs/source/vagrant_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/waiting_rooms.rst` & `dallinger-9.9.0/docs/source/waiting_rooms.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/web_api.rst` & `dallinger-9.9.0/docs/source/web_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/docs/source/writing_bots.rst` & `dallinger-9.9.0/docs/source/writing_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/incubator.png` & `dallinger-9.9.0/incubator.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/requirements.txt` & `dallinger-9.9.0/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,63 +6,61 @@
 #
 
     # via -r requirements.in
 apscheduler==3.10.1
     # via dallinger
 asttokens==2.2.1
     # via stack-data
-async-generator==1.10
-    # via trio
 async-timeout==4.0.2
     # via redis
 attrs==23.1.0
     # via
     #   outcome
     #   trio
 backcall==0.2.0
     # via ipython
 blinker==1.6.2
     # via flask
-boto3==1.26.158
+boto3==1.28.11
     # via dallinger
-botocore==1.29.158
+botocore==1.31.11
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
 cached-property==1.5.2
     # via dallinger
-certifi==2023.5.7
+certifi==2023.7.22
     # via
     #   requests
     #   selenium
 cffi==1.15.1
     # via cryptography
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via
     #   dallinger
     #   flask
     #   pip-tools
     #   rq
-cryptography==41.0.1
+cryptography==41.0.2
     # via pyopenssl
 decorator==5.1.1
     # via ipython
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.11.1
+faker==19.2.0
     # via dallinger
 flask==2.3.2
     # via
     #   dallinger
     #   flask-crossdomain
     #   flask-login
     #   flask-sockets
@@ -73,27 +71,27 @@
     # via dallinger
 flask-sockets==0.2.1
     # via dallinger
 flask-wtf==1.1.1
     # via dallinger
 future==0.18.3
     # via dallinger
-gevent==22.10.2
+gevent==23.7.0
     # via
     #   dallinger
     #   flask-sockets
     #   gevent-websocket
 gevent-websocket==0.10.1
     # via flask-sockets
 greenlet==2.0.2
     # via
     #   dallinger
     #   gevent
     #   sqlalchemy
-gunicorn==20.1.0
+gunicorn==21.2.0
     # via dallinger
 h11==0.14.0
     # via wsproto
 heroku3==5.2.1
     # via dallinger
 idna==3.4
     # via
@@ -118,31 +116,33 @@
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
     #   wtforms
 matplotlib-inline==0.1.6
     # via ipython
-numpy==1.24.3
+numpy==1.24.4
     # via dallinger
 outcome==1.2.0
     # via trio
 packaging==23.1
-    # via build
+    # via
+    #   build
+    #   gunicorn
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
-pip-tools==6.13.0
+pip-tools==7.1.0
     # via dallinger
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 psutil==5.9.5
     # via dallinger
 psycopg2==2.9.6
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
@@ -163,15 +163,15 @@
 python-dateutil==2.8.2
     # via
     #   botocore
     #   faker
     #   heroku3
 pytz==2023.3
     # via apscheduler
-redis==4.5.5
+redis==4.6.0
     # via
     #   dallinger
     #   rq
 requests==2.31.0
     # via
     #   dallinger
     #   heroku3
@@ -188,15 +188,15 @@
     #   dallinger
     #   python-dateutil
     #   sqlalchemy-postgres-copy
 sniffio==1.3.0
     # via trio
 sortedcontainers==2.4.0
     # via trio
-sqlalchemy==1.4.48
+sqlalchemy==1.4.49
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 sqlalchemy-postgres-copy==0.5.0
     # via dallinger
 stack-data==0.6.2
     # via ipython
@@ -205,30 +205,31 @@
 tenacity==8.2.2
     # via dallinger
 timeago==1.0.16
     # via dallinger
 tomli==2.0.1
     # via
     #   build
+    #   pip-tools
     #   pyproject-hooks
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-trio==0.22.0
+trio==0.22.2
     # via
     #   selenium
     #   trio-websocket
 trio-websocket==0.10.3
     # via selenium
 tzlocal==5.0.1
     # via
     #   apscheduler
     #   dallinger
-ua-parser==0.16.1
+ua-parser==0.18.0
     # via
     #   dallinger
     #   user-agents
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
@@ -237,21 +238,21 @@
     # via dallinger
 wcwidth==0.2.6
     # via prompt-toolkit
 werkzeug==2.3.6
     # via
     #   flask
     #   flask-login
-wheel==0.40.0
+wheel==0.41.0
     # via pip-tools
 wsproto==1.2.0
     # via trio-websocket
 wtforms==3.0.1
     # via flask-wtf
-zope-event==4.6
+zope-event==5.0
     # via gevent
 zope-interface==6.0
     # via gevent
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `dallinger-9.8.2/setup.py` & `dallinger-9.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
 
 setup_args = dict(
     name="dallinger",
     packages=["dallinger", "dallinger_scripts"],
-    version="9.8.2",
+    version="9.9.0",
     description="Laboratory automation for the behavioral and social sciences",
     long_description=README,
     long_description_content_type="text/markdown",
     url="http://github.com/Dallinger/Dallinger",
     maintainer="Jordan Suchow",
     maintainer_email="suchow@berkeley.edu",
     license="MIT",
@@ -94,15 +94,15 @@
         "data": [
             "pandas",
             "tablib[all]",
         ],
         "dev": [
             "alabaster",
             "black",
-            "bumpversion",
+            "bump2version",
             "coverage",
             "coverage_pth",
             "flake8",
             "isort",
             "mock",
             "myst-parser",
             "pre-commit",
```

### Comparing `dallinger-9.8.2/tests/test_agents.py` & `dallinger-9.9.0/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_api.py` & `dallinger-9.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_bots.py` & `dallinger-9.9.0/tests/test_bots.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_cli_config.py` & `dallinger-9.9.0/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_command_line.py` & `dallinger-9.9.0/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_config.py` & `dallinger-9.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_dashboard.py` & `dallinger-9.9.0/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_data.py` & `dallinger-9.9.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_db.py` & `dallinger-9.9.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_demos.py` & `dallinger-9.9.0/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_deployment.py` & `dallinger-9.9.0/tests/test_deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_docker.py` & `dallinger-9.9.0/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_environments.py` & `dallinger-9.9.0/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_experiment_server.py` & `dallinger-9.9.0/tests/test_experiment_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1741,14 +1741,15 @@
 def standard_args(experiment):
     from sqlalchemy.orm.scoping import scoped_session
 
     from dallinger.models import Participant
 
     participant = mock.Mock(
         spec_set=Participant,
+        id="42",
         status="working",
         worker_id="123",
         assignment_id="some assignment id",
     )
 
     return {
         "participant": participant,
@@ -1770,105 +1771,24 @@
         experiment.data_check.return_value = True
         experiment.bonus.return_value = 0.0
         experiment.bonus_reason.return_value = "You rock."
         standard_args["config"].update({"base_payment": 1.00})
 
         return AssignmentSubmitted(**standard_args)
 
-    def test_calls_reward_bonus_if_experiment_returns_bonus_more_than_one_cent(
-        self, runner
-    ):
-        runner.experiment.bonus.return_value = 0.02
+    def test_calls_on_assignment_submitted_to_recruiter(self, runner):
         runner()
-        runner.participant.recruiter.reward_bonus.assert_called_once_with(
-            runner.participant, 0.02, "You rock."
-        )
-
-    def test_no_reward_bonus_if_experiment_returns_bonus_less_than_one_cent(
-        self, runner
-    ):
-        runner()
-        runner.participant.recruiter.reward_bonus.assert_not_called()
-        assert "NOT paying bonus" in str(runner.experiment.log.call_args_list)
-
-    def test_sets_participant_bonus_regardless(self, runner):
-        runner.experiment.bonus.return_value = 0.005
-        runner()
-        assert runner.participant.bonus == 0.005
-
-    def test_approve_hit_called_on_recruiter(self, runner):
-        runner()
-        runner.participant.recruiter.approve_hit.assert_called_once_with(
-            "some assignment id"
-        )
-
-    def test_participant_base_pay_set(self, runner):
-        runner()
-        assert runner.participant.base_pay == 1.0
-
-    def test_participant_status_set(self, runner):
-        runner()
-        assert runner.participant.status == "approved"
-
-    def test_approves_overrecruited_participants(self, runner):
-        runner.participant.status = "overrecruited"
-        runner()
-        assert runner.participant.status == "approved"
-
-    def test_participant_end_time_set(self, runner):
-        runner()
-        assert runner.participant.end_time == end_time
-
-    def test_submission_successful_called_on_experiment(self, runner):
-        runner()
-        runner.experiment.submission_successful.assert_called_once_with(
-            participant=runner.participant
-        )
-
-    def test_recruit_called_on_experiment(self, runner):
-        runner()
-        runner.experiment.recruit.assert_called_once()
-
-    def test_does_nothing_if_already_approved_worker(self, runner):
-        runner.participant.status = "approved"
-        runner()
-        runner.session.assert_not_called()
-
-    def test_sets_participant_status_on_failed_data_check(self, runner):
-        runner.experiment.data_check.return_value = False
-        runner()
-        assert runner.participant.status == "bad_data"
-
-    def test_calls_data_check_failed_on_failed_data_check(self, runner):
-        runner.experiment.data_check.return_value = False
-        runner()
-        runner.experiment.data_check_failed.assert_called_once_with(
-            participant=runner.participant
-        )
-
-    def test_recruits_another_on_failed_data_check(self, runner):
-        runner.experiment.data_check.return_value = False
-        runner()
-        runner.experiment.recruiter.recruit.assert_called_once_with(n=1)
-
-    def test_no_bonus_inquiry_on_failed_data_check(self, runner):
-        runner.experiment.data_check.return_value = False
-        runner()
-        runner.experiment.bonus.assert_not_called()
-
-    def test_sets_participant_status_on_failed_attention_check(self, runner):
-        runner.experiment.attention_check.return_value = False
-        runner()
-        assert runner.participant.status == "did_not_attend"
-
-    def test_calls_attention_check_failed_on_failed_attention_check(self, runner):
-        runner.experiment.attention_check.return_value = False
-        runner()
-        runner.experiment.attention_check_failed.assert_called_once_with(
-            participant=runner.participant
+        runner.experiment.on_assignment_submitted_to_recruiter.assert_called_once_with(
+            participant=runner.participant,
+            event={
+                "event_type": "AssignmentSubmitted",
+                "participant_id": "42",
+                "assignment_id": "some assignment id",
+                "timestamp": end_time,
+            },
         )
 
 
 class TestBotAssignmentSubmitted(object):
     @pytest.fixture
     def runner(self, standard_args):
         from dallinger.experiment_server.worker_events import BotAssignmentSubmitted
```

### Comparing `dallinger-9.8.2/tests/test_griduniverse.py` & `dallinger-9.9.0/tests/test_griduniverse.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_heroku.py` & `dallinger-9.9.0/tests/test_heroku.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_information.py` & `dallinger-9.9.0/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_jupyter.py` & `dallinger-9.9.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_models.py` & `dallinger-9.9.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_mturk.py` & `dallinger-9.9.0/tests/test_mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_networks.py` & `dallinger-9.9.0/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_notifications.py` & `dallinger-9.9.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_processes.py` & `dallinger-9.9.0/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_prolific.py` & `dallinger-9.9.0/tests/test_prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_recruiters.py` & `dallinger-9.9.0/tests/test_recruiters.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
     def test_open_recruitment_uses_configured_mode(self, recruiter, active_config):
         active_config.extend({"mode": "new_mode"})
         result = recruiter.open_recruitment()
         assert "mode=new_mode" in result["items"][0]
 
     def test_returns_standard_submission_event_type(self, recruiter):
-        assert recruiter.submitted_event() == "AssignmentSubmitted"
+        assert recruiter.on_completion_event() == "AssignmentSubmitted"
 
 
 @pytest.mark.usefixtures("active_config")
 class TestHotAirRecruiter(object):
     @pytest.fixture
     def recruiter(self):
         from dallinger.recruiters import HotAirRecruiter
@@ -236,15 +236,15 @@
 
     def test_open_recruitment_ignores_configured_mode(self, recruiter, active_config):
         active_config.extend({"mode": "new_mode"})
         result = recruiter.open_recruitment()
         assert "mode=debug" in result["items"][0]
 
     def test_returns_standard_submission_event_type(self, recruiter):
-        assert recruiter.submitted_event() == "AssignmentSubmitted"
+        assert recruiter.on_completion_event() == "AssignmentSubmitted"
 
 
 class TestSimulatedRecruiter(object):
     @pytest.fixture
     def recruiter(self):
         from dallinger.recruiters import SimulatedRecruiter
 
@@ -259,15 +259,15 @@
     def test_open_recruitment_returns_empty_result(self, recruiter):
         assert recruiter.open_recruitment()["items"] == []
 
     def test_open_recruitment_multiple_returns_empty_result(self, recruiter):
         assert recruiter.open_recruitment(n=3)["items"] == []
 
     def test_returns_standard_submission_event_type(self, recruiter):
-        assert recruiter.submitted_event() == "AssignmentSubmitted"
+        assert recruiter.on_completion_event() == "AssignmentSubmitted"
 
     def test_close_recruitment(self, recruiter):
         assert recruiter.close_recruitment() is None
 
 
 class TestBotRecruiter(object):
     @pytest.fixture
@@ -308,15 +308,15 @@
     def test_approve_hit(self, recruiter):
         assert recruiter.approve_hit("any assignment id")
 
     def test_reward_bonus(self, a, recruiter):
         recruiter.reward_bonus(a.participant(), 0.01, "You're great!")
 
     def test_returns_specific_submission_event_type(self, recruiter):
-        assert recruiter.submitted_event() == "BotAssignmentSubmitted"
+        assert recruiter.on_completion_event() == "BotAssignmentSubmitted"
 
     def test_notify_duration_exceeded_rejects_participants(self, a, recruiter):
         bot = a.participant(recruiter_id="bots")
 
         recruiter.notify_duration_exceeded([bot], datetime.now())
 
         assert bot.status == "rejected"
@@ -420,16 +420,16 @@
         assert dallinger_format == {
             "hit_id": "some study ID",
             "worker_id": "some worker ID",
             "assignment_id": "some session ID",
             "entry_information": prolific_format,
         }
 
-    def test_defers_assignment_submission_via_null_submitted_event(self, recruiter):
-        assert recruiter.submitted_event() is None
+    def test_defers_assignment_submission_via_null_on_completion_event(self, recruiter):
+        assert recruiter.on_completion_event() is None
 
     @pytest.mark.usefixtures("experiment_dir_merged")
     def test_exit_page_includes_submission_prolific_button(self, a, webapp, recruiter):
         p = a.participant(recruiter_id="prolific")
 
         response = webapp.get(f"/recruiter-exit?participant_id={p.id}")
 
@@ -953,15 +953,15 @@
         from dallinger.recruiters import MTurkRecruiterException
 
         recruiter.open_recruitment()
         with pytest.raises(MTurkRecruiterException):
             recruiter.open_recruitment()
 
     def test_supresses_assignment_submitted(self, recruiter):
-        assert recruiter.submitted_event() is None
+        assert recruiter.on_completion_event() is None
 
     def test_current_hit_id_with_active_experiment(self, recruiter, fake_parsed_hit):
         recruiter.open_recruitment()
         assert recruiter.current_hit_id() == fake_parsed_hit["id"]
 
     def test_current_hit_id_with_no_active_experiment(self, recruiter):
         assert recruiter.current_hit_id() is None
```

### Comparing `dallinger-9.8.2/tests/test_replay.py` & `dallinger-9.9.0/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_replay_state.py` & `dallinger-9.9.0/tests/test_replay_state.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_sockets.py` & `dallinger-9.9.0/tests/test_sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_sources.py` & `dallinger-9.9.0/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_transformations.py` & `dallinger-9.9.0/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.2/tests/test_utils.py` & `dallinger-9.9.0/tests/test_utils.py`

 * *Files identical despite different names*

