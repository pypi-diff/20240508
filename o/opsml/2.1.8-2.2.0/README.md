# Comparing `tmp/opsml-2.1.8.tar.gz` & `tmp/opsml-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsml-2.1.8.tar", max compression
+gzip compressed data, was "opsml-2.2.0.tar", max compression
```

## Comparing `opsml-2.1.8.tar` & `opsml-2.2.0.tar`

### file list

```diff
@@ -1,213 +1,213 @@
--rw-r--r--   0        0        0     1067 2024-03-18 13:30:56.175730 opsml-2.1.8/LICENSE.md
--rw-r--r--   0        0        0    11724 2024-03-18 13:30:56.175730 opsml-2.1.8/README.md
--rw-r--r--   0        0        0     2091 2024-03-18 13:30:56.231730 opsml-2.1.8/opsml/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/core/__init__.py
--rw-r--r--   0        0        0     2807 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/core/dependencies.py
--rw-r--r--   0        0        0     2080 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/core/event_handlers.py
--rw-r--r--   0        0        0      876 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/core/gunicorn.py
--rw-r--r--   0        0        0     1395 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/core/login.py
--rw-r--r--   0        0        0      798 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/core/middleware.py
--rw-r--r--   0        0        0      540 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/gunicorn_conf.py
--rw-r--r--   0        0        0     1978 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/main.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/__init__.py
--rw-r--r--   0        0        0    11175 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/audit.py
--rw-r--r--   0        0        0     8379 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/cards.py
--rw-r--r--   0        0        0     3353 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/data.py
--rw-r--r--   0        0        0     8688 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/files.py
--rw-r--r--   0        0        0      949 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/healthcheck.py
--rw-r--r--   0        0        0      804 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/homepage.py
--rw-r--r--   0        0        0     2234 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/metrics.py
--rw-r--r--   0        0        0     8626 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/models.py
--rw-r--r--   0        0        0     2828 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/projects.py
--rw-r--r--   0        0        0    11427 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/pydantic_models.py
--rw-r--r--   0        0        0     1227 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/registry.py
--rw-r--r--   0        0        0    21813 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/route_helpers.py
--rw-r--r--   0        0        0     1153 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/router.py
--rw-r--r--   0        0        0    10983 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/routes/utils.py
--rw-r--r--   0        0        0    38854 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/DIGESTS.md
--rw-r--r--   0        0        0     1514 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/LICENSE
--rw-r--r--   0        0        0     1723 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/README.md
--rw-r--r--   0        0        0    76007 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/es/core.js
--rw-r--r--   0        0        0    20455 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/es/core.min.js
--rw-r--r--   0        0        0    76007 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/es/highlight.js
--rw-r--r--   0        0        0    20455 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/es/highlight.min.js
--rw-r--r--   0        0        0       20 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/es/package.json
--rw-r--r--   0        0        0    80693 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/highlight.js
--rw-r--r--   0        0        0    33245 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/highlight.min.js
--rw-r--r--   0        0        0      496 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/languages/json.min.js
--rw-r--r--   0        0        0     2119 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/languages/markdown.min.js
--rw-r--r--   0        0        0     3529 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/languages/python.min.js
--rw-r--r--   0        0        0     6544 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/languages/sql.min.js
--rw-r--r--   0        0        0     2945 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/package.json
--rw-r--r--   0        0        0     2116 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/styles/stackoverflow-dark.css
--rw-r--r--   0        0        0     1271 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/styles/stackoverflow-dark.min.css
--rw-r--r--   0        0        0     2118 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/styles/stackoverflow-light.css
--rw-r--r--   0        0        0     1285 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/code_highlight/styles/stackoverflow-light.min.css
--rw-r--r--   0        0        0      815 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/css/font.css
--rw-r--r--   0        0        0    21871 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/css/style.css
--rw-r--r--   0        0        0    59456 2024-03-18 13:30:56.235730 opsml-2.1.8/opsml/app/static/fonts/custom/bold.otf
--rw-r--r--   0        0        0    64836 2024-03-18 13:30:56.239730 opsml-2.1.8/opsml/app/static/fonts/custom/italic.otf
--rw-r--r--   0        0        0    60804 2024-03-18 13:30:56.239730 opsml-2.1.8/opsml/app/static/fonts/custom/medium.otf
--rw-r--r--   0        0        0    61244 2024-03-18 13:30:56.239730 opsml-2.1.8/opsml/app/static/fonts/custom/regular.otf
--rw-r--r--   0        0        0    62084 2024-03-18 13:30:56.239730 opsml-2.1.8/opsml/app/static/fonts/custom/semibold.otf
--rw-r--r--   0        0        0    29191 2024-03-18 13:30:56.239730 opsml-2.1.8/opsml/app/static/images/chip.png
--rw-r--r--   0        0        0   542303 2024-03-18 13:30:56.239730 opsml-2.1.8/opsml/app/static/images/machine-learning.png
--rw-r--r--   0        0        0  1498117 2024-03-18 13:30:56.243730 opsml-2.1.8/opsml/app/static/images/opsml-logo.png
--rw-r--r--   0        0        0    38936 2024-03-18 13:30:56.243730 opsml-2.1.8/opsml/app/static/images/opsml_word.png
--rw-r--r--   0        0        0   207720 2024-03-18 13:30:56.247730 opsml-2.1.8/opsml/app/static/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444233 2024-03-18 13:30:56.247730 opsml-2.1.8/opsml/app/static/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80668 2024-03-18 13:30:56.247730 opsml-2.1.8/opsml/app/static/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   331827 2024-03-18 13:30:56.247730 opsml-2.1.8/opsml/app/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135736 2024-03-18 13:30:56.247730 opsml-2.1.8/opsml/app/static/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305099 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/static/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    74154 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/static/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222450 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145302 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/static/js/bootstrap.js
--rw-r--r--   0        0        0   306267 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/static/js/bootstrap.js.map
--rw-r--r--   0        0        0    60582 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/static/js/bootstrap.min.js
--rw-r--r--   0        0        0   220293 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/static/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     2211 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/base.html
--rw-r--r--   0        0        0      880 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/500.html
--rw-r--r--   0        0        0     9072 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/audit/audit.html
--rw-r--r--   0        0        0     1380 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/audit/audit_section.html
--rw-r--r--   0        0        0     3088 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/audit/comment_card.html
--rw-r--r--   0        0        0      562 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/data/card.html
--rw-r--r--   0        0        0     1865 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/data/data.html
--rw-r--r--   0        0        0     3984 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/data/data_extras.html
--rw-r--r--   0        0        0     2905 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/data/data_metadata.html
--rw-r--r--   0        0        0      584 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/data/data_profile.html
--rw-r--r--   0        0        0      966 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/data/data_subnav.html
--rw-r--r--   0        0        0     1026 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/data/data_summary.html
--rw-r--r--   0        0        0      580 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/data/data_tags.html
--rw-r--r--   0        0        0     4957 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/data/data_version.html
--rw-r--r--   0        0        0      565 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/model/card.html
--rw-r--r--   0        0        0     4117 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/model/model_extras.html
--rw-r--r--   0        0        0     5384 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/model/model_metadata.html
--rw-r--r--   0        0        0      941 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/model/model_subnav.html
--rw-r--r--   0        0        0     1343 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/model/model_summary.html
--rw-r--r--   0        0        0      677 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/model/model_tags.html
--rw-r--r--   0        0        0     3667 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/model/model_version.html
--rw-r--r--   0        0        0     1925 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/model/models.html
--rw-r--r--   0        0        0     1604 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/navbar.html
--rw-r--r--   0        0        0     7310 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/project/metric_page.html
--rw-r--r--   0        0        0      578 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/project/no_projects.html
--rw-r--r--   0        0        0      342 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/project/plot_extras.html
--rw-r--r--   0        0        0     3264 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/project/projects.html
--rw-r--r--   0        0        0     3608 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/project/run_metadata.html
--rw-r--r--   0        0        0     8727 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/app/templates/include/project/runcard_extras.html
--rw-r--r--   0        0        0      651 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/cards/__init__.py
--rw-r--r--   0        0        0     8747 2024-03-18 13:30:56.251730 opsml-2.1.8/opsml/cards/audit.py
--rw-r--r--   0        0        0     3694 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cards/base.py
--rw-r--r--   0        0        0     5622 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cards/data.py
--rw-r--r--   0        0        0     5604 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cards/model.py
--rw-r--r--   0        0        0     2739 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cards/pipeline.py
--rw-r--r--   0        0        0      812 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cards/project.py
--rw-r--r--   0        0        0    17088 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cards/run.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cards/templates/__init__.py
--rw-r--r--   0        0        0    27313 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cards/templates/audit_card.yaml
--rw-r--r--   0        0        0       20 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cli/__init__.py
--rw-r--r--   0        0        0      839 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/cli/launch_server.py
--rw-r--r--   0        0        0     1119 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/__init__.py
--rw-r--r--   0        0        0     3176 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/formatter.py
--rw-r--r--   0        0        0      360 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/__init__.py
--rw-r--r--   0        0        0     1863 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/_arrow.py
--rw-r--r--   0        0        0     8145 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/_base.py
--rw-r--r--   0        0        0     5235 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/_image.py
--rw-r--r--   0        0        0     1628 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/_numpy.py
--rw-r--r--   0        0        0     2067 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/_pandas.py
--rw-r--r--   0        0        0     2063 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/_polars.py
--rw-r--r--   0        0        0      531 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/_sql.py
--rw-r--r--   0        0        0     4450 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/_text.py
--rw-r--r--   0        0        0     1816 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/_torch.py
--rw-r--r--   0        0        0     1631 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/backups.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/custom_data/__init__.py
--rw-r--r--   0        0        0     4287 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/custom_data/arrow_reader.py
--rw-r--r--   0        0        0     5896 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/custom_data/arrow_writer.py
--rw-r--r--   0        0        0     6498 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/custom_data/base.py
--rw-r--r--   0        0        0     2776 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/custom_data/image.py
--rw-r--r--   0        0        0     2023 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/interfaces/custom_data/text.py
--rw-r--r--   0        0        0     9951 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/data/splitter.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/helpers/__init__.py
--rw-r--r--   0        0        0     1983 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/helpers/data.py
--rw-r--r--   0        0        0      230 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/helpers/exceptions.py
--rw-r--r--   0        0        0     3014 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/helpers/gcp_utils.py
--rw-r--r--   0        0        0      624 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/helpers/logging.py
--rw-r--r--   0        0        0     9343 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/helpers/utils.py
--rw-r--r--   0        0        0     1143 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/__init__.py
--rw-r--r--   0        0        0    10822 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/challenger.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/__init__.py
--rw-r--r--   0        0        0     3543 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/backups.py
--rw-r--r--   0        0        0     7268 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/base.py
--rw-r--r--   0        0        0     7758 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/catboost_.py
--rw-r--r--   0        0        0    18883 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/huggingface.py
--rw-r--r--   0        0        0     5126 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/lgbm.py
--rw-r--r--   0        0        0     8888 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/pytorch.py
--rw-r--r--   0        0        0     5741 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/pytorch_lightning.py
--rw-r--r--   0        0        0     3681 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/sklearn.py
--rw-r--r--   0        0        0     5573 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/tf.py
--rw-r--r--   0        0        0     4372 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/vowpal.py
--rw-r--r--   0        0        0     7277 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/interfaces/xgb.py
--rw-r--r--   0        0        0     6209 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/loader.py
--rw-r--r--   0        0        0     3242 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/metadata_creator.py
--rw-r--r--   0        0        0     4013 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/onnx/__init__.py
--rw-r--r--   0        0        0     6724 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/onnx/base_converter.py
--rw-r--r--   0        0        0     8160 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/onnx/data_converters.py
--rw-r--r--   0        0        0     1123 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/onnx/lightgbm_converter.py
--rw-r--r--   0        0        0     4881 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/onnx/registry_updaters.py
--rw-r--r--   0        0        0     7604 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/onnx/sklearn_converter.py
--rw-r--r--   0        0        0     1379 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/onnx/tensorflow_converter.py
--rw-r--r--   0        0        0     4899 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/onnx/torch_converter.py
--rw-r--r--   0        0        0     6987 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/registrar.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/utils/__init__.py
--rw-r--r--   0        0        0    16551 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/utils/data_helper.py
--rw-r--r--   0        0        0     2853 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/model/utils/skl2onnx_data_types.py
--rw-r--r--   0        0        0       52 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/profile/__init__.py
--rw-r--r--   0        0        0     4489 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/profile/profile_config.yml
--rw-r--r--   0        0        0     2745 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/profile/profile_data.py
--rw-r--r--   0        0        0      217 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/projects/__init__.py
--rw-r--r--   0        0        0     5313 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/projects/_run_manager.py
--rw-r--r--   0        0        0    10841 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/projects/active_run.py
--rw-r--r--   0        0        0     7602 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/projects/project.py
--rw-r--r--   0        0        0     1833 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/projects/types.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.255730 opsml-2.1.8/opsml/py.typed
--rw-r--r--   0        0        0      111 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/__init__.py
--rw-r--r--   0        0        0     1400 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/backend.py
--rw-r--r--   0        0        0     3885 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/records.py
--rw-r--r--   0        0        0     9014 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/registry.py
--rw-r--r--   0        0        0    13638 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/semver.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/base/__init__.py
--rw-r--r--   0        0        0    14472 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/base/client.py
--rw-r--r--   0        0        0     2636 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/base/db_initializer.py
--rw-r--r--   0        0        0    17409 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/base/query_engine.py
--rw-r--r--   0        0        0    10972 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/base/registry_base.py
--rw-r--r--   0        0        0    14441 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/base/server.py
--rw-r--r--   0        0        0     5747 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/base/sql_schema.py
--rw-r--r--   0        0        0      633 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/base/utils.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/connectors/__init__.py
--rw-r--r--   0        0        0     4800 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/connectors/base.py
--rw-r--r--   0        0        0     3733 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/connectors/connector.py
--rw-r--r--   0        0        0       38 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/migration/alembic/README
--rw-r--r--   0        0        0     2121 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/migration/alembic/env.py
--rw-r--r--   0        0        0      510 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     3343 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/migration/alembic.ini
--rw-r--r--   0        0        0      507 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/registry/sql/migration/migrate.py
--rw-r--r--   0        0        0       91 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/settings/__init__.py
--rw-r--r--   0        0        0     2759 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/settings/config.py
--rw-r--r--   0        0        0        0 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/storage/__init__.py
--rw-r--r--   0        0        0     5420 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/storage/api.py
--rw-r--r--   0        0        0    21101 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/storage/card_loader.py
--rw-r--r--   0        0        0    17278 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/storage/card_saver.py
--rw-r--r--   0        0        0    13817 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/storage/client.py
--rw-r--r--   0        0        0     2975 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/types/__init__.py
--rw-r--r--   0        0        0     3850 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/types/card.py
--rw-r--r--   0        0        0     2408 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/types/data.py
--rw-r--r--   0        0        0     3790 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/types/extra.py
--rw-r--r--   0        0        0     3281 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/types/huggingface.py
--rw-r--r--   0        0        0    13778 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/types/model.py
--rw-r--r--   0        0        0     1460 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/types/sql.py
--rw-r--r--   0        0        0     3124 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/types/storage.py
--rw-r--r--   0        0        0      428 2024-03-18 13:30:56.259730 opsml-2.1.8/opsml/version.py
--rw-r--r--   0        0        0     8246 2024-03-18 13:30:56.263730 opsml-2.1.8/pyproject.toml
--rw-r--r--   0        0        0    14735 1970-01-01 00:00:00.000000 opsml-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-08 18:45:04.392200 opsml-2.2.0/LICENSE.md
+-rw-r--r--   0        0        0    11715 2024-05-08 18:45:04.392200 opsml-2.2.0/README.md
+-rw-r--r--   0        0        0     2091 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/core/__init__.py
+-rw-r--r--   0        0        0     2807 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/core/dependencies.py
+-rw-r--r--   0        0        0     2080 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/core/event_handlers.py
+-rw-r--r--   0        0        0      876 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/core/gunicorn.py
+-rw-r--r--   0        0        0     1395 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/core/login.py
+-rw-r--r--   0        0        0      812 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/core/middleware.py
+-rw-r--r--   0        0        0      540 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/gunicorn_conf.py
+-rw-r--r--   0        0        0     1978 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/__init__.py
+-rw-r--r--   0        0        0    11175 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/audit.py
+-rw-r--r--   0        0        0     8379 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/cards.py
+-rw-r--r--   0        0        0     3353 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/data.py
+-rw-r--r--   0        0        0     8688 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/files.py
+-rw-r--r--   0        0        0      949 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/healthcheck.py
+-rw-r--r--   0        0        0      804 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/homepage.py
+-rw-r--r--   0        0        0     2234 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/metrics.py
+-rw-r--r--   0        0        0     8626 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/models.py
+-rw-r--r--   0        0        0     2828 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/projects.py
+-rw-r--r--   0        0        0    11427 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/pydantic_models.py
+-rw-r--r--   0        0        0     1227 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/registry.py
+-rw-r--r--   0        0        0    21813 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/route_helpers.py
+-rw-r--r--   0        0        0     1153 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/router.py
+-rw-r--r--   0        0        0    10983 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/routes/utils.py
+-rw-r--r--   0        0        0    38854 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/static/code_highlight/DIGESTS.md
+-rw-r--r--   0        0        0     1514 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/static/code_highlight/LICENSE
+-rw-r--r--   0        0        0     1723 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/static/code_highlight/README.md
+-rw-r--r--   0        0        0    76007 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/static/code_highlight/es/core.js
+-rw-r--r--   0        0        0    20455 2024-05-08 18:45:04.452200 opsml-2.2.0/opsml/app/static/code_highlight/es/core.min.js
+-rw-r--r--   0        0        0    76007 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/es/highlight.js
+-rw-r--r--   0        0        0    20455 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/es/highlight.min.js
+-rw-r--r--   0        0        0       20 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/es/package.json
+-rw-r--r--   0        0        0    80693 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/highlight.js
+-rw-r--r--   0        0        0    33245 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/highlight.min.js
+-rw-r--r--   0        0        0      496 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/languages/json.min.js
+-rw-r--r--   0        0        0     2119 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/languages/markdown.min.js
+-rw-r--r--   0        0        0     3529 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/languages/python.min.js
+-rw-r--r--   0        0        0     6544 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/languages/sql.min.js
+-rw-r--r--   0        0        0     2945 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/package.json
+-rw-r--r--   0        0        0     2116 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/styles/stackoverflow-dark.css
+-rw-r--r--   0        0        0     1271 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/styles/stackoverflow-dark.min.css
+-rw-r--r--   0        0        0     2118 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/styles/stackoverflow-light.css
+-rw-r--r--   0        0        0     1285 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/code_highlight/styles/stackoverflow-light.min.css
+-rw-r--r--   0        0        0      815 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/css/font.css
+-rw-r--r--   0        0        0    21871 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/css/style.css
+-rw-r--r--   0        0        0    59456 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/fonts/custom/bold.otf
+-rw-r--r--   0        0        0    64836 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/fonts/custom/italic.otf
+-rw-r--r--   0        0        0    60804 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/fonts/custom/medium.otf
+-rw-r--r--   0        0        0    61244 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/fonts/custom/regular.otf
+-rw-r--r--   0        0        0    62084 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/fonts/custom/semibold.otf
+-rw-r--r--   0        0        0    29191 2024-05-08 18:45:04.456200 opsml-2.2.0/opsml/app/static/images/chip.png
+-rw-r--r--   0        0        0   542303 2024-05-08 18:45:04.460200 opsml-2.2.0/opsml/app/static/images/machine-learning.png
+-rw-r--r--   0        0        0  1498117 2024-05-08 18:45:04.464201 opsml-2.2.0/opsml/app/static/images/opsml-logo.png
+-rw-r--r--   0        0        0    38936 2024-05-08 18:45:04.464201 opsml-2.2.0/opsml/app/static/images/opsml_word.png
+-rw-r--r--   0        0        0   207720 2024-05-08 18:45:04.464201 opsml-2.2.0/opsml/app/static/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444233 2024-05-08 18:45:04.464201 opsml-2.2.0/opsml/app/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80668 2024-05-08 18:45:04.468201 opsml-2.2.0/opsml/app/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   331827 2024-05-08 18:45:04.468201 opsml-2.2.0/opsml/app/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135736 2024-05-08 18:45:04.468201 opsml-2.2.0/opsml/app/static/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305099 2024-05-08 18:45:04.468201 opsml-2.2.0/opsml/app/static/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    74154 2024-05-08 18:45:04.468201 opsml-2.2.0/opsml/app/static/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222450 2024-05-08 18:45:04.468201 opsml-2.2.0/opsml/app/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145302 2024-05-08 18:45:04.468201 opsml-2.2.0/opsml/app/static/js/bootstrap.js
+-rw-r--r--   0        0        0   306267 2024-05-08 18:45:04.468201 opsml-2.2.0/opsml/app/static/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60582 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220293 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/static/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     2211 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/base.html
+-rw-r--r--   0        0        0      880 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/500.html
+-rw-r--r--   0        0        0     9072 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/audit/audit.html
+-rw-r--r--   0        0        0     1380 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/audit/audit_section.html
+-rw-r--r--   0        0        0     3088 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/audit/comment_card.html
+-rw-r--r--   0        0        0      562 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/data/card.html
+-rw-r--r--   0        0        0     1865 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/data/data.html
+-rw-r--r--   0        0        0     3984 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/data/data_extras.html
+-rw-r--r--   0        0        0     2905 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/data/data_metadata.html
+-rw-r--r--   0        0        0      584 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/data/data_profile.html
+-rw-r--r--   0        0        0      966 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/data/data_subnav.html
+-rw-r--r--   0        0        0     1026 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/data/data_summary.html
+-rw-r--r--   0        0        0      580 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/data/data_tags.html
+-rw-r--r--   0        0        0     4957 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/data/data_version.html
+-rw-r--r--   0        0        0      565 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/model/card.html
+-rw-r--r--   0        0        0     4117 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/model/model_extras.html
+-rw-r--r--   0        0        0     5384 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/model/model_metadata.html
+-rw-r--r--   0        0        0      941 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/model/model_subnav.html
+-rw-r--r--   0        0        0     1343 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/model/model_summary.html
+-rw-r--r--   0        0        0      677 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/model/model_tags.html
+-rw-r--r--   0        0        0     3667 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/model/model_version.html
+-rw-r--r--   0        0        0     1925 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/model/models.html
+-rw-r--r--   0        0        0     1604 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/navbar.html
+-rw-r--r--   0        0        0     7310 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/project/metric_page.html
+-rw-r--r--   0        0        0      578 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/project/no_projects.html
+-rw-r--r--   0        0        0      342 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/project/plot_extras.html
+-rw-r--r--   0        0        0     3264 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/project/projects.html
+-rw-r--r--   0        0        0     3608 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/project/run_metadata.html
+-rw-r--r--   0        0        0     8727 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/app/templates/include/project/runcard_extras.html
+-rw-r--r--   0        0        0      651 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/__init__.py
+-rw-r--r--   0        0        0     8747 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/audit.py
+-rw-r--r--   0        0        0     3694 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/base.py
+-rw-r--r--   0        0        0     5622 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/data.py
+-rw-r--r--   0        0        0     5604 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/model.py
+-rw-r--r--   0        0        0     2739 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/pipeline.py
+-rw-r--r--   0        0        0      812 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/project.py
+-rw-r--r--   0        0        0    17087 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/run.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/templates/__init__.py
+-rw-r--r--   0        0        0    27313 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cards/templates/audit_card.yaml
+-rw-r--r--   0        0        0       20 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cli/__init__.py
+-rw-r--r--   0        0        0      839 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/cli/launch_server.py
+-rw-r--r--   0        0        0     1119 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/__init__.py
+-rw-r--r--   0        0        0     3176 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/formatter.py
+-rw-r--r--   0        0        0      360 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/__init__.py
+-rw-r--r--   0        0        0     1862 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/_arrow.py
+-rw-r--r--   0        0        0     8145 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/_base.py
+-rw-r--r--   0        0        0     5235 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/_image.py
+-rw-r--r--   0        0        0     1628 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/_numpy.py
+-rw-r--r--   0        0        0     2067 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/_pandas.py
+-rw-r--r--   0        0        0     2063 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/_polars.py
+-rw-r--r--   0        0        0      530 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/_sql.py
+-rw-r--r--   0        0        0     4450 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/_text.py
+-rw-r--r--   0        0        0     1816 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/_torch.py
+-rw-r--r--   0        0        0     1631 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/backups.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/custom_data/__init__.py
+-rw-r--r--   0        0        0     4287 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/custom_data/arrow_reader.py
+-rw-r--r--   0        0        0     5896 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/custom_data/arrow_writer.py
+-rw-r--r--   0        0        0     6498 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/custom_data/base.py
+-rw-r--r--   0        0        0     2776 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/custom_data/image.py
+-rw-r--r--   0        0        0     2023 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/interfaces/custom_data/text.py
+-rw-r--r--   0        0        0     9951 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/data/splitter.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/helpers/__init__.py
+-rw-r--r--   0        0        0     1983 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/helpers/data.py
+-rw-r--r--   0        0        0      230 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/helpers/exceptions.py
+-rw-r--r--   0        0        0     3014 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/helpers/gcp_utils.py
+-rw-r--r--   0        0        0      624 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/helpers/logging.py
+-rw-r--r--   0        0        0     9344 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/helpers/utils.py
+-rw-r--r--   0        0        0     1143 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/model/__init__.py
+-rw-r--r--   0        0        0    10822 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/model/challenger.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.472200 opsml-2.2.0/opsml/model/interfaces/__init__.py
+-rw-r--r--   0        0        0     3543 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/backups.py
+-rw-r--r--   0        0        0     7268 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/base.py
+-rw-r--r--   0        0        0     7758 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/catboost_.py
+-rw-r--r--   0        0        0    18883 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/huggingface.py
+-rw-r--r--   0        0        0     5126 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/lgbm.py
+-rw-r--r--   0        0        0     8890 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/pytorch.py
+-rw-r--r--   0        0        0     5741 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/pytorch_lightning.py
+-rw-r--r--   0        0        0     3681 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/sklearn.py
+-rw-r--r--   0        0        0     5573 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/tf.py
+-rw-r--r--   0        0        0     4372 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/vowpal.py
+-rw-r--r--   0        0        0     7277 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/interfaces/xgb.py
+-rw-r--r--   0        0        0     6209 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/loader.py
+-rw-r--r--   0        0        0     3242 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/metadata_creator.py
+-rw-r--r--   0        0        0     4013 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/onnx/__init__.py
+-rw-r--r--   0        0        0     6694 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/onnx/base_converter.py
+-rw-r--r--   0        0        0     8160 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/onnx/data_converters.py
+-rw-r--r--   0        0        0     1093 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/onnx/lightgbm_converter.py
+-rw-r--r--   0        0        0     4881 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/onnx/registry_updaters.py
+-rw-r--r--   0        0        0     7860 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/onnx/sklearn_converter.py
+-rw-r--r--   0        0        0     1349 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/onnx/tensorflow_converter.py
+-rw-r--r--   0        0        0     4899 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/onnx/torch_converter.py
+-rw-r--r--   0        0        0     7097 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/registrar.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/utils/__init__.py
+-rw-r--r--   0        0        0    16551 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/utils/data_helper.py
+-rw-r--r--   0        0        0     2853 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/model/utils/skl2onnx_data_types.py
+-rw-r--r--   0        0        0       52 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/profile/__init__.py
+-rw-r--r--   0        0        0     4489 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/profile/profile_config.yml
+-rw-r--r--   0        0        0     2745 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/profile/profile_data.py
+-rw-r--r--   0        0        0      217 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/projects/__init__.py
+-rw-r--r--   0        0        0     5309 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/projects/_run_manager.py
+-rw-r--r--   0        0        0    10841 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/projects/active_run.py
+-rw-r--r--   0        0        0     7602 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/projects/project.py
+-rw-r--r--   0        0        0     1833 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/projects/types.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/py.typed
+-rw-r--r--   0        0        0      111 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/__init__.py
+-rw-r--r--   0        0        0     1400 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/backend.py
+-rw-r--r--   0        0        0     3885 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/records.py
+-rw-r--r--   0        0        0     9014 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/registry.py
+-rw-r--r--   0        0        0    13638 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/semver.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/base/__init__.py
+-rw-r--r--   0        0        0    14472 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/base/client.py
+-rw-r--r--   0        0        0     2636 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/base/db_initializer.py
+-rw-r--r--   0        0        0    17409 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/base/query_engine.py
+-rw-r--r--   0        0        0    10972 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/base/registry_base.py
+-rw-r--r--   0        0        0    14441 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/base/server.py
+-rw-r--r--   0        0        0     5747 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/base/sql_schema.py
+-rw-r--r--   0        0        0      633 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/base/utils.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/connectors/__init__.py
+-rw-r--r--   0        0        0     4800 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/connectors/base.py
+-rw-r--r--   0        0        0     3733 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/connectors/connector.py
+-rw-r--r--   0        0        0       38 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/migration/alembic/README
+-rw-r--r--   0        0        0     2121 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/migration/alembic/env.py
+-rw-r--r--   0        0        0      510 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     3343 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/migration/alembic.ini
+-rw-r--r--   0        0        0      507 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/registry/sql/migration/migrate.py
+-rw-r--r--   0        0        0       91 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/settings/__init__.py
+-rw-r--r--   0        0        0     2759 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/settings/config.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/storage/__init__.py
+-rw-r--r--   0        0        0     5420 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/storage/api.py
+-rw-r--r--   0        0        0    21101 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/storage/card_loader.py
+-rw-r--r--   0        0        0    17278 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/storage/card_saver.py
+-rw-r--r--   0        0        0    13973 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/storage/client.py
+-rw-r--r--   0        0        0     2975 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/types/__init__.py
+-rw-r--r--   0        0        0     3849 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/types/card.py
+-rw-r--r--   0        0        0     2407 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/types/data.py
+-rw-r--r--   0        0        0     3790 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/types/extra.py
+-rw-r--r--   0        0        0     3281 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/types/huggingface.py
+-rw-r--r--   0        0        0    13733 2024-05-08 18:45:04.476201 opsml-2.2.0/opsml/types/model.py
+-rw-r--r--   0        0        0     1444 2024-05-08 18:45:04.480201 opsml-2.2.0/opsml/types/sql.py
+-rw-r--r--   0        0        0     3092 2024-05-08 18:45:04.480201 opsml-2.2.0/opsml/types/storage.py
+-rw-r--r--   0        0        0      428 2024-05-08 18:45:04.480201 opsml-2.2.0/opsml/version.py
+-rw-r--r--   0        0        0     8257 2024-05-08 18:45:04.480201 opsml-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14710 1970-01-01 00:00:00.000000 opsml-2.2.0/PKG-INFO
```

### Comparing `opsml-2.1.8/LICENSE.md` & `opsml-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/README.md` & `opsml-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <h1 align="center">
   <br>
   <img src="https://github.com/shipt/opsml/blob/main/images/opsml-logo.png?raw=true"  width="400" height="400" alt="opsml logo"/>
   <br>
 </h1>
 
