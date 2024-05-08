# Comparing `tmp/xbrl-us-0.0.42.tar.gz` & `tmp/xbrl-us-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbrl-us-0.0.42.tar", last modified: Fri Mar 29 23:12:00 2024, max compression
+gzip compressed data, was "xbrl-us-0.0.43.tar", last modified: Wed May  8 13:48:22 2024, max compression
```

## Comparing `xbrl-us-0.0.42.tar` & `xbrl-us-0.0.43.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.306252 xbrl-us-0.0.42/
--rw-r--r--   0 hamid      (501) staff       (20)      528 2024-03-29 22:54:37.000000 xbrl-us-0.0.42/.bumpversion.cfg
--rw-r--r--   0 hamid      (501) staff       (20)     2016 2024-03-29 22:54:37.000000 xbrl-us-0.0.42/.cookiecutterrc
--rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/.coveragerc
--rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/.editorconfig
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.291375 xbrl-us-0.0.42/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.294940 xbrl-us-0.0.42/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     3400 2023-07-14 19:39:33.000000 xbrl-us-0.0.42/.github/workflows/github-actions.yml
--rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.42/.pre-commit-config.yaml
--rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.42/.readthedocs.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1006 2024-03-29 22:51:51.000000 xbrl-us-0.0.42/CHANGELOG.rst
--rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/CONTRIBUTING.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.42/LICENSE
--rw-r--r--   0 hamid      (501) staff       (20)      457 2023-07-14 18:26:55.000000 xbrl-us-0.0.42/MANIFEST.in
--rw-r--r--   0 hamid      (501) staff       (20)    13951 2024-03-29 23:12:00.306029 xbrl-us-0.0.42/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)    11606 2023-07-18 17:14:45.000000 xbrl-us-0.0.42/README.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.295237 xbrl-us-0.0.42/ci/
--rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/ci/bootstrap.py
--rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/ci/requirements.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.291617 xbrl-us-0.0.42/ci/templates/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.291674 xbrl-us-0.0.42/ci/templates/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.295390 xbrl-us-0.0.42/ci/templates/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.296374 xbrl-us-0.0.42/docs/
--rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/docs/changelog.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1156 2024-03-29 22:54:37.000000 xbrl-us-0.0.42/docs/conf.py
--rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/docs/contributing.rst
--rw-r--r--   0 hamid      (501) staff       (20)      208 2023-07-17 22:11:31.000000 xbrl-us-0.0.42/docs/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)    10882 2023-07-19 13:02:53.000000 xbrl-us-0.0.42/docs/readme.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.296684 xbrl-us-0.0.42/docs/reference/
--rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.42/docs/reference/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.42/docs/reference/xbrl_us.rst
--rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.42/docs/requirements.txt
--rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/docs/spelling_wordlist.txt
--rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.42/pyproject.toml
--rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.42/pytest.ini
--rw-r--r--   0 hamid      (501) staff       (20)       54 2023-07-14 18:22:29.000000 xbrl-us-0.0.42/secrets.yml
--rw-r--r--   0 hamid      (501) staff       (20)       38 2024-03-29 23:12:00.306322 xbrl-us-0.0.42/setup.cfg
--rwxr-xr-x   0 hamid      (501) staff       (20)     3004 2024-03-29 22:54:37.000000 xbrl-us-0.0.42/setup.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.292048 xbrl-us-0.0.42/src/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.297483 xbrl-us-0.0.42/src/xbrl_us/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.298874 xbrl-us-0.0.42/src/xbrl_us/.streamlit/
--rw-r--r--   0 hamid      (501) staff       (20)      130 2023-11-01 18:34:08.000000 xbrl-us-0.0.42/src/xbrl_us/.streamlit/config.toml
--rw-r--r--   0 hamid      (501) staff       (20)       70 2024-03-29 22:54:37.000000 xbrl-us-0.0.42/src/xbrl_us/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.42/src/xbrl_us/__main__.py
--rw-r--r--   0 hamid      (501) staff       (20)    18316 2024-03-29 22:51:39.000000 xbrl-us-0.0.42/src/xbrl_us/app.py
--rw-r--r--   0 hamid      (501) staff       (20)      373 2023-08-03 21:05:17.000000 xbrl-us-0.0.42/src/xbrl_us/cli.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.303395 xbrl-us-0.0.42/src/xbrl_us/methods/
--rw-r--r--   0 hamid      (501) staff       (20)    12479 2023-08-04 01:52:45.000000 xbrl-us-0.0.42/src/xbrl_us/methods/_definitions.yaml
--rw-r--r--   0 hamid      (501) staff       (20)     1122 2023-08-21 09:18:39.000000 xbrl-us-0.0.42/src/xbrl_us/methods/assertion search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.42/src/xbrl_us/methods/assertion validate.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1569 2023-08-22 08:02:53.000000 xbrl-us-0.0.42/src/xbrl_us/methods/concept name search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1898 2023-08-22 08:01:50.000000 xbrl-us-0.0.42/src/xbrl_us/methods/concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1541 2023-08-22 07:58:28.000000 xbrl-us-0.0.42/src/xbrl_us/methods/cube search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1296 2023-08-22 07:58:03.000000 xbrl-us-0.0.42/src/xbrl_us/methods/dimension search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1214 2023-08-22 07:57:32.000000 xbrl-us-0.0.42/src/xbrl_us/methods/document search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      683 2023-08-21 16:41:08.000000 xbrl-us-0.0.42/src/xbrl_us/methods/dts id concept label.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1173 2023-08-21 16:41:08.000000 xbrl-us-0.0.42/src/xbrl_us/methods/dts id concept name.yml
--rw-r--r--   0 hamid      (501) staff       (20)      786 2023-08-21 16:41:08.000000 xbrl-us-0.0.42/src/xbrl_us/methods/dts id concept reference.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1123 2023-08-21 16:39:05.000000 xbrl-us-0.0.42/src/xbrl_us/methods/dts id concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1476 2023-08-21 16:39:05.000000 xbrl-us-0.0.42/src/xbrl_us/methods/dts id network search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1050 2023-08-21 16:39:05.000000 xbrl-us-0.0.42/src/xbrl_us/methods/dts id network.yml
--rw-r--r--   0 hamid      (501) staff       (20)      750 2023-08-21 16:36:56.000000 xbrl-us-0.0.42/src/xbrl_us/methods/dts search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1684 2023-08-21 09:07:51.000000 xbrl-us-0.0.42/src/xbrl_us/methods/entity id report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      451 2023-08-21 09:07:51.000000 xbrl-us-0.0.42/src/xbrl_us/methods/entity id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1728 2023-08-21 09:07:51.000000 xbrl-us-0.0.42/src/xbrl_us/methods/entity report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      486 2023-08-21 09:07:51.000000 xbrl-us-0.0.42/src/xbrl_us/methods/entity search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2013 2023-08-21 08:38:08.000000 xbrl-us-0.0.42/src/xbrl_us/methods/fact id.yml
--rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.42/src/xbrl_us/methods/fact search oim.yml
--rw-r--r--   0 hamid      (501) staff       (20)     3010 2023-08-21 08:38:08.000000 xbrl-us-0.0.42/src/xbrl_us/methods/fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      833 2023-08-21 16:56:52.000000 xbrl-us-0.0.42/src/xbrl_us/methods/label dts id search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      814 2023-08-21 16:56:52.000000 xbrl-us-0.0.42/src/xbrl_us/methods/label search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1454 2023-08-21 17:06:46.000000 xbrl-us-0.0.42/src/xbrl_us/methods/network id relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      449 2023-08-21 17:06:46.000000 xbrl-us-0.0.42/src/xbrl_us/methods/network id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1368 2023-08-21 17:06:46.000000 xbrl-us-0.0.42/src/xbrl_us/methods/network relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1386 2023-08-22 07:38:51.000000 xbrl-us-0.0.42/src/xbrl_us/methods/relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1069 2023-08-22 07:38:51.000000 xbrl-us-0.0.42/src/xbrl_us/methods/relationship tree search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     3890 2023-08-09 00:47:51.000000 xbrl-us-0.0.42/src/xbrl_us/methods/report fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.42/src/xbrl_us/methods/report id delete.yml
--rw-r--r--   0 hamid      (501) staff       (20)     3683 2023-08-04 21:40:49.000000 xbrl-us-0.0.42/src/xbrl_us/methods/report id fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1247 2023-08-04 20:05:33.000000 xbrl-us-0.0.42/src/xbrl_us/methods/report id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1673 2023-08-04 17:49:09.000000 xbrl-us-0.0.42/src/xbrl_us/methods/report search.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.305016 xbrl-us-0.0.42/src/xbrl_us/schemas/
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/assertion_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/concept_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/cube_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/dimension_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/document_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/dts_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/entity_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/fact_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/label_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/network_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/relationship_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.42/src/xbrl_us/schemas/report_details.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.305556 xbrl-us-0.0.42/src/xbrl_us/utils/
--rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.42/src/xbrl_us/utils/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)     1633 2023-07-16 19:19:32.000000 xbrl-us-0.0.42/src/xbrl_us/utils/exceptions.py
--rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.42/src/xbrl_us/utils/fields.py
--rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.42/src/xbrl_us/utils/paramters.py
--rw-r--r--   0 hamid      (501) staff       (20)    31511 2024-03-29 22:42:57.000000 xbrl-us-0.0.42/src/xbrl_us/xbrl_us.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.298735 xbrl-us-0.0.42/src/xbrl_us.egg-info/
--rw-r--r--   0 hamid      (501) staff       (20)    13951 2024-03-29 23:12:00.000000 xbrl-us-0.0.42/src/xbrl_us.egg-info/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)     2971 2024-03-29 23:12:00.000000 xbrl-us-0.0.42/src/xbrl_us.egg-info/SOURCES.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2024-03-29 23:12:00.000000 xbrl-us-0.0.42/src/xbrl_us.egg-info/dependency_links.txt
--rw-r--r--   0 hamid      (501) staff       (20)       45 2024-03-29 23:12:00.000000 xbrl-us-0.0.42/src/xbrl_us.egg-info/entry_points.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-11-01 19:29:02.000000 xbrl-us-0.0.42/src/xbrl_us.egg-info/not-zip-safe
--rw-r--r--   0 hamid      (501) staff       (20)      103 2024-03-29 23:12:00.000000 xbrl-us-0.0.42/src/xbrl_us.egg-info/requires.txt
--rw-r--r--   0 hamid      (501) staff       (20)        8 2024-03-29 23:12:00.000000 xbrl-us-0.0.42/src/xbrl_us.egg-info/top_level.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-03-29 23:12:00.305762 xbrl-us-0.0.42/tests/
--rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.42/tests/test_xbrl_us.py
--rw-r--r--   0 hamid      (501) staff       (20)     1486 2023-07-14 19:43:01.000000 xbrl-us-0.0.42/tox.ini
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.640071 xbrl-us-0.0.43/
+-rw-r--r--   0 hamid      (501) staff       (20)      528 2024-05-08 13:47:04.000000 xbrl-us-0.0.43/.bumpversion.cfg
+-rw-r--r--   0 hamid      (501) staff       (20)     2016 2024-05-08 13:47:04.000000 xbrl-us-0.0.43/.cookiecutterrc
+-rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/.coveragerc
+-rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/.editorconfig
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.624299 xbrl-us-0.0.43/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.628003 xbrl-us-0.0.43/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     3400 2023-07-14 19:39:33.000000 xbrl-us-0.0.43/.github/workflows/github-actions.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.43/.pre-commit-config.yaml
+-rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.43/.readthedocs.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1006 2024-03-29 22:51:51.000000 xbrl-us-0.0.43/CHANGELOG.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/CONTRIBUTING.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.43/LICENSE
+-rw-r--r--   0 hamid      (501) staff       (20)      457 2023-07-14 18:26:55.000000 xbrl-us-0.0.43/MANIFEST.in
+-rw-r--r--   0 hamid      (501) staff       (20)    13951 2024-05-08 13:48:22.639837 xbrl-us-0.0.43/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)    11606 2023-07-18 17:14:45.000000 xbrl-us-0.0.43/README.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.628306 xbrl-us-0.0.43/ci/
+-rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/ci/bootstrap.py
+-rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/ci/requirements.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.624547 xbrl-us-0.0.43/ci/templates/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.624611 xbrl-us-0.0.43/ci/templates/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.628470 xbrl-us-0.0.43/ci/templates/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.629544 xbrl-us-0.0.43/docs/
+-rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/docs/changelog.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1156 2024-05-08 13:47:04.000000 xbrl-us-0.0.43/docs/conf.py
+-rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/docs/contributing.rst
+-rw-r--r--   0 hamid      (501) staff       (20)      208 2023-07-17 22:11:31.000000 xbrl-us-0.0.43/docs/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)    10882 2023-07-19 13:02:53.000000 xbrl-us-0.0.43/docs/readme.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.629855 xbrl-us-0.0.43/docs/reference/
+-rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.43/docs/reference/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.43/docs/reference/xbrl_us.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.43/docs/requirements.txt
+-rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/docs/spelling_wordlist.txt
+-rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.43/pyproject.toml
+-rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.43/pytest.ini
+-rw-r--r--   0 hamid      (501) staff       (20)       54 2023-07-14 18:22:29.000000 xbrl-us-0.0.43/secrets.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       38 2024-05-08 13:48:22.640121 xbrl-us-0.0.43/setup.cfg
+-rwxr-xr-x   0 hamid      (501) staff       (20)     3004 2024-05-08 13:47:04.000000 xbrl-us-0.0.43/setup.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.625002 xbrl-us-0.0.43/src/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.630653 xbrl-us-0.0.43/src/xbrl_us/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.631882 xbrl-us-0.0.43/src/xbrl_us/.streamlit/
+-rw-r--r--   0 hamid      (501) staff       (20)      130 2023-11-01 18:34:08.000000 xbrl-us-0.0.43/src/xbrl_us/.streamlit/config.toml
+-rw-r--r--   0 hamid      (501) staff       (20)       70 2024-05-08 13:47:04.000000 xbrl-us-0.0.43/src/xbrl_us/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.43/src/xbrl_us/__main__.py
+-rw-r--r--   0 hamid      (501) staff       (20)    18316 2024-03-29 22:51:39.000000 xbrl-us-0.0.43/src/xbrl_us/app.py
+-rw-r--r--   0 hamid      (501) staff       (20)      373 2023-08-03 21:05:17.000000 xbrl-us-0.0.43/src/xbrl_us/cli.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.637287 xbrl-us-0.0.43/src/xbrl_us/methods/
+-rw-r--r--   0 hamid      (501) staff       (20)    12479 2023-08-04 01:52:45.000000 xbrl-us-0.0.43/src/xbrl_us/methods/_definitions.yaml
+-rw-r--r--   0 hamid      (501) staff       (20)     1122 2023-08-21 09:18:39.000000 xbrl-us-0.0.43/src/xbrl_us/methods/assertion search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.43/src/xbrl_us/methods/assertion validate.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1569 2023-08-22 08:02:53.000000 xbrl-us-0.0.43/src/xbrl_us/methods/concept name search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1898 2023-08-22 08:01:50.000000 xbrl-us-0.0.43/src/xbrl_us/methods/concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1541 2023-08-22 07:58:28.000000 xbrl-us-0.0.43/src/xbrl_us/methods/cube search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1296 2023-08-22 07:58:03.000000 xbrl-us-0.0.43/src/xbrl_us/methods/dimension search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1214 2023-08-22 07:57:32.000000 xbrl-us-0.0.43/src/xbrl_us/methods/document search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      683 2023-08-21 16:41:08.000000 xbrl-us-0.0.43/src/xbrl_us/methods/dts id concept label.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1173 2023-08-21 16:41:08.000000 xbrl-us-0.0.43/src/xbrl_us/methods/dts id concept name.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      786 2023-08-21 16:41:08.000000 xbrl-us-0.0.43/src/xbrl_us/methods/dts id concept reference.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1123 2023-08-21 16:39:05.000000 xbrl-us-0.0.43/src/xbrl_us/methods/dts id concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1476 2023-08-21 16:39:05.000000 xbrl-us-0.0.43/src/xbrl_us/methods/dts id network search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1050 2023-08-21 16:39:05.000000 xbrl-us-0.0.43/src/xbrl_us/methods/dts id network.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      750 2023-08-21 16:36:56.000000 xbrl-us-0.0.43/src/xbrl_us/methods/dts search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1684 2023-08-21 09:07:51.000000 xbrl-us-0.0.43/src/xbrl_us/methods/entity id report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      451 2023-08-21 09:07:51.000000 xbrl-us-0.0.43/src/xbrl_us/methods/entity id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1728 2023-08-21 09:07:51.000000 xbrl-us-0.0.43/src/xbrl_us/methods/entity report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      486 2023-08-21 09:07:51.000000 xbrl-us-0.0.43/src/xbrl_us/methods/entity search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2013 2023-08-21 08:38:08.000000 xbrl-us-0.0.43/src/xbrl_us/methods/fact id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.43/src/xbrl_us/methods/fact search oim.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     3010 2023-08-21 08:38:08.000000 xbrl-us-0.0.43/src/xbrl_us/methods/fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      833 2023-08-21 16:56:52.000000 xbrl-us-0.0.43/src/xbrl_us/methods/label dts id search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      814 2023-08-21 16:56:52.000000 xbrl-us-0.0.43/src/xbrl_us/methods/label search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1454 2023-08-21 17:06:46.000000 xbrl-us-0.0.43/src/xbrl_us/methods/network id relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      449 2023-08-21 17:06:46.000000 xbrl-us-0.0.43/src/xbrl_us/methods/network id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1368 2023-08-21 17:06:46.000000 xbrl-us-0.0.43/src/xbrl_us/methods/network relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1386 2023-08-22 07:38:51.000000 xbrl-us-0.0.43/src/xbrl_us/methods/relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1069 2023-08-22 07:38:51.000000 xbrl-us-0.0.43/src/xbrl_us/methods/relationship tree search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     3890 2023-08-09 00:47:51.000000 xbrl-us-0.0.43/src/xbrl_us/methods/report fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.43/src/xbrl_us/methods/report id delete.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     3683 2023-08-04 21:40:49.000000 xbrl-us-0.0.43/src/xbrl_us/methods/report id fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1247 2023-08-04 20:05:33.000000 xbrl-us-0.0.43/src/xbrl_us/methods/report id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1673 2023-08-04 17:49:09.000000 xbrl-us-0.0.43/src/xbrl_us/methods/report search.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.638863 xbrl-us-0.0.43/src/xbrl_us/schemas/
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/assertion_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/concept_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/cube_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/dimension_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/document_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/dts_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/entity_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/fact_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/label_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/network_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/relationship_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.43/src/xbrl_us/schemas/report_details.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.639397 xbrl-us-0.0.43/src/xbrl_us/utils/
+-rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.43/src/xbrl_us/utils/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1633 2023-07-16 19:19:32.000000 xbrl-us-0.0.43/src/xbrl_us/utils/exceptions.py
+-rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.43/src/xbrl_us/utils/fields.py
+-rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.43/src/xbrl_us/utils/paramters.py
+-rw-r--r--   0 hamid      (501) staff       (20)    31514 2024-05-08 13:45:42.000000 xbrl-us-0.0.43/src/xbrl_us/xbrl_us.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.631723 xbrl-us-0.0.43/src/xbrl_us.egg-info/
+-rw-r--r--   0 hamid      (501) staff       (20)    13951 2024-05-08 13:48:22.000000 xbrl-us-0.0.43/src/xbrl_us.egg-info/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)     2971 2024-05-08 13:48:22.000000 xbrl-us-0.0.43/src/xbrl_us.egg-info/SOURCES.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2024-05-08 13:48:22.000000 xbrl-us-0.0.43/src/xbrl_us.egg-info/dependency_links.txt
+-rw-r--r--   0 hamid      (501) staff       (20)       45 2024-05-08 13:48:22.000000 xbrl-us-0.0.43/src/xbrl_us.egg-info/entry_points.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-11-01 19:29:02.000000 xbrl-us-0.0.43/src/xbrl_us.egg-info/not-zip-safe
+-rw-r--r--   0 hamid      (501) staff       (20)      103 2024-05-08 13:48:22.000000 xbrl-us-0.0.43/src/xbrl_us.egg-info/requires.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        8 2024-05-08 13:48:22.000000 xbrl-us-0.0.43/src/xbrl_us.egg-info/top_level.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2024-05-08 13:48:22.639589 xbrl-us-0.0.43/tests/
+-rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.43/tests/test_xbrl_us.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1486 2023-07-14 19:43:01.000000 xbrl-us-0.0.43/tox.ini
```

### Comparing `xbrl-us-0.0.42/.bumpversion.cfg` & `xbrl-us-0.0.43/.bumpversion.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.42
+current_version = 0.0.43
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `xbrl-us-0.0.42/.cookiecutterrc` & `xbrl-us-0.0.43/.cookiecutterrc`

 * *Files 7% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://python-xbrl-us.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "furo"
     test_matrix_separate_coverage: "no"
