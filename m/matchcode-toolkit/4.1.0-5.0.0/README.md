# Comparing `tmp/matchcode-toolkit-4.1.0.tar.gz` & `tmp/matchcode_toolkit-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchcode-toolkit-4.1.0.tar", last modified: Tue Apr 16 19:53:44 2024, max compression
+gzip compressed data, was "matchcode_toolkit-5.0.0.tar", last modified: Wed May  8 21:49:21 2024, max compression
```

## Comparing `matchcode-toolkit-4.1.0.tar` & `matchcode_toolkit-5.0.0.tar`

### file list

```diff
@@ -1,97 +1,103 @@
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/
--rw-rw-r--   0 jono      (1000) jono      (1000)       89 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.gitattributes
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.281125 matchcode-toolkit-4.1.0/.github/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/.github/workflows/
--rw-rw-r--   0 jono      (1000) jono      (1000)      752 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.github/workflows/docs-ci.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     2023 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.github/workflows/pypi-release.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)      755 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.gitignore
--rw-rw-r--   0 jono      (1000) jono      (1000)      525 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.readthedocs.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)      104 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/AUTHORS.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     1588 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/CHANGELOG.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     3422 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      217 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/MANIFEST.in
--rw-rw-r--   0 jono      (1000) jono      (1000)     1702 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/Makefile
--rw-rw-r--   0 jono      (1000) jono      (1000)      769 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/NOTICE
--rw-r--r--   0 jono      (1000) jono      (1000)     4012 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)     2386 2024-04-16 19:50:16.000000 matchcode-toolkit-4.1.0/README.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/apache-2.0.LICENSE
--rw-rw-r--   0 jono      (1000) jono      (1000)      971 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/azure-pipelines.yml
--rwxrwxr-x   0 jono      (1000) jono      (1000)     6328 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/configure
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/
--rw-rw-r--   0 jono      (1000) jono      (1000)      890 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/Makefile
--rw-rw-r--   0 jono      (1000) jono      (1000)     1071 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/make.bat
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/scripts/
--rwxrwxr-x   0 jono      (1000) jono      (1000)      131 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/scripts/doc8_style_check.sh
--rw-rw-r--   0 jono      (1000) jono      (1000)      124 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/scripts/sphinx_build_link_check.sh
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/source/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/source/_static/
--rw-rw-r--   0 jono      (1000) jono      (1000)      474 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/_static/theme_overrides.css
--rw-rw-r--   0 jono      (1000) jono      (1000)     3518 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/conf.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/source/contribute/
--rw-rw-r--   0 jono      (1000) jono      (1000)    10245 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/contribute/contrib_doc.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      274 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/index.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     5491 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/skeleton-usage.rst
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.281125 matchcode-toolkit-4.1.0/etc/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.289125 matchcode-toolkit-4.1.0/etc/ci/
--rw-rw-r--   0 jono      (1000) jono      (1000)     1700 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/azure-container-deb.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1753 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/azure-container-rpm.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1240 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/azure-posix.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1215 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/azure-win.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)      257 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/install_sudo.sh
--rw-rw-r--   0 jono      (1000) jono      (1000)     8365 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/macports-ci
--rw-rw-r--   0 jono      (1000) jono      (1000)      684 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/macports-ci.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     1022 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/mit.LICENSE
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.293125 matchcode-toolkit-4.1.0/etc/scripts/
--rwxrwxr-x   0 jono      (1000) jono      (1000)     3744 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/README.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     1301 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/check_thirdparty.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     9486 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/fetch_thirdparty.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     9699 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      354 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     2776 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-rw-r--   0 jono      (1000) jono      (1000)     1715 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_requirements.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     2266 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_requirements_dev.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      101 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/requirements.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)     4497 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      504 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     2839 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      773 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     6418 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_dejacode.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     6704 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      494 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     2850 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_pypi_supported_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      741 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     6152 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_requirements.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    75931 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_thirdparty.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      608 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_thirdparty.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)      867 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/pyproject.toml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1617 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/requirements-dev.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)      314 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/requirements.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)     1492 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/setup.cfg
--rw-rw-r--   0 jono      (1000) jono      (1000)       92 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/setup.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.281125 matchcode-toolkit-4.1.0/src/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.293125 matchcode-toolkit-4.1.0/src/matchcode_toolkit/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     7504 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/fingerprinting.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2024-04-16 18:36:22.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/halohash.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.293125 matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1767 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     2321 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1445 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/plugin_fingerprint.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/
--rw-r--r--   0 jono      (1000) jono      (1000)     4012 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)     2451 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)      200 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-03-15 00:37:28.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 jono      (1000) jono      (1000)      303 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/requires.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)       18 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.293125 matchcode-toolkit-4.1.0/tests/
--rw-rw-r--   0 jono      (1000) jono      (1000)     7473 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/tests/test_fingerprinting.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.281125 matchcode-toolkit-4.1.0/tests/testfiles/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/
--rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
--rw-rw-r--   0 jono      (1000) jono      (1000)    55466 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/inflate-mod.c
--rw-rw-r--   0 jono      (1000) jono      (1000)    55546 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/inflate-mod2.c
--rw-rw-r--   0 jono      (1000) jono      (1000)    55519 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/inflate.c
--rw-rw-r--   0 jono      (1000) jono      (1000)     5962 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/test.json
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.843298 matchcode_toolkit-5.0.0/
+-rw-rw-r--   0 jono      (1000) jono      (1000)       89 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/.gitattributes
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.803299 matchcode_toolkit-5.0.0/.github/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.815299 matchcode_toolkit-5.0.0/.github/workflows/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      752 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/.github/workflows/docs-ci.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2023 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/.github/workflows/pypi-release.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)      756 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/.gitignore
+-rw-rw-r--   0 jono      (1000) jono      (1000)      525 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/.readthedocs.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)      104 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/AUTHORS.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1685 2024-05-08 21:46:04.000000 matchcode_toolkit-5.0.0/CHANGELOG.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3422 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      217 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/MANIFEST.in
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1702 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/Makefile
+-rw-rw-r--   0 jono      (1000) jono      (1000)      769 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/NOTICE
+-rw-r--r--   0 jono      (1000) jono      (1000)     4107 2024-05-08 21:49:21.843298 matchcode_toolkit-5.0.0/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2481 2024-05-08 21:47:52.000000 matchcode_toolkit-5.0.0/README.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/apache-2.0.LICENSE
+-rw-rw-r--   0 jono      (1000) jono      (1000)      971 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/azure-pipelines.yml
+-rwxrwxr-x   0 jono      (1000) jono      (1000)     6328 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/configure
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.815299 matchcode_toolkit-5.0.0/docs/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      890 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/Makefile
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1071 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/make.bat
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.819299 matchcode_toolkit-5.0.0/docs/scripts/
+-rwxrwxr-x   0 jono      (1000) jono      (1000)      131 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/scripts/doc8_style_check.sh
+-rw-rw-r--   0 jono      (1000) jono      (1000)      124 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/scripts/sphinx_build_link_check.sh
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.819299 matchcode_toolkit-5.0.0/docs/source/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.819299 matchcode_toolkit-5.0.0/docs/source/_static/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      474 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/_static/theme_overrides.css
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3518 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/conf.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.819299 matchcode_toolkit-5.0.0/docs/source/contribute/
+-rw-rw-r--   0 jono      (1000) jono      (1000)    10245 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/contribute/contrib_doc.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      274 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/index.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     5491 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/skeleton-usage.rst
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.807299 matchcode_toolkit-5.0.0/etc/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.823299 matchcode_toolkit-5.0.0/etc/ci/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1700 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/azure-container-deb.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1753 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/azure-container-rpm.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1401 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/etc/ci/azure-posix.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1215 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/azure-win.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)      257 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/install_sudo.sh
+-rw-rw-r--   0 jono      (1000) jono      (1000)     8365 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/macports-ci
+-rw-rw-r--   0 jono      (1000) jono      (1000)      684 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/macports-ci.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1022 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/mit.LICENSE
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.831298 matchcode_toolkit-5.0.0/etc/scripts/
+-rwxrwxr-x   0 jono      (1000) jono      (1000)     3744 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/README.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1301 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/check_thirdparty.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     9486 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/fetch_thirdparty.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     9699 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      354 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2776 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1715 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_requirements.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2266 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_requirements_dev.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      101 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/requirements.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4497 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      504 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2839 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      773 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     6418 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_dejacode.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     6704 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_pip_compatibility_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      494 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2850 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_pypi_supported_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      741 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     6152 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_requirements.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    75931 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_thirdparty.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      608 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)      867 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/pyproject.toml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1617 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/requirements-dev.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)      314 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/requirements.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1492 2024-05-08 21:49:21.843298 matchcode_toolkit-5.0.0/setup.cfg
+-rw-rw-r--   0 jono      (1000) jono      (1000)       92 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/setup.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.807299 matchcode_toolkit-5.0.0/src/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.831298 matchcode_toolkit-5.0.0/src/matchcode_toolkit/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     8251 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/fingerprinting.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2024-04-16 18:36:22.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/halohash.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.835298 matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1767 2024-04-16 19:44:23.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2321 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1445 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/plugin_fingerprint.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.839298 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/
+-rw-r--r--   0 jono      (1000) jono      (1000)     4107 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2659 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)      200 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-03-15 00:37:28.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 jono      (1000) jono      (1000)      303 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)       18 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.835298 matchcode_toolkit-5.0.0/tests/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     8603 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/test_fingerprinting.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     7866 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/test_halohash.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.807299 matchcode_toolkit-5.0.0/tests/testfiles/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.839298 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
+-rw-rw-r--   0 jono      (1000) jono      (1000)    55466 2024-04-16 19:44:23.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate-mod.c
+-rw-rw-r--   0 jono      (1000) jono      (1000)    55546 2024-04-16 19:44:23.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate-mod2.c
+-rw-rw-r--   0 jono      (1000) jono      (1000)    55519 2024-04-16 19:44:23.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate.c
+-rw-rw-r--   0 jono      (1000) jono      (1000)     5962 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/test.json
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.839298 matchcode_toolkit-5.0.0/tests/testfiles/halohash/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      752 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/testfiles/halohash/500-delete-expected-results.csv
+-rwxrwxr-x   0 jono      (1000) jono      (1000)      696 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/testfiles/halohash/500-replaced-expected-results.csv
+-rwxrwxr-x   0 jono      (1000) jono      (1000)     3051 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/testfiles/halohash/index.js
+-rw-rw-r--   0 jono      (1000) jono      (1000)     9425 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/testfiles/halohash/words.txt
```

### Comparing `matchcode-toolkit-4.1.0/.github/workflows/docs-ci.yml` & `matchcode_toolkit-5.0.0/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/.github/workflows/pypi-release.yml` & `matchcode_toolkit-5.0.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/.gitignore` & `matchcode_toolkit-5.0.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 docs/build
 docs/include
 docs/Lib
 doc/pyvenv.cfg
 pyvenv.cfg
 
 # Various junk and temp files
