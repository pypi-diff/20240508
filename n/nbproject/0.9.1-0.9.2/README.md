# Comparing `tmp/nbproject-0.9.1.tar.gz` & `tmp/nbproject-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbproject-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nbproject-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nbproject-0.9.1.tar` & `nbproject-0.9.2.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0     2475 2023-06-15 19:08:05.360108 nbproject-0.9.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-06-10 19:50:58.313927 nbproject-0.9.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-06-10 19:50:58.314964 nbproject-0.9.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1880 2022-07-10 12:10:29.382368 nbproject-0.9.1/.gitignore
--rw-r--r--   0        0        0     1645 2022-08-29 09:33:05.135542 nbproject-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      740 2022-10-24 12:29:45.346974 nbproject-0.9.1/CITATION.cff
--rw-r--r--   0        0        0    11357 2022-04-18 20:46:44.681265 nbproject-0.9.1/LICENSE
--rw-r--r--   0        0        0     1374 2023-08-04 20:32:42.822118 nbproject-0.9.1/README.md
--rw-r--r--   0        0        0    20948 2023-08-04 20:33:09.651587 nbproject-0.9.1/docs/changelog.md
--rw-r--r--   0        0        0     1216 2023-08-04 20:32:42.822676 nbproject-0.9.1/docs/faq.md
--rw-r--r--   0        0        0     1874 2023-08-04 20:19:19.961650 nbproject-0.9.1/docs/faq/example-after-init-set-filename.ipynb
--rw-r--r--   0        0        0      153 2023-08-04 20:32:42.823012 nbproject-0.9.1/docs/faq/example-project-uninitialized.md
--rw-r--r--   0        0        0     1481 2023-08-04 20:19:19.962250 nbproject-0.9.1/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb
--rw-r--r--   0        0        0      117 2023-08-04 20:32:42.823159 nbproject-0.9.1/docs/faq/example-project.md
--rw-r--r--   0        0        0     1874 2023-08-04 20:19:19.963880 nbproject-0.9.1/docs/faq/example-project/2022-05-13-my-task-x.ipynb
--rw-r--r--   0        0        0     1661 2023-08-04 20:19:19.964730 nbproject-0.9.1/docs/faq/example-project/2022-07-18-my-task-y.ipynb
--rw-r--r--   0        0        0      364 2023-08-04 20:19:19.965113 nbproject-0.9.1/docs/faq/example-project/nbproject_metadata.yml
--rw-r--r--   0        0        0     1873 2023-08-04 20:19:19.965699 nbproject-0.9.1/docs/faq/header-author-field.ipynb
--rw-r--r--   0        0        0     1520 2023-08-04 20:19:19.966010 nbproject-0.9.1/docs/faq/inconsistent-packages-parents-no-store.ipynb
--rw-r--r--   0        0        0     2330 2023-08-04 20:19:19.966373 nbproject-0.9.1/docs/faq/inconsistent-packages-parents-store.ipynb
--rw-r--r--   0        0        0     1311 2023-08-04 20:19:19.967100 nbproject-0.9.1/docs/faq/initialize-set-env.ipynb
--rw-r--r--   0        0        0     2049 2023-08-04 20:19:19.967641 nbproject-0.9.1/docs/faq/initialize.ipynb
--rw-r--r--   0        0        0     4086 2023-08-04 20:19:19.967960 nbproject-0.9.1/docs/faq/internal-functions.ipynb
--rw-r--r--   0        0        0     2708 2023-08-04 20:19:19.968582 nbproject-0.9.1/docs/faq/not-initialized.ipynb
--rw-r--r--   0        0        0     1803 2023-08-04 20:19:19.968950 nbproject-0.9.1/docs/faq/publish-not-last-cell.ipynb
--rw-r--r--   0        0        0     1399 2023-08-04 20:19:19.969256 nbproject-0.9.1/docs/faq/publish-set-version.ipynb
--rw-r--r--   0        0        0     1818 2023-08-04 20:19:19.969587 nbproject-0.9.1/docs/faq/publish-without-saving.ipynb
--rw-r--r--   0        0        0     1787 2023-08-04 20:19:19.969884 nbproject-0.9.1/docs/faq/publish-without-title.ipynb
--rw-r--r--   0        0        0     1653 2023-08-04 20:19:19.970180 nbproject-0.9.1/docs/faq/publish-wrapper.ipynb
--rw-r--r--   0        0        0     1577 2023-08-04 20:19:19.970709 nbproject-0.9.1/docs/faq/set-env-via-environment-var.ipynb
--rw-r--r--   0        0        0      679 2022-10-10 14:54:28.366976 nbproject-0.9.1/docs/faq/setup.md
--rw-r--r--   0        0        0     1357 2023-08-04 20:19:19.971363 nbproject-0.9.1/docs/faq/trigger-exit-upon-init.ipynb
--rw-r--r--   0        0        0      317 2023-08-04 20:32:42.823391 nbproject-0.9.1/docs/guide.md
--rw-r--r--   0        0        0     2694 2023-08-04 20:19:19.971912 nbproject-0.9.1/docs/guide/basic-metadata.ipynb
--rw-r--r--   0        0        0     4639 2023-08-04 20:19:19.972453 nbproject-0.9.1/docs/guide/meta.ipynb
--rw-r--r--   0        0        0     1637 2023-08-04 20:19:19.972875 nbproject-0.9.1/docs/guide/received.ipynb
--rw-r--r--   0        0        0     2964 2023-08-04 20:19:19.973146 nbproject-0.9.1/docs/guide/update-metadata.ipynb
--rw-r--r--   0        0        0      130 2023-08-04 20:32:42.823650 nbproject-0.9.1/docs/index.md
--rw-r--r--   0        0        0     2755 2023-08-04 20:19:19.973501 nbproject-0.9.1/docs/quickstart.ipynb
--rw-r--r--   0        0        0       57 2023-04-17 07:11:01.413670 nbproject-0.9.1/docs/reference.md
--rw-r--r--   0        0        0      137 2022-06-01 14:27:38.468097 nbproject-0.9.1/lamin-project.yaml
--rw-r--r--   0        0        0      763 2023-08-04 20:33:32.020959 nbproject-0.9.1/nbproject/__init__.py
--rw-r--r--   0        0        0     1631 2022-08-17 11:48:35.494040 nbproject-0.9.1/nbproject/__main__.py
--rw-r--r--   0        0        0     5121 2022-11-12 18:33:53.216715 nbproject-0.9.1/nbproject/_cli.py
--rw-r--r--   0        0        0     5756 2023-07-02 08:17:43.608229 nbproject-0.9.1/nbproject/_header.py
--rw-r--r--   0        0        0      285 2022-11-13 23:00:04.437788 nbproject-0.9.1/nbproject/_is_run_from_ipython.py
--rw-r--r--   0        0        0       47 2023-08-04 20:32:42.823933 nbproject-0.9.1/nbproject/_logger.py
--rw-r--r--   0        0        0     3080 2022-10-10 12:03:49.455892 nbproject-0.9.1/nbproject/_meta.py
--rw-r--r--   0        0        0     3943 2022-11-12 18:52:44.680900 nbproject-0.9.1/nbproject/_publish.py
--rw-r--r--   0        0        0     4007 2022-11-12 18:33:53.217134 nbproject-0.9.1/nbproject/_schemas.py
--rw-r--r--   0        0        0      836 2023-06-04 20:57:48.693471 nbproject-0.9.1/nbproject/dev/__init__.py
--rw-r--r--   0        0        0      590 2022-10-07 21:00:16.805272 nbproject-0.9.1/nbproject/dev/_check_last_cell.py
--rw-r--r--   0        0        0      681 2022-08-17 11:48:35.496655 nbproject-0.9.1/nbproject/dev/_classic_nb_commands.py
--rw-r--r--   0        0        0     1473 2023-06-04 20:57:48.693977 nbproject-0.9.1/nbproject/dev/_consecutiveness.py
--rw-r--r--   0        0        0      525 2022-08-17 11:48:35.496751 nbproject-0.9.1/nbproject/dev/_frontend_commands.py
--rw-r--r--   0        0        0     1843 2023-06-04 20:57:48.694457 nbproject-0.9.1/nbproject/dev/_initialize.py
--rw-r--r--   0        0        0     5137 2023-06-13 15:37:27.141838 nbproject-0.9.1/nbproject/dev/_jupyter_communicate.py
--rw-r--r--   0        0        0      822 2023-04-17 07:11:01.415333 nbproject-0.9.1/nbproject/dev/_jupyter_lab_commands.py
--rw-r--r--   0        0        0      343 2023-04-17 07:11:01.415771 nbproject-0.9.1/nbproject/dev/_lamin_communicate.py
--rw-r--r--   0        0        0     3642 2022-10-10 18:44:26.046429 nbproject-0.9.1/nbproject/dev/_meta_live.py
--rw-r--r--   0        0        0     4541 2022-11-12 18:33:53.217570 nbproject-0.9.1/nbproject/dev/_meta_store.py
--rw-r--r--   0        0        0     5242 2023-06-15 19:08:05.361229 nbproject-0.9.1/nbproject/dev/_metadata_display.py
--rw-r--r--   0        0        0      922 2022-07-15 19:53:53.061564 nbproject-0.9.1/nbproject/dev/_notebook.py
--rw-r--r--   0        0        0     3900 2022-07-23 14:31:43.204220 nbproject-0.9.1/nbproject/dev/_pypackage.py
--rw-r--r--   0        0        0      575 2022-11-12 18:52:44.681103 nbproject-0.9.1/nbproject/dev/_set_version.py
--rw-r--r--   0        0        0      483 2023-08-04 19:43:05.490269 nbproject-0.9.1/noxfile.py
--rw-r--r--   0        0        0     1076 2023-08-04 20:32:42.824213 nbproject-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      920 2022-09-06 11:40:41.175303 nbproject-0.9.1/tests/conftest.py
--rw-r--r--   0        0        0     2428 2022-09-06 11:40:41.175526 nbproject-0.9.1/tests/test_cli.py
--rw-r--r--   0        0        0     1472 2023-04-17 07:11:01.416978 nbproject-0.9.1/tests/test_jupyter.py
--rw-r--r--   0        0        0      322 2023-06-04 20:57:48.695931 nbproject-0.9.1/tests/test_notebooks.py
--rw-r--r--   0        0        0      303 2022-11-12 18:52:44.681259 nbproject-0.9.1/tests/test_set_version.py
--rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 nbproject-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2196 2023-08-15 11:21:22.548025 nbproject-0.9.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-06-10 19:50:58.313927 nbproject-0.9.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-06-10 19:50:58.314964 nbproject-0.9.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1880 2022-07-10 12:10:29.382368 nbproject-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1645 2022-08-29 09:33:05.135542 nbproject-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      740 2022-10-24 12:29:45.346974 nbproject-0.9.2/CITATION.cff
+-rw-r--r--   0        0        0    11357 2022-04-18 20:46:44.681265 nbproject-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1374 2023-08-04 20:32:42.822118 nbproject-0.9.2/README.md
+-rw-r--r--   0        0        0    21101 2023-08-15 11:22:32.234212 nbproject-0.9.2/docs/changelog.md
+-rw-r--r--   0        0        0     1285 2023-08-15 11:21:22.548236 nbproject-0.9.2/docs/faq.md
+-rw-r--r--   0        0        0     1874 2023-08-04 20:19:19.961650 nbproject-0.9.2/docs/faq/example-after-init-set-filename.ipynb
+-rw-r--r--   0        0        0      153 2023-08-04 20:32:42.823012 nbproject-0.9.2/docs/faq/example-project-uninitialized.md
+-rw-r--r--   0        0        0     1481 2023-08-04 20:19:19.962250 nbproject-0.9.2/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb
+-rw-r--r--   0        0        0      117 2023-08-04 20:32:42.823159 nbproject-0.9.2/docs/faq/example-project.md
+-rw-r--r--   0        0        0     1874 2023-08-04 20:19:19.963880 nbproject-0.9.2/docs/faq/example-project/2022-05-13-my-task-x.ipynb
+-rw-r--r--   0        0        0     1661 2023-08-04 20:19:19.964730 nbproject-0.9.2/docs/faq/example-project/2022-07-18-my-task-y.ipynb
+-rw-r--r--   0        0        0      364 2023-08-04 20:19:19.965113 nbproject-0.9.2/docs/faq/example-project/nbproject_metadata.yml
+-rw-r--r--   0        0        0     1873 2023-08-04 20:19:19.965699 nbproject-0.9.2/docs/faq/header-author-field.ipynb
+-rw-r--r--   0        0        0     1520 2023-08-04 20:19:19.966010 nbproject-0.9.2/docs/faq/inconsistent-packages-parents-no-store.ipynb
+-rw-r--r--   0        0        0     2330 2023-08-04 20:19:19.966373 nbproject-0.9.2/docs/faq/inconsistent-packages-parents-store.ipynb
+-rw-r--r--   0        0        0     1311 2023-08-04 20:19:19.967100 nbproject-0.9.2/docs/faq/initialize-set-env.ipynb
+-rw-r--r--   0        0        0     1874 2023-08-15 11:21:22.548394 nbproject-0.9.2/docs/faq/initialize.ipynb
+-rw-r--r--   0        0        0     4086 2023-08-04 20:19:19.967960 nbproject-0.9.2/docs/faq/internal-functions.ipynb
+-rw-r--r--   0        0        0     2708 2023-08-04 20:19:19.968582 nbproject-0.9.2/docs/faq/not-initialized.ipynb
+-rw-r--r--   0        0        0     1803 2023-08-04 20:19:19.968950 nbproject-0.9.2/docs/faq/publish-not-last-cell.ipynb
+-rw-r--r--   0        0        0     1399 2023-08-04 20:19:19.969256 nbproject-0.9.2/docs/faq/publish-set-version.ipynb
+-rw-r--r--   0        0        0     1818 2023-08-04 20:19:19.969587 nbproject-0.9.2/docs/faq/publish-without-saving.ipynb
+-rw-r--r--   0        0        0     1632 2023-08-15 11:21:22.548552 nbproject-0.9.2/docs/faq/publish-without-title.ipynb
+-rw-r--r--   0        0        0     1653 2023-08-04 20:19:19.970180 nbproject-0.9.2/docs/faq/publish-wrapper.ipynb
+-rw-r--r--   0        0        0     1577 2023-08-04 20:19:19.970709 nbproject-0.9.2/docs/faq/set-env-via-environment-var.ipynb
+-rw-r--r--   0        0        0      679 2022-10-10 14:54:28.366976 nbproject-0.9.2/docs/faq/setup.md
+-rw-r--r--   0        0        0     1523 2023-08-15 11:21:22.548666 nbproject-0.9.2/docs/faq/title-not-at-top.ipynb
+-rw-r--r--   0        0        0     1357 2023-08-04 20:19:19.971363 nbproject-0.9.2/docs/faq/trigger-exit-upon-init.ipynb
+-rw-r--r--   0        0        0      317 2023-08-04 20:32:42.823391 nbproject-0.9.2/docs/guide.md
+-rw-r--r--   0        0        0     2694 2023-08-04 20:19:19.971912 nbproject-0.9.2/docs/guide/basic-metadata.ipynb
+-rw-r--r--   0        0        0     4639 2023-08-04 20:19:19.972453 nbproject-0.9.2/docs/guide/meta.ipynb
+-rw-r--r--   0        0        0     1637 2023-08-04 20:19:19.972875 nbproject-0.9.2/docs/guide/received.ipynb
+-rw-r--r--   0        0        0     2964 2023-08-04 20:19:19.973146 nbproject-0.9.2/docs/guide/update-metadata.ipynb
+-rw-r--r--   0        0        0      130 2023-08-04 20:32:42.823650 nbproject-0.9.2/docs/index.md
+-rw-r--r--   0        0        0     2755 2023-08-04 20:19:19.973501 nbproject-0.9.2/docs/quickstart.ipynb
+-rw-r--r--   0        0        0       57 2023-04-17 07:11:01.413670 nbproject-0.9.2/docs/reference.md
+-rw-r--r--   0        0        0      137 2022-06-01 14:27:38.468097 nbproject-0.9.2/lamin-project.yaml
+-rw-r--r--   0        0        0      763 2023-08-15 11:22:27.880032 nbproject-0.9.2/nbproject/__init__.py
+-rw-r--r--   0        0        0     1631 2022-08-17 11:48:35.494040 nbproject-0.9.2/nbproject/__main__.py
+-rw-r--r--   0        0        0     5121 2022-11-12 18:33:53.216715 nbproject-0.9.2/nbproject/_cli.py
+-rw-r--r--   0        0        0     5756 2023-07-02 08:17:43.608229 nbproject-0.9.2/nbproject/_header.py
+-rw-r--r--   0        0        0      285 2022-11-13 23:00:04.437788 nbproject-0.9.2/nbproject/_is_run_from_ipython.py
+-rw-r--r--   0        0        0       47 2023-08-04 20:32:42.823933 nbproject-0.9.2/nbproject/_logger.py
+-rw-r--r--   0        0        0     3080 2022-10-10 12:03:49.455892 nbproject-0.9.2/nbproject/_meta.py
+-rw-r--r--   0        0        0     3943 2022-11-12 18:52:44.680900 nbproject-0.9.2/nbproject/_publish.py
+-rw-r--r--   0        0        0     4007 2022-11-12 18:33:53.217134 nbproject-0.9.2/nbproject/_schemas.py
+-rw-r--r--   0        0        0      836 2023-06-04 20:57:48.693471 nbproject-0.9.2/nbproject/dev/__init__.py
+-rw-r--r--   0        0        0      590 2022-10-07 21:00:16.805272 nbproject-0.9.2/nbproject/dev/_check_last_cell.py
+-rw-r--r--   0        0        0      681 2022-08-17 11:48:35.496655 nbproject-0.9.2/nbproject/dev/_classic_nb_commands.py
+-rw-r--r--   0        0        0     1473 2023-06-04 20:57:48.693977 nbproject-0.9.2/nbproject/dev/_consecutiveness.py
+-rw-r--r--   0        0        0      525 2022-08-17 11:48:35.496751 nbproject-0.9.2/nbproject/dev/_frontend_commands.py
+-rw-r--r--   0        0        0     1843 2023-06-04 20:57:48.694457 nbproject-0.9.2/nbproject/dev/_initialize.py
+-rw-r--r--   0        0        0     5137 2023-06-13 15:37:27.141838 nbproject-0.9.2/nbproject/dev/_jupyter_communicate.py
+-rw-r--r--   0        0        0      822 2023-04-17 07:11:01.415333 nbproject-0.9.2/nbproject/dev/_jupyter_lab_commands.py
+-rw-r--r--   0        0        0      343 2023-04-17 07:11:01.415771 nbproject-0.9.2/nbproject/dev/_lamin_communicate.py
+-rw-r--r--   0        0        0     3864 2023-08-15 11:21:22.548843 nbproject-0.9.2/nbproject/dev/_meta_live.py
+-rw-r--r--   0        0        0     4541 2022-11-12 18:33:53.217570 nbproject-0.9.2/nbproject/dev/_meta_store.py
+-rw-r--r--   0        0        0     5242 2023-06-15 19:08:05.361229 nbproject-0.9.2/nbproject/dev/_metadata_display.py
+-rw-r--r--   0        0        0      922 2022-07-15 19:53:53.061564 nbproject-0.9.2/nbproject/dev/_notebook.py
+-rw-r--r--   0        0        0     3900 2022-07-23 14:31:43.204220 nbproject-0.9.2/nbproject/dev/_pypackage.py
+-rw-r--r--   0        0        0      575 2022-11-12 18:52:44.681103 nbproject-0.9.2/nbproject/dev/_set_version.py
+-rw-r--r--   0        0        0      437 2023-08-15 11:21:22.548982 nbproject-0.9.2/noxfile.py
+-rw-r--r--   0        0        0     1091 2023-08-15 11:21:22.549131 nbproject-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      920 2022-09-06 11:40:41.175303 nbproject-0.9.2/tests/conftest.py
+-rw-r--r--   0        0        0     2428 2022-09-06 11:40:41.175526 nbproject-0.9.2/tests/test_cli.py
+-rw-r--r--   0        0        0     1472 2023-04-17 07:11:01.416978 nbproject-0.9.2/tests/test_jupyter.py
+-rw-r--r--   0        0        0      322 2023-06-04 20:57:48.695931 nbproject-0.9.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0      303 2022-11-12 18:52:44.681259 nbproject-0.9.2/tests/test_set_version.py
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 nbproject-0.9.2/PKG-INFO
```

### Comparing `nbproject-0.9.1/.github/workflows/build.yml` & `nbproject-0.9.2/.github/workflows/build.yml`

 * *Files 15% similar despite different names*

```diff
@@ -42,35 +42,27 @@
         with:
           path: ~/.cache/pre-commit
           key: pre-commit-${{ runner.os }}-${{ hashFiles('.pre-commit-config.yaml') }}
       - name: Install Python dependencies
         run: |
           python -m pip install -U pip
           pip install -U laminci