-    version: "0.0.42"
+    version: "0.0.43"
     version_manager: "bump2version"
     website: "https://hamidvakilzadeh.com"
     year_from: "2023"
     year_to: "2023"
```

### Comparing `xbrl-us-0.0.42/.github/workflows/github-actions.yml` & `xbrl-us-0.0.43/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/.pre-commit-config.yaml` & `xbrl-us-0.0.43/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/CHANGELOG.rst` & `xbrl-us-0.0.43/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/CONTRIBUTING.rst` & `xbrl-us-0.0.43/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/LICENSE` & `xbrl-us-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/PKG-INFO` & `xbrl-us-0.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.42
+Version: 0.0.43
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
```

### Comparing `xbrl-us-0.0.42/README.rst` & `xbrl-us-0.0.43/README.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/ci/bootstrap.py` & `xbrl-us-0.0.43/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/ci/templates/.github/workflows/github-actions.yml` & `xbrl-us-0.0.43/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/docs/conf.py` & `xbrl-us-0.0.43/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "xbrl-us"
 year = "2023"
 author = "hamid-vakilzadeh"
 copyright = f"{year}, {author}"
-version = release = "0.0.42"
+version = release = "0.0.43"
 
 pygments_style = "emacs"
 highlight_language = "python"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/issues/%s", "#"),
     "pr": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/pull/%s", "PR #"),