+
 <h2 align="center">Universal Artifact Registration System for Machine Learning</h2>
 
 <h1 align="center"><a href="https://thorrester.github.io/opsml-ghpages/">OpsML Documentation</h1>
 
 [![Tests](https://github.com/shipt/opsml/actions/workflows/lint-unit-tests.yml/badge.svg?branch=main)](https://github.com/shipt/opsml/actions/workflows/lint-unit-tests.yml)
 [![Examples](https://github.com/shipt/opsml/actions/workflows/examples.yml/badge.svg)](https://github.com/shipt/opsml/actions/workflows/examples.yml)
 ![Style](https://img.shields.io/badge/code%20style-black-000000.svg)
@@ -37,15 +38,15 @@
 
 ## Incorporate into Existing Workflows
 
 Add quality control to your ML projects with little effort! With `opsml`, data and models are added to interfaces and cards, which are then registered via card registries. 
 
 # Incorporate into Existing Workflows
 
-Given it's simple and modular design, `opsml` can be easily incorporated into existing workflows. 
+Given its simple and modular design, `opsml` can be easily incorporated into existing workflows. 
 
 <h1 align="center">
   <br>
   <img src="https://github.com/shipt/opsml/blob/main/images/opsml-chip.png?raw=true"  width="800" alt="opsml logo"/>
   <br>
 </h1>
 
@@ -262,13 +263,15 @@
 | TensorFlow      | `TensorFlowModel`        | [link](examples/tensorflow/tf_example.py)           | 
 | HuggingFace     | `HuggingFaceModel`       | [link](examples/huggingface/hf_example.py)          | 
 | Vowpal Wabbit   | `VowpalWabbitModel`      | [link](examples/vowpal/vowpal_example.py)           | 
 
 ## Contributing
 If you'd like to contribute, be sure to check out our [contributing guide](./CONTRIBUTING.md)! If you'd like to work on any outstanding items, check out the `roadmap` section in the docs and get started :smiley:
 
-Thanks goes to these phenomenal [projects and people](./ATTRIBUTIONS.md) and people for creating a great foundation to build from!
+Thanks goes to these phenomenal [projects and people](./ATTRIBUTIONS.md) for creating a great foundation to build from!
 
 <a href="https://github.com/shipt/opsml/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=shipt/opsml" />
 </a>
 
+
+
```

#### html2text {}

```diff
@@ -27,17 +27,17 @@
 projects) and a SQL-based card registry system. Think `trading cards for
 machine learning`. - **Type Checking**: Strongly typed and type checking for
 data and model artifacts. - **Support**: Robust support for a variety of ML and
 data libraries. - **Automation**: Automated processes including onnx model
 conversion, metadata creation and production packaging. ## Incorporate into
 Existing Workflows Add quality control to your ML projects with little effort!
 With `opsml`, data and models are added to interfaces and cards, which are then
-registered via card registries. # Incorporate into Existing Workflows Given
-it's simple and modular design, `opsml` can be easily incorporated into
-existing workflows.
+registered via card registries. # Incorporate into Existing Workflows Given its
+simple and modular design, `opsml` can be easily incorporated into existing
+workflows.
                                     ************
                                  [[ooppssmmll llooggoo]]
                                      ************
 ## Installation: ### Poetry ```bash poetry add opsml ``` ### Pip ```bash pip
 install opsml ``` Setup your local environment: By default, `opsml` will log
 artifacts and experiments locally. To change this behavior and log to a remote
 server, you'll need to set the following environment variables: ```shell export
@@ -123,9 +123,9 @@
 TensorFlow | `TensorFlowModel` | [link](examples/tensorflow/tf_example.py) | |
 HuggingFace | `HuggingFaceModel` | [link](examples/huggingface/hf_example.py) |
 | Vowpal Wabbit | `VowpalWabbitModel` | [link](examples/vowpal/
 vowpal_example.py) | ## Contributing If you'd like to contribute, be sure to
 check out our [contributing guide](./CONTRIBUTING.md)! If you'd like to work on
 any outstanding items, check out the `roadmap` section in the docs and get
 started :smiley: Thanks goes to these phenomenal [projects and people](./
-ATTRIBUTIONS.md) and people for creating a great foundation to build from!
-_[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_s_h_i_p_t_/_o_p_s_m_l_]
+ATTRIBUTIONS.md) for creating a great foundation to build from!_[_h_t_t_p_s_:_/_/
+_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_s_h_i_p_t_/_o_p_s_m_l_]
```

### Comparing `opsml-2.1.8/opsml/__init__.py` & `opsml-2.2.0/opsml/__init__.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/core/dependencies.py` & `opsml-2.2.0/opsml/app/core/dependencies.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/core/event_handlers.py` & `opsml-2.2.0/opsml/app/core/event_handlers.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/core/gunicorn.py` & `opsml-2.2.0/opsml/app/core/gunicorn.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/core/login.py` & `opsml-2.2.0/opsml/app/core/login.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/core/middleware.py` & `opsml-2.2.0/opsml/app/core/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 
 
 async def rollbar_middleware(
     request: Request, call_next: Callable[[Request], MiddlewareReturnType]
 ) -> MiddlewareReturnType:
     try:
         return await call_next(request)  # type: ignore
-    except Exception:  # pylint: disable=broad-except
+    except Exception as ex:  # pylint: disable=broad-except
         rollbar.report_exc_info()
-        logger.error("unhandled API error")
+        logger.error("unhandled API error: {}", ex)
         return Response("Internal server error", status_code=500)
```

### Comparing `opsml-2.1.8/opsml/app/gunicorn_conf.py` & `opsml-2.2.0/opsml/app/gunicorn_conf.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/main.py` & `opsml-2.2.0/opsml/app/main.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/audit.py` & `opsml-2.2.0/opsml/app/routes/audit.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/cards.py` & `opsml-2.2.0/opsml/app/routes/cards.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/data.py` & `opsml-2.2.0/opsml/app/routes/data.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/files.py` & `opsml-2.2.0/opsml/app/routes/files.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/healthcheck.py` & `opsml-2.2.0/opsml/app/routes/healthcheck.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/homepage.py` & `opsml-2.2.0/opsml/app/routes/homepage.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/metrics.py` & `opsml-2.2.0/opsml/app/routes/metrics.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/models.py` & `opsml-2.2.0/opsml/app/routes/models.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/projects.py` & `opsml-2.2.0/opsml/app/routes/projects.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/pydantic_models.py` & `opsml-2.2.0/opsml/app/routes/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/registry.py` & `opsml-2.2.0/opsml/app/routes/registry.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/route_helpers.py` & `opsml-2.2.0/opsml/app/routes/route_helpers.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/router.py` & `opsml-2.2.0/opsml/app/routes/router.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/routes/utils.py` & `opsml-2.2.0/opsml/app/routes/utils.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/DIGESTS.md` & `opsml-2.2.0/opsml/app/static/code_highlight/DIGESTS.md`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/LICENSE` & `opsml-2.2.0/opsml/app/static/code_highlight/LICENSE`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/README.md` & `opsml-2.2.0/opsml/app/static/code_highlight/README.md`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/es/core.js` & `opsml-2.2.0/opsml/app/static/code_highlight/es/core.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/es/core.min.js` & `opsml-2.2.0/opsml/app/static/code_highlight/es/core.min.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/es/highlight.js` & `opsml-2.2.0/opsml/app/static/code_highlight/es/highlight.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/es/highlight.min.js` & `opsml-2.2.0/opsml/app/static/code_highlight/es/highlight.min.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/highlight.js` & `opsml-2.2.0/opsml/app/static/code_highlight/highlight.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/highlight.min.js` & `opsml-2.2.0/opsml/app/static/code_highlight/highlight.min.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/languages/markdown.min.js` & `opsml-2.2.0/opsml/app/static/code_highlight/languages/markdown.min.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/languages/python.min.js` & `opsml-2.2.0/opsml/app/static/code_highlight/languages/python.min.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/languages/sql.min.js` & `opsml-2.2.0/opsml/app/static/code_highlight/languages/sql.min.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/package.json` & `opsml-2.2.0/opsml/app/static/code_highlight/package.json`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/styles/stackoverflow-dark.css` & `opsml-2.2.0/opsml/app/static/code_highlight/styles/stackoverflow-dark.css`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/styles/stackoverflow-dark.min.css` & `opsml-2.2.0/opsml/app/static/code_highlight/styles/stackoverflow-dark.min.css`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/styles/stackoverflow-light.css` & `opsml-2.2.0/opsml/app/static/code_highlight/styles/stackoverflow-light.css`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/code_highlight/styles/stackoverflow-light.min.css` & `opsml-2.2.0/opsml/app/static/code_highlight/styles/stackoverflow-light.min.css`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/css/font.css` & `opsml-2.2.0/opsml/app/static/css/font.css`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/css/style.css` & `opsml-2.2.0/opsml/app/static/css/style.css`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/fonts/custom/bold.otf` & `opsml-2.2.0/opsml/app/static/fonts/custom/bold.otf`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/fonts/custom/italic.otf` & `opsml-2.2.0/opsml/app/static/fonts/custom/italic.otf`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/fonts/custom/medium.otf` & `opsml-2.2.0/opsml/app/static/fonts/custom/medium.otf`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/fonts/custom/regular.otf` & `opsml-2.2.0/opsml/app/static/fonts/custom/regular.otf`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/fonts/custom/semibold.otf` & `opsml-2.2.0/opsml/app/static/fonts/custom/semibold.otf`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/images/chip.png` & `opsml-2.2.0/opsml/app/static/images/chip.png`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/images/machine-learning.png` & `opsml-2.2.0/opsml/app/static/images/machine-learning.png`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/images/opsml-logo.png` & `opsml-2.2.0/opsml/app/static/images/opsml-logo.png`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/images/opsml_word.png` & `opsml-2.2.0/opsml/app/static/images/opsml_word.png`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.bundle.js` & `opsml-2.2.0/opsml/app/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.bundle.js.map` & `opsml-2.2.0/opsml/app/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.bundle.min.js` & `opsml-2.2.0/opsml/app/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.bundle.min.js.map` & `opsml-2.2.0/opsml/app/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.esm.js` & `opsml-2.2.0/opsml/app/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.esm.js.map` & `opsml-2.2.0/opsml/app/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.esm.min.js` & `opsml-2.2.0/opsml/app/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.esm.min.js.map` & `opsml-2.2.0/opsml/app/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.js` & `opsml-2.2.0/opsml/app/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.js.map` & `opsml-2.2.0/opsml/app/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.min.js` & `opsml-2.2.0/opsml/app/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/static/js/bootstrap.min.js.map` & `opsml-2.2.0/opsml/app/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/base.html` & `opsml-2.2.0/opsml/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/500.html` & `opsml-2.2.0/opsml/app/templates/include/500.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/audit/audit.html` & `opsml-2.2.0/opsml/app/templates/include/audit/audit.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/audit/audit_section.html` & `opsml-2.2.0/opsml/app/templates/include/audit/audit_section.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/audit/comment_card.html` & `opsml-2.2.0/opsml/app/templates/include/audit/comment_card.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/data/card.html` & `opsml-2.2.0/opsml/app/templates/include/data/card.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/data/data.html` & `opsml-2.2.0/opsml/app/templates/include/data/data.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/data/data_extras.html` & `opsml-2.2.0/opsml/app/templates/include/data/data_extras.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/data/data_metadata.html` & `opsml-2.2.0/opsml/app/templates/include/data/data_metadata.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/data/data_profile.html` & `opsml-2.2.0/opsml/app/templates/include/data/data_profile.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/data/data_subnav.html` & `opsml-2.2.0/opsml/app/templates/include/data/data_subnav.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/data/data_summary.html` & `opsml-2.2.0/opsml/app/templates/include/data/data_summary.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/data/data_tags.html` & `opsml-2.2.0/opsml/app/templates/include/data/data_tags.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/data/data_version.html` & `opsml-2.2.0/opsml/app/templates/include/data/data_version.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/model/card.html` & `opsml-2.2.0/opsml/app/templates/include/model/card.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/model/model_extras.html` & `opsml-2.2.0/opsml/app/templates/include/model/model_extras.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/model/model_metadata.html` & `opsml-2.2.0/opsml/app/templates/include/model/model_metadata.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/model/model_subnav.html` & `opsml-2.2.0/opsml/app/templates/include/model/model_subnav.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/model/model_summary.html` & `opsml-2.2.0/opsml/app/templates/include/model/model_summary.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/model/model_tags.html` & `opsml-2.2.0/opsml/app/templates/include/model/model_tags.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/model/model_version.html` & `opsml-2.2.0/opsml/app/templates/include/model/model_version.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/model/models.html` & `opsml-2.2.0/opsml/app/templates/include/model/models.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/navbar.html` & `opsml-2.2.0/opsml/app/templates/include/navbar.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/project/metric_page.html` & `opsml-2.2.0/opsml/app/templates/include/project/metric_page.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/project/no_projects.html` & `opsml-2.2.0/opsml/app/templates/include/project/no_projects.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/project/projects.html` & `opsml-2.2.0/opsml/app/templates/include/project/projects.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/project/run_metadata.html` & `opsml-2.2.0/opsml/app/templates/include/project/run_metadata.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/app/templates/include/project/runcard_extras.html` & `opsml-2.2.0/opsml/app/templates/include/project/runcard_extras.html`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/cards/__init__.py` & `opsml-2.2.0/opsml/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/cards/audit.py` & `opsml-2.2.0/opsml/cards/audit.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/cards/base.py` & `opsml-2.2.0/opsml/cards/base.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/cards/data.py` & `opsml-2.2.0/opsml/cards/data.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/cards/model.py` & `opsml-2.2.0/opsml/cards/model.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/cards/pipeline.py` & `opsml-2.2.0/opsml/cards/pipeline.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/cards/project.py` & `opsml-2.2.0/opsml/cards/project.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/cards/run.py` & `opsml-2.2.0/opsml/cards/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,14 @@
     assert isinstance(y, list), "y must be a list or dictionary"
     y = _decimate_list(y)
     assert x_length == len(y), "x and y must be the same length"
     return y, "single"
 
 
 class RunCard(ArtifactCard):
-
     """
     Create a RunCard from specified arguments.
 
     Apart from required args, a RunCard must be associated with one of
     datacard_uid, modelcard_uids or pipelinecard_uid
 
     Args:
```

### Comparing `opsml-2.1.8/opsml/cards/templates/audit_card.yaml` & `opsml-2.2.0/opsml/cards/templates/audit_card.yaml`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/cli/launch_server.py` & `opsml-2.2.0/opsml/cli/launch_server.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/__init__.py` & `opsml-2.2.0/opsml/data/__init__.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/formatter.py` & `opsml-2.2.0/opsml/data/formatter.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/_arrow.py` & `opsml-2.2.0/opsml/data/interfaces/_arrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import pyarrow.parquet as pq
 
 from opsml.data.interfaces._base import DataInterface
 from opsml.types import AllowedDataType, Feature, Suffix
 
 
 class ArrowData(DataInterface):
-
     """Arrow Table data interface
 
     Args:
         data:
             Pyarrow Table
         dependent_vars:
             List of dependent variables. Can be string or index if using numpy
```

### Comparing `opsml-2.1.8/opsml/data/interfaces/_base.py` & `opsml-2.2.0/opsml/data/interfaces/_base.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/_image.py` & `opsml-2.2.0/opsml/data/interfaces/_image.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/_numpy.py` & `opsml-2.2.0/opsml/data/interfaces/_numpy.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/_pandas.py` & `opsml-2.2.0/opsml/data/interfaces/_pandas.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/_polars.py` & `opsml-2.2.0/opsml/data/interfaces/_polars.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/_sql.py` & `opsml-2.2.0/opsml/data/interfaces/_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from opsml.data.interfaces._base import DataInterface
 from opsml.types import AllowedDataType
 
 
 class SqlData(DataInterface):
-
     """Arrow Table data interface
 
     Args:
 
         sql_logic:
             Dictionary of strings containing sql logic or sql files used to create the data
         feature_descriptions:
```

### Comparing `opsml-2.1.8/opsml/data/interfaces/_text.py` & `opsml-2.2.0/opsml/data/interfaces/_text.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/_torch.py` & `opsml-2.2.0/opsml/data/interfaces/_torch.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/backups.py` & `opsml-2.2.0/opsml/data/interfaces/backups.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/custom_data/arrow_reader.py` & `opsml-2.2.0/opsml/data/interfaces/custom_data/arrow_reader.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/custom_data/arrow_writer.py` & `opsml-2.2.0/opsml/data/interfaces/custom_data/arrow_writer.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/custom_data/base.py` & `opsml-2.2.0/opsml/data/interfaces/custom_data/base.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/custom_data/image.py` & `opsml-2.2.0/opsml/data/interfaces/custom_data/image.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/interfaces/custom_data/text.py` & `opsml-2.2.0/opsml/data/interfaces/custom_data/text.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/data/splitter.py` & `opsml-2.2.0/opsml/data/splitter.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/helpers/data.py` & `opsml-2.2.0/opsml/helpers/data.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/helpers/gcp_utils.py` & `opsml-2.2.0/opsml/helpers/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/helpers/logging.py` & `opsml-2.2.0/opsml/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/helpers/utils.py` & `opsml-2.2.0/opsml/helpers/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Suite of helper objects"""
+
 # Copyright (c) Shipt, Inc.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import importlib.util
 import os
 import re
```

### Comparing `opsml-2.1.8/opsml/model/__init__.py` & `opsml-2.2.0/opsml/model/__init__.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/challenger.py` & `opsml-2.2.0/opsml/model/challenger.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/backups.py` & `opsml-2.2.0/opsml/model/interfaces/backups.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/base.py` & `opsml-2.2.0/opsml/model/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/catboost_.py` & `opsml-2.2.0/opsml/model/interfaces/catboost_.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/huggingface.py` & `opsml-2.2.0/opsml/model/interfaces/huggingface.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/lgbm.py` & `opsml-2.2.0/opsml/model/interfaces/lgbm.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/pytorch.py` & `opsml-2.2.0/opsml/model/interfaces/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,17 @@
                 Optional arguments for ONNX conversion. See `TorchOnnxArgs` for supported arguments.
 
         Returns:
         TorchModel
         """
 
         model: Optional[torch.nn.Module] = None
-        sample_data: Optional[
-            Union[torch.Tensor, Dict[str, torch.Tensor], List[torch.Tensor], Tuple[torch.Tensor]]
-        ] = None
+        sample_data: Optional[Union[torch.Tensor, Dict[str, torch.Tensor], List[torch.Tensor], Tuple[torch.Tensor]]] = (
+            None
+        )
         onnx_args: Optional[TorchOnnxArgs] = None
         save_args: TorchSaveArgs = TorchSaveArgs()
         preprocessor: Optional[Any] = None
         preprocessor_name: str = CommonKwargs.UNDEFINED.value
 
         @property
         def model_class(self) -> str:
```

### Comparing `opsml-2.1.8/opsml/model/interfaces/pytorch_lightning.py` & `opsml-2.2.0/opsml/model/interfaces/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/sklearn.py` & `opsml-2.2.0/opsml/model/interfaces/sklearn.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/tf.py` & `opsml-2.2.0/opsml/model/interfaces/tf.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/vowpal.py` & `opsml-2.2.0/opsml/model/interfaces/vowpal.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/interfaces/xgb.py` & `opsml-2.2.0/opsml/model/interfaces/xgb.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/loader.py` & `opsml-2.2.0/opsml/model/loader.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/metadata_creator.py` & `opsml-2.2.0/opsml/model/metadata_creator.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/onnx/__init__.py` & `opsml-2.2.0/opsml/model/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/onnx/base_converter.py` & `opsml-2.2.0/opsml/model/onnx/base_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, Dict, List, Optional, Tuple
 
 import onnx
 import onnxruntime as rt
-from onnx import ModelProto  # type: ignore[attr-defined]
+from onnx import ModelProto
 
 from opsml.helpers.logging import ArtifactLogger
 from opsml.helpers.utils import OpsmlImportExceptions
 from opsml.model.interfaces.base import ModelInterface
 from opsml.model.onnx.data_converters import OnnxDataConverter
 from opsml.model.onnx.registry_updaters import OnnxRegistryUpdater
 from opsml.model.utils.data_helper import ModelDataHelper
```

### Comparing `opsml-2.1.8/opsml/model/onnx/data_converters.py` & `opsml-2.2.0/opsml/model/onnx/data_converters.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/onnx/lightgbm_converter.py` & `opsml-2.2.0/opsml/model/onnx/lightgbm_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Code for generating Onnx Models"""
 # Copyright (c) Shipt, Inc.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, List, cast
 
-from onnx import ModelProto  # type: ignore[attr-defined]
+from onnx import ModelProto
 
 from opsml.helpers.logging import ArtifactLogger
 from opsml.model.onnx.base_converter import _ModelConverter
 from opsml.types import LIGHTGBM_SUPPORTED_MODEL_TYPES
 
 logger = ArtifactLogger.get_logger()
```

### Comparing `opsml-2.1.8/opsml/model/onnx/registry_updaters.py` & `opsml-2.2.0/opsml/model/onnx/registry_updaters.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/onnx/sklearn_converter.py` & `opsml-2.2.0/opsml/model/onnx/sklearn_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import re
 import warnings
 from typing import Any, Dict, List, Optional, cast
 
-from onnx import ModelProto  # type: ignore[attr-defined]
+from onnx import ModelProto
 
 from opsml.helpers.logging import ArtifactLogger
 from opsml.model.onnx.base_converter import _ModelConverter
 from opsml.model.onnx.registry_updaters import OnnxRegistryUpdater
 from opsml.model.utils.data_helper import FloatTypeConverter
 from opsml.types import (
     SKLEARN_SUPPORTED_MODEL_TYPES,
@@ -176,14 +176,19 @@
         try:
             return cast(
                 ModelProto,
                 convert_sklearn(
                     model=self.trained_model,
                     initial_types=initial_types,
                     options=self.options,
+                    target_opset={
+                        "": 19,
+                        "ai.onnx.ml": 3,
+                    },  # need to pin since skl2onnx is not in sync with latest onnx release
+                    # opset 19/3 is the latest supported by skl2onnx (onnx v 1.14.1)
                 ),
             )
         except NameError as name_error:
             # There may be a small amount of instances where a sklearn classifier does
             # not support zipmap as a default option (LinearSVC). This catches those errors
             if re.search("Option 'zipmap' not in", str(name_error), re.IGNORECASE):
                 logger.info("Zipmap not supported for classifier")
```

### Comparing `opsml-2.1.8/opsml/model/onnx/tensorflow_converter.py` & `opsml-2.2.0/opsml/model/onnx/tensorflow_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Code for generating Onnx Models"""
 # Copyright (c) Shipt, Inc.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, List, cast
 
-from onnx import ModelProto  # type: ignore[attr-defined]
+from onnx import ModelProto
 
 from opsml.helpers.logging import ArtifactLogger
 from opsml.model.interfaces.tf import TensorFlowModel
 from opsml.model.onnx.base_converter import _ModelConverter
 from opsml.types import TrainedModelType
 
 logger = ArtifactLogger.get_logger()
```

### Comparing `opsml-2.1.8/opsml/model/onnx/torch_converter.py` & `opsml-2.2.0/opsml/model/onnx/torch_converter.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/registrar.py` & `opsml-2.2.0/opsml/model/registrar.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,33 @@
         """
         if storage_client is None:
             raise ValueError("storage_client is required")
         self.storage_client = storage_client
 
     def _registry_path(self, request: RegistrationRequest) -> Path:
         """Returns hardcoded uri"""
-        return Path(f"{config.opsml_registry_path}/{request.repository}/{request.name}/v{request.version}")
+        return Path(
+            f"{config.storage_root}/{config.opsml_registry_path}/{request.repository}/{request.name}/v{request.version}"
+        )
 
     def is_registered(self, request: RegistrationRequest) -> bool:
         """Checks if registry path is empty.
 
         You can call `is_registered` before attempting to register a model, but
         it's not required. Attempting to register a model that's already been
         registered will overwrite the currently registered model.
 
         Args:
             request: The model registration request.
         """
         path = self._registry_path(request)
-        files = self.storage_client.find(path)
+        try:
+            files = self.storage_client.find(path)
+        except OSError:
+            return False
         return bool(files)
 
     def _get_correct_model_uri(self, request: RegistrationRequest, metadata: ModelMetadata) -> Path:
         """Gets correct model uri based on the request's onnx flag.
 
         Args:
             request: The model registration request.
```

### Comparing `opsml-2.1.8/opsml/model/utils/data_helper.py` & `opsml-2.2.0/opsml/model/utils/data_helper.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/model/utils/skl2onnx_data_types.py` & `opsml-2.2.0/opsml/model/utils/skl2onnx_data_types.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/profile/profile_config.yml` & `opsml-2.2.0/opsml/profile/profile_config.yml`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/profile/profile_data.py` & `opsml-2.2.0/opsml/profile/profile_data.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/projects/_run_manager.py` & `opsml-2.2.0/opsml/projects/_run_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from opsml.projects.types import ProjectInfo, Tags
 from opsml.registry import CardRegistries
 from opsml.types import CommonKwargs
 
 logger = ArtifactLogger.get_logger()
 
 
-class ActiveRunException(Exception):
-    ...
+class ActiveRunException(Exception): ...
 
 
 class _RunManager:
     def __init__(self, project_info: ProjectInfo, registries: CardRegistries):
         """
         Manages runs for a given project including storing general attributes and creating, activating and
         ending runs. Also holds storage client needed to store artifacts associated with a run.
```

### Comparing `opsml-2.1.8/opsml/projects/active_run.py` & `opsml-2.2.0/opsml/projects/active_run.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/projects/project.py` & `opsml-2.2.0/opsml/projects/project.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/projects/types.py` & `opsml-2.2.0/opsml/projects/types.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/backend.py` & `opsml-2.2.0/opsml/registry/backend.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/records.py` & `opsml-2.2.0/opsml/registry/records.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/registry.py` & `opsml-2.2.0/opsml/registry/registry.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/semver.py` & `opsml-2.2.0/opsml/registry/semver.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/base/client.py` & `opsml-2.2.0/opsml/registry/sql/base/client.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/base/db_initializer.py` & `opsml-2.2.0/opsml/registry/sql/base/db_initializer.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/base/query_engine.py` & `opsml-2.2.0/opsml/registry/sql/base/query_engine.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/base/registry_base.py` & `opsml-2.2.0/opsml/registry/sql/base/registry_base.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/base/server.py` & `opsml-2.2.0/opsml/registry/sql/base/server.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/base/sql_schema.py` & `opsml-2.2.0/opsml/registry/sql/base/sql_schema.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/base/utils.py` & `opsml-2.2.0/opsml/registry/sql/base/utils.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/connectors/base.py` & `opsml-2.2.0/opsml/registry/sql/connectors/base.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/connectors/connector.py` & `opsml-2.2.0/opsml/registry/sql/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/migration/alembic/env.py` & `opsml-2.2.0/opsml/registry/sql/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/registry/sql/migration/alembic.ini` & `opsml-2.2.0/opsml/registry/sql/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/settings/config.py` & `opsml-2.2.0/opsml/settings/config.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/storage/api.py` & `opsml-2.2.0/opsml/storage/api.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/storage/card_loader.py` & `opsml-2.2.0/opsml/storage/card_loader.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/storage/card_saver.py` & `opsml-2.2.0/opsml/storage/card_saver.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/storage/client.py` & `opsml-2.2.0/opsml/storage/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,23 +178,29 @@
             client=client,
         )
 
     @cached_property
     def gcs_client(self) -> GCSClient:
         from google.cloud import storage
 
-        return cast(GCSClient, storage.Client())
+        assert isinstance(self.settings, GcsStorageClientSettings)
 
-    # cached_property is a decorator that caches the result of the function it decorates.
+        return cast(
+            GCSClient,
+            storage.Client(
+                credentials=self.settings.credentials,
+            ),
+        )
 
     @cached_property
     def get_id_credentials(self) -> Any:
         assert isinstance(self.settings, GcsStorageClientSettings)
 
         if self.settings.default_creds:
+            logger.debug("Default Creds: {}", self.settings.default_creds)
             from google.auth import compute_engine
             from google.auth.transport import requests
 
             auth_request = requests.Request()
             return compute_engine.IDTokenCredentials(auth_request, "")
 
         return self.settings.credentials
@@ -207,15 +213,15 @@
             blob = bucket.blob(str(path))
             return blob.generate_signed_url(
                 expiration=datetime.timedelta(seconds=expiration),
                 credentials=self.get_id_credentials,
                 method="GET",
             )
         except Exception as error:
-            logger.error(f"Failed to generate presigned URL: {error}")
+            logger.error("Failed to generate presigned URL: {}", error)
             return None
 
 
 class S3StorageClient(StorageClientBase):
     def __init__(
         self,
         settings: StorageSettings,
```

### Comparing `opsml-2.1.8/opsml/types/__init__.py` & `opsml-2.2.0/opsml/types/__init__.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/types/card.py` & `opsml-2.2.0/opsml/types/card.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         if not isinstance(other, Comment):
             return False
         return self.__dict__ == other.__dict__
 
 
 @dataclass
 class CardInfo:
-
     """
     Class that holds info related to an Artifact Card
 
     Args:
         name:
             Name of card
         repository:
```

### Comparing `opsml-2.1.8/opsml/types/data.py` & `opsml-2.2.0/opsml/types/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     LIST = "list"
     STR = "str"
     ORDERED_DICT = "collections.OrderedDict"
     JOBLIB = "joblib"
 
 
 class DataCardMetadata(BaseModel):
-
     """Create a DataCard metadata
 
     Args:
         description:
             Description for your data
         feature_map:
             Map of features in data (inferred when converting to pyarrow table)
```

### Comparing `opsml-2.1.8/opsml/types/extra.py` & `opsml-2.2.0/opsml/types/extra.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/types/huggingface.py` & `opsml-2.2.0/opsml/types/huggingface.py`

 * *Files identical despite different names*

### Comparing `opsml-2.1.8/opsml/types/model.py` & `opsml-2.2.0/opsml/types/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,14 @@
 @dataclass
 class OnnxAttr:
     onnx_path: Optional[str] = None
     onnx_version: Optional[str] = None
 
 
 class ModelMetadata(BaseModel):
-
     """Model metadata associated with all registered models
 
     Args:
         model_name:
             Name of model
         model_class:
             Name of model class
@@ -382,27 +381,24 @@
     model_config = ConfigDict(
         protected_namespaces=("protect_",),
         extra="allow",
     )
 
 
 # Sklearn protocol stub
-class BaseEstimator(Protocol):
-    ...
+class BaseEstimator(Protocol): ...
 
 
 # Onnx protocol stubs
 class Graph:
     @property
-    def output(self) -> Any:
-        ...
+    def output(self) -> Any: ...
 
     @property
-    def input(self) -> Any:
-        ...
+    def input(self) -> Any: ...
 
 
 class ModelProto(Protocol):
     ir_version: int
     producer_name: str
     producer_version: str
     domain: str
@@ -505,17 +501,14 @@
     @staticmethod
     def validate(model_class_name: str) -> bool:
         return model_class_name == "Booster"
 
 
 class ModelCard(Protocol):
     @property
-    def metadata(self) -> ModelCardMetadata:
-        ...
+    def metadata(self) -> ModelCardMetadata: ...
 
     @property
-    def model(self) -> Any:
-        ...
+    def model(self) -> Any: ...
 
     @property
-    def to_onnx(self) -> bool:
-        ...
+    def to_onnx(self) -> bool: ...
```

### Comparing `opsml-2.1.8/opsml/types/sql.py` & `opsml-2.2.0/opsml/types/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,15 @@
             return RegistryTableNames.PROJECT
         if l_name == "audit":
             return RegistryTableNames.AUDIT
         raise NotImplementedError()
 
 
 class RunCardRegistry(Protocol):
-    def insert_metric(self, metric: List[Dict[str, Any]]) -> None:
-        ...
+    def insert_metric(self, metric: List[Dict[str, Any]]) -> None: ...
 
     def get_metric(
         self,
         run_uid: str,
         name: Optional[List[str]] = None,
         names_only: bool = False,
-    ) -> Optional[List[Dict[str, Any]]]:
-        ...
+    ) -> Optional[List[Dict[str, Any]]]: ...
```

### Comparing `opsml-2.1.8/opsml/types/storage.py` & `opsml-2.2.0/opsml/types/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,33 +58,29 @@
 
 class BotoClient(Protocol):
     def generate_presigned_url(
         self,
         operation_name: str,
         Params: Dict[str, Any],  # pylint: disable=invalid-name
         ExpiresIn: int,  # pylint: disable=invalid-name
-    ) -> str:
-        ...
+    ) -> str: ...
 
 
 class Blob(Protocol):
     def generate_signed_url(
         self, credentials: Any, version: str = "v4", expiration: datetime.timedelta = 600, method: str = "GET"
-    ) -> str:
-        ...
+    ) -> str: ...
 
 
 class Bucket(Protocol):
-    def blob(self, name: str) -> Blob:
-        ...
+    def blob(self, name: str) -> Blob: ...
 
 
 class GCSClient(Protocol):
-    def bucket(self, name: str) -> Bucket:
-        ...
+    def bucket(self, name: str) -> Bucket: ...
 
 
 class StorageClientProtocol(Protocol):
     def get(self, rpath: Path, lpath: Path) -> None:
         """Copies file(s) from remote path (rpath) to local path (lpath)"""
 
     def ls(self, path: Path) -> List[Path]:  # pylint:  disable=invalid-name
```

### Comparing `opsml-2.1.8/pyproject.toml` & `opsml-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 [project.urls]
 Homepage = "https://github.com/shipt/opsml"
 Source = "https://github.com/shipt/opsml"
 
 
 [tool.poetry]
 name = "opsml"
-version = "2.1.8"
+version = "2.2.0"
 readme = "README.md"
 description = "Python MLOPs quality control tooling for your production ML workflows"
 authors = [
     "Steven Forrester <steven.forrester@shipt.com>",
     "Damon Allison <damon@shipt.com>",
 ]
 
@@ -66,23 +66,23 @@
 zarr = ">2.12.0"
 
 
 # optional dependencies for sql
 psycopg2 = { version = "^2.9.6", optional = true }
 
 # optional dependencies for onnx
-onnx = { version = ">=1.14.0, <1.15.0", optional = true }
+onnx = { version = ">=1.16.0", optional = true }
 onnxruntime = { version = ">=1.13.0, <1.17.0", optional = true }
 
 # optional dependencies for sklearn onnx
 skl2onnx = { version = "^1.14.1", optional = true }
 onnxmltools = { version = "^1.11.1", optional = true }
 
 # optional dependencies for tensorflow onnx
-tf2onnx = { version = ">=1.13.0, <1.15.0", optional = true }
+tf2onnx = { version = ">=1.16.1", optional = true }
 
 # optional dependencies for server
 alembic = { version = "^1.10.3", optional = true }
 fastapi = { version = "^0.109.0", optional = true }
 gunicorn = { version = "^20.1.0", optional = true }
 jinja2 = { version = "^3.1.2", optional = true }
 prometheus-fastapi-instrumentator = { version = "^6.0.0", optional = true }
@@ -160,15 +160,15 @@
 [tool.poetry.group.dev-lints]
 optional = true
 
 [tool.poetry.group.dev-lints.dependencies]
 ruff = "^0.1.0"
 types-pymysql = "^1.0.19.1"
 types-requests = "^2.28.11.7"
-black = "22.3.0"
+black = ">=24.3.0"
 mypy = "^1"
 types-protobuf = "^4.21.0.3"
 pylint = "^2.17.5"
 pylint-pydantic = "^0.2.4"
 types-pyyaml = "^6.0.12.12"
 isort = "^5.12.0"
 
@@ -192,14 +192,15 @@
 [tool.pylint.MASTER]
 ignore-paths = ["opsml/.local_tests/*", "opsml/registry/sql/migration/*"]
 load-plugins = ["pylint_pydantic", "pylint.extensions.docparams"]
 
 [tool.pylint.messages_control]
 max-line-length = 130
 disable = [
+    "multiple-statements",
     "too-few-public-methods",
     "design",
     "duplicate-code",
     "missing-class-docstring",
     "missing-function-docstring",
     "missing-module-docstring",
     "too-many-nested-blocks",
```

### Comparing `opsml-2.1.8/PKG-INFO` & `opsml-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsml
-Version: 2.1.8
+Version: 2.2.0
 Summary: Python MLOPs quality control tooling for your production ML workflows
 Author: Steven Forrester
 Author-email: steven.forrester@shipt.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,15 +26,15 @@
 Requires-Dist: fastapi (>=0.109.0,<0.110.0) ; extra == "server"
 Requires-Dist: fsspec (>=2023.1.0,<=2024.2.0)
 Requires-Dist: gcsfs (>=2023.5.0,<2024.0.0) ; extra == "gcp-mysql" or extra == "gcp-postgres" or extra == "gcs"
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "server"
 Requires-Dist: httpx (>=0.23.3,<1.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "server"
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
-Requires-Dist: onnx (>=1.14.0,<1.15.0) ; extra == "tf-onnx" or extra == "sklearn-onnx" or extra == "torch-onnx"
+Requires-Dist: onnx (>=1.16.0) ; extra == "tf-onnx" or extra == "sklearn-onnx" or extra == "torch-onnx"
 Requires-Dist: onnxmltools (>=1.11.1,<2.0.0) ; extra == "sklearn-onnx"
 Requires-Dist: onnxruntime (>=1.13.0,<1.17.0) ; extra == "tf-onnx" or extra == "sklearn-onnx" or extra == "torch-onnx"
 Requires-Dist: opsml-cli (>=0.4.0,<0.5.0)
 Requires-Dist: pandas (>=1.5.3,<3)
 Requires-Dist: pg8000 (>=1.29.4,<2.0.0) ; extra == "gcp-postgres"
 Requires-Dist: polars (>=0.18.0,<0.19.0)
 Requires-Dist: prometheus-fastapi-instrumentator (>=6.0.0,<7.0.0) ; extra == "server"
@@ -50,26 +50,27 @@
 Requires-Dist: rusty-logger (>=0.3.0,<0.4.0)
 Requires-Dist: s3fs (>=2023.5.0,<2024.0.0) ; extra == "s3"
 Requires-Dist: semver (>=2.13.0,<3.0.0)
 Requires-Dist: skl2onnx (>=1.14.1,<2.0.0) ; extra == "sklearn-onnx"
 Requires-Dist: sqlalchemy[mypy] (>=2,<3) ; extra == "server"
 Requires-Dist: streaming-form-data (>=1.11.0,<2.0.0) ; extra == "server"
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
-Requires-Dist: tf2onnx (>=1.13.0,<1.15.0) ; extra == "tf-onnx"
+Requires-Dist: tf2onnx (>=1.16.1) ; extra == "tf-onnx"
 Requires-Dist: uvicorn (>=0.24.0) ; extra == "server"
 Requires-Dist: ydata-profiling (>=4.6.1,<5.0.0) ; extra == "profiling"
 Requires-Dist: zarr (>2.12.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
   <img src="https://github.com/shipt/opsml/blob/main/images/opsml-logo.png?raw=true"  width="400" height="400" alt="opsml logo"/>
   <br>
 </h1>
 
+
 <h2 align="center">Universal Artifact Registration System for Machine Learning</h2>
 
 <h1 align="center"><a href="https://thorrester.github.io/opsml-ghpages/">OpsML Documentation</h1>
 
 [![Tests](https://github.com/shipt/opsml/actions/workflows/lint-unit-tests.yml/badge.svg?branch=main)](https://github.com/shipt/opsml/actions/workflows/lint-unit-tests.yml)
 [![Examples](https://github.com/shipt/opsml/actions/workflows/examples.yml/badge.svg)](https://github.com/shipt/opsml/actions/workflows/examples.yml)
 ![Style](https://img.shields.io/badge/code%20style-black-000000.svg)
@@ -99,15 +100,15 @@
 
 ## Incorporate into Existing Workflows
 
 Add quality control to your ML projects with little effort! With `opsml`, data and models are added to interfaces and cards, which are then registered via card registries. 
 
 # Incorporate into Existing Workflows
 
-Given it's simple and modular design, `opsml` can be easily incorporated into existing workflows. 
+Given its simple and modular design, `opsml` can be easily incorporated into existing workflows. 
 
 <h1 align="center">
   <br>
   <img src="https://github.com/shipt/opsml/blob/main/images/opsml-chip.png?raw=true"  width="800" alt="opsml logo"/>
   <br>
 </h1>
 
@@ -324,14 +325,16 @@
 | TensorFlow      | `TensorFlowModel`        | [link](examples/tensorflow/tf_example.py)           | 
 | HuggingFace     | `HuggingFaceModel`       | [link](examples/huggingface/hf_example.py)          | 
 | Vowpal Wabbit   | `VowpalWabbitModel`      | [link](examples/vowpal/vowpal_example.py)           | 
 
 ## Contributing
 If you'd like to contribute, be sure to check out our [contributing guide](./CONTRIBUTING.md)! If you'd like to work on any outstanding items, check out the `roadmap` section in the docs and get started :smiley:
 
-Thanks goes to these phenomenal [projects and people](./ATTRIBUTIONS.md) and people for creating a great foundation to build from!
+Thanks goes to these phenomenal [projects and people](./ATTRIBUTIONS.md) for creating a great foundation to build from!
 
 <a href="https://github.com/shipt/opsml/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=shipt/opsml" />
 </a>
 
 
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opsml Version: 2.1.8 Summary: Python MLOPs quality
+Metadata-Version: 2.1 Name: opsml Version: 2.2.0 Summary: Python MLOPs quality
 control tooling for your production ML workflows Author: Steven Forrester
 Author-email: steven.forrester@shipt.com Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: gcp-mysql
 Provides-Extra: gcp-postgres Provides-Extra: gcs Provides-Extra: mysql
 Provides-Extra: postgres Provides-Extra: profiling Provides-Extra: s3 Provides-
@@ -12,37 +12,36 @@
 python-connector (>=1.2.0,<2.0.0) ; extra == "gcp-mysql" or extra == "gcp-
 postgres" Requires-Dist: fastapi (>=0.109.0,<0.110.0) ; extra == "server"
 Requires-Dist: fsspec (>=2023.1.0,<=2024.2.0) Requires-Dist: gcsfs
 (>=2023.5.0,<2024.0.0) ; extra == "gcp-mysql" or extra == "gcp-postgres" or
 extra == "gcs" Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "server"
 Requires-Dist: httpx (>=0.23.3,<1.0.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ;
 extra == "server" Requires-Dist: joblib (>=1.3.2,<2.0.0) Requires-Dist: onnx
-(>=1.14.0,<1.15.0) ; extra == "tf-onnx" or extra == "sklearn-onnx" or extra ==
-"torch-onnx" Requires-Dist: onnxmltools (>=1.11.1,<2.0.0) ; extra == "sklearn-
-onnx" Requires-Dist: onnxruntime (>=1.13.0,<1.17.0) ; extra == "tf-onnx" or
-extra == "sklearn-onnx" or extra == "torch-onnx" Requires-Dist: opsml-cli
+(>=1.16.0) ; extra == "tf-onnx" or extra == "sklearn-onnx" or extra == "torch-
+onnx" Requires-Dist: onnxmltools (>=1.11.1,<2.0.0) ; extra == "sklearn-onnx"
+Requires-Dist: onnxruntime (>=1.13.0,<1.17.0) ; extra == "tf-onnx" or extra ==
+"sklearn-onnx" or extra == "torch-onnx" Requires-Dist: opsml-cli
 (>=0.4.0,<0.5.0) Requires-Dist: pandas (>=1.5.3,<3) Requires-Dist: pg8000
 (>=1.29.4,<2.0.0) ; extra == "gcp-postgres" Requires-Dist: polars
 (>=0.18.0,<0.19.0) Requires-Dist: prometheus-fastapi-instrumentator
 (>=6.0.0,<7.0.0) ; extra == "server" Requires-Dist: psycopg2 (>=2.9.6,<3.0.0) ;
 extra == "postgres" Requires-Dist: pyarrow (>=10.0.0) Requires-Dist: pydantic
 (>=2,<3) Requires-Dist: pydantic_settings (>=2,<3) Requires-Dist: pymysql
 (>=1.0.2,<2.0.0) ; extra == "gcp-mysql" or extra == "mysql" Requires-Dist:
 python-multipart (>=0.0.7,<0.0.8) ; extra == "server" Requires-Dist: pyyaml
 (>=6.0.1,<7.0.0) Requires-Dist: rich (>=13.3.5,<14.0.0) Requires-Dist: rollbar
 (>=0.16.3) ; extra == "server" Requires-Dist: rusty-logger (>=0.3.0,<0.4.0)
 Requires-Dist: s3fs (>=2023.5.0,<2024.0.0) ; extra == "s3" Requires-Dist:
 semver (>=2.13.0,<3.0.0) Requires-Dist: skl2onnx (>=1.14.1,<2.0.0) ; extra ==
 "sklearn-onnx" Requires-Dist: sqlalchemy[mypy] (>=2,<3) ; extra == "server"
 Requires-Dist: streaming-form-data (>=1.11.0,<2.0.0) ; extra == "server"
-Requires-Dist: tenacity (>=8.2.2,<9.0.0) Requires-Dist: tf2onnx
-(>=1.13.0,<1.15.0) ; extra == "tf-onnx" Requires-Dist: uvicorn (>=0.24.0) ;
-extra == "server" Requires-Dist: ydata-profiling (>=4.6.1,<5.0.0) ; extra ==
-"profiling" Requires-Dist: zarr (>2.12.0) Description-Content-Type: text/
-markdown
+Requires-Dist: tenacity (>=8.2.2,<9.0.0) Requires-Dist: tf2onnx (>=1.16.1) ;
+extra == "tf-onnx" Requires-Dist: uvicorn (>=0.24.0) ; extra == "server"
+Requires-Dist: ydata-profiling (>=4.6.1,<5.0.0) ; extra == "profiling"
+Requires-Dist: zarr (>2.12.0) Description-Content-Type: text/markdown
                                     ************
                                  [[ooppssmmll llooggoo]]
                                      ************
     ********** UUnniivveerrssaall AArrttiiffaacctt RReeggiissttrraattiioonn SSyysstteemm ffoorr MMaacchhiinnee LLeeaarrnniinngg **********
                        ************ _OO_pp_ss_MM_LL_ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ************
 [![Tests](https://github.com/shipt/opsml/actions/workflows/lint-unit-tests.yml/
 badge.svg?branch=main)](https://github.com/shipt/opsml/actions/workflows/lint-
@@ -68,17 +67,17 @@
 projects) and a SQL-based card registry system. Think `trading cards for
 machine learning`. - **Type Checking**: Strongly typed and type checking for
 data and model artifacts. - **Support**: Robust support for a variety of ML and
 data libraries. - **Automation**: Automated processes including onnx model
 conversion, metadata creation and production packaging. ## Incorporate into
 Existing Workflows Add quality control to your ML projects with little effort!
 With `opsml`, data and models are added to interfaces and cards, which are then
-registered via card registries. # Incorporate into Existing Workflows Given
-it's simple and modular design, `opsml` can be easily incorporated into
-existing workflows.
+registered via card registries. # Incorporate into Existing Workflows Given its
+simple and modular design, `opsml` can be easily incorporated into existing
+workflows.
                                     ************
                                  [[ooppssmmll llooggoo]]
                                      ************
 ## Installation: ### Poetry ```bash poetry add opsml ``` ### Pip ```bash pip
 install opsml ``` Setup your local environment: By default, `opsml` will log
 artifacts and experiments locally. To change this behavior and log to a remote
 server, you'll need to set the following environment variables: ```shell export
@@ -164,9 +163,9 @@
 TensorFlow | `TensorFlowModel` | [link](examples/tensorflow/tf_example.py) | |
 HuggingFace | `HuggingFaceModel` | [link](examples/huggingface/hf_example.py) |
 | Vowpal Wabbit | `VowpalWabbitModel` | [link](examples/vowpal/
 vowpal_example.py) | ## Contributing If you'd like to contribute, be sure to
 check out our [contributing guide](./CONTRIBUTING.md)! If you'd like to work on
 any outstanding items, check out the `roadmap` section in the docs and get
 started :smiley: Thanks goes to these phenomenal [projects and people](./
-ATTRIBUTIONS.md) and people for creating a great foundation to build from!
-_[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_s_h_i_p_t_/_o_p_s_m_l_]
+ATTRIBUTIONS.md) for creating a great foundation to build from!_[_h_t_t_p_s_:_/_/
+_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_s_h_i_p_t_/_o_p_s_m_l_]
```