-          pip install -U lamindb
       - name: Configure AWS
         uses: aws-actions/configure-aws-credentials@v2
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
       # - run: nox -s lint
       - run: nox -s build
       - name: Codecov
         if: matrix.python-version == '3.9'
         uses: codecov/codecov-action@v2
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
-      - name: Read lamin-project.yaml
-        if: matrix.python-version == '3.9'
-        id: lamin-project
-        uses: CumulusDS/get-yaml-paths-action@v0.1.0
-        with:
-          file: lamin-project.yaml
-          project_slug: project_slug
       - name: Deploy docs
         if: matrix.python-version == '3.9'
         id: netlify
         uses: nwtgck/actions-netlify@v1.2
         with:
           publish-dir: "_build/html"
           production-deploy: ${{ github.event_name == 'push' }}
```

### Comparing `nbproject-0.9.1/.github/workflows/latest-changes.yml` & `nbproject-0.9.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/.gitignore` & `nbproject-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/.pre-commit-config.yaml` & `nbproject-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/CITATION.cff` & `nbproject-0.9.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/LICENSE` & `nbproject-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/README.md` & `nbproject-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/changelog.md` & `nbproject-0.9.2/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚸 More robust title parsing | [270](https://github.com/laminlabs/nbproject/pull/270) | [falexwolf](https://github.com/falexwolf) | 2023-08-15 | 0.9.2
 📝 Simplify docs, adopt new lamin.ai static site architecture | [269](https://github.com/laminlabs/nbproject/pull/269) | [falexwolf](https://github.com/falexwolf) | 2023-08-04 | 0.9.1
 ♻️ Remove loguru-dependent call, expand `metadata_only` return signature | [268](https://github.com/laminlabs/nbproject/pull/268) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.9.0
 📝 Position nbproject | [264](https://github.com/laminlabs/nbproject/pull/264) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 |
 🩹 Try to get vs code path first | [267](https://github.com/laminlabs/nbproject/pull/267) | [Koncopd](https://github.com/Koncopd) | 2023-06-10 |
 🦺 Safer parsing during initialization | [266](https://github.com/laminlabs/nbproject/pull/266) | [Koncopd](https://github.com/Koncopd) | 2023-06-03 | 0.8.7
 ➖ Remove nbproject-test from dependencies | [262](https://github.com/laminlabs/nbproject/pull/262) | [Koncopd](https://github.com/Koncopd) | 2023-05-30 |
 🐛 Safer ipylab initialization | [263](https://github.com/laminlabs/nbproject/pull/263) | [Koncopd](https://github.com/Koncopd) | 2023-04-18 | 0.8.6
```

### Comparing `nbproject-0.9.1/docs/faq.md` & `nbproject-0.9.2/docs/faq.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 - {doc}`faq/initialize-set-env`
 - {doc}`faq/inconsistent-packages-parents-store`
 - {doc}`faq/inconsistent-packages-parents-no-store`
 - {doc}`faq/example-project`
 - {doc}`faq/example-project-uninitialized`
 - {doc}`faq/example-after-init-set-filename`
 - {doc}`faq/publish-set-version`
-- {doc}`faq/publish-without-title`
+- [Publish without title](faq/publish-without-title)
 - {doc}`faq/publish-without-saving`
 - {doc}`faq/publish-not-last-cell`
+- {doc}`faq/title-not-at-top`
 - {doc}`faq/publish-wrapper`
 - {doc}`faq/trigger-exit-upon-init`
 - {doc}`faq/not-initialized`
 - {doc}`faq/internal-functions`
 - {doc}`faq/set-env-via-environment-var`
 - {doc}`faq/header-author-field`
 
@@ -37,13 +38,14 @@
 faq/example-project-uninitialized
 faq/example-after-init-set-filename
 faq/publish-set-version
 faq/publish-without-title
 faq/publish-without-saving
 faq/publish-not-last-cell
 faq/publish-wrapper
+faq/title-not-at-top
 faq/trigger-exit-upon-init
 faq/not-initialized
 faq/internal-functions
 faq/set-env-via-environment-var
 faq/header-author-field
 ```
```

### Comparing `nbproject-0.9.1/docs/faq/example-after-init-set-filename.ipynb` & `nbproject-0.9.2/docs/faq/example-after-init-set-filename.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb` & `nbproject-0.9.2/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/example-project/2022-05-13-my-task-x.ipynb` & `nbproject-0.9.2/docs/faq/example-project/2022-05-13-my-task-x.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/example-project/2022-07-18-my-task-y.ipynb` & `nbproject-0.9.2/docs/faq/example-project/2022-07-18-my-task-y.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/header-author-field.ipynb` & `nbproject-0.9.2/docs/faq/header-author-field.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/inconsistent-packages-parents-no-store.ipynb` & `nbproject-0.9.2/docs/faq/inconsistent-packages-parents-no-store.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/inconsistent-packages-parents-store.ipynb` & `nbproject-0.9.2/docs/faq/inconsistent-packages-parents-store.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/initialize-set-env.ipynb` & `nbproject-0.9.2/docs/faq/initialize-set-env.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/initialize.ipynb` & `nbproject-0.9.2/docs/faq/initialize.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'cells'": "{3: {'source': {delete: [11, 10, 9, 8, 7, 6]}}}"}*

```diff
@@ -30,20 +30,14 @@
                 "```{important}\n",
                 "\n",
                 "- You'll have the best interactive experience in **Jupyter Lab**.\n",
                 "- In other editors, you'll need to manually hit save and reload the changed `.ipynb` file from disk (discard the editor content).\n",
                 "\n",
                 "We recommend you use Jupyter Lab for a seamless interactive experience.\n",
                 "\n",
-                "```\n",
-                "\n",
-                "```{hint}\n",
-                "\n",
-                "If you instead want to bulk-initialize a whole folder with notebooks, use the CLI: {doc}`../guide/cli`.\n",
-                "\n",
                 "```"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.9.12 ('base1')",
```

### Comparing `nbproject-0.9.1/docs/faq/internal-functions.ipynb` & `nbproject-0.9.2/docs/faq/internal-functions.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/not-initialized.ipynb` & `nbproject-0.9.2/docs/faq/not-initialized.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/publish-not-last-cell.ipynb` & `nbproject-0.9.2/docs/faq/publish-not-last-cell.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/publish-set-version.ipynb` & `nbproject-0.9.2/docs/faq/publish-set-version.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/publish-without-saving.ipynb` & `nbproject-0.9.2/docs/faq/publish-without-saving.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/publish-without-title.ipynb` & `nbproject-0.9.2/docs/faq/publish-without-title.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'cells'": '{delete: [1]}'}*

```diff
@@ -5,22 +5,14 @@
             "id": "37b372a5-fae0-4177-986f-0adeea86158f",
             "metadata": {},
             "source": [
                 "This notebooks shows how a warning and an error is raised when there is no title in the first cell."
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "411d20ca-f637-4d3f-9047-1b5782b1d7ea",
-            "metadata": {},
-            "source": [
-                "# Publish without title"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "id": "d55181fa-9114-473b-a38d-27349d267f90",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from nbproject import header, meta, publish\n",
```

### Comparing `nbproject-0.9.1/docs/faq/publish-wrapper.ipynb` & `nbproject-0.9.2/docs/faq/publish-wrapper.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/set-env-via-environment-var.ipynb` & `nbproject-0.9.2/docs/faq/set-env-via-environment-var.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/setup.md` & `nbproject-0.9.2/docs/faq/setup.md`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/faq/trigger-exit-upon-init.ipynb` & `nbproject-0.9.2/docs/faq/trigger-exit-upon-init.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/guide/basic-metadata.ipynb` & `nbproject-0.9.2/docs/guide/basic-metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/guide/meta.ipynb` & `nbproject-0.9.2/docs/guide/meta.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/guide/received.ipynb` & `nbproject-0.9.2/docs/guide/received.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/guide/update-metadata.ipynb` & `nbproject-0.9.2/docs/guide/update-metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/docs/quickstart.ipynb` & `nbproject-0.9.2/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/__init__.py` & `nbproject-0.9.2/nbproject/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 .. autosummary::
    :toctree:
 
    meta
    dev
 
 """
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 # init jupyter lab frontend immediately on import
 # nothing happens if this is not jupyter lab
 from .dev._jupyter_lab_commands import _init_frontend
 
 # trying to init ipylab JupyterFrontEnd can lead to errors on jupyter notebook
 try:
```

### Comparing `nbproject-0.9.1/nbproject/__main__.py` & `nbproject-0.9.2/nbproject/__main__.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/_cli.py` & `nbproject-0.9.2/nbproject/_cli.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/_header.py` & `nbproject-0.9.2/nbproject/_header.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/_meta.py` & `nbproject-0.9.2/nbproject/_meta.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/_publish.py` & `nbproject-0.9.2/nbproject/_publish.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/_schemas.py` & `nbproject-0.9.2/nbproject/_schemas.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/__init__.py` & `nbproject-0.9.2/nbproject/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_check_last_cell.py` & `nbproject-0.9.2/nbproject/dev/_check_last_cell.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_classic_nb_commands.py` & `nbproject-0.9.2/nbproject/dev/_classic_nb_commands.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_consecutiveness.py` & `nbproject-0.9.2/nbproject/dev/_consecutiveness.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_frontend_commands.py` & `nbproject-0.9.2/nbproject/dev/_frontend_commands.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_initialize.py` & `nbproject-0.9.2/nbproject/dev/_initialize.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_jupyter_communicate.py` & `nbproject-0.9.2/nbproject/dev/_jupyter_communicate.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_jupyter_lab_commands.py` & `nbproject-0.9.2/nbproject/dev/_jupyter_lab_commands.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_meta_live.py` & `nbproject-0.9.2/nbproject/dev/_meta_live.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 from ._lamin_communicate import lamin_user_settings
 from ._notebook import Notebook, read_notebook
 from ._pypackage import infer_pypackages
 
 
 def get_title(nb: Notebook) -> Optional[str]:
     """Get title of the notebook."""
-    if nb.cells[0]["cell_type"] != "markdown":
-        title = None
-    else:
-        title = nb.cells[0]["source"][0]
-        if not title.startswith("# "):
-            title = None
-        else:
-            title = title.lstrip("#").strip(" .").strip("\n")
-    return title
+    # loop through all cells
+    for cell in nb.cells:
+        # only consider markdown
+        if cell["cell_type"] == "markdown":
+            # grab source
+            text = cell["source"][0]
+            # loop through lines
+            for line in text.split("\n"):
+                # if finding a level-1 heading, consider it a title
+                if line.startswith("# "):
+                    title = line.lstrip("#").strip(" .").strip("\n")
+                    return title
+    return None
 
 
 class MetaLive:
     """Live properties of the notebook.
 
     All attributes represent either the execution information or properties inferred
     on access from the notebook's content.
```

### Comparing `nbproject-0.9.1/nbproject/dev/_meta_store.py` & `nbproject-0.9.2/nbproject/dev/_meta_store.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_metadata_display.py` & `nbproject-0.9.2/nbproject/dev/_metadata_display.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_notebook.py` & `nbproject-0.9.2/nbproject/dev/_notebook.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_pypackage.py` & `nbproject-0.9.2/nbproject/dev/_pypackage.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/nbproject/dev/_set_version.py` & `nbproject-0.9.2/nbproject/dev/_set_version.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/pyproject.toml` & `nbproject-0.9.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "pre-commit",
     "black",
     "pytest>=6.0",
     "pytest-cov",
     "pandas",
     "nbformat",
     "nbproject_test >= 0.4.5",
+    "laminci",
 ]
 
 [project.scripts]
 nbproject = "nbproject.__main__:main"
 
 [tool.black]
 preview = true
```

### Comparing `nbproject-0.9.1/tests/conftest.py` & `nbproject-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/tests/test_cli.py` & `nbproject-0.9.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/tests/test_jupyter.py` & `nbproject-0.9.2/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.1/PKG-INFO` & `nbproject-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbproject
-Version: 0.9.1
+Version: 0.9.2
 Summary: nbproject: Manage Jupyter notebooks.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,14 +19,15 @@
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pandas ; extra == "dev"
 Requires-Dist: nbformat ; extra == "dev"
 Requires-Dist: nbproject_test >= 0.4.5 ; extra == "dev"
+Requires-Dist: laminci ; extra == "dev"
 Project-URL: Home, https://github.com/laminlabs/nbproject
 Provides-Extra: dev
 
 [![Stars](https://img.shields.io/github/stars/laminlabs/nbproject?logo=GitHub&color=yellow)](https://github.com/laminlabs/nbproject)
 [![coverage](https://codecov.io/gh/laminlabs/nbproject/branch/main/graph/badge.svg?token=05R04PR9RB)](https://codecov.io/gh/laminlabs/nbproject)
 [![pypi](https://img.shields.io/pypi/v/nbproject?color=blue&label=pypi%20package)](https://pypi.org/project/nbproject)
 [![doi](https://img.shields.io/badge/doi-10.56528%2Fnbp-lightgrey)](https://doi.org/10.56528/nbp)
```