```

### Comparing `xbrl-us-0.0.42/docs/readme.rst` & `xbrl-us-0.0.43/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/pyproject.toml` & `xbrl-us-0.0.43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/pytest.ini` & `xbrl-us-0.0.43/pytest.ini`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/setup.py` & `xbrl-us-0.0.43/setup.py`

 * *Files identical despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="xbrl-us",
-    version="0.0.42",
+    version="0.0.43",
     license="MIT",
     description="Python wrapper for xbrl.us API",
     long_description_content_type="text/x-rst",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
```

### Comparing `xbrl-us-0.0.42/src/xbrl_us/app.py` & `xbrl-us-0.0.43/src/xbrl_us/app.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/_definitions.yaml` & `xbrl-us-0.0.43/src/xbrl_us/methods/_definitions.yaml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/assertion search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/assertion search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/concept name search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/concept name search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/concept search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/cube search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/cube search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/dimension search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/dimension search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/document search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/document search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/dts id concept label.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/dts id concept label.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/dts id concept name.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/dts id concept name.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/dts id concept reference.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/dts id concept reference.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/dts id concept search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/dts id concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/dts id network search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/dts id network search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/dts id network.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/dts id network.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/dts search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/dts search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/entity id report search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/entity id report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/entity report search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/entity report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/fact id.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/fact id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/fact search oim.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/fact search oim.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/fact search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/label dts id search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/label dts id search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/label search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/label search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/network id relationship search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/network id relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/network relationship search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/network relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/relationship search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/relationship tree search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/relationship tree search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/report fact search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/report fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/report id fact search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/report id fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/report id.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/report id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/methods/report search.yml` & `xbrl-us-0.0.43/src/xbrl_us/methods/report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/schemas/concept_details.py` & `xbrl-us-0.0.43/src/xbrl_us/schemas/concept_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/schemas/dimension_details.py` & `xbrl-us-0.0.43/src/xbrl_us/schemas/dimension_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/utils/exceptions.py` & `xbrl-us-0.0.43/src/xbrl_us/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/utils/paramters.py` & `xbrl-us-0.0.43/src/xbrl_us/utils/paramters.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/src/xbrl_us/xbrl_us.py` & `xbrl-us-0.0.43/src/xbrl_us/xbrl_us.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
             if limit_field in fields_copy:
                 # if the field is in the fields list, remove the field
                 fields_copy.remove(limit_field)
             fields_copy.append(limit_arg)
 
     # Handle offset
     if offset:
-        if offset_field is None:
+        if offset_field is not None:
             # name and add the field name followed by .offset(value)
             offset_arg = f"{offset_field}.offset({offset})"
             if offset_field in fields_copy:
                 fields_copy.remove(offset_field)
             fields_copy.append(offset_arg)
 
     query_params["fields"] = ",".join(fields_copy)
@@ -653,20 +653,15 @@
 
         method_url = self._get_method_url(method_name=method, parameters=parameters, unique=unique)
         # if limit is all
         if limit == "all":
             # arbitrary large number
             limit = 999999999
 
-        query_params = _build_query_params(
-            method=method,
-            fields=fields,
-            parameters=parameters,
-            sort=sort,
-        )
+        query_params = _build_query_params(method=method, fields=fields, parameters=parameters, sort=sort, limit=100)
 
         # check if the account limit has been set
         if not self.account_limit:
             self._get_account_limit(url=method_url, params=query_params)
 
         # ensure the limit is not greater than the account limit
         chunk_limit = min(limit, self.account_limit) if limit is not None else self.account_limit
@@ -686,15 +681,15 @@
             fields=fields,
             parameters=parameters,
             limit=chunk_limit,
             sort=sort,
         )
 
         if print_query:
-            print(query_params)
+            print(f"\n{query_params}")
 
         try:
             response = self._make_request(
                 method="get",
                 url=method_url,
                 params=query_params,
                 timeout=timeout,
@@ -717,28 +712,28 @@
 
         if limit is None:
             # Return the items from the first response if no user limit is provided
             if as_dataframe:
                 return DataFrame.from_dict(data)
             else:
                 return data
-        elif chunk_limit >= len(data):
+        elif chunk_limit > len(data):
             # Return the items from the first response if the user limit is greater than the number of items
             if as_dataframe:
                 return DataFrame.from_dict(data)
             else:
                 return data
 
         else:
             remaining_limit = limit - len(data)
 
         # To store all the items from the API response
         all_data = data
-
         offset = len(data)
+        del data, response_data, response
 
         while remaining_limit > 0:
             # Determine the limit for the current request
             try:
                 current_limit = min(chunk_limit, remaining_limit)
                 query_params = _build_query_params(
                     method=method,
```

### Comparing `xbrl-us-0.0.42/src/xbrl_us.egg-info/PKG-INFO` & `xbrl-us-0.0.43/src/xbrl_us.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.42
+Version: 0.0.43
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
```

### Comparing `xbrl-us-0.0.42/src/xbrl_us.egg-info/SOURCES.txt` & `xbrl-us-0.0.43/src/xbrl_us.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/tests/test_xbrl_us.py` & `xbrl-us-0.0.43/tests/test_xbrl_us.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.42/tox.ini` & `xbrl-us-0.0.43/tox.ini`

 * *Files identical despite different names*