-.DS_Store
+*.DS_Store
 *~
 .*.sw[po]
 .build
 .ve
 *.bak
 /.cache/
```

### Comparing `matchcode-toolkit-4.1.0/.readthedocs.yml` & `matchcode_toolkit-5.0.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/CHANGELOG.rst` & `matchcode_toolkit-5.0.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+v5.0.0
+-----
+
+*2024-04-30* -- Update file fingerprint to include number of ngrams hashed in it.
+
 v4.1.0
 ------
 
 *2024-04-15* -- Add new functions to compute fingerprints on text resources for approximate file matching (https://github.com/nexB/matchcode-toolkit/issues/5)
 
 v4.0.0
 ------
```

### Comparing `matchcode-toolkit-4.1.0/CODE_OF_CONDUCT.rst` & `matchcode_toolkit-5.0.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/Makefile` & `matchcode_toolkit-5.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/NOTICE` & `matchcode_toolkit-5.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/PKG-INFO` & `matchcode_toolkit-5.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 4.1.0
+Version: 5.0.0
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: matchcode,ScanCode.io,open source
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,19 +39,19 @@
 Requires-Dist: doc8>=0.11.2; extra == "docs"
 Requires-Dist: sphinx-autobuild; extra == "docs"
 Requires-Dist: sphinx-rtd-dark-mode>=1.3.0; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 
 MatchCode toolkit
 =================
-MatchCode toolkit is a Python library that provides the directory fingerprinting
-functionality for `ScanCode toolkit <https://github.com/nexB/scancode-toolkit>`_
-and `ScanCode.io <https://github.com/nexB/scancode.io>`_ by implementing the
-HaloHash algorithm and using it in ScanCode toolkit and ScanCode.io plugins and
-pipelines.
+MatchCode toolkit is a Python library that provides the file and directory
+fingerprinting functionality for `ScanCode toolkit
+<https://github.com/nexB/scancode-toolkit>`_ and `ScanCode.io
+<https://github.com/nexB/scancode.io>`_ by implementing the HaloHash algorithm
+and using it in ScanCode toolkit and ScanCode.io plugins and pipelines.
 
 
 Installation
 ------------
 
 MatchCode toolkit must be installed in the same environment as ScanCode toolkit
 or ScanCode.io.
@@ -87,14 +87,16 @@
 
   scancode --info --fingerprint <scan target location> --json-pp <output location>
 
 
 MatchCode toolkit provides the ``scan_and_fingerprint_package`` and
 ``fingerprint_codebase`` pipelines for ScanCode.io.
 
+These pipelines add resource and directory fingerprints to the ``extra_data`` field.
+
 
 License
 -------
 
 SPDX-License-Identifier: Apache-2.0
 
 The ScanCode.io software is licensed under the Apache License version 2.0.
```

### Comparing `matchcode-toolkit-4.1.0/README.rst` & `matchcode_toolkit-5.0.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 MatchCode toolkit
 =================
-MatchCode toolkit is a Python library that provides the directory fingerprinting
-functionality for `ScanCode toolkit <https://github.com/nexB/scancode-toolkit>`_
-and `ScanCode.io <https://github.com/nexB/scancode.io>`_ by implementing the
-HaloHash algorithm and using it in ScanCode toolkit and ScanCode.io plugins and
-pipelines.
+MatchCode toolkit is a Python library that provides the file and directory
+fingerprinting functionality for `ScanCode toolkit
+<https://github.com/nexB/scancode-toolkit>`_ and `ScanCode.io
+<https://github.com/nexB/scancode.io>`_ by implementing the HaloHash algorithm
+and using it in ScanCode toolkit and ScanCode.io plugins and pipelines.
 
 
 Installation
 ------------
 
 MatchCode toolkit must be installed in the same environment as ScanCode toolkit
 or ScanCode.io.
@@ -44,14 +44,16 @@
 
   scancode --info --fingerprint <scan target location> --json-pp <output location>
 
 
 MatchCode toolkit provides the ``scan_and_fingerprint_package`` and
 ``fingerprint_codebase`` pipelines for ScanCode.io.
 
+These pipelines add resource and directory fingerprints to the ``extra_data`` field.
+
 
 License
 -------
 
 SPDX-License-Identifier: Apache-2.0
 
 The ScanCode.io software is licensed under the Apache License version 2.0.
```

### Comparing `matchcode-toolkit-4.1.0/apache-2.0.LICENSE` & `matchcode_toolkit-5.0.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/azure-pipelines.yml` & `matchcode_toolkit-5.0.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/configure` & `matchcode_toolkit-5.0.0/configure`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/docs/Makefile` & `matchcode_toolkit-5.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/docs/make.bat` & `matchcode_toolkit-5.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/docs/source/conf.py` & `matchcode_toolkit-5.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/docs/source/contribute/contrib_doc.rst` & `matchcode_toolkit-5.0.0/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/docs/source/skeleton-usage.rst` & `matchcode_toolkit-5.0.0/docs/source/skeleton-usage.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/ci/azure-container-deb.yml` & `matchcode_toolkit-5.0.0/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/ci/azure-container-rpm.yml` & `matchcode_toolkit-5.0.0/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/ci/azure-posix.yml` & `matchcode_toolkit-5.0.0/etc/ci/azure-posix.yml`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,18 @@
               - task: UsePythonVersion@0
                 inputs:
                     versionSpec: '${{ pyver }}'
                     architecture: '${{ parameters.python_architecture }}'
                 displayName: '${{ pyver }} - Install Python'
 
               - script: |
+                    sudo apt-get install wamerican
+                displayName: '${{ pyver }} - Install wamerican dictionary package'
+
+              - script: |
                     python${{ pyver }} --version
                     echo "python${{ pyver }}" > PYTHON_EXECUTABLE
                     ./configure --clean && ./configure --dev
                 displayName: '${{ pyver }} - Configure'
 
               - script: $(test_suite)
                 displayName: '${{ pyver }} - $(test_suite_label) on ${{ parameters.job_name }}'
```

### Comparing `matchcode-toolkit-4.1.0/etc/ci/azure-win.yml` & `matchcode_toolkit-5.0.0/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/ci/macports-ci` & `matchcode_toolkit-5.0.0/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/ci/macports-ci.ABOUT` & `matchcode_toolkit-5.0.0/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/ci/mit.LICENSE` & `matchcode_toolkit-5.0.0/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/README.rst` & `matchcode_toolkit-5.0.0/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/check_thirdparty.py` & `matchcode_toolkit-5.0.0/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/fetch_thirdparty.py` & `matchcode_toolkit-5.0.0/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py` & `matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/gen_requirements.py` & `matchcode_toolkit-5.0.0/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/gen_requirements_dev.py` & `matchcode_toolkit-5.0.0/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `matchcode_toolkit-5.0.0/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/test_utils_pypi_supported_tags.py` & `matchcode_toolkit-5.0.0/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `matchcode_toolkit-5.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/utils_dejacode.py` & `matchcode_toolkit-5.0.0/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/utils_pip_compatibility_tags.py` & `matchcode_toolkit-5.0.0/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/utils_pypi_supported_tags.py` & `matchcode_toolkit-5.0.0/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `matchcode_toolkit-5.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/utils_requirements.py` & `matchcode_toolkit-5.0.0/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/utils_thirdparty.py` & `matchcode_toolkit-5.0.0/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/etc/scripts/utils_thirdparty.py.ABOUT` & `matchcode_toolkit-5.0.0/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/pyproject.toml` & `matchcode_toolkit-5.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/requirements-dev.txt` & `matchcode_toolkit-5.0.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/setup.cfg` & `matchcode_toolkit-5.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/src/matchcode_toolkit/fingerprinting.py` & `matchcode_toolkit-5.0.0/src/matchcode_toolkit/fingerprinting.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,22 +121,22 @@
     for resource in codebase.walk(topdown=False):
         if resource.is_file or not resource.path:
             continue
         _ = _compute_directory_fingerprints(resource, codebase)
     return codebase
 
 
-def split_fingerprint(directory_fingerprint):
+def split_fingerprint(fingerprint):
     """
-    Given a string `directory_fingerprint`, return the indexed elements count as
-    an integer and the bah128 fingerprint string
+    Given a string `fingerprint`, return the indexed elements count as an
+    integer and the bah128 fingerprint string
     """
-    indexed_elements_count_hash = directory_fingerprint[0:8]
+    indexed_elements_count_hash = fingerprint[0:8]
     indexed_elements_count = int(indexed_elements_count_hash, 16)
-    bah128 = directory_fingerprint[8:]
+    bah128 = fingerprint[8:]
     return indexed_elements_count, bah128
 
 
 def hexstring_to_binarray(hex_string):
     """
     Convert a hex string to binary form, then store in a bytearray
     """
@@ -204,34 +204,64 @@
 
     - We start by breaking the file into words (tokens)
     - We compute ngrams over the list of tokens
 
     Return an empty mapping if `location` is not a text file
     """
     from commoncode import filetype
-    from licensedcode.tokenize import ngrams
     from typecode.contenttype import get_type
 
     # Do not process `location` if it's not a text file
     ft = get_type(location)
     if not (filetype.is_file(location) and ft.is_text):
         return {}
 
     with open(location, encoding='utf-8') as f:
         content = f.read()
 
+    file_fingerprint = create_file_fingerprint(
+        content,
+        ngram_length=ngram_length
+    )
+    return dict(
+        halo1=file_fingerprint
+    )
+
+
+def create_content_hash(content, ngram_length=8):
+    """
+    Return a 128-bit BitAverageHaloHash from file `content` and the number of
+    ngrams inserted into the hash
+    """
+    from licensedcode.tokenize import ngrams
+
     # Break content into words, then create ngrams from words
     words = tokenizer(content)
     ngs = ngrams(words, ngram_length)
 
     # Convert each list of ngrams to a sequence of bytes
     ngs_bytes = [[g.encode('utf-8') for g in ng] for ng in ngs]
 
     # Join all ngrams into a single bytearray
     ngs_bytes = [b''.join(ng) for ng in ngs_bytes]
 
     # Create fingerprints and return fingerprint hashes
-    file_fingerprint = BitAverageHaloHash(ngs_bytes) if ngs_bytes else None
+    if ngs_bytes:
+        return BitAverageHaloHash(ngs_bytes), len(ngs_bytes)
+    else:
+        return None, 0
 
-    return dict(
-        halo1=file_fingerprint.hexdigest().decode('utf-8') if file_fingerprint else ''
+
+def create_file_fingerprint(content, ngram_length=8):
+    """
+    Return a 128-bit BitAverageHaloHash fingerprint in hex from file `content`
+    """
+    # Create fingerprint
+    content_hash, ngs_count = create_content_hash(
+        content,
+        ngram_length=ngram_length
     )
+    if content_hash:
+        content_fingerprint = content_hash.hexdigest().decode('utf-8')
+        ngs_count_hex_str = '%08x' % ngs_count
+        file_fingerprint = ngs_count_hex_str + content_fingerprint
+        return file_fingerprint
```

### Comparing `matchcode-toolkit-4.1.0/src/matchcode_toolkit/halohash.py` & `matchcode_toolkit-5.0.0/src/matchcode_toolkit/halohash.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py` & `matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py` & `matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/src/matchcode_toolkit/plugin_fingerprint.py` & `matchcode_toolkit-5.0.0/src/matchcode_toolkit/plugin_fingerprint.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/PKG-INFO` & `matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 4.1.0
+Version: 5.0.0
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: matchcode,ScanCode.io,open source
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,19 +39,19 @@
 Requires-Dist: doc8>=0.11.2; extra == "docs"
 Requires-Dist: sphinx-autobuild; extra == "docs"
 Requires-Dist: sphinx-rtd-dark-mode>=1.3.0; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 
 MatchCode toolkit
 =================
-MatchCode toolkit is a Python library that provides the directory fingerprinting
-functionality for `ScanCode toolkit <https://github.com/nexB/scancode-toolkit>`_
-and `ScanCode.io <https://github.com/nexB/scancode.io>`_ by implementing the
-HaloHash algorithm and using it in ScanCode toolkit and ScanCode.io plugins and
-pipelines.
+MatchCode toolkit is a Python library that provides the file and directory
+fingerprinting functionality for `ScanCode toolkit
+<https://github.com/nexB/scancode-toolkit>`_ and `ScanCode.io
+<https://github.com/nexB/scancode.io>`_ by implementing the HaloHash algorithm
+and using it in ScanCode toolkit and ScanCode.io plugins and pipelines.
 
 
 Installation
 ------------
 
 MatchCode toolkit must be installed in the same environment as ScanCode toolkit
 or ScanCode.io.
@@ -87,14 +87,16 @@
 
   scancode --info --fingerprint <scan target location> --json-pp <output location>
 
 
 MatchCode toolkit provides the ``scan_and_fingerprint_package`` and
 ``fingerprint_codebase`` pipelines for ScanCode.io.
 
+These pipelines add resource and directory fingerprints to the ``extra_data`` field.
+
 
 License
 -------
 
 SPDX-License-Identifier: Apache-2.0
 
 The ScanCode.io software is licensed under the Apache License version 2.0.
```

### Comparing `matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt` & `matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -67,12 +67,17 @@
 src/matchcode_toolkit.egg-info/not-zip-safe
 src/matchcode_toolkit.egg-info/requires.txt
 src/matchcode_toolkit.egg-info/top_level.txt
 src/matchcode_toolkit/pipelines/__init__.py
 src/matchcode_toolkit/pipelines/fingerprint_codebase.py
 src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
 tests/test_fingerprinting.py
+tests/test_halohash.py
 tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
 tests/testfiles/fingerprinting/inflate-mod.c
 tests/testfiles/fingerprinting/inflate-mod2.c
 tests/testfiles/fingerprinting/inflate.c
-tests/testfiles/fingerprinting/test.json
+tests/testfiles/fingerprinting/test.json
+tests/testfiles/halohash/500-delete-expected-results.csv
+tests/testfiles/halohash/500-replaced-expected-results.csv
+tests/testfiles/halohash/index.js
+tests/testfiles/halohash/words.txt
```

### Comparing `matchcode-toolkit-4.1.0/tests/test_fingerprinting.py` & `matchcode_toolkit-5.0.0/tests/test_fingerprinting.py`

 * *Files 12% similar despite different names*

```diff
@@ -130,25 +130,43 @@
     def test_get_file_fingerprint_hashes_one_line_removed(self):
         test_file1 = self.get_test_loc('inflate.c')
         test_file2 = self.get_test_loc('inflate-mod.c')
         result1 = get_file_fingerprint_hashes(test_file1)
         result2 = get_file_fingerprint_hashes(test_file2)
         result1 = result1.get('halo1')
         result2 = result2.get('halo1')
-        expected_result1 = 'a23a49e4cd40718d1297be719e6564a4'
-        expected_result2 = 'aa3a49e4cd40718d1297be519e6564a4'
-        assert result1 == expected_result1
-        assert result2 == expected_result2
-        assert byte_hamming_distance(result1, result2) == 2
+        result1_indexed_elements_count, result1_fingerprint = split_fingerprint(result1)
+        result2_indexed_elements_count, result2_fingerprint = split_fingerprint(result2)
+
+        expected_result1_indexed_elements_count = 6395
+        expected_result2_indexed_elements_count = 6388
+        assert result1_indexed_elements_count == expected_result1_indexed_elements_count
+        assert result2_indexed_elements_count == expected_result2_indexed_elements_count
+
+        expected_result1_fingerprint = 'a23a49e4cd40718d1297be719e6564a4'
+        expected_result2_fingerprint = 'aa3a49e4cd40718d1297be519e6564a4'
+        assert result1_fingerprint == expected_result1_fingerprint
+        assert result2_fingerprint == expected_result2_fingerprint
+
+        assert byte_hamming_distance(result1_fingerprint, result2_fingerprint) == 2
 
     def test_get_file_fingerprint_hashes_one_line_added(self):
         test_file1 = self.get_test_loc('inflate.c')
         test_file2 = self.get_test_loc('inflate-mod2.c')
         result1 = get_file_fingerprint_hashes(test_file1)
         result2 = get_file_fingerprint_hashes(test_file2)
         result1 = result1.get('halo1')
         result2 = result2.get('halo1')
-        expected_result1 = 'a23a49e4cd40718d1297be719e6564a4'
-        expected_result2 = 'a23b49e4cd40708d1297be719c6564a4'
-        assert result1 == expected_result1
-        assert result2 == expected_result2
-        assert byte_hamming_distance(result1, result2) == 3
+        result1_indexed_elements_count, result1_fingerprint = split_fingerprint(result1)
+        result2_indexed_elements_count, result2_fingerprint = split_fingerprint(result2)
+
+        expected_result1_indexed_elements_count = 6395
+        expected_result2_indexed_elements_count = 6398
+        assert result1_indexed_elements_count == expected_result1_indexed_elements_count
+        assert result2_indexed_elements_count == expected_result2_indexed_elements_count
+
+        expected_result1_fingerprint = 'a23a49e4cd40718d1297be719e6564a4'
+        expected_result2_fingerprint = 'a23b49e4cd40708d1297be719c6564a4'
+        assert result1_fingerprint == expected_result1_fingerprint
+        assert result2_fingerprint == expected_result2_fingerprint
+
+        assert byte_hamming_distance(result1_fingerprint, result2_fingerprint) == 3
```

### Comparing `matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json` & `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/inflate-mod.c` & `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate-mod.c`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/inflate-mod2.c` & `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate-mod2.c`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/inflate.c` & `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate.c`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/test.json` & `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/test.json`

 * *Files identical despite different names*

