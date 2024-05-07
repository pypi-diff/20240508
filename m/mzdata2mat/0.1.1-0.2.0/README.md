# Comparing `tmp/mzdata2mat-0.1.1.tar.gz` & `tmp/mzdata2mat-0.2.0.tar.gz`

## Comparing `mzdata2mat-0.1.1.tar` & `mzdata2mat-0.2.0.tar`

### file list

```diff
@@ -1,92 +1,99 @@
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/.readthedocs.yaml
--rwxr-xr-x   0        0        0     1376 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/Changelog.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/make.bat
--rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/requirements.txt
--rw-r--r--   0        0        0    12788 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/Changelog.doctree
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/code-example.doctree
--rw-r--r--   0        0        0   156157 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0    14052 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/installation.doctree
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/matStructure.doctree
--rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/mzData.doctree
--rw-r--r--   0        0        0    28514 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/mzDataManager.doctree
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/mzDataXMLStruct.doctree
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/doctrees/mzdata2mat-verify.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/.buildinfo
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/Changelog.html
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/code-example.html
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/genindex.html
--rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/index.html
--rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/installation.html
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/matStructure.html
--rw-r--r--   0        0        0    11941 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/mzData.html
--rw-r--r--   0        0        0    20922 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/mzDataManager.html
--rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/mzDataXMLStruct.html
--rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/mzdata2mat-verify.html
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/objects.inv
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/search.html
--rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/searchindex.js
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_sources/Changelog.md.txt
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_sources/code-example.md.txt
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_sources/installation.md.txt
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_sources/matStructure.md.txt
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_sources/mzData.md.txt
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_sources/mzDataManager.md.txt
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_sources/mzDataXMLStruct.md.txt
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_sources/mzdata2mat-verify.md.txt
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/build/html/_static/js/theme.js
--rwxr-xr-x   0        0        0     1376 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/Changelog.md
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/code-example.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/installation.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/matStructure.md
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/mzData.md
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/mzDataManager.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/mzDataXMLStruct.md
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/docs/source/mzdata2mat-verify.md
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/src/mzdata2mat/__init__.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/src/mzdata2mat/errors.py
--rwxr-xr-x   0        0        0     8705 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/src/mzdata2mat/mzdata2mat.py
--rw-r--r--   0        0        0    33514 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/src/mzdata2mat/tiny1.mzData.xml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/.gitignore
--rwxr-xr-x   0        0        0     4486 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/README.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 mzdata2mat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0    32392 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/Changelog.doctree
+-rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/advancedLoadSaveLogic.doctree
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/code-example.doctree
+-rw-r--r--   0        0        0   283102 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0    14573 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0     8939 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/installation.doctree
+-rw-r--r--   0        0        0    19861 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/matStruct.doctree
+-rw-r--r--   0        0        0    34484 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/mzData.doctree
+-rw-r--r--   0        0        0    28965 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/mzDataManager.doctree
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/mzDataXMLStruct.doctree
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/doctrees/mzdata2mat-verify.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0    19186 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/Changelog.html
+-rw-r--r--   0        0        0    15433 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/advancedLoadSaveLogic.html
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/code-example.html
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/index.html
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/installation.html
+-rw-r--r--   0        0        0    14789 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/matStruct.html
+-rw-r--r--   0        0        0    31543 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/mzData.html
+-rw-r--r--   0        0        0    21548 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/mzDataManager.html
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/mzDataXMLStruct.html
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/mzdata2mat-verify.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/search.html
+-rw-r--r--   0        0        0    15155 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/Changelog.md.txt
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/advancedLoadSaveLogic.md.txt
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/code-example.md.txt
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/installation.md.txt
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/matStruct.md.txt
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/mzData.md.txt
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/mzDataManager.md.txt
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/mzDataXMLStruct.md.txt
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_sources/mzdata2mat-verify.md.txt
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    16018 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/Changelog.md
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/advancedLoadSaveLogic.md
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/code-example.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/installation.md
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/matStruct.md
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/mzData.md
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/mzDataManager.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/mzDataXMLStruct.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/docs/source/mzdata2mat-verify.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/src/mzdata2mat/__init__.py
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/src/mzdata2mat/classes.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/src/mzdata2mat/errors.py
+-rw-r--r--   0        0        0    11017 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/src/mzdata2mat/mzdata2mat.py
+-rw-r--r--   0        0        0    33514 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/src/mzdata2mat/tiny1.mzData.xml
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/tests/test_mzData.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/tests/test_mzDataManager.py
+-rw-r--r--   0        0        0    33514 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/tests/tiny1.mzData.xml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/.gitignore
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/README.md
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 mzdata2mat-0.2.0/PKG-INFO
```

### Comparing `mzdata2mat-0.1.1/docs/Makefile` & `mzdata2mat-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/make.bat` & `mzdata2mat-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/doctrees/code-example.doctree` & `mzdata2mat-0.2.0/docs/build/doctrees/code-example.doctree`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9583 1600 0000 0000 008c 0f73 7068  .............sph
+00000000: 8005 956e 1600 0000 0000 008c 0f73 7068  ...n.........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -14,348 +14,347 @@
 000000d0: 6375 6d65 6e74 9468 038c 0673 6f75 7263  cument.h...sourc
 000000e0: 6594 4e8c 046c 696e 6594 4e75 6261 8c0a  e.N..line.Nuba..
 000000f0: 6174 7472 6962 7574 6573 947d 9428 8c03  attributes.}.(..
 00000100: 6964 7394 5d94 8c07 636c 6173 7365 7394  ids.]...classes.
 00000110: 5d94 8c05 6e61 6d65 7394 5d94 8c08 6475  ]...names.]...du
 00000120: 706e 616d 6573 945d 948c 0862 6163 6b72  pnames.]...backr
 00000130: 6566 7394 5d94 758c 0774 6167 6e61 6d65  efs.].u..tagname
-00000140: 9468 0f68 1e4b 0168 1d8c 7a2f 5573 6572  .h.h.K.h..z/User
-00000150: 732f 6c69 6368 3931 312f 4c69 6272 6172  s/lich911/Librar
-00000160: 792f 436c 6f75 6453 746f 7261 6765 2f4f  y/CloudStorage/O
-00000170: 6e65 4472 6976 652d 5065 7273 6f6e 6e65  neDrive-Personne
-00000180: 6c2f 446f 6375 6d65 6e74 732f 5079 7468  l/Documents/Pyth
-00000190: 6f6e 2f50 6163 6b61 6765 732f 6d7a 4461  on/Packages/mzDa
-000001a0: 7461 584d 4c32 4d61 742f 646f 6373 2f73  taXML2Mat/docs/s
-000001b0: 6f75 7263 652f 636f 6465 2d65 7861 6d70  ource/code-examp
-000001c0: 6c65 2e6d 6494 681b 680c 681c 6803 7562  le.md.h.h.h.h.ub
-000001d0: 6809 8c09 7061 7261 6772 6170 6894 9394  h...paragraph...
-000001e0: 2981 947d 9428 6805 8c62 5468 6973 2070  )..}.(h..bThis p
-000001f0: 6167 6520 6769 7665 7320 7477 6f20 6578  age gives two ex
-00000200: 616d 706c 6573 206f 6e20 686f 7720 746f  amples on how to
-00000210: 2075 7365 2074 6865 2070 6163 6b61 6765   use the package
-00000220: 2e20 4d6f 7265 2065 7861 6d70 6c65 7320  . More examples 
-00000230: 7769 6c6c 2062 6520 6164 6465 6420 696e  will be added in
-00000240: 2074 6865 2066 7574 7572 652e 9468 075d   the future..h.]
-00000250: 9468 168c 6254 6869 7320 7061 6765 2067  .h..bThis page g
-00000260: 6976 6573 2074 776f 2065 7861 6d70 6c65  ives two example
-00000270: 7320 6f6e 2068 6f77 2074 6f20 7573 6520  s on how to use 
-00000280: 7468 6520 7061 636b 6167 652e 204d 6f72  the package. Mor
-00000290: 6520 6578 616d 706c 6573 2077 696c 6c20  e examples will 
-000002a0: 6265 2061 6464 6564 2069 6e20 7468 6520  be added in the 
-000002b0: 6675 7475 7265 2e94 8594 8194 7d94 2868  future......}.(h
-000002c0: 1b68 2f68 1c68 0368 1d4e 681e 4e75 6261  .h/h.h.h.Nh.Nuba
-000002d0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-000002e0: 9468 275d 9468 295d 9475 682b 682d 681e  .h'].h)].uh+h-h.
-000002f0: 4b02 681d 682c 681b 680c 681c 6803 7562  K.h.h,h.h.h.h.ub
-00000300: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
-00000310: 2868 1029 8194 7d94 2868 058c 0c49 6e20  (h.)..}.(h...In 
-00000320: 7477 6f20 6c69 6e65 7394 6807 5d94 6816  two lines.h.].h.
-00000330: 8c0c 496e 2074 776f 206c 696e 6573 9485  ..In two lines..
-00000340: 9481 947d 9428 681b 6840 681c 6803 681d  ...}.(h.h@h.h.h.
-00000350: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00000360: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00000370: 7568 2b68 0f68 1e4b 0468 1d68 2c68 1b68  uh+h.h.K.h.h,h.h
-00000380: 3d68 1c68 0375 6268 2e29 8194 7d94 2868  =h.h.ubh.)..}.(h
-00000390: 058c 3c59 6f75 2063 616e 2061 6368 6569  ..<You can achei
-000003a0: 7665 2074 6865 2063 6f6e 7665 7273 696f  ve the conversio
-000003b0: 6e20 7769 7468 206f 6e6c 7920 7477 6f20  n with only two 
-000003c0: 6c69 6e65 7320 6f66 2063 6f64 6520 3a94  lines of code :.
-000003d0: 6807 5d94 6816 8c3c 596f 7520 6361 6e20  h.].h..<You can 
-000003e0: 6163 6865 6976 6520 7468 6520 636f 6e76  acheive the conv
-000003f0: 6572 7369 6f6e 2077 6974 6820 6f6e 6c79  ersion with only
-00000400: 2074 776f 206c 696e 6573 206f 6620 636f   two lines of co
-00000410: 6465 203a 9485 9481 947d 9428 681b 684e  de :.....}.(h.hN
-00000420: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00000430: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00000440: 5d94 6829 5d94 7568 2b68 2d68 1e4b 0568  ].h)].uh+h-h.K.h
-00000450: 1d68 2c68 1b68 3d68 1c68 0375 6268 098c  .h,h.h=h.h.ubh..
-00000460: 0d6c 6974 6572 616c 5f62 6c6f 636b 9493  .literal_block..
-00000470: 9429 8194 7d94 2868 058c 7c66 726f 6d20  .)..}.(h..|from 
-00000480: 6d7a 6461 7461 326d 6174 2069 6d70 6f72  mzdata2mat impor
-00000490: 7420 6d7a 4461 7461 4d61 6e61 6765 720a  t mzDataManager.
-000004a0: 0a6d 7a44 6174 614d 616e 6167 6572 2875  .mzDataManager(u
-000004b0: 7365 4469 7265 6374 6f72 793d 4661 6c73  seDirectory=Fals
-000004c0: 6529 2e63 6f6e 7665 7274 4669 6c65 283c  e).convertFile(<
-000004d0: 7061 7468 326d 7a44 6174 6146 696c 653e  path2mzDataFile>
-000004e0: 2c20 3c70 6174 6832 666f 6c64 6572 3273  , <path2folder2s
-000004f0: 6176 653e 290a 0a94 6807 5d94 6816 8c7c  ave>)...h.].h..|
-00000500: 6672 6f6d 206d 7a64 6174 6132 6d61 7420  from mzdata2mat 
-00000510: 696d 706f 7274 206d 7a44 6174 614d 616e  import mzDataMan
-00000520: 6167 6572 0a0a 6d7a 4461 7461 4d61 6e61  ager..mzDataMana
-00000530: 6765 7228 7573 6544 6972 6563 746f 7279  ger(useDirectory
-00000540: 3d46 616c 7365 292e 636f 6e76 6572 7446  =False).convertF
-00000550: 696c 6528 3c70 6174 6832 6d7a 4461 7461  ile(<path2mzData
-00000560: 4669 6c65 3e2c 203c 7061 7468 3266 6f6c  File>, <path2fol
-00000570: 6465 7232 7361 7665 3e29 0a0a 9485 9481  der2save>)......
-00000580: 947d 9468 1b68 5e73 6261 681f 7d94 2868  .}.h.h^sbah.}.(h
-00000590: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000005a0: 295d 948c 086c 616e 6775 6167 6594 8c06  )]...language...
-000005b0: 7079 7468 6f6e 948c 0978 6d6c 3a73 7061  python...xml:spa
-000005c0: 6365 948c 0870 7265 7365 7276 6594 7568  ce...preserve.uh
-000005d0: 2b68 5c68 1d68 2c68 1e4b 0768 1b68 3d68  +h\h.h,h.K.h.h=h
-000005e0: 1c68 0375 6265 681f 7d94 2868 215d 948c  .h.ubeh.}.(h!]..
-000005f0: 0c69 6e2d 7477 6f2d 6c69 6e65 7394 6168  .in-two-lines.ah
-00000600: 235d 9468 255d 948c 0c69 6e20 7477 6f20  #].h%]...in two 
-00000610: 6c69 6e65 7394 6168 275d 9468 295d 9475  lines.ah'].h)].u
-00000620: 682b 680a 681e 4b04 681d 682c 681b 680c  h+h.h.K.h.h,h.h.
-00000630: 681c 6803 7562 680b 2981 947d 9428 6805  h.h.ubh.)..}.(h.
-00000640: 6806 6807 5d94 2868 1029 8194 7d94 2868  h.h.].(h.)..}.(h
-00000650: 058c 164d 6f72 6520 6465 7461 696c 6c65  ...More detaille
-00000660: 6420 6578 616d 706c 6594 6807 5d94 6816  d example.h.].h.
-00000670: 8c16 4d6f 7265 2064 6574 6169 6c6c 6564  ..More detailled
-00000680: 2065 7861 6d70 6c65 9485 9481 947d 9428   example.....}.(
-00000690: 681b 687b 681c 6803 681d 4e68 1e4e 7562  h.h{h.h.h.Nh.Nub
-000006a0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-000006b0: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
-000006c0: 1e4b 0d68 1d68 2c68 1b68 7868 1c68 0375  .K.h.h,h.hxh.h.u
-000006d0: 6268 5d29 8194 7d94 2868 0558 c802 0000  bh])..}.(h.X....
-000006e0: 0a23 2048 6572 6520 7765 2069 6d70 6f72  .# Here we impor
-000006f0: 7420 7468 6520 6d61 696e 2063 6c61 7373  t the main class
-00000700: 2075 7365 6420 666f 7220 7468 6520 636f   used for the co
-00000710: 6e76 6572 7369 6f6e 2e0a 3120 6672 6f6d  nversion..1 from
-00000720: 206d 7a64 6174 6132 6d61 7420 696d 706f   mzdata2mat impo
-00000730: 7274 206d 7a44 6174 614d 616e 6167 6572  rt mzDataManager
-00000740: 0a0a 2320 5765 2069 6e69 7469 616c 697a  ..# We initializ
-00000750: 6520 7468 6520 636c 6173 730a 2320 4966  e the class.# If
-00000760: 2061 6c6c 206d 7a44 6174 6120 6669 6c65   all mzData file
-00000770: 7320 6172 6520 7374 6f72 6564 2069 6e20  s are stored in 
-00000780: 7468 6520 7361 6d65 2064 6972 6563 746f  the same directo
-00000790: 7279 2c20 7765 2063 616e 2073 7065 6369  ry, we can speci
-000007a0: 6679 2074 6865 2070 6172 616d 6574 6572  fy the parameter
-000007b0: 2060 6d7a 4461 7461 5061 7468 6020 696e   `mzDataPath` in
-000007c0: 7374 6561 6420 6f66 2060 7573 6544 6972  stead of `useDir
-000007d0: 6563 746f 7279 602e 0a32 2063 6f6e 7665  ectory`..2 conve
-000007e0: 7274 6572 4167 656e 7420 3d20 6d7a 4461  rterAgent = mzDa
-000007f0: 7461 4d61 6e61 6765 7228 7573 6544 6972  taManager(useDir
-00000800: 6563 746f 7279 3d46 616c 7365 290a 0a33  ectory=False)..3
-00000810: 2070 6174 6832 6d7a 4461 7461 4669 6c65   path2mzDataFile
-00000820: 203a 2073 7472 203d 2022 7061 7468 2f74   : str = "path/t
-00000830: 6f2f 7374 6f72 6564 2f66 696c 6573 220a  o/stored/files".
-00000840: 0a34 2073 6f6d 6544 6972 6563 746f 7279  .4 someDirectory
-00000850: 203a 2073 7472 203d 2022 7061 7468 2f74   : str = "path/t
-00000860: 6f2f 7361 7665 2f66 696c 652f 220a 0a23  o/save/file/"..#
-00000870: 204e 6f77 2077 6520 6361 6e20 6361 6c6c   Now we can call
-00000880: 2074 6865 206d 7a44 6174 6158 4d4c 7265   the mzDataXMLre
-00000890: 6164 2066 756e 6374 696f 6e20 746f 2072  ad function to r
-000008a0: 6561 6420 7468 6520 2e6d 7a44 6174 612e  ead the .mzData.
-000008b0: 786d 6c20 6669 6c65 3a0a 3520 6461 7461  xml file:.5 data
-000008c0: 203d 2063 6f6e 7665 7274 6572 4167 656e   = converterAgen
-000008d0: 742e 6d7a 4461 7461 584d 4c72 6561 6428  t.mzDataXMLread(
-000008e0: 6669 6c65 4e61 6d65 3d70 6174 6832 6d7a  fileName=path2mz
-000008f0: 4461 7461 4669 6c65 290a 0a23 2054 6865  DataFile)..# The
-00000900: 2064 6174 6120 7765 2776 6520 676f 7420   data we've got 
-00000910: 6672 6f6d 2074 6865 2070 7265 7669 6f75  from the previou
-00000920: 7320 6675 6e63 7469 6f6e 2063 616e 2062  s function can b
-00000930: 6520 7361 7665 6420 746f 2061 202e 6d61  e saved to a .ma
-00000940: 7420 6669 6c65 2077 6974 6820 7468 6520  t file with the 
-00000950: 7361 7665 4d61 7466 696c 6520 6675 6e74  saveMatfile funt
-00000960: 696f 6e3a 0a36 2063 6f6e 7665 7274 6572  ion:.6 converter
-00000970: 4167 656e 742e 7361 7665 4d61 7466 696c  Agent.saveMatfil
-00000980: 6528 6d7a 4461 7461 3d64 6174 612c 2064  e(mzData=data, d
-00000990: 6972 3273 6176 653d 736f 6d65 4469 7265  ir2save=someDire
-000009a0: 6374 6f72 7929 0a0a 9468 075d 9468 1658  ctory)...h.].h.X
-000009b0: c802 0000 0a23 2048 6572 6520 7765 2069  .....# Here we i
-000009c0: 6d70 6f72 7420 7468 6520 6d61 696e 2063  mport the main c
-000009d0: 6c61 7373 2075 7365 6420 666f 7220 7468  lass used for th
-000009e0: 6520 636f 6e76 6572 7369 6f6e 2e0a 3120  e conversion..1 
-000009f0: 6672 6f6d 206d 7a64 6174 6132 6d61 7420  from mzdata2mat 
-00000a00: 696d 706f 7274 206d 7a44 6174 614d 616e  import mzDataMan
-00000a10: 6167 6572 0a0a 2320 5765 2069 6e69 7469  ager..# We initi
-00000a20: 616c 697a 6520 7468 6520 636c 6173 730a  alize the class.
-00000a30: 2320 4966 2061 6c6c 206d 7a44 6174 6120  # If all mzData 
-00000a40: 6669 6c65 7320 6172 6520 7374 6f72 6564  files are stored
-00000a50: 2069 6e20 7468 6520 7361 6d65 2064 6972   in the same dir
-00000a60: 6563 746f 7279 2c20 7765 2063 616e 2073  ectory, we can s
-00000a70: 7065 6369 6679 2074 6865 2070 6172 616d  pecify the param
-00000a80: 6574 6572 2060 6d7a 4461 7461 5061 7468  eter `mzDataPath
-00000a90: 6020 696e 7374 6561 6420 6f66 2060 7573  ` instead of `us
-00000aa0: 6544 6972 6563 746f 7279 602e 0a32 2063  eDirectory`..2 c
-00000ab0: 6f6e 7665 7274 6572 4167 656e 7420 3d20  onverterAgent = 
-00000ac0: 6d7a 4461 7461 4d61 6e61 6765 7228 7573  mzDataManager(us
-00000ad0: 6544 6972 6563 746f 7279 3d46 616c 7365  eDirectory=False
-00000ae0: 290a 0a33 2070 6174 6832 6d7a 4461 7461  )..3 path2mzData
-00000af0: 4669 6c65 203a 2073 7472 203d 2022 7061  File : str = "pa
-00000b00: 7468 2f74 6f2f 7374 6f72 6564 2f66 696c  th/to/stored/fil
-00000b10: 6573 220a 0a34 2073 6f6d 6544 6972 6563  es"..4 someDirec
-00000b20: 746f 7279 203a 2073 7472 203d 2022 7061  tory : str = "pa
-00000b30: 7468 2f74 6f2f 7361 7665 2f66 696c 652f  th/to/save/file/
-00000b40: 220a 0a23 204e 6f77 2077 6520 6361 6e20  "..# Now we can 
-00000b50: 6361 6c6c 2074 6865 206d 7a44 6174 6158  call the mzDataX
-00000b60: 4d4c 7265 6164 2066 756e 6374 696f 6e20  MLread function 
-00000b70: 746f 2072 6561 6420 7468 6520 2e6d 7a44  to read the .mzD
-00000b80: 6174 612e 786d 6c20 6669 6c65 3a0a 3520  ata.xml file:.5 
-00000b90: 6461 7461 203d 2063 6f6e 7665 7274 6572  data = converter
-00000ba0: 4167 656e 742e 6d7a 4461 7461 584d 4c72  Agent.mzDataXMLr
-00000bb0: 6561 6428 6669 6c65 4e61 6d65 3d70 6174  ead(fileName=pat
-00000bc0: 6832 6d7a 4461 7461 4669 6c65 290a 0a23  h2mzDataFile)..#
-00000bd0: 2054 6865 2064 6174 6120 7765 2776 6520   The data we've 
-00000be0: 676f 7420 6672 6f6d 2074 6865 2070 7265  got from the pre
-00000bf0: 7669 6f75 7320 6675 6e63 7469 6f6e 2063  vious function c
-00000c00: 616e 2062 6520 7361 7665 6420 746f 2061  an be saved to a
-00000c10: 202e 6d61 7420 6669 6c65 2077 6974 6820   .mat file with 
-00000c20: 7468 6520 7361 7665 4d61 7466 696c 6520  the saveMatfile 
-00000c30: 6675 6e74 696f 6e3a 0a36 2063 6f6e 7665  funtion:.6 conve
-00000c40: 7274 6572 4167 656e 742e 7361 7665 4d61  rterAgent.saveMa
-00000c50: 7466 696c 6528 6d7a 4461 7461 3d64 6174  tfile(mzData=dat
-00000c60: 612c 2064 6972 3273 6176 653d 736f 6d65  a, dir2save=some
-00000c70: 4469 7265 6374 6f72 7929 0a0a 9485 9481  Directory)......
-00000c80: 947d 9468 1b68 8973 6261 681f 7d94 2868  .}.h.h.sbah.}.(h
-00000c90: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00000ca0: 295d 948c 086c 616e 6775 6167 6594 8c06  )]...language...
-00000cb0: 7079 7468 6f6e 9468 6e68 6f75 682b 685c  python.hnhouh+h\
-00000cc0: 681d 682c 681e 4b0f 681b 6878 681c 6803  h.h,h.K.h.hxh.h.
-00000cd0: 7562 6568 1f7d 9428 6821 5d94 8c16 6d6f  ubeh.}.(h!]...mo
-00000ce0: 7265 2d64 6574 6169 6c6c 6564 2d65 7861  re-detailled-exa
-00000cf0: 6d70 6c65 9461 6823 5d94 6825 5d94 8c16  mple.ah#].h%]...
-00000d00: 6d6f 7265 2064 6574 6169 6c6c 6564 2065  more detailled e
-00000d10: 7861 6d70 6c65 9461 6827 5d94 6829 5d94  xample.ah'].h)].
-00000d20: 7568 2b68 0a68 1e4b 0d68 1d68 2c68 1b68  uh+h.h.K.h.h,h.h
-00000d30: 0c68 1c68 0375 6265 681f 7d94 2868 215d  .h.h.ubeh.}.(h!]
-00000d40: 948c 0c65 7861 6d70 6c65 2d63 6f64 6594  ...example-code.
-00000d50: 6168 235d 9468 255d 948c 0c65 7861 6d70  ah#].h%]...examp
-00000d60: 6c65 2063 6f64 6594 6168 275d 9468 295d  le code.ah'].h)]
-00000d70: 9475 682b 680a 681e 4b01 681d 682c 681b  .uh+h.h.K.h.h,h.
-00000d80: 6803 681c 6803 7562 6168 1f7d 9428 6821  h.h.h.ubah.}.(h!
-00000d90: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00000da0: 5d94 8c06 736f 7572 6365 9468 2c8c 1474  ]...source.h,..t
-00000db0: 7261 6e73 6c61 7469 6f6e 5f70 726f 6772  ranslation_progr
-00000dc0: 6573 7394 7d94 288c 0574 6f74 616c 944b  ess.}.(..total.K
-00000dd0: 008c 0a74 7261 6e73 6c61 7465 6494 4b00  ...translated.K.
-00000de0: 7575 682b 6801 8c0e 6375 7272 656e 745f  uuh+h...current_
-00000df0: 736f 7572 6365 944e 8c0c 6375 7272 656e  source.N..curren
-00000e00: 745f 6c69 6e65 944e 8c08 7365 7474 696e  t_line.N..settin
-00000e10: 6773 948c 1164 6f63 7574 696c 732e 6672  gs...docutils.fr
-00000e20: 6f6e 7465 6e64 948c 0656 616c 7565 7394  ontend...Values.
-00000e30: 9394 2981 947d 9428 680f 4e8c 0967 656e  ..)..}.(h.N..gen
-00000e40: 6572 6174 6f72 944e 8c09 6461 7465 7374  erator.N..datest
-00000e50: 616d 7094 4e8c 0b73 6f75 7263 655f 6c69  amp.N..source_li
-00000e60: 6e6b 944e 8c0a 736f 7572 6365 5f75 726c  nk.N..source_url
-00000e70: 944e 8c0d 746f 635f 6261 636b 6c69 6e6b  .N..toc_backlink
-00000e80: 7394 8c05 656e 7472 7994 8c12 666f 6f74  s...entry...foot
-00000e90: 6e6f 7465 5f62 6163 6b6c 696e 6b73 944b  note_backlinks.K
-00000ea0: 018c 0d73 6563 746e 756d 5f78 666f 726d  ...sectnum_xform
-00000eb0: 944b 018c 0e73 7472 6970 5f63 6f6d 6d65  .K...strip_comme
-00000ec0: 6e74 7394 4e8c 1b73 7472 6970 5f65 6c65  nts.N..strip_ele
-00000ed0: 6d65 6e74 735f 7769 7468 5f63 6c61 7373  ments_with_class
-00000ee0: 6573 944e 8c0d 7374 7269 705f 636c 6173  es.N..strip_clas
-00000ef0: 7365 7394 4e8c 0c72 6570 6f72 745f 6c65  ses.N..report_le
-00000f00: 7665 6c94 4b02 8c0a 6861 6c74 5f6c 6576  vel.K...halt_lev
-00000f10: 656c 944b 058c 1165 7869 745f 7374 6174  el.K...exit_stat
-00000f20: 7573 5f6c 6576 656c 944b 058c 0564 6562  us_level.K...deb
-00000f30: 7567 944e 8c0e 7761 726e 696e 675f 7374  ug.N..warning_st
-00000f40: 7265 616d 944e 8c09 7472 6163 6562 6163  ream.N..tracebac
-00000f50: 6b94 888c 0e69 6e70 7574 5f65 6e63 6f64  k....input_encod
-00000f60: 696e 6794 8c09 7574 662d 382d 7369 6794  ing...utf-8-sig.
-00000f70: 8c1c 696e 7075 745f 656e 636f 6469 6e67  ..input_encoding
-00000f80: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
-00000f90: 0673 7472 6963 7494 8c0f 6f75 7470 7574  .strict...output
-00000fa0: 5f65 6e63 6f64 696e 6794 8c05 7574 662d  _encoding...utf-
-00000fb0: 3894 8c1d 6f75 7470 7574 5f65 6e63 6f64  8...output_encod
-00000fc0: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
-00000fd0: 7294 68d0 8c0e 6572 726f 725f 656e 636f  r.h...error_enco
-00000fe0: 6469 6e67 948c 0575 7466 2d38 948c 1c65  ding...utf-8...e
-00000ff0: 7272 6f72 5f65 6e63 6f64 696e 675f 6572  rror_encoding_er
-00001000: 726f 725f 6861 6e64 6c65 7294 8c10 6261  ror_handler...ba
-00001010: 636b 736c 6173 6872 6570 6c61 6365 948c  ckslashreplace..
-00001020: 0d6c 616e 6775 6167 655f 636f 6465 948c  .language_code..
-00001030: 0265 6e94 8c13 7265 636f 7264 5f64 6570  .en...record_dep
-00001040: 656e 6465 6e63 6965 7394 4e8c 0663 6f6e  endencies.N..con
-00001050: 6669 6794 4e8c 0969 645f 7072 6566 6978  fig.N..id_prefix
-00001060: 9468 068c 0e61 7574 6f5f 6964 5f70 7265  .h...auto_id_pre
-00001070: 6669 7894 8c02 6964 948c 0d64 756d 705f  fix...id...dump_
-00001080: 7365 7474 696e 6773 944e 8c0e 6475 6d70  settings.N..dump
-00001090: 5f69 6e74 6572 6e61 6c73 944e 8c0f 6475  _internals.N..du
-000010a0: 6d70 5f74 7261 6e73 666f 726d 7394 4e8c  mp_transforms.N.
-000010b0: 0f64 756d 705f 7073 6575 646f 5f78 6d6c  .dump_pseudo_xml
-000010c0: 944e 8c10 6578 706f 7365 5f69 6e74 6572  .N..expose_inter
-000010d0: 6e61 6c73 944e 8c0e 7374 7269 6374 5f76  nals.N..strict_v
-000010e0: 6973 6974 6f72 944e 8c0f 5f64 6973 6162  isitor.N.._disab
-000010f0: 6c65 5f63 6f6e 6669 6794 4e8c 075f 736f  le_config.N.._so
-00001100: 7572 6365 9468 2c8c 0c5f 6465 7374 696e  urce.h,.._destin
-00001110: 6174 696f 6e94 4e8c 0d5f 636f 6e66 6967  ation.N.._config
-00001120: 5f66 696c 6573 945d 948c 1666 696c 655f  _files.]...file_
-00001130: 696e 7365 7274 696f 6e5f 656e 6162 6c65  insertion_enable
-00001140: 6494 888c 0b72 6177 5f65 6e61 626c 6564  d....raw_enabled
-00001150: 944b 018c 116c 696e 655f 6c65 6e67 7468  .K...line_length
-00001160: 5f6c 696d 6974 944d 1027 8c0e 7065 705f  _limit.M.'..pep_
-00001170: 7265 6665 7265 6e63 6573 944e 8c0c 7065  references.N..pe
-00001180: 705f 6261 7365 5f75 726c 948c 1868 7474  p_base_url...htt
-00001190: 7073 3a2f 2f70 6570 732e 7079 7468 6f6e  ps://peps.python
-000011a0: 2e6f 7267 2f94 8c15 7065 705f 6669 6c65  .org/...pep_file
-000011b0: 5f75 726c 5f74 656d 706c 6174 6594 8c08  _url_template...
-000011c0: 7065 702d 2530 3464 948c 0e72 6663 5f72  pep-%04d...rfc_r
-000011d0: 6566 6572 656e 6365 7394 4e8c 0c72 6663  eferences.N..rfc
-000011e0: 5f62 6173 655f 7572 6c94 8c26 6874 7470  _base_url..&http
-000011f0: 733a 2f2f 6461 7461 7472 6163 6b65 722e  s://datatracker.
-00001200: 6965 7466 2e6f 7267 2f64 6f63 2f68 746d  ietf.org/doc/htm
-00001210: 6c2f 948c 0974 6162 5f77 6964 7468 944b  l/...tab_width.K
-00001220: 088c 1d74 7269 6d5f 666f 6f74 6e6f 7465  ...trim_footnote
-00001230: 5f72 6566 6572 656e 6365 5f73 7061 6365  _reference_space
-00001240: 9489 8c10 7379 6e74 6178 5f68 6967 686c  ....syntax_highl
-00001250: 6967 6874 948c 046c 6f6e 6794 8c0c 736d  ight...long...sm
-00001260: 6172 745f 7175 6f74 6573 9488 8c13 736d  art_quotes....sm
-00001270: 6172 7471 756f 7465 735f 6c6f 6361 6c65  artquotes_locale
-00001280: 7394 5d94 8c1d 6368 6172 6163 7465 725f  s.]...character_
-00001290: 6c65 7665 6c5f 696e 6c69 6e65 5f6d 6172  level_inline_mar
-000012a0: 6b75 7094 898c 0e64 6f63 7469 746c 655f  kup....doctitle_
-000012b0: 7866 6f72 6d94 898c 0d64 6f63 696e 666f  xform....docinfo
-000012c0: 5f78 666f 726d 944b 018c 1273 6563 7473  _xform.K...sects
-000012d0: 7562 7469 746c 655f 7866 6f72 6d94 898c  ubtitle_xform...
-000012e0: 0d69 6d61 6765 5f6c 6f61 6469 6e67 948c  .image_loading..
-000012f0: 046c 696e 6b94 8c10 656d 6265 645f 7374  .link...embed_st
-00001300: 796c 6573 6865 6574 9489 8c15 636c 6f61  ylesheet....cloa
-00001310: 6b5f 656d 6169 6c5f 6164 6472 6573 7365  k_email_addresse
-00001320: 7394 888c 1173 6563 7469 6f6e 5f73 656c  s....section_sel
-00001330: 665f 6c69 6e6b 9489 8c03 656e 7694 4e75  f_link....env.Nu
-00001340: 628c 0872 6570 6f72 7465 7294 4e8c 1069  b..reporter.N..i
-00001350: 6e64 6972 6563 745f 7461 7267 6574 7394  ndirect_targets.
-00001360: 5d94 8c11 7375 6273 7469 7475 7469 6f6e  ]...substitution
-00001370: 5f64 6566 7394 7d94 288c 0f77 6f72 6463  _defs.}.(..wordc
-00001380: 6f75 6e74 2d77 6f72 6473 9468 098c 1773  ount-words.h...s
-00001390: 7562 7374 6974 7574 696f 6e5f 6465 6669  ubstitution_defi
-000013a0: 6e69 7469 6f6e 9493 9429 8194 7d94 2868  nition...)..}.(h
-000013b0: 058c 0233 3894 6807 5d94 6816 8c02 3338  ...38.h.].h...38
-000013c0: 9485 9481 947d 9468 1b6a 0e01 0000 7362  .....}.h.j....sb
-000013d0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-000013e0: 5d94 8c0f 776f 7264 636f 756e 742d 776f  ]...wordcount-wo
-000013f0: 7264 7394 6168 275d 9468 295d 9475 682b  rds.ah'].h)].uh+
-00001400: 6a0c 0100 0068 1d68 2c75 628c 1177 6f72  j....h.h,ub..wor
-00001410: 6463 6f75 6e74 2d6d 696e 7574 6573 946a  dcount-minutes.j
-00001420: 0d01 0000 2981 947d 9428 6805 8c01 3094  ....)..}.(h...0.
-00001430: 6807 5d94 6816 8c01 3094 8594 8194 7d94  h.].h...0.....}.
-00001440: 681b 6a1e 0100 0073 6261 681f 7d94 2868  h.j....sbah.}.(h
-00001450: 215d 9468 235d 9468 255d 948c 1177 6f72  !].h#].h%]...wor
-00001460: 6463 6f75 6e74 2d6d 696e 7574 6573 9461  dcount-minutes.a
-00001470: 6827 5d94 6829 5d94 7568 2b6a 0c01 0000  h'].h)].uh+j....
-00001480: 681d 682c 7562 758c 1273 7562 7374 6974  h.h,ubu..substit
-00001490: 7574 696f 6e5f 6e61 6d65 7394 7d94 288c  ution_names.}.(.
-000014a0: 0f77 6f72 6463 6f75 6e74 2d77 6f72 6473  .wordcount-words
-000014b0: 946a 0b01 0000 8c11 776f 7264 636f 756e  .j......wordcoun
-000014c0: 742d 6d69 6e75 7465 7394 6a1d 0100 0075  t-minutes.j....u
-000014d0: 8c08 7265 666e 616d 6573 947d 948c 0672  ..refnames.}...r
-000014e0: 6566 6964 7394 7d94 8c07 6e61 6d65 6964  efids.}...nameid
-000014f0: 7394 7d94 2868 a668 a368 7568 7268 9e68  s.}.(h.h.huhrh.h
-00001500: 9b75 8c09 6e61 6d65 7479 7065 7394 7d94  .u..nametypes.}.
-00001510: 2868 a689 6875 8968 9e89 7568 217d 9428  (h..hu.h..uh!}.(
-00001520: 68a3 680c 6872 683d 689b 6878 758c 0d66  h.h.hrh=h.hxu..f
-00001530: 6f6f 746e 6f74 655f 7265 6673 947d 948c  ootnote_refs.}..
-00001540: 0d63 6974 6174 696f 6e5f 7265 6673 947d  .citation_refs.}
-00001550: 948c 0d61 7574 6f66 6f6f 746e 6f74 6573  ...autofootnotes
-00001560: 945d 948c 1161 7574 6f66 6f6f 746e 6f74  .]...autofootnot
-00001570: 655f 7265 6673 945d 948c 1073 796d 626f  e_refs.]...symbo
-00001580: 6c5f 666f 6f74 6e6f 7465 7394 5d94 8c14  l_footnotes.]...
-00001590: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
-000015a0: 7265 6673 945d 948c 0966 6f6f 746e 6f74  refs.]...footnot
-000015b0: 6573 945d 948c 0963 6974 6174 696f 6e73  es.]...citations
-000015c0: 945d 948c 1261 7574 6f66 6f6f 746e 6f74  .]...autofootnot
-000015d0: 655f 7374 6172 7494 4b01 8c15 7379 6d62  e_start.K...symb
-000015e0: 6f6c 5f66 6f6f 746e 6f74 655f 7374 6172  ol_footnote_star
-000015f0: 7494 4b00 8c0a 6964 5f63 6f75 6e74 6572  t.K...id_counter
-00001600: 948c 0b63 6f6c 6c65 6374 696f 6e73 948c  ...collections..
-00001610: 0743 6f75 6e74 6572 9493 947d 9485 9452  .Counter...}...R
-00001620: 948c 0e70 6172 7365 5f6d 6573 7361 6765  ...parse_message
-00001630: 7394 5d94 8c12 7472 616e 7366 6f72 6d5f  s.]...transform_
-00001640: 6d65 7373 6167 6573 945d 948c 0b74 7261  messages.]...tra
-00001650: 6e73 666f 726d 6572 944e 8c0b 696e 636c  nsformer.N..incl
-00001660: 7564 655f 6c6f 6794 5d94 8c0a 6465 636f  ude_log.]...deco
-00001670: 7261 7469 6f6e 944e 681c 6803 8c0a 6d79  ration.Nh.h...my
-00001680: 7374 5f73 6c75 6773 947d 9475 622e       st_slugs.}.ub.
+00000140: 9468 0f68 1e4b 0168 1d8c 5b43 3a5c 5573  .h.h.K.h..[C:\Us
+00000150: 6572 735c 6d61 7869 6d5c 4f6e 6544 7269  ers\maxim\OneDri
+00000160: 7665 5c44 6f63 756d 656e 7473 5c50 7974  ve\Documents\Pyt
+00000170: 686f 6e5c 5061 636b 6167 6573 5c6d 7a44  hon\Packages\mzD
+00000180: 6174 6158 4d4c 324d 6174 5c64 6f63 735c  ataXML2Mat\docs\
+00000190: 736f 7572 6365 5c63 6f64 652d 6578 616d  source\code-exam
+000001a0: 706c 652e 6d64 9468 1b68 0c68 1c68 0375  ple.md.h.h.h.h.u
+000001b0: 6268 098c 0970 6172 6167 7261 7068 9493  bh...paragraph..
+000001c0: 9429 8194 7d94 2868 058c 6254 6869 7320  .)..}.(h..bThis 
+000001d0: 7061 6765 2067 6976 6573 2074 776f 2065  page gives two e
+000001e0: 7861 6d70 6c65 7320 6f6e 2068 6f77 2074  xamples on how t
+000001f0: 6f20 7573 6520 7468 6520 7061 636b 6167  o use the packag
+00000200: 652e 204d 6f72 6520 6578 616d 706c 6573  e. More examples
+00000210: 2077 696c 6c20 6265 2061 6464 6564 2069   will be added i
+00000220: 6e20 7468 6520 6675 7475 7265 2e94 6807  n the future..h.
+00000230: 5d94 6816 8c62 5468 6973 2070 6167 6520  ].h..bThis page 
+00000240: 6769 7665 7320 7477 6f20 6578 616d 706c  gives two exampl
+00000250: 6573 206f 6e20 686f 7720 746f 2075 7365  es on how to use
+00000260: 2074 6865 2070 6163 6b61 6765 2e20 4d6f   the package. Mo
+00000270: 7265 2065 7861 6d70 6c65 7320 7769 6c6c  re examples will
+00000280: 2062 6520 6164 6465 6420 696e 2074 6865   be added in the
+00000290: 2066 7574 7572 652e 9485 9481 947d 9428   future......}.(
+000002a0: 681b 682f 681c 6803 681d 4e68 1e4e 7562  h.h/h.h.h.Nh.Nub
+000002b0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000002c0: 5d94 6827 5d94 6829 5d94 7568 2b68 2d68  ].h'].h)].uh+h-h
+000002d0: 1e4b 0268 1d68 2c68 1b68 0c68 1c68 0375  .K.h.h,h.h.h.h.u
+000002e0: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
+000002f0: 9428 6810 2981 947d 9428 6805 8c0c 496e  .(h.)..}.(h...In
+00000300: 2074 776f 206c 696e 6573 9468 075d 9468   two lines.h.].h
+00000310: 168c 0c49 6e20 7477 6f20 6c69 6e65 7394  ...In two lines.
+00000320: 8594 8194 7d94 2868 1b68 4068 1c68 0368  ....}.(h.h@h.h.h
+00000330: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00000340: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00000350: 9475 682b 680f 681e 4b04 681d 682c 681b  .uh+h.h.K.h.h,h.
+00000360: 683d 681c 6803 7562 682e 2981 947d 9428  h=h.h.ubh.)..}.(
+00000370: 6805 8c3c 596f 7520 6361 6e20 6163 6865  h..<You can ache
+00000380: 6976 6520 7468 6520 636f 6e76 6572 7369  ive the conversi
+00000390: 6f6e 2077 6974 6820 6f6e 6c79 2074 776f  on with only two
+000003a0: 206c 696e 6573 206f 6620 636f 6465 203a   lines of code :
+000003b0: 9468 075d 9468 168c 3c59 6f75 2063 616e  .h.].h..<You can
+000003c0: 2061 6368 6569 7665 2074 6865 2063 6f6e   acheive the con
+000003d0: 7665 7273 696f 6e20 7769 7468 206f 6e6c  version with onl
+000003e0: 7920 7477 6f20 6c69 6e65 7320 6f66 2063  y two lines of c
+000003f0: 6f64 6520 3a94 8594 8194 7d94 2868 1b68  ode :.....}.(h.h
+00000400: 4e68 1c68 0368 1d4e 681e 4e75 6261 681f  Nh.h.h.Nh.Nubah.
+00000410: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00000420: 275d 9468 295d 9475 682b 682d 681e 4b05  '].h)].uh+h-h.K.
+00000430: 681d 682c 681b 683d 681c 6803 7562 6809  h.h,h.h=h.h.ubh.
+00000440: 8c0d 6c69 7465 7261 6c5f 626c 6f63 6b94  ..literal_block.
+00000450: 9394 2981 947d 9428 6805 8c7c 6672 6f6d  ..)..}.(h..|from
+00000460: 206d 7a64 6174 6132 6d61 7420 696d 706f   mzdata2mat impo
+00000470: 7274 206d 7a44 6174 614d 616e 6167 6572  rt mzDataManager
+00000480: 0a0a 6d7a 4461 7461 4d61 6e61 6765 7228  ..mzDataManager(
+00000490: 7573 6544 6972 6563 746f 7279 3d46 616c  useDirectory=Fal
+000004a0: 7365 292e 636f 6e76 6572 7446 696c 6528  se).convertFile(
+000004b0: 3c70 6174 6832 6d7a 4461 7461 4669 6c65  <path2mzDataFile
+000004c0: 3e2c 203c 7061 7468 3266 6f6c 6465 7232  >, <path2folder2
+000004d0: 7361 7665 3e29 0a0a 9468 075d 9468 168c  save>)...h.].h..
+000004e0: 7c66 726f 6d20 6d7a 6461 7461 326d 6174  |from mzdata2mat
+000004f0: 2069 6d70 6f72 7420 6d7a 4461 7461 4d61   import mzDataMa
+00000500: 6e61 6765 720a 0a6d 7a44 6174 614d 616e  nager..mzDataMan
+00000510: 6167 6572 2875 7365 4469 7265 6374 6f72  ager(useDirector
+00000520: 793d 4661 6c73 6529 2e63 6f6e 7665 7274  y=False).convert
+00000530: 4669 6c65 283c 7061 7468 326d 7a44 6174  File(<path2mzDat
+00000540: 6146 696c 653e 2c20 3c70 6174 6832 666f  aFile>, <path2fo
+00000550: 6c64 6572 3273 6176 653e 290a 0a94 8594  lder2save>).....
+00000560: 8194 7d94 681b 685e 7362 6168 1f7d 9428  ..}.h.h^sbah.}.(
+00000570: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00000580: 6829 5d94 8c08 6c61 6e67 7561 6765 948c  h)]...language..
+00000590: 0670 7974 686f 6e94 8c09 786d 6c3a 7370  .python...xml:sp
+000005a0: 6163 6594 8c08 7072 6573 6572 7665 9475  ace...preserve.u
+000005b0: 682b 685c 681d 682c 681e 4b07 681b 683d  h+h\h.h,h.K.h.h=
+000005c0: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
+000005d0: 8c0c 696e 2d74 776f 2d6c 696e 6573 9461  ..in-two-lines.a
+000005e0: 6823 5d94 6825 5d94 8c0c 696e 2074 776f  h#].h%]...in two
+000005f0: 206c 696e 6573 9461 6827 5d94 6829 5d94   lines.ah'].h)].
+00000600: 7568 2b68 0a68 1e4b 0468 1d68 2c68 1b68  uh+h.h.K.h.h,h.h
+00000610: 0c68 1c68 0375 6268 0b29 8194 7d94 2868  .h.h.ubh.)..}.(h
+00000620: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
+00000630: 6805 8c16 4d6f 7265 2064 6574 6169 6c6c  h...More detaill
+00000640: 6564 2065 7861 6d70 6c65 9468 075d 9468  ed example.h.].h
+00000650: 168c 164d 6f72 6520 6465 7461 696c 6c65  ...More detaille
+00000660: 6420 6578 616d 706c 6594 8594 8194 7d94  d example.....}.
+00000670: 2868 1b68 7b68 1c68 0368 1d4e 681e 4e75  (h.h{h.h.h.Nh.Nu
+00000680: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00000690: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
+000006a0: 681e 4b0d 681d 682c 681b 6878 681c 6803  h.K.h.h,h.hxh.h.
+000006b0: 7562 685d 2981 947d 9428 6805 58c8 0200  ubh])..}.(h.X...
+000006c0: 000a 2320 4865 7265 2077 6520 696d 706f  ..# Here we impo
+000006d0: 7274 2074 6865 206d 6169 6e20 636c 6173  rt the main clas
+000006e0: 7320 7573 6564 2066 6f72 2074 6865 2063  s used for the c
+000006f0: 6f6e 7665 7273 696f 6e2e 0a31 2066 726f  onversion..1 fro
+00000700: 6d20 6d7a 6461 7461 326d 6174 2069 6d70  m mzdata2mat imp
+00000710: 6f72 7420 6d7a 4461 7461 4d61 6e61 6765  ort mzDataManage
+00000720: 720a 0a23 2057 6520 696e 6974 6961 6c69  r..# We initiali
+00000730: 7a65 2074 6865 2063 6c61 7373 0a23 2049  ze the class.# I
+00000740: 6620 616c 6c20 6d7a 4461 7461 2066 696c  f all mzData fil
+00000750: 6573 2061 7265 2073 746f 7265 6420 696e  es are stored in
+00000760: 2074 6865 2073 616d 6520 6469 7265 6374   the same direct
+00000770: 6f72 792c 2077 6520 6361 6e20 7370 6563  ory, we can spec
+00000780: 6966 7920 7468 6520 7061 7261 6d65 7465  ify the paramete
+00000790: 7220 606d 7a44 6174 6150 6174 6860 2069  r `mzDataPath` i
+000007a0: 6e73 7465 6164 206f 6620 6075 7365 4469  nstead of `useDi
+000007b0: 7265 6374 6f72 7960 2e0a 3220 636f 6e76  rectory`..2 conv
+000007c0: 6572 7465 7241 6765 6e74 203d 206d 7a44  erterAgent = mzD
+000007d0: 6174 614d 616e 6167 6572 2875 7365 4469  ataManager(useDi
+000007e0: 7265 6374 6f72 793d 4661 6c73 6529 0a0a  rectory=False)..
+000007f0: 3320 7061 7468 326d 7a44 6174 6146 696c  3 path2mzDataFil
+00000800: 6520 3a20 7374 7220 3d20 2270 6174 682f  e : str = "path/
+00000810: 746f 2f73 746f 7265 642f 6669 6c65 7322  to/stored/files"
+00000820: 0a0a 3420 736f 6d65 4469 7265 6374 6f72  ..4 someDirector
+00000830: 7920 3a20 7374 7220 3d20 2270 6174 682f  y : str = "path/
+00000840: 746f 2f73 6176 652f 6669 6c65 2f22 0a0a  to/save/file/"..
+00000850: 2320 4e6f 7720 7765 2063 616e 2063 616c  # Now we can cal
+00000860: 6c20 7468 6520 6d7a 4461 7461 584d 4c72  l the mzDataXMLr
+00000870: 6561 6420 6675 6e63 7469 6f6e 2074 6f20  ead function to 
+00000880: 7265 6164 2074 6865 202e 6d7a 4461 7461  read the .mzData
+00000890: 2e78 6d6c 2066 696c 653a 0a35 2064 6174  .xml file:.5 dat
+000008a0: 6120 3d20 636f 6e76 6572 7465 7241 6765  a = converterAge
+000008b0: 6e74 2e6d 7a44 6174 6158 4d4c 7265 6164  nt.mzDataXMLread
+000008c0: 2866 696c 654e 616d 653d 7061 7468 326d  (fileName=path2m
+000008d0: 7a44 6174 6146 696c 6529 0a0a 2320 5468  zDataFile)..# Th
+000008e0: 6520 6461 7461 2077 6527 7665 2067 6f74  e data we've got
+000008f0: 2066 726f 6d20 7468 6520 7072 6576 696f   from the previo
+00000900: 7573 2066 756e 6374 696f 6e20 6361 6e20  us function can 
+00000910: 6265 2073 6176 6564 2074 6f20 6120 2e6d  be saved to a .m
+00000920: 6174 2066 696c 6520 7769 7468 2074 6865  at file with the
+00000930: 2073 6176 654d 6174 6669 6c65 2066 756e   saveMatfile fun
+00000940: 7469 6f6e 3a0a 3620 636f 6e76 6572 7465  tion:.6 converte
+00000950: 7241 6765 6e74 2e73 6176 654d 6174 6669  rAgent.saveMatfi
+00000960: 6c65 286d 7a44 6174 613d 6461 7461 2c20  le(mzData=data, 
+00000970: 6469 7232 7361 7665 3d73 6f6d 6544 6972  dir2save=someDir
+00000980: 6563 746f 7279 290a 0a94 6807 5d94 6816  ectory)...h.].h.
+00000990: 58c8 0200 000a 2320 4865 7265 2077 6520  X.....# Here we 
+000009a0: 696d 706f 7274 2074 6865 206d 6169 6e20  import the main 
+000009b0: 636c 6173 7320 7573 6564 2066 6f72 2074  class used for t
+000009c0: 6865 2063 6f6e 7665 7273 696f 6e2e 0a31  he conversion..1
+000009d0: 2066 726f 6d20 6d7a 6461 7461 326d 6174   from mzdata2mat
+000009e0: 2069 6d70 6f72 7420 6d7a 4461 7461 4d61   import mzDataMa
+000009f0: 6e61 6765 720a 0a23 2057 6520 696e 6974  nager..# We init
+00000a00: 6961 6c69 7a65 2074 6865 2063 6c61 7373  ialize the class
+00000a10: 0a23 2049 6620 616c 6c20 6d7a 4461 7461  .# If all mzData
+00000a20: 2066 696c 6573 2061 7265 2073 746f 7265   files are store
+00000a30: 6420 696e 2074 6865 2073 616d 6520 6469  d in the same di
+00000a40: 7265 6374 6f72 792c 2077 6520 6361 6e20  rectory, we can 
+00000a50: 7370 6563 6966 7920 7468 6520 7061 7261  specify the para
+00000a60: 6d65 7465 7220 606d 7a44 6174 6150 6174  meter `mzDataPat
+00000a70: 6860 2069 6e73 7465 6164 206f 6620 6075  h` instead of `u
+00000a80: 7365 4469 7265 6374 6f72 7960 2e0a 3220  seDirectory`..2 
+00000a90: 636f 6e76 6572 7465 7241 6765 6e74 203d  converterAgent =
+00000aa0: 206d 7a44 6174 614d 616e 6167 6572 2875   mzDataManager(u
+00000ab0: 7365 4469 7265 6374 6f72 793d 4661 6c73  seDirectory=Fals
+00000ac0: 6529 0a0a 3320 7061 7468 326d 7a44 6174  e)..3 path2mzDat
+00000ad0: 6146 696c 6520 3a20 7374 7220 3d20 2270  aFile : str = "p
+00000ae0: 6174 682f 746f 2f73 746f 7265 642f 6669  ath/to/stored/fi
+00000af0: 6c65 7322 0a0a 3420 736f 6d65 4469 7265  les"..4 someDire
+00000b00: 6374 6f72 7920 3a20 7374 7220 3d20 2270  ctory : str = "p
+00000b10: 6174 682f 746f 2f73 6176 652f 6669 6c65  ath/to/save/file
+00000b20: 2f22 0a0a 2320 4e6f 7720 7765 2063 616e  /"..# Now we can
+00000b30: 2063 616c 6c20 7468 6520 6d7a 4461 7461   call the mzData
+00000b40: 584d 4c72 6561 6420 6675 6e63 7469 6f6e  XMLread function
+00000b50: 2074 6f20 7265 6164 2074 6865 202e 6d7a   to read the .mz
+00000b60: 4461 7461 2e78 6d6c 2066 696c 653a 0a35  Data.xml file:.5
+00000b70: 2064 6174 6120 3d20 636f 6e76 6572 7465   data = converte
+00000b80: 7241 6765 6e74 2e6d 7a44 6174 6158 4d4c  rAgent.mzDataXML
+00000b90: 7265 6164 2866 696c 654e 616d 653d 7061  read(fileName=pa
+00000ba0: 7468 326d 7a44 6174 6146 696c 6529 0a0a  th2mzDataFile)..
+00000bb0: 2320 5468 6520 6461 7461 2077 6527 7665  # The data we've
+00000bc0: 2067 6f74 2066 726f 6d20 7468 6520 7072   got from the pr
+00000bd0: 6576 696f 7573 2066 756e 6374 696f 6e20  evious function 
+00000be0: 6361 6e20 6265 2073 6176 6564 2074 6f20  can be saved to 
+00000bf0: 6120 2e6d 6174 2066 696c 6520 7769 7468  a .mat file with
+00000c00: 2074 6865 2073 6176 654d 6174 6669 6c65   the saveMatfile
+00000c10: 2066 756e 7469 6f6e 3a0a 3620 636f 6e76   funtion:.6 conv
+00000c20: 6572 7465 7241 6765 6e74 2e73 6176 654d  erterAgent.saveM
+00000c30: 6174 6669 6c65 286d 7a44 6174 613d 6461  atfile(mzData=da
+00000c40: 7461 2c20 6469 7232 7361 7665 3d73 6f6d  ta, dir2save=som
+00000c50: 6544 6972 6563 746f 7279 290a 0a94 8594  eDirectory).....
+00000c60: 8194 7d94 681b 6889 7362 6168 1f7d 9428  ..}.h.h.sbah.}.(
+00000c70: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00000c80: 6829 5d94 8c08 6c61 6e67 7561 6765 948c  h)]...language..
+00000c90: 0670 7974 686f 6e94 686e 686f 7568 2b68  .python.hnhouh+h
+00000ca0: 5c68 1d68 2c68 1e4b 0f68 1b68 7868 1c68  \h.h,h.K.h.hxh.h
+00000cb0: 0375 6265 681f 7d94 2868 215d 948c 166d  .ubeh.}.(h!]...m
+00000cc0: 6f72 652d 6465 7461 696c 6c65 642d 6578  ore-detailled-ex
+00000cd0: 616d 706c 6594 6168 235d 9468 255d 948c  ample.ah#].h%]..
+00000ce0: 166d 6f72 6520 6465 7461 696c 6c65 6420  .more detailled 
+00000cf0: 6578 616d 706c 6594 6168 275d 9468 295d  example.ah'].h)]
+00000d00: 9475 682b 680a 681e 4b0d 681d 682c 681b  .uh+h.h.K.h.h,h.
+00000d10: 680c 681c 6803 7562 6568 1f7d 9428 6821  h.h.h.ubeh.}.(h!
+00000d20: 5d94 8c0c 6578 616d 706c 652d 636f 6465  ]...example-code
+00000d30: 9461 6823 5d94 6825 5d94 8c0c 6578 616d  .ah#].h%]...exam
+00000d40: 706c 6520 636f 6465 9461 6827 5d94 6829  ple code.ah'].h)
+00000d50: 5d94 7568 2b68 0a68 1e4b 0168 1d68 2c68  ].uh+h.h.K.h.h,h
+00000d60: 1b68 0368 1c68 0375 6261 681f 7d94 2868  .h.h.h.ubah.}.(h
+00000d70: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00000d80: 295d 948c 0673 6f75 7263 6594 682c 8c14  )]...source.h,..
+00000d90: 7472 616e 736c 6174 696f 6e5f 7072 6f67  translation_prog
+00000da0: 7265 7373 947d 9428 8c05 746f 7461 6c94  ress.}.(..total.
+00000db0: 4b00 8c0a 7472 616e 736c 6174 6564 944b  K...translated.K
+00000dc0: 0075 7568 2b68 018c 0e63 7572 7265 6e74  .uuh+h...current
+00000dd0: 5f73 6f75 7263 6594 4e8c 0c63 7572 7265  _source.N..curre
+00000de0: 6e74 5f6c 696e 6594 4e8c 0873 6574 7469  nt_line.N..setti
+00000df0: 6e67 7394 8c11 646f 6375 7469 6c73 2e66  ngs...docutils.f
+00000e00: 726f 6e74 656e 6494 8c06 5661 6c75 6573  rontend...Values
+00000e10: 9493 9429 8194 7d94 288c 066f 7574 7075  ...)..}.(..outpu
+00000e20: 7494 4e68 0f4e 8c09 6765 6e65 7261 746f  t.Nh.N..generato
+00000e30: 7294 4e8c 0964 6174 6573 7461 6d70 944e  r.N..datestamp.N
+00000e40: 8c0b 736f 7572 6365 5f6c 696e 6b94 4e8c  ..source_link.N.
+00000e50: 0a73 6f75 7263 655f 7572 6c94 4e8c 0d74  .source_url.N..t
+00000e60: 6f63 5f62 6163 6b6c 696e 6b73 948c 0565  oc_backlinks...e
+00000e70: 6e74 7279 948c 1266 6f6f 746e 6f74 655f  ntry...footnote_
+00000e80: 6261 636b 6c69 6e6b 7394 4b01 8c0d 7365  backlinks.K...se
+00000e90: 6374 6e75 6d5f 7866 6f72 6d94 4b01 8c0e  ctnum_xform.K...
+00000ea0: 7374 7269 705f 636f 6d6d 656e 7473 944e  strip_comments.N
+00000eb0: 8c1b 7374 7269 705f 656c 656d 656e 7473  ..strip_elements
+00000ec0: 5f77 6974 685f 636c 6173 7365 7394 4e8c  _with_classes.N.
+00000ed0: 0d73 7472 6970 5f63 6c61 7373 6573 944e  .strip_classes.N
+00000ee0: 8c0c 7265 706f 7274 5f6c 6576 656c 944b  ..report_level.K
+00000ef0: 028c 0a68 616c 745f 6c65 7665 6c94 4b05  ...halt_level.K.
+00000f00: 8c11 6578 6974 5f73 7461 7475 735f 6c65  ..exit_status_le
+00000f10: 7665 6c94 4b05 8c05 6465 6275 6794 4e8c  vel.K...debug.N.
+00000f20: 0e77 6172 6e69 6e67 5f73 7472 6561 6d94  .warning_stream.
+00000f30: 4e8c 0974 7261 6365 6261 636b 9488 8c0e  N..traceback....
+00000f40: 696e 7075 745f 656e 636f 6469 6e67 948c  input_encoding..
+00000f50: 0975 7466 2d38 2d73 6967 948c 1c69 6e70  .utf-8-sig...inp
+00000f60: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
+00000f70: 725f 6861 6e64 6c65 7294 8c06 7374 7269  r_handler...stri
+00000f80: 6374 948c 0f6f 7574 7075 745f 656e 636f  ct...output_enco
+00000f90: 6469 6e67 948c 0575 7466 2d38 948c 1d6f  ding...utf-8...o
+00000fa0: 7574 7075 745f 656e 636f 6469 6e67 5f65  utput_encoding_e
+00000fb0: 7272 6f72 5f68 616e 646c 6572 9468 d18c  rror_handler.h..
+00000fc0: 0e65 7272 6f72 5f65 6e63 6f64 696e 6794  .error_encoding.
+00000fd0: 8c05 7574 662d 3894 8c1c 6572 726f 725f  ..utf-8...error_
+00000fe0: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
+00000ff0: 616e 646c 6572 948c 1062 6163 6b73 6c61  andler...backsla
+00001000: 7368 7265 706c 6163 6594 8c0d 6c61 6e67  shreplace...lang
+00001010: 7561 6765 5f63 6f64 6594 8c02 656e 948c  uage_code...en..
+00001020: 1372 6563 6f72 645f 6465 7065 6e64 656e  .record_dependen
+00001030: 6369 6573 944e 8c06 636f 6e66 6967 944e  cies.N..config.N
+00001040: 8c09 6964 5f70 7265 6669 7894 6806 8c0e  ..id_prefix.h...
+00001050: 6175 746f 5f69 645f 7072 6566 6978 948c  auto_id_prefix..
+00001060: 0269 6494 8c0d 6475 6d70 5f73 6574 7469  .id...dump_setti
+00001070: 6e67 7394 4e8c 0e64 756d 705f 696e 7465  ngs.N..dump_inte
+00001080: 726e 616c 7394 4e8c 0f64 756d 705f 7472  rnals.N..dump_tr
+00001090: 616e 7366 6f72 6d73 944e 8c0f 6475 6d70  ansforms.N..dump
+000010a0: 5f70 7365 7564 6f5f 786d 6c94 4e8c 1065  _pseudo_xml.N..e
+000010b0: 7870 6f73 655f 696e 7465 726e 616c 7394  xpose_internals.
+000010c0: 4e8c 0e73 7472 6963 745f 7669 7369 746f  N..strict_visito
+000010d0: 7294 4e8c 0f5f 6469 7361 626c 655f 636f  r.N.._disable_co
+000010e0: 6e66 6967 944e 8c07 5f73 6f75 7263 6594  nfig.N.._source.
+000010f0: 682c 8c0c 5f64 6573 7469 6e61 7469 6f6e  h,.._destination
+00001100: 944e 8c0d 5f63 6f6e 6669 675f 6669 6c65  .N.._config_file
+00001110: 7394 5d94 8c16 6669 6c65 5f69 6e73 6572  s.]...file_inser
+00001120: 7469 6f6e 5f65 6e61 626c 6564 9488 8c0b  tion_enabled....
+00001130: 7261 775f 656e 6162 6c65 6494 4b01 8c11  raw_enabled.K...
+00001140: 6c69 6e65 5f6c 656e 6774 685f 6c69 6d69  line_length_limi
+00001150: 7494 4d10 278c 0e70 6570 5f72 6566 6572  t.M.'..pep_refer
+00001160: 656e 6365 7394 4e8c 0c70 6570 5f62 6173  ences.N..pep_bas
+00001170: 655f 7572 6c94 8c18 6874 7470 733a 2f2f  e_url...https://
+00001180: 7065 7073 2e70 7974 686f 6e2e 6f72 672f  peps.python.org/
+00001190: 948c 1570 6570 5f66 696c 655f 7572 6c5f  ...pep_file_url_
+000011a0: 7465 6d70 6c61 7465 948c 0870 6570 2d25  template...pep-%
+000011b0: 3034 6494 8c0e 7266 635f 7265 6665 7265  04d...rfc_refere
+000011c0: 6e63 6573 944e 8c0c 7266 635f 6261 7365  nces.N..rfc_base
+000011d0: 5f75 726c 948c 2668 7474 7073 3a2f 2f64  _url..&https://d
+000011e0: 6174 6174 7261 636b 6572 2e69 6574 662e  atatracker.ietf.
+000011f0: 6f72 672f 646f 632f 6874 6d6c 2f94 8c09  org/doc/html/...
+00001200: 7461 625f 7769 6474 6894 4b08 8c1d 7472  tab_width.K...tr
+00001210: 696d 5f66 6f6f 746e 6f74 655f 7265 6665  im_footnote_refe
+00001220: 7265 6e63 655f 7370 6163 6594 898c 1073  rence_space....s
+00001230: 796e 7461 785f 6869 6768 6c69 6768 7494  yntax_highlight.
+00001240: 8c04 6c6f 6e67 948c 0c73 6d61 7274 5f71  ..long...smart_q
+00001250: 756f 7465 7394 888c 1373 6d61 7274 7175  uotes....smartqu
+00001260: 6f74 6573 5f6c 6f63 616c 6573 945d 948c  otes_locales.]..
+00001270: 1d63 6861 7261 6374 6572 5f6c 6576 656c  .character_level
+00001280: 5f69 6e6c 696e 655f 6d61 726b 7570 9489  _inline_markup..
+00001290: 8c0e 646f 6374 6974 6c65 5f78 666f 726d  ..doctitle_xform
+000012a0: 9489 8c0d 646f 6369 6e66 6f5f 7866 6f72  ....docinfo_xfor
+000012b0: 6d94 4b01 8c12 7365 6374 7375 6274 6974  m.K...sectsubtit
+000012c0: 6c65 5f78 666f 726d 9489 8c0d 696d 6167  le_xform....imag
+000012d0: 655f 6c6f 6164 696e 6794 8c04 6c69 6e6b  e_loading...link
+000012e0: 948c 1065 6d62 6564 5f73 7479 6c65 7368  ...embed_stylesh
+000012f0: 6565 7494 898c 1563 6c6f 616b 5f65 6d61  eet....cloak_ema
+00001300: 696c 5f61 6464 7265 7373 6573 9488 8c11  il_addresses....
+00001310: 7365 6374 696f 6e5f 7365 6c66 5f6c 696e  section_self_lin
+00001320: 6b94 898c 0365 6e76 944e 7562 8c08 7265  k....env.Nub..re
+00001330: 706f 7274 6572 944e 8c10 696e 6469 7265  porter.N..indire
+00001340: 6374 5f74 6172 6765 7473 945d 948c 1173  ct_targets.]...s
+00001350: 7562 7374 6974 7574 696f 6e5f 6465 6673  ubstitution_defs
+00001360: 947d 9428 8c0f 776f 7264 636f 756e 742d  .}.(..wordcount-
+00001370: 776f 7264 7394 6809 8c17 7375 6273 7469  words.h...substi
+00001380: 7475 7469 6f6e 5f64 6566 696e 6974 696f  tution_definitio
+00001390: 6e94 9394 2981 947d 9428 6805 8c02 3338  n...)..}.(h...38
+000013a0: 9468 075d 9468 168c 0233 3894 8594 8194  .h.].h...38.....
+000013b0: 7d94 681b 6a0f 0100 0073 6261 681f 7d94  }.h.j....sbah.}.
+000013c0: 2868 215d 9468 235d 9468 255d 948c 0f77  (h!].h#].h%]...w
+000013d0: 6f72 6463 6f75 6e74 2d77 6f72 6473 9461  ordcount-words.a
+000013e0: 6827 5d94 6829 5d94 7568 2b6a 0d01 0000  h'].h)].uh+j....
+000013f0: 681d 682c 7562 8c11 776f 7264 636f 756e  h.h,ub..wordcoun
+00001400: 742d 6d69 6e75 7465 7394 6a0e 0100 0029  t-minutes.j....)
+00001410: 8194 7d94 2868 058c 0130 9468 075d 9468  ..}.(h...0.h.].h
+00001420: 168c 0130 9485 9481 947d 9468 1b6a 1f01  ...0.....}.h.j..
+00001430: 0000 7362 6168 1f7d 9428 6821 5d94 6823  ..sbah.}.(h!].h#
+00001440: 5d94 6825 5d94 8c11 776f 7264 636f 756e  ].h%]...wordcoun
+00001450: 742d 6d69 6e75 7465 7394 6168 275d 9468  t-minutes.ah'].h
+00001460: 295d 9475 682b 6a0d 0100 0068 1d68 2c75  )].uh+j....h.h,u
+00001470: 6275 8c12 7375 6273 7469 7475 7469 6f6e  bu..substitution
+00001480: 5f6e 616d 6573 947d 9428 8c0f 776f 7264  _names.}.(..word
+00001490: 636f 756e 742d 776f 7264 7394 6a0c 0100  count-words.j...
+000014a0: 008c 1177 6f72 6463 6f75 6e74 2d6d 696e  ...wordcount-min
+000014b0: 7574 6573 946a 1e01 0000 758c 0872 6566  utes.j....u..ref
+000014c0: 6e61 6d65 7394 7d94 8c06 7265 6669 6473  names.}...refids
+000014d0: 947d 948c 076e 616d 6569 6473 947d 9428  .}...nameids.}.(
+000014e0: 68a6 68a3 6875 6872 689e 689b 758c 096e  h.h.huhrh.h.u..n
+000014f0: 616d 6574 7970 6573 947d 9428 68a6 8968  ametypes.}.(h..h
+00001500: 7589 689e 8975 6821 7d94 2868 a368 0c68  u.h..uh!}.(h.h.h
+00001510: 7268 3d68 9b68 7875 8c0d 666f 6f74 6e6f  rh=h.hxu..footno
+00001520: 7465 5f72 6566 7394 7d94 8c0d 6369 7461  te_refs.}...cita
+00001530: 7469 6f6e 5f72 6566 7394 7d94 8c0d 6175  tion_refs.}...au
+00001540: 746f 666f 6f74 6e6f 7465 7394 5d94 8c11  tofootnotes.]...
+00001550: 6175 746f 666f 6f74 6e6f 7465 5f72 6566  autofootnote_ref
+00001560: 7394 5d94 8c10 7379 6d62 6f6c 5f66 6f6f  s.]...symbol_foo
+00001570: 746e 6f74 6573 945d 948c 1473 796d 626f  tnotes.]...symbo
+00001580: 6c5f 666f 6f74 6e6f 7465 5f72 6566 7394  l_footnote_refs.
+00001590: 5d94 8c09 666f 6f74 6e6f 7465 7394 5d94  ]...footnotes.].
+000015a0: 8c09 6369 7461 7469 6f6e 7394 5d94 8c12  ..citations.]...
+000015b0: 6175 746f 666f 6f74 6e6f 7465 5f73 7461  autofootnote_sta
+000015c0: 7274 944b 018c 1573 796d 626f 6c5f 666f  rt.K...symbol_fo
+000015d0: 6f74 6e6f 7465 5f73 7461 7274 944b 008c  otnote_start.K..
+000015e0: 0a69 645f 636f 756e 7465 7294 8c0b 636f  .id_counter...co
+000015f0: 6c6c 6563 7469 6f6e 7394 8c07 436f 756e  llections...Coun
+00001600: 7465 7294 9394 7d94 8594 5294 8c0e 7061  ter...}...R...pa
+00001610: 7273 655f 6d65 7373 6167 6573 945d 948c  rse_messages.]..
+00001620: 1274 7261 6e73 666f 726d 5f6d 6573 7361  .transform_messa
+00001630: 6765 7394 5d94 8c0b 7472 616e 7366 6f72  ges.]...transfor
+00001640: 6d65 7294 4e8c 0b69 6e63 6c75 6465 5f6c  mer.N..include_l
+00001650: 6f67 945d 948c 0a64 6563 6f72 6174 696f  og.]...decoratio
+00001660: 6e94 4e68 1c68 038c 0a6d 7973 745f 736c  n.Nh.h...myst_sl
+00001670: 7567 7394 7d94 7562 2e                   ugs.}.ub.
```

### Comparing `mzdata2mat-0.1.1/docs/build/doctrees/index.doctree` & `mzdata2mat-0.2.0/docs/build/doctrees/index.doctree`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 95d9 3600 0000 0000 008c 0f73 7068  ....6........sph
+00000000: 8005 95e2 3800 0000 0000 008c 0f73 7068  ....8........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
 00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
 00000060: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
 00000070: 6805 8ccf 6d7a 6461 7461 326d 6174 2064  h...mzdata2mat d
@@ -38,842 +38,874 @@
 00000250: 948c 0763 6c61 7373 6573 945d 948c 056e  ...classes.]...n
 00000260: 616d 6573 945d 948c 0864 7570 6e61 6d65  ames.]...dupname
 00000270: 7394 5d94 8c08 6261 636b 7265 6673 945d  s.]...backrefs.]
 00000280: 948c 0978 6d6c 3a73 7061 6365 948c 0870  ...xml:space...p
 00000290: 7265 7365 7276 6594 758c 0774 6167 6e61  reserve.u..tagna
 000002a0: 6d65 9468 0a68 1668 038c 095f 646f 6375  me.h.h.h..._docu
 000002b0: 6d65 6e74 9468 038c 0673 6f75 7263 6594  ment.h...source.
-000002c0: 8c74 2f55 7365 7273 2f6c 6963 6839 3131  .t/Users/lich911
-000002d0: 2f4c 6962 7261 7279 2f43 6c6f 7564 5374  /Library/CloudSt
-000002e0: 6f72 6167 652f 4f6e 6544 7269 7665 2d50  orage/OneDrive-P
-000002f0: 6572 736f 6e6e 656c 2f44 6f63 756d 656e  ersonnel/Documen
-00000300: 7473 2f50 7974 686f 6e2f 5061 636b 6167  ts/Python/Packag
-00000310: 6573 2f6d 7a44 6174 6158 4d4c 324d 6174  es/mzDataXML2Mat
-00000320: 2f64 6f63 732f 736f 7572 6365 2f69 6e64  /docs/source/ind
-00000330: 6578 2e72 7374 948c 046c 696e 6594 4b05  ex.rst...line.K.
-00000340: 7562 6809 8c07 7365 6374 696f 6e94 9394  ubh...section...
-00000350: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
-00000360: 098c 0574 6974 6c65 9493 9429 8194 7d94  ...title...)..}.
-00000370: 2868 058c 0757 656c 636f 6d65 9468 075d  (h...Welcome.h.]
-00000380: 9468 118c 0757 656c 636f 6d65 9485 9481  .h...Welcome....
-00000390: 947d 9428 6816 6831 6826 6803 6827 4e68  .}.(h.h1h&h.h'Nh
-000003a0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-000003b0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-000003c0: 2568 2f68 1668 2c68 2668 0368 2768 2868  %h/h.h,h&h.h'h(h
-000003d0: 294b 0775 6268 098c 0970 6172 6167 7261  )K.ubh...paragra
-000003e0: 7068 9493 9429 8194 7d94 2868 058c d757  ph...)..}.(h...W
-000003f0: 656c 636f 6d65 2021 2060 606d 7a64 6174  elcome ! ``mzdat
-00000400: 6132 6d61 7460 6020 6973 2061 2050 7974  a2mat`` is a Pyt
-00000410: 686f 6e20 7061 636b 6167 6520 6672 6f6d  hon package from
-00000420: 2060 4c41 5254 4943 2072 6573 6561 7263   `LARTIC researc
-00000430: 6820 7465 616d 203c 6874 7470 733a 2f2f  h team <https://
-00000440: 6c61 7274 6963 2e66 7361 612e 756c 6176  lartic.fsaa.ulav
-00000450: 616c 2e63 612f 3e60 5f5f 2c20 7768 6963  al.ca/>`__, whic
-00000460: 6820 636f 6e76 6572 7473 206d 7a44 6174  h converts mzDat
-00000470: 612e 786d 6c20 6669 6c65 7320 2876 6572  a.xml files (ver
-00000480: 7369 6f6e 2031 2e30 352c 2041 6769 6c65  sion 1.05, Agile
-00000490: 6e74 2054 6563 686e 6f6c 6f67 6965 7329  nt Technologies)
-000004a0: 2069 6e74 6f20 6d61 7420 6669 6c65 7320   into mat files 
-000004b0: 7265 6164 6162 6c65 2075 7369 6e67 206d  readable using m
-000004c0: 6174 6c61 622e 9468 075d 9428 6811 8c0a  atlab..h.].(h...
-000004d0: 5765 6c63 6f6d 6520 2120 9485 9481 947d  Welcome ! .....}
-000004e0: 9428 6816 6841 6826 6803 6827 4e68 294e  .(h.hAh&h.h'Nh)N
-000004f0: 7562 6809 8c07 6c69 7465 7261 6c94 9394  ubh...literal...
-00000500: 2981 947d 9428 6805 8c0e 6060 6d7a 6461  )..}.(h...``mzda
-00000510: 7461 326d 6174 6060 9468 075d 9468 118c  ta2mat``.h.].h..
-00000520: 0a6d 7a64 6174 6132 6d61 7494 8594 8194  .mzdata2mat.....
-00000530: 7d94 2868 1668 4b68 2668 0368 274e 6829  }.(h.hKh&h.h'Nh)
-00000540: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
-00000550: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
-00000560: 6849 6816 6841 7562 6811 8c1a 2069 7320  hIh.hAubh... is 
-00000570: 6120 5079 7468 6f6e 2070 6163 6b61 6765  a Python package
-00000580: 2066 726f 6d20 9485 9481 947d 9428 6816   from .....}.(h.
-00000590: 6841 6826 6803 6827 4e68 294e 7562 6809  hAh&h.h'Nh)Nubh.
-000005a0: 8c09 7265 6665 7265 6e63 6594 9394 2981  ..reference...).
-000005b0: 947d 9428 6805 8c39 604c 4152 5449 4320  .}.(h..9`LARTIC 
-000005c0: 7265 7365 6172 6368 2074 6561 6d20 3c68  research team <h
-000005d0: 7474 7073 3a2f 2f6c 6172 7469 632e 6673  ttps://lartic.fs
-000005e0: 6161 2e75 6c61 7661 6c2e 6361 2f3e 605f  aa.ulaval.ca/>`_
-000005f0: 5f94 6807 5d94 6811 8c14 4c41 5254 4943  _.h.].h...LARTIC
-00000600: 2072 6573 6561 7263 6820 7465 616d 9485   research team..
-00000610: 9481 947d 9428 6816 685f 6826 6803 6827  ...}.(h.h_h&h.h'
-00000620: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00000630: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00000640: 8c04 6e61 6d65 948c 144c 4152 5449 4320  ..name...LARTIC 
-00000650: 7265 7365 6172 6368 2074 6561 6d94 8c06  research team...
-00000660: 7265 6675 7269 948c 1e68 7474 7073 3a2f  refuri...https:/
-00000670: 2f6c 6172 7469 632e 6673 6161 2e75 6c61  /lartic.fsaa.ula
-00000680: 7661 6c2e 6361 2f94 7568 2568 5d68 1668  val.ca/.uh%h]h.h
-00000690: 4175 6268 118c 6c2c 2077 6869 6368 2063  Aubh..l, which c
-000006a0: 6f6e 7665 7274 7320 6d7a 4461 7461 2e78  onverts mzData.x
-000006b0: 6d6c 2066 696c 6573 2028 7665 7273 696f  ml files (versio
-000006c0: 6e20 312e 3035 2c20 4167 696c 656e 7420  n 1.05, Agilent 
-000006d0: 5465 6368 6e6f 6c6f 6769 6573 2920 696e  Technologies) in
-000006e0: 746f 206d 6174 2066 696c 6573 2072 6561  to mat files rea
-000006f0: 6461 626c 6520 7573 696e 6720 6d61 746c  dable using matl
-00000700: 6162 2e94 8594 8194 7d94 2868 1668 4168  ab......}.(h.hAh
-00000710: 2668 0368 274e 6829 4e75 6265 6817 7d94  &h.h'Nh)Nubeh.}.
-00000720: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00000730: 9468 215d 9475 6825 683f 6827 6828 6829  .h!].uh%h?h'h(h)
-00000740: 4b09 6816 682c 6826 6803 7562 6840 2981  K.h.h,h&h.ubh@).
-00000750: 947d 9428 6805 8c1d 4175 7468 6f72 203a  .}.(h...Author :
-00000760: 204d 6178 696d 6520 522e 412e 2043 6f72   Maxime R.A. Cor
-00000770: 6465 6c6c 6194 6807 5d94 6811 8c1d 4175  della.h.].h...Au
-00000780: 7468 6f72 203a 204d 6178 696d 6520 522e  thor : Maxime R.
-00000790: 412e 2043 6f72 6465 6c6c 6194 8594 8194  A. Cordella.....
-000007a0: 7d94 2868 1668 7b68 2668 0368 274e 6829  }.(h.h{h&h.h'Nh)
-000007b0: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
-000007c0: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
-000007d0: 683f 6827 6828 6829 4b0c 6816 682c 6826  h?h'h(h)K.h.h,h&
-000007e0: 6803 7562 6840 2981 947d 9428 6805 8c2a  h.ubh@)..}.(h..*
-000007f0: 5465 616d 206c 6561 6465 7220 3a20 5072  Team leader : Pr
-00000800: 2e20 4368 7269 7374 6f70 6865 2042 2e59  . Christophe B.Y
-00000810: 2e20 436f 7264 656c 6c61 9468 075d 9468  . Cordella.h.].h
-00000820: 118c 2a54 6561 6d20 6c65 6164 6572 203a  ..*Team leader :
-00000830: 2050 722e 2043 6872 6973 746f 7068 6520   Pr. Christophe 
-00000840: 422e 592e 2043 6f72 6465 6c6c 6194 8594  B.Y. Cordella...
-00000850: 8194 7d94 2868 1668 8968 2668 0368 274e  ..}.(h.h.h&h.h'N
-00000860: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
-00000870: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
-00000880: 6825 683f 6827 6828 6829 4b0e 6816 682c  h%h?h'h(h)K.h.h,
-00000890: 6826 6803 7562 6840 2981 947d 9428 6805  h&h.ubh@)..}.(h.
-000008a0: 8c17 436f 7079 7269 6768 7428 6329 3230  ..Copyright(c)20
-000008b0: 3234 5f4c 4152 5449 4394 6807 5d94 6811  24_LARTIC.h.].h.
-000008c0: 8c17 436f 7079 7269 6768 7428 6329 3230  ..Copyright(c)20
-000008d0: 3234 5f4c 4152 5449 4394 8594 8194 7d94  24_LARTIC.....}.
-000008e0: 2868 1668 9768 2668 0368 274e 6829 4e75  (h.h.h&h.h'Nh)Nu
-000008f0: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
-00000900: 1d5d 9468 1f5d 9468 215d 9475 6825 683f  .].h.].h!].uh%h?
-00000910: 6827 6828 6829 4b10 6816 682c 6826 6803  h'h(h)K.h.h,h&h.
-00000920: 7562 6840 2981 947d 9428 6805 8c29 7c44  ubh@)..}.(h..)|D
-00000930: 6f63 756d 656e 7461 7469 6f6e 2053 7461  ocumentation Sta
-00000940: 7475 737c 207c 5079 5049 7c20 7c64 6f77  tus| |PyPI| |dow
-00000950: 6e6c 6f61 6473 7c94 6807 5d94 2868 5e29  nloads|.h.].(h^)
-00000960: 8194 7d94 2868 075d 9468 098c 0569 6d61  ..}.(h.].h...ima
-00000970: 6765 9493 9429 8194 7d94 2868 075d 9468  ge...)..}.(h.].h
-00000980: 058c 8f69 6d61 6765 3a3a 2068 7474 7073  ...image:: https
-00000990: 3a2f 2f72 6561 6474 6865 646f 6373 2e6f  ://readthedocs.o
-000009a0: 7267 2f70 726f 6a65 6374 732f 6d7a 6461  rg/projects/mzda
-000009b0: 7461 326d 6174 2f62 6164 6765 2f3f 7665  ta2mat/badge/?ve
-000009c0: 7273 696f 6e3d 6c61 7465 7374 0a20 2020  rsion=latest.   
-000009d0: 3a74 6172 6765 743a 2068 7474 7073 3a2f  :target: https:/
-000009e0: 2f6d 7a64 6174 6132 6d61 742e 7265 6164  /mzdata2mat.read
-000009f0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000a00: 7465 7374 2f3f 6261 6467 653d 6c61 7465  test/?badge=late
-00000a10: 7374 9468 2568 ac68 177d 9428 6819 5d94  st.h%h.h.}.(h.].
-00000a20: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00000a30: 8c03 616c 7494 8c14 446f 6375 6d65 6e74  ..alt...Document
-00000a40: 6174 696f 6e20 5374 6174 7573 948c 0375  ation Status...u
-00000a50: 7269 948c 4168 7474 7073 3a2f 2f72 6561  ri..Ahttps://rea
-00000a60: 6474 6865 646f 6373 2e6f 7267 2f70 726f  dthedocs.org/pro
-00000a70: 6a65 6374 732f 6d7a 6461 7461 326d 6174  jects/mzdata2mat
-00000a80: 2f62 6164 6765 2f3f 7665 7273 696f 6e3d  /badge/?version=
-00000a90: 6c61 7465 7374 948c 0a63 616e 6469 6461  latest...candida
-00000aa0: 7465 7394 7d94 8c01 3f94 68bb 7375 6829  tes.}...?.h.suh)
-00000ab0: 4b00 6827 6828 6816 68a9 6826 6803 7562  K.h'h(h.h.h&h.ub
-00000ac0: 6168 0568 b968 2568 5d68 177d 9428 6819  ah.h.h%h]h.}.(h.
-00000ad0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-00000ae0: 5d94 8c06 7265 6675 7269 948c 3968 7474  ]...refuri..9htt
-00000af0: 7073 3a2f 2f6d 7a64 6174 6132 6d61 742e  ps://mzdata2mat.
-00000b00: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00000b10: 6e2f 6c61 7465 7374 2f3f 6261 6467 653d  n/latest/?badge=
-00000b20: 6c61 7465 7374 9475 6829 4e68 274e 6816  latest.uh)Nh'Nh.
-00000b30: 68a5 6826 6803 7562 6811 8c01 2094 8594  h.h&h.ubh... ...
-00000b40: 8194 7d94 2868 1668 a568 2668 0368 274e  ..}.(h.h.h&h.h'N
-00000b50: 6829 4e75 6268 5e29 8194 7d94 2868 075d  h)Nubh^)..}.(h.]
-00000b60: 9468 ad29 8194 7d94 2868 075d 9468 058c  .h.)..}.(h.].h..
-00000b70: 6169 6d61 6765 3a3a 2068 7474 7073 3a2f  aimage:: https:/
-00000b80: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000b90: 7079 7069 2f76 2f6d 7a64 6174 6132 6d61  pypi/v/mzdata2ma
-00000ba0: 740a 2020 203a 7461 7267 6574 3a20 6874  t.   :target: ht
-00000bb0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000bc0: 726f 6a65 6374 2f6d 7a64 6174 6132 6d61  roject/mzdata2ma
-00000bd0: 742f 9468 2568 ac68 177d 9428 6819 5d94  t/.h%h.h.}.(h.].
-00000be0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00000bf0: 8c03 616c 7494 8c04 5079 5049 948c 0375  ..alt...PyPI...u
-00000c00: 7269 948c 2868 7474 7073 3a2f 2f69 6d67  ri..(https://img
-00000c10: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000c20: 2f76 2f6d 7a64 6174 6132 6d61 7494 68bc  /v/mzdata2mat.h.
-00000c30: 7d94 68be 68db 7375 6829 4b00 6827 6828  }.h.h.suh)K.h'h(
-00000c40: 6816 68cb 6826 6803 7562 6168 0568 d968  h.h.h&h.ubah.h.h
-00000c50: 2568 5d68 177d 9428 6819 5d94 681b 5d94  %h]h.}.(h.].h.].
-00000c60: 681d 5d94 681f 5d94 6821 5d94 8c06 7265  h.].h.].h!]...re
-00000c70: 6675 7269 948c 2468 7474 7073 3a2f 2f70  furi..$https://p
-00000c80: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000c90: 6d7a 6461 7461 326d 6174 2f94 7568 294e  mzdata2mat/.uh)N
-00000ca0: 6827 4e68 1668 a568 2668 0375 6268 118c  h'Nh.h.h&h.ubh..
-00000cb0: 0120 9485 9481 947d 9468 1668 a573 6268  . .....}.h.h.sbh
-00000cc0: 5e29 8194 7d94 2868 075d 9468 ad29 8194  ^)..}.(h.].h.)..
-00000cd0: 7d94 2868 075d 9468 058c 6869 6d61 6765  }.(h.].h..himage
-00000ce0: 3a3a 2068 7474 7073 3a2f 2f73 7461 7469  :: https://stati
-00000cf0: 632e 7065 7079 2e74 6563 682f 6261 6467  c.pepy.tech/badg
-00000d00: 652f 6d7a 6461 7461 326d 6174 2f6d 6f6e  e/mzdata2mat/mon
-00000d10: 7468 0a20 2020 3a74 6172 6765 743a 2068  th.   :target: h
-00000d20: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-00000d30: 2f70 726f 6a65 6374 2f6d 7a64 6174 6132  /project/mzdata2
-00000d40: 6d61 7494 6825 68ac 6817 7d94 2868 195d  mat.h%h.h.}.(h.]
-00000d50: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
-00000d60: 948c 0361 6c74 948c 0964 6f77 6e6c 6f61  ...alt...downloa
-00000d70: 6473 948c 0375 7269 948c 2f68 7474 7073  ds...uri../https
-00000d80: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
-00000d90: 6563 682f 6261 6467 652f 6d7a 6461 7461  ech/badge/mzdata
-00000da0: 326d 6174 2f6d 6f6e 7468 9468 bc7d 9468  2mat/month.h.}.h
-00000db0: be68 f973 7568 294b 0068 2768 2868 1668  .h.suh)K.h'h(h.h
-00000dc0: e968 2668 0375 6261 6805 68f7 6825 685d  .h&h.ubah.h.h%h]
-00000dd0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-00000de0: 9468 1f5d 9468 215d 948c 0672 6566 7572  .h.].h!]...refur
-00000df0: 6994 8c24 6874 7470 733a 2f2f 7065 7079  i..$https://pepy
-00000e00: 2e74 6563 682f 7072 6f6a 6563 742f 6d7a  .tech/project/mz
-00000e10: 6461 7461 326d 6174 9475 6829 4e68 274e  data2mat.uh)Nh'N
-00000e20: 6816 68a5 6826 6803 7562 6568 177d 9428  h.h.h&h.ubeh.}.(
-00000e30: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-00000e40: 6821 5d94 7568 2568 3f68 2768 2868 294b  h!].uh%h?h'h(h)K
-00000e50: 1268 1668 2c68 2668 0375 6268 2b29 8194  .h.h,h&h.ubh+)..
-00000e60: 7d94 2868 0568 0668 075d 9428 6830 2981  }.(h.h.h.].(h0).
-00000e70: 947d 9428 6805 8c19 4375 7272 656e 7420  .}.(h...Current 
-00000e80: 7665 7273 696f 6e20 6060 302e 312e 3060  version ``0.1.0`
-00000e90: 6094 6807 5d94 2868 118c 1043 7572 7265  `.h.].(h...Curre
-00000ea0: 6e74 2076 6572 7369 6f6e 2094 8594 8194  nt version .....
-00000eb0: 7d94 2868 166a 0c01 0000 6826 6803 6827  }.(h.j....h&h.h'
-00000ec0: 4e68 294e 7562 684a 2981 947d 9428 6805  Nh)NubhJ)..}.(h.
-00000ed0: 8c09 6060 302e 312e 3060 6094 6807 5d94  ..``0.1.0``.h.].
-00000ee0: 6811 8c05 302e 312e 3094 8594 8194 7d94  h...0.1.0.....}.
-00000ef0: 2868 166a 1401 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
-00000f00: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-00000f10: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-00000f20: 2568 4968 166a 0c01 0000 7562 6568 177d  %hIh.j....ubeh.}
-00000f30: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00000f40: 5d94 6821 5d94 7568 2568 2f68 166a 0901  ].h!].uh%h/h.j..
-00000f50: 0000 6826 6803 6827 6828 6829 4b15 7562  ..h&h.h'h(h)K.ub
-00000f60: 6840 2981 947d 9428 6805 8c3e 5468 6520  h@)..}.(h..>The 
-00000f70: 6375 7272 656e 7420 7665 7273 696f 6e20  current version 
-00000f80: 6f66 206d 7a64 6174 6132 6d61 7420 6973  of mzdata2mat is
-00000f90: 2074 6865 2066 6f6c 6c6f 7769 6e67 203a   the following :
-00000fa0: 2060 6030 2e31 2e30 6060 9468 075d 9428   ``0.1.0``.h.].(
-00000fb0: 6811 8c35 5468 6520 6375 7272 656e 7420  h..5The current 
-00000fc0: 7665 7273 696f 6e20 6f66 206d 7a64 6174  version of mzdat
-00000fd0: 6132 6d61 7420 6973 2074 6865 2066 6f6c  a2mat is the fol
-00000fe0: 6c6f 7769 6e67 203a 2094 8594 8194 7d94  lowing : .....}.
-00000ff0: 2868 166a 2801 0000 6826 6803 6827 4e68  (h.j(...h&h.h'Nh
-00001000: 294e 7562 684a 2981 947d 9428 6805 8c09  )NubhJ)..}.(h...
-00001010: 6060 302e 312e 3060 6094 6807 5d94 6811  ``0.1.0``.h.].h.
-00001020: 8c05 302e 312e 3094 8594 8194 7d94 2868  ..0.1.0.....}.(h
-00001030: 166a 3001 0000 6826 6803 6827 4e68 294e  .j0...h&h.h'Nh)N
-00001040: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00001050: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-00001060: 4968 166a 2801 0000 7562 6568 177d 9428  Ih.j(...ubeh.}.(
-00001070: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-00001080: 6821 5d94 7568 2568 3f68 2768 2868 294b  h!].uh%h?h'h(h)K
-00001090: 1768 166a 0901 0000 6826 6803 7562 6840  .h.j....h&h.ubh@
-000010a0: 2981 947d 9428 6805 8c3c 596f 7520 6361  )..}.(h..<You ca
-000010b0: 6e20 7365 6520 7468 6520 636f 6d70 6c65  n see the comple
-000010c0: 7465 2063 6861 6e67 656c 6f67 2060 6865  te changelog `he
-000010d0: 7265 203c 4368 616e 6765 6c6f 672e 6874  re <Changelog.ht
-000010e0: 6d6c 3e60 5f5f 9468 075d 9428 6811 8c23  ml>`__.h.].(h..#
-000010f0: 596f 7520 6361 6e20 7365 6520 7468 6520  You can see the 
-00001100: 636f 6d70 6c65 7465 2063 6861 6e67 656c  complete changel
-00001110: 6f67 2094 8594 8194 7d94 2868 166a 4401  og .....}.(h.jD.
-00001120: 0000 6826 6803 6827 4e68 294e 7562 685e  ..h&h.h'Nh)Nubh^
-00001130: 2981 947d 9428 6805 8c19 6068 6572 6520  )..}.(h...`here 
-00001140: 3c43 6861 6e67 656c 6f67 2e68 746d 6c3e  <Changelog.html>
-00001150: 605f 5f94 6807 5d94 6811 8c04 6865 7265  `__.h.].h...here
-00001160: 9485 9481 947d 9428 6816 6a4c 0100 0068  .....}.(h.jL...h
-00001170: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-00001180: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00001190: 9468 215d 948c 046e 616d 6594 8c04 6865  .h!]...name...he
-000011a0: 7265 9468 6f8c 0e43 6861 6e67 656c 6f67  re.ho..Changelog
-000011b0: 2e68 746d 6c94 7568 2568 5d68 166a 4401  .html.uh%h]h.jD.
-000011c0: 0000 7562 6568 177d 9428 6819 5d94 681b  ..ubeh.}.(h.].h.
-000011d0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-000011e0: 2568 3f68 2768 2868 294b 1968 166a 0901  %h?h'h(h)K.h.j..
-000011f0: 0000 6826 6803 7562 6568 177d 9428 6819  ..h&h.ubeh.}.(h.
-00001200: 5d94 8c15 6375 7272 656e 742d 7665 7273  ]...current-vers
-00001210: 696f 6e2d 302d 312d 3094 6168 1b5d 9468  ion-0-1-0.ah.].h
-00001220: 1d5d 948c 1563 7572 7265 6e74 2076 6572  .]...current ver
-00001230: 7369 6f6e 2030 2e31 2e30 9461 681f 5d94  sion 0.1.0.ah.].
-00001240: 6821 5d94 7568 2568 2a68 1668 2c68 2668  h!].uh%h*h.h,h&h
-00001250: 0368 2768 2868 294b 1575 6268 2b29 8194  .h'h(h)K.ubh+)..
-00001260: 7d94 2868 0568 0668 075d 9428 6830 2981  }.(h.h.h.].(h0).
-00001270: 947d 9428 6805 8c13 436f 6d70 6174 6962  .}.(h...Compatib
-00001280: 6c65 2068 6172 6477 6172 6594 6807 5d94  le hardware.h.].
-00001290: 6811 8c13 436f 6d70 6174 6962 6c65 2068  h...Compatible h
-000012a0: 6172 6477 6172 6594 8594 8194 7d94 2868  ardware.....}.(h
-000012b0: 166a 6e01 0000 6826 6803 6827 4e68 294e  .jn...h&h.h'Nh)N
-000012c0: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-000012d0: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-000012e0: 2f68 166a 6b01 0000 6826 6803 6827 6828  /h.jk...h&h.h'h(
-000012f0: 6829 4b1c 7562 6840 2981 947d 9428 6805  h)K.ubh@)..}.(h.
-00001300: 8c33 4174 2074 6869 7320 7469 6d65 2c20  .3At this time, 
-00001310: 7468 6520 666f 6c6c 6f77 696e 6720 4f53  the following OS
-00001320: 6573 2068 6176 6520 6265 656e 2074 6573  es have been tes
-00001330: 7465 6420 3a94 6807 5d94 6811 8c33 4174  ted :.h.].h..3At
-00001340: 2074 6869 7320 7469 6d65 2c20 7468 6520   this time, the 
-00001350: 666f 6c6c 6f77 696e 6720 4f53 6573 2068  following OSes h
-00001360: 6176 6520 6265 656e 2074 6573 7465 6420  ave been tested 
-00001370: 3a94 8594 8194 7d94 2868 166a 7c01 0000  :.....}.(h.j|...
-00001380: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
-00001390: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-000013a0: 5d94 6821 5d94 7568 2568 3f68 2768 2868  ].h!].uh%h?h'h(h
-000013b0: 294b 1e68 166a 6b01 0000 6826 6803 7562  )K.h.jk...h&h.ub
-000013c0: 682b 2981 947d 9428 6805 6806 6807 5d94  h+)..}.(h.h.h.].
-000013d0: 2868 3029 8194 7d94 2868 058c 056d 6163  (h0)..}.(h...mac
-000013e0: 4f53 9468 075d 9468 118c 056d 6163 4f53  OS.h.].h...macOS
-000013f0: 9485 9481 947d 9428 6816 6a8d 0100 0068  .....}.(h.j....h
-00001400: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-00001410: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00001420: 9468 215d 9475 6825 682f 6816 6a8a 0100  .h!].uh%h/h.j...
-00001430: 0068 2668 0368 2768 2868 294b 2175 6268  .h&h.h'h(h)K!ubh
-00001440: 4029 8194 7d94 2868 058c 9a41 7420 7468  @)..}.(h...At th
-00001450: 6973 2074 696d 652c 2060 606d 6163 4f53  is time, ``macOS
-00001460: 2053 6f6e 6f6d 6120 3134 2e30 6060 2069   Sonoma 14.0`` i
-00001470: 7320 6f66 6669 6369 616c 6c79 2073 7570  s officially sup
-00001480: 706f 7274 6564 2c20 6f74 6865 7220 6d61  ported, other ma
-00001490: 634f 530a 7665 7273 696f 6e73 2063 6f75  cOS.versions cou
-000014a0: 6c64 2062 6520 7375 7070 6f72 7465 6420  ld be supported 
-000014b0: 6173 206c 6f6e 6720 6173 2074 6865 7920  as long as they 
-000014c0: 666f 6c6c 6f77 2074 6865 2072 6571 7569  follow the requi
-000014d0: 7265 6d65 6e74 730a 6c69 7374 6564 2062  rements.listed b
-000014e0: 656c 6f77 2e94 6807 5d94 2868 118c 0e41  elow..h.].(h...A
-000014f0: 7420 7468 6973 2074 696d 652c 2094 8594  t this time, ...
-00001500: 8194 7d94 2868 166a 9b01 0000 6826 6803  ..}.(h.j....h&h.
-00001510: 6827 4e68 294e 7562 684a 2981 947d 9428  h'Nh)NubhJ)..}.(
-00001520: 6805 8c15 6060 6d61 634f 5320 536f 6e6f  h...``macOS Sono
-00001530: 6d61 2031 342e 3060 6094 6807 5d94 6811  ma 14.0``.h.].h.
-00001540: 8c11 6d61 634f 5320 536f 6e6f 6d61 2031  ..macOS Sonoma 1
-00001550: 342e 3094 8594 8194 7d94 2868 166a a301  4.0.....}.(h.j..
-00001560: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
-00001570: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
-00001580: 681f 5d94 6821 5d94 7568 2568 4968 166a  h.].h!].uh%hIh.j
-00001590: 9b01 0000 7562 6811 8c77 2069 7320 6f66  ....ubh..w is of
-000015a0: 6669 6369 616c 6c79 2073 7570 706f 7274  ficially support
-000015b0: 6564 2c20 6f74 6865 7220 6d61 634f 530a  ed, other macOS.
-000015c0: 7665 7273 696f 6e73 2063 6f75 6c64 2062  versions could b
-000015d0: 6520 7375 7070 6f72 7465 6420 6173 206c  e supported as l
-000015e0: 6f6e 6720 6173 2074 6865 7920 666f 6c6c  ong as they foll
-000015f0: 6f77 2074 6865 2072 6571 7569 7265 6d65  ow the requireme
-00001600: 6e74 730a 6c69 7374 6564 2062 656c 6f77  nts.listed below
-00001610: 2e94 8594 8194 7d94 2868 166a 9b01 0000  ......}.(h.j....
-00001620: 6826 6803 6827 4e68 294e 7562 6568 177d  h&h.h'Nh)Nubeh.}
-00001630: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00001640: 5d94 6821 5d94 7568 2568 3f68 2768 2868  ].h!].uh%h?h'h(h
-00001650: 294b 2368 166a 8a01 0000 6826 6803 7562  )K#h.j....h&h.ub
-00001660: 6568 177d 9428 6819 5d94 8c05 6d61 636f  eh.}.(h.]...maco
-00001670: 7394 6168 1b5d 9468 1d5d 948c 056d 6163  s.ah.].h.]...mac
-00001680: 6f73 9461 681f 5d94 6821 5d94 7568 2568  os.ah.].h!].uh%h
-00001690: 2a68 166a 6b01 0000 6826 6803 6827 6828  *h.jk...h&h.h'h(
-000016a0: 6829 4b21 7562 682b 2981 947d 9428 6805  h)K!ubh+)..}.(h.
-000016b0: 6806 6807 5d94 2868 3029 8194 7d94 2868  h.h.].(h0)..}.(h
-000016c0: 058c 0757 696e 646f 7773 9468 075d 9468  ...Windows.h.].h
-000016d0: 118c 0757 696e 646f 7773 9485 9481 947d  ...Windows.....}
-000016e0: 9428 6816 6ac6 0100 0068 2668 0368 274e  .(h.j....h&h.h'N
-000016f0: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
-00001700: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
-00001710: 6825 682f 6816 6ac3 0100 0068 2668 0368  h%h/h.j....h&h.h
-00001720: 2768 2868 294b 2875 6268 4029 8194 7d94  'h(h)K(ubh@)..}.
-00001730: 2868 058c e141 7420 7468 6973 2074 696d  (h...At this tim
-00001740: 652c 2060 606d 7a64 6174 6132 6d61 7460  e, ``mzdata2mat`
-00001750: 6020 6861 7665 2062 6565 6e20 7465 7374  ` have been test
-00001760: 6564 2061 6e64 2069 7320 7375 7070 6f72  ed and is suppor
-00001770: 7465 6420 6f6e 0a60 6057 696e 646f 7773  ted on.``Windows
-00001780: 2031 3160 602c 206e 6f20 7465 7374 696e   11``, no testin
-00001790: 6720 6861 7320 6265 656e 2064 6f6e 6520  g has been done 
-000017a0: 6f6e 2057 696e 646f 7773 2031 3020 6f72  on Windows 10 or
-000017b0: 2037 2062 7574 2069 6620 796f 750a 7761   7 but if you.wa
-000017c0: 6e74 2074 6f20 6578 7465 6e64 2074 6865  nt to extend the
-000017d0: 2063 6f6d 7061 7469 6269 6c69 7479 2c20   compatibility, 
-000017e0: 7765 2061 7265 206f 7065 6e20 746f 2074  we are open to t
-000017f0: 6573 7465 72e2 8099 7320 6665 6564 6261  ester...s feedba
-00001800: 636b 206f 6e0a 7468 6f73 6573 206d 6163  ck on.thoses mac
-00001810: 6869 6e65 732e 9468 075d 9428 6811 8c0e  hines..h.].(h...
-00001820: 4174 2074 6869 7320 7469 6d65 2c20 9485  At this time, ..
-00001830: 9481 947d 9428 6816 6ad4 0100 0068 2668  ...}.(h.j....h&h
-00001840: 0368 274e 6829 4e75 6268 4a29 8194 7d94  .h'Nh)NubhJ)..}.
-00001850: 2868 058c 0e60 606d 7a64 6174 6132 6d61  (h...``mzdata2ma
-00001860: 7460 6094 6807 5d94 6811 8c0a 6d7a 6461  t``.h.].h...mzda
-00001870: 7461 326d 6174 9485 9481 947d 9428 6816  ta2mat.....}.(h.
-00001880: 6adc 0100 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
-00001890: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
-000018a0: 1d5d 9468 1f5d 9468 215d 9475 6825 6849  .].h.].h!].uh%hI
-000018b0: 6816 6ad4 0100 0075 6268 118c 2620 6861  h.j....ubh..& ha
-000018c0: 7665 2062 6565 6e20 7465 7374 6564 2061  ve been tested a
-000018d0: 6e64 2069 7320 7375 7070 6f72 7465 6420  nd is supported 
-000018e0: 6f6e 0a94 8594 8194 7d94 2868 166a d401  on......}.(h.j..
-000018f0: 0000 6826 6803 6827 4e68 294e 7562 684a  ..h&h.h'Nh)NubhJ
-00001900: 2981 947d 9428 6805 8c0e 6060 5769 6e64  )..}.(h...``Wind
-00001910: 6f77 7320 3131 6060 9468 075d 9468 118c  ows 11``.h.].h..
-00001920: 0a57 696e 646f 7773 2031 3194 8594 8194  .Windows 11.....
-00001930: 7d94 2868 166a ee01 0000 6826 6803 6827  }.(h.j....h&h.h'
-00001940: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00001950: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00001960: 7568 2568 4968 166a d401 0000 7562 6811  uh%hIh.j....ubh.
-00001970: 8c91 2c20 6e6f 2074 6573 7469 6e67 2068  .., no testing h
-00001980: 6173 2062 6565 6e20 646f 6e65 206f 6e20  as been done on 
-00001990: 5769 6e64 6f77 7320 3130 206f 7220 3720  Windows 10 or 7 
-000019a0: 6275 7420 6966 2079 6f75 0a77 616e 7420  but if you.want 
-000019b0: 746f 2065 7874 656e 6420 7468 6520 636f  to extend the co
-000019c0: 6d70 6174 6962 696c 6974 792c 2077 6520  mpatibility, we 
-000019d0: 6172 6520 6f70 656e 2074 6f20 7465 7374  are open to test
-000019e0: 6572 e280 9973 2066 6565 6462 6163 6b20  er...s feedback 
-000019f0: 6f6e 0a74 686f 7365 7320 6d61 6368 696e  on.thoses machin
-00001a00: 6573 2e94 8594 8194 7d94 2868 166a d401  es......}.(h.j..
-00001a10: 0000 6826 6803 6827 4e68 294e 7562 6568  ..h&h.h'Nh)Nubeh
-00001a20: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
-00001a30: 681f 5d94 6821 5d94 7568 2568 3f68 2768  h.].h!].uh%h?h'h
-00001a40: 2868 294b 2a68 166a c301 0000 6826 6803  (h)K*h.j....h&h.
-00001a50: 7562 6568 177d 9428 6819 5d94 8c07 7769  ubeh.}.(h.]...wi
-00001a60: 6e64 6f77 7394 6168 1b5d 9468 1d5d 948c  ndows.ah.].h.]..
-00001a70: 0777 696e 646f 7773 9461 681f 5d94 6821  .windows.ah.].h!
-00001a80: 5d94 7568 2568 2a68 166a 6b01 0000 6826  ].uh%h*h.jk...h&
-00001a90: 6803 6827 6828 6829 4b28 7562 6568 177d  h.h'h(h)K(ubeh.}
-00001aa0: 9428 6819 5d94 8c13 636f 6d70 6174 6962  .(h.]...compatib
-00001ab0: 6c65 2d68 6172 6477 6172 6594 6168 1b5d  le-hardware.ah.]
-00001ac0: 9468 1d5d 948c 1363 6f6d 7061 7469 626c  .h.]...compatibl
-00001ad0: 6520 6861 7264 7761 7265 9461 681f 5d94  e hardware.ah.].
-00001ae0: 6821 5d94 7568 2568 2a68 1668 2c68 2668  h!].uh%h*h.h,h&h
-00001af0: 0368 2768 2868 294b 1c75 6268 2b29 8194  .h'h(h)K.ubh+)..
-00001b00: 7d94 2868 0568 0668 075d 9428 6830 2981  }.(h.h.h.].(h0).
-00001b10: 947d 9428 6805 8c0c 5265 7175 6972 656d  .}.(h...Requirem
-00001b20: 656e 7473 9468 075d 9468 118c 0c52 6571  ents.h.].h...Req
-00001b30: 7569 7265 6d65 6e74 7394 8594 8194 7d94  uirements.....}.
-00001b40: 2868 166a 1902 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
-00001b50: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-00001b60: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-00001b70: 2568 2f68 166a 1602 0000 6826 6803 6827  %h/h.j....h&h.h'
-00001b80: 6828 6829 4b30 7562 682b 2981 947d 9428  h(h)K0ubh+)..}.(
-00001b90: 6805 6806 6807 5d94 2868 3029 8194 7d94  h.h.h.].(h0)..}.
-00001ba0: 2868 058c 114f 7468 6572 2074 6861 6e20  (h...Other than 
-00001bb0: 5079 7468 6f6e 9468 075d 9468 118c 114f  Python.h.].h...O
-00001bc0: 7468 6572 2074 6861 6e20 5079 7468 6f6e  ther than Python
-00001bd0: 9485 9481 947d 9428 6816 6a2a 0200 0068  .....}.(h.j*...h
-00001be0: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-00001bf0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00001c00: 9468 215d 9475 6825 682f 6816 6a27 0200  .h!].uh%h/h.j'..
-00001c10: 0068 2668 0368 2768 2868 294b 3375 6268  .h&h.h'h(h)K3ubh
-00001c20: 4029 8194 7d94 2868 058c ac54 6869 7320  @)..}.(h...This 
-00001c30: 7061 636b 6167 6520 2a2a 7265 7175 6972  package **requir
-00001c40: 6573 206e 6f64 652e 6a73 2069 6e73 7461  es node.js insta
-00001c50: 6c6c 6564 2a2a 2e20 796f 7520 6361 6e20  lled**. you can 
-00001c60: 646f 776e 6c6f 6164 2061 6e64 0a69 6e73  download and.ins
-00001c70: 7461 6c6c 2069 7420 6174 2060 6e6f 6465  tall it at `node
-00001c80: 6a73 2e6f 7267 203c 6874 7470 733a 2f2f  js.org <https://
-00001c90: 6e6f 6465 6a73 2e6f 7267 2f65 6e3e 605f  nodejs.org/en>`_
-00001ca0: 5f2e 2049 7420 6973 2061 7661 696c 6162  _. It is availab
-00001cb0: 6c65 0a66 6f72 2062 6f74 6820 6d61 634f  le.for both macO
-00001cc0: 5320 616e 6420 5769 6e64 6f77 7320 666f  S and Windows fo
-00001cd0: 7220 6672 6565 2e94 6807 5d94 2868 118c  r free..h.].(h..
-00001ce0: 0d54 6869 7320 7061 636b 6167 6520 9485  .This package ..
-00001cf0: 9481 947d 9428 6816 6a38 0200 0068 2668  ...}.(h.j8...h&h
-00001d00: 0368 274e 6829 4e75 6268 098c 0673 7472  .h'Nh)Nubh...str
-00001d10: 6f6e 6794 9394 2981 947d 9428 6805 8c1e  ong...)..}.(h...
-00001d20: 2a2a 7265 7175 6972 6573 206e 6f64 652e  **requires node.
-00001d30: 6a73 2069 6e73 7461 6c6c 6564 2a2a 9468  js installed**.h
-00001d40: 075d 9468 118c 1a72 6571 7569 7265 7320  .].h...requires 
-00001d50: 6e6f 6465 2e6a 7320 696e 7374 616c 6c65  node.js installe
-00001d60: 6494 8594 8194 7d94 2868 166a 4202 0000  d.....}.(h.jB...
-00001d70: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
-00001d80: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00001d90: 5d94 6821 5d94 7568 256a 4002 0000 6816  ].h!].uh%j@...h.
-00001da0: 6a38 0200 0075 6268 118c 252e 2079 6f75  j8...ubh..%. you
-00001db0: 2063 616e 2064 6f77 6e6c 6f61 6420 616e   can download an
-00001dc0: 640a 696e 7374 616c 6c20 6974 2061 7420  d.install it at 
-00001dd0: 9485 9481 947d 9428 6816 6a38 0200 0068  .....}.(h.j8...h
-00001de0: 2668 0368 274e 6829 4e75 6268 5e29 8194  &h.h'Nh)Nubh^)..
-00001df0: 7d94 2868 058c 2660 6e6f 6465 6a73 2e6f  }.(h..&`nodejs.o
-00001e00: 7267 203c 6874 7470 733a 2f2f 6e6f 6465  rg <https://node
-00001e10: 6a73 2e6f 7267 2f65 6e3e 605f 5f94 6807  js.org/en>`__.h.
-00001e20: 5d94 6811 8c0a 6e6f 6465 6a73 2e6f 7267  ].h...nodejs.org
-00001e30: 9485 9481 947d 9428 6816 6a54 0200 0068  .....}.(h.jT...h
-00001e40: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-00001e50: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00001e60: 9468 215d 948c 046e 616d 6594 8c0a 6e6f  .h!]...name...no
-00001e70: 6465 6a73 2e6f 7267 9468 6f8c 1568 7474  dejs.org.ho..htt
-00001e80: 7073 3a2f 2f6e 6f64 656a 732e 6f72 672f  ps://nodejs.org/
-00001e90: 656e 9475 6825 685d 6816 6a38 0200 0075  en.uh%h]h.j8...u
-00001ea0: 6268 118c 362e 2049 7420 6973 2061 7661  bh..6. It is ava
-00001eb0: 696c 6162 6c65 0a66 6f72 2062 6f74 6820  ilable.for both 
-00001ec0: 6d61 634f 5320 616e 6420 5769 6e64 6f77  macOS and Window
-00001ed0: 7320 666f 7220 6672 6565 2e94 8594 8194  s for free......
-00001ee0: 7d94 2868 166a 3802 0000 6826 6803 6827  }.(h.j8...h&h.h'
-00001ef0: 4e68 294e 7562 6568 177d 9428 6819 5d94  Nh)Nubeh.}.(h.].
-00001f00: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00001f10: 7568 2568 3f68 2768 2868 294b 3568 166a  uh%h?h'h(h)K5h.j
-00001f20: 2702 0000 6826 6803 7562 6568 177d 9428  '...h&h.ubeh.}.(
-00001f30: 6819 5d94 8c11 6f74 6865 722d 7468 616e  h.]...other-than
-00001f40: 2d70 7974 686f 6e94 6168 1b5d 9468 1d5d  -python.ah.].h.]
-00001f50: 948c 116f 7468 6572 2074 6861 6e20 7079  ...other than py
-00001f60: 7468 6f6e 9461 681f 5d94 6821 5d94 7568  thon.ah.].h!].uh
-00001f70: 2568 2a68 166a 1602 0000 6826 6803 6827  %h*h.j....h&h.h'
-00001f80: 6828 6829 4b33 7562 682b 2981 947d 9428  h(h)K3ubh+)..}.(
-00001f90: 6805 6806 6807 5d94 2868 3029 8194 7d94  h.h.h.].(h0)..}.
-00001fa0: 2868 058c 0e50 7974 686f 6e20 7665 7273  (h...Python vers
-00001fb0: 696f 6e94 6807 5d94 6811 8c0e 5079 7468  ion.h.].h...Pyth
-00001fc0: 6f6e 2076 6572 7369 6f6e 9485 9481 947d  on version.....}
-00001fd0: 9428 6816 6a7a 0200 0068 2668 0368 274e  .(h.jz...h&h.h'N
-00001fe0: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
-00001ff0: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
-00002000: 6825 682f 6816 6a77 0200 0068 2668 0368  h%h/h.jw...h&h.h
-00002010: 2768 2868 294b 3a75 6268 4029 8194 7d94  'h(h)K:ubh@)..}.
-00002020: 2868 058c 4d54 6869 7320 7061 636b 6167  (h..MThis packag
-00002030: 6520 6973 2063 6f6d 7061 7469 626c 6520  e is compatible 
-00002040: 746f 2061 6e79 2070 7974 686f 6e20 7665  to any python ve
-00002050: 7273 696f 6e20 6571 7561 6c20 6f72 206e  rsion equal or n
-00002060: 6577 6572 2074 6861 6e0a 6060 332e 3960  ewer than.``3.9`
-00002070: 602e 9468 075d 9428 6811 8c45 5468 6973  `..h.].(h..EThis
-00002080: 2070 6163 6b61 6765 2069 7320 636f 6d70   package is comp
-00002090: 6174 6962 6c65 2074 6f20 616e 7920 7079  atible to any py
-000020a0: 7468 6f6e 2076 6572 7369 6f6e 2065 7175  thon version equ
-000020b0: 616c 206f 7220 6e65 7765 7220 7468 616e  al or newer than
-000020c0: 0a94 8594 8194 7d94 2868 166a 8802 0000  ......}.(h.j....
-000020d0: 6826 6803 6827 4e68 294e 7562 684a 2981  h&h.h'Nh)NubhJ).
-000020e0: 947d 9428 6805 8c07 6060 332e 3960 6094  .}.(h...``3.9``.
-000020f0: 6807 5d94 6811 8c03 332e 3994 8594 8194  h.].h...3.9.....
-00002100: 7d94 2868 166a 9002 0000 6826 6803 6827  }.(h.j....h&h.h'
-00002110: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00002120: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00002130: 7568 2568 4968 166a 8802 0000 7562 6811  uh%hIh.j....ubh.
-00002140: 8c01 2e94 8594 8194 7d94 2868 166a 8802  ........}.(h.j..
-00002150: 0000 6826 6803 6827 4e68 294e 7562 6568  ..h&h.h'Nh)Nubeh
-00002160: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
-00002170: 681f 5d94 6821 5d94 7568 2568 3f68 2768  h.].h!].uh%h?h'h
-00002180: 2868 294b 3c68 166a 7702 0000 6826 6803  (h)K<h.jw...h&h.
-00002190: 7562 6568 177d 9428 6819 5d94 8c0e 7079  ubeh.}.(h.]...py
-000021a0: 7468 6f6e 2d76 6572 7369 6f6e 9461 681b  thon-version.ah.
-000021b0: 5d94 681d 5d94 8c0e 7079 7468 6f6e 2076  ].h.]...python v
-000021c0: 6572 7369 6f6e 9461 681f 5d94 6821 5d94  ersion.ah.].h!].
-000021d0: 7568 2568 2a68 166a 1602 0000 6826 6803  uh%h*h.j....h&h.
-000021e0: 6827 6828 6829 4b3a 7562 682b 2981 947d  h'h(h)K:ubh+)..}
-000021f0: 9428 6805 6806 6807 5d94 2868 3029 8194  .(h.h.h.].(h0)..
-00002200: 7d94 2868 058c 0f50 7974 686f 6e20 7061  }.(h...Python pa
-00002210: 636b 6167 6573 9468 075d 9468 118c 0f50  ckages.h.].h...P
-00002220: 7974 686f 6e20 7061 636b 6167 6573 9485  ython packages..
-00002230: 9481 947d 9428 6816 6ab3 0200 0068 2668  ...}.(h.j....h&h
-00002240: 0368 274e 6829 4e75 6261 6817 7d94 2868  .h'Nh)Nubah.}.(h
-00002250: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
-00002260: 215d 9475 6825 682f 6816 6ab0 0200 0068  !].uh%h/h.j....h
-00002270: 2668 0368 2768 2868 294b 4075 6268 4029  &h.h'h(h)K@ubh@)
-00002280: 8194 7d94 2868 058c 9157 6865 6e20 6d7a  ..}.(h...When mz
-00002290: 6461 7461 326d 6174 2077 696c 6c20 6265  data2mat will be
-000022a0: 2069 6e73 7461 6c6c 6564 206f 6e20 796f   installed on yo
-000022b0: 7572 2073 7973 7465 6d2c 2074 6865 2066  ur system, the f
-000022c0: 6f6c 6c6f 7769 6e67 2070 6163 6b61 6765  ollowing package
-000022d0: 730a 7769 6c6c 2061 6c73 6f20 6265 2069  s.will also be i
-000022e0: 6e73 7461 6c6c 6564 2028 6966 2074 6865  nstalled (if the
-000022f0: 7920 6172 6520 6e6f 7429 2069 6e74 6f20  y are not) into 
-00002300: 796f 7572 2050 7974 686f 6e20 656e 7669  your Python envi
-00002310: 7572 6f6e 6d65 6e74 203a 9468 075d 9468  uronment :.h.].h
-00002320: 118c 9157 6865 6e20 6d7a 6461 7461 326d  ...When mzdata2m
-00002330: 6174 2077 696c 6c20 6265 2069 6e73 7461  at will be insta
-00002340: 6c6c 6564 206f 6e20 796f 7572 2073 7973  lled on your sys
-00002350: 7465 6d2c 2074 6865 2066 6f6c 6c6f 7769  tem, the followi
-00002360: 6e67 2070 6163 6b61 6765 730a 7769 6c6c  ng packages.will
-00002370: 2061 6c73 6f20 6265 2069 6e73 7461 6c6c   also be install
-00002380: 6564 2028 6966 2074 6865 7920 6172 6520  ed (if they are 
-00002390: 6e6f 7429 2069 6e74 6f20 796f 7572 2050  not) into your P
-000023a0: 7974 686f 6e20 656e 7669 7572 6f6e 6d65  ython enviuronme
-000023b0: 6e74 203a 9485 9481 947d 9428 6816 6ac1  nt :.....}.(h.j.
-000023c0: 0200 0068 2668 0368 274e 6829 4e75 6261  ...h&h.h'Nh)Nuba
-000023d0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-000023e0: 9468 1f5d 9468 215d 9475 6825 683f 6827  .h.].h!].uh%h?h'
-000023f0: 6828 6829 4b42 6816 6ab0 0200 0068 2668  h(h)KBh.j....h&h
-00002400: 0375 6268 098c 0d6c 6974 6572 616c 5f62  .ubh...literal_b
-00002410: 6c6f 636b 9493 9429 8194 7d94 2868 058c  lock...)..}.(h..
-00002420: 3170 7964 616e 7469 633e 3d32 2e36 2e34  1pydantic>=2.6.4
-00002430: 0a6d 6174 3470 793e 3d30 2e36 2e30 0a6a  .mat4py>=0.6.0.j
-00002440: 6176 6173 6372 6970 743e 3d31 2131 2e31  avascript>=1!1.1
-00002450: 2e33 9468 075d 9468 118c 3170 7964 616e  .3.h.].h..1pydan
-00002460: 7469 633e 3d32 2e36 2e34 0a6d 6174 3470  tic>=2.6.4.mat4p
-00002470: 793e 3d30 2e36 2e30 0a6a 6176 6173 6372  y>=0.6.0.javascr
-00002480: 6970 743e 3d31 2131 2e31 2e33 9485 9481  ipt>=1!1.1.3....
-00002490: 947d 9468 166a d102 0000 7362 6168 177d  .}.h.j....sbah.}
-000024a0: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-000024b0: 5d94 6821 5d94 6823 6824 7568 256a cf02  ].h!].h#h$uh%j..
-000024c0: 0000 6827 6828 6829 4b47 6816 6ab0 0200  ..h'h(h)KGh.j...
-000024d0: 0068 2668 0375 6268 098c 1773 7562 7374  .h&h.ubh...subst
-000024e0: 6974 7574 696f 6e5f 6465 6669 6e69 7469  itution_definiti
-000024f0: 6f6e 9493 9429 8194 7d94 2868 058c a92e  on...)..}.(h....
-00002500: 2e20 7c44 6f63 756d 656e 7461 7469 6f6e  . |Documentation
-00002510: 2053 7461 7475 737c 2069 6d61 6765 3a3a   Status| image::
-00002520: 2068 7474 7073 3a2f 2f72 6561 6474 6865   https://readthe
-00002530: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
-00002540: 732f 6d7a 6461 7461 326d 6174 2f62 6164  s/mzdata2mat/bad
-00002550: 6765 2f3f 7665 7273 696f 6e3d 6c61 7465  ge/?version=late
-00002560: 7374 0a20 2020 3a74 6172 6765 743a 2068  st.   :target: h
-00002570: 7474 7073 3a2f 2f6d 7a64 6174 6132 6d61  ttps://mzdata2ma
-00002580: 742e 7265 6164 7468 6564 6f63 732e 696f  t.readthedocs.io
-00002590: 2f65 6e2f 6c61 7465 7374 2f3f 6261 6467  /en/latest/?badg
-000025a0: 653d 6c61 7465 7374 9468 075d 9468 5e29  e=latest.h.].h^)
-000025b0: 8194 7d94 2868 0568 b968 075d 9468 ad29  ..}.(h.h.h.].h.)
-000025c0: 8194 7d94 2868 0568 b168 075d 9468 177d  ..}.(h.h.h.].h.}
-000025d0: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-000025e0: 5d94 6821 5d94 68b8 68b9 68ba 68bb 68bc  ].h!].h.h.h.h.h.
-000025f0: 7d94 68be 68bb 7375 6825 68ac 6816 6ae5  }.h.h.suh%h.h.j.
-00002600: 0200 0068 2768 2868 294b 0075 6261 6817  ...h'h(h)K.ubah.
-00002610: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00002620: 1f5d 9468 215d 9468 c568 c675 6825 685d  .].h!].h.h.uh%h]
-00002630: 6816 6ae1 0200 0075 6261 6817 7d94 2868  h.j....ubah.}.(h
-00002640: 195d 9468 1b5d 9468 1d5d 9468 b961 681f  .].h.].h.].h.ah.
-00002650: 5d94 6821 5d94 7568 256a df02 0000 6827  ].h!].uh%j....h'
-00002660: 6828 6829 4b4b 6816 6ab0 0200 0068 2668  h(h)KKh.j....h&h
-00002670: 0375 626a e002 0000 2981 947d 9428 6805  .ubj....)..}.(h.
-00002680: 8c6b 2e2e 207c 5079 5049 7c20 696d 6167  .k.. |PyPI| imag
-00002690: 653a 3a20 6874 7470 733a 2f2f 696d 672e  e:: https://img.
-000026a0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-000026b0: 762f 6d7a 6461 7461 326d 6174 0a20 2020  v/mzdata2mat.   
-000026c0: 3a74 6172 6765 743a 2068 7474 7073 3a2f  :target: https:/
-000026d0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-000026e0: 742f 6d7a 6461 7461 326d 6174 2f94 6807  t/mzdata2mat/.h.
-000026f0: 5d94 685e 2981 947d 9428 6805 68d9 6807  ].h^)..}.(h.h.h.
-00002700: 5d94 68ad 2981 947d 9428 6805 68d1 6807  ].h.)..}.(h.h.h.
-00002710: 5d94 6817 7d94 2868 195d 9468 1b5d 9468  ].h.}.(h.].h.].h
-00002720: 1d5d 9468 1f5d 9468 215d 9468 d868 d968  .].h.].h!].h.h.h
-00002730: da68 db68 bc7d 9468 be68 db73 7568 2568  .h.h.}.h.h.suh%h
-00002740: ac68 166a 0203 0000 6827 6828 6829 4b00  .h.j....h'h(h)K.
-00002750: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00002760: 681d 5d94 681f 5d94 6821 5d94 68e3 68e4  h.].h.].h!].h.h.
-00002770: 7568 2568 5d68 166a fe02 0000 7562 6168  uh%h]h.j....ubah
-00002780: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
-00002790: 68d9 6168 1f5d 9468 215d 9475 6825 6adf  h.ah.].h!].uh%j.
-000027a0: 0200 0068 2768 2868 294b 4d68 166a b002  ...h'h(h)KMh.j..
-000027b0: 0000 6826 6803 7562 6ae0 0200 0029 8194  ..h&h.ubj....)..
-000027c0: 7d94 2868 058c 782e 2e20 7c64 6f77 6e6c  }.(h..x.. |downl
-000027d0: 6f61 6473 7c20 696d 6167 653a 3a20 6874  oads| image:: ht
-000027e0: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
-000027f0: 792e 7465 6368 2f62 6164 6765 2f6d 7a64  y.tech/badge/mzd
-00002800: 6174 6132 6d61 742f 6d6f 6e74 680a 2020  ata2mat/month.  
-00002810: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-00002820: 2f2f 7065 7079 2e74 6563 682f 7072 6f6a  //pepy.tech/proj
-00002830: 6563 742f 6d7a 6461 7461 326d 6174 0a94  ect/mzdata2mat..
-00002840: 6807 5d94 685e 2981 947d 9428 6805 68f7  h.].h^)..}.(h.h.
-00002850: 6807 5d94 68ad 2981 947d 9428 6805 68ef  h.].h.)..}.(h.h.
-00002860: 6807 5d94 6817 7d94 2868 195d 9468 1b5d  h.].h.}.(h.].h.]
-00002870: 9468 1d5d 9468 1f5d 9468 215d 9468 f668  .h.].h.].h!].h.h
-00002880: f768 f868 f968 bc7d 9468 be68 f973 7568  .h.h.h.}.h.h.suh
-00002890: 2568 ac68 166a 1f03 0000 6827 6828 6829  %h.h.j....h'h(h)
-000028a0: 4b00 7562 6168 177d 9428 6819 5d94 681b  K.ubah.}.(h.].h.
-000028b0: 5d94 681d 5d94 681f 5d94 6821 5d94 6a01  ].h.].h.].h!].j.
-000028c0: 0100 006a 0201 0000 7568 2568 5d68 166a  ...j....uh%h]h.j
-000028d0: 1b03 0000 7562 6168 177d 9428 6819 5d94  ....ubah.}.(h.].
-000028e0: 681b 5d94 681d 5d94 68f7 6168 1f5d 9468  h.].h.].h.ah.].h
-000028f0: 215d 9475 6825 6adf 0200 0068 2768 2868  !].uh%j....h'h(h
-00002900: 294b 4f68 166a b002 0000 6826 6803 7562  )KOh.j....h&h.ub
-00002910: 6809 8c08 636f 6d70 6f75 6e64 9493 9429  h...compound...)
-00002920: 8194 7d94 2868 0568 0668 075d 9468 008c  ..}.(h.h.h.].h..
-00002930: 0774 6f63 7472 6565 9493 9429 8194 7d94  .toctree...)..}.
-00002940: 2868 0568 0668 075d 9468 177d 9428 6819  (h.h.h.].h.}.(h.
-00002950: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-00002960: 5d94 6816 8c05 696e 6465 7894 8c07 656e  ].h...index...en
-00002970: 7472 6965 7394 5d94 4e8c 0943 6861 6e67  tries.].N..Chang
-00002980: 656c 6f67 9486 9461 8c0c 696e 636c 7564  elog...a..includ
-00002990: 6566 696c 6573 945d 946a 4b03 0000 618c  efiles.].jK...a.
-000029a0: 086d 6178 6465 7074 6894 4b04 8c07 6361  .maxdepth.K...ca
-000029b0: 7074 696f 6e94 8c05 496e 666f 7394 8c04  ption...Infos...
-000029c0: 676c 6f62 9489 8c06 6869 6464 656e 9488  glob....hidden..
-000029d0: 8c0d 696e 636c 7564 6568 6964 6465 6e94  ..includehidden.
-000029e0: 898c 086e 756d 6265 7265 6494 4b00 8c0a  ...numbered.K...
-000029f0: 7469 746c 6573 6f6e 6c79 9489 8c0a 7261  titlesonly....ra
-00002a00: 7765 6e74 7269 6573 945d 948c 0a72 6177  wentries.]...raw
-00002a10: 6361 7074 696f 6e94 6a51 0300 0075 6825  caption.jQ...uh%
-00002a20: 6a3d 0300 0068 2768 2868 294b 5268 166a  j=...h'h(h)KRh.j
-00002a30: 3a03 0000 7562 6168 177d 9428 6819 5d94  :...ubah.}.(h.].
-00002a40: 681b 5d94 8c0f 746f 6374 7265 652d 7772  h.]...toctree-wr
-00002a50: 6170 7065 7294 6168 1d5d 9468 1f5d 9468  apper.ah.].h.].h
-00002a60: 215d 9475 6825 6a38 0300 0068 166a b002  !].uh%j8...h.j..
-00002a70: 0000 6826 6803 6827 6828 6829 4e75 626a  ..h&h.h'h(h)Nubj
-00002a80: 3903 0000 2981 947d 9428 6805 6806 6807  9...)..}.(h.h.h.
-00002a90: 5d94 6a3e 0300 0029 8194 7d94 2868 0568  ].j>...)..}.(h.h
-00002aa0: 0668 075d 9468 177d 9428 6819 5d94 681b  .h.].h.}.(h.].h.
-00002ab0: 5d94 681d 5d94 681f 5d94 6821 5d94 6816  ].h.].h.].h!].h.
-00002ac0: 6a48 0300 006a 4903 0000 5d94 284e 8c0c  jH...jI...].(N..
-00002ad0: 696e 7374 616c 6c61 7469 6f6e 9486 944e  installation...N
-00002ae0: 8c0c 636f 6465 2d65 7861 6d70 6c65 9486  ..code-example..
-00002af0: 9465 6a4d 0300 005d 9428 6a6e 0300 006a  .ejM...].(jn...j
-00002b00: 7003 0000 656a 4f03 0000 4b04 6a50 0300  p...ejO...K.jP..
-00002b10: 008c 0a51 7569 636b 7374 6172 7494 6a52  ...Quickstart.jR
-00002b20: 0300 0089 6a53 0300 0088 6a54 0300 0089  ....jS....jT....
-00002b30: 6a55 0300 004b 006a 5603 0000 896a 5703  jU...K.jV....jW.
-00002b40: 0000 5d94 6a59 0300 006a 7303 0000 7568  ..].jY...js...uh
-00002b50: 256a 3d03 0000 6827 6828 6829 4b59 6816  %j=...h'h(h)KYh.
-00002b60: 6a61 0300 0075 6261 6817 7d94 2868 195d  ja...ubah.}.(h.]
-00002b70: 9468 1b5d 946a 5d03 0000 6168 1d5d 9468  .h.].j]...ah.].h
-00002b80: 1f5d 9468 215d 9475 6825 6a38 0300 0068  .].h!].uh%j8...h
-00002b90: 166a b002 0000 6826 6803 6827 6828 6829  .j....h&h.h'h(h)
-00002ba0: 4e75 626a 3903 0000 2981 947d 9428 6805  Nubj9...)..}.(h.
-00002bb0: 6806 6807 5d94 6a3e 0300 0029 8194 7d94  h.h.].j>...)..}.
-00002bc0: 2868 0568 0668 075d 9468 177d 9428 6819  (h.h.h.].h.}.(h.
-00002bd0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-00002be0: 5d94 6816 6a48 0300 006a 4903 0000 5d94  ].h.jH...jI...].
-00002bf0: 284e 8c0d 6d7a 4461 7461 4d61 6e61 6765  (N..mzDataManage
-00002c00: 7294 8694 4e8c 0c6d 6174 5374 7275 6374  r...N..matStruct
-00002c10: 7572 6594 8694 4e8c 066d 7a44 6174 6194  ure...N..mzData.
-00002c20: 8694 4e8c 116d 7a64 6174 6132 6d61 742d  ..N..mzdata2mat-
-00002c30: 7665 7269 6679 9486 944e 8c0f 6d7a 4461  verify...N..mzDa
-00002c40: 7461 584d 4c53 7472 7563 7494 8694 656a  taXMLStruct...ej
-00002c50: 4d03 0000 5d94 286a 8803 0000 6a8a 0300  M...].(j....j...
-00002c60: 006a 8c03 0000 6a8e 0300 006a 9003 0000  .j....j....j....
-00002c70: 656a 4f03 0000 4b04 6a50 0300 008c 0d41  ejO...K.jP.....A
-00002c80: 5049 2052 6566 6572 656e 6365 946a 5203  PI Reference.jR.
-00002c90: 0000 896a 5303 0000 886a 5403 0000 896a  ...jS....jT....j
-00002ca0: 5503 0000 4b00 6a56 0300 0089 6a57 0300  U...K.jV....jW..
-00002cb0: 005d 946a 5903 0000 6a93 0300 0075 6825  .].jY...j....uh%
-00002cc0: 6a3d 0300 0068 2768 2868 294b 6268 166a  j=...h'h(h)Kbh.j
-00002cd0: 7b03 0000 7562 6168 177d 9428 6819 5d94  {...ubah.}.(h.].
-00002ce0: 681b 5d94 6a5d 0300 0061 681d 5d94 681f  h.].j]...ah.].h.
-00002cf0: 5d94 6821 5d94 7568 256a 3803 0000 6816  ].h!].uh%j8...h.
-00002d00: 6ab0 0200 0068 2668 0368 2768 2868 294e  j....h&h.h'h(h)N
-00002d10: 7562 6568 177d 9428 6819 5d94 8c0f 7079  ubeh.}.(h.]...py
-00002d20: 7468 6f6e 2d70 6163 6b61 6765 7394 6168  thon-packages.ah
-00002d30: 1b5d 9468 1d5d 948c 0f70 7974 686f 6e20  .].h.]...python 
-00002d40: 7061 636b 6167 6573 9461 681f 5d94 6821  packages.ah.].h!
-00002d50: 5d94 7568 2568 2a68 166a 1602 0000 6826  ].uh%h*h.j....h&
-00002d60: 6803 6827 6828 6829 4b40 7562 6568 177d  h.h'h(h)K@ubeh.}
-00002d70: 9428 6819 5d94 8c0c 7265 7175 6972 656d  .(h.]...requirem
-00002d80: 656e 7473 9461 681b 5d94 681d 5d94 8c0c  ents.ah.].h.]...
-00002d90: 7265 7175 6972 656d 656e 7473 9461 681f  requirements.ah.
-00002da0: 5d94 6821 5d94 7568 2568 2a68 1668 2c68  ].h!].uh%h*h.h,h
-00002db0: 2668 0368 2768 2868 294b 3075 6265 6817  &h.h'h(h)K0ubeh.
-00002dc0: 7d94 2868 195d 948c 0777 656c 636f 6d65  }.(h.]...welcome
-00002dd0: 9461 681b 5d94 681d 5d94 8c07 7765 6c63  .ah.].h.]...welc
-00002de0: 6f6d 6594 6168 1f5d 9468 215d 9475 6825  ome.ah.].h!].uh%
-00002df0: 682a 6816 6803 6826 6803 6827 6828 6829  h*h.h.h&h.h'h(h)
-00002e00: 4b07 7562 6568 177d 9428 6819 5d94 681b  K.ubeh.}.(h.].h.
-00002e10: 5d94 681d 5d94 681f 5d94 6821 5d94 8c06  ].h.].h.].h!]...
-00002e20: 736f 7572 6365 9468 288c 1474 7261 6e73  source.h(..trans
-00002e30: 6c61 7469 6f6e 5f70 726f 6772 6573 7394  lation_progress.
-00002e40: 7d94 288c 0574 6f74 616c 944b 008c 0a74  }.(..total.K...t
-00002e50: 7261 6e73 6c61 7465 6494 4b00 7575 6825  ranslated.K.uuh%
-00002e60: 6801 8c0e 6375 7272 656e 745f 736f 7572  h...current_sour
-00002e70: 6365 944e 8c0c 6375 7272 656e 745f 6c69  ce.N..current_li
-00002e80: 6e65 944e 8c08 7365 7474 696e 6773 948c  ne.N..settings..
-00002e90: 1164 6f63 7574 696c 732e 6672 6f6e 7465  .docutils.fronte
-00002ea0: 6e64 948c 0656 616c 7565 7394 9394 2981  nd...Values...).
-00002eb0: 947d 9428 682f 4e8c 0967 656e 6572 6174  .}.(h/N..generat
-00002ec0: 6f72 944e 8c09 6461 7465 7374 616d 7094  or.N..datestamp.
-00002ed0: 4e8c 0b73 6f75 7263 655f 6c69 6e6b 944e  N..source_link.N
-00002ee0: 8c0a 736f 7572 6365 5f75 726c 944e 8c0d  ..source_url.N..
-00002ef0: 746f 635f 6261 636b 6c69 6e6b 7394 8c05  toc_backlinks...
-00002f00: 656e 7472 7994 8c12 666f 6f74 6e6f 7465  entry...footnote
-00002f10: 5f62 6163 6b6c 696e 6b73 944b 018c 0d73  _backlinks.K...s
-00002f20: 6563 746e 756d 5f78 666f 726d 944b 018c  ectnum_xform.K..
-00002f30: 0e73 7472 6970 5f63 6f6d 6d65 6e74 7394  .strip_comments.
-00002f40: 4e8c 1b73 7472 6970 5f65 6c65 6d65 6e74  N..strip_element
-00002f50: 735f 7769 7468 5f63 6c61 7373 6573 944e  s_with_classes.N
-00002f60: 8c0d 7374 7269 705f 636c 6173 7365 7394  ..strip_classes.
-00002f70: 4e8c 0c72 6570 6f72 745f 6c65 7665 6c94  N..report_level.
-00002f80: 4b02 8c0a 6861 6c74 5f6c 6576 656c 944b  K...halt_level.K
-00002f90: 058c 1165 7869 745f 7374 6174 7573 5f6c  ...exit_status_l
-00002fa0: 6576 656c 944b 058c 0564 6562 7567 944e  evel.K...debug.N
-00002fb0: 8c0e 7761 726e 696e 675f 7374 7265 616d  ..warning_stream
-00002fc0: 944e 8c09 7472 6163 6562 6163 6b94 888c  .N..traceback...
-00002fd0: 0e69 6e70 7574 5f65 6e63 6f64 696e 6794  .input_encoding.
-00002fe0: 8c09 7574 662d 382d 7369 6794 8c1c 696e  ..utf-8-sig...in
-00002ff0: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
-00003000: 6f72 5f68 616e 646c 6572 948c 0673 7472  or_handler...str
-00003010: 6963 7494 8c0f 6f75 7470 7574 5f65 6e63  ict...output_enc
-00003020: 6f64 696e 6794 8c05 7574 662d 3894 8c1d  oding...utf-8...
-00003030: 6f75 7470 7574 5f65 6e63 6f64 696e 675f  output_encoding_
-00003040: 6572 726f 725f 6861 6e64 6c65 7294 6ada  error_handler.j.
-00003050: 0300 008c 0e65 7272 6f72 5f65 6e63 6f64  .....error_encod
-00003060: 696e 6794 8c05 7574 662d 3894 8c1c 6572  ing...utf-8...er
-00003070: 726f 725f 656e 636f 6469 6e67 5f65 7272  ror_encoding_err
-00003080: 6f72 5f68 616e 646c 6572 948c 1062 6163  or_handler...bac
-00003090: 6b73 6c61 7368 7265 706c 6163 6594 8c0d  kslashreplace...
-000030a0: 6c61 6e67 7561 6765 5f63 6f64 6594 8c02  language_code...
-000030b0: 656e 948c 1372 6563 6f72 645f 6465 7065  en...record_depe
-000030c0: 6e64 656e 6369 6573 944e 8c06 636f 6e66  ndencies.N..conf
-000030d0: 6967 944e 8c09 6964 5f70 7265 6669 7894  ig.N..id_prefix.
-000030e0: 6806 8c0e 6175 746f 5f69 645f 7072 6566  h...auto_id_pref
-000030f0: 6978 948c 0269 6494 8c0d 6475 6d70 5f73  ix...id...dump_s
-00003100: 6574 7469 6e67 7394 4e8c 0e64 756d 705f  ettings.N..dump_
-00003110: 696e 7465 726e 616c 7394 4e8c 0f64 756d  internals.N..dum
-00003120: 705f 7472 616e 7366 6f72 6d73 944e 8c0f  p_transforms.N..
-00003130: 6475 6d70 5f70 7365 7564 6f5f 786d 6c94  dump_pseudo_xml.
-00003140: 4e8c 1065 7870 6f73 655f 696e 7465 726e  N..expose_intern
-00003150: 616c 7394 4e8c 0e73 7472 6963 745f 7669  als.N..strict_vi
-00003160: 7369 746f 7294 4e8c 0f5f 6469 7361 626c  sitor.N.._disabl
-00003170: 655f 636f 6e66 6967 944e 8c07 5f73 6f75  e_config.N.._sou
-00003180: 7263 6594 6828 8c0c 5f64 6573 7469 6e61  rce.h(.._destina
-00003190: 7469 6f6e 944e 8c0d 5f63 6f6e 6669 675f  tion.N.._config_
-000031a0: 6669 6c65 7394 5d94 8c16 6669 6c65 5f69  files.]...file_i
-000031b0: 6e73 6572 7469 6f6e 5f65 6e61 626c 6564  nsertion_enabled
-000031c0: 9488 8c0b 7261 775f 656e 6162 6c65 6494  ....raw_enabled.
-000031d0: 4b01 8c11 6c69 6e65 5f6c 656e 6774 685f  K...line_length_
-000031e0: 6c69 6d69 7494 4d10 278c 0e70 6570 5f72  limit.M.'..pep_r
-000031f0: 6566 6572 656e 6365 7394 4e8c 0c70 6570  eferences.N..pep
-00003200: 5f62 6173 655f 7572 6c94 8c18 6874 7470  _base_url...http
-00003210: 733a 2f2f 7065 7073 2e70 7974 686f 6e2e  s://peps.python.
-00003220: 6f72 672f 948c 1570 6570 5f66 696c 655f  org/...pep_file_
-00003230: 7572 6c5f 7465 6d70 6c61 7465 948c 0870  url_template...p
-00003240: 6570 2d25 3034 6494 8c0e 7266 635f 7265  ep-%04d...rfc_re
-00003250: 6665 7265 6e63 6573 944e 8c0c 7266 635f  ferences.N..rfc_
-00003260: 6261 7365 5f75 726c 948c 2668 7474 7073  base_url..&https
-00003270: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
-00003280: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
-00003290: 2f94 8c09 7461 625f 7769 6474 6894 4b08  /...tab_width.K.
-000032a0: 8c1d 7472 696d 5f66 6f6f 746e 6f74 655f  ..trim_footnote_
-000032b0: 7265 6665 7265 6e63 655f 7370 6163 6594  reference_space.
-000032c0: 898c 1073 796e 7461 785f 6869 6768 6c69  ...syntax_highli
-000032d0: 6768 7494 8c04 6c6f 6e67 948c 0c73 6d61  ght...long...sma
-000032e0: 7274 5f71 756f 7465 7394 888c 1373 6d61  rt_quotes....sma
-000032f0: 7274 7175 6f74 6573 5f6c 6f63 616c 6573  rtquotes_locales
-00003300: 945d 948c 1d63 6861 7261 6374 6572 5f6c  .]...character_l
-00003310: 6576 656c 5f69 6e6c 696e 655f 6d61 726b  evel_inline_mark
-00003320: 7570 9489 8c0e 646f 6374 6974 6c65 5f78  up....doctitle_x
-00003330: 666f 726d 9489 8c0d 646f 6369 6e66 6f5f  form....docinfo_
-00003340: 7866 6f72 6d94 4b01 8c12 7365 6374 7375  xform.K...sectsu
-00003350: 6274 6974 6c65 5f78 666f 726d 9489 8c0d  btitle_xform....
-00003360: 696d 6167 655f 6c6f 6164 696e 6794 8c04  image_loading...
-00003370: 6c69 6e6b 948c 1065 6d62 6564 5f73 7479  link...embed_sty
-00003380: 6c65 7368 6565 7494 898c 1563 6c6f 616b  lesheet....cloak
-00003390: 5f65 6d61 696c 5f61 6464 7265 7373 6573  _email_addresses
-000033a0: 9488 8c11 7365 6374 696f 6e5f 7365 6c66  ....section_self
-000033b0: 5f6c 696e 6b94 898c 0365 6e76 944e 7562  _link....env.Nub
-000033c0: 8c08 7265 706f 7274 6572 944e 8c10 696e  ..reporter.N..in
-000033d0: 6469 7265 6374 5f74 6172 6765 7473 945d  direct_targets.]
-000033e0: 948c 1173 7562 7374 6974 7574 696f 6e5f  ...substitution_
-000033f0: 6465 6673 947d 9428 8c14 446f 6375 6d65  defs.}.(..Docume
-00003400: 6e74 6174 696f 6e20 5374 6174 7573 946a  ntation Status.j
-00003410: e102 0000 68d9 6afe 0200 0068 f76a 1b03  ....h.j....h.j..
-00003420: 0000 758c 1273 7562 7374 6974 7574 696f  ..u..substitutio
-00003430: 6e5f 6e61 6d65 7394 7d94 288c 1464 6f63  n_names.}.(..doc
-00003440: 756d 656e 7461 7469 6f6e 2073 7461 7475  umentation statu
-00003450: 7394 6a15 0400 008c 0470 7970 6994 68d9  s.j......pypi.h.
-00003460: 8c09 646f 776e 6c6f 6164 7394 68f7 758c  ..downloads.h.u.
-00003470: 0872 6566 6e61 6d65 7394 7d94 8c06 7265  .refnames.}...re
-00003480: 6669 6473 947d 948c 076e 616d 6569 6473  fids.}...nameids
-00003490: 947d 9428 6ab0 0300 006a ad03 0000 6a68  .}.(j....j....jh
-000034a0: 0100 006a 6501 0000 6a13 0200 006a 1002  ...je...j....j..
-000034b0: 0000 6ac0 0100 006a bd01 0000 6a0b 0200  ..j....j....j...
-000034c0: 006a 0802 0000 6aa8 0300 006a a503 0000  .j....j....j....
-000034d0: 6a74 0200 006a 7102 0000 6aad 0200 006a  jt...jq...j....j
-000034e0: aa02 0000 6aa0 0300 006a 9d03 0000 758c  ....j....j....u.
-000034f0: 096e 616d 6574 7970 6573 947d 9428 6ab0  .nametypes.}.(j.
-00003500: 0300 0089 6a68 0100 0089 6a13 0200 0089  ....jh....j.....
-00003510: 6ac0 0100 0089 6a0b 0200 0089 6aa8 0300  j.....j.....j...
-00003520: 0089 6a74 0200 0089 6aad 0200 0089 6aa0  ..jt....j.....j.
-00003530: 0300 0089 7568 197d 9428 6aad 0300 0068  ....uh.}.(j....h
-00003540: 2c6a 6501 0000 6a09 0100 006a 1002 0000  ,je...j....j....
-00003550: 6a6b 0100 006a bd01 0000 6a8a 0100 006a  jk...j....j....j
-00003560: 0802 0000 6ac3 0100 006a a503 0000 6a16  ....j....j....j.
-00003570: 0200 006a 7102 0000 6a27 0200 006a aa02  ...jq...j'...j..
-00003580: 0000 6a77 0200 006a 9d03 0000 6ab0 0200  ..jw...j....j...
-00003590: 0075 8c0d 666f 6f74 6e6f 7465 5f72 6566  .u..footnote_ref
-000035a0: 7394 7d94 8c0d 6369 7461 7469 6f6e 5f72  s.}...citation_r
-000035b0: 6566 7394 7d94 8c0d 6175 746f 666f 6f74  efs.}...autofoot
-000035c0: 6e6f 7465 7394 5d94 8c11 6175 746f 666f  notes.]...autofo
-000035d0: 6f74 6e6f 7465 5f72 6566 7394 5d94 8c10  otnote_refs.]...
-000035e0: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 6573  symbol_footnotes
-000035f0: 945d 948c 1473 796d 626f 6c5f 666f 6f74  .]...symbol_foot
-00003600: 6e6f 7465 5f72 6566 7394 5d94 8c09 666f  note_refs.]...fo
-00003610: 6f74 6e6f 7465 7394 5d94 8c09 6369 7461  otnotes.]...cita
-00003620: 7469 6f6e 7394 5d94 8c12 6175 746f 666f  tions.]...autofo
-00003630: 6f74 6e6f 7465 5f73 7461 7274 944b 018c  otnote_start.K..
-00003640: 1573 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
-00003650: 5f73 7461 7274 944b 008c 0a69 645f 636f  _start.K...id_co
-00003660: 756e 7465 7294 8c0b 636f 6c6c 6563 7469  unter...collecti
-00003670: 6f6e 7394 8c07 436f 756e 7465 7294 9394  ons...Counter...
-00003680: 7d94 8594 5294 8c0e 7061 7273 655f 6d65  }...R...parse_me
-00003690: 7373 6167 6573 945d 948c 1274 7261 6e73  ssages.]...trans
-000036a0: 666f 726d 5f6d 6573 7361 6765 7394 5d94  form_messages.].
-000036b0: 8c0b 7472 616e 7366 6f72 6d65 7294 4e8c  ..transformer.N.
-000036c0: 0b69 6e63 6c75 6465 5f6c 6f67 945d 948c  .include_log.]..
-000036d0: 0a64 6563 6f72 6174 696f 6e94 4e68 2668  .decoration.Nh&h
-000036e0: 0375 622e                                .ub.
+000002c0: 8c55 433a 5c55 7365 7273 5c6d 6178 696d  .UC:\Users\maxim
+000002d0: 5c4f 6e65 4472 6976 655c 446f 6375 6d65  \OneDrive\Docume
+000002e0: 6e74 735c 5079 7468 6f6e 5c50 6163 6b61  nts\Python\Packa
+000002f0: 6765 735c 6d7a 4461 7461 584d 4c32 4d61  ges\mzDataXML2Ma
+00000300: 745c 646f 6373 5c73 6f75 7263 655c 696e  t\docs\source\in
+00000310: 6465 782e 7273 7494 8c04 6c69 6e65 944b  dex.rst...line.K
+00000320: 0575 6268 098c 0773 6563 7469 6f6e 9493  .ubh...section..
+00000330: 9429 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+00000340: 6809 8c05 7469 746c 6594 9394 2981 947d  h...title...)..}
+00000350: 9428 6805 8c07 5765 6c63 6f6d 6594 6807  .(h...Welcome.h.
+00000360: 5d94 6811 8c07 5765 6c63 6f6d 6594 8594  ].h...Welcome...
+00000370: 8194 7d94 2868 1668 3168 2668 0368 274e  ..}.(h.h1h&h.h'N
+00000380: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
+00000390: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
+000003a0: 6825 682f 6816 682c 6826 6803 6827 6828  h%h/h.h,h&h.h'h(
+000003b0: 6829 4b07 7562 6809 8c09 7061 7261 6772  h)K.ubh...paragr
+000003c0: 6170 6894 9394 2981 947d 9428 6805 8cd7  aph...)..}.(h...
+000003d0: 5765 6c63 6f6d 6520 2120 6060 6d7a 6461  Welcome ! ``mzda
+000003e0: 7461 326d 6174 6060 2069 7320 6120 5079  ta2mat`` is a Py
+000003f0: 7468 6f6e 2070 6163 6b61 6765 2066 726f  thon package fro
+00000400: 6d20 604c 4152 5449 4320 7265 7365 6172  m `LARTIC resear
+00000410: 6368 2074 6561 6d20 3c68 7474 7073 3a2f  ch team <https:/
+00000420: 2f6c 6172 7469 632e 6673 6161 2e75 6c61  /lartic.fsaa.ula
+00000430: 7661 6c2e 6361 2f3e 605f 5f2c 2077 6869  val.ca/>`__, whi
+00000440: 6368 2063 6f6e 7665 7274 7320 6d7a 4461  ch converts mzDa
+00000450: 7461 2e78 6d6c 2066 696c 6573 2028 7665  ta.xml files (ve
+00000460: 7273 696f 6e20 312e 3035 2c20 4167 696c  rsion 1.05, Agil
+00000470: 656e 7420 5465 6368 6e6f 6c6f 6769 6573  ent Technologies
+00000480: 2920 696e 746f 206d 6174 2066 696c 6573  ) into mat files
+00000490: 2072 6561 6461 626c 6520 7573 696e 6720   readable using 
+000004a0: 6d61 746c 6162 2e94 6807 5d94 2868 118c  matlab..h.].(h..
+000004b0: 0a57 656c 636f 6d65 2021 2094 8594 8194  .Welcome ! .....
+000004c0: 7d94 2868 1668 4168 2668 0368 274e 6829  }.(h.hAh&h.h'Nh)
+000004d0: 4e75 6268 098c 076c 6974 6572 616c 9493  Nubh...literal..
+000004e0: 9429 8194 7d94 2868 058c 0e60 606d 7a64  .)..}.(h...``mzd
+000004f0: 6174 6132 6d61 7460 6094 6807 5d94 6811  ata2mat``.h.].h.
+00000500: 8c0a 6d7a 6461 7461 326d 6174 9485 9481  ..mzdata2mat....
+00000510: 947d 9428 6816 684b 6826 6803 6827 4e68  .}.(h.hKh&h.h'Nh
+00000520: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+00000530: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+00000540: 2568 4968 1668 4175 6268 118c 1a20 6973  %hIh.hAubh... is
+00000550: 2061 2050 7974 686f 6e20 7061 636b 6167   a Python packag
+00000560: 6520 6672 6f6d 2094 8594 8194 7d94 2868  e from .....}.(h
+00000570: 1668 4168 2668 0368 274e 6829 4e75 6268  .hAh&h.h'Nh)Nubh
+00000580: 098c 0972 6566 6572 656e 6365 9493 9429  ...reference...)
+00000590: 8194 7d94 2868 058c 3960 4c41 5254 4943  ..}.(h..9`LARTIC
+000005a0: 2072 6573 6561 7263 6820 7465 616d 203c   research team <
+000005b0: 6874 7470 733a 2f2f 6c61 7274 6963 2e66  https://lartic.f
+000005c0: 7361 612e 756c 6176 616c 2e63 612f 3e60  saa.ulaval.ca/>`
+000005d0: 5f5f 9468 075d 9468 118c 144c 4152 5449  __.h.].h...LARTI
+000005e0: 4320 7265 7365 6172 6368 2074 6561 6d94  C research team.
+000005f0: 8594 8194 7d94 2868 1668 5f68 2668 0368  ....}.(h.h_h&h.h
+00000600: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
+00000610: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00000620: 948c 046e 616d 6594 8c14 4c41 5254 4943  ...name...LARTIC
+00000630: 2072 6573 6561 7263 6820 7465 616d 948c   research team..
+00000640: 0672 6566 7572 6994 8c1e 6874 7470 733a  .refuri...https:
+00000650: 2f2f 6c61 7274 6963 2e66 7361 612e 756c  //lartic.fsaa.ul
+00000660: 6176 616c 2e63 612f 9475 6825 685d 6816  aval.ca/.uh%h]h.
+00000670: 6841 7562 6811 8c6c 2c20 7768 6963 6820  hAubh..l, which 
+00000680: 636f 6e76 6572 7473 206d 7a44 6174 612e  converts mzData.
+00000690: 786d 6c20 6669 6c65 7320 2876 6572 7369  xml files (versi
+000006a0: 6f6e 2031 2e30 352c 2041 6769 6c65 6e74  on 1.05, Agilent
+000006b0: 2054 6563 686e 6f6c 6f67 6965 7329 2069   Technologies) i
+000006c0: 6e74 6f20 6d61 7420 6669 6c65 7320 7265  nto mat files re
+000006d0: 6164 6162 6c65 2075 7369 6e67 206d 6174  adable using mat
+000006e0: 6c61 622e 9485 9481 947d 9428 6816 6841  lab......}.(h.hA
+000006f0: 6826 6803 6827 4e68 294e 7562 6568 177d  h&h.h'Nh)Nubeh.}
+00000700: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+00000710: 5d94 6821 5d94 7568 2568 3f68 2768 2868  ].h!].uh%h?h'h(h
+00000720: 294b 0968 1668 2c68 2668 0375 6268 4029  )K.h.h,h&h.ubh@)
+00000730: 8194 7d94 2868 058c 1d41 7574 686f 7220  ..}.(h...Author 
+00000740: 3a20 4d61 7869 6d65 2052 2e41 2e20 436f  : Maxime R.A. Co
+00000750: 7264 656c 6c61 9468 075d 9468 118c 1d41  rdella.h.].h...A
+00000760: 7574 686f 7220 3a20 4d61 7869 6d65 2052  uthor : Maxime R
+00000770: 2e41 2e20 436f 7264 656c 6c61 9485 9481  .A. Cordella....
+00000780: 947d 9428 6816 687b 6826 6803 6827 4e68  .}.(h.h{h&h.h'Nh
+00000790: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+000007a0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+000007b0: 2568 3f68 2768 2868 294b 0c68 1668 2c68  %h?h'h(h)K.h.h,h
+000007c0: 2668 0375 6268 4029 8194 7d94 2868 058c  &h.ubh@)..}.(h..
+000007d0: 2a54 6561 6d20 6c65 6164 6572 203a 2050  *Team leader : P
+000007e0: 722e 2043 6872 6973 746f 7068 6520 422e  r. Christophe B.
+000007f0: 592e 2043 6f72 6465 6c6c 6194 6807 5d94  Y. Cordella.h.].
+00000800: 6811 8c2a 5465 616d 206c 6561 6465 7220  h..*Team leader 
+00000810: 3a20 5072 2e20 4368 7269 7374 6f70 6865  : Pr. Christophe
+00000820: 2042 2e59 2e20 436f 7264 656c 6c61 9485   B.Y. Cordella..
+00000830: 9481 947d 9428 6816 6889 6826 6803 6827  ...}.(h.h.h&h.h'
+00000840: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
+00000850: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+00000860: 7568 2568 3f68 2768 2868 294b 0e68 1668  uh%h?h'h(h)K.h.h
+00000870: 2c68 2668 0375 6268 4029 8194 7d94 2868  ,h&h.ubh@)..}.(h
+00000880: 058c 1843 6f70 7972 6967 6874 2863 2920  ...Copyright(c) 
+00000890: 3230 3234 5f4c 4152 5449 4394 6807 5d94  2024_LARTIC.h.].
+000008a0: 6811 8c18 436f 7079 7269 6768 7428 6329  h...Copyright(c)
+000008b0: 2032 3032 345f 4c41 5254 4943 9485 9481   2024_LARTIC....
+000008c0: 947d 9428 6816 6897 6826 6803 6827 4e68  .}.(h.h.h&h.h'Nh
+000008d0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+000008e0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+000008f0: 2568 3f68 2768 2868 294b 1068 1668 2c68  %h?h'h(h)K.h.h,h
+00000900: 2668 0375 6268 4029 8194 7d94 2868 058c  &h.ubh@)..}.(h..
+00000910: 297c 446f 6375 6d65 6e74 6174 696f 6e20  )|Documentation 
+00000920: 5374 6174 7573 7c20 7c50 7950 497c 207c  Status| |PyPI| |
+00000930: 646f 776e 6c6f 6164 737c 9468 075d 9428  downloads|.h.].(
+00000940: 685e 2981 947d 9428 6807 5d94 6809 8c05  h^)..}.(h.].h...
+00000950: 696d 6167 6594 9394 2981 947d 9428 6807  image...)..}.(h.
+00000960: 5d94 6805 8c8f 696d 6167 653a 3a20 6874  ].h...image:: ht
+00000970: 7470 733a 2f2f 7265 6164 7468 6564 6f63  tps://readthedoc
+00000980: 732e 6f72 672f 7072 6f6a 6563 7473 2f6d  s.org/projects/m
+00000990: 7a64 6174 6132 6d61 742f 6261 6467 652f  zdata2mat/badge/
+000009a0: 3f76 6572 7369 6f6e 3d6c 6174 6573 740a  ?version=latest.
+000009b0: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
+000009c0: 733a 2f2f 6d7a 6461 7461 326d 6174 2e72  s://mzdata2mat.r
+000009d0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+000009e0: 2f6c 6174 6573 742f 3f62 6164 6765 3d6c  /latest/?badge=l
+000009f0: 6174 6573 7494 6825 68ac 6817 7d94 2868  atest.h%h.h.}.(h
+00000a00: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+00000a10: 215d 948c 0361 6c74 948c 1444 6f63 756d  !]...alt...Docum
+00000a20: 656e 7461 7469 6f6e 2053 7461 7475 7394  entation Status.
+00000a30: 8c03 7572 6994 8c41 6874 7470 733a 2f2f  ..uri..Ahttps://
+00000a40: 7265 6164 7468 6564 6f63 732e 6f72 672f  readthedocs.org/
+00000a50: 7072 6f6a 6563 7473 2f6d 7a64 6174 6132  projects/mzdata2
+00000a60: 6d61 742f 6261 6467 652f 3f76 6572 7369  mat/badge/?versi
+00000a70: 6f6e 3d6c 6174 6573 7494 8c0a 6361 6e64  on=latest...cand
+00000a80: 6964 6174 6573 947d 948c 013f 9468 bb73  idates.}...?.h.s
+00000a90: 7568 294b 0068 2768 2868 1668 a968 2668  uh)K.h'h(h.h.h&h
+00000aa0: 0375 6261 6805 68b9 6825 685d 6817 7d94  .ubah.h.h%h]h.}.
+00000ab0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00000ac0: 9468 215d 948c 0672 6566 7572 6994 8c39  .h!]...refuri..9
+00000ad0: 6874 7470 733a 2f2f 6d7a 6461 7461 326d  https://mzdata2m
+00000ae0: 6174 2e72 6561 6474 6865 646f 6373 2e69  at.readthedocs.i
+00000af0: 6f2f 656e 2f6c 6174 6573 742f 3f62 6164  o/en/latest/?bad
+00000b00: 6765 3d6c 6174 6573 7494 7568 294e 6827  ge=latest.uh)Nh'
+00000b10: 4e68 1668 a568 2668 0375 6268 118c 0120  Nh.h.h&h.ubh... 
+00000b20: 9485 9481 947d 9428 6816 68a5 6826 6803  .....}.(h.h.h&h.
+00000b30: 6827 4e68 294e 7562 685e 2981 947d 9428  h'Nh)Nubh^)..}.(
+00000b40: 6807 5d94 68ad 2981 947d 9428 6807 5d94  h.].h.)..}.(h.].
+00000b50: 6805 8c61 696d 6167 653a 3a20 6874 7470  h..aimage:: http
+00000b60: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000b70: 696f 2f70 7970 692f 762f 6d7a 6461 7461  io/pypi/v/mzdata
+00000b80: 326d 6174 0a20 2020 3a74 6172 6765 743a  2mat.   :target:
+00000b90: 2068 7474 7073 3a2f 2f70 7970 692e 6f72   https://pypi.or
+00000ba0: 672f 7072 6f6a 6563 742f 6d7a 6461 7461  g/project/mzdata
+00000bb0: 326d 6174 2f94 6825 68ac 6817 7d94 2868  2mat/.h%h.h.}.(h
+00000bc0: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+00000bd0: 215d 948c 0361 6c74 948c 0450 7950 4994  !]...alt...PyPI.
+00000be0: 8c03 7572 6994 8c28 6874 7470 733a 2f2f  ..uri..(https://
+00000bf0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000c00: 7970 692f 762f 6d7a 6461 7461 326d 6174  ypi/v/mzdata2mat
+00000c10: 9468 bc7d 9468 be68 db73 7568 294b 0068  .h.}.h.h.suh)K.h
+00000c20: 2768 2868 1668 cb68 2668 0375 6261 6805  'h(h.h.h&h.ubah.
+00000c30: 68d9 6825 685d 6817 7d94 2868 195d 9468  h.h%h]h.}.(h.].h
+00000c40: 1b5d 9468 1d5d 9468 1f5d 9468 215d 948c  .].h.].h.].h!]..
+00000c50: 0672 6566 7572 6994 8c24 6874 7470 733a  .refuri..$https:
+00000c60: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000c70: 6374 2f6d 7a64 6174 6132 6d61 742f 9475  ct/mzdata2mat/.u
+00000c80: 6829 4e68 274e 6816 68a5 6826 6803 7562  h)Nh'Nh.h.h&h.ub
+00000c90: 6811 8c01 2094 8594 8194 7d94 6816 68a5  h... .....}.h.h.
+00000ca0: 7362 685e 2981 947d 9428 6807 5d94 68ad  sbh^)..}.(h.].h.
+00000cb0: 2981 947d 9428 6807 5d94 6805 8c68 696d  )..}.(h.].h..him
+00000cc0: 6167 653a 3a20 6874 7470 733a 2f2f 7374  age:: https://st
+00000cd0: 6174 6963 2e70 6570 792e 7465 6368 2f62  atic.pepy.tech/b
+00000ce0: 6164 6765 2f6d 7a64 6174 6132 6d61 742f  adge/mzdata2mat/
+00000cf0: 6d6f 6e74 680a 2020 203a 7461 7267 6574  month.   :target
+00000d00: 3a20 6874 7470 733a 2f2f 7065 7079 2e74  : https://pepy.t
+00000d10: 6563 682f 7072 6f6a 6563 742f 6d7a 6461  ech/project/mzda
+00000d20: 7461 326d 6174 9468 2568 ac68 177d 9428  ta2mat.h%h.h.}.(
+00000d30: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00000d40: 6821 5d94 8c03 616c 7494 8c09 646f 776e  h!]...alt...down
+00000d50: 6c6f 6164 7394 8c03 7572 6994 8c2f 6874  loads...uri../ht
+00000d60: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
+00000d70: 792e 7465 6368 2f62 6164 6765 2f6d 7a64  y.tech/badge/mzd
+00000d80: 6174 6132 6d61 742f 6d6f 6e74 6894 68bc  ata2mat/month.h.
+00000d90: 7d94 68be 68f9 7375 6829 4b00 6827 6828  }.h.h.suh)K.h'h(
+00000da0: 6816 68e9 6826 6803 7562 6168 0568 f768  h.h.h&h.ubah.h.h
+00000db0: 2568 5d68 177d 9428 6819 5d94 681b 5d94  %h]h.}.(h.].h.].
+00000dc0: 681d 5d94 681f 5d94 6821 5d94 8c06 7265  h.].h.].h!]...re
+00000dd0: 6675 7269 948c 2468 7474 7073 3a2f 2f70  furi..$https://p
+00000de0: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+00000df0: 2f6d 7a64 6174 6132 6d61 7494 7568 294e  /mzdata2mat.uh)N
+00000e00: 6827 4e68 1668 a568 2668 0375 6265 6817  h'Nh.h.h&h.ubeh.
+00000e10: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00000e20: 1f5d 9468 215d 9475 6825 683f 6827 6828  .].h!].uh%h?h'h(
+00000e30: 6829 4b12 6816 682c 6826 6803 7562 682b  h)K.h.h,h&h.ubh+
+00000e40: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+00000e50: 3029 8194 7d94 2868 058c 1943 7572 7265  0)..}.(h...Curre
+00000e60: 6e74 2076 6572 7369 6f6e 2060 6030 2e32  nt version ``0.2
+00000e70: 2e30 6060 9468 075d 9428 6811 8c10 4375  .0``.h.].(h...Cu
+00000e80: 7272 656e 7420 7665 7273 696f 6e20 9485  rrent version ..
+00000e90: 9481 947d 9428 6816 6a0c 0100 0068 2668  ...}.(h.j....h&h
+00000ea0: 0368 274e 6829 4e75 6268 4a29 8194 7d94  .h'Nh)NubhJ)..}.
+00000eb0: 2868 058c 0960 6030 2e32 2e30 6060 9468  (h...``0.2.0``.h
+00000ec0: 075d 9468 118c 0530 2e32 2e30 9485 9481  .].h...0.2.0....
+00000ed0: 947d 9428 6816 6a14 0100 0068 2668 0368  .}.(h.j....h&h.h
+00000ee0: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
+00000ef0: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00000f00: 9475 6825 6849 6816 6a0c 0100 0075 6265  .uh%hIh.j....ube
+00000f10: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00000f20: 9468 1f5d 9468 215d 9475 6825 682f 6816  .h.].h!].uh%h/h.
+00000f30: 6a09 0100 0068 2668 0368 2768 2868 294b  j....h&h.h'h(h)K
+00000f40: 1575 6268 4029 8194 7d94 2868 058c 3e54  .ubh@)..}.(h..>T
+00000f50: 6865 2063 7572 7265 6e74 2076 6572 7369  he current versi
+00000f60: 6f6e 206f 6620 6d7a 6461 7461 326d 6174  on of mzdata2mat
+00000f70: 2069 7320 7468 6520 666f 6c6c 6f77 696e   is the followin
+00000f80: 6720 3a20 6060 302e 322e 3060 6094 6807  g : ``0.2.0``.h.
+00000f90: 5d94 2868 118c 3554 6865 2063 7572 7265  ].(h..5The curre
+00000fa0: 6e74 2076 6572 7369 6f6e 206f 6620 6d7a  nt version of mz
+00000fb0: 6461 7461 326d 6174 2069 7320 7468 6520  data2mat is the 
+00000fc0: 666f 6c6c 6f77 696e 6720 3a20 9485 9481  following : ....
+00000fd0: 947d 9428 6816 6a28 0100 0068 2668 0368  .}.(h.j(...h&h.h
+00000fe0: 274e 6829 4e75 6268 4a29 8194 7d94 2868  'Nh)NubhJ)..}.(h
+00000ff0: 058c 0960 6030 2e32 2e30 6060 9468 075d  ...``0.2.0``.h.]
+00001000: 9468 118c 0530 2e32 2e30 9485 9481 947d  .h...0.2.0.....}
+00001010: 9428 6816 6a30 0100 0068 2668 0368 274e  .(h.j0...h&h.h'N
+00001020: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
+00001030: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
+00001040: 6825 6849 6816 6a28 0100 0075 6265 6817  h%hIh.j(...ubeh.
+00001050: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00001060: 1f5d 9468 215d 9475 6825 683f 6827 6828  .].h!].uh%h?h'h(
+00001070: 6829 4b17 6816 6a09 0100 0068 2668 0375  h)K.h.j....h&h.u
+00001080: 6268 4029 8194 7d94 2868 058c 3c59 6f75  bh@)..}.(h..<You
+00001090: 2063 616e 2073 6565 2074 6865 2063 6f6d   can see the com
+000010a0: 706c 6574 6520 6368 616e 6765 6c6f 6720  plete changelog 
+000010b0: 6068 6572 6520 3c43 6861 6e67 656c 6f67  `here <Changelog
+000010c0: 2e68 746d 6c3e 605f 5f94 6807 5d94 2868  .html>`__.h.].(h
+000010d0: 118c 2359 6f75 2063 616e 2073 6565 2074  ..#You can see t
+000010e0: 6865 2063 6f6d 706c 6574 6520 6368 616e  he complete chan
+000010f0: 6765 6c6f 6720 9485 9481 947d 9428 6816  gelog .....}.(h.
+00001100: 6a44 0100 0068 2668 0368 274e 6829 4e75  jD...h&h.h'Nh)Nu
+00001110: 6268 5e29 8194 7d94 2868 058c 1960 6865  bh^)..}.(h...`he
+00001120: 7265 203c 4368 616e 6765 6c6f 672e 6874  re <Changelog.ht
+00001130: 6d6c 3e60 5f5f 9468 075d 9468 118c 0468  ml>`__.h.].h...h
+00001140: 6572 6594 8594 8194 7d94 2868 166a 4c01  ere.....}.(h.jL.
+00001150: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+00001160: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00001170: 681f 5d94 6821 5d94 8c04 6e61 6d65 948c  h.].h!]...name..
+00001180: 0468 6572 6594 686f 8c0e 4368 616e 6765  .here.ho..Change
+00001190: 6c6f 672e 6874 6d6c 9475 6825 685d 6816  log.html.uh%h]h.
+000011a0: 6a44 0100 0075 6265 6817 7d94 2868 195d  jD...ubeh.}.(h.]
+000011b0: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+000011c0: 9475 6825 683f 6827 6828 6829 4b19 6816  .uh%h?h'h(h)K.h.
+000011d0: 6a09 0100 0068 2668 0375 6265 6817 7d94  j....h&h.ubeh.}.
+000011e0: 2868 195d 948c 1563 7572 7265 6e74 2d76  (h.]...current-v
+000011f0: 6572 7369 6f6e 2d30 2d32 2d30 9461 681b  ersion-0-2-0.ah.
+00001200: 5d94 681d 5d94 8c15 6375 7272 656e 7420  ].h.]...current 
+00001210: 7665 7273 696f 6e20 302e 322e 3094 6168  version 0.2.0.ah
+00001220: 1f5d 9468 215d 9475 6825 682a 6816 682c  .].h!].uh%h*h.h,
+00001230: 6826 6803 6827 6828 6829 4b15 7562 682b  h&h.h'h(h)K.ubh+
+00001240: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+00001250: 3029 8194 7d94 2868 058c 1343 6f6d 7061  0)..}.(h...Compa
+00001260: 7469 626c 6520 6861 7264 7761 7265 9468  tible hardware.h
+00001270: 075d 9468 118c 1343 6f6d 7061 7469 626c  .].h...Compatibl
+00001280: 6520 6861 7264 7761 7265 9485 9481 947d  e hardware.....}
+00001290: 9428 6816 6a6e 0100 0068 2668 0368 274e  .(h.jn...h&h.h'N
+000012a0: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
+000012b0: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
+000012c0: 6825 682f 6816 6a6b 0100 0068 2668 0368  h%h/h.jk...h&h.h
+000012d0: 2768 2868 294b 1c75 6268 4029 8194 7d94  'h(h)K.ubh@)..}.
+000012e0: 2868 058c 3341 7420 7468 6973 2074 696d  (h..3At this tim
+000012f0: 652c 2074 6865 2066 6f6c 6c6f 7769 6e67  e, the following
+00001300: 204f 5365 7320 6861 7665 2062 6565 6e20   OSes have been 
+00001310: 7465 7374 6564 203a 9468 075d 9468 118c  tested :.h.].h..
+00001320: 3341 7420 7468 6973 2074 696d 652c 2074  3At this time, t
+00001330: 6865 2066 6f6c 6c6f 7769 6e67 204f 5365  he following OSe
+00001340: 7320 6861 7665 2062 6565 6e20 7465 7374  s have been test
+00001350: 6564 203a 9485 9481 947d 9428 6816 6a7c  ed :.....}.(h.j|
+00001360: 0100 0068 2668 0368 274e 6829 4e75 6261  ...h&h.h'Nh)Nuba
+00001370: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00001380: 9468 1f5d 9468 215d 9475 6825 683f 6827  .h.].h!].uh%h?h'
+00001390: 6828 6829 4b1e 6816 6a6b 0100 0068 2668  h(h)K.h.jk...h&h
+000013a0: 0375 6268 2b29 8194 7d94 2868 0568 0668  .ubh+)..}.(h.h.h
+000013b0: 075d 9428 6830 2981 947d 9428 6805 8c05  .].(h0)..}.(h...
+000013c0: 6d61 634f 5394 6807 5d94 6811 8c05 6d61  macOS.h.].h...ma
+000013d0: 634f 5394 8594 8194 7d94 2868 166a 8d01  cOS.....}.(h.j..
+000013e0: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+000013f0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00001400: 681f 5d94 6821 5d94 7568 2568 2f68 166a  h.].h!].uh%h/h.j
+00001410: 8a01 0000 6826 6803 6827 6828 6829 4b21  ....h&h.h'h(h)K!
+00001420: 7562 6840 2981 947d 9428 6805 8c9a 4174  ubh@)..}.(h...At
+00001430: 2074 6869 7320 7469 6d65 2c20 6060 6d61   this time, ``ma
+00001440: 634f 5320 536f 6e6f 6d61 2031 342e 3060  cOS Sonoma 14.0`
+00001450: 6020 6973 206f 6666 6963 6961 6c6c 7920  ` is officially 
+00001460: 7375 7070 6f72 7465 642c 206f 7468 6572  supported, other
+00001470: 206d 6163 4f53 0a76 6572 7369 6f6e 7320   macOS.versions 
+00001480: 636f 756c 6420 6265 2073 7570 706f 7274  could be support
+00001490: 6564 2061 7320 6c6f 6e67 2061 7320 7468  ed as long as th
+000014a0: 6579 2066 6f6c 6c6f 7720 7468 6520 7265  ey follow the re
+000014b0: 7175 6972 656d 656e 7473 0a6c 6973 7465  quirements.liste
+000014c0: 6420 6265 6c6f 772e 9468 075d 9428 6811  d below..h.].(h.
+000014d0: 8c0e 4174 2074 6869 7320 7469 6d65 2c20  ..At this time, 
+000014e0: 9485 9481 947d 9428 6816 6a9b 0100 0068  .....}.(h.j....h
+000014f0: 2668 0368 274e 6829 4e75 6268 4a29 8194  &h.h'Nh)NubhJ)..
+00001500: 7d94 2868 058c 1560 606d 6163 4f53 2053  }.(h...``macOS S
+00001510: 6f6e 6f6d 6120 3134 2e30 6060 9468 075d  onoma 14.0``.h.]
+00001520: 9468 118c 116d 6163 4f53 2053 6f6e 6f6d  .h...macOS Sonom
+00001530: 6120 3134 2e30 9485 9481 947d 9428 6816  a 14.0.....}.(h.
+00001540: 6aa3 0100 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00001550: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00001560: 1d5d 9468 1f5d 9468 215d 9475 6825 6849  .].h.].h!].uh%hI
+00001570: 6816 6a9b 0100 0075 6268 118c 7720 6973  h.j....ubh..w is
+00001580: 206f 6666 6963 6961 6c6c 7920 7375 7070   officially supp
+00001590: 6f72 7465 642c 206f 7468 6572 206d 6163  orted, other mac
+000015a0: 4f53 0a76 6572 7369 6f6e 7320 636f 756c  OS.versions coul
+000015b0: 6420 6265 2073 7570 706f 7274 6564 2061  d be supported a
+000015c0: 7320 6c6f 6e67 2061 7320 7468 6579 2066  s long as they f
+000015d0: 6f6c 6c6f 7720 7468 6520 7265 7175 6972  ollow the requir
+000015e0: 656d 656e 7473 0a6c 6973 7465 6420 6265  ements.listed be
+000015f0: 6c6f 772e 9485 9481 947d 9428 6816 6a9b  low......}.(h.j.
+00001600: 0100 0068 2668 0368 274e 6829 4e75 6265  ...h&h.h'Nh)Nube
+00001610: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00001620: 9468 1f5d 9468 215d 9475 6825 683f 6827  .h.].h!].uh%h?h'
+00001630: 6828 6829 4b23 6816 6a8a 0100 0068 2668  h(h)K#h.j....h&h
+00001640: 0375 6265 6817 7d94 2868 195d 948c 056d  .ubeh.}.(h.]...m
+00001650: 6163 6f73 9461 681b 5d94 681d 5d94 8c05  acos.ah.].h.]...
+00001660: 6d61 636f 7394 6168 1f5d 9468 215d 9475  macos.ah.].h!].u
+00001670: 6825 682a 6816 6a6b 0100 0068 2668 0368  h%h*h.jk...h&h.h
+00001680: 2768 2868 294b 2175 6268 2b29 8194 7d94  'h(h)K!ubh+)..}.
+00001690: 2868 0568 0668 075d 9428 6830 2981 947d  (h.h.h.].(h0)..}
+000016a0: 9428 6805 8c07 5769 6e64 6f77 7394 6807  .(h...Windows.h.
+000016b0: 5d94 6811 8c07 5769 6e64 6f77 7394 8594  ].h...Windows...
+000016c0: 8194 7d94 2868 166a c601 0000 6826 6803  ..}.(h.j....h&h.
+000016d0: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
+000016e0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+000016f0: 5d94 7568 2568 2f68 166a c301 0000 6826  ].uh%h/h.j....h&
+00001700: 6803 6827 6828 6829 4b28 7562 6840 2981  h.h'h(h)K(ubh@).
+00001710: 947d 9428 6805 8ce1 4174 2074 6869 7320  .}.(h...At this 
+00001720: 7469 6d65 2c20 6060 6d7a 6461 7461 326d  time, ``mzdata2m
+00001730: 6174 6060 2068 6176 6520 6265 656e 2074  at`` have been t
+00001740: 6573 7465 6420 616e 6420 6973 2073 7570  ested and is sup
+00001750: 706f 7274 6564 206f 6e0a 6060 5769 6e64  ported on.``Wind
+00001760: 6f77 7320 3131 6060 2c20 6e6f 2074 6573  ows 11``, no tes
+00001770: 7469 6e67 2068 6173 2062 6565 6e20 646f  ting has been do
+00001780: 6e65 206f 6e20 5769 6e64 6f77 7320 3130  ne on Windows 10
+00001790: 206f 7220 3720 6275 7420 6966 2079 6f75   or 7 but if you
+000017a0: 0a77 616e 7420 746f 2065 7874 656e 6420  .want to extend 
+000017b0: 7468 6520 636f 6d70 6174 6962 696c 6974  the compatibilit
+000017c0: 792c 2077 6520 6172 6520 6f70 656e 2074  y, we are open t
+000017d0: 6f20 7465 7374 6572 e280 9973 2066 6565  o tester...s fee
+000017e0: 6462 6163 6b20 6f6e 0a74 686f 7365 7320  dback on.thoses 
+000017f0: 6d61 6368 696e 6573 2e94 6807 5d94 2868  machines..h.].(h
+00001800: 118c 0e41 7420 7468 6973 2074 696d 652c  ...At this time,
+00001810: 2094 8594 8194 7d94 2868 166a d401 0000   .....}.(h.j....
+00001820: 6826 6803 6827 4e68 294e 7562 684a 2981  h&h.h'Nh)NubhJ).
+00001830: 947d 9428 6805 8c0e 6060 6d7a 6461 7461  .}.(h...``mzdata
+00001840: 326d 6174 6060 9468 075d 9468 118c 0a6d  2mat``.h.].h...m
+00001850: 7a64 6174 6132 6d61 7494 8594 8194 7d94  zdata2mat.....}.
+00001860: 2868 166a dc01 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
+00001870: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+00001880: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+00001890: 2568 4968 166a d401 0000 7562 6811 8c26  %hIh.j....ubh..&
+000018a0: 2068 6176 6520 6265 656e 2074 6573 7465   have been teste
+000018b0: 6420 616e 6420 6973 2073 7570 706f 7274  d and is support
+000018c0: 6564 206f 6e0a 9485 9481 947d 9428 6816  ed on......}.(h.
+000018d0: 6ad4 0100 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+000018e0: 6268 4a29 8194 7d94 2868 058c 0e60 6057  bhJ)..}.(h...``W
+000018f0: 696e 646f 7773 2031 3160 6094 6807 5d94  indows 11``.h.].
+00001900: 6811 8c0a 5769 6e64 6f77 7320 3131 9485  h...Windows 11..
+00001910: 9481 947d 9428 6816 6aee 0100 0068 2668  ...}.(h.j....h&h
+00001920: 0368 274e 6829 4e75 6261 6817 7d94 2868  .h'Nh)Nubah.}.(h
+00001930: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+00001940: 215d 9475 6825 6849 6816 6ad4 0100 0075  !].uh%hIh.j....u
+00001950: 6268 118c 912c 206e 6f20 7465 7374 696e  bh..., no testin
+00001960: 6720 6861 7320 6265 656e 2064 6f6e 6520  g has been done 
+00001970: 6f6e 2057 696e 646f 7773 2031 3020 6f72  on Windows 10 or
+00001980: 2037 2062 7574 2069 6620 796f 750a 7761   7 but if you.wa
+00001990: 6e74 2074 6f20 6578 7465 6e64 2074 6865  nt to extend the
+000019a0: 2063 6f6d 7061 7469 6269 6c69 7479 2c20   compatibility, 
+000019b0: 7765 2061 7265 206f 7065 6e20 746f 2074  we are open to t
+000019c0: 6573 7465 72e2 8099 7320 6665 6564 6261  ester...s feedba
+000019d0: 636b 206f 6e0a 7468 6f73 6573 206d 6163  ck on.thoses mac
+000019e0: 6869 6e65 732e 9485 9481 947d 9428 6816  hines......}.(h.
+000019f0: 6ad4 0100 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00001a00: 6265 6817 7d94 2868 195d 9468 1b5d 9468  beh.}.(h.].h.].h
+00001a10: 1d5d 9468 1f5d 9468 215d 9475 6825 683f  .].h.].h!].uh%h?
+00001a20: 6827 6828 6829 4b2a 6816 6ac3 0100 0068  h'h(h)K*h.j....h
+00001a30: 2668 0375 6265 6817 7d94 2868 195d 948c  &h.ubeh.}.(h.]..
+00001a40: 0777 696e 646f 7773 9461 681b 5d94 681d  .windows.ah.].h.
+00001a50: 5d94 8c07 7769 6e64 6f77 7394 6168 1f5d  ]...windows.ah.]
+00001a60: 9468 215d 9475 6825 682a 6816 6a6b 0100  .h!].uh%h*h.jk..
+00001a70: 0068 2668 0368 2768 2868 294b 2875 6265  .h&h.h'h(h)K(ube
+00001a80: 6817 7d94 2868 195d 948c 1363 6f6d 7061  h.}.(h.]...compa
+00001a90: 7469 626c 652d 6861 7264 7761 7265 9461  tible-hardware.a
+00001aa0: 681b 5d94 681d 5d94 8c13 636f 6d70 6174  h.].h.]...compat
+00001ab0: 6962 6c65 2068 6172 6477 6172 6594 6168  ible hardware.ah
+00001ac0: 1f5d 9468 215d 9475 6825 682a 6816 682c  .].h!].uh%h*h.h,
+00001ad0: 6826 6803 6827 6828 6829 4b1c 7562 682b  h&h.h'h(h)K.ubh+
+00001ae0: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+00001af0: 3029 8194 7d94 2868 058c 0c52 6571 7569  0)..}.(h...Requi
+00001b00: 7265 6d65 6e74 7394 6807 5d94 6811 8c0c  rements.h.].h...
+00001b10: 5265 7175 6972 656d 656e 7473 9485 9481  Requirements....
+00001b20: 947d 9428 6816 6a19 0200 0068 2668 0368  .}.(h.j....h&h.h
+00001b30: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
+00001b40: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00001b50: 9475 6825 682f 6816 6a16 0200 0068 2668  .uh%h/h.j....h&h
+00001b60: 0368 2768 2868 294b 3075 6268 2b29 8194  .h'h(h)K0ubh+)..
+00001b70: 7d94 2868 0568 0668 075d 9428 6830 2981  }.(h.h.h.].(h0).
+00001b80: 947d 9428 6805 8c11 4f74 6865 7220 7468  .}.(h...Other th
+00001b90: 616e 2050 7974 686f 6e94 6807 5d94 6811  an Python.h.].h.
+00001ba0: 8c11 4f74 6865 7220 7468 616e 2050 7974  ..Other than Pyt
+00001bb0: 686f 6e94 8594 8194 7d94 2868 166a 2a02  hon.....}.(h.j*.
+00001bc0: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+00001bd0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00001be0: 681f 5d94 6821 5d94 7568 2568 2f68 166a  h.].h!].uh%h/h.j
+00001bf0: 2702 0000 6826 6803 6827 6828 6829 4b33  '...h&h.h'h(h)K3
+00001c00: 7562 6840 2981 947d 9428 6805 8cac 5468  ubh@)..}.(h...Th
+00001c10: 6973 2070 6163 6b61 6765 202a 2a72 6571  is package **req
+00001c20: 7569 7265 7320 6e6f 6465 2e6a 7320 696e  uires node.js in
+00001c30: 7374 616c 6c65 642a 2a2e 2079 6f75 2063  stalled**. you c
+00001c40: 616e 2064 6f77 6e6c 6f61 6420 616e 640a  an download and.
+00001c50: 696e 7374 616c 6c20 6974 2061 7420 606e  install it at `n
+00001c60: 6f64 656a 732e 6f72 6720 3c68 7474 7073  odejs.org <https
+00001c70: 3a2f 2f6e 6f64 656a 732e 6f72 672f 656e  ://nodejs.org/en
+00001c80: 3e60 5f5f 2e20 4974 2069 7320 6176 6169  >`__. It is avai
+00001c90: 6c61 626c 650a 666f 7220 626f 7468 206d  lable.for both m
+00001ca0: 6163 4f53 2061 6e64 2057 696e 646f 7773  acOS and Windows
+00001cb0: 2066 6f72 2066 7265 652e 9468 075d 9428   for free..h.].(
+00001cc0: 6811 8c0d 5468 6973 2070 6163 6b61 6765  h...This package
+00001cd0: 2094 8594 8194 7d94 2868 166a 3802 0000   .....}.(h.j8...
+00001ce0: 6826 6803 6827 4e68 294e 7562 6809 8c06  h&h.h'Nh)Nubh...
+00001cf0: 7374 726f 6e67 9493 9429 8194 7d94 2868  strong...)..}.(h
+00001d00: 058c 1e2a 2a72 6571 7569 7265 7320 6e6f  ...**requires no
+00001d10: 6465 2e6a 7320 696e 7374 616c 6c65 642a  de.js installed*
+00001d20: 2a94 6807 5d94 6811 8c1a 7265 7175 6972  *.h.].h...requir
+00001d30: 6573 206e 6f64 652e 6a73 2069 6e73 7461  es node.js insta
+00001d40: 6c6c 6564 9485 9481 947d 9428 6816 6a42  lled.....}.(h.jB
+00001d50: 0200 0068 2668 0368 274e 6829 4e75 6261  ...h&h.h'Nh)Nuba
+00001d60: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00001d70: 9468 1f5d 9468 215d 9475 6825 6a40 0200  .h.].h!].uh%j@..
+00001d80: 0068 166a 3802 0000 7562 6811 8c25 2e20  .h.j8...ubh..%. 
+00001d90: 796f 7520 6361 6e20 646f 776e 6c6f 6164  you can download
+00001da0: 2061 6e64 0a69 6e73 7461 6c6c 2069 7420   and.install it 
+00001db0: 6174 2094 8594 8194 7d94 2868 166a 3802  at .....}.(h.j8.
+00001dc0: 0000 6826 6803 6827 4e68 294e 7562 685e  ..h&h.h'Nh)Nubh^
+00001dd0: 2981 947d 9428 6805 8c26 606e 6f64 656a  )..}.(h..&`nodej
+00001de0: 732e 6f72 6720 3c68 7474 7073 3a2f 2f6e  s.org <https://n
+00001df0: 6f64 656a 732e 6f72 672f 656e 3e60 5f5f  odejs.org/en>`__
+00001e00: 9468 075d 9468 118c 0a6e 6f64 656a 732e  .h.].h...nodejs.
+00001e10: 6f72 6794 8594 8194 7d94 2868 166a 5402  org.....}.(h.jT.
+00001e20: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+00001e30: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00001e40: 681f 5d94 6821 5d94 8c04 6e61 6d65 948c  h.].h!]...name..
+00001e50: 0a6e 6f64 656a 732e 6f72 6794 686f 8c15  .nodejs.org.ho..
+00001e60: 6874 7470 733a 2f2f 6e6f 6465 6a73 2e6f  https://nodejs.o
+00001e70: 7267 2f65 6e94 7568 2568 5d68 166a 3802  rg/en.uh%h]h.j8.
+00001e80: 0000 7562 6811 8c36 2e20 4974 2069 7320  ..ubh..6. It is 
+00001e90: 6176 6169 6c61 626c 650a 666f 7220 626f  available.for bo
+00001ea0: 7468 206d 6163 4f53 2061 6e64 2057 696e  th macOS and Win
+00001eb0: 646f 7773 2066 6f72 2066 7265 652e 9485  dows for free...
+00001ec0: 9481 947d 9428 6816 6a38 0200 0068 2668  ...}.(h.j8...h&h
+00001ed0: 0368 274e 6829 4e75 6265 6817 7d94 2868  .h'Nh)Nubeh.}.(h
+00001ee0: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+00001ef0: 215d 9475 6825 683f 6827 6828 6829 4b35  !].uh%h?h'h(h)K5
+00001f00: 6816 6a27 0200 0068 2668 0375 6265 6817  h.j'...h&h.ubeh.
+00001f10: 7d94 2868 195d 948c 116f 7468 6572 2d74  }.(h.]...other-t
+00001f20: 6861 6e2d 7079 7468 6f6e 9461 681b 5d94  han-python.ah.].
+00001f30: 681d 5d94 8c11 6f74 6865 7220 7468 616e  h.]...other than
+00001f40: 2070 7974 686f 6e94 6168 1f5d 9468 215d   python.ah.].h!]
+00001f50: 9475 6825 682a 6816 6a16 0200 0068 2668  .uh%h*h.j....h&h
+00001f60: 0368 2768 2868 294b 3375 6268 2b29 8194  .h'h(h)K3ubh+)..
+00001f70: 7d94 2868 0568 0668 075d 9428 6830 2981  }.(h.h.h.].(h0).
+00001f80: 947d 9428 6805 8c0e 5079 7468 6f6e 2076  .}.(h...Python v
+00001f90: 6572 7369 6f6e 9468 075d 9468 118c 0e50  ersion.h.].h...P
+00001fa0: 7974 686f 6e20 7665 7273 696f 6e94 8594  ython version...
+00001fb0: 8194 7d94 2868 166a 7a02 0000 6826 6803  ..}.(h.jz...h&h.
+00001fc0: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
+00001fd0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+00001fe0: 5d94 7568 2568 2f68 166a 7702 0000 6826  ].uh%h/h.jw...h&
+00001ff0: 6803 6827 6828 6829 4b3a 7562 6840 2981  h.h'h(h)K:ubh@).
+00002000: 947d 9428 6805 8c4d 5468 6973 2070 6163  .}.(h..MThis pac
+00002010: 6b61 6765 2069 7320 636f 6d70 6174 6962  kage is compatib
+00002020: 6c65 2074 6f20 616e 7920 7079 7468 6f6e  le to any python
+00002030: 2076 6572 7369 6f6e 2065 7175 616c 206f   version equal o
+00002040: 7220 6e65 7765 7220 7468 616e 0a60 6033  r newer than.``3
+00002050: 2e39 6060 2e94 6807 5d94 2868 118c 4554  .9``..h.].(h..ET
+00002060: 6869 7320 7061 636b 6167 6520 6973 2063  his package is c
+00002070: 6f6d 7061 7469 626c 6520 746f 2061 6e79  ompatible to any
+00002080: 2070 7974 686f 6e20 7665 7273 696f 6e20   python version 
+00002090: 6571 7561 6c20 6f72 206e 6577 6572 2074  equal or newer t
+000020a0: 6861 6e0a 9485 9481 947d 9428 6816 6a88  han......}.(h.j.
+000020b0: 0200 0068 2668 0368 274e 6829 4e75 6268  ...h&h.h'Nh)Nubh
+000020c0: 4a29 8194 7d94 2868 058c 0760 6033 2e39  J)..}.(h...``3.9
+000020d0: 6060 9468 075d 9468 118c 0333 2e39 9485  ``.h.].h...3.9..
+000020e0: 9481 947d 9428 6816 6a90 0200 0068 2668  ...}.(h.j....h&h
+000020f0: 0368 274e 6829 4e75 6261 6817 7d94 2868  .h'Nh)Nubah.}.(h
+00002100: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+00002110: 215d 9475 6825 6849 6816 6a88 0200 0075  !].uh%hIh.j....u
+00002120: 6268 118c 012e 9485 9481 947d 9428 6816  bh.........}.(h.
+00002130: 6a88 0200 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00002140: 6265 6817 7d94 2868 195d 9468 1b5d 9468  beh.}.(h.].h.].h
+00002150: 1d5d 9468 1f5d 9468 215d 9475 6825 683f  .].h.].h!].uh%h?
+00002160: 6827 6828 6829 4b3c 6816 6a77 0200 0068  h'h(h)K<h.jw...h
+00002170: 2668 0375 6265 6817 7d94 2868 195d 948c  &h.ubeh.}.(h.]..
+00002180: 0e70 7974 686f 6e2d 7665 7273 696f 6e94  .python-version.
+00002190: 6168 1b5d 9468 1d5d 948c 0e70 7974 686f  ah.].h.]...pytho
+000021a0: 6e20 7665 7273 696f 6e94 6168 1f5d 9468  n version.ah.].h
+000021b0: 215d 9475 6825 682a 6816 6a16 0200 0068  !].uh%h*h.j....h
+000021c0: 2668 0368 2768 2868 294b 3a75 6268 2b29  &h.h'h(h)K:ubh+)
+000021d0: 8194 7d94 2868 0568 0668 075d 9428 6830  ..}.(h.h.h.].(h0
+000021e0: 2981 947d 9428 6805 8c0f 5079 7468 6f6e  )..}.(h...Python
+000021f0: 2070 6163 6b61 6765 7394 6807 5d94 6811   packages.h.].h.
+00002200: 8c0f 5079 7468 6f6e 2070 6163 6b61 6765  ..Python package
+00002210: 7394 8594 8194 7d94 2868 166a b302 0000  s.....}.(h.j....
+00002220: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
+00002230: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+00002240: 5d94 6821 5d94 7568 2568 2f68 166a b002  ].h!].uh%h/h.j..
+00002250: 0000 6826 6803 6827 6828 6829 4b40 7562  ..h&h.h'h(h)K@ub
+00002260: 6840 2981 947d 9428 6805 8c91 5768 656e  h@)..}.(h...When
+00002270: 206d 7a64 6174 6132 6d61 7420 7769 6c6c   mzdata2mat will
+00002280: 2062 6520 696e 7374 616c 6c65 6420 6f6e   be installed on
+00002290: 2079 6f75 7220 7379 7374 656d 2c20 7468   your system, th
+000022a0: 6520 666f 6c6c 6f77 696e 6720 7061 636b  e following pack
+000022b0: 6167 6573 0a77 696c 6c20 616c 736f 2062  ages.will also b
+000022c0: 6520 696e 7374 616c 6c65 6420 2869 6620  e installed (if 
+000022d0: 7468 6579 2061 7265 206e 6f74 2920 696e  they are not) in
+000022e0: 746f 2079 6f75 7220 5079 7468 6f6e 2065  to your Python e
+000022f0: 6e76 6975 726f 6e6d 656e 7420 3a94 6807  nviuronment :.h.
+00002300: 5d94 6811 8c91 5768 656e 206d 7a64 6174  ].h...When mzdat
+00002310: 6132 6d61 7420 7769 6c6c 2062 6520 696e  a2mat will be in
+00002320: 7374 616c 6c65 6420 6f6e 2079 6f75 7220  stalled on your 
+00002330: 7379 7374 656d 2c20 7468 6520 666f 6c6c  system, the foll
+00002340: 6f77 696e 6720 7061 636b 6167 6573 0a77  owing packages.w
+00002350: 696c 6c20 616c 736f 2062 6520 696e 7374  ill also be inst
+00002360: 616c 6c65 6420 2869 6620 7468 6579 2061  alled (if they a
+00002370: 7265 206e 6f74 2920 696e 746f 2079 6f75  re not) into you
+00002380: 7220 5079 7468 6f6e 2065 6e76 6975 726f  r Python enviuro
+00002390: 6e6d 656e 7420 3a94 8594 8194 7d94 2868  nment :.....}.(h
+000023a0: 166a c102 0000 6826 6803 6827 4e68 294e  .j....h&h.h'Nh)N
+000023b0: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
+000023c0: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
+000023d0: 3f68 2768 2868 294b 4268 166a b002 0000  ?h'h(h)KBh.j....
+000023e0: 6826 6803 7562 6809 8c0d 6c69 7465 7261  h&h.ubh...litera
+000023f0: 6c5f 626c 6f63 6b94 9394 2981 947d 9428  l_block...)..}.(
+00002400: 6805 8c41 7079 6461 6e74 6963 3e3d 322e  h..Apydantic>=2.
+00002410: 362e 340a 6d61 7434 7079 3e3d 302e 362e  6.4.mat4py>=0.6.
+00002420: 300a 6a61 7661 7363 7269 7074 3e3d 3121  0.javascript>=1!
+00002430: 312e 312e 330a 636f 6c6f 7261 6d61 3e3d  1.1.3.colorama>=
+00002440: 302e 342e 3694 6807 5d94 6811 8c41 7079  0.4.6.h.].h..Apy
+00002450: 6461 6e74 6963 3e3d 322e 362e 340a 6d61  dantic>=2.6.4.ma
+00002460: 7434 7079 3e3d 302e 362e 300a 6a61 7661  t4py>=0.6.0.java
+00002470: 7363 7269 7074 3e3d 3121 312e 312e 330a  script>=1!1.1.3.
+00002480: 636f 6c6f 7261 6d61 3e3d 302e 342e 3694  colorama>=0.4.6.
+00002490: 8594 8194 7d94 6816 6ad1 0200 0073 6261  ....}.h.j....sba
+000024a0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+000024b0: 9468 1f5d 9468 215d 9468 2368 2475 6825  .h.].h!].h#h$uh%
+000024c0: 6acf 0200 0068 2768 2868 294b 4768 166a  j....h'h(h)KGh.j
+000024d0: b002 0000 6826 6803 7562 6809 8c17 7375  ....h&h.ubh...su
+000024e0: 6273 7469 7475 7469 6f6e 5f64 6566 696e  bstitution_defin
+000024f0: 6974 696f 6e94 9394 2981 947d 9428 6805  ition...)..}.(h.
+00002500: 8ca9 2e2e 207c 446f 6375 6d65 6e74 6174  .... |Documentat
+00002510: 696f 6e20 5374 6174 7573 7c20 696d 6167  ion Status| imag
+00002520: 653a 3a20 6874 7470 733a 2f2f 7265 6164  e:: https://read
+00002530: 7468 6564 6f63 732e 6f72 672f 7072 6f6a  thedocs.org/proj
+00002540: 6563 7473 2f6d 7a64 6174 6132 6d61 742f  ects/mzdata2mat/
+00002550: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00002560: 6174 6573 740a 2020 203a 7461 7267 6574  atest.   :target
+00002570: 3a20 6874 7470 733a 2f2f 6d7a 6461 7461  : https://mzdata
+00002580: 326d 6174 2e72 6561 6474 6865 646f 6373  2mat.readthedocs
+00002590: 2e69 6f2f 656e 2f6c 6174 6573 742f 3f62  .io/en/latest/?b
+000025a0: 6164 6765 3d6c 6174 6573 7494 6807 5d94  adge=latest.h.].
+000025b0: 685e 2981 947d 9428 6805 68b9 6807 5d94  h^)..}.(h.h.h.].
+000025c0: 68ad 2981 947d 9428 6805 68b1 6807 5d94  h.)..}.(h.h.h.].
+000025d0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+000025e0: 9468 1f5d 9468 215d 9468 b868 b968 ba68  .h.].h!].h.h.h.h
+000025f0: bb68 bc7d 9468 be68 bb73 7568 2568 ac68  .h.}.h.h.suh%h.h
+00002600: 166a e502 0000 6827 6828 6829 4b00 7562  .j....h'h(h)K.ub
+00002610: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
+00002620: 5d94 681f 5d94 6821 5d94 68c5 68c6 7568  ].h.].h!].h.h.uh
+00002630: 2568 5d68 166a e102 0000 7562 6168 177d  %h]h.j....ubah.}
+00002640: 9428 6819 5d94 681b 5d94 681d 5d94 68b9  .(h.].h.].h.].h.
+00002650: 6168 1f5d 9468 215d 9475 6825 6adf 0200  ah.].h!].uh%j...
+00002660: 0068 2768 2868 294b 4c68 166a b002 0000  .h'h(h)KLh.j....
+00002670: 6826 6803 7562 6ae0 0200 0029 8194 7d94  h&h.ubj....)..}.
+00002680: 2868 058c 6b2e 2e20 7c50 7950 497c 2069  (h..k.. |PyPI| i
+00002690: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f69  mage:: https://i
+000026a0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000026b0: 7069 2f76 2f6d 7a64 6174 6132 6d61 740a  pi/v/mzdata2mat.
+000026c0: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
+000026d0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000026e0: 6a65 6374 2f6d 7a64 6174 6132 6d61 742f  ject/mzdata2mat/
+000026f0: 9468 075d 9468 5e29 8194 7d94 2868 0568  .h.].h^)..}.(h.h
+00002700: d968 075d 9468 ad29 8194 7d94 2868 0568  .h.].h.)..}.(h.h
+00002710: d168 075d 9468 177d 9428 6819 5d94 681b  .h.].h.}.(h.].h.
+00002720: 5d94 681d 5d94 681f 5d94 6821 5d94 68d8  ].h.].h.].h!].h.
+00002730: 68d9 68da 68db 68bc 7d94 68be 68db 7375  h.h.h.h.}.h.h.su
+00002740: 6825 68ac 6816 6a02 0300 0068 2768 2868  h%h.h.j....h'h(h
+00002750: 294b 0075 6261 6817 7d94 2868 195d 9468  )K.ubah.}.(h.].h
+00002760: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9468  .].h.].h.].h!].h
+00002770: e368 e475 6825 685d 6816 6afe 0200 0075  .h.uh%h]h.j....u
+00002780: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00002790: 1d5d 9468 d961 681f 5d94 6821 5d94 7568  .].h.ah.].h!].uh
+000027a0: 256a df02 0000 6827 6828 6829 4b4e 6816  %j....h'h(h)KNh.
+000027b0: 6ab0 0200 0068 2668 0375 626a e002 0000  j....h&h.ubj....
+000027c0: 2981 947d 9428 6805 8c78 2e2e 207c 646f  )..}.(h..x.. |do
+000027d0: 776e 6c6f 6164 737c 2069 6d61 6765 3a3a  wnloads| image::
+000027e0: 2068 7474 7073 3a2f 2f73 7461 7469 632e   https://static.
+000027f0: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
+00002800: 6d7a 6461 7461 326d 6174 2f6d 6f6e 7468  mzdata2mat/month
+00002810: 0a20 2020 3a74 6172 6765 743a 2068 7474  .   :target: htt
+00002820: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+00002830: 726f 6a65 6374 2f6d 7a64 6174 6132 6d61  roject/mzdata2ma
+00002840: 740a 9468 075d 9468 5e29 8194 7d94 2868  t..h.].h^)..}.(h
+00002850: 0568 f768 075d 9468 ad29 8194 7d94 2868  .h.h.].h.)..}.(h
+00002860: 0568 ef68 075d 9468 177d 9428 6819 5d94  .h.h.].h.}.(h.].
+00002870: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+00002880: 68f6 68f7 68f8 68f9 68bc 7d94 68be 68f9  h.h.h.h.h.}.h.h.
+00002890: 7375 6825 68ac 6816 6a1f 0300 0068 2768  suh%h.h.j....h'h
+000028a0: 2868 294b 0075 6261 6817 7d94 2868 195d  (h)K.ubah.}.(h.]
+000028b0: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+000028c0: 946a 0101 0000 6a02 0100 0075 6825 685d  .j....j....uh%h]
+000028d0: 6816 6a1b 0300 0075 6261 6817 7d94 2868  h.j....ubah.}.(h
+000028e0: 195d 9468 1b5d 9468 1d5d 9468 f761 681f  .].h.].h.].h.ah.
+000028f0: 5d94 6821 5d94 7568 256a df02 0000 6827  ].h!].uh%j....h'
+00002900: 6828 6829 4b50 6816 6ab0 0200 0068 2668  h(h)KPh.j....h&h
+00002910: 0375 6268 098c 0863 6f6d 706f 756e 6494  .ubh...compound.
+00002920: 9394 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00002930: 6800 8c07 746f 6374 7265 6594 9394 2981  h...toctree...).
+00002940: 947d 9428 6805 6806 6807 5d94 6817 7d94  .}.(h.h.h.].h.}.
+00002950: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00002960: 9468 215d 9468 168c 0569 6e64 6578 948c  .h!].h...index..
+00002970: 0765 6e74 7269 6573 945d 944e 8c09 4368  .entries.].N..Ch
+00002980: 616e 6765 6c6f 6794 8694 618c 0c69 6e63  angelog...a..inc
+00002990: 6c75 6465 6669 6c65 7394 5d94 6a4b 0300  ludefiles.].jK..
+000029a0: 0061 8c08 6d61 7864 6570 7468 944b 048c  .a..maxdepth.K..
+000029b0: 0763 6170 7469 6f6e 948c 0549 6e66 6f73  .caption...Infos
+000029c0: 948c 0467 6c6f 6294 898c 0668 6964 6465  ...glob....hidde
+000029d0: 6e94 888c 0d69 6e63 6c75 6465 6869 6464  n....includehidd
+000029e0: 656e 9489 8c08 6e75 6d62 6572 6564 944b  en....numbered.K
+000029f0: 008c 0a74 6974 6c65 736f 6e6c 7994 898c  ...titlesonly...
+00002a00: 0a72 6177 656e 7472 6965 7394 5d94 8c0a  .rawentries.]...
+00002a10: 7261 7763 6170 7469 6f6e 946a 5103 0000  rawcaption.jQ...
+00002a20: 7568 256a 3d03 0000 6827 6828 6829 4b53  uh%j=...h'h(h)KS
+00002a30: 6816 6a3a 0300 0075 6261 6817 7d94 2868  h.j:...ubah.}.(h
+00002a40: 195d 9468 1b5d 948c 0f74 6f63 7472 6565  .].h.]...toctree
+00002a50: 2d77 7261 7070 6572 9461 681d 5d94 681f  -wrapper.ah.].h.
+00002a60: 5d94 6821 5d94 7568 256a 3803 0000 6816  ].h!].uh%j8...h.
+00002a70: 6ab0 0200 0068 2668 0368 2768 2868 294e  j....h&h.h'h(h)N
+00002a80: 7562 6a39 0300 0029 8194 7d94 2868 0568  ubj9...)..}.(h.h
+00002a90: 0668 075d 946a 3e03 0000 2981 947d 9428  .h.].j>...)..}.(
+00002aa0: 6805 6806 6807 5d94 6817 7d94 2868 195d  h.h.h.].h.}.(h.]
+00002ab0: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00002ac0: 9468 166a 4803 0000 6a49 0300 005d 9428  .h.jH...jI...].(
+00002ad0: 4e8c 0c69 6e73 7461 6c6c 6174 696f 6e94  N..installation.
+00002ae0: 8694 4e8c 0c63 6f64 652d 6578 616d 706c  ..N..code-exampl
+00002af0: 6594 8694 656a 4d03 0000 5d94 286a 6e03  e...ejM...].(jn.
+00002b00: 0000 6a70 0300 0065 6a4f 0300 004b 046a  ..jp...ejO...K.j
+00002b10: 5003 0000 8c0a 5175 6963 6b73 7461 7274  P.....Quickstart
+00002b20: 946a 5203 0000 896a 5303 0000 886a 5403  .jR....jS....jT.
+00002b30: 0000 896a 5503 0000 4b00 6a56 0300 0089  ...jU...K.jV....
+00002b40: 6a57 0300 005d 946a 5903 0000 6a73 0300  jW...].jY...js..
+00002b50: 0075 6825 6a3d 0300 0068 2768 2868 294b  .uh%j=...h'h(h)K
+00002b60: 5a68 166a 6103 0000 7562 6168 177d 9428  Zh.ja...ubah.}.(
+00002b70: 6819 5d94 681b 5d94 6a5d 0300 0061 681d  h.].h.].j]...ah.
+00002b80: 5d94 681f 5d94 6821 5d94 7568 256a 3803  ].h.].h!].uh%j8.
+00002b90: 0000 6816 6ab0 0200 0068 2668 0368 2768  ..h.j....h&h.h'h
+00002ba0: 2868 294e 7562 6a39 0300 0029 8194 7d94  (h)Nubj9...)..}.
+00002bb0: 2868 0568 0668 075d 946a 3e03 0000 2981  (h.h.h.].j>...).
+00002bc0: 947d 9428 6805 6806 6807 5d94 6817 7d94  .}.(h.h.h.].h.}.
+00002bd0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00002be0: 9468 215d 9468 166a 4803 0000 6a49 0300  .h!].h.jH...jI..
+00002bf0: 005d 944e 8c15 6164 7661 6e63 6564 4c6f  .].N..advancedLo
+00002c00: 6164 5361 7665 4c6f 6769 6394 8694 616a  adSaveLogic...aj
+00002c10: 4d03 0000 5d94 6a88 0300 0061 6a4f 0300  M...].j....ajO..
+00002c20: 004b 046a 5003 0000 8c08 4164 7661 6e63  .K.jP.....Advanc
+00002c30: 6564 946a 5203 0000 896a 5303 0000 886a  ed.jR....jS....j
+00002c40: 5403 0000 896a 5503 0000 4b00 6a56 0300  T....jU...K.jV..
+00002c50: 0089 6a57 0300 005d 946a 5903 0000 6a8b  ..jW...].jY...j.
+00002c60: 0300 0075 6825 6a3d 0300 0068 2768 2868  ...uh%j=...h'h(h
+00002c70: 294b 6268 166a 7b03 0000 7562 6168 177d  )Kbh.j{...ubah.}
+00002c80: 9428 6819 5d94 681b 5d94 6a5d 0300 0061  .(h.].h.].j]...a
+00002c90: 681d 5d94 681f 5d94 6821 5d94 7568 256a  h.].h.].h!].uh%j
+00002ca0: 3803 0000 6816 6ab0 0200 0068 2668 0368  8...h.j....h&h.h
+00002cb0: 2768 2868 294e 7562 6a39 0300 0029 8194  'h(h)Nubj9...)..
+00002cc0: 7d94 2868 0568 0668 075d 946a 3e03 0000  }.(h.h.h.].j>...
+00002cd0: 2981 947d 9428 6805 6806 6807 5d94 6817  )..}.(h.h.h.].h.
+00002ce0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00002cf0: 1f5d 9468 215d 9468 166a 4803 0000 6a49  .].h!].h.jH...jI
+00002d00: 0300 005d 9428 4e8c 0d6d 7a44 6174 614d  ...].(N..mzDataM
+00002d10: 616e 6167 6572 9486 944e 8c09 6d61 7453  anager...N..matS
+00002d20: 7472 7563 7494 8694 4e8c 066d 7a44 6174  truct...N..mzDat
+00002d30: 6194 8694 4e8c 0f6d 7a44 6174 6158 4d4c  a...N..mzDataXML
+00002d40: 5374 7275 6374 9486 9465 6a4d 0300 005d  Struct...ejM...]
+00002d50: 9428 6aa0 0300 006a a203 0000 6aa4 0300  .(j....j....j...
+00002d60: 006a a603 0000 656a 4f03 0000 4b04 6a50  .j....ejO...K.jP
+00002d70: 0300 008c 0d41 5049 2052 6566 6572 656e  .....API Referen
+00002d80: 6365 946a 5203 0000 896a 5303 0000 886a  ce.jR....jS....j
+00002d90: 5403 0000 896a 5503 0000 4b00 6a56 0300  T....jU...K.jV..
+00002da0: 0089 6a57 0300 005d 946a 5903 0000 6aa9  ..jW...].jY...j.
+00002db0: 0300 0075 6825 6a3d 0300 0068 2768 2868  ...uh%j=...h'h(h
+00002dc0: 294b 6968 166a 9303 0000 7562 6168 177d  )Kih.j....ubah.}
+00002dd0: 9428 6819 5d94 681b 5d94 6a5d 0300 0061  .(h.].h.].j]...a
+00002de0: 681d 5d94 681f 5d94 6821 5d94 7568 256a  h.].h.].h!].uh%j
+00002df0: 3803 0000 6816 6ab0 0200 0068 2668 0368  8...h.j....h&h.h
+00002e00: 2768 2868 294e 7562 6a39 0300 0029 8194  'h(h)Nubj9...)..
+00002e10: 7d94 2868 0568 0668 075d 946a 3e03 0000  }.(h.h.h.].j>...
+00002e20: 2981 947d 9428 6805 6806 6807 5d94 6817  )..}.(h.h.h.].h.
+00002e30: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00002e40: 1f5d 9468 215d 9468 166a 4803 0000 6a49  .].h!].h.jH...jI
+00002e50: 0300 005d 944e 8c11 6d7a 6461 7461 326d  ...].N..mzdata2m
+00002e60: 6174 2d76 6572 6966 7994 8694 616a 4d03  at-verify...ajM.
+00002e70: 0000 5d94 6abe 0300 0061 6a4f 0300 004b  ..].j....ajO...K
+00002e80: 046a 5003 0000 8c03 434c 4994 6a52 0300  .jP.....CLI.jR..
+00002e90: 0089 6a53 0300 0088 6a54 0300 0089 6a55  ..jS....jT....jU
+00002ea0: 0300 004b 006a 5603 0000 896a 5703 0000  ...K.jV....jW...
+00002eb0: 5d94 6a59 0300 006a c103 0000 7568 256a  ].jY...j....uh%j
+00002ec0: 3d03 0000 6827 6828 6829 4b73 6816 6ab1  =...h'h(h)Ksh.j.
+00002ed0: 0300 0075 6261 6817 7d94 2868 195d 9468  ...ubah.}.(h.].h
+00002ee0: 1b5d 946a 5d03 0000 6168 1d5d 9468 1f5d  .].j]...ah.].h.]
+00002ef0: 9468 215d 9475 6825 6a38 0300 0068 166a  .h!].uh%j8...h.j
+00002f00: b002 0000 6826 6803 6827 6828 6829 4e75  ....h&h.h'h(h)Nu
+00002f10: 6265 6817 7d94 2868 195d 948c 0f70 7974  beh.}.(h.]...pyt
+00002f20: 686f 6e2d 7061 636b 6167 6573 9461 681b  hon-packages.ah.
+00002f30: 5d94 681d 5d94 8c0f 7079 7468 6f6e 2070  ].h.]...python p
+00002f40: 6163 6b61 6765 7394 6168 1f5d 9468 215d  ackages.ah.].h!]
+00002f50: 9475 6825 682a 6816 6a16 0200 0068 2668  .uh%h*h.j....h&h
+00002f60: 0368 2768 2868 294b 4075 6265 6817 7d94  .h'h(h)K@ubeh.}.
+00002f70: 2868 195d 948c 0c72 6571 7569 7265 6d65  (h.]...requireme
+00002f80: 6e74 7394 6168 1b5d 9468 1d5d 948c 0c72  nts.ah.].h.]...r
+00002f90: 6571 7569 7265 6d65 6e74 7394 6168 1f5d  equirements.ah.]
+00002fa0: 9468 215d 9475 6825 682a 6816 682c 6826  .h!].uh%h*h.h,h&
+00002fb0: 6803 6827 6828 6829 4b30 7562 6568 177d  h.h'h(h)K0ubeh.}
+00002fc0: 9428 6819 5d94 8c07 7765 6c63 6f6d 6594  .(h.]...welcome.
+00002fd0: 6168 1b5d 9468 1d5d 948c 0777 656c 636f  ah.].h.]...welco
+00002fe0: 6d65 9461 681f 5d94 6821 5d94 7568 2568  me.ah.].h!].uh%h
+00002ff0: 2a68 1668 0368 2668 0368 2768 2868 294b  *h.h.h&h.h'h(h)K
+00003000: 0775 6265 6817 7d94 2868 195d 9468 1b5d  .ubeh.}.(h.].h.]
+00003010: 9468 1d5d 9468 1f5d 9468 215d 948c 0673  .h.].h.].h!]...s
+00003020: 6f75 7263 6594 6828 8c14 7472 616e 736c  ource.h(..transl
+00003030: 6174 696f 6e5f 7072 6f67 7265 7373 947d  ation_progress.}
+00003040: 9428 8c05 746f 7461 6c94 4b00 8c0a 7472  .(..total.K...tr
+00003050: 616e 736c 6174 6564 944b 0075 7568 2568  anslated.K.uuh%h
+00003060: 018c 0e63 7572 7265 6e74 5f73 6f75 7263  ...current_sourc
+00003070: 6594 4e8c 0c63 7572 7265 6e74 5f6c 696e  e.N..current_lin
+00003080: 6594 4e8c 0873 6574 7469 6e67 7394 8c11  e.N..settings...
+00003090: 646f 6375 7469 6c73 2e66 726f 6e74 656e  docutils.fronten
+000030a0: 6494 8c06 5661 6c75 6573 9493 9429 8194  d...Values...)..
+000030b0: 7d94 288c 066f 7574 7075 7494 4e68 2f4e  }.(..output.Nh/N
+000030c0: 8c09 6765 6e65 7261 746f 7294 4e8c 0964  ..generator.N..d
+000030d0: 6174 6573 7461 6d70 944e 8c0b 736f 7572  atestamp.N..sour
+000030e0: 6365 5f6c 696e 6b94 4e8c 0a73 6f75 7263  ce_link.N..sourc
+000030f0: 655f 7572 6c94 4e8c 0d74 6f63 5f62 6163  e_url.N..toc_bac
+00003100: 6b6c 696e 6b73 948c 0565 6e74 7279 948c  klinks...entry..
+00003110: 1266 6f6f 746e 6f74 655f 6261 636b 6c69  .footnote_backli
+00003120: 6e6b 7394 4b01 8c0d 7365 6374 6e75 6d5f  nks.K...sectnum_
+00003130: 7866 6f72 6d94 4b01 8c0e 7374 7269 705f  xform.K...strip_
+00003140: 636f 6d6d 656e 7473 944e 8c1b 7374 7269  comments.N..stri
+00003150: 705f 656c 656d 656e 7473 5f77 6974 685f  p_elements_with_
+00003160: 636c 6173 7365 7394 4e8c 0d73 7472 6970  classes.N..strip
+00003170: 5f63 6c61 7373 6573 944e 8c0c 7265 706f  _classes.N..repo
+00003180: 7274 5f6c 6576 656c 944b 028c 0a68 616c  rt_level.K...hal
+00003190: 745f 6c65 7665 6c94 4b05 8c11 6578 6974  t_level.K...exit
+000031a0: 5f73 7461 7475 735f 6c65 7665 6c94 4b05  _status_level.K.
+000031b0: 8c05 6465 6275 6794 4e8c 0e77 6172 6e69  ..debug.N..warni
+000031c0: 6e67 5f73 7472 6561 6d94 4e8c 0974 7261  ng_stream.N..tra
+000031d0: 6365 6261 636b 9488 8c0e 696e 7075 745f  ceback....input_
+000031e0: 656e 636f 6469 6e67 948c 0975 7466 2d38  encoding...utf-8
+000031f0: 2d73 6967 948c 1c69 6e70 7574 5f65 6e63  -sig...input_enc
+00003200: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
+00003210: 6c65 7294 8c06 7374 7269 6374 948c 0f6f  ler...strict...o
+00003220: 7574 7075 745f 656e 636f 6469 6e67 948c  utput_encoding..
+00003230: 0575 7466 2d38 948c 1d6f 7574 7075 745f  .utf-8...output_
+00003240: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
+00003250: 616e 646c 6572 946a 0904 0000 8c0e 6572  andler.j......er
+00003260: 726f 725f 656e 636f 6469 6e67 948c 0575  ror_encoding...u
+00003270: 7466 2d38 948c 1c65 7272 6f72 5f65 6e63  tf-8...error_enc
+00003280: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
+00003290: 6c65 7294 8c10 6261 636b 736c 6173 6872  ler...backslashr
+000032a0: 6570 6c61 6365 948c 0d6c 616e 6775 6167  eplace...languag
+000032b0: 655f 636f 6465 948c 0265 6e94 8c13 7265  e_code...en...re
+000032c0: 636f 7264 5f64 6570 656e 6465 6e63 6965  cord_dependencie
+000032d0: 7394 4e8c 0663 6f6e 6669 6794 4e8c 0969  s.N..config.N..i
+000032e0: 645f 7072 6566 6978 9468 068c 0e61 7574  d_prefix.h...aut
+000032f0: 6f5f 6964 5f70 7265 6669 7894 8c02 6964  o_id_prefix...id
+00003300: 948c 0d64 756d 705f 7365 7474 696e 6773  ...dump_settings
+00003310: 944e 8c0e 6475 6d70 5f69 6e74 6572 6e61  .N..dump_interna
+00003320: 6c73 944e 8c0f 6475 6d70 5f74 7261 6e73  ls.N..dump_trans
+00003330: 666f 726d 7394 4e8c 0f64 756d 705f 7073  forms.N..dump_ps
+00003340: 6575 646f 5f78 6d6c 944e 8c10 6578 706f  eudo_xml.N..expo
+00003350: 7365 5f69 6e74 6572 6e61 6c73 944e 8c0e  se_internals.N..
+00003360: 7374 7269 6374 5f76 6973 6974 6f72 944e  strict_visitor.N
+00003370: 8c0f 5f64 6973 6162 6c65 5f63 6f6e 6669  .._disable_confi
+00003380: 6794 4e8c 075f 736f 7572 6365 9468 288c  g.N.._source.h(.
+00003390: 0c5f 6465 7374 696e 6174 696f 6e94 4e8c  ._destination.N.
+000033a0: 0d5f 636f 6e66 6967 5f66 696c 6573 945d  ._config_files.]
+000033b0: 948c 1666 696c 655f 696e 7365 7274 696f  ...file_insertio
+000033c0: 6e5f 656e 6162 6c65 6494 888c 0b72 6177  n_enabled....raw
+000033d0: 5f65 6e61 626c 6564 944b 018c 116c 696e  _enabled.K...lin
+000033e0: 655f 6c65 6e67 7468 5f6c 696d 6974 944d  e_length_limit.M
+000033f0: 1027 8c0e 7065 705f 7265 6665 7265 6e63  .'..pep_referenc
+00003400: 6573 944e 8c0c 7065 705f 6261 7365 5f75  es.N..pep_base_u
+00003410: 726c 948c 1868 7474 7073 3a2f 2f70 6570  rl...https://pep
+00003420: 732e 7079 7468 6f6e 2e6f 7267 2f94 8c15  s.python.org/...
+00003430: 7065 705f 6669 6c65 5f75 726c 5f74 656d  pep_file_url_tem
+00003440: 706c 6174 6594 8c08 7065 702d 2530 3464  plate...pep-%04d
+00003450: 948c 0e72 6663 5f72 6566 6572 656e 6365  ...rfc_reference
+00003460: 7394 4e8c 0c72 6663 5f62 6173 655f 7572  s.N..rfc_base_ur
+00003470: 6c94 8c26 6874 7470 733a 2f2f 6461 7461  l..&https://data
+00003480: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
+00003490: 2f64 6f63 2f68 746d 6c2f 948c 0974 6162  /doc/html/...tab
+000034a0: 5f77 6964 7468 944b 088c 1d74 7269 6d5f  _width.K...trim_
+000034b0: 666f 6f74 6e6f 7465 5f72 6566 6572 656e  footnote_referen
+000034c0: 6365 5f73 7061 6365 9489 8c10 7379 6e74  ce_space....synt
+000034d0: 6178 5f68 6967 686c 6967 6874 948c 046c  ax_highlight...l
+000034e0: 6f6e 6794 8c0c 736d 6172 745f 7175 6f74  ong...smart_quot
+000034f0: 6573 9488 8c13 736d 6172 7471 756f 7465  es....smartquote
+00003500: 735f 6c6f 6361 6c65 7394 5d94 8c1d 6368  s_locales.]...ch
+00003510: 6172 6163 7465 725f 6c65 7665 6c5f 696e  aracter_level_in
+00003520: 6c69 6e65 5f6d 6172 6b75 7094 898c 0e64  line_markup....d
+00003530: 6f63 7469 746c 655f 7866 6f72 6d94 898c  octitle_xform...
+00003540: 0d64 6f63 696e 666f 5f78 666f 726d 944b  .docinfo_xform.K
+00003550: 018c 1273 6563 7473 7562 7469 746c 655f  ...sectsubtitle_
+00003560: 7866 6f72 6d94 898c 0d69 6d61 6765 5f6c  xform....image_l
+00003570: 6f61 6469 6e67 948c 046c 696e 6b94 8c10  oading...link...
+00003580: 656d 6265 645f 7374 796c 6573 6865 6574  embed_stylesheet
+00003590: 9489 8c15 636c 6f61 6b5f 656d 6169 6c5f  ....cloak_email_
+000035a0: 6164 6472 6573 7365 7394 888c 1173 6563  addresses....sec
+000035b0: 7469 6f6e 5f73 656c 665f 6c69 6e6b 9489  tion_self_link..
+000035c0: 8c03 656e 7694 4e75 628c 0872 6570 6f72  ..env.Nub..repor
+000035d0: 7465 7294 4e8c 1069 6e64 6972 6563 745f  ter.N..indirect_
+000035e0: 7461 7267 6574 7394 5d94 8c11 7375 6273  targets.]...subs
+000035f0: 7469 7475 7469 6f6e 5f64 6566 7394 7d94  titution_defs.}.
+00003600: 288c 1444 6f63 756d 656e 7461 7469 6f6e  (..Documentation
+00003610: 2053 7461 7475 7394 6ae1 0200 0068 d96a   Status.j....h.j
+00003620: fe02 0000 68f7 6a1b 0300 0075 8c12 7375  ....h.j....u..su
+00003630: 6273 7469 7475 7469 6f6e 5f6e 616d 6573  bstitution_names
+00003640: 947d 9428 8c14 646f 6375 6d65 6e74 6174  .}.(..documentat
+00003650: 696f 6e20 7374 6174 7573 946a 4404 0000  ion status.jD...
+00003660: 8c04 7079 7069 9468 d98c 0964 6f77 6e6c  ..pypi.h...downl
+00003670: 6f61 6473 9468 f775 8c08 7265 666e 616d  oads.h.u..refnam
+00003680: 6573 947d 948c 0672 6566 6964 7394 7d94  es.}...refids.}.
+00003690: 8c07 6e61 6d65 6964 7394 7d94 286a de03  ..nameids.}.(j..
+000036a0: 0000 6adb 0300 006a 6801 0000 6a65 0100  ..j....jh...je..
+000036b0: 006a 1302 0000 6a10 0200 006a c001 0000  .j....j....j....
+000036c0: 6abd 0100 006a 0b02 0000 6a08 0200 006a  j....j....j....j
+000036d0: d603 0000 6ad3 0300 006a 7402 0000 6a71  ....j....jt...jq
+000036e0: 0200 006a ad02 0000 6aaa 0200 006a ce03  ...j....j....j..
+000036f0: 0000 6acb 0300 0075 8c09 6e61 6d65 7479  ..j....u..namety
+00003700: 7065 7394 7d94 286a de03 0000 896a 6801  pes.}.(j.....jh.
+00003710: 0000 896a 1302 0000 896a c001 0000 896a  ...j.....j.....j
+00003720: 0b02 0000 896a d603 0000 896a 7402 0000  .....j.....jt...
+00003730: 896a ad02 0000 896a ce03 0000 8975 6819  .j.....j.....uh.
+00003740: 7d94 286a db03 0000 682c 6a65 0100 006a  }.(j....h,je...j
+00003750: 0901 0000 6a10 0200 006a 6b01 0000 6abd  ....j....jk...j.
+00003760: 0100 006a 8a01 0000 6a08 0200 006a c301  ...j....j....j..
+00003770: 0000 6ad3 0300 006a 1602 0000 6a71 0200  ..j....j....jq..
+00003780: 006a 2702 0000 6aaa 0200 006a 7702 0000  .j'...j....jw...
+00003790: 6acb 0300 006a b002 0000 758c 0d66 6f6f  j....j....u..foo
+000037a0: 746e 6f74 655f 7265 6673 947d 948c 0d63  tnote_refs.}...c
+000037b0: 6974 6174 696f 6e5f 7265 6673 947d 948c  itation_refs.}..
+000037c0: 0d61 7574 6f66 6f6f 746e 6f74 6573 945d  .autofootnotes.]
+000037d0: 948c 1161 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+000037e0: 7265 6673 945d 948c 1073 796d 626f 6c5f  refs.]...symbol_
+000037f0: 666f 6f74 6e6f 7465 7394 5d94 8c14 7379  footnotes.]...sy
+00003800: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7265  mbol_footnote_re
+00003810: 6673 945d 948c 0966 6f6f 746e 6f74 6573  fs.]...footnotes
+00003820: 945d 948c 0963 6974 6174 696f 6e73 945d  .]...citations.]
+00003830: 948c 1261 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+00003840: 7374 6172 7494 4b01 8c15 7379 6d62 6f6c  start.K...symbol
+00003850: 5f66 6f6f 746e 6f74 655f 7374 6172 7494  _footnote_start.
+00003860: 4b00 8c0a 6964 5f63 6f75 6e74 6572 948c  K...id_counter..
+00003870: 0b63 6f6c 6c65 6374 696f 6e73 948c 0743  .collections...C
+00003880: 6f75 6e74 6572 9493 947d 9485 9452 948c  ounter...}...R..
+00003890: 0e70 6172 7365 5f6d 6573 7361 6765 7394  .parse_messages.
+000038a0: 5d94 8c12 7472 616e 7366 6f72 6d5f 6d65  ]...transform_me
+000038b0: 7373 6167 6573 945d 948c 0b74 7261 6e73  ssages.]...trans
+000038c0: 666f 726d 6572 944e 8c0b 696e 636c 7564  former.N..includ
+000038d0: 655f 6c6f 6794 5d94 8c0a 6465 636f 7261  e_log.]...decora
+000038e0: 7469 6f6e 944e 6826 6803 7562 2e         tion.Nh&h.ub.
```

### Comparing `mzdata2mat-0.1.1/docs/build/doctrees/installation.doctree` & `mzdata2mat-0.2.0/docs/build/doctrees/installation.doctree`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 95f5 2200 0000 0000 008c 0f73 7068  ...."........sph
+00000000: 8005 95e0 2200 0000 0000 008c 0f73 7068  ...."........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -14,547 +14,546 @@
 000000d0: 6375 6d65 6e74 9468 038c 0673 6f75 7263  cument.h...sourc
 000000e0: 6594 4e8c 046c 696e 6594 4e75 6261 8c0a  e.N..line.Nuba..
 000000f0: 6174 7472 6962 7574 6573 947d 9428 8c03  attributes.}.(..
 00000100: 6964 7394 5d94 8c07 636c 6173 7365 7394  ids.]...classes.
 00000110: 5d94 8c05 6e61 6d65 7394 5d94 8c08 6475  ]...names.]...du
 00000120: 706e 616d 6573 945d 948c 0862 6163 6b72  pnames.]...backr
 00000130: 6566 7394 5d94 758c 0774 6167 6e61 6d65  efs.].u..tagname
-00000140: 9468 0f68 1e4b 0168 1d8c 7a2f 5573 6572  .h.h.K.h..z/User
-00000150: 732f 6c69 6368 3931 312f 4c69 6272 6172  s/lich911/Librar
-00000160: 792f 436c 6f75 6453 746f 7261 6765 2f4f  y/CloudStorage/O
-00000170: 6e65 4472 6976 652d 5065 7273 6f6e 6e65  neDrive-Personne
-00000180: 6c2f 446f 6375 6d65 6e74 732f 5079 7468  l/Documents/Pyth
-00000190: 6f6e 2f50 6163 6b61 6765 732f 6d7a 4461  on/Packages/mzDa
-000001a0: 7461 584d 4c32 4d61 742f 646f 6373 2f73  taXML2Mat/docs/s
-000001b0: 6f75 7263 652f 696e 7374 616c 6c61 7469  ource/installati
-000001c0: 6f6e 2e6d 6494 681b 680c 681c 6803 7562  on.md.h.h.h.h.ub
-000001d0: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
-000001e0: 2868 1029 8194 7d94 2868 058c 0743 6f6d  (h.)..}.(h...Com
-000001f0: 6d61 6e64 9468 075d 9468 168c 0743 6f6d  mand.h.].h...Com
-00000200: 6d61 6e64 9485 9481 947d 9428 681b 6830  mand.....}.(h.h0
-00000210: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00000220: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00000230: 5d94 6829 5d94 7568 2b68 0f68 1e4b 0268  ].h)].uh+h.h.K.h
-00000240: 1d68 2c68 1b68 2d68 1c68 0375 6268 098c  .h,h.h-h.h.ubh..
-00000250: 0970 6172 6167 7261 7068 9493 9429 8194  .paragraph...)..
-00000260: 7d94 2868 058c 6654 6f20 696e 7374 616c  }.(h..fTo instal
-00000270: 6c20 606d 7a64 6174 6132 6d61 7460 2069  l `mzdata2mat` i
-00000280: 6e74 6f20 796f 7572 2050 7974 686f 6e20  nto your Python 
-00000290: 656e 7669 726f 6e6d 656e 742c 2072 756e  environment, run
-000002a0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-000002b0: 6f6d 6d61 6e64 2069 6e73 6964 6520 796f  ommand inside yo
-000002c0: 7572 2074 6572 6d69 6e61 6c20 3a94 6807  ur terminal :.h.
-000002d0: 5d94 2868 168c 0b54 6f20 696e 7374 616c  ].(h...To instal
-000002e0: 6c20 9485 9481 947d 9428 681b 6840 681c  l .....}.(h.h@h.
-000002f0: 6803 681d 4e68 1e4e 7562 6809 8c07 6c69  h.h.Nh.Nubh...li
-00000300: 7465 7261 6c94 9394 2981 947d 9428 6805  teral...)..}.(h.
-00000310: 8c0a 6d7a 6461 7461 326d 6174 9468 075d  ..mzdata2mat.h.]
-00000320: 9468 168c 0a6d 7a64 6174 6132 6d61 7494  .h...mzdata2mat.
-00000330: 8594 8194 7d94 2868 1b68 4a68 1c68 0368  ....}.(h.hJh.h.h
-00000340: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00000350: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00000360: 9475 682b 6848 681e 4b03 681d 682c 681b  .uh+hHh.K.h.h,h.
-00000370: 6840 681c 6803 7562 6816 8c4f 2069 6e74  h@h.h.ubh..O int
-00000380: 6f20 796f 7572 2050 7974 686f 6e20 656e  o your Python en
-00000390: 7669 726f 6e6d 656e 742c 2072 756e 2074  vironment, run t
-000003a0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-000003b0: 6d61 6e64 2069 6e73 6964 6520 796f 7572  mand inside your
-000003c0: 2074 6572 6d69 6e61 6c20 3a94 8594 8194   terminal :.....
-000003d0: 7d94 2868 1b68 4068 1c68 0368 1d4e 681e  }.(h.h@h.h.h.Nh.
-000003e0: 4e75 6265 681f 7d94 2868 215d 9468 235d  Nubeh.}.(h!].h#]
-000003f0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00000400: 683e 681e 4b03 681d 682c 681b 682d 681c  h>h.K.h.h,h.h-h.
-00000410: 6803 7562 6809 8c0d 6c69 7465 7261 6c5f  h.ubh...literal_
-00000420: 626c 6f63 6b94 9394 2981 947d 9428 6805  block...)..}.(h.
-00000430: 8c19 2420 7069 7020 696e 7374 616c 6c20  ..$ pip install 
-00000440: 6d7a 6461 7461 326d 6174 0a94 6807 5d94  mzdata2mat..h.].
-00000450: 6816 8c19 2420 7069 7020 696e 7374 616c  h...$ pip instal
-00000460: 6c20 6d7a 6461 7461 326d 6174 0a94 8594  l mzdata2mat....
-00000470: 8194 7d94 681b 6864 7362 6168 1f7d 9428  ..}.h.hdsbah.}.(
-00000480: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00000490: 6829 5d94 8c08 6c61 6e67 7561 6765 948c  h)]...language..
-000004a0: 0573 6865 6c6c 948c 0978 6d6c 3a73 7061  .shell...xml:spa
-000004b0: 6365 948c 0870 7265 7365 7276 6594 7568  ce...preserve.uh
-000004c0: 2b68 6268 1d68 2c68 1e4b 0468 1b68 2d68  +hbh.h,h.K.h.h-h
-000004d0: 1c68 0375 6268 3f29 8194 7d94 2868 058c  .h.ubh?)..}.(h..
-000004e0: aa49 6620 796f 7520 6861 7665 206d 756c  .If you have mul
-000004f0: 7469 706c 6520 696e 7374 616e 6365 7320  tiple instances 
-00000500: 6f66 2050 7974 686f 6e20 696e 7374 616c  of Python instal
-00000510: 6c65 642c 2072 756e 2074 6869 7320 636f  led, run this co
-00000520: 6d6d 616e 6420 7769 7468 2074 6865 2063  mmand with the c
-00000530: 686f 7365 6e20 5079 7468 6f6e 2069 6e74  hosen Python int
-00000540: 6572 7072 6574 6572 2074 6f20 696e 7374  erpreter to inst
-00000550: 616c 6c20 606d 7a64 6174 6132 6d61 7460  all `mzdata2mat`
-00000560: 2069 6e20 7468 6520 636f 7272 6573 706f   in the correspo
-00000570: 6e64 696e 6720 5079 7468 6f6e 2069 6e73  nding Python ins
-00000580: 7461 6c6c 6174 696f 6e20 3a94 6807 5d94  tallation :.h.].
-00000590: 2868 168c 7349 6620 796f 7520 6861 7665  (h..sIf you have
-000005a0: 206d 756c 7469 706c 6520 696e 7374 616e   multiple instan
-000005b0: 6365 7320 6f66 2050 7974 686f 6e20 696e  ces of Python in
-000005c0: 7374 616c 6c65 642c 2072 756e 2074 6869  stalled, run thi
-000005d0: 7320 636f 6d6d 616e 6420 7769 7468 2074  s command with t
-000005e0: 6865 2063 686f 7365 6e20 5079 7468 6f6e  he chosen Python
-000005f0: 2069 6e74 6572 7072 6574 6572 2074 6f20   interpreter to 
-00000600: 696e 7374 616c 6c20 9485 9481 947d 9428  install .....}.(
-00000610: 681b 6876 681c 6803 681d 4e68 1e4e 7562  h.hvh.h.h.Nh.Nub
-00000620: 6849 2981 947d 9428 6805 8c0a 6d7a 6461  hI)..}.(h...mzda
-00000630: 7461 326d 6174 9468 075d 9468 168c 0a6d  ta2mat.h.].h...m
-00000640: 7a64 6174 6132 6d61 7494 8594 8194 7d94  zdata2mat.....}.
-00000650: 2868 1b68 7e68 1c68 0368 1d4e 681e 4e75  (h.h~h.h.h.Nh.Nu
-00000660: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000670: 255d 9468 275d 9468 295d 9475 682b 6848  %].h'].h)].uh+hH
-00000680: 681e 4b07 681d 682c 681b 6876 681c 6803  h.K.h.h,h.hvh.h.
-00000690: 7562 6816 8c2b 2069 6e20 7468 6520 636f  ubh..+ in the co
-000006a0: 7272 6573 706f 6e64 696e 6720 5079 7468  rresponding Pyth
-000006b0: 6f6e 2069 6e73 7461 6c6c 6174 696f 6e20  on installation 
-000006c0: 3a94 8594 8194 7d94 2868 1b68 7668 1c68  :.....}.(h.hvh.h
-000006d0: 0368 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
-000006e0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000006f0: 295d 9475 682b 683e 681e 4b07 681d 682c  )].uh+h>h.K.h.h,
-00000700: 681b 682d 681c 6803 7562 6863 2981 947d  h.h-h.h.ubhc)..}
-00000710: 9428 6805 8c2e 2420 3c70 6174 6854 6f50  .(h...$ <pathToP
-00000720: 7974 686f 6e41 7070 3e20 2d6d 2070 6970  ythonApp> -m pip
-00000730: 2069 6e73 7461 6c6c 206d 7a64 6174 6132   install mzdata2
-00000740: 6d61 740a 9468 075d 9468 168c 2e24 203c  mat..h.].h...$ <
-00000750: 7061 7468 546f 5079 7468 6f6e 4170 703e  pathToPythonApp>
-00000760: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
-00000770: 6d7a 6461 7461 326d 6174 0a94 8594 8194  mzdata2mat......
-00000780: 7d94 681b 6896 7362 6168 1f7d 9428 6821  }.h.h.sbah.}.(h!
-00000790: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-000007a0: 5d94 8c08 6c61 6e67 7561 6765 948c 0573  ]...language...s
-000007b0: 6865 6c6c 9468 7468 7575 682b 6862 681d  hell.hthuuh+hbh.
-000007c0: 682c 681e 4b08 681b 682d 681c 6803 7562  h,h.K.h.h-h.h.ub
-000007d0: 683f 2981 947d 9428 6805 8c49 5768 656e  h?)..}.(h..IWhen
-000007e0: 2074 6865 2063 6f6d 6d61 6e64 2074 6572   the command ter
-000007f0: 6d69 6e61 7465 732c 2079 6f75 2068 6176  minates, you hav
-00000800: 6520 7375 6363 6573 7366 756c 6c79 2069  e successfully i
-00000810: 6e73 7461 6c6c 6564 206d 7a64 6174 6132  nstalled mzdata2
-00000820: 6d61 7420 2194 6807 5d94 6816 8c49 5768  mat !.h.].h..IWh
-00000830: 656e 2074 6865 2063 6f6d 6d61 6e64 2074  en the command t
-00000840: 6572 6d69 6e61 7465 732c 2079 6f75 2068  erminates, you h
-00000850: 6176 6520 7375 6363 6573 7366 756c 6c79  ave successfully
-00000860: 2069 6e73 7461 6c6c 6564 206d 7a64 6174   installed mzdat
-00000870: 6132 6d61 7420 2194 8594 8194 7d94 2868  a2mat !.....}.(h
-00000880: 1b68 a668 1c68 0368 1d4e 681e 4e75 6261  .h.h.h.h.Nh.Nuba
-00000890: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-000008a0: 9468 275d 9468 295d 9475 682b 683e 681e  .h'].h)].uh+h>h.
-000008b0: 4b0b 681d 682c 681b 682d 681c 6803 7562  K.h.h,h.h-h.h.ub
-000008c0: 6568 1f7d 9428 6821 5d94 8c07 636f 6d6d  eh.}.(h!]...comm
-000008d0: 616e 6494 6168 235d 9468 255d 948c 0763  and.ah#].h%]...c
-000008e0: 6f6d 6d61 6e64 9461 6827 5d94 6829 5d94  ommand.ah'].h)].
-000008f0: 7568 2b68 0a68 1e4b 0268 1d68 2c68 1b68  uh+h.h.K.h.h,h.h
-00000900: 0c68 1c68 0375 6268 0b29 8194 7d94 2868  .h.h.ubh.)..}.(h
-00000910: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
-00000920: 6805 8c17 5665 7269 6679 2074 6865 2069  h...Verify the i
-00000930: 6e73 7461 6c6c 6174 696f 6e94 6807 5d94  nstallation.h.].
-00000940: 6816 8c17 5665 7269 6679 2074 6865 2069  h...Verify the i
-00000950: 6e73 7461 6c6c 6174 696f 6e94 8594 8194  nstallation.....
-00000960: 7d94 2868 1b68 bf68 1c68 0368 1d4e 681e  }.(h.h.h.h.h.Nh.
-00000970: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00000980: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00000990: 680f 681e 4b0d 681d 682c 681b 68bc 681c  h.h.K.h.h,h.h.h.
-000009a0: 6803 7562 683f 2981 947d 9428 6805 8c51  h.ubh?)..}.(h..Q
-000009b0: 546f 2076 6572 6669 7920 6966 2074 6865  To verfiy if the
-000009c0: 2069 6e73 7461 6c6c 6174 696f 6e20 7761   installation wa
-000009d0: 7320 7375 6363 6573 7366 756c 2c20 7275  s successful, ru
-000009e0: 6e20 696e 2079 6f75 7220 7465 726d 696e  n in your termin
-000009f0: 616c 2074 6869 7320 636f 6d6d 616e 6420  al this command 
-00000a00: 3a94 6807 5d94 6816 8c51 546f 2076 6572  :.h.].h..QTo ver
-00000a10: 6669 7920 6966 2074 6865 2069 6e73 7461  fiy if the insta
-00000a20: 6c6c 6174 696f 6e20 7761 7320 7375 6363  llation was succ
-00000a30: 6573 7366 756c 2c20 7275 6e20 696e 2079  essful, run in y
-00000a40: 6f75 7220 7465 726d 696e 616c 2074 6869  our terminal thi
-00000a50: 7320 636f 6d6d 616e 6420 3a94 8594 8194  s command :.....
-00000a60: 7d94 2868 1b68 cd68 1c68 0368 1d4e 681e  }.(h.h.h.h.h.Nh.
-00000a70: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00000a80: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00000a90: 683e 681e 4b0e 681d 682c 681b 68bc 681c  h>h.K.h.h,h.h.h.
-00000aa0: 6803 7562 6863 2981 947d 9428 6805 8c14  h.ubhc)..}.(h...
-00000ab0: 2420 6d7a 6461 7461 326d 6174 2d76 6572  $ mzdata2mat-ver
-00000ac0: 6966 790a 9468 075d 9468 168c 1424 206d  ify..h.].h...$ m
-00000ad0: 7a64 6174 6132 6d61 742d 7665 7269 6679  zdata2mat-verify
-00000ae0: 0a94 8594 8194 7d94 681b 68db 7362 6168  ......}.h.h.sbah
-00000af0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00000b00: 6827 5d94 6829 5d94 8c08 6c61 6e67 7561  h'].h)]...langua
-00000b10: 6765 948c 0573 6865 6c6c 9468 7468 7575  ge...shell.hthuu
-00000b20: 682b 6862 681d 682c 681e 4b0f 681b 68bc  h+hbh.h,h.K.h.h.
-00000b30: 681c 6803 7562 683f 2981 947d 9428 6805  h.h.ubh?)..}.(h.
-00000b40: 8cde 5768 656e 2079 6f75 2077 696c 6c20  ..When you will 
-00000b50: 6669 7273 7420 7275 6e20 7468 6973 2063  first run this c
-00000b60: 6f6d 6d61 6e64 2c20 6e6f 6465 2e6a 7320  ommand, node.js 
-00000b70: 7769 6c6c 2064 6f77 6e6c 6f61 6420 616e  will download an
-00000b80: 6420 696e 7374 616c 6c20 7468 6520 606d  d install the `m
-00000b90: 7a64 6174 6160 2070 6163 6b61 6765 2066  zdata` package f
-00000ba0: 726f 6d20 606e 706d 602e 2054 6869 7320  rom `npm`. This 
-00000bb0: 7769 6c6c 206f 6e6c 7920 6861 7070 656e  will only happen
-00000bc0: 2074 6865 2066 6972 7374 2074 696d 6520   the first time 
-00000bd0: 796f 7520 7275 6e20 7468 6520 636f 6d6d  you run the comm
-00000be0: 616e 642e 2054 6865 2074 6572 6d69 6e61  and. The termina
-00000bf0: 6c20 7769 6c6c 2073 686f 7720 796f 7520  l will show you 
-00000c00: 7468 6573 6520 6c69 6e65 7320 6475 7269  these lines duri
-00000c10: 6e67 2074 6865 2070 726f 6365 7373 203a  ng the process :
-00000c20: 9468 075d 9428 6816 8c4c 5768 656e 2079  .h.].(h..LWhen y
-00000c30: 6f75 2077 696c 6c20 6669 7273 7420 7275  ou will first ru
-00000c40: 6e20 7468 6973 2063 6f6d 6d61 6e64 2c20  n this command, 
-00000c50: 6e6f 6465 2e6a 7320 7769 6c6c 2064 6f77  node.js will dow
-00000c60: 6e6c 6f61 6420 616e 6420 696e 7374 616c  nload and instal
-00000c70: 6c20 7468 6520 9485 9481 947d 9428 681b  l the .....}.(h.
-00000c80: 68eb 681c 6803 681d 4e68 1e4e 7562 6849  h.h.h.h.Nh.NubhI
-00000c90: 2981 947d 9428 6805 8c06 6d7a 6461 7461  )..}.(h...mzdata
-00000ca0: 9468 075d 9468 168c 066d 7a64 6174 6194  .h.].h...mzdata.
-00000cb0: 8594 8194 7d94 2868 1b68 f368 1c68 0368  ....}.(h.h.h.h.h
-00000cc0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00000cd0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00000ce0: 9475 682b 6848 681e 4b12 681d 682c 681b  .uh+hHh.K.h.h,h.
-00000cf0: 68eb 681c 6803 7562 6816 8c0e 2070 6163  h.h.h.ubh... pac
-00000d00: 6b61 6765 2066 726f 6d20 9485 9481 947d  kage from .....}
-00000d10: 9428 681b 68eb 681c 6803 681d 4e68 1e4e  .(h.h.h.h.h.Nh.N
-00000d20: 7562 6849 2981 947d 9428 6805 8c03 6e70  ubhI)..}.(h...np
-00000d30: 6d94 6807 5d94 6816 8c03 6e70 6d94 8594  m.h.].h...npm...
-00000d40: 8194 7d94 2868 1b6a 0501 0000 681c 6803  ..}.(h.j....h.h.
-00000d50: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00000d60: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00000d70: 5d94 7568 2b68 4868 1e4b 1268 1d68 2c68  ].uh+hHh.K.h.h,h
-00000d80: 1b68 eb68 1c68 0375 6268 168c 772e 2054  .h.h.h.ubh..w. T
-00000d90: 6869 7320 7769 6c6c 206f 6e6c 7920 6861  his will only ha
-00000da0: 7070 656e 2074 6865 2066 6972 7374 2074  ppen the first t
-00000db0: 696d 6520 796f 7520 7275 6e20 7468 6520  ime you run the 
-00000dc0: 636f 6d6d 616e 642e 2054 6865 2074 6572  command. The ter
-00000dd0: 6d69 6e61 6c20 7769 6c6c 2073 686f 7720  minal will show 
-00000de0: 796f 7520 7468 6573 6520 6c69 6e65 7320  you these lines 
-00000df0: 6475 7269 6e67 2074 6865 2070 726f 6365  during the proce
-00000e00: 7373 203a 9485 9481 947d 9428 681b 68eb  ss :.....}.(h.h.
-00000e10: 681c 6803 681d 4e68 1e4e 7562 6568 1f7d  h.h.h.Nh.Nubeh.}
-00000e20: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00000e30: 5d94 6829 5d94 7568 2b68 3e68 1e4b 1268  ].h)].uh+h>h.K.h
-00000e40: 1d68 2c68 1b68 bc68 1c68 0375 6268 6329  .h,h.h.h.h.ubhc)
-00000e50: 8194 7d94 2868 058c e420 496e 7374 616c  ..}.(h... Instal
-00000e60: 6c69 6e67 2027 6d7a 6461 7461 2720 7665  ling 'mzdata' ve
-00000e70: 7273 696f 6e20 276c 6174 6573 7427 2e2e  rsion 'latest'..
-00000e80: 2e20 5468 6973 2077 696c 6c20 6f6e 6c79  . This will only
-00000e90: 2068 6170 7065 6e20 6f6e 6365 2e20 0a0a   happen once. ..
-00000ea0: 6164 6465 6420 3720 7061 636b 6167 6573  added 7 packages
-00000eb0: 2c20 616e 6420 6175 6469 7465 6420 3820  , and audited 8 
-00000ec0: 7061 636b 6167 6573 2069 6e20 3273 0a0a  packages in 2s..
-00000ed0: 3120 7061 636b 6167 6520 6973 206c 6f6f  1 package is loo
-00000ee0: 6b69 6e67 2066 6f72 2066 756e 6469 6e67  king for funding
-00000ef0: 0a20 2072 756e 2060 6e70 6d20 6675 6e64  .  run `npm fund
-00000f00: 6020 666f 7220 6465 7461 696c 730a 0a66  ` for details..f
-00000f10: 6f75 6e64 2030 2076 756c 6e65 7261 6269  ound 0 vulnerabi
-00000f20: 6c69 7469 6573 0a0a 204f 4b2e 200a 5b4a  lities.. OK. .[J
-00000f30: 5345 5d20 0a0a 5b4a 5345 5d20 0a94 6807  SE] ..[JSE] ..h.
-00000f40: 5d94 6816 8ce4 2049 6e73 7461 6c6c 696e  ].h... Installin
-00000f50: 6720 276d 7a64 6174 6127 2076 6572 7369  g 'mzdata' versi
-00000f60: 6f6e 2027 6c61 7465 7374 272e 2e2e 2054  on 'latest'... T
-00000f70: 6869 7320 7769 6c6c 206f 6e6c 7920 6861  his will only ha
-00000f80: 7070 656e 206f 6e63 652e 200a 0a61 6464  ppen once. ..add
-00000f90: 6564 2037 2070 6163 6b61 6765 732c 2061  ed 7 packages, a
-00000fa0: 6e64 2061 7564 6974 6564 2038 2070 6163  nd audited 8 pac
-00000fb0: 6b61 6765 7320 696e 2032 730a 0a31 2070  kages in 2s..1 p
-00000fc0: 6163 6b61 6765 2069 7320 6c6f 6f6b 696e  ackage is lookin
-00000fd0: 6720 666f 7220 6675 6e64 696e 670a 2020  g for funding.  
-00000fe0: 7275 6e20 606e 706d 2066 756e 6460 2066  run `npm fund` f
-00000ff0: 6f72 2064 6574 6169 6c73 0a0a 666f 756e  or details..foun
-00001000: 6420 3020 7675 6c6e 6572 6162 696c 6974  d 0 vulnerabilit
-00001010: 6965 730a 0a20 4f4b 2e20 0a5b 4a53 455d  ies.. OK. .[JSE]
-00001020: 200a 0a5b 4a53 455d 200a 9485 9481 947d   ..[JSE] ......}
-00001030: 9468 1b6a 1d01 0000 7362 6168 1f7d 9428  .h.j....sbah.}.(
-00001040: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00001050: 6829 5d94 8c08 6c61 6e67 7561 6765 948c  h)]...language..
-00001060: 0573 6865 6c6c 9468 7468 7575 682b 6862  .shell.hthuuh+hb
-00001070: 681d 682c 681e 4b13 681b 68bc 681c 6803  h.h,h.K.h.h.h.h.
-00001080: 7562 683f 2981 947d 9428 6805 8ca8 5768  ubh?)..}.(h...Wh
-00001090: 656e 2069 7427 7320 646f 6e65 2c20 7468  en it's done, th
-000010a0: 6520 606d 7a64 6174 6132 6d61 7460 2070  e `mzdata2mat` p
-000010b0: 6163 6b61 6765 2077 696c 6c20 6174 7465  ackage will atte
-000010c0: 6d70 7420 746f 2063 6f6e 7665 7274 2061  mpt to convert a
-000010d0: 6e20 6578 616d 706c 6520 602e 6d7a 6461  n example `.mzda
-000010e0: 7461 2e78 6d6c 6020 6669 6c65 2069 6e74  ta.xml` file int
-000010f0: 6f20 6120 602e 6d61 7460 2066 696c 652e  o a `.mat` file.
-00001100: 2049 6620 6576 6572 7974 6869 6e67 2067   If everything g
-00001110: 6f65 7320 7269 6768 742c 2079 6f75 2077  oes right, you w
-00001120: 696c 6c20 6765 7420 7468 6973 206d 6573  ill get this mes
-00001130: 7361 6765 203a 9468 075d 9428 6816 8c16  sage :.h.].(h...
-00001140: 5768 656e 2069 74e2 8099 7320 646f 6e65  When it...s done
-00001150: 2c20 7468 6520 9485 9481 947d 9428 681b  , the .....}.(h.
-00001160: 6a2d 0100 0068 1c68 0368 1d4e 681e 4e75  j-...h.h.h.Nh.Nu
-00001170: 6268 4929 8194 7d94 2868 058c 0a6d 7a64  bhI)..}.(h...mzd
-00001180: 6174 6132 6d61 7494 6807 5d94 6816 8c0a  ata2mat.h.].h...
-00001190: 6d7a 6461 7461 326d 6174 9485 9481 947d  mzdata2mat.....}
-000011a0: 9428 681b 6a35 0100 0068 1c68 0368 1d4e  .(h.j5...h.h.h.N
-000011b0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-000011c0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-000011d0: 682b 6848 681e 4b22 681d 682c 681b 6a2d  h+hHh.K"h.h,h.j-
-000011e0: 0100 0068 1c68 0375 6268 168c 2c20 7061  ...h.h.ubh.., pa
-000011f0: 636b 6167 6520 7769 6c6c 2061 7474 656d  ckage will attem
-00001200: 7074 2074 6f20 636f 6e76 6572 7420 616e  pt to convert an
-00001210: 2065 7861 6d70 6c65 2094 8594 8194 7d94   example .....}.
-00001220: 2868 1b6a 2d01 0000 681c 6803 681d 4e68  (h.j-...h.h.h.Nh
-00001230: 1e4e 7562 6849 2981 947d 9428 6805 8c0b  .NubhI)..}.(h...
-00001240: 2e6d 7a64 6174 612e 786d 6c94 6807 5d94  .mzdata.xml.h.].
-00001250: 6816 8c0b 2e6d 7a64 6174 612e 786d 6c94  h....mzdata.xml.
-00001260: 8594 8194 7d94 2868 1b6a 4701 0000 681c  ....}.(h.jG...h.
-00001270: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00001280: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00001290: 6829 5d94 7568 2b68 4868 1e4b 2268 1d68  h)].uh+hHh.K"h.h
-000012a0: 2c68 1b6a 2d01 0000 681c 6803 7562 6816  ,h.j-...h.h.ubh.
-000012b0: 8c0d 2066 696c 6520 696e 746f 2061 2094  .. file into a .
-000012c0: 8594 8194 7d94 2868 1b6a 2d01 0000 681c  ....}.(h.j-...h.
-000012d0: 6803 681d 4e68 1e4e 7562 6849 2981 947d  h.h.Nh.NubhI)..}
-000012e0: 9428 6805 8c04 2e6d 6174 9468 075d 9468  .(h....mat.h.].h
-000012f0: 168c 042e 6d61 7494 8594 8194 7d94 2868  ....mat.....}.(h
-00001300: 1b6a 5901 0000 681c 6803 681d 4e68 1e4e  .jY...h.h.h.Nh.N
-00001310: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00001320: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-00001330: 4868 1e4b 2268 1d68 2c68 1b6a 2d01 0000  Hh.K"h.h,h.j-...
-00001340: 681c 6803 7562 6816 8c3c 2066 696c 652e  h.h.ubh..< file.
-00001350: 2049 6620 6576 6572 7974 6869 6e67 2067   If everything g
-00001360: 6f65 7320 7269 6768 742c 2079 6f75 2077  oes right, you w
-00001370: 696c 6c20 6765 7420 7468 6973 206d 6573  ill get this mes
-00001380: 7361 6765 203a 9485 9481 947d 9428 681b  sage :.....}.(h.
-00001390: 6a2d 0100 0068 1c68 0368 1d4e 681e 4e75  j-...h.h.h.Nh.Nu
-000013a0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-000013b0: 255d 9468 275d 9468 295d 9475 682b 683e  %].h'].h)].uh+h>
-000013c0: 681e 4b22 681d 682c 681b 68bc 681c 6803  h.K"h.h,h.h.h.h.
-000013d0: 7562 6863 2981 947d 9428 6805 8c1e 2420  ubhc)..}.(h...$ 
-000013e0: 6d7a 6461 7461 326d 6174 202d 2052 6561  mzdata2mat - Rea
-000013f0: 6479 2074 6f20 7573 6520 210a 9468 075d  dy to use !..h.]
-00001400: 9468 168c 1e24 206d 7a64 6174 6132 6d61  .h...$ mzdata2ma
-00001410: 7420 2d20 5265 6164 7920 746f 2075 7365  t - Ready to use
-00001420: 2021 0a94 8594 8194 7d94 681b 6a71 0100   !......}.h.jq..
-00001430: 0073 6261 681f 7d94 2868 215d 9468 235d  .sbah.}.(h!].h#]
-00001440: 9468 255d 9468 275d 9468 295d 948c 086c  .h%].h'].h)]...l
-00001450: 616e 6775 6167 6594 8c05 7368 656c 6c94  anguage...shell.
-00001460: 6874 6875 7568 2b68 6268 1d68 2c68 1e4b  hthuuh+hbh.h,h.K
-00001470: 2368 1b68 bc68 1c68 0375 6268 3f29 8194  #h.h.h.h.ubh?)..
-00001480: 7d94 2868 058c 9e54 6865 2065 7861 6d70  }.(h...The examp
-00001490: 6c65 2066 696c 6520 282e 6d7a 6461 7461  le file (.mzdata
-000014a0: 2e78 6d6c 2920 7769 6c6c 2062 6520 636f  .xml) will be co
-000014b0: 7069 6564 2069 6e20 7468 6520 6375 7272  pied in the curr
-000014c0: 656e 7420 776f 726b 696e 6720 6469 7265  ent working dire
-000014d0: 6374 6f72 7920 616e 6420 7468 6520 636f  ctory and the co
-000014e0: 6e76 6572 7465 6420 6669 6c65 2028 2e6d  nverted file (.m
-000014f0: 6174 2920 7769 6c6c 2062 6520 6164 6465  at) will be adde
-00001500: 6420 6173 2073 6f6f 6e20 6173 2074 6865  d as soon as the
-00001510: 2063 6f6e 7665 7273 696f 6e20 6669 6e69   conversion fini
-00001520: 7368 6573 2e94 6807 5d94 6816 8c9e 5468  shes..h.].h...Th
-00001530: 6520 6578 616d 706c 6520 6669 6c65 2028  e example file (
-00001540: 2e6d 7a64 6174 612e 786d 6c29 2077 696c  .mzdata.xml) wil
-00001550: 6c20 6265 2063 6f70 6965 6420 696e 2074  l be copied in t
-00001560: 6865 2063 7572 7265 6e74 2077 6f72 6b69  he current worki
-00001570: 6e67 2064 6972 6563 746f 7279 2061 6e64  ng directory and
-00001580: 2074 6865 2063 6f6e 7665 7274 6564 2066   the converted f
-00001590: 696c 6520 282e 6d61 7429 2077 696c 6c20  ile (.mat) will 
-000015a0: 6265 2061 6464 6564 2061 7320 736f 6f6e  be added as soon
-000015b0: 2061 7320 7468 6520 636f 6e76 6572 7369   as the conversi
-000015c0: 6f6e 2066 696e 6973 6865 732e 9485 9481  on finishes.....
-000015d0: 947d 9428 681b 6a81 0100 0068 1c68 0368  .}.(h.j....h.h.h
-000015e0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000015f0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001600: 9475 682b 683e 681e 4b26 681d 682c 681b  .uh+h>h.K&h.h,h.
-00001610: 68bc 681c 6803 7562 6568 1f7d 9428 6821  h.h.h.ubeh.}.(h!
-00001620: 5d94 8c17 7665 7269 6679 2d74 6865 2d69  ]...verify-the-i
-00001630: 6e73 7461 6c6c 6174 696f 6e94 6168 235d  nstallation.ah#]
-00001640: 9468 255d 948c 1776 6572 6966 7920 7468  .h%]...verify th
-00001650: 6520 696e 7374 616c 6c61 7469 6f6e 9461  e installation.a
-00001660: 6827 5d94 6829 5d94 7568 2b68 0a68 1e4b  h'].h)].uh+h.h.K
-00001670: 0d68 1d68 2c68 1b68 0c68 1c68 0375 6268  .h.h,h.h.h.h.ubh
-00001680: 0b29 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
-00001690: 6810 2981 947d 9428 6805 8c10 5472 6f75  h.)..}.(h...Trou
-000016a0: 6262 6c65 7368 6f6f 7469 6e67 9468 075d  bbleshooting.h.]
-000016b0: 9468 168c 1054 726f 7562 626c 6573 686f  .h...Troubblesho
-000016c0: 6f74 696e 6794 8594 8194 7d94 2868 1b6a  oting.....}.(h.j
-000016d0: 9a01 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-000016e0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-000016f0: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
-00001700: 1e4b 2868 1d68 2c68 1b6a 9701 0000 681c  .K(h.h,h.j....h.
-00001710: 6803 7562 683f 2981 947d 9428 6805 8c85  h.ubh?)..}.(h...
-00001720: 4966 2061 6e20 6572 726f 7220 6f63 6375  If an error occu
-00001730: 7273 2c20 7468 6973 2070 726f 6261 626c  rs, this probabl
-00001740: 7920 6d65 616e 7320 7468 6174 2079 6f75  y means that you
-00001750: 2064 6f20 6e6f 7420 6861 7665 205f 5f6e   do not have __n
-00001760: 6f64 652e 6a73 5f5f 2069 6e73 7461 6c6c  ode.js__ install
-00001770: 6564 206f 6e20 796f 7572 206d 6163 6869  ed on your machi
-00001780: 6e65 206f 7220 796f 7520 6469 646e 2774  ne or you didn't
-00001790: 2061 6464 2069 7420 746f 2079 6f75 7220   add it to your 
-000017a0: 5041 5448 2e94 6807 5d94 2868 168c 3d49  PATH..h.].(h..=I
-000017b0: 6620 616e 2065 7272 6f72 206f 6363 7572  f an error occur
-000017c0: 732c 2074 6869 7320 7072 6f62 6162 6c79  s, this probably
-000017d0: 206d 6561 6e73 2074 6861 7420 796f 7520   means that you 
-000017e0: 646f 206e 6f74 2068 6176 6520 9485 9481  do not have ....
-000017f0: 947d 9428 681b 6aa8 0100 0068 1c68 0368  .}.(h.j....h.h.h
-00001800: 1d4e 681e 4e75 6268 098c 0673 7472 6f6e  .Nh.Nubh...stron
-00001810: 6794 9394 2981 947d 9428 6805 8c07 6e6f  g...)..}.(h...no
-00001820: 6465 2e6a 7394 6807 5d94 6816 8c07 6e6f  de.js.h.].h...no
-00001830: 6465 2e6a 7394 8594 8194 7d94 2868 1b6a  de.js.....}.(h.j
-00001840: b201 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00001850: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00001860: 5d94 6827 5d94 6829 5d94 7568 2b6a b001  ].h'].h)].uh+j..
-00001870: 0000 681e 4b29 681d 682c 681b 6aa8 0100  ..h.K)h.h,h.j...
-00001880: 0068 1c68 0375 6268 168c 3f20 696e 7374  .h.h.ubh..? inst
-00001890: 616c 6c65 6420 6f6e 2079 6f75 7220 6d61  alled on your ma
-000018a0: 6368 696e 6520 6f72 2079 6f75 2064 6964  chine or you did
-000018b0: 6ee2 8099 7420 6164 6420 6974 2074 6f20  n...t add it to 
-000018c0: 796f 7572 2050 4154 482e 9485 9481 947d  your PATH......}
-000018d0: 9428 681b 6aa8 0100 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-000018e0: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
-000018f0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00001900: 682b 683e 681e 4b29 681d 682c 681b 6a97  h+h>h.K)h.h,h.j.
-00001910: 0100 0068 1c68 0375 6265 681f 7d94 2868  ...h.h.ubeh.}.(h
-00001920: 215d 948c 1074 726f 7562 626c 6573 686f  !]...troubblesho
-00001930: 6f74 696e 6794 6168 235d 9468 255d 948c  oting.ah#].h%]..
-00001940: 1074 726f 7562 626c 6573 686f 6f74 696e  .troubbleshootin
-00001950: 6794 6168 275d 9468 295d 9475 682b 680a  g.ah'].h)].uh+h.
-00001960: 681e 4b28 681d 682c 681b 680c 681c 6803  h.K(h.h,h.h.h.h.
-00001970: 7562 6568 1f7d 9428 6821 5d94 8c0c 696e  ubeh.}.(h!]...in
-00001980: 7374 616c 6c61 7469 6f6e 9461 6823 5d94  stallation.ah#].
-00001990: 6825 5d94 8c0c 696e 7374 616c 6c61 7469  h%]...installati
-000019a0: 6f6e 9461 6827 5d94 6829 5d94 7568 2b68  on.ah'].h)].uh+h
-000019b0: 0a68 1e4b 0168 1d68 2c68 1b68 0368 1c68  .h.K.h.h,h.h.h.h
-000019c0: 0375 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
-000019d0: 9468 255d 9468 275d 9468 295d 948c 0673  .h%].h'].h)]...s
-000019e0: 6f75 7263 6594 682c 8c14 7472 616e 736c  ource.h,..transl
-000019f0: 6174 696f 6e5f 7072 6f67 7265 7373 947d  ation_progress.}
-00001a00: 9428 8c05 746f 7461 6c94 4b00 8c0a 7472  .(..total.K...tr
-00001a10: 616e 736c 6174 6564 944b 0075 7568 2b68  anslated.K.uuh+h
-00001a20: 018c 0e63 7572 7265 6e74 5f73 6f75 7263  ...current_sourc
-00001a30: 6594 4e8c 0c63 7572 7265 6e74 5f6c 696e  e.N..current_lin
-00001a40: 6594 4e8c 0873 6574 7469 6e67 7394 8c11  e.N..settings...
-00001a50: 646f 6375 7469 6c73 2e66 726f 6e74 656e  docutils.fronten
-00001a60: 6494 8c06 5661 6c75 6573 9493 9429 8194  d...Values...)..
-00001a70: 7d94 2868 0f4e 8c09 6765 6e65 7261 746f  }.(h.N..generato
-00001a80: 7294 4e8c 0964 6174 6573 7461 6d70 944e  r.N..datestamp.N
-00001a90: 8c0b 736f 7572 6365 5f6c 696e 6b94 4e8c  ..source_link.N.
-00001aa0: 0a73 6f75 7263 655f 7572 6c94 4e8c 0d74  .source_url.N..t
-00001ab0: 6f63 5f62 6163 6b6c 696e 6b73 948c 0565  oc_backlinks...e
-00001ac0: 6e74 7279 948c 1266 6f6f 746e 6f74 655f  ntry...footnote_
-00001ad0: 6261 636b 6c69 6e6b 7394 4b01 8c0d 7365  backlinks.K...se
-00001ae0: 6374 6e75 6d5f 7866 6f72 6d94 4b01 8c0e  ctnum_xform.K...
-00001af0: 7374 7269 705f 636f 6d6d 656e 7473 944e  strip_comments.N
-00001b00: 8c1b 7374 7269 705f 656c 656d 656e 7473  ..strip_elements
-00001b10: 5f77 6974 685f 636c 6173 7365 7394 4e8c  _with_classes.N.
-00001b20: 0d73 7472 6970 5f63 6c61 7373 6573 944e  .strip_classes.N
-00001b30: 8c0c 7265 706f 7274 5f6c 6576 656c 944b  ..report_level.K
-00001b40: 028c 0a68 616c 745f 6c65 7665 6c94 4b05  ...halt_level.K.
-00001b50: 8c11 6578 6974 5f73 7461 7475 735f 6c65  ..exit_status_le
-00001b60: 7665 6c94 4b05 8c05 6465 6275 6794 4e8c  vel.K...debug.N.
-00001b70: 0e77 6172 6e69 6e67 5f73 7472 6561 6d94  .warning_stream.
-00001b80: 4e8c 0974 7261 6365 6261 636b 9488 8c0e  N..traceback....
-00001b90: 696e 7075 745f 656e 636f 6469 6e67 948c  input_encoding..
-00001ba0: 0975 7466 2d38 2d73 6967 948c 1c69 6e70  .utf-8-sig...inp
-00001bb0: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
-00001bc0: 725f 6861 6e64 6c65 7294 8c06 7374 7269  r_handler...stri
-00001bd0: 6374 948c 0f6f 7574 7075 745f 656e 636f  ct...output_enco
-00001be0: 6469 6e67 948c 0575 7466 2d38 948c 1d6f  ding...utf-8...o
-00001bf0: 7574 7075 745f 656e 636f 6469 6e67 5f65  utput_encoding_e
-00001c00: 7272 6f72 5f68 616e 646c 6572 946a 0102  rror_handler.j..
-00001c10: 0000 8c0e 6572 726f 725f 656e 636f 6469  ....error_encodi
-00001c20: 6e67 948c 0575 7466 2d38 948c 1c65 7272  ng...utf-8...err
-00001c30: 6f72 5f65 6e63 6f64 696e 675f 6572 726f  or_encoding_erro
-00001c40: 725f 6861 6e64 6c65 7294 8c10 6261 636b  r_handler...back
-00001c50: 736c 6173 6872 6570 6c61 6365 948c 0d6c  slashreplace...l
-00001c60: 616e 6775 6167 655f 636f 6465 948c 0265  anguage_code...e
-00001c70: 6e94 8c13 7265 636f 7264 5f64 6570 656e  n...record_depen
-00001c80: 6465 6e63 6965 7394 4e8c 0663 6f6e 6669  dencies.N..confi
-00001c90: 6794 4e8c 0969 645f 7072 6566 6978 9468  g.N..id_prefix.h
-00001ca0: 068c 0e61 7574 6f5f 6964 5f70 7265 6669  ...auto_id_prefi
-00001cb0: 7894 8c02 6964 948c 0d64 756d 705f 7365  x...id...dump_se
-00001cc0: 7474 696e 6773 944e 8c0e 6475 6d70 5f69  ttings.N..dump_i
-00001cd0: 6e74 6572 6e61 6c73 944e 8c0f 6475 6d70  nternals.N..dump
-00001ce0: 5f74 7261 6e73 666f 726d 7394 4e8c 0f64  _transforms.N..d
-00001cf0: 756d 705f 7073 6575 646f 5f78 6d6c 944e  ump_pseudo_xml.N
-00001d00: 8c10 6578 706f 7365 5f69 6e74 6572 6e61  ..expose_interna
-00001d10: 6c73 944e 8c0e 7374 7269 6374 5f76 6973  ls.N..strict_vis
-00001d20: 6974 6f72 944e 8c0f 5f64 6973 6162 6c65  itor.N.._disable
-00001d30: 5f63 6f6e 6669 6794 4e8c 075f 736f 7572  _config.N.._sour
-00001d40: 6365 9468 2c8c 0c5f 6465 7374 696e 6174  ce.h,.._destinat
-00001d50: 696f 6e94 4e8c 0d5f 636f 6e66 6967 5f66  ion.N.._config_f
-00001d60: 696c 6573 945d 948c 1666 696c 655f 696e  iles.]...file_in
-00001d70: 7365 7274 696f 6e5f 656e 6162 6c65 6494  sertion_enabled.
-00001d80: 888c 0b72 6177 5f65 6e61 626c 6564 944b  ...raw_enabled.K
-00001d90: 018c 116c 696e 655f 6c65 6e67 7468 5f6c  ...line_length_l
-00001da0: 696d 6974 944d 1027 8c0e 7065 705f 7265  imit.M.'..pep_re
-00001db0: 6665 7265 6e63 6573 944e 8c0c 7065 705f  ferences.N..pep_
-00001dc0: 6261 7365 5f75 726c 948c 1868 7474 7073  base_url...https
-00001dd0: 3a2f 2f70 6570 732e 7079 7468 6f6e 2e6f  ://peps.python.o
-00001de0: 7267 2f94 8c15 7065 705f 6669 6c65 5f75  rg/...pep_file_u
-00001df0: 726c 5f74 656d 706c 6174 6594 8c08 7065  rl_template...pe
-00001e00: 702d 2530 3464 948c 0e72 6663 5f72 6566  p-%04d...rfc_ref
-00001e10: 6572 656e 6365 7394 4e8c 0c72 6663 5f62  erences.N..rfc_b
-00001e20: 6173 655f 7572 6c94 8c26 6874 7470 733a  ase_url..&https:
-00001e30: 2f2f 6461 7461 7472 6163 6b65 722e 6965  //datatracker.ie
-00001e40: 7466 2e6f 7267 2f64 6f63 2f68 746d 6c2f  tf.org/doc/html/
-00001e50: 948c 0974 6162 5f77 6964 7468 944b 088c  ...tab_width.K..
-00001e60: 1d74 7269 6d5f 666f 6f74 6e6f 7465 5f72  .trim_footnote_r
-00001e70: 6566 6572 656e 6365 5f73 7061 6365 9489  eference_space..
-00001e80: 8c10 7379 6e74 6178 5f68 6967 686c 6967  ..syntax_highlig
-00001e90: 6874 948c 046c 6f6e 6794 8c0c 736d 6172  ht...long...smar
-00001ea0: 745f 7175 6f74 6573 9488 8c13 736d 6172  t_quotes....smar
-00001eb0: 7471 756f 7465 735f 6c6f 6361 6c65 7394  tquotes_locales.
-00001ec0: 5d94 8c1d 6368 6172 6163 7465 725f 6c65  ]...character_le
-00001ed0: 7665 6c5f 696e 6c69 6e65 5f6d 6172 6b75  vel_inline_marku
-00001ee0: 7094 898c 0e64 6f63 7469 746c 655f 7866  p....doctitle_xf
-00001ef0: 6f72 6d94 898c 0d64 6f63 696e 666f 5f78  orm....docinfo_x
-00001f00: 666f 726d 944b 018c 1273 6563 7473 7562  form.K...sectsub
-00001f10: 7469 746c 655f 7866 6f72 6d94 898c 0d69  title_xform....i
-00001f20: 6d61 6765 5f6c 6f61 6469 6e67 948c 046c  mage_loading...l
-00001f30: 696e 6b94 8c10 656d 6265 645f 7374 796c  ink...embed_styl
-00001f40: 6573 6865 6574 9489 8c15 636c 6f61 6b5f  esheet....cloak_
-00001f50: 656d 6169 6c5f 6164 6472 6573 7365 7394  email_addresses.
-00001f60: 888c 1173 6563 7469 6f6e 5f73 656c 665f  ...section_self_
-00001f70: 6c69 6e6b 9489 8c03 656e 7694 4e75 628c  link....env.Nub.
-00001f80: 0872 6570 6f72 7465 7294 4e8c 1069 6e64  .reporter.N..ind
-00001f90: 6972 6563 745f 7461 7267 6574 7394 5d94  irect_targets.].
-00001fa0: 8c11 7375 6273 7469 7475 7469 6f6e 5f64  ..substitution_d
-00001fb0: 6566 7394 7d94 288c 0f77 6f72 6463 6f75  efs.}.(..wordcou
-00001fc0: 6e74 2d77 6f72 6473 9468 098c 1773 7562  nt-words.h...sub
-00001fd0: 7374 6974 7574 696f 6e5f 6465 6669 6e69  stitution_defini
-00001fe0: 7469 6f6e 9493 9429 8194 7d94 2868 058c  tion...)..}.(h..
-00001ff0: 0331 3639 9468 075d 9468 168c 0331 3639  .169.h.].h...169
-00002000: 9485 9481 947d 9468 1b6a 3f02 0000 7362  .....}.h.j?...sb
-00002010: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00002020: 5d94 8c0f 776f 7264 636f 756e 742d 776f  ]...wordcount-wo
-00002030: 7264 7394 6168 275d 9468 295d 9475 682b  rds.ah'].h)].uh+
-00002040: 6a3d 0200 0068 1d68 2c75 628c 1177 6f72  j=...h.h,ub..wor
-00002050: 6463 6f75 6e74 2d6d 696e 7574 6573 946a  dcount-minutes.j
-00002060: 3e02 0000 2981 947d 9428 6805 8c01 3194  >...)..}.(h...1.
-00002070: 6807 5d94 6816 8c01 3194 8594 8194 7d94  h.].h...1.....}.
-00002080: 681b 6a4f 0200 0073 6261 681f 7d94 2868  h.jO...sbah.}.(h
-00002090: 215d 9468 235d 9468 255d 948c 1177 6f72  !].h#].h%]...wor
-000020a0: 6463 6f75 6e74 2d6d 696e 7574 6573 9461  dcount-minutes.a
-000020b0: 6827 5d94 6829 5d94 7568 2b6a 3d02 0000  h'].h)].uh+j=...
-000020c0: 681d 682c 7562 758c 1273 7562 7374 6974  h.h,ubu..substit
-000020d0: 7574 696f 6e5f 6e61 6d65 7394 7d94 288c  ution_names.}.(.
-000020e0: 0f77 6f72 6463 6f75 6e74 2d77 6f72 6473  .wordcount-words
-000020f0: 946a 3c02 0000 8c11 776f 7264 636f 756e  .j<.....wordcoun
-00002100: 742d 6d69 6e75 7465 7394 6a4e 0200 0075  t-minutes.jN...u
-00002110: 8c08 7265 666e 616d 6573 947d 948c 0672  ..refnames.}...r
-00002120: 6566 6964 7394 7d94 8c07 6e61 6d65 6964  efids.}...nameid
-00002130: 7394 7d94 286a d701 0000 6ad4 0100 0068  s.}.(j....j....h
-00002140: b968 b66a 9401 0000 6a91 0100 006a cf01  .h.j....j....j..
-00002150: 0000 6acc 0100 0075 8c09 6e61 6d65 7479  ..j....u..namety
-00002160: 7065 7394 7d94 286a d701 0000 8968 b989  pes.}.(j.....h..
-00002170: 6a94 0100 0089 6acf 0100 0089 7568 217d  j.....j.....uh!}
-00002180: 9428 6ad4 0100 0068 0c68 b668 2d6a 9101  .(j....h.h.h-j..
-00002190: 0000 68bc 6acc 0100 006a 9701 0000 758c  ..h.j....j....u.
-000021a0: 0d66 6f6f 746e 6f74 655f 7265 6673 947d  .footnote_refs.}
-000021b0: 948c 0d63 6974 6174 696f 6e5f 7265 6673  ...citation_refs
-000021c0: 947d 948c 0d61 7574 6f66 6f6f 746e 6f74  .}...autofootnot
-000021d0: 6573 945d 948c 1161 7574 6f66 6f6f 746e  es.]...autofootn
-000021e0: 6f74 655f 7265 6673 945d 948c 1073 796d  ote_refs.]...sym
-000021f0: 626f 6c5f 666f 6f74 6e6f 7465 7394 5d94  bol_footnotes.].
-00002200: 8c14 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-00002210: 655f 7265 6673 945d 948c 0966 6f6f 746e  e_refs.]...footn
-00002220: 6f74 6573 945d 948c 0963 6974 6174 696f  otes.]...citatio
-00002230: 6e73 945d 948c 1261 7574 6f66 6f6f 746e  ns.]...autofootn
-00002240: 6f74 655f 7374 6172 7494 4b01 8c15 7379  ote_start.K...sy
-00002250: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7374  mbol_footnote_st
-00002260: 6172 7494 4b00 8c0a 6964 5f63 6f75 6e74  art.K...id_count
-00002270: 6572 948c 0b63 6f6c 6c65 6374 696f 6e73  er...collections
-00002280: 948c 0743 6f75 6e74 6572 9493 947d 9485  ...Counter...}..
-00002290: 9452 948c 0e70 6172 7365 5f6d 6573 7361  .R...parse_messa
-000022a0: 6765 7394 5d94 8c12 7472 616e 7366 6f72  ges.]...transfor
-000022b0: 6d5f 6d65 7373 6167 6573 945d 948c 0b74  m_messages.]...t
-000022c0: 7261 6e73 666f 726d 6572 944e 8c0b 696e  ransformer.N..in
-000022d0: 636c 7564 655f 6c6f 6794 5d94 8c0a 6465  clude_log.]...de
-000022e0: 636f 7261 7469 6f6e 944e 681c 6803 8c0a  coration.Nh.h...
-000022f0: 6d79 7374 5f73 6c75 6773 947d 9475 622e  myst_slugs.}.ub.
+00000140: 9468 0f68 1e4b 0168 1d8c 5b43 3a5c 5573  .h.h.K.h..[C:\Us
+00000150: 6572 735c 6d61 7869 6d5c 4f6e 6544 7269  ers\maxim\OneDri
+00000160: 7665 5c44 6f63 756d 656e 7473 5c50 7974  ve\Documents\Pyt
+00000170: 686f 6e5c 5061 636b 6167 6573 5c6d 7a44  hon\Packages\mzD
+00000180: 6174 6158 4d4c 324d 6174 5c64 6f63 735c  ataXML2Mat\docs\
+00000190: 736f 7572 6365 5c69 6e73 7461 6c6c 6174  source\installat
+000001a0: 696f 6e2e 6d64 9468 1b68 0c68 1c68 0375  ion.md.h.h.h.h.u
+000001b0: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
+000001c0: 9428 6810 2981 947d 9428 6805 8c07 436f  .(h.)..}.(h...Co
+000001d0: 6d6d 616e 6494 6807 5d94 6816 8c07 436f  mmand.h.].h...Co
+000001e0: 6d6d 616e 6494 8594 8194 7d94 2868 1b68  mmand.....}.(h.h
+000001f0: 3068 1c68 0368 1d4e 681e 4e75 6261 681f  0h.h.h.Nh.Nubah.
+00000200: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00000210: 275d 9468 295d 9475 682b 680f 681e 4b02  '].h)].uh+h.h.K.
+00000220: 681d 682c 681b 682d 681c 6803 7562 6809  h.h,h.h-h.h.ubh.
+00000230: 8c09 7061 7261 6772 6170 6894 9394 2981  ..paragraph...).
+00000240: 947d 9428 6805 8c66 546f 2069 6e73 7461  .}.(h..fTo insta
+00000250: 6c6c 2060 6d7a 6461 7461 326d 6174 6020  ll `mzdata2mat` 
+00000260: 696e 746f 2079 6f75 7220 5079 7468 6f6e  into your Python
+00000270: 2065 6e76 6972 6f6e 6d65 6e74 2c20 7275   environment, ru
+00000280: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+00000290: 636f 6d6d 616e 6420 696e 7369 6465 2079  command inside y
+000002a0: 6f75 7220 7465 726d 696e 616c 203a 9468  our terminal :.h
+000002b0: 075d 9428 6816 8c0b 546f 2069 6e73 7461  .].(h...To insta
+000002c0: 6c6c 2094 8594 8194 7d94 2868 1b68 4068  ll .....}.(h.h@h
+000002d0: 1c68 0368 1d4e 681e 4e75 6268 098c 076c  .h.h.Nh.Nubh...l
+000002e0: 6974 6572 616c 9493 9429 8194 7d94 2868  iteral...)..}.(h
+000002f0: 058c 0a6d 7a64 6174 6132 6d61 7494 6807  ...mzdata2mat.h.
+00000300: 5d94 6816 8c0a 6d7a 6461 7461 326d 6174  ].h...mzdata2mat
+00000310: 9485 9481 947d 9428 681b 684a 681c 6803  .....}.(h.hJh.h.
+00000320: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00000330: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00000340: 5d94 7568 2b68 4868 1e4b 0368 1d68 2c68  ].uh+hHh.K.h.h,h
+00000350: 1b68 4068 1c68 0375 6268 168c 4f20 696e  .h@h.h.ubh..O in
+00000360: 746f 2079 6f75 7220 5079 7468 6f6e 2065  to your Python e
+00000370: 6e76 6972 6f6e 6d65 6e74 2c20 7275 6e20  nvironment, run 
+00000380: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+00000390: 6d6d 616e 6420 696e 7369 6465 2079 6f75  mmand inside you
+000003a0: 7220 7465 726d 696e 616c 203a 9485 9481  r terminal :....
+000003b0: 947d 9428 681b 6840 681c 6803 681d 4e68  .}.(h.h@h.h.h.Nh
+000003c0: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
+000003d0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+000003e0: 2b68 3e68 1e4b 0368 1d68 2c68 1b68 2d68  +h>h.K.h.h,h.h-h
+000003f0: 1c68 0375 6268 098c 0d6c 6974 6572 616c  .h.ubh...literal
+00000400: 5f62 6c6f 636b 9493 9429 8194 7d94 2868  _block...)..}.(h
+00000410: 058c 1924 2070 6970 2069 6e73 7461 6c6c  ...$ pip install
+00000420: 206d 7a64 6174 6132 6d61 740a 9468 075d   mzdata2mat..h.]
+00000430: 9468 168c 1924 2070 6970 2069 6e73 7461  .h...$ pip insta
+00000440: 6c6c 206d 7a64 6174 6132 6d61 740a 9485  ll mzdata2mat...
+00000450: 9481 947d 9468 1b68 6473 6261 681f 7d94  ...}.h.hdsbah.}.
+00000460: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00000470: 9468 295d 948c 086c 616e 6775 6167 6594  .h)]...language.
+00000480: 8c05 7368 656c 6c94 8c09 786d 6c3a 7370  ..shell...xml:sp
+00000490: 6163 6594 8c08 7072 6573 6572 7665 9475  ace...preserve.u
+000004a0: 682b 6862 681d 682c 681e 4b04 681b 682d  h+hbh.h,h.K.h.h-
+000004b0: 681c 6803 7562 683f 2981 947d 9428 6805  h.h.ubh?)..}.(h.
+000004c0: 8caa 4966 2079 6f75 2068 6176 6520 6d75  ..If you have mu
+000004d0: 6c74 6970 6c65 2069 6e73 7461 6e63 6573  ltiple instances
+000004e0: 206f 6620 5079 7468 6f6e 2069 6e73 7461   of Python insta
+000004f0: 6c6c 6564 2c20 7275 6e20 7468 6973 2063  lled, run this c
+00000500: 6f6d 6d61 6e64 2077 6974 6820 7468 6520  ommand with the 
+00000510: 6368 6f73 656e 2050 7974 686f 6e20 696e  chosen Python in
+00000520: 7465 7270 7265 7465 7220 746f 2069 6e73  terpreter to ins
+00000530: 7461 6c6c 2060 6d7a 6461 7461 326d 6174  tall `mzdata2mat
+00000540: 6020 696e 2074 6865 2063 6f72 7265 7370  ` in the corresp
+00000550: 6f6e 6469 6e67 2050 7974 686f 6e20 696e  onding Python in
+00000560: 7374 616c 6c61 7469 6f6e 203a 9468 075d  stallation :.h.]
+00000570: 9428 6816 8c73 4966 2079 6f75 2068 6176  .(h..sIf you hav
+00000580: 6520 6d75 6c74 6970 6c65 2069 6e73 7461  e multiple insta
+00000590: 6e63 6573 206f 6620 5079 7468 6f6e 2069  nces of Python i
+000005a0: 6e73 7461 6c6c 6564 2c20 7275 6e20 7468  nstalled, run th
+000005b0: 6973 2063 6f6d 6d61 6e64 2077 6974 6820  is command with 
+000005c0: 7468 6520 6368 6f73 656e 2050 7974 686f  the chosen Pytho
+000005d0: 6e20 696e 7465 7270 7265 7465 7220 746f  n interpreter to
+000005e0: 2069 6e73 7461 6c6c 2094 8594 8194 7d94   install .....}.
+000005f0: 2868 1b68 7668 1c68 0368 1d4e 681e 4e75  (h.hvh.h.h.Nh.Nu
+00000600: 6268 4929 8194 7d94 2868 058c 0a6d 7a64  bhI)..}.(h...mzd
+00000610: 6174 6132 6d61 7494 6807 5d94 6816 8c0a  ata2mat.h.].h...
+00000620: 6d7a 6461 7461 326d 6174 9485 9481 947d  mzdata2mat.....}
+00000630: 9428 681b 687e 681c 6803 681d 4e68 1e4e  .(h.h~h.h.h.Nh.N
+00000640: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00000650: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00000660: 4868 1e4b 0768 1d68 2c68 1b68 7668 1c68  Hh.K.h.h,h.hvh.h
+00000670: 0375 6268 168c 2b20 696e 2074 6865 2063  .ubh..+ in the c
+00000680: 6f72 7265 7370 6f6e 6469 6e67 2050 7974  orresponding Pyt
+00000690: 686f 6e20 696e 7374 616c 6c61 7469 6f6e  hon installation
+000006a0: 203a 9485 9481 947d 9428 681b 6876 681c   :.....}.(h.hvh.
+000006b0: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
+000006c0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000006d0: 6829 5d94 7568 2b68 3e68 1e4b 0768 1d68  h)].uh+h>h.K.h.h
+000006e0: 2c68 1b68 2d68 1c68 0375 6268 6329 8194  ,h.h-h.h.ubhc)..
+000006f0: 7d94 2868 058c 2e24 203c 7061 7468 546f  }.(h...$ <pathTo
+00000700: 5079 7468 6f6e 4170 703e 202d 6d20 7069  PythonApp> -m pi
+00000710: 7020 696e 7374 616c 6c20 6d7a 6461 7461  p install mzdata
+00000720: 326d 6174 0a94 6807 5d94 6816 8c2e 2420  2mat..h.].h...$ 
+00000730: 3c70 6174 6854 6f50 7974 686f 6e41 7070  <pathToPythonApp
+00000740: 3e20 2d6d 2070 6970 2069 6e73 7461 6c6c  > -m pip install
+00000750: 206d 7a64 6174 6132 6d61 740a 9485 9481   mzdata2mat.....
+00000760: 947d 9468 1b68 9673 6261 681f 7d94 2868  .}.h.h.sbah.}.(h
+00000770: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00000780: 295d 948c 086c 616e 6775 6167 6594 8c05  )]...language...
+00000790: 7368 656c 6c94 6874 6875 7568 2b68 6268  shell.hthuuh+hbh
+000007a0: 1d68 2c68 1e4b 0868 1b68 2d68 1c68 0375  .h,h.K.h.h-h.h.u
+000007b0: 6268 3f29 8194 7d94 2868 058c 4957 6865  bh?)..}.(h..IWhe
+000007c0: 6e20 7468 6520 636f 6d6d 616e 6420 7465  n the command te
+000007d0: 726d 696e 6174 6573 2c20 796f 7520 6861  rminates, you ha
+000007e0: 7665 2073 7563 6365 7373 6675 6c6c 7920  ve successfully 
+000007f0: 696e 7374 616c 6c65 6420 6d7a 6461 7461  installed mzdata
+00000800: 326d 6174 2021 9468 075d 9468 168c 4957  2mat !.h.].h..IW
+00000810: 6865 6e20 7468 6520 636f 6d6d 616e 6420  hen the command 
+00000820: 7465 726d 696e 6174 6573 2c20 796f 7520  terminates, you 
+00000830: 6861 7665 2073 7563 6365 7373 6675 6c6c  have successfull
+00000840: 7920 696e 7374 616c 6c65 6420 6d7a 6461  y installed mzda
+00000850: 7461 326d 6174 2021 9485 9481 947d 9428  ta2mat !.....}.(
+00000860: 681b 68a6 681c 6803 681d 4e68 1e4e 7562  h.h.h.h.h.Nh.Nub
+00000870: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00000880: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
+00000890: 1e4b 0b68 1d68 2c68 1b68 2d68 1c68 0375  .K.h.h,h.h-h.h.u
+000008a0: 6265 681f 7d94 2868 215d 948c 0763 6f6d  beh.}.(h!]...com
+000008b0: 6d61 6e64 9461 6823 5d94 6825 5d94 8c07  mand.ah#].h%]...
+000008c0: 636f 6d6d 616e 6494 6168 275d 9468 295d  command.ah'].h)]
+000008d0: 9475 682b 680a 681e 4b02 681d 682c 681b  .uh+h.h.K.h.h,h.
+000008e0: 680c 681c 6803 7562 680b 2981 947d 9428  h.h.h.ubh.)..}.(
+000008f0: 6805 6806 6807 5d94 2868 1029 8194 7d94  h.h.h.].(h.)..}.
+00000900: 2868 058c 1756 6572 6966 7920 7468 6520  (h...Verify the 
+00000910: 696e 7374 616c 6c61 7469 6f6e 9468 075d  installation.h.]
+00000920: 9468 168c 1756 6572 6966 7920 7468 6520  .h...Verify the 
+00000930: 696e 7374 616c 6c61 7469 6f6e 9485 9481  installation....
+00000940: 947d 9428 681b 68bf 681c 6803 681d 4e68  .}.(h.h.h.h.h.Nh
+00000950: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00000960: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00000970: 2b68 0f68 1e4b 0d68 1d68 2c68 1b68 bc68  +h.h.K.h.h,h.h.h
+00000980: 1c68 0375 6268 3f29 8194 7d94 2868 058c  .h.ubh?)..}.(h..
+00000990: 5154 6f20 7665 7266 6979 2069 6620 7468  QTo verfiy if th
+000009a0: 6520 696e 7374 616c 6c61 7469 6f6e 2077  e installation w
+000009b0: 6173 2073 7563 6365 7373 6675 6c2c 2072  as successful, r
+000009c0: 756e 2069 6e20 796f 7572 2074 6572 6d69  un in your termi
+000009d0: 6e61 6c20 7468 6973 2063 6f6d 6d61 6e64  nal this command
+000009e0: 203a 9468 075d 9468 168c 5154 6f20 7665   :.h.].h..QTo ve
+000009f0: 7266 6979 2069 6620 7468 6520 696e 7374  rfiy if the inst
+00000a00: 616c 6c61 7469 6f6e 2077 6173 2073 7563  allation was suc
+00000a10: 6365 7373 6675 6c2c 2072 756e 2069 6e20  cessful, run in 
+00000a20: 796f 7572 2074 6572 6d69 6e61 6c20 7468  your terminal th
+00000a30: 6973 2063 6f6d 6d61 6e64 203a 9485 9481  is command :....
+00000a40: 947d 9428 681b 68cd 681c 6803 681d 4e68  .}.(h.h.h.h.h.Nh
+00000a50: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00000a60: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00000a70: 2b68 3e68 1e4b 0e68 1d68 2c68 1b68 bc68  +h>h.K.h.h,h.h.h
+00000a80: 1c68 0375 6268 6329 8194 7d94 2868 058c  .h.ubhc)..}.(h..
+00000a90: 1424 206d 7a64 6174 6132 6d61 742d 7665  .$ mzdata2mat-ve
+00000aa0: 7269 6679 0a94 6807 5d94 6816 8c14 2420  rify..h.].h...$ 
+00000ab0: 6d7a 6461 7461 326d 6174 2d76 6572 6966  mzdata2mat-verif
+00000ac0: 790a 9485 9481 947d 9468 1b68 db73 6261  y......}.h.h.sba
+00000ad0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00000ae0: 9468 275d 9468 295d 948c 086c 616e 6775  .h'].h)]...langu
+00000af0: 6167 6594 8c05 7368 656c 6c94 6874 6875  age...shell.hthu
+00000b00: 7568 2b68 6268 1d68 2c68 1e4b 0f68 1b68  uh+hbh.h,h.K.h.h
+00000b10: bc68 1c68 0375 6268 3f29 8194 7d94 2868  .h.h.ubh?)..}.(h
+00000b20: 058c de57 6865 6e20 796f 7520 7769 6c6c  ...When you will
+00000b30: 2066 6972 7374 2072 756e 2074 6869 7320   first run this 
+00000b40: 636f 6d6d 616e 642c 206e 6f64 652e 6a73  command, node.js
+00000b50: 2077 696c 6c20 646f 776e 6c6f 6164 2061   will download a
+00000b60: 6e64 2069 6e73 7461 6c6c 2074 6865 2060  nd install the `
+00000b70: 6d7a 6461 7461 6020 7061 636b 6167 6520  mzdata` package 
+00000b80: 6672 6f6d 2060 6e70 6d60 2e20 5468 6973  from `npm`. This
+00000b90: 2077 696c 6c20 6f6e 6c79 2068 6170 7065   will only happe
+00000ba0: 6e20 7468 6520 6669 7273 7420 7469 6d65  n the first time
+00000bb0: 2079 6f75 2072 756e 2074 6865 2063 6f6d   you run the com
+00000bc0: 6d61 6e64 2e20 5468 6520 7465 726d 696e  mand. The termin
+00000bd0: 616c 2077 696c 6c20 7368 6f77 2079 6f75  al will show you
+00000be0: 2074 6865 7365 206c 696e 6573 2064 7572   these lines dur
+00000bf0: 696e 6720 7468 6520 7072 6f63 6573 7320  ing the process 
+00000c00: 3a94 6807 5d94 2868 168c 4c57 6865 6e20  :.h.].(h..LWhen 
+00000c10: 796f 7520 7769 6c6c 2066 6972 7374 2072  you will first r
+00000c20: 756e 2074 6869 7320 636f 6d6d 616e 642c  un this command,
+00000c30: 206e 6f64 652e 6a73 2077 696c 6c20 646f   node.js will do
+00000c40: 776e 6c6f 6164 2061 6e64 2069 6e73 7461  wnload and insta
+00000c50: 6c6c 2074 6865 2094 8594 8194 7d94 2868  ll the .....}.(h
+00000c60: 1b68 eb68 1c68 0368 1d4e 681e 4e75 6268  .h.h.h.h.Nh.Nubh
+00000c70: 4929 8194 7d94 2868 058c 066d 7a64 6174  I)..}.(h...mzdat
+00000c80: 6194 6807 5d94 6816 8c06 6d7a 6461 7461  a.h.].h...mzdata
+00000c90: 9485 9481 947d 9428 681b 68f3 681c 6803  .....}.(h.h.h.h.
+00000ca0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00000cb0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00000cc0: 5d94 7568 2b68 4868 1e4b 1268 1d68 2c68  ].uh+hHh.K.h.h,h
+00000cd0: 1b68 eb68 1c68 0375 6268 168c 0e20 7061  .h.h.h.ubh... pa
+00000ce0: 636b 6167 6520 6672 6f6d 2094 8594 8194  ckage from .....
+00000cf0: 7d94 2868 1b68 eb68 1c68 0368 1d4e 681e  }.(h.h.h.h.h.Nh.
+00000d00: 4e75 6268 4929 8194 7d94 2868 058c 036e  NubhI)..}.(h...n
+00000d10: 706d 9468 075d 9468 168c 036e 706d 9485  pm.h.].h...npm..
+00000d20: 9481 947d 9428 681b 6a05 0100 0068 1c68  ...}.(h.j....h.h
+00000d30: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00000d40: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00000d50: 295d 9475 682b 6848 681e 4b12 681d 682c  )].uh+hHh.K.h.h,
+00000d60: 681b 68eb 681c 6803 7562 6816 8c77 2e20  h.h.h.h.ubh..w. 
+00000d70: 5468 6973 2077 696c 6c20 6f6e 6c79 2068  This will only h
+00000d80: 6170 7065 6e20 7468 6520 6669 7273 7420  appen the first 
+00000d90: 7469 6d65 2079 6f75 2072 756e 2074 6865  time you run the
+00000da0: 2063 6f6d 6d61 6e64 2e20 5468 6520 7465   command. The te
+00000db0: 726d 696e 616c 2077 696c 6c20 7368 6f77  rminal will show
+00000dc0: 2079 6f75 2074 6865 7365 206c 696e 6573   you these lines
+00000dd0: 2064 7572 696e 6720 7468 6520 7072 6f63   during the proc
+00000de0: 6573 7320 3a94 8594 8194 7d94 2868 1b68  ess :.....}.(h.h
+00000df0: eb68 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
+00000e00: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00000e10: 275d 9468 295d 9475 682b 683e 681e 4b12  '].h)].uh+h>h.K.
+00000e20: 681d 682c 681b 68bc 681c 6803 7562 6863  h.h,h.h.h.h.ubhc
+00000e30: 2981 947d 9428 6805 8ce4 2049 6e73 7461  )..}.(h... Insta
+00000e40: 6c6c 696e 6720 276d 7a64 6174 6127 2076  lling 'mzdata' v
+00000e50: 6572 7369 6f6e 2027 6c61 7465 7374 272e  ersion 'latest'.
+00000e60: 2e2e 2054 6869 7320 7769 6c6c 206f 6e6c  .. This will onl
+00000e70: 7920 6861 7070 656e 206f 6e63 652e 200a  y happen once. .
+00000e80: 0a61 6464 6564 2037 2070 6163 6b61 6765  .added 7 package
+00000e90: 732c 2061 6e64 2061 7564 6974 6564 2038  s, and audited 8
+00000ea0: 2070 6163 6b61 6765 7320 696e 2032 730a   packages in 2s.
+00000eb0: 0a31 2070 6163 6b61 6765 2069 7320 6c6f  .1 package is lo
+00000ec0: 6f6b 696e 6720 666f 7220 6675 6e64 696e  oking for fundin
+00000ed0: 670a 2020 7275 6e20 606e 706d 2066 756e  g.  run `npm fun
+00000ee0: 6460 2066 6f72 2064 6574 6169 6c73 0a0a  d` for details..
+00000ef0: 666f 756e 6420 3020 7675 6c6e 6572 6162  found 0 vulnerab
+00000f00: 696c 6974 6965 730a 0a20 4f4b 2e20 0a5b  ilities.. OK. .[
+00000f10: 4a53 455d 200a 0a5b 4a53 455d 200a 9468  JSE] ..[JSE] ..h
+00000f20: 075d 9468 168c e420 496e 7374 616c 6c69  .].h... Installi
+00000f30: 6e67 2027 6d7a 6461 7461 2720 7665 7273  ng 'mzdata' vers
+00000f40: 696f 6e20 276c 6174 6573 7427 2e2e 2e20  ion 'latest'... 
+00000f50: 5468 6973 2077 696c 6c20 6f6e 6c79 2068  This will only h
+00000f60: 6170 7065 6e20 6f6e 6365 2e20 0a0a 6164  appen once. ..ad
+00000f70: 6465 6420 3720 7061 636b 6167 6573 2c20  ded 7 packages, 
+00000f80: 616e 6420 6175 6469 7465 6420 3820 7061  and audited 8 pa
+00000f90: 636b 6167 6573 2069 6e20 3273 0a0a 3120  ckages in 2s..1 
+00000fa0: 7061 636b 6167 6520 6973 206c 6f6f 6b69  package is looki
+00000fb0: 6e67 2066 6f72 2066 756e 6469 6e67 0a20  ng for funding. 
+00000fc0: 2072 756e 2060 6e70 6d20 6675 6e64 6020   run `npm fund` 
+00000fd0: 666f 7220 6465 7461 696c 730a 0a66 6f75  for details..fou
+00000fe0: 6e64 2030 2076 756c 6e65 7261 6269 6c69  nd 0 vulnerabili
+00000ff0: 7469 6573 0a0a 204f 4b2e 200a 5b4a 5345  ties.. OK. .[JSE
+00001000: 5d20 0a0a 5b4a 5345 5d20 0a94 8594 8194  ] ..[JSE] ......
+00001010: 7d94 681b 6a1d 0100 0073 6261 681f 7d94  }.h.j....sbah.}.
+00001020: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001030: 9468 295d 948c 086c 616e 6775 6167 6594  .h)]...language.
+00001040: 8c05 7368 656c 6c94 6874 6875 7568 2b68  ..shell.hthuuh+h
+00001050: 6268 1d68 2c68 1e4b 1368 1b68 bc68 1c68  bh.h,h.K.h.h.h.h
+00001060: 0375 6268 3f29 8194 7d94 2868 058c a857  .ubh?)..}.(h...W
+00001070: 6865 6e20 6974 2773 2064 6f6e 652c 2074  hen it's done, t
+00001080: 6865 2060 6d7a 6461 7461 326d 6174 6020  he `mzdata2mat` 
+00001090: 7061 636b 6167 6520 7769 6c6c 2061 7474  package will att
+000010a0: 656d 7074 2074 6f20 636f 6e76 6572 7420  empt to convert 
+000010b0: 616e 2065 7861 6d70 6c65 2060 2e6d 7a64  an example `.mzd
+000010c0: 6174 612e 786d 6c60 2066 696c 6520 696e  ata.xml` file in
+000010d0: 746f 2061 2060 2e6d 6174 6020 6669 6c65  to a `.mat` file
+000010e0: 2e20 4966 2065 7665 7279 7468 696e 6720  . If everything 
+000010f0: 676f 6573 2072 6967 6874 2c20 796f 7520  goes right, you 
+00001100: 7769 6c6c 2067 6574 2074 6869 7320 6d65  will get this me
+00001110: 7373 6167 6520 3a94 6807 5d94 2868 168c  ssage :.h.].(h..
+00001120: 1657 6865 6e20 6974 e280 9973 2064 6f6e  .When it...s don
+00001130: 652c 2074 6865 2094 8594 8194 7d94 2868  e, the .....}.(h
+00001140: 1b6a 2d01 0000 681c 6803 681d 4e68 1e4e  .j-...h.h.h.Nh.N
+00001150: 7562 6849 2981 947d 9428 6805 8c0a 6d7a  ubhI)..}.(h...mz
+00001160: 6461 7461 326d 6174 9468 075d 9468 168c  data2mat.h.].h..
+00001170: 0a6d 7a64 6174 6132 6d61 7494 8594 8194  .mzdata2mat.....
+00001180: 7d94 2868 1b6a 3501 0000 681c 6803 681d  }.(h.j5...h.h.h.
+00001190: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+000011a0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000011b0: 7568 2b68 4868 1e4b 2268 1d68 2c68 1b6a  uh+hHh.K"h.h,h.j
+000011c0: 2d01 0000 681c 6803 7562 6816 8c2c 2070  -...h.h.ubh.., p
+000011d0: 6163 6b61 6765 2077 696c 6c20 6174 7465  ackage will atte
+000011e0: 6d70 7420 746f 2063 6f6e 7665 7274 2061  mpt to convert a
+000011f0: 6e20 6578 616d 706c 6520 9485 9481 947d  n example .....}
+00001200: 9428 681b 6a2d 0100 0068 1c68 0368 1d4e  .(h.j-...h.h.h.N
+00001210: 681e 4e75 6268 4929 8194 7d94 2868 058c  h.NubhI)..}.(h..
+00001220: 0b2e 6d7a 6461 7461 2e78 6d6c 9468 075d  ..mzdata.xml.h.]
+00001230: 9468 168c 0b2e 6d7a 6461 7461 2e78 6d6c  .h....mzdata.xml
+00001240: 9485 9481 947d 9428 681b 6a47 0100 0068  .....}.(h.jG...h
+00001250: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00001260: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001270: 9468 295d 9475 682b 6848 681e 4b22 681d  .h)].uh+hHh.K"h.
+00001280: 682c 681b 6a2d 0100 0068 1c68 0375 6268  h,h.j-...h.h.ubh
+00001290: 168c 0d20 6669 6c65 2069 6e74 6f20 6120  ... file into a 
+000012a0: 9485 9481 947d 9428 681b 6a2d 0100 0068  .....}.(h.j-...h
+000012b0: 1c68 0368 1d4e 681e 4e75 6268 4929 8194  .h.h.Nh.NubhI)..
+000012c0: 7d94 2868 058c 042e 6d61 7494 6807 5d94  }.(h....mat.h.].
+000012d0: 6816 8c04 2e6d 6174 9485 9481 947d 9428  h....mat.....}.(
+000012e0: 681b 6a59 0100 0068 1c68 0368 1d4e 681e  h.jY...h.h.h.Nh.
+000012f0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00001300: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00001310: 6848 681e 4b22 681d 682c 681b 6a2d 0100  hHh.K"h.h,h.j-..
+00001320: 0068 1c68 0375 6268 168c 3c20 6669 6c65  .h.h.ubh..< file
+00001330: 2e20 4966 2065 7665 7279 7468 696e 6720  . If everything 
+00001340: 676f 6573 2072 6967 6874 2c20 796f 7520  goes right, you 
+00001350: 7769 6c6c 2067 6574 2074 6869 7320 6d65  will get this me
+00001360: 7373 6167 6520 3a94 8594 8194 7d94 2868  ssage :.....}.(h
+00001370: 1b6a 2d01 0000 681c 6803 681d 4e68 1e4e  .j-...h.h.h.Nh.N
+00001380: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+00001390: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+000013a0: 3e68 1e4b 2268 1d68 2c68 1b68 bc68 1c68  >h.K"h.h,h.h.h.h
+000013b0: 0375 6268 6329 8194 7d94 2868 058c 1e24  .ubhc)..}.(h...$
+000013c0: 206d 7a64 6174 6132 6d61 7420 2d20 5265   mzdata2mat - Re
+000013d0: 6164 7920 746f 2075 7365 2021 0a94 6807  ady to use !..h.
+000013e0: 5d94 6816 8c1e 2420 6d7a 6461 7461 326d  ].h...$ mzdata2m
+000013f0: 6174 202d 2052 6561 6479 2074 6f20 7573  at - Ready to us
+00001400: 6520 210a 9485 9481 947d 9468 1b6a 7101  e !......}.h.jq.
+00001410: 0000 7362 6168 1f7d 9428 6821 5d94 6823  ..sbah.}.(h!].h#
+00001420: 5d94 6825 5d94 6827 5d94 6829 5d94 8c08  ].h%].h'].h)]...
+00001430: 6c61 6e67 7561 6765 948c 0573 6865 6c6c  language...shell
+00001440: 9468 7468 7575 682b 6862 681d 682c 681e  .hthuuh+hbh.h,h.
+00001450: 4b23 681b 68bc 681c 6803 7562 683f 2981  K#h.h.h.h.ubh?).
+00001460: 947d 9428 6805 8c9e 5468 6520 6578 616d  .}.(h...The exam
+00001470: 706c 6520 6669 6c65 2028 2e6d 7a64 6174  ple file (.mzdat
+00001480: 612e 786d 6c29 2077 696c 6c20 6265 2063  a.xml) will be c
+00001490: 6f70 6965 6420 696e 2074 6865 2063 7572  opied in the cur
+000014a0: 7265 6e74 2077 6f72 6b69 6e67 2064 6972  rent working dir
+000014b0: 6563 746f 7279 2061 6e64 2074 6865 2063  ectory and the c
+000014c0: 6f6e 7665 7274 6564 2066 696c 6520 282e  onverted file (.
+000014d0: 6d61 7429 2077 696c 6c20 6265 2061 6464  mat) will be add
+000014e0: 6564 2061 7320 736f 6f6e 2061 7320 7468  ed as soon as th
+000014f0: 6520 636f 6e76 6572 7369 6f6e 2066 696e  e conversion fin
+00001500: 6973 6865 732e 9468 075d 9468 168c 9e54  ishes..h.].h...T
+00001510: 6865 2065 7861 6d70 6c65 2066 696c 6520  he example file 
+00001520: 282e 6d7a 6461 7461 2e78 6d6c 2920 7769  (.mzdata.xml) wi
+00001530: 6c6c 2062 6520 636f 7069 6564 2069 6e20  ll be copied in 
+00001540: 7468 6520 6375 7272 656e 7420 776f 726b  the current work
+00001550: 696e 6720 6469 7265 6374 6f72 7920 616e  ing directory an
+00001560: 6420 7468 6520 636f 6e76 6572 7465 6420  d the converted 
+00001570: 6669 6c65 2028 2e6d 6174 2920 7769 6c6c  file (.mat) will
+00001580: 2062 6520 6164 6465 6420 6173 2073 6f6f   be added as soo
+00001590: 6e20 6173 2074 6865 2063 6f6e 7665 7273  n as the convers
+000015a0: 696f 6e20 6669 6e69 7368 6573 2e94 8594  ion finishes....
+000015b0: 8194 7d94 2868 1b6a 8101 0000 681c 6803  ..}.(h.j....h.h.
+000015c0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000015d0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000015e0: 5d94 7568 2b68 3e68 1e4b 2668 1d68 2c68  ].uh+h>h.K&h.h,h
+000015f0: 1b68 bc68 1c68 0375 6265 681f 7d94 2868  .h.h.h.ubeh.}.(h
+00001600: 215d 948c 1776 6572 6966 792d 7468 652d  !]...verify-the-
+00001610: 696e 7374 616c 6c61 7469 6f6e 9461 6823  installation.ah#
+00001620: 5d94 6825 5d94 8c17 7665 7269 6679 2074  ].h%]...verify t
+00001630: 6865 2069 6e73 7461 6c6c 6174 696f 6e94  he installation.
+00001640: 6168 275d 9468 295d 9475 682b 680a 681e  ah'].h)].uh+h.h.
+00001650: 4b0d 681d 682c 681b 680c 681c 6803 7562  K.h.h,h.h.h.h.ub
+00001660: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
+00001670: 2868 1029 8194 7d94 2868 058c 1054 726f  (h.)..}.(h...Tro
+00001680: 7562 626c 6573 686f 6f74 696e 6794 6807  ubbleshooting.h.
+00001690: 5d94 6816 8c10 5472 6f75 6262 6c65 7368  ].h...Troubblesh
+000016a0: 6f6f 7469 6e67 9485 9481 947d 9428 681b  ooting.....}.(h.
+000016b0: 6a9a 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+000016c0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+000016d0: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
+000016e0: 681e 4b28 681d 682c 681b 6a97 0100 0068  h.K(h.h,h.j....h
+000016f0: 1c68 0375 6268 3f29 8194 7d94 2868 058c  .h.ubh?)..}.(h..
+00001700: 8549 6620 616e 2065 7272 6f72 206f 6363  .If an error occ
+00001710: 7572 732c 2074 6869 7320 7072 6f62 6162  urs, this probab
+00001720: 6c79 206d 6561 6e73 2074 6861 7420 796f  ly means that yo
+00001730: 7520 646f 206e 6f74 2068 6176 6520 5f5f  u do not have __
+00001740: 6e6f 6465 2e6a 735f 5f20 696e 7374 616c  node.js__ instal
+00001750: 6c65 6420 6f6e 2079 6f75 7220 6d61 6368  led on your mach
+00001760: 696e 6520 6f72 2079 6f75 2064 6964 6e27  ine or you didn'
+00001770: 7420 6164 6420 6974 2074 6f20 796f 7572  t add it to your
+00001780: 2050 4154 482e 9468 075d 9428 6816 8c3d   PATH..h.].(h..=
+00001790: 4966 2061 6e20 6572 726f 7220 6f63 6375  If an error occu
+000017a0: 7273 2c20 7468 6973 2070 726f 6261 626c  rs, this probabl
+000017b0: 7920 6d65 616e 7320 7468 6174 2079 6f75  y means that you
+000017c0: 2064 6f20 6e6f 7420 6861 7665 2094 8594   do not have ...
+000017d0: 8194 7d94 2868 1b6a a801 0000 681c 6803  ..}.(h.j....h.h.
+000017e0: 681d 4e68 1e4e 7562 6809 8c06 7374 726f  h.Nh.Nubh...stro
+000017f0: 6e67 9493 9429 8194 7d94 2868 058c 076e  ng...)..}.(h...n
+00001800: 6f64 652e 6a73 9468 075d 9468 168c 076e  ode.js.h.].h...n
+00001810: 6f64 652e 6a73 9485 9481 947d 9428 681b  ode.js.....}.(h.
+00001820: 6ab2 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00001830: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00001840: 255d 9468 275d 9468 295d 9475 682b 6ab0  %].h'].h)].uh+j.
+00001850: 0100 0068 1e4b 2968 1d68 2c68 1b6a a801  ...h.K)h.h,h.j..
+00001860: 0000 681c 6803 7562 6816 8c3f 2069 6e73  ..h.h.ubh..? ins
+00001870: 7461 6c6c 6564 206f 6e20 796f 7572 206d  talled on your m
+00001880: 6163 6869 6e65 206f 7220 796f 7520 6469  achine or you di
+00001890: 646e e280 9974 2061 6464 2069 7420 746f  dn...t add it to
+000018a0: 2079 6f75 7220 5041 5448 2e94 8594 8194   your PATH......
+000018b0: 7d94 2868 1b6a a801 0000 681c 6803 681d  }.(h.j....h.h.h.
+000018c0: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
+000018d0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000018e0: 7568 2b68 3e68 1e4b 2968 1d68 2c68 1b6a  uh+h>h.K)h.h,h.j
+000018f0: 9701 0000 681c 6803 7562 6568 1f7d 9428  ....h.h.ubeh.}.(
+00001900: 6821 5d94 8c10 7472 6f75 6262 6c65 7368  h!]...troubblesh
+00001910: 6f6f 7469 6e67 9461 6823 5d94 6825 5d94  ooting.ah#].h%].
+00001920: 8c10 7472 6f75 6262 6c65 7368 6f6f 7469  ..troubbleshooti
+00001930: 6e67 9461 6827 5d94 6829 5d94 7568 2b68  ng.ah'].h)].uh+h
+00001940: 0a68 1e4b 2868 1d68 2c68 1b68 0c68 1c68  .h.K(h.h,h.h.h.h
+00001950: 0375 6265 681f 7d94 2868 215d 948c 0c69  .ubeh.}.(h!]...i
+00001960: 6e73 7461 6c6c 6174 696f 6e94 6168 235d  nstallation.ah#]
+00001970: 9468 255d 948c 0c69 6e73 7461 6c6c 6174  .h%]...installat
+00001980: 696f 6e94 6168 275d 9468 295d 9475 682b  ion.ah'].h)].uh+
+00001990: 680a 681e 4b01 681d 682c 681b 6803 681c  h.h.K.h.h,h.h.h.
+000019a0: 6803 7562 6168 1f7d 9428 6821 5d94 6823  h.ubah.}.(h!].h#
+000019b0: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
+000019c0: 736f 7572 6365 9468 2c8c 1474 7261 6e73  source.h,..trans
+000019d0: 6c61 7469 6f6e 5f70 726f 6772 6573 7394  lation_progress.
+000019e0: 7d94 288c 0574 6f74 616c 944b 008c 0a74  }.(..total.K...t
+000019f0: 7261 6e73 6c61 7465 6494 4b00 7575 682b  ranslated.K.uuh+
+00001a00: 6801 8c0e 6375 7272 656e 745f 736f 7572  h...current_sour
+00001a10: 6365 944e 8c0c 6375 7272 656e 745f 6c69  ce.N..current_li
+00001a20: 6e65 944e 8c08 7365 7474 696e 6773 948c  ne.N..settings..
+00001a30: 1164 6f63 7574 696c 732e 6672 6f6e 7465  .docutils.fronte
+00001a40: 6e64 948c 0656 616c 7565 7394 9394 2981  nd...Values...).
+00001a50: 947d 9428 8c06 6f75 7470 7574 944e 680f  .}.(..output.Nh.
+00001a60: 4e8c 0967 656e 6572 6174 6f72 944e 8c09  N..generator.N..
+00001a70: 6461 7465 7374 616d 7094 4e8c 0b73 6f75  datestamp.N..sou
+00001a80: 7263 655f 6c69 6e6b 944e 8c0a 736f 7572  rce_link.N..sour
+00001a90: 6365 5f75 726c 944e 8c0d 746f 635f 6261  ce_url.N..toc_ba
+00001aa0: 636b 6c69 6e6b 7394 8c05 656e 7472 7994  cklinks...entry.
+00001ab0: 8c12 666f 6f74 6e6f 7465 5f62 6163 6b6c  ..footnote_backl
+00001ac0: 696e 6b73 944b 018c 0d73 6563 746e 756d  inks.K...sectnum
+00001ad0: 5f78 666f 726d 944b 018c 0e73 7472 6970  _xform.K...strip
+00001ae0: 5f63 6f6d 6d65 6e74 7394 4e8c 1b73 7472  _comments.N..str
+00001af0: 6970 5f65 6c65 6d65 6e74 735f 7769 7468  ip_elements_with
+00001b00: 5f63 6c61 7373 6573 944e 8c0d 7374 7269  _classes.N..stri
+00001b10: 705f 636c 6173 7365 7394 4e8c 0c72 6570  p_classes.N..rep
+00001b20: 6f72 745f 6c65 7665 6c94 4b02 8c0a 6861  ort_level.K...ha
+00001b30: 6c74 5f6c 6576 656c 944b 058c 1165 7869  lt_level.K...exi
+00001b40: 745f 7374 6174 7573 5f6c 6576 656c 944b  t_status_level.K
+00001b50: 058c 0564 6562 7567 944e 8c0e 7761 726e  ...debug.N..warn
+00001b60: 696e 675f 7374 7265 616d 944e 8c09 7472  ing_stream.N..tr
+00001b70: 6163 6562 6163 6b94 888c 0e69 6e70 7574  aceback....input
+00001b80: 5f65 6e63 6f64 696e 6794 8c09 7574 662d  _encoding...utf-
+00001b90: 382d 7369 6794 8c1c 696e 7075 745f 656e  8-sig...input_en
+00001ba0: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
+00001bb0: 646c 6572 948c 0673 7472 6963 7494 8c0f  dler...strict...
+00001bc0: 6f75 7470 7574 5f65 6e63 6f64 696e 6794  output_encoding.
+00001bd0: 8c05 7574 662d 3894 8c1d 6f75 7470 7574  ..utf-8...output
+00001be0: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
+00001bf0: 6861 6e64 6c65 7294 6a02 0200 008c 0e65  handler.j......e
+00001c00: 7272 6f72 5f65 6e63 6f64 696e 6794 8c05  rror_encoding...
+00001c10: 7574 662d 3894 8c1c 6572 726f 725f 656e  utf-8...error_en
+00001c20: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
+00001c30: 646c 6572 948c 1062 6163 6b73 6c61 7368  dler...backslash
+00001c40: 7265 706c 6163 6594 8c0d 6c61 6e67 7561  replace...langua
+00001c50: 6765 5f63 6f64 6594 8c02 656e 948c 1372  ge_code...en...r
+00001c60: 6563 6f72 645f 6465 7065 6e64 656e 6369  ecord_dependenci
+00001c70: 6573 944e 8c06 636f 6e66 6967 944e 8c09  es.N..config.N..
+00001c80: 6964 5f70 7265 6669 7894 6806 8c0e 6175  id_prefix.h...au
+00001c90: 746f 5f69 645f 7072 6566 6978 948c 0269  to_id_prefix...i
+00001ca0: 6494 8c0d 6475 6d70 5f73 6574 7469 6e67  d...dump_setting
+00001cb0: 7394 4e8c 0e64 756d 705f 696e 7465 726e  s.N..dump_intern
+00001cc0: 616c 7394 4e8c 0f64 756d 705f 7472 616e  als.N..dump_tran
+00001cd0: 7366 6f72 6d73 944e 8c0f 6475 6d70 5f70  sforms.N..dump_p
+00001ce0: 7365 7564 6f5f 786d 6c94 4e8c 1065 7870  seudo_xml.N..exp
+00001cf0: 6f73 655f 696e 7465 726e 616c 7394 4e8c  ose_internals.N.
+00001d00: 0e73 7472 6963 745f 7669 7369 746f 7294  .strict_visitor.
+00001d10: 4e8c 0f5f 6469 7361 626c 655f 636f 6e66  N.._disable_conf
+00001d20: 6967 944e 8c07 5f73 6f75 7263 6594 682c  ig.N.._source.h,
+00001d30: 8c0c 5f64 6573 7469 6e61 7469 6f6e 944e  .._destination.N
+00001d40: 8c0d 5f63 6f6e 6669 675f 6669 6c65 7394  .._config_files.
+00001d50: 5d94 8c16 6669 6c65 5f69 6e73 6572 7469  ]...file_inserti
+00001d60: 6f6e 5f65 6e61 626c 6564 9488 8c0b 7261  on_enabled....ra
+00001d70: 775f 656e 6162 6c65 6494 4b01 8c11 6c69  w_enabled.K...li
+00001d80: 6e65 5f6c 656e 6774 685f 6c69 6d69 7494  ne_length_limit.
+00001d90: 4d10 278c 0e70 6570 5f72 6566 6572 656e  M.'..pep_referen
+00001da0: 6365 7394 4e8c 0c70 6570 5f62 6173 655f  ces.N..pep_base_
+00001db0: 7572 6c94 8c18 6874 7470 733a 2f2f 7065  url...https://pe
+00001dc0: 7073 2e70 7974 686f 6e2e 6f72 672f 948c  ps.python.org/..
+00001dd0: 1570 6570 5f66 696c 655f 7572 6c5f 7465  .pep_file_url_te
+00001de0: 6d70 6c61 7465 948c 0870 6570 2d25 3034  mplate...pep-%04
+00001df0: 6494 8c0e 7266 635f 7265 6665 7265 6e63  d...rfc_referenc
+00001e00: 6573 944e 8c0c 7266 635f 6261 7365 5f75  es.N..rfc_base_u
+00001e10: 726c 948c 2668 7474 7073 3a2f 2f64 6174  rl..&https://dat
+00001e20: 6174 7261 636b 6572 2e69 6574 662e 6f72  atracker.ietf.or
+00001e30: 672f 646f 632f 6874 6d6c 2f94 8c09 7461  g/doc/html/...ta
+00001e40: 625f 7769 6474 6894 4b08 8c1d 7472 696d  b_width.K...trim
+00001e50: 5f66 6f6f 746e 6f74 655f 7265 6665 7265  _footnote_refere
+00001e60: 6e63 655f 7370 6163 6594 898c 1073 796e  nce_space....syn
+00001e70: 7461 785f 6869 6768 6c69 6768 7494 8c04  tax_highlight...
+00001e80: 6c6f 6e67 948c 0c73 6d61 7274 5f71 756f  long...smart_quo
+00001e90: 7465 7394 888c 1373 6d61 7274 7175 6f74  tes....smartquot
+00001ea0: 6573 5f6c 6f63 616c 6573 945d 948c 1d63  es_locales.]...c
+00001eb0: 6861 7261 6374 6572 5f6c 6576 656c 5f69  haracter_level_i
+00001ec0: 6e6c 696e 655f 6d61 726b 7570 9489 8c0e  nline_markup....
+00001ed0: 646f 6374 6974 6c65 5f78 666f 726d 9489  doctitle_xform..
+00001ee0: 8c0d 646f 6369 6e66 6f5f 7866 6f72 6d94  ..docinfo_xform.
+00001ef0: 4b01 8c12 7365 6374 7375 6274 6974 6c65  K...sectsubtitle
+00001f00: 5f78 666f 726d 9489 8c0d 696d 6167 655f  _xform....image_
+00001f10: 6c6f 6164 696e 6794 8c04 6c69 6e6b 948c  loading...link..
+00001f20: 1065 6d62 6564 5f73 7479 6c65 7368 6565  .embed_styleshee
+00001f30: 7494 898c 1563 6c6f 616b 5f65 6d61 696c  t....cloak_email
+00001f40: 5f61 6464 7265 7373 6573 9488 8c11 7365  _addresses....se
+00001f50: 6374 696f 6e5f 7365 6c66 5f6c 696e 6b94  ction_self_link.
+00001f60: 898c 0365 6e76 944e 7562 8c08 7265 706f  ...env.Nub..repo
+00001f70: 7274 6572 944e 8c10 696e 6469 7265 6374  rter.N..indirect
+00001f80: 5f74 6172 6765 7473 945d 948c 1173 7562  _targets.]...sub
+00001f90: 7374 6974 7574 696f 6e5f 6465 6673 947d  stitution_defs.}
+00001fa0: 9428 8c0f 776f 7264 636f 756e 742d 776f  .(..wordcount-wo
+00001fb0: 7264 7394 6809 8c17 7375 6273 7469 7475  rds.h...substitu
+00001fc0: 7469 6f6e 5f64 6566 696e 6974 696f 6e94  tion_definition.
+00001fd0: 9394 2981 947d 9428 6805 8c03 3136 3994  ..)..}.(h...169.
+00001fe0: 6807 5d94 6816 8c03 3136 3994 8594 8194  h.].h...169.....
+00001ff0: 7d94 681b 6a40 0200 0073 6261 681f 7d94  }.h.j@...sbah.}.
+00002000: 2868 215d 9468 235d 9468 255d 948c 0f77  (h!].h#].h%]...w
+00002010: 6f72 6463 6f75 6e74 2d77 6f72 6473 9461  ordcount-words.a
+00002020: 6827 5d94 6829 5d94 7568 2b6a 3e02 0000  h'].h)].uh+j>...
+00002030: 681d 682c 7562 8c11 776f 7264 636f 756e  h.h,ub..wordcoun
+00002040: 742d 6d69 6e75 7465 7394 6a3f 0200 0029  t-minutes.j?...)
+00002050: 8194 7d94 2868 058c 0131 9468 075d 9468  ..}.(h...1.h.].h
+00002060: 168c 0131 9485 9481 947d 9468 1b6a 5002  ...1.....}.h.jP.
+00002070: 0000 7362 6168 1f7d 9428 6821 5d94 6823  ..sbah.}.(h!].h#
+00002080: 5d94 6825 5d94 8c11 776f 7264 636f 756e  ].h%]...wordcoun
+00002090: 742d 6d69 6e75 7465 7394 6168 275d 9468  t-minutes.ah'].h
+000020a0: 295d 9475 682b 6a3e 0200 0068 1d68 2c75  )].uh+j>...h.h,u
+000020b0: 6275 8c12 7375 6273 7469 7475 7469 6f6e  bu..substitution
+000020c0: 5f6e 616d 6573 947d 9428 8c0f 776f 7264  _names.}.(..word
+000020d0: 636f 756e 742d 776f 7264 7394 6a3d 0200  count-words.j=..
+000020e0: 008c 1177 6f72 6463 6f75 6e74 2d6d 696e  ...wordcount-min
+000020f0: 7574 6573 946a 4f02 0000 758c 0872 6566  utes.jO...u..ref
+00002100: 6e61 6d65 7394 7d94 8c06 7265 6669 6473  names.}...refids
+00002110: 947d 948c 076e 616d 6569 6473 947d 9428  .}...nameids.}.(
+00002120: 6ad7 0100 006a d401 0000 68b9 68b6 6a94  j....j....h.h.j.
+00002130: 0100 006a 9101 0000 6acf 0100 006a cc01  ...j....j....j..
+00002140: 0000 758c 096e 616d 6574 7970 6573 947d  ..u..nametypes.}
+00002150: 9428 6ad7 0100 0089 68b9 896a 9401 0000  .(j.....h..j....
+00002160: 896a cf01 0000 8975 6821 7d94 286a d401  .j.....uh!}.(j..
+00002170: 0000 680c 68b6 682d 6a91 0100 0068 bc6a  ..h.h.h-j....h.j
+00002180: cc01 0000 6a97 0100 0075 8c0d 666f 6f74  ....j....u..foot
+00002190: 6e6f 7465 5f72 6566 7394 7d94 8c0d 6369  note_refs.}...ci
+000021a0: 7461 7469 6f6e 5f72 6566 7394 7d94 8c0d  tation_refs.}...
+000021b0: 6175 746f 666f 6f74 6e6f 7465 7394 5d94  autofootnotes.].
+000021c0: 8c11 6175 746f 666f 6f74 6e6f 7465 5f72  ..autofootnote_r
+000021d0: 6566 7394 5d94 8c10 7379 6d62 6f6c 5f66  efs.]...symbol_f
+000021e0: 6f6f 746e 6f74 6573 945d 948c 1473 796d  ootnotes.]...sym
+000021f0: 626f 6c5f 666f 6f74 6e6f 7465 5f72 6566  bol_footnote_ref
+00002200: 7394 5d94 8c09 666f 6f74 6e6f 7465 7394  s.]...footnotes.
+00002210: 5d94 8c09 6369 7461 7469 6f6e 7394 5d94  ]...citations.].
+00002220: 8c12 6175 746f 666f 6f74 6e6f 7465 5f73  ..autofootnote_s
+00002230: 7461 7274 944b 018c 1573 796d 626f 6c5f  tart.K...symbol_
+00002240: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
+00002250: 008c 0a69 645f 636f 756e 7465 7294 8c0b  ...id_counter...
+00002260: 636f 6c6c 6563 7469 6f6e 7394 8c07 436f  collections...Co
+00002270: 756e 7465 7294 9394 7d94 8594 5294 8c0e  unter...}...R...
+00002280: 7061 7273 655f 6d65 7373 6167 6573 945d  parse_messages.]
+00002290: 948c 1274 7261 6e73 666f 726d 5f6d 6573  ...transform_mes
+000022a0: 7361 6765 7394 5d94 8c0b 7472 616e 7366  sages.]...transf
+000022b0: 6f72 6d65 7294 4e8c 0b69 6e63 6c75 6465  ormer.N..include
+000022c0: 5f6c 6f67 945d 948c 0a64 6563 6f72 6174  _log.]...decorat
+000022d0: 696f 6e94 4e68 1c68 038c 0a6d 7973 745f  ion.Nh.h...myst_
+000022e0: 736c 7567 7394 7d94 7562 2e              slugs.}.ub.
```

### Comparing `mzdata2mat-0.1.1/docs/build/doctrees/mzData.doctree` & `mzdata2mat-0.2.0/docs/build/doctrees/mzDataXMLStruct.doctree`

 * *Files 22% similar despite different names*

```diff
@@ -1,551 +1,411 @@
-00000000: 8005 9564 2200 0000 0000 008c 0f73 7068  ...d"........sph
+00000000: 8005 959f 1900 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
-00000080: 6594 9394 2981 947d 9428 6805 8c06 6d7a  e...)..}.(h...mz
-00000090: 4461 7461 9468 075d 9468 098c 0454 6578  Data.h.].h...Tex
-000000a0: 7494 9394 8c06 6d7a 4461 7461 9485 9481  t.....mzData....
-000000b0: 947d 9428 8c06 7061 7265 6e74 9468 118c  .}.(..parent.h..
-000000c0: 095f 646f 6375 6d65 6e74 9468 038c 0673  ._document.h...s
-000000d0: 6f75 7263 6594 4e8c 046c 696e 6594 4e75  ource.N..line.Nu
-000000e0: 6261 8c0a 6174 7472 6962 7574 6573 947d  ba..attributes.}
-000000f0: 9428 8c03 6964 7394 5d94 8c07 636c 6173  .(..ids.]...clas
-00000100: 7365 7394 5d94 8c05 6e61 6d65 7394 5d94  ses.]...names.].
-00000110: 8c08 6475 706e 616d 6573 945d 948c 0862  ..dupnames.]...b
-00000120: 6163 6b72 6566 7394 5d94 758c 0774 6167  ackrefs.].u..tag
-00000130: 6e61 6d65 9468 0f68 1e4b 0168 1d8c 742f  name.h.h.K.h..t/
-00000140: 5573 6572 732f 6c69 6368 3931 312f 4c69  Users/lich911/Li
-00000150: 6272 6172 792f 436c 6f75 6453 746f 7261  brary/CloudStora
-00000160: 6765 2f4f 6e65 4472 6976 652d 5065 7273  ge/OneDrive-Pers
-00000170: 6f6e 6e65 6c2f 446f 6375 6d65 6e74 732f  onnel/Documents/
-00000180: 5079 7468 6f6e 2f50 6163 6b61 6765 732f  Python/Packages/
-00000190: 6d7a 4461 7461 584d 4c32 4d61 742f 646f  mzDataXML2Mat/do
-000001a0: 6373 2f73 6f75 7263 652f 6d7a 4461 7461  cs/source/mzData
-000001b0: 2e6d 6494 681b 680c 681c 6803 7562 680b  .md.h.h.h.h.ubh.
-000001c0: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
-000001d0: 1029 8194 7d94 2868 058c 0c50 7265 7365  .)..}.(h...Prese
-000001e0: 6e74 6174 696f 6e94 6807 5d94 6816 8c0c  ntation.h.].h...
-000001f0: 5072 6573 656e 7461 7469 6f6e 9485 9481  Presentation....
-00000200: 947d 9428 681b 6830 681c 6803 681d 4e68  .}.(h.h0h.h.h.Nh
-00000210: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00000220: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00000230: 2b68 0f68 1e4b 0368 1d68 2c68 1b68 2d68  +h.h.K.h.h,h.h-h
-00000240: 1c68 0375 6268 098c 0970 6172 6167 7261  .h.ubh...paragra
-00000250: 7068 9493 9429 8194 7d94 2868 0558 0e01  ph...)..}.(h.X..
-00000260: 0000 5468 6973 2069 7320 7468 6520 4261  ..This is the Ba
-00000270: 7365 2063 6c61 7373 2077 6869 6368 2068  se class which h
-00000280: 6f6c 6473 2061 6c6c 2074 6865 2064 6174  olds all the dat
-00000290: 6120 636f 6c6c 6563 7465 6420 6672 6f6d  a collected from
-000002a0: 2061 2067 6976 656e 2060 6d7a 6461 7461   a given `mzdata
-000002b0: 2e78 6d6c 6020 6669 6c65 2e20 5468 6973  .xml` file. This
-000002c0: 2069 7320 7468 6520 6461 7461 2063 6c61   is the data cla
-000002d0: 7373 2075 7365 6420 7768 656e 2074 6865  ss used when the
-000002e0: 2060 6d7a 4461 7461 4d61 6e61 6765 7260   `mzDataManager`
-000002f0: 2063 7265 6174 6573 2061 2060 2e6d 6174   creates a `.mat
-00000300: 6020 6669 6c65 2e3c 6272 3e0a 596f 7520  ` file.<br>.You 
-00000310: 6361 6e20 6372 6561 7465 2079 6f75 7220  can create your 
-00000320: 6f77 6e20 696e 7374 616e 6365 7320 6f66  own instances of
-00000330: 2074 6869 7320 636c 6173 7320 6966 2079   this class if y
-00000340: 6f75 7220 6461 7461 2069 7320 6e6f 7420  our data is not 
-00000350: 636f 6c6c 6563 7465 6420 6672 6f6d 2074  collected from t
-00000360: 6865 206d 7a44 6174 6120 6669 6c65 732e  he mzData files.
-00000370: 9468 075d 9428 6816 8c47 5468 6973 2069  .h.].(h..GThis i
-00000380: 7320 7468 6520 4261 7365 2063 6c61 7373  s the Base class
-00000390: 2077 6869 6368 2068 6f6c 6473 2061 6c6c   which holds all
-000003a0: 2074 6865 2064 6174 6120 636f 6c6c 6563   the data collec
-000003b0: 7465 6420 6672 6f6d 2061 2067 6976 656e  ted from a given
-000003c0: 2094 8594 8194 7d94 2868 1b68 4068 1c68   .....}.(h.h@h.h
-000003d0: 0368 1d4e 681e 4e75 6268 098c 076c 6974  .h.Nh.Nubh...lit
-000003e0: 6572 616c 9493 9429 8194 7d94 2868 058c  eral...)..}.(h..
-000003f0: 0a6d 7a64 6174 612e 786d 6c94 6807 5d94  .mzdata.xml.h.].
-00000400: 6816 8c0a 6d7a 6461 7461 2e78 6d6c 9485  h...mzdata.xml..
-00000410: 9481 947d 9428 681b 684a 681c 6803 681d  ...}.(h.hJh.h.h.
-00000420: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00000430: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00000440: 7568 2b68 4868 1e4b 0468 1d68 2c68 1b68  uh+hHh.K.h.h,h.h
-00000450: 4068 1c68 0375 6268 168c 2c20 6669 6c65  @h.h.ubh.., file
-00000460: 2e20 5468 6973 2069 7320 7468 6520 6461  . This is the da
-00000470: 7461 2063 6c61 7373 2075 7365 6420 7768  ta class used wh
-00000480: 656e 2074 6865 2094 8594 8194 7d94 2868  en the .....}.(h
-00000490: 1b68 4068 1c68 0368 1d4e 681e 4e75 6268  .h@h.h.h.Nh.Nubh
-000004a0: 4929 8194 7d94 2868 058c 0d6d 7a44 6174  I)..}.(h...mzDat
-000004b0: 614d 616e 6167 6572 9468 075d 9468 168c  aManager.h.].h..
-000004c0: 0d6d 7a44 6174 614d 616e 6167 6572 9485  .mzDataManager..
-000004d0: 9481 947d 9428 681b 685c 681c 6803 681d  ...}.(h.h\h.h.h.
-000004e0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-000004f0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00000500: 7568 2b68 4868 1e4b 0468 1d68 2c68 1b68  uh+hHh.K.h.h,h.h
-00000510: 4068 1c68 0375 6268 168c 0b20 6372 6561  @h.h.ubh... crea
-00000520: 7465 7320 6120 9485 9481 947d 9428 681b  tes a .....}.(h.
-00000530: 6840 681c 6803 681d 4e68 1e4e 7562 6849  h@h.h.h.Nh.NubhI
-00000540: 2981 947d 9428 6805 8c04 2e6d 6174 9468  )..}.(h....mat.h
-00000550: 075d 9468 168c 042e 6d61 7494 8594 8194  .].h....mat.....
-00000560: 7d94 2868 1b68 6e68 1c68 0368 1d4e 681e  }.(h.hnh.h.h.Nh.
-00000570: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00000580: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00000590: 6848 681e 4b04 681d 682c 681b 6840 681c  hHh.K.h.h,h.h@h.
-000005a0: 6803 7562 6816 8c06 2066 696c 652e 9485  h.ubh... file...
-000005b0: 9481 947d 9428 681b 6840 681c 6803 681d  ...}.(h.h@h.h.h.
-000005c0: 4e68 1e4e 7562 6809 8c03 7261 7794 9394  Nh.Nubh...raw...
-000005d0: 2981 947d 9428 6805 8c04 3c62 723e 9468  )..}.(h...<br>.h
-000005e0: 075d 9468 168c 043c 6272 3e94 8594 8194  .].h...<br>.....
-000005f0: 7d94 2868 1b68 8268 1c68 0368 1d4e 681e  }.(h.h.h.h.h.Nh.
-00000600: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00000610: 9468 255d 9468 275d 9468 295d 948c 0666  .h%].h'].h)]...f
-00000620: 6f72 6d61 7494 8c04 6874 6d6c 948c 0978  ormat...html...x
-00000630: 6d6c 3a73 7061 6365 948c 0870 7265 7365  ml:space...prese
-00000640: 7276 6594 7568 2b68 8068 1d68 2c68 1e4b  rve.uh+h.h.h,h.K
-00000650: 0468 1b68 4068 1c68 0375 6268 168c 010a  .h.h@h.h.ubh....
-00000660: 9485 9481 947d 9428 681b 6840 681c 6803  .....}.(h.h@h.h.
-00000670: 681d 4e68 1e4e 7562 6816 8c64 596f 7520  h.Nh.Nubh..dYou 
-00000680: 6361 6e20 6372 6561 7465 2079 6f75 7220  can create your 
-00000690: 6f77 6e20 696e 7374 616e 6365 7320 6f66  own instances of
-000006a0: 2074 6869 7320 636c 6173 7320 6966 2079   this class if y
-000006b0: 6f75 7220 6461 7461 2069 7320 6e6f 7420  our data is not 
-000006c0: 636f 6c6c 6563 7465 6420 6672 6f6d 2074  collected from t
-000006d0: 6865 206d 7a44 6174 6120 6669 6c65 732e  he mzData files.
-000006e0: 9485 9481 947d 9428 681b 6840 681c 6803  .....}.(h.h@h.h.
-000006f0: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
-00000700: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00000710: 5d94 7568 2b68 3e68 1e4b 0468 1d68 2c68  ].uh+h>h.K.h.h,h
-00000720: 1b68 2d68 1c68 0375 6265 681f 7d94 2868  .h-h.h.ubeh.}.(h
-00000730: 215d 948c 0c70 7265 7365 6e74 6174 696f  !]...presentatio
-00000740: 6e94 6168 235d 9468 255d 948c 0c70 7265  n.ah#].h%]...pre
-00000750: 7365 6e74 6174 696f 6e94 6168 275d 9468  sentation.ah'].h
-00000760: 295d 9475 682b 680a 681e 4b03 681d 682c  )].uh+h.h.K.h.h,
-00000770: 681b 680c 681c 6803 7562 680b 2981 947d  h.h.h.h.ubh.)..}
-00000780: 9428 6805 6806 6807 5d94 2868 1029 8194  .(h.h.h.].(h.)..
-00000790: 7d94 2868 058c 0a44 6566 696e 6974 696f  }.(h...Definitio
-000007a0: 6e94 6807 5d94 6816 8c0a 4465 6669 6e69  n.h.].h...Defini
-000007b0: 7469 6f6e 9485 9481 947d 9428 681b 68ad  tion.....}.(h.h.
-000007c0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-000007d0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000007e0: 5d94 6829 5d94 7568 2b68 0f68 1e4b 0768  ].h)].uh+h.h.K.h
-000007f0: 1d68 2c68 1b68 aa68 1c68 0375 6268 098c  .h,h.h.h.h.ubh..
-00000800: 0d6c 6974 6572 616c 5f62 6c6f 636b 9493  .literal_block..
-00000810: 9429 8194 7d94 2868 058c d163 6c61 7373  .)..}.(h...class
-00000820: 206d 7a44 6174 6128 4261 7365 4d6f 6465   mzData(BaseMode
-00000830: 6c29 3a0a 2020 2020 6669 6c65 4e61 6d65  l):.    fileName
-00000840: 203a 2073 7472 203d 204e 6f6e 650a 2020   : str = None.  
-00000850: 2020 6669 6c65 5061 7468 203a 2073 7472    filePath : str
-00000860: 203d 204e 6f6e 650a 2020 2020 6d65 7461   = None.    meta
-00000870: 6461 7461 203a 2064 6963 7420 3d20 4e6f  data : dict = No
-00000880: 6e65 0a20 2020 206d 7a20 3a20 6c69 7374  ne.    mz : list
-00000890: 5b6c 6973 745b 666c 6f61 745d 5d20 3d20  [list[float]] = 
-000008a0: 5b5b 5d5d 0a20 2020 2069 6e74 656e 7369  [[]].    intensi
-000008b0: 7469 6573 203a 206c 6973 745b 6c69 7374  ties : list[list
-000008c0: 5b66 6c6f 6174 5d5d 203d 205b 5b5d 5d0a  [float]] = [[]].
-000008d0: 2020 2020 7469 6d65 203a 206c 6973 745b      time : list[
-000008e0: 666c 6f61 745d 203d 205b 5d0a 9468 075d  float] = []..h.]
-000008f0: 9468 168c d163 6c61 7373 206d 7a44 6174  .h...class mzDat
-00000900: 6128 4261 7365 4d6f 6465 6c29 3a0a 2020  a(BaseModel):.  
-00000910: 2020 6669 6c65 4e61 6d65 203a 2073 7472    fileName : str
-00000920: 203d 204e 6f6e 650a 2020 2020 6669 6c65   = None.    file
-00000930: 5061 7468 203a 2073 7472 203d 204e 6f6e  Path : str = Non
-00000940: 650a 2020 2020 6d65 7461 6461 7461 203a  e.    metadata :
-00000950: 2064 6963 7420 3d20 4e6f 6e65 0a20 2020   dict = None.   
-00000960: 206d 7a20 3a20 6c69 7374 5b6c 6973 745b   mz : list[list[
-00000970: 666c 6f61 745d 5d20 3d20 5b5b 5d5d 0a20  float]] = [[]]. 
-00000980: 2020 2069 6e74 656e 7369 7469 6573 203a     intensities :
-00000990: 206c 6973 745b 6c69 7374 5b66 6c6f 6174   list[list[float
-000009a0: 5d5d 203d 205b 5b5d 5d0a 2020 2020 7469  ]] = [[]].    ti
-000009b0: 6d65 203a 206c 6973 745b 666c 6f61 745d  me : list[float]
-000009c0: 203d 205b 5d0a 9485 9481 947d 9468 1b68   = []......}.h.h
-000009d0: bd73 6261 681f 7d94 2868 215d 9468 235d  .sbah.}.(h!].h#]
-000009e0: 9468 255d 9468 275d 9468 295d 948c 086c  .h%].h'].h)]...l
-000009f0: 616e 6775 6167 6594 8c06 7079 7468 6f6e  anguage...python
-00000a00: 9468 9268 9375 682b 68bb 681d 682c 681e  .h.h.uh+h.h.h,h.
-00000a10: 4b08 681b 68aa 681c 6803 7562 6568 1f7d  K.h.h.h.h.ubeh.}
-00000a20: 9428 6821 5d94 8c0a 6465 6669 6e69 7469  .(h!]...definiti
-00000a30: 6f6e 9461 6823 5d94 6825 5d94 8c0a 6465  on.ah#].h%]...de
-00000a40: 6669 6e69 7469 6f6e 9461 6827 5d94 6829  finition.ah'].h)
-00000a50: 5d94 7568 2b68 0a68 1e4b 0768 1d68 2c68  ].uh+h.h.K.h.h,h
-00000a60: 1b68 0c68 1c68 0375 6268 0b29 8194 7d94  .h.h.h.ubh.)..}.
-00000a70: 2868 0568 0668 075d 9428 6810 2981 947d  (h.h.h.].(h.)..}
-00000a80: 9428 6805 8c0a 486f 7720 746f 2075 7365  .(h...How to use
-00000a90: 9468 075d 9468 168c 0a48 6f77 2074 6f20  .h.].h...How to 
-00000aa0: 7573 6594 8594 8194 7d94 2868 1b68 d868  use.....}.(h.h.h
-00000ab0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-00000ac0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00000ad0: 9468 295d 9475 682b 680f 681e 4b12 681d  .h)].uh+h.h.K.h.
-00000ae0: 682c 681b 68d5 681c 6803 7562 683f 2981  h,h.h.h.h.ubh?).
-00000af0: 947d 9428 6805 8c4b 5468 6572 6520 6172  .}.(h..KThere ar
-00000b00: 6520 7477 6f20 7761 7973 206f 6620 6372  e two ways of cr
-00000b10: 6561 7469 6e67 2074 6869 7320 636c 6173  eating this clas
-00000b20: 732c 2074 6865 2066 6972 7374 206f 6e65  s, the first one
-00000b30: 2069 7320 7468 6520 666f 6c6c 6f77 696e   is the followin
-00000b40: 6720 3a94 6807 5d94 6816 8c4b 5468 6572  g :.h.].h..KTher
-00000b50: 6520 6172 6520 7477 6f20 7761 7973 206f  e are two ways o
-00000b60: 6620 6372 6561 7469 6e67 2074 6869 7320  f creating this 
-00000b70: 636c 6173 732c 2074 6865 2066 6972 7374  class, the first
-00000b80: 206f 6e65 2069 7320 7468 6520 666f 6c6c   one is the foll
-00000b90: 6f77 696e 6720 3a94 8594 8194 7d94 2868  owing :.....}.(h
-00000ba0: 1b68 e668 1c68 0368 1d4e 681e 4e75 6261  .h.h.h.h.Nh.Nuba
-00000bb0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00000bc0: 9468 275d 9468 295d 9475 682b 683e 681e  .h'].h)].uh+h>h.
-00000bd0: 4b13 681d 682c 681b 68d5 681c 6803 7562  K.h.h,h.h.h.h.ub
-00000be0: 68bc 2981 947d 9428 6805 58c2 0100 0023  h.)..}.(h.X....#
-00000bf0: 2043 6c61 7373 2063 7265 6174 696f 6e0a   Class creation.
-00000c00: 6461 7461 203d 206d 7a44 6174 6128 290a  data = mzData().
-00000c10: 0a23 2054 6865 2073 6372 6970 7420 6265  .# The script be
-00000c20: 6c6f 7720 636f 756c 6420 6265 2063 616c  low could be cal
-00000c30: 6c65 6420 616e 7977 6865 7265 2079 6f75  led anywhere you
-00000c40: 2077 616e 742c 206a 7573 7420 6265 2073   want, just be s
-00000c50: 7572 6520 746f 2066 696c 6c20 616c 6c20  ure to fill all 
-00000c60: 6e65 6365 7373 6172 7920 6461 7461 2062  necessary data b
-00000c70: 6566 6f72 6520 6361 6c6c 696e 6720 7468  efore calling th
-00000c80: 6520 7361 7665 4d61 7466 696c 6520 6675  e saveMatfile fu
-00000c90: 6e63 7469 6f6e 2066 726f 6d20 7468 6520  nction from the 
-00000ca0: 6d7a 6461 7461 4d61 6e61 6765 7220 636c  mzdataManager cl
-00000cb0: 6173 732e 0a64 6174 612e 6669 6c65 4e61  ass..data.fileNa
-00000cc0: 6d65 203d 2022 7361 6d70 6c65 2e6d 7a64  me = "sample.mzd
-00000cd0: 6174 612e 786d 6c22 0a64 6174 612e 6669  ata.xml".data.fi
-00000ce0: 6c65 5061 7468 203d 2022 736f 6d65 2f70  lePath = "some/p
-00000cf0: 6174 682f 220a 6461 7461 2e6d 6574 6164  ath/".data.metad
-00000d00: 6174 6120 3d20 7b0a 2020 2020 2773 6f66  ata = {.    'sof
-00000d10: 7477 6172 6527 203a 2027 736f 6d65 536f  tware' : 'someSo
-00000d20: 6674 7761 7265 272c 0a20 2020 2027 616e  ftware',.    'an
-00000d30: 616c 7973 6572 2720 3a20 274a 6f68 6e20  alyser' : 'John 
-00000d40: 446f 6527 2c0a 2020 2020 2764 6574 6563  Doe',.    'detec
-00000d50: 746f 7227 203a 2027 736f 6d65 4465 7465  tor' : 'someDete
-00000d60: 6374 6f72 270a 7d0a 6461 7461 2e6d 7a20  ctor'.}.data.mz 
-00000d70: 3d20 6d7a 4c69 7374 0a64 6174 612e 696e  = mzList.data.in
-00000d80: 7465 6e73 6974 6965 7320 3d20 696e 7465  tensities = inte
-00000d90: 6e73 6974 6965 734c 6973 740a 6461 7461  nsitiesList.data
-00000da0: 2e74 696d 6520 3d20 7469 6d65 4c69 7374  .time = timeList
-00000db0: 0a94 6807 5d94 6816 58c2 0100 0023 2043  ..h.].h.X....# C
-00000dc0: 6c61 7373 2063 7265 6174 696f 6e0a 6461  lass creation.da
-00000dd0: 7461 203d 206d 7a44 6174 6128 290a 0a23  ta = mzData()..#
-00000de0: 2054 6865 2073 6372 6970 7420 6265 6c6f   The script belo
-00000df0: 7720 636f 756c 6420 6265 2063 616c 6c65  w could be calle
-00000e00: 6420 616e 7977 6865 7265 2079 6f75 2077  d anywhere you w
-00000e10: 616e 742c 206a 7573 7420 6265 2073 7572  ant, just be sur
-00000e20: 6520 746f 2066 696c 6c20 616c 6c20 6e65  e to fill all ne
-00000e30: 6365 7373 6172 7920 6461 7461 2062 6566  cessary data bef
-00000e40: 6f72 6520 6361 6c6c 696e 6720 7468 6520  ore calling the 
-00000e50: 7361 7665 4d61 7466 696c 6520 6675 6e63  saveMatfile func
-00000e60: 7469 6f6e 2066 726f 6d20 7468 6520 6d7a  tion from the mz
-00000e70: 6461 7461 4d61 6e61 6765 7220 636c 6173  dataManager clas
-00000e80: 732e 0a64 6174 612e 6669 6c65 4e61 6d65  s..data.fileName
-00000e90: 203d 2022 7361 6d70 6c65 2e6d 7a64 6174   = "sample.mzdat
-00000ea0: 612e 786d 6c22 0a64 6174 612e 6669 6c65  a.xml".data.file
-00000eb0: 5061 7468 203d 2022 736f 6d65 2f70 6174  Path = "some/pat
-00000ec0: 682f 220a 6461 7461 2e6d 6574 6164 6174  h/".data.metadat
-00000ed0: 6120 3d20 7b0a 2020 2020 2773 6f66 7477  a = {.    'softw
-00000ee0: 6172 6527 203a 2027 736f 6d65 536f 6674  are' : 'someSoft
-00000ef0: 7761 7265 272c 0a20 2020 2027 616e 616c  ware',.    'anal
-00000f00: 7973 6572 2720 3a20 274a 6f68 6e20 446f  yser' : 'John Do
-00000f10: 6527 2c0a 2020 2020 2764 6574 6563 746f  e',.    'detecto
-00000f20: 7227 203a 2027 736f 6d65 4465 7465 6374  r' : 'someDetect
-00000f30: 6f72 270a 7d0a 6461 7461 2e6d 7a20 3d20  or'.}.data.mz = 
-00000f40: 6d7a 4c69 7374 0a64 6174 612e 696e 7465  mzList.data.inte
-00000f50: 6e73 6974 6965 7320 3d20 696e 7465 6e73  nsities = intens
-00000f60: 6974 6965 734c 6973 740a 6461 7461 2e74  itiesList.data.t
-00000f70: 696d 6520 3d20 7469 6d65 4c69 7374 0a94  ime = timeList..
-00000f80: 8594 8194 7d94 681b 68f4 7362 6168 1f7d  ....}.h.h.sbah.}
-00000f90: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00000fa0: 5d94 6829 5d94 8c08 6c61 6e67 7561 6765  ].h)]...language
-00000fb0: 948c 0670 7974 686f 6e94 6892 6893 7568  ...python.h.h.uh
-00000fc0: 2b68 bb68 1d68 2c68 1e4b 1468 1b68 d568  +h.h.h,h.K.h.h.h
-00000fd0: 1c68 0375 6268 3f29 8194 7d94 2868 058c  .h.ubh?)..}.(h..
-00000fe0: 6349 6620 796f 7520 6861 7665 2061 6c6c  cIf you have all
-00000ff0: 2069 6e66 6f72 6d61 7469 6f6e 7320 6174   informations at
-00001000: 2074 6865 2073 616d 6520 7469 6d65 2c20   the same time, 
-00001010: 796f 7520 636f 756c 6420 7573 6520 7468  you could use th
-00001020: 6520 7365 636f 6e64 2077 6179 206f 6620  e second way of 
-00001030: 6465 6669 6e69 6e67 2074 6865 2063 6c61  defining the cla
-00001040: 7373 203a 9468 075d 9468 168c 6349 6620  ss :.h.].h..cIf 
-00001050: 796f 7520 6861 7665 2061 6c6c 2069 6e66  you have all inf
-00001060: 6f72 6d61 7469 6f6e 7320 6174 2074 6865  ormations at the
-00001070: 2073 616d 6520 7469 6d65 2c20 796f 7520   same time, you 
-00001080: 636f 756c 6420 7573 6520 7468 6520 7365  could use the se
-00001090: 636f 6e64 2077 6179 206f 6620 6465 6669  cond way of defi
-000010a0: 6e69 6e67 2074 6865 2063 6c61 7373 203a  ning the class :
-000010b0: 9485 9481 947d 9428 681b 6a04 0100 0068  .....}.(h.j....h
-000010c0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-000010d0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-000010e0: 9468 295d 9475 682b 683e 681e 4b24 681d  .h)].uh+h>h.K$h.
-000010f0: 682c 681b 68d5 681c 6803 7562 68bc 2981  h,h.h.h.h.ubh.).
-00001100: 947d 9428 6805 5810 0100 0064 6174 6120  .}.(h.X....data 
-00001110: 3d20 6d7a 4461 7461 280a 2020 2020 6669  = mzData(.    fi
-00001120: 6c65 4e61 6d65 203d 2022 7361 6d70 6c65  leName = "sample
-00001130: 2e6d 7a64 6174 612e 786d 6c22 2c0a 2020  .mzdata.xml",.  
-00001140: 2020 6669 6c65 5061 7468 203d 2022 736f    filePath = "so
-00001150: 6d65 2f70 6174 682f 222c 0a20 2020 206d  me/path/",.    m
-00001160: 6574 6164 6174 6120 3d20 7b0a 2020 2020  etadata = {.    
-00001170: 2773 6f66 7477 6172 6527 203a 2027 736f  'software' : 'so
-00001180: 6d65 536f 6674 7761 7265 272c 0a20 2020  meSoftware',.   
-00001190: 2027 616e 616c 7973 6572 2720 3a20 274a   'analyser' : 'J
-000011a0: 6f68 6e20 446f 6527 2c0a 2020 2020 2764  ohn Doe',.    'd
-000011b0: 6574 6563 746f 7227 203a 2027 736f 6d65  etector' : 'some
-000011c0: 4465 7465 6374 6f72 270a 2020 2020 7d2c  Detector'.    },
-000011d0: 0a20 2020 206d 7a20 3d20 6d7a 4c69 7374  .    mz = mzList
-000011e0: 2c0a 2020 2020 696e 7465 6e73 6974 6965  ,.    intensitie
-000011f0: 7320 3d20 696e 7465 6e73 6974 6965 734c  s = intensitiesL
-00001200: 6973 742c 0a20 2020 2074 696d 6520 3d20  ist,.    time = 
-00001210: 7469 6d65 4c69 7374 0a29 0a94 6807 5d94  timeList.)..h.].
-00001220: 6816 5810 0100 0064 6174 6120 3d20 6d7a  h.X....data = mz
-00001230: 4461 7461 280a 2020 2020 6669 6c65 4e61  Data(.    fileNa
-00001240: 6d65 203d 2022 7361 6d70 6c65 2e6d 7a64  me = "sample.mzd
-00001250: 6174 612e 786d 6c22 2c0a 2020 2020 6669  ata.xml",.    fi
-00001260: 6c65 5061 7468 203d 2022 736f 6d65 2f70  lePath = "some/p
-00001270: 6174 682f 222c 0a20 2020 206d 6574 6164  ath/",.    metad
-00001280: 6174 6120 3d20 7b0a 2020 2020 2773 6f66  ata = {.    'sof
-00001290: 7477 6172 6527 203a 2027 736f 6d65 536f  tware' : 'someSo
-000012a0: 6674 7761 7265 272c 0a20 2020 2027 616e  ftware',.    'an
-000012b0: 616c 7973 6572 2720 3a20 274a 6f68 6e20  alyser' : 'John 
-000012c0: 446f 6527 2c0a 2020 2020 2764 6574 6563  Doe',.    'detec
-000012d0: 746f 7227 203a 2027 736f 6d65 4465 7465  tor' : 'someDete
-000012e0: 6374 6f72 270a 2020 2020 7d2c 0a20 2020  ctor'.    },.   
-000012f0: 206d 7a20 3d20 6d7a 4c69 7374 2c0a 2020   mz = mzList,.  
-00001300: 2020 696e 7465 6e73 6974 6965 7320 3d20    intensities = 
-00001310: 696e 7465 6e73 6974 6965 734c 6973 742c  intensitiesList,
-00001320: 0a20 2020 2074 696d 6520 3d20 7469 6d65  .    time = time
-00001330: 4c69 7374 0a29 0a94 8594 8194 7d94 681b  List.)......}.h.
-00001340: 6a12 0100 0073 6261 681f 7d94 2868 215d  j....sbah.}.(h!]
-00001350: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001360: 948c 086c 616e 6775 6167 6594 8c06 7079  ...language...py
-00001370: 7468 6f6e 9468 9268 9375 682b 68bb 681d  thon.h.h.uh+h.h.
-00001380: 682c 681e 4b25 681b 68d5 681c 6803 7562  h,h.K%h.h.h.h.ub
-00001390: 6568 1f7d 9428 6821 5d94 8c0a 686f 772d  eh.}.(h!]...how-
-000013a0: 746f 2d75 7365 9461 6823 5d94 6825 5d94  to-use.ah#].h%].
-000013b0: 8c0a 686f 7720 746f 2075 7365 9461 6827  ..how to use.ah'
-000013c0: 5d94 6829 5d94 7568 2b68 0a68 1e4b 1268  ].h)].uh+h.h.K.h
-000013d0: 1d68 2c68 1b68 0c68 1c68 0375 6268 0b29  .h,h.h.h.h.ubh.)
-000013e0: 8194 7d94 2868 0568 0668 075d 9428 6810  ..}.(h.h.h.].(h.
-000013f0: 2981 947d 9428 6805 8c09 4675 6e63 7469  )..}.(h...Functi
-00001400: 6f6e 7394 6807 5d94 6816 8c09 4675 6e63  ons.h.].h...Func
-00001410: 7469 6f6e 7394 8594 8194 7d94 2868 1b6a  tions.....}.(h.j
-00001420: 2d01 0000 681c 6803 681d 4e68 1e4e 7562  -...h.h.h.Nh.Nub
-00001430: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00001440: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
-00001450: 1e4b 3468 1d68 2c68 1b6a 2a01 0000 681c  .K4h.h,h.j*...h.
-00001460: 6803 7562 683f 2981 947d 9428 6805 8c04  h.ubh?)..}.(h...
-00001470: 4e6f 6e65 9468 075d 9468 168c 044e 6f6e  None.h.].h...Non
-00001480: 6594 8594 8194 7d94 2868 1b6a 3b01 0000  e.....}.(h.j;...
-00001490: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-000014a0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000014b0: 5d94 6829 5d94 7568 2b68 3e68 1e4b 3568  ].h)].uh+h>h.K5h
-000014c0: 1d68 2c68 1b6a 2a01 0000 681c 6803 7562  .h,h.j*...h.h.ub
-000014d0: 6568 1f7d 9428 6821 5d94 8c09 6675 6e63  eh.}.(h!]...func
-000014e0: 7469 6f6e 7394 6168 235d 9468 255d 948c  tions.ah#].h%]..
-000014f0: 0966 756e 6374 696f 6e73 9461 6827 5d94  .functions.ah'].
-00001500: 6829 5d94 7568 2b68 0a68 1e4b 3468 1d68  h)].uh+h.h.K4h.h
-00001510: 2c68 1b68 0c68 1c68 0375 6268 0b29 8194  ,h.h.h.h.ubh.)..
-00001520: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
-00001530: 947d 9428 6805 8c05 4e6f 7465 7394 6807  .}.(h...Notes.h.
-00001540: 5d94 6816 8c05 4e6f 7465 7394 8594 8194  ].h...Notes.....
-00001550: 7d94 2868 1b6a 5401 0000 681c 6803 681d  }.(h.jT...h.h.h.
-00001560: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00001570: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00001580: 7568 2b68 0f68 1e4b 3768 1d68 2c68 1b6a  uh+h.h.K7h.h,h.j
-00001590: 5101 0000 681c 6803 7562 683f 2981 947d  Q...h.h.ubh?)..}
-000015a0: 9428 6805 8cbd 5468 6572 6520 6973 2069  .(h...There is i
-000015b0: 6e20 6661 6374 2061 2066 756e 6374 696f  n fact a functio
-000015c0: 6e20 6361 6c6c 6564 2060 746f 4469 6374  n called `toDict
-000015d0: 602c 2062 7574 2069 7420 6973 2069 6e74  `, but it is int
-000015e0: 656e 6465 6420 746f 2062 6520 7573 6564  ended to be used
-000015f0: 2062 7920 7468 6520 6d61 6e61 6765 7220   by the manager 
-00001600: 636c 6173 732e 2054 6865 206f 6e6c 7920  class. The only 
-00001610: 7468 696e 6720 6974 2064 6f65 7320 6973  thing it does is
-00001620: 2063 6f6e 7665 7274 2074 6865 2073 7472   convert the str
-00001630: 7563 7475 7265 2069 6e74 6f20 7468 6520  ucture into the 
-00001640: 666f 726d 6174 206e 6565 6465 6420 6279  format needed by
-00001650: 2074 6865 2060 2e6d 6174 6020 666f 726d   the `.mat` form
-00001660: 6174 2e94 6807 5d94 2868 168c 2354 6865  at..h.].(h..#The
-00001670: 7265 2069 7320 696e 2066 6163 7420 6120  re is in fact a 
-00001680: 6675 6e63 7469 6f6e 2063 616c 6c65 6420  function called 
-00001690: 9485 9481 947d 9428 681b 6a62 0100 0068  .....}.(h.jb...h
-000016a0: 1c68 0368 1d4e 681e 4e75 6268 4929 8194  .h.h.Nh.NubhI)..
-000016b0: 7d94 2868 058c 0674 6f44 6963 7494 6807  }.(h...toDict.h.
-000016c0: 5d94 6816 8c06 746f 4469 6374 9485 9481  ].h...toDict....
-000016d0: 947d 9428 681b 6a6a 0100 0068 1c68 0368  .}.(h.jj...h.h.h
-000016e0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000016f0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001700: 9475 682b 6848 681e 4b38 681d 682c 681b  .uh+hHh.K8h.h,h.
-00001710: 6a62 0100 0068 1c68 0375 6268 168c 842c  jb...h.h.ubh...,
-00001720: 2062 7574 2069 7420 6973 2069 6e74 656e   but it is inten
-00001730: 6465 6420 746f 2062 6520 7573 6564 2062  ded to be used b
-00001740: 7920 7468 6520 6d61 6e61 6765 7220 636c  y the manager cl
-00001750: 6173 732e 2054 6865 206f 6e6c 7920 7468  ass. The only th
-00001760: 696e 6720 6974 2064 6f65 7320 6973 2063  ing it does is c
-00001770: 6f6e 7665 7274 2074 6865 2073 7472 7563  onvert the struc
-00001780: 7475 7265 2069 6e74 6f20 7468 6520 666f  ture into the fo
-00001790: 726d 6174 206e 6565 6465 6420 6279 2074  rmat needed by t
-000017a0: 6865 2094 8594 8194 7d94 2868 1b6a 6201  he .....}.(h.jb.
-000017b0: 0000 681c 6803 681d 4e68 1e4e 7562 6849  ..h.h.h.Nh.NubhI
-000017c0: 2981 947d 9428 6805 8c04 2e6d 6174 9468  )..}.(h....mat.h
-000017d0: 075d 9468 168c 042e 6d61 7494 8594 8194  .].h....mat.....
-000017e0: 7d94 2868 1b6a 7c01 0000 681c 6803 681d  }.(h.j|...h.h.h.
-000017f0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00001800: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00001810: 7568 2b68 4868 1e4b 3868 1d68 2c68 1b6a  uh+hHh.K8h.h,h.j
-00001820: 6201 0000 681c 6803 7562 6816 8c08 2066  b...h.h.ubh... f
-00001830: 6f72 6d61 742e 9485 9481 947d 9428 681b  ormat......}.(h.
-00001840: 6a62 0100 0068 1c68 0368 1d4e 681e 4e75  jb...h.h.h.Nh.Nu
-00001850: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-00001860: 255d 9468 275d 9468 295d 9475 682b 683e  %].h'].h)].uh+h>
-00001870: 681e 4b38 681d 682c 681b 6a51 0100 0068  h.K8h.h,h.jQ...h
-00001880: 1c68 0375 6265 681f 7d94 2868 215d 948c  .h.ubeh.}.(h!]..
-00001890: 056e 6f74 6573 9461 6823 5d94 6825 5d94  .notes.ah#].h%].
-000018a0: 8c05 6e6f 7465 7394 6168 275d 9468 295d  ..notes.ah'].h)]
-000018b0: 9475 682b 680a 681e 4b37 681d 682c 681b  .uh+h.h.K7h.h,h.
-000018c0: 680c 681c 6803 7562 6568 1f7d 9428 6821  h.h.h.ubeh.}.(h!
-000018d0: 5d94 8c06 6d7a 6461 7461 9461 6823 5d94  ]...mzdata.ah#].
-000018e0: 6825 5d94 8c06 6d7a 6461 7461 9461 6827  h%]...mzdata.ah'
-000018f0: 5d94 6829 5d94 7568 2b68 0a68 1e4b 0168  ].h)].uh+h.h.K.h
-00001900: 1d68 2c68 1b68 0368 1c68 0375 6261 681f  .h,h.h.h.h.ubah.
-00001910: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00001920: 275d 9468 295d 948c 0673 6f75 7263 6594  '].h)]...source.
-00001930: 682c 8c14 7472 616e 736c 6174 696f 6e5f  h,..translation_
-00001940: 7072 6f67 7265 7373 947d 9428 8c05 746f  progress.}.(..to
-00001950: 7461 6c94 4b00 8c0a 7472 616e 736c 6174  tal.K...translat
-00001960: 6564 944b 0075 7568 2b68 018c 0e63 7572  ed.K.uuh+h...cur
-00001970: 7265 6e74 5f73 6f75 7263 6594 4e8c 0c63  rent_source.N..c
-00001980: 7572 7265 6e74 5f6c 696e 6594 4e8c 0873  urrent_line.N..s
-00001990: 6574 7469 6e67 7394 8c11 646f 6375 7469  ettings...docuti
-000019a0: 6c73 2e66 726f 6e74 656e 6494 8c06 5661  ls.frontend...Va
-000019b0: 6c75 6573 9493 9429 8194 7d94 2868 0f4e  lues...)..}.(h.N
-000019c0: 8c09 6765 6e65 7261 746f 7294 4e8c 0964  ..generator.N..d
-000019d0: 6174 6573 7461 6d70 944e 8c0b 736f 7572  atestamp.N..sour
-000019e0: 6365 5f6c 696e 6b94 4e8c 0a73 6f75 7263  ce_link.N..sourc
-000019f0: 655f 7572 6c94 4e8c 0d74 6f63 5f62 6163  e_url.N..toc_bac
-00001a00: 6b6c 696e 6b73 948c 0565 6e74 7279 948c  klinks...entry..
-00001a10: 1266 6f6f 746e 6f74 655f 6261 636b 6c69  .footnote_backli
-00001a20: 6e6b 7394 4b01 8c0d 7365 6374 6e75 6d5f  nks.K...sectnum_
-00001a30: 7866 6f72 6d94 4b01 8c0e 7374 7269 705f  xform.K...strip_
-00001a40: 636f 6d6d 656e 7473 944e 8c1b 7374 7269  comments.N..stri
-00001a50: 705f 656c 656d 656e 7473 5f77 6974 685f  p_elements_with_
-00001a60: 636c 6173 7365 7394 4e8c 0d73 7472 6970  classes.N..strip
-00001a70: 5f63 6c61 7373 6573 944e 8c0c 7265 706f  _classes.N..repo
-00001a80: 7274 5f6c 6576 656c 944b 028c 0a68 616c  rt_level.K...hal
-00001a90: 745f 6c65 7665 6c94 4b05 8c11 6578 6974  t_level.K...exit
-00001aa0: 5f73 7461 7475 735f 6c65 7665 6c94 4b05  _status_level.K.
-00001ab0: 8c05 6465 6275 6794 4e8c 0e77 6172 6e69  ..debug.N..warni
-00001ac0: 6e67 5f73 7472 6561 6d94 4e8c 0974 7261  ng_stream.N..tra
-00001ad0: 6365 6261 636b 9488 8c0e 696e 7075 745f  ceback....input_
-00001ae0: 656e 636f 6469 6e67 948c 0975 7466 2d38  encoding...utf-8
-00001af0: 2d73 6967 948c 1c69 6e70 7574 5f65 6e63  -sig...input_enc
-00001b00: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-00001b10: 6c65 7294 8c06 7374 7269 6374 948c 0f6f  ler...strict...o
-00001b20: 7574 7075 745f 656e 636f 6469 6e67 948c  utput_encoding..
-00001b30: 0575 7466 2d38 948c 1d6f 7574 7075 745f  .utf-8...output_
-00001b40: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
-00001b50: 616e 646c 6572 946a cb01 0000 8c0e 6572  andler.j......er
-00001b60: 726f 725f 656e 636f 6469 6e67 948c 0575  ror_encoding...u
-00001b70: 7466 2d38 948c 1c65 7272 6f72 5f65 6e63  tf-8...error_enc
-00001b80: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-00001b90: 6c65 7294 8c10 6261 636b 736c 6173 6872  ler...backslashr
-00001ba0: 6570 6c61 6365 948c 0d6c 616e 6775 6167  eplace...languag
-00001bb0: 655f 636f 6465 948c 0265 6e94 8c13 7265  e_code...en...re
-00001bc0: 636f 7264 5f64 6570 656e 6465 6e63 6965  cord_dependencie
-00001bd0: 7394 4e8c 0663 6f6e 6669 6794 4e8c 0969  s.N..config.N..i
-00001be0: 645f 7072 6566 6978 9468 068c 0e61 7574  d_prefix.h...aut
-00001bf0: 6f5f 6964 5f70 7265 6669 7894 8c02 6964  o_id_prefix...id
-00001c00: 948c 0d64 756d 705f 7365 7474 696e 6773  ...dump_settings
-00001c10: 944e 8c0e 6475 6d70 5f69 6e74 6572 6e61  .N..dump_interna
-00001c20: 6c73 944e 8c0f 6475 6d70 5f74 7261 6e73  ls.N..dump_trans
-00001c30: 666f 726d 7394 4e8c 0f64 756d 705f 7073  forms.N..dump_ps
-00001c40: 6575 646f 5f78 6d6c 944e 8c10 6578 706f  eudo_xml.N..expo
-00001c50: 7365 5f69 6e74 6572 6e61 6c73 944e 8c0e  se_internals.N..
-00001c60: 7374 7269 6374 5f76 6973 6974 6f72 944e  strict_visitor.N
-00001c70: 8c0f 5f64 6973 6162 6c65 5f63 6f6e 6669  .._disable_confi
-00001c80: 6794 4e8c 075f 736f 7572 6365 9468 2c8c  g.N.._source.h,.
-00001c90: 0c5f 6465 7374 696e 6174 696f 6e94 4e8c  ._destination.N.
-00001ca0: 0d5f 636f 6e66 6967 5f66 696c 6573 945d  ._config_files.]
-00001cb0: 948c 1666 696c 655f 696e 7365 7274 696f  ...file_insertio
-00001cc0: 6e5f 656e 6162 6c65 6494 888c 0b72 6177  n_enabled....raw
-00001cd0: 5f65 6e61 626c 6564 944b 018c 116c 696e  _enabled.K...lin
-00001ce0: 655f 6c65 6e67 7468 5f6c 696d 6974 944d  e_length_limit.M
-00001cf0: 1027 8c0e 7065 705f 7265 6665 7265 6e63  .'..pep_referenc
-00001d00: 6573 944e 8c0c 7065 705f 6261 7365 5f75  es.N..pep_base_u
-00001d10: 726c 948c 1868 7474 7073 3a2f 2f70 6570  rl...https://pep
-00001d20: 732e 7079 7468 6f6e 2e6f 7267 2f94 8c15  s.python.org/...
-00001d30: 7065 705f 6669 6c65 5f75 726c 5f74 656d  pep_file_url_tem
-00001d40: 706c 6174 6594 8c08 7065 702d 2530 3464  plate...pep-%04d
-00001d50: 948c 0e72 6663 5f72 6566 6572 656e 6365  ...rfc_reference
-00001d60: 7394 4e8c 0c72 6663 5f62 6173 655f 7572  s.N..rfc_base_ur
-00001d70: 6c94 8c26 6874 7470 733a 2f2f 6461 7461  l..&https://data
-00001d80: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
-00001d90: 2f64 6f63 2f68 746d 6c2f 948c 0974 6162  /doc/html/...tab
-00001da0: 5f77 6964 7468 944b 088c 1d74 7269 6d5f  _width.K...trim_
-00001db0: 666f 6f74 6e6f 7465 5f72 6566 6572 656e  footnote_referen
-00001dc0: 6365 5f73 7061 6365 9489 8c10 7379 6e74  ce_space....synt
-00001dd0: 6178 5f68 6967 686c 6967 6874 948c 046c  ax_highlight...l
-00001de0: 6f6e 6794 8c0c 736d 6172 745f 7175 6f74  ong...smart_quot
-00001df0: 6573 9488 8c13 736d 6172 7471 756f 7465  es....smartquote
-00001e00: 735f 6c6f 6361 6c65 7394 5d94 8c1d 6368  s_locales.]...ch
-00001e10: 6172 6163 7465 725f 6c65 7665 6c5f 696e  aracter_level_in
-00001e20: 6c69 6e65 5f6d 6172 6b75 7094 898c 0e64  line_markup....d
-00001e30: 6f63 7469 746c 655f 7866 6f72 6d94 898c  octitle_xform...
-00001e40: 0d64 6f63 696e 666f 5f78 666f 726d 944b  .docinfo_xform.K
-00001e50: 018c 1273 6563 7473 7562 7469 746c 655f  ...sectsubtitle_
-00001e60: 7866 6f72 6d94 898c 0d69 6d61 6765 5f6c  xform....image_l
-00001e70: 6f61 6469 6e67 948c 046c 696e 6b94 8c10  oading...link...
-00001e80: 656d 6265 645f 7374 796c 6573 6865 6574  embed_stylesheet
-00001e90: 9489 8c15 636c 6f61 6b5f 656d 6169 6c5f  ....cloak_email_
-00001ea0: 6164 6472 6573 7365 7394 888c 1173 6563  addresses....sec
-00001eb0: 7469 6f6e 5f73 656c 665f 6c69 6e6b 9489  tion_self_link..
-00001ec0: 8c03 656e 7694 4e75 628c 0872 6570 6f72  ..env.Nub..repor
-00001ed0: 7465 7294 4e8c 1069 6e64 6972 6563 745f  ter.N..indirect_
-00001ee0: 7461 7267 6574 7394 5d94 8c11 7375 6273  targets.]...subs
-00001ef0: 7469 7475 7469 6f6e 5f64 6566 7394 7d94  titution_defs.}.
-00001f00: 288c 0f77 6f72 6463 6f75 6e74 2d77 6f72  (..wordcount-wor
-00001f10: 6473 9468 098c 1773 7562 7374 6974 7574  ds.h...substitut
-00001f20: 696f 6e5f 6465 6669 6e69 7469 6f6e 9493  ion_definition..
-00001f30: 9429 8194 7d94 2868 058c 0331 3231 9468  .)..}.(h...121.h
-00001f40: 075d 9468 168c 0331 3231 9485 9481 947d  .].h...121.....}
-00001f50: 9468 1b6a 0902 0000 7362 6168 1f7d 9428  .h.j....sbah.}.(
-00001f60: 6821 5d94 6823 5d94 6825 5d94 8c0f 776f  h!].h#].h%]...wo
-00001f70: 7264 636f 756e 742d 776f 7264 7394 6168  rdcount-words.ah
-00001f80: 275d 9468 295d 9475 682b 6a07 0200 0068  '].h)].uh+j....h
-00001f90: 1d68 2c75 628c 1177 6f72 6463 6f75 6e74  .h,ub..wordcount
-00001fa0: 2d6d 696e 7574 6573 946a 0802 0000 2981  -minutes.j....).
-00001fb0: 947d 9428 6805 8c01 3194 6807 5d94 6816  .}.(h...1.h.].h.
-00001fc0: 8c01 3194 8594 8194 7d94 681b 6a19 0200  ..1.....}.h.j...
-00001fd0: 0073 6261 681f 7d94 2868 215d 9468 235d  .sbah.}.(h!].h#]
-00001fe0: 9468 255d 948c 1177 6f72 6463 6f75 6e74  .h%]...wordcount
-00001ff0: 2d6d 696e 7574 6573 9461 6827 5d94 6829  -minutes.ah'].h)
-00002000: 5d94 7568 2b6a 0702 0000 681d 682c 7562  ].uh+j....h.h,ub
-00002010: 758c 1273 7562 7374 6974 7574 696f 6e5f  u..substitution_
-00002020: 6e61 6d65 7394 7d94 288c 0f77 6f72 6463  names.}.(..wordc
-00002030: 6f75 6e74 2d77 6f72 6473 946a 0602 0000  ount-words.j....
-00002040: 8c11 776f 7264 636f 756e 742d 6d69 6e75  ..wordcount-minu
-00002050: 7465 7394 6a18 0200 0075 8c08 7265 666e  tes.j....u..refn
-00002060: 616d 6573 947d 948c 0672 6566 6964 7394  ames.}...refids.
-00002070: 7d94 8c07 6e61 6d65 6964 7394 7d94 286a  }...nameids.}.(j
-00002080: a101 0000 6a9e 0100 0068 a768 a468 d268  ....j....h.h.h.h
-00002090: cf6a 2701 0000 6a24 0100 006a 4e01 0000  .j'...j$...jN...
-000020a0: 6a4b 0100 006a 9901 0000 6a96 0100 0075  jK...j....j....u
-000020b0: 8c09 6e61 6d65 7479 7065 7394 7d94 286a  ..nametypes.}.(j
-000020c0: a101 0000 8968 a789 68d2 896a 2701 0000  .....h..h..j'...
-000020d0: 896a 4e01 0000 896a 9901 0000 8975 6821  .jN....j.....uh!
-000020e0: 7d94 286a 9e01 0000 680c 68a4 682d 68cf  }.(j....h.h.h-h.
-000020f0: 68aa 6a24 0100 0068 d56a 4b01 0000 6a2a  h.j$...h.jK...j*
-00002100: 0100 006a 9601 0000 6a51 0100 0075 8c0d  ...j....jQ...u..
-00002110: 666f 6f74 6e6f 7465 5f72 6566 7394 7d94  footnote_refs.}.
-00002120: 8c0d 6369 7461 7469 6f6e 5f72 6566 7394  ..citation_refs.
-00002130: 7d94 8c0d 6175 746f 666f 6f74 6e6f 7465  }...autofootnote
-00002140: 7394 5d94 8c11 6175 746f 666f 6f74 6e6f  s.]...autofootno
-00002150: 7465 5f72 6566 7394 5d94 8c10 7379 6d62  te_refs.]...symb
-00002160: 6f6c 5f66 6f6f 746e 6f74 6573 945d 948c  ol_footnotes.]..
-00002170: 1473 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
-00002180: 5f72 6566 7394 5d94 8c09 666f 6f74 6e6f  _refs.]...footno
-00002190: 7465 7394 5d94 8c09 6369 7461 7469 6f6e  tes.]...citation
-000021a0: 7394 5d94 8c12 6175 746f 666f 6f74 6e6f  s.]...autofootno
-000021b0: 7465 5f73 7461 7274 944b 018c 1573 796d  te_start.K...sym
-000021c0: 626f 6c5f 666f 6f74 6e6f 7465 5f73 7461  bol_footnote_sta
-000021d0: 7274 944b 008c 0a69 645f 636f 756e 7465  rt.K...id_counte
-000021e0: 7294 8c0b 636f 6c6c 6563 7469 6f6e 7394  r...collections.
-000021f0: 8c07 436f 756e 7465 7294 9394 7d94 8594  ..Counter...}...
-00002200: 5294 8c0e 7061 7273 655f 6d65 7373 6167  R...parse_messag
-00002210: 6573 945d 948c 1274 7261 6e73 666f 726d  es.]...transform
-00002220: 5f6d 6573 7361 6765 7394 5d94 8c0b 7472  _messages.]...tr
-00002230: 616e 7366 6f72 6d65 7294 4e8c 0b69 6e63  ansformer.N..inc
-00002240: 6c75 6465 5f6c 6f67 945d 948c 0a64 6563  lude_log.]...dec
-00002250: 6f72 6174 696f 6e94 4e68 1c68 038c 0a6d  oration.Nh.h...m
-00002260: 7973 745f 736c 7567 7394 7d94 7562 2e    yst_slugs.}.ub.
+00000080: 6594 9394 2981 947d 9428 6805 8c0f 6d7a  e...)..}.(h...mz
+00000090: 4461 7461 584d 4c53 7472 7563 7494 6807  DataXMLStruct.h.
+000000a0: 5d94 6809 8c04 5465 7874 9493 948c 0f6d  ].h...Text.....m
+000000b0: 7a44 6174 6158 4d4c 5374 7275 6374 9485  zDataXMLStruct..
+000000c0: 9481 947d 9428 8c06 7061 7265 6e74 9468  ...}.(..parent.h
+000000d0: 118c 095f 646f 6375 6d65 6e74 9468 038c  ..._document.h..
+000000e0: 0673 6f75 7263 6594 4e8c 046c 696e 6594  .source.N..line.
+000000f0: 4e75 6261 8c0a 6174 7472 6962 7574 6573  Nuba..attributes
+00000100: 947d 9428 8c03 6964 7394 5d94 8c07 636c  .}.(..ids.]...cl
+00000110: 6173 7365 7394 5d94 8c05 6e61 6d65 7394  asses.]...names.
+00000120: 5d94 8c08 6475 706e 616d 6573 945d 948c  ]...dupnames.]..
+00000130: 0862 6163 6b72 6566 7394 5d94 758c 0774  .backrefs.].u..t
+00000140: 6167 6e61 6d65 9468 0f68 1e4b 0168 1d8c  agname.h.h.K.h..
+00000150: 5e43 3a5c 5573 6572 735c 6d61 7869 6d5c  ^C:\Users\maxim\
+00000160: 4f6e 6544 7269 7665 5c44 6f63 756d 656e  OneDrive\Documen
+00000170: 7473 5c50 7974 686f 6e5c 5061 636b 6167  ts\Python\Packag
+00000180: 6573 5c6d 7a44 6174 6158 4d4c 324d 6174  es\mzDataXML2Mat
+00000190: 5c64 6f63 735c 736f 7572 6365 5c6d 7a44  \docs\source\mzD
+000001a0: 6174 6158 4d4c 5374 7275 6374 2e6d 6494  ataXMLStruct.md.
+000001b0: 681b 680c 681c 6803 7562 680b 2981 947d  h.h.h.h.ubh.)..}
+000001c0: 9428 6805 6806 6807 5d94 2868 1029 8194  .(h.h.h.].(h.)..
+000001d0: 7d94 2868 058c 0c50 7265 7365 6e74 6174  }.(h...Presentat
+000001e0: 696f 6e94 6807 5d94 6816 8c0c 5072 6573  ion.h.].h...Pres
+000001f0: 656e 7461 7469 6f6e 9485 9481 947d 9428  entation.....}.(
+00000200: 681b 6830 681c 6803 681d 4e68 1e4e 7562  h.h0h.h.h.Nh.Nub
+00000210: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00000220: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
+00000230: 1e4b 0368 1d68 2c68 1b68 2d68 1c68 0375  .K.h.h,h.h-h.h.u
+00000240: 6268 098c 0970 6172 6167 7261 7068 9493  bh...paragraph..
+00000250: 9429 8194 7d94 2868 058c 5e49 6e74 6572  .)..}.(h..^Inter
+00000260: 6e61 6c20 636c 6173 732c 2064 6f20 6e6f  nal class, do no
+00000270: 7420 7573 6520 6974 2074 6f20 7374 6f72  t use it to stor
+00000280: 6520 6461 7461 2e20 436f 6e73 6964 6572  e data. Consider
+00000290: 2075 7369 6e67 205b 6d7a 4461 7461 5d28   using [mzData](
+000002a0: 6d7a 4461 7461 2e6d 6429 2063 6c61 7373  mzData.md) class
+000002b0: 2069 6e73 7465 6164 2e94 6807 5d94 2868   instead..h.].(h
+000002c0: 168c 3c49 6e74 6572 6e61 6c20 636c 6173  ..<Internal clas
+000002d0: 732c 2064 6f20 6e6f 7420 7573 6520 6974  s, do not use it
+000002e0: 2074 6f20 7374 6f72 6520 6461 7461 2e20   to store data. 
+000002f0: 436f 6e73 6964 6572 2075 7369 6e67 2094  Consider using .
+00000300: 8594 8194 7d94 2868 1b68 4068 1c68 0368  ....}.(h.h@h.h.h
+00000310: 1d4e 681e 4e75 6268 008c 0c70 656e 6469  .Nh.Nubh...pendi
+00000320: 6e67 5f78 7265 6694 9394 2981 947d 9428  ng_xref...)..}.(
+00000330: 6805 6806 6807 5d94 6809 8c06 696e 6c69  h.h.h.].h...inli
+00000340: 6e65 9493 9429 8194 7d94 2868 058c 066d  ne...)..}.(h...m
+00000350: 7a44 6174 6194 6807 5d94 6816 8c06 6d7a  zData.h.].h...mz
+00000360: 4461 7461 9485 9481 947d 9428 681b 684f  Data.....}.(h.hO
+00000370: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00000380: 9428 6821 5d94 6823 5d94 288c 0478 7265  .(h!].h#].(..xre
+00000390: 6694 8c04 6d79 7374 9465 6825 5d94 6827  f...myst.eh%].h'
+000003a0: 5d94 6829 5d94 7568 2b68 4d68 1b68 4a68  ].h)].uh+hMh.hJh
+000003b0: 1c68 0368 1d68 2c68 1e4b 0075 6261 681f  .h.h.h,h.K.ubah.
+000003c0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+000003d0: 275d 9468 295d 948c 0972 6566 646f 6d61  '].h)]...refdoma
+000003e0: 696e 948c 0364 6f63 948c 0972 6566 7461  in...doc...refta
+000003f0: 7267 6574 948c 066d 7a44 6174 6194 8c0b  rget...mzData...
+00000400: 7265 6674 6172 6765 7469 6494 4e8c 0672  reftargetid.N..r
+00000410: 6566 646f 6394 8c0f 6d7a 4461 7461 584d  efdoc...mzDataXM
+00000420: 4c53 7472 7563 7494 8c07 7265 6674 7970  LStruct...reftyp
+00000430: 6594 685b 8c0b 7265 6665 7870 6c69 6369  e.h[..refexplici
+00000440: 7494 8875 682b 6848 681e 4b04 681d 682c  t..uh+hHh.K.h.h,
+00000450: 681b 6840 681c 6803 7562 6816 8c0f 2063  h.h@h.h.ubh... c
+00000460: 6c61 7373 2069 6e73 7465 6164 2e94 8594  lass instead....
+00000470: 8194 7d94 2868 1b68 4068 1c68 0368 1d4e  ..}.(h.h@h.h.h.N
+00000480: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
+00000490: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+000004a0: 682b 683e 681e 4b04 681d 682c 681b 682d  h+h>h.K.h.h,h.h-
+000004b0: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
+000004c0: 8c0c 7072 6573 656e 7461 7469 6f6e 9461  ..presentation.a
+000004d0: 6823 5d94 6825 5d94 8c0c 7072 6573 656e  h#].h%]...presen
+000004e0: 7461 7469 6f6e 9461 6827 5d94 6829 5d94  tation.ah'].h)].
+000004f0: 7568 2b68 0a68 1e4b 0368 1d68 2c68 1b68  uh+h.h.K.h.h,h.h
+00000500: 0c68 1c68 0375 6268 0b29 8194 7d94 2868  .h.h.ubh.)..}.(h
+00000510: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
+00000520: 6805 8c0a 4465 6669 6e69 7469 6f6e 9468  h...Definition.h
+00000530: 075d 9468 168c 0a44 6566 696e 6974 696f  .].h...Definitio
+00000540: 6e94 8594 8194 7d94 2868 1b68 8368 1c68  n.....}.(h.h.h.h
+00000550: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00000560: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00000570: 295d 9475 682b 680f 681e 4b06 681d 682c  )].uh+h.h.K.h.h,
+00000580: 681b 6880 681c 6803 7562 6809 8c0d 6c69  h.h.h.h.ubh...li
+00000590: 7465 7261 6c5f 626c 6f63 6b94 9394 2981  teral_block...).
+000005a0: 947d 9428 6805 8c5f 636c 6173 7320 6d7a  .}.(h.._class mz
+000005b0: 4461 7461 584d 4c53 7472 7563 7428 4261  DataXMLStruct(Ba
+000005c0: 7365 4d6f 6465 6c29 3a0a 2020 2020 6d65  seModel):.    me
+000005d0: 7461 6461 7461 203a 2064 6963 740a 2020  tadata : dict.  
+000005e0: 2020 7469 6d65 7320 3a20 6c69 7374 5b66    times : list[f
+000005f0: 6c6f 6174 5d0a 2020 2020 7365 7269 6573  loat].    series
+00000600: 203a 2041 6e79 0a94 6807 5d94 6816 8c5f   : Any..h.].h.._
+00000610: 636c 6173 7320 6d7a 4461 7461 584d 4c53  class mzDataXMLS
+00000620: 7472 7563 7428 4261 7365 4d6f 6465 6c29  truct(BaseModel)
+00000630: 3a0a 2020 2020 6d65 7461 6461 7461 203a  :.    metadata :
+00000640: 2064 6963 740a 2020 2020 7469 6d65 7320   dict.    times 
+00000650: 3a20 6c69 7374 5b66 6c6f 6174 5d0a 2020  : list[float].  
+00000660: 2020 7365 7269 6573 203a 2041 6e79 0a94    series : Any..
+00000670: 8594 8194 7d94 681b 6893 7362 6168 1f7d  ....}.h.h.sbah.}
+00000680: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00000690: 5d94 6829 5d94 8c08 6c61 6e67 7561 6765  ].h)]...language
+000006a0: 948c 0670 7974 686f 6e94 8c09 786d 6c3a  ...python...xml:
+000006b0: 7370 6163 6594 8c08 7072 6573 6572 7665  space...preserve
+000006c0: 9475 682b 6891 681d 682c 681e 4b07 681b  .uh+h.h.h,h.K.h.
+000006d0: 6880 681c 6803 7562 6568 1f7d 9428 6821  h.h.h.ubeh.}.(h!
+000006e0: 5d94 8c0a 6465 6669 6e69 7469 6f6e 9461  ]...definition.a
+000006f0: 6823 5d94 6825 5d94 8c0a 6465 6669 6e69  h#].h%]...defini
+00000700: 7469 6f6e 9461 6827 5d94 6829 5d94 7568  tion.ah'].h)].uh
+00000710: 2b68 0a68 1e4b 0668 1d68 2c68 1b68 0c68  +h.h.K.h.h,h.h.h
+00000720: 1c68 0375 6268 0b29 8194 7d94 2868 0568  .h.ubh.)..}.(h.h
+00000730: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
+00000740: 8c0a 486f 7720 746f 2075 7365 9468 075d  ..How to use.h.]
+00000750: 9468 168c 0a48 6f77 2074 6f20 7573 6594  .h...How to use.
+00000760: 8594 8194 7d94 2868 1b68 b068 1c68 0368  ....}.(h.h.h.h.h
+00000770: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00000780: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00000790: 9475 682b 680f 681e 4b0d 681d 682c 681b  .uh+h.h.K.h.h,h.
+000007a0: 68ad 681c 6803 7562 6892 2981 947d 9428  h.h.h.ubh.)..}.(
+000007b0: 6805 8c61 7661 6c75 6520 3d20 6d7a 4461  h..avalue = mzDa
+000007c0: 7461 584d 4c53 7472 7563 7428 0a20 2020  taXMLStruct(.   
+000007d0: 206d 6574 6164 6174 6120 3d20 736f 6d65   metadata = some
+000007e0: 4469 6374 2c0a 2020 2020 7469 6d65 7320  Dict,.    times 
+000007f0: 3d20 6c69 7374 4f66 5469 6d65 732c 0a20  = listOfTimes,. 
+00000800: 2020 2073 6572 6965 7320 3d20 7365 7269     series = seri
+00000810: 6573 0a29 0a94 6807 5d94 6816 8c61 7661  es.)..h.].h..ava
+00000820: 6c75 6520 3d20 6d7a 4461 7461 584d 4c53  lue = mzDataXMLS
+00000830: 7472 7563 7428 0a20 2020 206d 6574 6164  truct(.    metad
+00000840: 6174 6120 3d20 736f 6d65 4469 6374 2c0a  ata = someDict,.
+00000850: 2020 2020 7469 6d65 7320 3d20 6c69 7374      times = list
+00000860: 4f66 5469 6d65 732c 0a20 2020 2073 6572  OfTimes,.    ser
+00000870: 6965 7320 3d20 7365 7269 6573 0a29 0a94  ies = series.)..
+00000880: 8594 8194 7d94 681b 68be 7362 6168 1f7d  ....}.h.h.sbah.}
+00000890: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+000008a0: 5d94 6829 5d94 8c08 6c61 6e67 7561 6765  ].h)]...language
+000008b0: 948c 0670 7974 686f 6e94 68a3 68a4 7568  ...python.h.h.uh
+000008c0: 2b68 9168 1d68 2c68 1e4b 0e68 1b68 ad68  +h.h.h,h.K.h.h.h
+000008d0: 1c68 0375 6265 681f 7d94 2868 215d 948c  .h.ubeh.}.(h!]..
+000008e0: 0a68 6f77 2d74 6f2d 7573 6594 6168 235d  .how-to-use.ah#]
+000008f0: 9468 255d 948c 0a68 6f77 2074 6f20 7573  .h%]...how to us
+00000900: 6594 6168 275d 9468 295d 9475 682b 680a  e.ah'].h)].uh+h.
+00000910: 681e 4b0d 681d 682c 681b 680c 681c 6803  h.K.h.h,h.h.h.h.
+00000920: 7562 680b 2981 947d 9428 6805 6806 6807  ubh.)..}.(h.h.h.
+00000930: 5d94 2868 1029 8194 7d94 2868 058c 0946  ].(h.)..}.(h...F
+00000940: 756e 6374 696f 6e73 9468 075d 9468 168c  unctions.h.].h..
+00000950: 0946 756e 6374 696f 6e73 9485 9481 947d  .Functions.....}
+00000960: 9428 681b 68d9 681c 6803 681d 4e68 1e4e  .(h.h.h.h.h.Nh.N
+00000970: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00000980: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00000990: 0f68 1e4b 1668 1d68 2c68 1b68 d668 1c68  .h.K.h.h,h.h.h.h
+000009a0: 0375 6268 3f29 8194 7d94 2868 058c 044e  .ubh?)..}.(h...N
+000009b0: 6f6e 6594 6807 5d94 6816 8c04 4e6f 6e65  one.h.].h...None
+000009c0: 9485 9481 947d 9428 681b 68e7 681c 6803  .....}.(h.h.h.h.
+000009d0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000009e0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000009f0: 5d94 7568 2b68 3e68 1e4b 1768 1d68 2c68  ].uh+h>h.K.h.h,h
+00000a00: 1b68 d668 1c68 0375 6265 681f 7d94 2868  .h.h.h.ubeh.}.(h
+00000a10: 215d 948c 0966 756e 6374 696f 6e73 9461  !]...functions.a
+00000a20: 6823 5d94 6825 5d94 8c09 6675 6e63 7469  h#].h%]...functi
+00000a30: 6f6e 7394 6168 275d 9468 295d 9475 682b  ons.ah'].h)].uh+
+00000a40: 680a 681e 4b16 681d 682c 681b 680c 681c  h.h.K.h.h,h.h.h.
+00000a50: 6803 7562 680b 2981 947d 9428 6805 6806  h.ubh.)..}.(h.h.
+00000a60: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
+00000a70: 054e 6f74 6573 9468 075d 9468 168c 054e  .Notes.h.].h...N
+00000a80: 6f74 6573 9485 9481 947d 9428 681b 6a00  otes.....}.(h.j.
+00000a90: 0100 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00000aa0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00000ab0: 9468 275d 9468 295d 9475 682b 680f 681e  .h'].h)].uh+h.h.
+00000ac0: 4b19 681d 682c 681b 68fd 681c 6803 7562  K.h.h,h.h.h.h.ub
+00000ad0: 683f 2981 947d 9428 6805 8c9f 5468 6973  h?)..}.(h...This
+00000ae0: 2069 7320 616e 205f 5f69 6e74 6572 6e61   is an __interna
+00000af0: 6c5f 5f20 636c 6173 732c 2069 7420 7368  l__ class, it sh
+00000b00: 6f75 6c64 6e27 7420 6265 2075 7365 6420  ouldn't be used 
+00000b10: 746f 2073 746f 7265 206d 7a20 7661 6c75  to store mz valu
+00000b20: 6573 2e20 5468 6973 2063 6c61 7373 2069  es. This class i
+00000b30: 7320 6175 746f 6d61 7469 6361 6c6c 7920  s automatically 
+00000b40: 706f 7075 6c61 7465 6420 7768 656e 2070  populated when p
+00000b50: 6172 7369 6e67 2061 2060 2e6d 7a44 6174  arsing a `.mzDat
+00000b60: 612e 786d 6c60 2066 696c 6520 616e 6420  a.xml` file and 
+00000b70: 6973 2070 7269 7661 7465 2e94 6807 5d94  is private..h.].
+00000b80: 2868 168c 0b54 6869 7320 6973 2061 6e20  (h...This is an 
+00000b90: 9485 9481 947d 9428 681b 6a0e 0100 0068  .....}.(h.j....h
+00000ba0: 1c68 0368 1d4e 681e 4e75 6268 098c 0673  .h.h.Nh.Nubh...s
+00000bb0: 7472 6f6e 6794 9394 2981 947d 9428 6805  trong...)..}.(h.
+00000bc0: 8c08 696e 7465 726e 616c 9468 075d 9468  ..internal.h.].h
+00000bd0: 168c 0869 6e74 6572 6e61 6c94 8594 8194  ...internal.....
+00000be0: 7d94 2868 1b6a 1801 0000 681c 6803 681d  }.(h.j....h.h.h.
+00000bf0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00000c00: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00000c10: 7568 2b6a 1601 0000 681e 4b1a 681d 682c  uh+j....h.K.h.h,
+00000c20: 681b 6a0e 0100 0068 1c68 0375 6268 168c  h.j....h.h.ubh..
+00000c30: 6820 636c 6173 732c 2069 7420 7368 6f75  h class, it shou
+00000c40: 6c64 6ee2 8099 7420 6265 2075 7365 6420  ldn...t be used 
+00000c50: 746f 2073 746f 7265 206d 7a20 7661 6c75  to store mz valu
+00000c60: 6573 2e20 5468 6973 2063 6c61 7373 2069  es. This class i
+00000c70: 7320 6175 746f 6d61 7469 6361 6c6c 7920  s automatically 
+00000c80: 706f 7075 6c61 7465 6420 7768 656e 2070  populated when p
+00000c90: 6172 7369 6e67 2061 2094 8594 8194 7d94  arsing a .....}.
+00000ca0: 2868 1b6a 0e01 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00000cb0: 1e4e 7562 6809 8c07 6c69 7465 7261 6c94  .Nubh...literal.
+00000cc0: 9394 2981 947d 9428 6805 8c0b 2e6d 7a44  ..)..}.(h....mzD
+00000cd0: 6174 612e 786d 6c94 6807 5d94 6816 8c0b  ata.xml.h.].h...
+00000ce0: 2e6d 7a44 6174 612e 786d 6c94 8594 8194  .mzData.xml.....
+00000cf0: 7d94 2868 1b6a 2c01 0000 681c 6803 681d  }.(h.j,...h.h.h.
+00000d00: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00000d10: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00000d20: 7568 2b6a 2a01 0000 681e 4b1a 681d 682c  uh+j*...h.K.h.h,
+00000d30: 681b 6a0e 0100 0068 1c68 0375 6268 168c  h.j....h.h.ubh..
+00000d40: 1520 6669 6c65 2061 6e64 2069 7320 7072  . file and is pr
+00000d50: 6976 6174 652e 9485 9481 947d 9428 681b  ivate......}.(h.
+00000d60: 6a0e 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00000d70: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00000d80: 255d 9468 275d 9468 295d 9475 682b 683e  %].h'].h)].uh+h>
+00000d90: 681e 4b1a 681d 682c 681b 68fd 681c 6803  h.K.h.h,h.h.h.h.
+00000da0: 7562 683f 2981 947d 9428 6805 8c51 436f  ubh?)..}.(h..QCo
+00000db0: 6e73 6964 6572 2075 7369 6e67 205b 6d7a  nsider using [mz
+00000dc0: 4461 7461 5d28 6d7a 4461 7461 2e6d 6429  Data](mzData.md)
+00000dd0: 2063 6c61 7373 2074 6f20 7374 6f72 6520   class to store 
+00000de0: 796f 7572 206d 7a20 616e 6420 696e 7465  your mz and inte
+00000df0: 6e73 6974 6965 7320 7661 6c75 6573 2e94  nsities values..
+00000e00: 6807 5d94 2868 168c 0f43 6f6e 7369 6465  h.].(h...Conside
+00000e10: 7220 7573 696e 6720 9485 9481 947d 9428  r using .....}.(
+00000e20: 681b 6a44 0100 0068 1c68 0368 1d4e 681e  h.jD...h.h.h.Nh.
+00000e30: 4e75 6268 4929 8194 7d94 2868 0568 0668  NubhI)..}.(h.h.h
+00000e40: 075d 9468 4e29 8194 7d94 2868 058c 066d  .].hN)..}.(h...m
+00000e50: 7a44 6174 6194 6807 5d94 6816 8c06 6d7a  zData.h.].h...mz
+00000e60: 4461 7461 9485 9481 947d 9428 681b 6a4f  Data.....}.(h.jO
+00000e70: 0100 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00000e80: 681f 7d94 2868 215d 9468 235d 9428 685a  h.}.(h!].h#].(hZ
+00000e90: 685b 6568 255d 9468 275d 9468 295d 9475  h[eh%].h'].h)].u
+00000ea0: 682b 684d 681b 6a4c 0100 0068 1c68 0368  h+hMh.jL...h.h.h
+00000eb0: 1d68 2c68 1e4b 0075 6261 681f 7d94 2868  .h,h.K.ubah.}.(h
+00000ec0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00000ed0: 295d 948c 0972 6566 646f 6d61 696e 9468  )]...refdomain.h
+00000ee0: 668c 0972 6566 7461 7267 6574 948c 066d  f..reftarget...m
+00000ef0: 7a44 6174 6194 8c0b 7265 6674 6172 6765  zData...reftarge
+00000f00: 7469 6494 4e8c 0672 6566 646f 6394 686b  tid.N..refdoc.hk
+00000f10: 8c07 7265 6674 7970 6594 685b 8c0b 7265  ..reftype.h[..re
+00000f20: 6665 7870 6c69 6369 7494 8875 682b 6848  fexplicit..uh+hH
+00000f30: 681e 4b1c 681d 682c 681b 6a44 0100 0068  h.K.h.h,h.jD...h
+00000f40: 1c68 0375 6268 168c 2f20 636c 6173 7320  .h.ubh../ class 
+00000f50: 746f 2073 746f 7265 2079 6f75 7220 6d7a  to store your mz
+00000f60: 2061 6e64 2069 6e74 656e 7369 7469 6573   and intensities
+00000f70: 2076 616c 7565 732e 9485 9481 947d 9428   values......}.(
+00000f80: 681b 6a44 0100 0068 1c68 0368 1d4e 681e  h.jD...h.h.h.Nh.
+00000f90: 4e75 6265 681f 7d94 2868 215d 9468 235d  Nubeh.}.(h!].h#]
+00000fa0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00000fb0: 683e 681e 4b1c 681d 682c 681b 68fd 681c  h>h.K.h.h,h.h.h.
+00000fc0: 6803 7562 6568 1f7d 9428 6821 5d94 8c05  h.ubeh.}.(h!]...
+00000fd0: 6e6f 7465 7394 6168 235d 9468 255d 948c  notes.ah#].h%]..
+00000fe0: 056e 6f74 6573 9461 6827 5d94 6829 5d94  .notes.ah'].h)].
+00000ff0: 7568 2b68 0a68 1e4b 1968 1d68 2c68 1b68  uh+h.h.K.h.h,h.h
+00001000: 0c68 1c68 0375 6265 681f 7d94 2868 215d  .h.h.ubeh.}.(h!]
+00001010: 948c 0f6d 7a64 6174 6178 6d6c 7374 7275  ...mzdataxmlstru
+00001020: 6374 9461 6823 5d94 6825 5d94 8c0f 6d7a  ct.ah#].h%]...mz
+00001030: 6461 7461 786d 6c73 7472 7563 7494 6168  dataxmlstruct.ah
+00001040: 275d 9468 295d 9475 682b 680a 681e 4b01  '].h)].uh+h.h.K.
+00001050: 681d 682c 681b 6803 681c 6803 7562 6168  h.h,h.h.h.h.ubah
+00001060: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00001070: 6827 5d94 6829 5d94 8c06 736f 7572 6365  h'].h)]...source
+00001080: 9468 2c8c 1474 7261 6e73 6c61 7469 6f6e  .h,..translation
+00001090: 5f70 726f 6772 6573 7394 7d94 288c 0574  _progress.}.(..t
+000010a0: 6f74 616c 944b 008c 0a74 7261 6e73 6c61  otal.K...transla
+000010b0: 7465 6494 4b00 7575 682b 6801 8c0e 6375  ted.K.uuh+h...cu
+000010c0: 7272 656e 745f 736f 7572 6365 944e 8c0c  rrent_source.N..
+000010d0: 6375 7272 656e 745f 6c69 6e65 944e 8c08  current_line.N..
+000010e0: 7365 7474 696e 6773 948c 1164 6f63 7574  settings...docut
+000010f0: 696c 732e 6672 6f6e 7465 6e64 948c 0656  ils.frontend...V
+00001100: 616c 7565 7394 9394 2981 947d 9428 8c06  alues...)..}.(..
+00001110: 6f75 7470 7574 944e 680f 4e8c 0967 656e  output.Nh.N..gen
+00001120: 6572 6174 6f72 944e 8c09 6461 7465 7374  erator.N..datest
+00001130: 616d 7094 4e8c 0b73 6f75 7263 655f 6c69  amp.N..source_li
+00001140: 6e6b 944e 8c0a 736f 7572 6365 5f75 726c  nk.N..source_url
+00001150: 944e 8c0d 746f 635f 6261 636b 6c69 6e6b  .N..toc_backlink
+00001160: 7394 8c05 656e 7472 7994 8c12 666f 6f74  s...entry...foot
+00001170: 6e6f 7465 5f62 6163 6b6c 696e 6b73 944b  note_backlinks.K
+00001180: 018c 0d73 6563 746e 756d 5f78 666f 726d  ...sectnum_xform
+00001190: 944b 018c 0e73 7472 6970 5f63 6f6d 6d65  .K...strip_comme
+000011a0: 6e74 7394 4e8c 1b73 7472 6970 5f65 6c65  nts.N..strip_ele
+000011b0: 6d65 6e74 735f 7769 7468 5f63 6c61 7373  ments_with_class
+000011c0: 6573 944e 8c0d 7374 7269 705f 636c 6173  es.N..strip_clas
+000011d0: 7365 7394 4e8c 0c72 6570 6f72 745f 6c65  ses.N..report_le
+000011e0: 7665 6c94 4b02 8c0a 6861 6c74 5f6c 6576  vel.K...halt_lev
+000011f0: 656c 944b 058c 1165 7869 745f 7374 6174  el.K...exit_stat
+00001200: 7573 5f6c 6576 656c 944b 058c 0564 6562  us_level.K...deb
+00001210: 7567 944e 8c0e 7761 726e 696e 675f 7374  ug.N..warning_st
+00001220: 7265 616d 944e 8c09 7472 6163 6562 6163  ream.N..tracebac
+00001230: 6b94 888c 0e69 6e70 7574 5f65 6e63 6f64  k....input_encod
+00001240: 696e 6794 8c09 7574 662d 382d 7369 6794  ing...utf-8-sig.
+00001250: 8c1c 696e 7075 745f 656e 636f 6469 6e67  ..input_encoding
+00001260: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+00001270: 0673 7472 6963 7494 8c0f 6f75 7470 7574  .strict...output
+00001280: 5f65 6e63 6f64 696e 6794 8c05 7574 662d  _encoding...utf-
+00001290: 3894 8c1d 6f75 7470 7574 5f65 6e63 6f64  8...output_encod
+000012a0: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
+000012b0: 7294 6aac 0100 008c 0e65 7272 6f72 5f65  r.j......error_e
+000012c0: 6e63 6f64 696e 6794 8c05 7574 662d 3894  ncoding...utf-8.
+000012d0: 8c1c 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
+000012e0: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+000012f0: 1062 6163 6b73 6c61 7368 7265 706c 6163  .backslashreplac
+00001300: 6594 8c0d 6c61 6e67 7561 6765 5f63 6f64  e...language_cod
+00001310: 6594 8c02 656e 948c 1372 6563 6f72 645f  e...en...record_
+00001320: 6465 7065 6e64 656e 6369 6573 944e 8c06  dependencies.N..
+00001330: 636f 6e66 6967 944e 8c09 6964 5f70 7265  config.N..id_pre
+00001340: 6669 7894 6806 8c0e 6175 746f 5f69 645f  fix.h...auto_id_
+00001350: 7072 6566 6978 948c 0269 6494 8c0d 6475  prefix...id...du
+00001360: 6d70 5f73 6574 7469 6e67 7394 4e8c 0e64  mp_settings.N..d
+00001370: 756d 705f 696e 7465 726e 616c 7394 4e8c  ump_internals.N.
+00001380: 0f64 756d 705f 7472 616e 7366 6f72 6d73  .dump_transforms
+00001390: 944e 8c0f 6475 6d70 5f70 7365 7564 6f5f  .N..dump_pseudo_
+000013a0: 786d 6c94 4e8c 1065 7870 6f73 655f 696e  xml.N..expose_in
+000013b0: 7465 726e 616c 7394 4e8c 0e73 7472 6963  ternals.N..stric
+000013c0: 745f 7669 7369 746f 7294 4e8c 0f5f 6469  t_visitor.N.._di
+000013d0: 7361 626c 655f 636f 6e66 6967 944e 8c07  sable_config.N..
+000013e0: 5f73 6f75 7263 6594 682c 8c0c 5f64 6573  _source.h,.._des
+000013f0: 7469 6e61 7469 6f6e 944e 8c0d 5f63 6f6e  tination.N.._con
+00001400: 6669 675f 6669 6c65 7394 5d94 8c16 6669  fig_files.]...fi
+00001410: 6c65 5f69 6e73 6572 7469 6f6e 5f65 6e61  le_insertion_ena
+00001420: 626c 6564 9488 8c0b 7261 775f 656e 6162  bled....raw_enab
+00001430: 6c65 6494 4b01 8c11 6c69 6e65 5f6c 656e  led.K...line_len
+00001440: 6774 685f 6c69 6d69 7494 4d10 278c 0e70  gth_limit.M.'..p
+00001450: 6570 5f72 6566 6572 656e 6365 7394 4e8c  ep_references.N.
+00001460: 0c70 6570 5f62 6173 655f 7572 6c94 8c18  .pep_base_url...
+00001470: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
+00001480: 686f 6e2e 6f72 672f 948c 1570 6570 5f66  hon.org/...pep_f
+00001490: 696c 655f 7572 6c5f 7465 6d70 6c61 7465  ile_url_template
+000014a0: 948c 0870 6570 2d25 3034 6494 8c0e 7266  ...pep-%04d...rf
+000014b0: 635f 7265 6665 7265 6e63 6573 944e 8c0c  c_references.N..
+000014c0: 7266 635f 6261 7365 5f75 726c 948c 2668  rfc_base_url..&h
+000014d0: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
+000014e0: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
+000014f0: 6874 6d6c 2f94 8c09 7461 625f 7769 6474  html/...tab_widt
+00001500: 6894 4b08 8c1d 7472 696d 5f66 6f6f 746e  h.K...trim_footn
+00001510: 6f74 655f 7265 6665 7265 6e63 655f 7370  ote_reference_sp
+00001520: 6163 6594 898c 1073 796e 7461 785f 6869  ace....syntax_hi
+00001530: 6768 6c69 6768 7494 8c04 6c6f 6e67 948c  ghlight...long..
+00001540: 0c73 6d61 7274 5f71 756f 7465 7394 888c  .smart_quotes...
+00001550: 1373 6d61 7274 7175 6f74 6573 5f6c 6f63  .smartquotes_loc
+00001560: 616c 6573 945d 948c 1d63 6861 7261 6374  ales.]...charact
+00001570: 6572 5f6c 6576 656c 5f69 6e6c 696e 655f  er_level_inline_
+00001580: 6d61 726b 7570 9489 8c0e 646f 6374 6974  markup....doctit
+00001590: 6c65 5f78 666f 726d 9489 8c0d 646f 6369  le_xform....doci
+000015a0: 6e66 6f5f 7866 6f72 6d94 4b01 8c12 7365  nfo_xform.K...se
+000015b0: 6374 7375 6274 6974 6c65 5f78 666f 726d  ctsubtitle_xform
+000015c0: 9489 8c0d 696d 6167 655f 6c6f 6164 696e  ....image_loadin
+000015d0: 6794 8c04 6c69 6e6b 948c 1065 6d62 6564  g...link...embed
+000015e0: 5f73 7479 6c65 7368 6565 7494 898c 1563  _stylesheet....c
+000015f0: 6c6f 616b 5f65 6d61 696c 5f61 6464 7265  loak_email_addre
+00001600: 7373 6573 9488 8c11 7365 6374 696f 6e5f  sses....section_
+00001610: 7365 6c66 5f6c 696e 6b94 898c 0365 6e76  self_link....env
+00001620: 944e 7562 8c08 7265 706f 7274 6572 944e  .Nub..reporter.N
+00001630: 8c10 696e 6469 7265 6374 5f74 6172 6765  ..indirect_targe
+00001640: 7473 945d 948c 1173 7562 7374 6974 7574  ts.]...substitut
+00001650: 696f 6e5f 6465 6673 947d 9428 8c0f 776f  ion_defs.}.(..wo
+00001660: 7264 636f 756e 742d 776f 7264 7394 6809  rdcount-words.h.
+00001670: 8c17 7375 6273 7469 7475 7469 6f6e 5f64  ..substitution_d
+00001680: 6566 696e 6974 696f 6e94 9394 2981 947d  efinition...)..}
+00001690: 9428 6805 8c02 3538 9468 075d 9468 168c  .(h...58.h.].h..
+000016a0: 0235 3894 8594 8194 7d94 681b 6aea 0100  .58.....}.h.j...
+000016b0: 0073 6261 681f 7d94 2868 215d 9468 235d  .sbah.}.(h!].h#]
+000016c0: 9468 255d 948c 0f77 6f72 6463 6f75 6e74  .h%]...wordcount
+000016d0: 2d77 6f72 6473 9461 6827 5d94 6829 5d94  -words.ah'].h)].
+000016e0: 7568 2b6a e801 0000 681d 682c 7562 8c11  uh+j....h.h,ub..
+000016f0: 776f 7264 636f 756e 742d 6d69 6e75 7465  wordcount-minute
+00001700: 7394 6ae9 0100 0029 8194 7d94 2868 058c  s.j....)..}.(h..
+00001710: 0130 9468 075d 9468 168c 0130 9485 9481  .0.h.].h...0....
+00001720: 947d 9468 1b6a fa01 0000 7362 6168 1f7d  .}.h.j....sbah.}
+00001730: 9428 6821 5d94 6823 5d94 6825 5d94 8c11  .(h!].h#].h%]...
+00001740: 776f 7264 636f 756e 742d 6d69 6e75 7465  wordcount-minute
+00001750: 7394 6168 275d 9468 295d 9475 682b 6ae8  s.ah'].h)].uh+j.
+00001760: 0100 0068 1d68 2c75 6275 8c12 7375 6273  ...h.h,ubu..subs
+00001770: 7469 7475 7469 6f6e 5f6e 616d 6573 947d  titution_names.}
+00001780: 9428 8c0f 776f 7264 636f 756e 742d 776f  .(..wordcount-wo
+00001790: 7264 7394 6ae7 0100 008c 1177 6f72 6463  rds.j......wordc
+000017a0: 6f75 6e74 2d6d 696e 7574 6573 946a f901  ount-minutes.j..
+000017b0: 0000 758c 0872 6566 6e61 6d65 7394 7d94  ..u..refnames.}.
+000017c0: 8c06 7265 6669 6473 947d 948c 076e 616d  ..refids.}...nam
+000017d0: 6569 6473 947d 9428 6a81 0100 006a 7e01  eids.}.(j....j~.
+000017e0: 0000 687d 687a 68aa 68a7 68d3 68d0 68fa  ..h}hzh.h.h.h.h.
+000017f0: 68f7 6a79 0100 006a 7601 0000 758c 096e  h.jy...jv...u..n
+00001800: 616d 6574 7970 6573 947d 9428 6a81 0100  ametypes.}.(j...
+00001810: 0089 687d 8968 aa89 68d3 8968 fa89 6a79  ..h}.h..h..h..jy
+00001820: 0100 0089 7568 217d 9428 6a7e 0100 0068  ....uh!}.(j~...h
+00001830: 0c68 7a68 2d68 a768 8068 d068 ad68 f768  .hzh-h.h.h.h.h.h
+00001840: d66a 7601 0000 68fd 758c 0d66 6f6f 746e  .jv...h.u..footn
+00001850: 6f74 655f 7265 6673 947d 948c 0d63 6974  ote_refs.}...cit
+00001860: 6174 696f 6e5f 7265 6673 947d 948c 0d61  ation_refs.}...a
+00001870: 7574 6f66 6f6f 746e 6f74 6573 945d 948c  utofootnotes.]..
+00001880: 1161 7574 6f66 6f6f 746e 6f74 655f 7265  .autofootnote_re
+00001890: 6673 945d 948c 1073 796d 626f 6c5f 666f  fs.]...symbol_fo
+000018a0: 6f74 6e6f 7465 7394 5d94 8c14 7379 6d62  otnotes.]...symb
+000018b0: 6f6c 5f66 6f6f 746e 6f74 655f 7265 6673  ol_footnote_refs
+000018c0: 945d 948c 0966 6f6f 746e 6f74 6573 945d  .]...footnotes.]
+000018d0: 948c 0963 6974 6174 696f 6e73 945d 948c  ...citations.]..
+000018e0: 1261 7574 6f66 6f6f 746e 6f74 655f 7374  .autofootnote_st
+000018f0: 6172 7494 4b01 8c15 7379 6d62 6f6c 5f66  art.K...symbol_f
+00001900: 6f6f 746e 6f74 655f 7374 6172 7494 4b00  ootnote_start.K.
+00001910: 8c0a 6964 5f63 6f75 6e74 6572 948c 0b63  ..id_counter...c
+00001920: 6f6c 6c65 6374 696f 6e73 948c 0743 6f75  ollections...Cou
+00001930: 6e74 6572 9493 947d 9485 9452 948c 0e70  nter...}...R...p
+00001940: 6172 7365 5f6d 6573 7361 6765 7394 5d94  arse_messages.].
+00001950: 8c12 7472 616e 7366 6f72 6d5f 6d65 7373  ..transform_mess
+00001960: 6167 6573 945d 948c 0b74 7261 6e73 666f  ages.]...transfo
+00001970: 726d 6572 944e 8c0b 696e 636c 7564 655f  rmer.N..include_
+00001980: 6c6f 6794 5d94 8c0a 6465 636f 7261 7469  log.]...decorati
+00001990: 6f6e 944e 681c 6803 8c0a 6d79 7374 5f73  on.Nh.h...myst_s
+000019a0: 6c75 6773 947d 9475 622e                 lugs.}.ub.
```

### Comparing `mzdata2mat-0.1.1/docs/build/doctrees/mzDataManager.doctree` & `mzdata2mat-0.2.0/docs/build/doctrees/mzDataManager.doctree`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9557 6f00 0000 0000 008c 0f73 7068  ...Wo........sph
+00000000: 8005 951a 7100 0000 0000 008c 0f73 7068  ....q........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -14,1770 +14,1798 @@
 000000d0: 646f 6375 6d65 6e74 9468 038c 0673 6f75  document.h...sou
 000000e0: 7263 6594 4e8c 046c 696e 6594 4e75 6261  rce.N..line.Nuba
 000000f0: 8c0a 6174 7472 6962 7574 6573 947d 9428  ..attributes.}.(
 00000100: 8c03 6964 7394 5d94 8c07 636c 6173 7365  ..ids.]...classe
 00000110: 7394 5d94 8c05 6e61 6d65 7394 5d94 8c08  s.]...names.]...
 00000120: 6475 706e 616d 6573 945d 948c 0862 6163  dupnames.]...bac
 00000130: 6b72 6566 7394 5d94 758c 0774 6167 6e61  krefs.].u..tagna
-00000140: 6d65 9468 0f68 1e4b 0168 1d8c 7b2f 5573  me.h.h.K.h..{/Us
-00000150: 6572 732f 6c69 6368 3931 312f 4c69 6272  ers/lich911/Libr
-00000160: 6172 792f 436c 6f75 6453 746f 7261 6765  ary/CloudStorage
-00000170: 2f4f 6e65 4472 6976 652d 5065 7273 6f6e  /OneDrive-Person
-00000180: 6e65 6c2f 446f 6375 6d65 6e74 732f 5079  nel/Documents/Py
-00000190: 7468 6f6e 2f50 6163 6b61 6765 732f 6d7a  thon/Packages/mz
-000001a0: 4461 7461 584d 4c32 4d61 742f 646f 6373  DataXML2Mat/docs
-000001b0: 2f73 6f75 7263 652f 6d7a 4461 7461 4d61  /source/mzDataMa
-000001c0: 6e61 6765 722e 6d64 9468 1b68 0c68 1c68  nager.md.h.h.h.h
-000001d0: 0375 6268 0b29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
-000001e0: 075d 9428 6810 2981 947d 9428 6805 8c0c  .].(h.)..}.(h...
-000001f0: 5072 6573 656e 7461 7469 6f6e 9468 075d  Presentation.h.]
-00000200: 9468 168c 0c50 7265 7365 6e74 6174 696f  .h...Presentatio
-00000210: 6e94 8594 8194 7d94 2868 1b68 3068 1c68  n.....}.(h.h0h.h
-00000220: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00000230: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00000240: 295d 9475 682b 680f 681e 4b03 681d 682c  )].uh+h.h.K.h.h,
-00000250: 681b 682d 681c 6803 7562 6809 8c09 7061  h.h-h.h.ubh...pa
-00000260: 7261 6772 6170 6894 9394 2981 947d 9428  ragraph...)..}.(
-00000270: 6805 8c3e 4d61 696e 2063 6c61 7373 2075  h..>Main class u
-00000280: 7365 6420 666f 7220 636f 6e76 6572 7469  sed for converti
-00000290: 6e67 206d 7a44 6174 6120 6669 6c65 7320  ng mzData files 
-000002a0: 696e 746f 206d 6174 6c61 6220 6669 6c65  into matlab file
-000002b0: 732e 9468 075d 9468 168c 3e4d 6169 6e20  s..h.].h..>Main 
-000002c0: 636c 6173 7320 7573 6564 2066 6f72 2063  class used for c
-000002d0: 6f6e 7665 7274 696e 6720 6d7a 4461 7461  onverting mzData
-000002e0: 2066 696c 6573 2069 6e74 6f20 6d61 746c   files into matl
-000002f0: 6162 2066 696c 6573 2e94 8594 8194 7d94  ab files......}.
-00000300: 2868 1b68 4068 1c68 0368 1d4e 681e 4e75  (h.h@h.h.h.Nh.Nu
-00000310: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000320: 255d 9468 275d 9468 295d 9475 682b 683e  %].h'].h)].uh+h>
-00000330: 681e 4b04 681d 682c 681b 682d 681c 6803  h.K.h.h,h.h-h.h.
-00000340: 7562 6568 1f7d 9428 6821 5d94 8c0c 7072  ubeh.}.(h!]...pr
-00000350: 6573 656e 7461 7469 6f6e 9461 6823 5d94  esentation.ah#].
-00000360: 6825 5d94 6827 5d94 8c0c 7072 6573 656e  h%].h']...presen
-00000370: 7461 7469 6f6e 9461 6829 5d94 7568 2b68  tation.ah)].uh+h
-00000380: 0a68 1e4b 0368 1d68 2c68 1b68 0c68 1c68  .h.K.h.h,h.h.h.h
-00000390: 038c 0a72 6566 6572 656e 6365 6494 4b01  ...referenced.K.
-000003a0: 7562 680b 2981 947d 9428 6805 6806 6807  ubh.)..}.(h.h.h.
-000003b0: 5d94 2868 1029 8194 7d94 2868 058c 0a44  ].(h.)..}.(h...D
-000003c0: 6566 696e 6974 696f 6e94 6807 5d94 6816  efinition.h.].h.
-000003d0: 8c0a 4465 6669 6e69 7469 6f6e 9485 9481  ..Definition....
-000003e0: 947d 9428 681b 685a 681c 6803 681d 4e68  .}.(h.hZh.h.h.Nh
-000003f0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00000400: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00000410: 2b68 0f68 1e4b 0668 1d68 2c68 1b68 5768  +h.h.K.h.h,h.hWh
-00000420: 1c68 0375 6268 098c 0d6c 6974 6572 616c  .h.ubh...literal
-00000430: 5f62 6c6f 636b 9493 9429 8194 7d94 2868  _block...)..}.(h
-00000440: 058c 7763 6c61 7373 206d 7a44 6174 614d  ..wclass mzDataM
-00000450: 616e 6167 6572 2842 6173 654d 6f64 656c  anager(BaseModel
-00000460: 293a 0a20 2020 206d 7a44 6174 6150 6174  ):.    mzDataPat
-00000470: 6820 3a20 7374 7220 3d20 4e6f 6e65 0a20  h : str = None. 
-00000480: 2020 2065 7870 6f72 7450 6174 6820 3a20     exportPath : 
-00000490: 7374 7220 3d20 4e6f 6e65 0a20 2020 2075  str = None.    u
-000004a0: 7365 4469 7265 6374 6f72 7920 3a20 626f  seDirectory : bo
-000004b0: 6f6c 203d 2054 7275 650a 9468 075d 9468  ol = True..h.].h
-000004c0: 168c 7763 6c61 7373 206d 7a44 6174 614d  ..wclass mzDataM
-000004d0: 616e 6167 6572 2842 6173 654d 6f64 656c  anager(BaseModel
-000004e0: 293a 0a20 2020 206d 7a44 6174 6150 6174  ):.    mzDataPat
-000004f0: 6820 3a20 7374 7220 3d20 4e6f 6e65 0a20  h : str = None. 
-00000500: 2020 2065 7870 6f72 7450 6174 6820 3a20     exportPath : 
-00000510: 7374 7220 3d20 4e6f 6e65 0a20 2020 2075  str = None.    u
-00000520: 7365 4469 7265 6374 6f72 7920 3a20 626f  seDirectory : bo
-00000530: 6f6c 203d 2054 7275 650a 9485 9481 947d  ol = True......}
-00000540: 9468 1b68 6a73 6261 681f 7d94 2868 215d  .h.hjsbah.}.(h!]
-00000550: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00000560: 948c 086c 616e 6775 6167 6594 8c06 7079  ...language...py
-00000570: 7468 6f6e 948c 0978 6d6c 3a73 7061 6365  thon...xml:space
-00000580: 948c 0870 7265 7365 7276 6594 7568 2b68  ...preserve.uh+h
-00000590: 6868 1d68 2c68 1e4b 0768 1b68 5768 1c68  hh.h,h.K.h.hWh.h
-000005a0: 0375 6265 681f 7d94 2868 215d 948c 0a64  .ubeh.}.(h!]...d
-000005b0: 6566 696e 6974 696f 6e94 6168 235d 9468  efinition.ah#].h
-000005c0: 255d 9468 275d 948c 0a64 6566 696e 6974  %].h']...definit
-000005d0: 696f 6e94 6168 295d 9475 682b 680a 681e  ion.ah)].uh+h.h.
-000005e0: 4b06 681d 682c 681b 680c 681c 6803 6856  K.h.h,h.h.h.h.hV
-000005f0: 4b01 7562 680b 2981 947d 9428 6805 6806  K.ubh.)..}.(h.h.
-00000600: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
-00000610: 0a48 6f77 2074 6f20 7573 6594 6807 5d94  .How to use.h.].
-00000620: 6816 8c0a 486f 7720 746f 2075 7365 9485  h...How to use..
-00000630: 9481 947d 9428 681b 6887 681c 6803 681d  ...}.(h.h.h.h.h.
-00000640: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00000650: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00000660: 7568 2b68 0f68 1e4b 0e68 1d68 2c68 1b68  uh+h.h.K.h.h,h.h
-00000670: 8468 1c68 0375 6268 0b29 8194 7d94 2868  .h.h.ubh.)..}.(h
-00000680: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
-00000690: 6805 8c09 5769 7468 2070 6174 6894 6807  h...With path.h.
-000006a0: 5d94 6816 8c09 5769 7468 2070 6174 6894  ].h...With path.
-000006b0: 8594 8194 7d94 2868 1b68 9868 1c68 0368  ....}.(h.h.h.h.h
-000006c0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000006d0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-000006e0: 9475 682b 680f 681e 4b0f 681d 682c 681b  .uh+h.h.K.h.h,h.
-000006f0: 6895 681c 6803 7562 6869 2981 947d 9428  h.h.h.ubhi)..}.(
-00000700: 6805 8c5e 6d61 6e61 6765 7220 3d20 6d7a  h..^manager = mz
-00000710: 4461 7461 4d61 6e61 6765 7228 0a20 2020  DataManager(.   
-00000720: 206d 7a44 6174 6150 6174 6820 3d20 2253   mzDataPath = "S
-00000730: 6f6d 652f 5061 7468 222c 0a20 2020 2065  ome/Path",.    e
-00000740: 7870 6f72 7450 6174 6820 3d20 2253 6f6d  xportPath = "Som
-00000750: 652f 4578 706f 7274 2f50 6174 6822 2c0a  e/Export/Path",.
-00000760: 290a 9468 075d 9468 168c 5e6d 616e 6167  )..h.].h..^manag
-00000770: 6572 203d 206d 7a44 6174 614d 616e 6167  er = mzDataManag
-00000780: 6572 280a 2020 2020 6d7a 4461 7461 5061  er(.    mzDataPa
-00000790: 7468 203d 2022 536f 6d65 2f50 6174 6822  th = "Some/Path"
-000007a0: 2c0a 2020 2020 6578 706f 7274 5061 7468  ,.    exportPath
-000007b0: 203d 2022 536f 6d65 2f45 7870 6f72 742f   = "Some/Export/
-000007c0: 5061 7468 222c 0a29 0a94 8594 8194 7d94  Path",.)......}.
-000007d0: 681b 68a6 7362 6168 1f7d 9428 6821 5d94  h.h.sbah.}.(h!].
-000007e0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000007f0: 8c08 6c61 6e67 7561 6765 948c 0670 7974  ..language...pyt
-00000800: 686f 6e94 687a 687b 7568 2b68 6868 1d68  hon.hzh{uh+hhh.h
-00000810: 2c68 1e4b 1068 1b68 9568 1c68 0375 6268  ,h.K.h.h.h.h.ubh
-00000820: 3f29 8194 7d94 2868 058c a654 6865 2070  ?)..}.(h...The p
-00000830: 6174 6820 796f 7520 7370 6563 6966 7920  ath you specify 
-00000840: 696e 2074 686f 7365 2061 7267 756d 656e  in those argumen
-00000850: 7473 2077 696c 6c20 6265 2073 746f 7265  ts will be store
-00000860: 6420 696e 2074 6865 2063 6c61 7373 2c20  d in the class, 
-00000870: 736f 2077 6865 6e20 796f 7520 7573 6520  so when you use 
-00000880: 7468 6520 696e 7465 6772 6174 6564 2066  the integrated f
-00000890: 756e 6374 696f 6e73 2c20 796f 7520 6f6e  unctions, you on
-000008a0: 6c79 206e 6565 6420 746f 2073 7065 6369  ly need to speci
-000008b0: 6679 2074 6865 2072 656c 6174 6976 6520  fy the relative 
-000008c0: 7061 7468 2074 6f20 7468 6520 6669 6c65  path to the file
-000008d0: 2e94 6807 5d94 6816 8ca6 5468 6520 7061  ..h.].h...The pa
-000008e0: 7468 2079 6f75 2073 7065 6369 6679 2069  th you specify i
-000008f0: 6e20 7468 6f73 6520 6172 6775 6d65 6e74  n those argument
-00000900: 7320 7769 6c6c 2062 6520 7374 6f72 6564  s will be stored
-00000910: 2069 6e20 7468 6520 636c 6173 732c 2073   in the class, s
-00000920: 6f20 7768 656e 2079 6f75 2075 7365 2074  o when you use t
-00000930: 6865 2069 6e74 6567 7261 7465 6420 6675  he integrated fu
-00000940: 6e63 7469 6f6e 732c 2079 6f75 206f 6e6c  nctions, you onl
-00000950: 7920 6e65 6564 2074 6f20 7370 6563 6966  y need to specif
-00000960: 7920 7468 6520 7265 6c61 7469 7665 2070  y the relative p
-00000970: 6174 6820 746f 2074 6865 2066 696c 652e  ath to the file.
-00000980: 9485 9481 947d 9428 681b 68b6 681c 6803  .....}.(h.h.h.h.
-00000990: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-000009a0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-000009b0: 5d94 7568 2b68 3e68 1e4b 1668 1d68 2c68  ].uh+h>h.K.h.h,h
-000009c0: 1b68 9568 1c68 0375 6265 681f 7d94 2868  .h.h.h.ubeh.}.(h
-000009d0: 215d 948c 0977 6974 682d 7061 7468 9461  !]...with-path.a
-000009e0: 6823 5d94 6825 5d94 8c09 7769 7468 2070  h#].h%]...with p
-000009f0: 6174 6894 6168 275d 9468 295d 9475 682b  ath.ah'].h)].uh+
-00000a00: 680a 681e 4b0f 681d 682c 681b 6884 681c  h.h.K.h.h,h.h.h.
-00000a10: 6803 7562 680b 2981 947d 9428 6805 6806  h.ubh.)..}.(h.h.
-00000a20: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
-00000a30: 0c57 6974 686f 7574 2070 6174 6894 6807  .Without path.h.
-00000a40: 5d94 6816 8c0c 5769 7468 6f75 7420 7061  ].h...Without pa
-00000a50: 7468 9485 9481 947d 9428 681b 68cf 681c  th.....}.(h.h.h.
-00000a60: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00000a70: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00000a80: 6829 5d94 7568 2b68 0f68 1e4b 1868 1d68  h)].uh+h.h.K.h.h
-00000a90: 2c68 1b68 cc68 1c68 0375 6268 6929 8194  ,h.h.h.h.ubhi)..
-00000aa0: 7d94 2868 058c 2c6d 616e 6167 6572 203d  }.(h..,manager =
-00000ab0: 206d 7a44 6174 614d 616e 6167 6572 2875   mzDataManager(u
-00000ac0: 7365 4469 7265 6374 6f72 793d 4661 6c73  seDirectory=Fals
-00000ad0: 6529 0a94 6807 5d94 6816 8c2c 6d61 6e61  e)..h.].h..,mana
-00000ae0: 6765 7220 3d20 6d7a 4461 7461 4d61 6e61  ger = mzDataMana
-00000af0: 6765 7228 7573 6544 6972 6563 746f 7279  ger(useDirectory
-00000b00: 3d46 616c 7365 290a 9485 9481 947d 9468  =False)......}.h
-00000b10: 1b68 dd73 6261 681f 7d94 2868 215d 9468  .h.sbah.}.(h!].h
-00000b20: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
-00000b30: 086c 616e 6775 6167 6594 8c06 7079 7468  .language...pyth
-00000b40: 6f6e 9468 7a68 7b75 682b 6868 681d 682c  on.hzh{uh+hhh.h,
-00000b50: 681e 4b19 681b 68cc 681c 6803 7562 683f  h.K.h.h.h.h.ubh?
-00000b60: 2981 947d 9428 6805 8c83 5365 7474 696e  )..}.(h...Settin
-00000b70: 6720 7570 2074 6865 2063 6c61 7373 2074  g up the class t
-00000b80: 6869 7320 7761 7920 7769 6c6c 2072 6571  his way will req
-00000b90: 7569 7265 2074 6f20 7370 6563 6966 7920  uire to specify 
-00000ba0: 6561 6368 2074 696d 6520 796f 7520 6361  each time you ca
-00000bb0: 6c6c 2061 2066 756e 6374 696f 6e20 746f  ll a function to
-00000bc0: 2067 6976 6520 7468 6520 6675 6c6c 2070   give the full p
-00000bd0: 6174 6820 616e 6420 7468 6520 6578 706f  ath and the expo
-00000be0: 7274 2064 6972 6563 746f 7279 2e94 6807  rt directory..h.
-00000bf0: 5d94 6816 8c83 5365 7474 696e 6720 7570  ].h...Setting up
-00000c00: 2074 6865 2063 6c61 7373 2074 6869 7320   the class this 
-00000c10: 7761 7920 7769 6c6c 2072 6571 7569 7265  way will require
-00000c20: 2074 6f20 7370 6563 6966 7920 6561 6368   to specify each
-00000c30: 2074 696d 6520 796f 7520 6361 6c6c 2061   time you call a
-00000c40: 2066 756e 6374 696f 6e20 746f 2067 6976   function to giv
-00000c50: 6520 7468 6520 6675 6c6c 2070 6174 6820  e the full path 
-00000c60: 616e 6420 7468 6520 6578 706f 7274 2064  and the export d
-00000c70: 6972 6563 746f 7279 2e94 8594 8194 7d94  irectory......}.
-00000c80: 2868 1b68 ed68 1c68 0368 1d4e 681e 4e75  (h.h.h.h.h.Nh.Nu
-00000c90: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000ca0: 255d 9468 275d 9468 295d 9475 682b 683e  %].h'].h)].uh+h>
-00000cb0: 681e 4b1c 681d 682c 681b 68cc 681c 6803  h.K.h.h,h.h.h.h.
-00000cc0: 7562 6568 1f7d 9428 6821 5d94 8c0c 7769  ubeh.}.(h!]...wi
-00000cd0: 7468 6f75 742d 7061 7468 9461 6823 5d94  thout-path.ah#].
-00000ce0: 6825 5d94 8c0c 7769 7468 6f75 7420 7061  h%]...without pa
-00000cf0: 7468 9461 6827 5d94 6829 5d94 7568 2b68  th.ah'].h)].uh+h
-00000d00: 0a68 1e4b 1868 1d68 2c68 1b68 8468 1c68  .h.K.h.h,h.h.h.h
-00000d10: 0375 6265 681f 7d94 2868 215d 948c 0a68  .ubeh.}.(h!]...h
-00000d20: 6f77 2d74 6f2d 7573 6594 6168 235d 9468  ow-to-use.ah#].h
-00000d30: 255d 9468 275d 948c 0a68 6f77 2074 6f20  %].h']...how to 
-00000d40: 7573 6594 6168 295d 9475 682b 680a 681e  use.ah)].uh+h.h.
-00000d50: 4b0e 681d 682c 681b 680c 681c 6803 6856  K.h.h,h.h.h.h.hV
-00000d60: 4b01 7562 680b 2981 947d 9428 6805 6806  K.ubh.)..}.(h.h.
-00000d70: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
-00000d80: 0946 756e 6374 696f 6e73 9468 075d 9468  .Functions.h.].h
-00000d90: 168c 0946 756e 6374 696f 6e73 9485 9481  ...Functions....
-00000da0: 947d 9428 681b 6a0e 0100 0068 1c68 0368  .}.(h.j....h.h.h
-00000db0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00000dc0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00000dd0: 9475 682b 680f 681e 4b1e 681d 682c 681b  .uh+h.h.K.h.h,h.
-00000de0: 6a0b 0100 0068 1c68 0375 6268 0b29 8194  j....h.h.ubh.)..
-00000df0: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
-00000e00: 947d 9428 6805 8c0d 6d7a 4461 7461 584d  .}.(h...mzDataXM
-00000e10: 4c72 6561 6494 6807 5d94 6816 8c0d 6d7a  Lread.h.].h...mz
-00000e20: 4461 7461 584d 4c72 6561 6494 8594 8194  DataXMLread.....
-00000e30: 7d94 2868 1b6a 1f01 0000 681c 6803 681d  }.(h.j....h.h.h.
-00000e40: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00000e50: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00000e60: 7568 2b68 0f68 1e4b 2068 1d68 2c68 1b6a  uh+h.h.K h.h,h.j
-00000e70: 1c01 0000 681c 6803 7562 680b 2981 947d  ....h.h.ubh.)..}
-00000e80: 9428 6805 6806 6807 5d94 2868 1029 8194  .(h.h.h.].(h.)..
-00000e90: 7d94 2868 058c 0c50 7265 7365 6e74 6174  }.(h...Presentat
-00000ea0: 696f 6e94 6807 5d94 6816 8c0c 5072 6573  ion.h.].h...Pres
-00000eb0: 656e 7461 7469 6f6e 9485 9481 947d 9428  entation.....}.(
-00000ec0: 681b 6a30 0100 0068 1c68 0368 1d4e 681e  h.j0...h.h.h.Nh.
-00000ed0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00000ee0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00000ef0: 680f 681e 4b22 681d 682c 681b 6a2d 0100  h.h.K"h.h,h.j-..
-00000f00: 0068 1c68 0375 6268 3f29 8194 7d94 2868  .h.h.ubh?)..}.(h
-00000f10: 058c bd54 6869 7320 6675 6e63 7469 6f6e  ...This function
-00000f20: 2072 6561 6473 2061 2060 2e6d 7a44 6174   reads a `.mzDat
-00000f30: 612e 786d 6c60 2066 696c 6520 616e 6420  a.xml` file and 
-00000f40: 7265 7475 726e 7320 6120 606d 7a44 6174  returns a `mzDat
-00000f50: 6160 2073 7472 7563 7475 7265 2077 6869  a` structure whi
-00000f60: 6368 2063 616e 2062 6520 6d6f 6469 6669  ch can be modifi
-00000f70: 6564 2062 6566 6f72 6520 7361 7669 6e67  ed before saving
-00000f80: 2069 7427 7320 6461 7461 2074 6f20 6120   it's data to a 
-00000f90: 602e 6d61 7460 2066 696c 6520 2853 6565  `.mat` file (See
-00000fa0: 205b 6d7a 4461 7461 5d28 6d7a 4461 7461   [mzData](mzData
-00000fb0: 2e6d 6429 2063 6c61 7373 2066 6f72 2066  .md) class for f
-00000fc0: 7572 7468 6572 2064 6574 6169 6c73 292e  urther details).
-00000fd0: 9468 075d 9428 6816 8c16 5468 6973 2066  .h.].(h...This f
-00000fe0: 756e 6374 696f 6e20 7265 6164 7320 6120  unction reads a 
-00000ff0: 9485 9481 947d 9428 681b 6a3e 0100 0068  .....}.(h.j>...h
-00001000: 1c68 0368 1d4e 681e 4e75 6268 098c 076c  .h.h.Nh.Nubh...l
-00001010: 6974 6572 616c 9493 9429 8194 7d94 2868  iteral...)..}.(h
-00001020: 058c 0b2e 6d7a 4461 7461 2e78 6d6c 9468  ....mzData.xml.h
-00001030: 075d 9468 168c 0b2e 6d7a 4461 7461 2e78  .].h....mzData.x
-00001040: 6d6c 9485 9481 947d 9428 681b 6a48 0100  ml.....}.(h.jH..
-00001050: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00001060: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00001070: 275d 9468 295d 9475 682b 6a46 0100 0068  '].h)].uh+jF...h
-00001080: 1e4b 2368 1d68 2c68 1b6a 3e01 0000 681c  .K#h.h,h.j>...h.
-00001090: 6803 7562 6816 8c14 2066 696c 6520 616e  h.ubh... file an
-000010a0: 6420 7265 7475 726e 7320 6120 9485 9481  d returns a ....
-000010b0: 947d 9428 681b 6a3e 0100 0068 1c68 0368  .}.(h.j>...h.h.h
-000010c0: 1d4e 681e 4e75 626a 4701 0000 2981 947d  .Nh.NubjG...)..}
-000010d0: 9428 6805 8c06 6d7a 4461 7461 9468 075d  .(h...mzData.h.]
-000010e0: 9468 168c 066d 7a44 6174 6194 8594 8194  .h...mzData.....
-000010f0: 7d94 2868 1b6a 5a01 0000 681c 6803 681d  }.(h.jZ...h.h.h.
-00001100: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00001110: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00001120: 7568 2b6a 4601 0000 681e 4b23 681d 682c  uh+jF...h.K#h.h,
-00001130: 681b 6a3e 0100 0068 1c68 0375 6268 168c  h.j>...h.h.ubh..
-00001140: 4020 7374 7275 6374 7572 6520 7768 6963  @ structure whic
-00001150: 6820 6361 6e20 6265 206d 6f64 6966 6965  h can be modifie
-00001160: 6420 6265 666f 7265 2073 6176 696e 6720  d before saving 
-00001170: 6974 e280 9973 2064 6174 6120 746f 2061  it...s data to a
-00001180: 2094 8594 8194 7d94 2868 1b6a 3e01 0000   .....}.(h.j>...
-00001190: 681c 6803 681d 4e68 1e4e 7562 6a47 0100  h.h.h.Nh.NubjG..
-000011a0: 0029 8194 7d94 2868 058c 042e 6d61 7494  .)..}.(h....mat.
-000011b0: 6807 5d94 6816 8c04 2e6d 6174 9485 9481  h.].h....mat....
-000011c0: 947d 9428 681b 6a6c 0100 0068 1c68 0368  .}.(h.jl...h.h.h
-000011d0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000011e0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-000011f0: 9475 682b 6a46 0100 0068 1e4b 2368 1d68  .uh+jF...h.K#h.h
-00001200: 2c68 1b6a 3e01 0000 681c 6803 7562 6816  ,h.j>...h.h.ubh.
-00001210: 8c0b 2066 696c 6520 2853 6565 2094 8594  .. file (See ...
-00001220: 8194 7d94 2868 1b6a 3e01 0000 681c 6803  ..}.(h.j>...h.h.
-00001230: 681d 4e68 1e4e 7562 6800 8c0c 7065 6e64  h.Nh.Nubh...pend
-00001240: 696e 675f 7872 6566 9493 9429 8194 7d94  ing_xref...)..}.
-00001250: 2868 0568 0668 075d 9468 098c 0669 6e6c  (h.h.h.].h...inl
-00001260: 696e 6594 9394 2981 947d 9428 6805 8c06  ine...)..}.(h...
-00001270: 6d7a 4461 7461 9468 075d 9468 168c 066d  mzData.h.].h...m
-00001280: 7a44 6174 6194 8594 8194 7d94 2868 1b6a  zData.....}.(h.j
-00001290: 8501 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-000012a0: 6168 1f7d 9428 6821 5d94 6823 5d94 288c  ah.}.(h!].h#].(.
-000012b0: 0478 7265 6694 8c04 6d79 7374 9465 6825  .xref...myst.eh%
-000012c0: 5d94 6827 5d94 6829 5d94 7568 2b6a 8301  ].h'].h)].uh+j..
-000012d0: 0000 681b 6a80 0100 0068 1c68 0368 1d68  ..h.j....h.h.h.h
-000012e0: 2c68 1e4b 0075 6261 681f 7d94 2868 215d  ,h.K.ubah.}.(h!]
-000012f0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001300: 948c 0972 6566 646f 6d61 696e 948c 0364  ...refdomain...d
-00001310: 6f63 948c 0972 6566 7461 7267 6574 948c  oc...reftarget..
-00001320: 066d 7a44 6174 6194 8c0b 7265 6674 6172  .mzData...reftar
-00001330: 6765 7469 6494 4e8c 0672 6566 646f 6394  getid.N..refdoc.
-00001340: 8c0d 6d7a 4461 7461 4d61 6e61 6765 7294  ..mzDataManager.
-00001350: 8c07 7265 6674 7970 6594 6a91 0100 008c  ..reftype.j.....
-00001360: 0b72 6566 6578 706c 6963 6974 9488 7568  .refexplicit..uh
-00001370: 2b6a 7e01 0000 681e 4b23 681d 682c 681b  +j~...h.K#h.h,h.
-00001380: 6a3e 0100 0068 1c68 0375 6268 168c 1c20  j>...h.h.ubh... 
-00001390: 636c 6173 7320 666f 7220 6675 7274 6865  class for furthe
-000013a0: 7220 6465 7461 696c 7329 2e94 8594 8194  r details)......
-000013b0: 7d94 2868 1b6a 3e01 0000 681c 6803 681d  }.(h.j>...h.h.h.
-000013c0: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
-000013d0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000013e0: 7568 2b68 3e68 1e4b 2368 1d68 2c68 1b6a  uh+h>h.K#h.h,h.j
-000013f0: 2d01 0000 681c 6803 7562 6568 1f7d 9428  -...h.h.ubeh.}.(
-00001400: 6821 5d94 8c03 6964 3194 6168 235d 9468  h!]...id1.ah#].h
-00001410: 255d 9468 275d 9468 5461 6829 5d94 7568  %].h'].hTah)].uh
-00001420: 2b68 0a68 1e4b 2268 1d68 2c68 1b6a 1c01  +h.h.K"h.h,h.j..
-00001430: 0000 681c 6803 6856 4b01 7562 680b 2981  ..h.h.hVK.ubh.).
-00001440: 947d 9428 6805 6806 6807 5d94 2868 1029  .}.(h.h.h.].(h.)
-00001450: 8194 7d94 2868 058c 0a44 6566 696e 6974  ..}.(h...Definit
-00001460: 696f 6e94 6807 5d94 6816 8c0a 4465 6669  ion.h.].h...Defi
-00001470: 6e69 7469 6f6e 9485 9481 947d 9428 681b  nition.....}.(h.
-00001480: 6ab8 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00001490: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-000014a0: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
-000014b0: 681e 4b25 681d 682c 681b 6ab5 0100 0068  h.K%h.h,h.j....h
-000014c0: 1c68 0375 6268 6929 8194 7d94 2868 058c  .h.ubhi)..}.(h..
-000014d0: 5664 6566 206d 7a44 6174 6158 4d4c 7265  Vdef mzDataXMLre
-000014e0: 6164 2873 656c 6640 6d7a 4461 7461 4d61  ad(self@mzDataMa
-000014f0: 6e61 6765 722c 2066 696c 654e 616d 6520  nager, fileName 
-00001500: 3a20 7374 722c 2063 7573 746f 6d44 6972  : str, customDir
-00001510: 6563 746f 7279 203a 2062 6f6f 6c20 3d20  ectory : bool = 
-00001520: 4661 6c73 6529 0a94 6807 5d94 6816 8c56  False)..h.].h..V
-00001530: 6465 6620 6d7a 4461 7461 584d 4c72 6561  def mzDataXMLrea
-00001540: 6428 7365 6c66 406d 7a44 6174 614d 616e  d(self@mzDataMan
-00001550: 6167 6572 2c20 6669 6c65 4e61 6d65 203a  ager, fileName :
-00001560: 2073 7472 2c20 6375 7374 6f6d 4469 7265   str, customDire
-00001570: 6374 6f72 7920 3a20 626f 6f6c 203d 2046  ctory : bool = F
-00001580: 616c 7365 290a 9485 9481 947d 9468 1b6a  alse)......}.h.j
-00001590: c601 0000 7362 6168 1f7d 9428 6821 5d94  ....sbah.}.(h!].
-000015a0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000015b0: 8c08 6c61 6e67 7561 6765 948c 0670 7974  ..language...pyt
-000015c0: 686f 6e94 687a 687b 7568 2b68 6868 1d68  hon.hzh{uh+hhh.h
-000015d0: 2c68 1e4b 2668 1b6a b501 0000 681c 6803  ,h.K&h.j....h.h.
-000015e0: 7562 6568 1f7d 9428 6821 5d94 8c03 6964  ubeh.}.(h!]...id
-000015f0: 3294 6168 235d 9468 255d 9468 275d 9468  2.ah#].h%].h'].h
-00001600: 8261 6829 5d94 7568 2b68 0a68 1e4b 2568  .ah)].uh+h.h.K%h
-00001610: 1d68 2c68 1b6a 1c01 0000 681c 6803 6856  .h,h.j....h.h.hV
-00001620: 4b01 7562 680b 2981 947d 9428 6805 6806  K.ubh.)..}.(h.h.
-00001630: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
-00001640: 0a48 6f77 2074 6f20 7573 6594 6807 5d94  .How to use.h.].
-00001650: 6816 8c0a 486f 7720 746f 2075 7365 9485  h...How to use..
-00001660: 9481 947d 9428 681b 6ae0 0100 0068 1c68  ...}.(h.j....h.h
-00001670: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00001680: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00001690: 295d 9475 682b 680f 681e 4b2a 681d 682c  )].uh+h.h.K*h.h,
-000016a0: 681b 6add 0100 0068 1c68 0375 6268 6929  h.j....h.h.ubhi)
-000016b0: 8194 7d94 2868 058c 9c23 2043 6f6e 7369  ..}.(h...# Consi
-000016c0: 6465 7269 6e67 2074 6861 7420 6d7a 4461  dering that mzDa
-000016d0: 7461 4d61 6e61 6765 7220 636c 6173 7320  taManager class 
-000016e0: 6861 7320 6265 656e 2069 6e74 6961 6c69  has been intiali
-000016f0: 7a65 6420 6265 666f 7265 2061 6e64 2073  zed before and s
-00001700: 746f 7265 6420 6173 206d 616e 6167 6572  tored as manager
-00001710: 2076 6172 6961 626c 650a 0a63 6f6e 7465   variable..conte
-00001720: 6e74 203d 206d 616e 6167 6572 2e6d 7a44  nt = manager.mzD
-00001730: 6174 6158 4d4c 7265 6164 280a 2020 2020  ataXMLread(.    
-00001740: 6669 6c65 4e61 6d65 3d50 6174 6832 4669  fileName=Path2Fi
-00001750: 6c65 0a29 0a94 6807 5d94 6816 8c9c 2320  le.)..h.].h...# 
-00001760: 436f 6e73 6964 6572 696e 6720 7468 6174  Considering that
-00001770: 206d 7a44 6174 614d 616e 6167 6572 2063   mzDataManager c
-00001780: 6c61 7373 2068 6173 2062 6565 6e20 696e  lass has been in
-00001790: 7469 616c 697a 6564 2062 6566 6f72 6520  tialized before 
-000017a0: 616e 6420 7374 6f72 6564 2061 7320 6d61  and stored as ma
-000017b0: 6e61 6765 7220 7661 7269 6162 6c65 0a0a  nager variable..
-000017c0: 636f 6e74 656e 7420 3d20 6d61 6e61 6765  content = manage
-000017d0: 722e 6d7a 4461 7461 584d 4c72 6561 6428  r.mzDataXMLread(
-000017e0: 0a20 2020 2066 696c 654e 616d 653d 5061  .    fileName=Pa
-000017f0: 7468 3246 696c 650a 290a 9485 9481 947d  th2File.)......}
-00001800: 9468 1b6a ee01 0000 7362 6168 1f7d 9428  .h.j....sbah.}.(
-00001810: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00001820: 6829 5d94 8c08 6c61 6e67 7561 6765 948c  h)]...language..
-00001830: 0670 7974 686f 6e94 687a 687b 7568 2b68  .python.hzh{uh+h
-00001840: 6868 1d68 2c68 1e4b 2b68 1b6a dd01 0000  hh.h,h.K+h.j....
-00001850: 681c 6803 7562 683f 2981 947d 9428 6805  h.h.ubh?)..}.(h.
-00001860: 8c11 3c75 3e50 6172 616d 6574 6572 733c  ..<u>Parameters<
-00001870: 2f75 3e94 6807 5d94 2868 098c 0372 6177  /u>.h.].(h...raw
-00001880: 9493 9429 8194 7d94 2868 058c 033c 753e  ...)..}.(h...<u>
-00001890: 9468 075d 9468 168c 033c 753e 9485 9481  .h.].h...<u>....
-000018a0: 947d 9428 681b 6a04 0200 0068 1c68 0368  .}.(h.j....h.h.h
-000018b0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000018c0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-000018d0: 948c 0666 6f72 6d61 7494 8c04 6874 6d6c  ...format...html
-000018e0: 9468 7a68 7b75 682b 6a02 0200 0068 1d68  .hzh{uh+j....h.h
-000018f0: 2c68 1e4b 3268 1b6a fe01 0000 681c 6803  ,h.K2h.j....h.h.
-00001900: 7562 6816 8c0a 5061 7261 6d65 7465 7273  ubh...Parameters
-00001910: 9485 9481 947d 9428 681b 6afe 0100 0068  .....}.(h.j....h
-00001920: 1c68 0368 1d4e 681e 4e75 626a 0302 0000  .h.h.Nh.Nubj....
-00001930: 2981 947d 9428 6805 8c04 3c2f 753e 9468  )..}.(h...</u>.h
-00001940: 075d 9468 168c 043c 2f75 3e94 8594 8194  .].h...</u>.....
-00001950: 7d94 2868 1b6a 1802 0000 681c 6803 681d  }.(h.j....h.h.h.
-00001960: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00001970: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00001980: 8c06 666f 726d 6174 946a 1302 0000 687a  ..format.j....hz
-00001990: 687b 7568 2b6a 0202 0000 681d 682c 681e  h{uh+j....h.h,h.
-000019a0: 4b32 681b 6afe 0100 0068 1c68 0375 6265  K2h.j....h.h.ube
-000019b0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-000019c0: 9468 275d 9468 295d 9475 682b 683e 681e  .h'].h)].uh+h>h.
-000019d0: 4b32 681d 682c 681b 6add 0100 0068 1c68  K2h.h,h.j....h.h
-000019e0: 0375 6268 098c 0b62 756c 6c65 745f 6c69  .ubh...bullet_li
-000019f0: 7374 9493 9429 8194 7d94 2868 0568 0668  st...)..}.(h.h.h
-00001a00: 075d 9428 6809 8c09 6c69 7374 5f69 7465  .].(h...list_ite
-00001a10: 6d94 9394 2981 947d 9428 6805 6806 6807  m...)..}.(h.h.h.
-00001a20: 5d94 2868 3f29 8194 7d94 2868 058c 3249  ].(h?)..}.(h..2I
-00001a30: 6620 6469 7265 6374 6f72 6965 7320 7765  f directories we
-00001a40: 7265 2070 726f 7669 6465 6420 696e 2074  re provided in t
-00001a50: 6865 2069 6e69 7420 7072 6f63 6573 7320  he init process 
-00001a60: 3a94 6807 5d94 6816 8c32 4966 2064 6972  :.h.].h..2If dir
-00001a70: 6563 746f 7269 6573 2077 6572 6520 7072  ectories were pr
-00001a80: 6f76 6964 6564 2069 6e20 7468 6520 696e  ovided in the in
-00001a90: 6974 2070 726f 6365 7373 203a 9485 9481  it process :....
-00001aa0: 947d 9428 681b 6a37 0200 0068 1c68 0368  .}.(h.j7...h.h.h
-00001ab0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00001ac0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001ad0: 9475 682b 683e 681e 4b33 681d 682c 681b  .uh+h>h.K3h.h,h.
-00001ae0: 6a34 0200 0068 1c68 0375 626a 2e02 0000  j4...h.h.ubj....
-00001af0: 2981 947d 9428 6805 6806 6807 5d94 286a  )..}.(h.h.h.].(j
-00001b00: 3302 0000 2981 947d 9428 6805 6806 6807  3...)..}.(h.h.h.
-00001b10: 5d94 683f 2981 947d 9428 6805 8c3b 6066  ].h?)..}.(h..;`f
-00001b20: 696c 654e 616d 6560 203a 2052 656c 6174  ileName` : Relat
-00001b30: 6976 6520 7061 7468 206f 6620 7468 6520  ive path of the 
-00001b40: 606d 7a44 6174 612e 786d 6c60 2066 696c  `mzData.xml` fil
-00001b50: 6520 746f 2072 6561 6494 6807 5d94 286a  e to read.h.].(j
-00001b60: 4701 0000 2981 947d 9428 6805 8c08 6669  G...)..}.(h...fi
-00001b70: 6c65 4e61 6d65 9468 075d 9468 168c 0866  leName.h.].h...f
-00001b80: 696c 654e 616d 6594 8594 8194 7d94 2868  ileName.....}.(h
-00001b90: 1b6a 4f02 0000 681c 6803 681d 4e68 1e4e  .jO...h.h.h.Nh.N
-00001ba0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00001bb0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00001bc0: 4601 0000 681e 4b34 681d 682c 681b 6a4b  F...h.K4h.h,h.jK
-00001bd0: 0200 0068 1c68 0375 6268 168c 1820 3a20  ...h.h.ubh... : 
-00001be0: 5265 6c61 7469 7665 2070 6174 6820 6f66  Relative path of
-00001bf0: 2074 6865 2094 8594 8194 7d94 2868 1b6a   the .....}.(h.j
-00001c00: 4b02 0000 681c 6803 681d 4e68 1e4e 7562  K...h.h.h.Nh.Nub
-00001c10: 6a47 0100 0029 8194 7d94 2868 058c 0a6d  jG...)..}.(h...m
-00001c20: 7a44 6174 612e 786d 6c94 6807 5d94 6816  zData.xml.h.].h.
-00001c30: 8c0a 6d7a 4461 7461 2e78 6d6c 9485 9481  ..mzData.xml....
-00001c40: 947d 9428 681b 6a61 0200 0068 1c68 0368  .}.(h.ja...h.h.h
-00001c50: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00001c60: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001c70: 9475 682b 6a46 0100 0068 1e4b 3468 1d68  .uh+jF...h.K4h.h
-00001c80: 2c68 1b6a 4b02 0000 681c 6803 7562 6816  ,h.jK...h.h.ubh.
-00001c90: 8c0d 2066 696c 6520 746f 2072 6561 6494  .. file to read.
-00001ca0: 8594 8194 7d94 2868 1b6a 4b02 0000 681c  ....}.(h.jK...h.
-00001cb0: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
-00001cc0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00001cd0: 6829 5d94 7568 2b68 3e68 1e4b 3468 1d68  h)].uh+h>h.K4h.h
-00001ce0: 2c68 1b6a 4802 0000 681c 6803 7562 6168  ,h.jH...h.h.ubah
-00001cf0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00001d00: 6827 5d94 6829 5d94 7568 2b6a 3202 0000  h'].h)].uh+j2...
-00001d10: 681e 4b34 681d 682c 681b 6a45 0200 0068  h.K4h.h,h.jE...h
-00001d20: 1c68 0375 626a 3302 0000 2981 947d 9428  .h.ubj3...)..}.(
-00001d30: 6805 6806 6807 5d94 683f 2981 947d 9428  h.h.h.].h?)..}.(
-00001d40: 6805 8c8a 6063 7573 746f 6d44 6972 6563  h...`customDirec
-00001d50: 746f 7279 6020 3a20 5365 7420 7468 6973  tory` : Set this
-00001d60: 2070 6172 616d 6574 6572 2074 6f20 6054   parameter to `T
-00001d70: 7275 6560 2069 6620 796f 7520 7072 6f76  rue` if you prov
-00001d80: 6964 6520 6120 6675 6c6c 2070 6174 6820  ide a full path 
-00001d90: 7768 6963 6820 6973 2064 6966 6665 7265  which is differe
-00001da0: 6e74 2074 6861 6e20 7468 6520 6f6e 6520  nt than the one 
-00001db0: 7370 6563 6966 6965 6420 696e 2074 6865  specified in the
-00001dc0: 2069 6e69 7420 7072 6f63 6573 732e 9468   init process..h
-00001dd0: 075d 9428 6a47 0100 0029 8194 7d94 2868  .].(jG...)..}.(h
-00001de0: 058c 0f63 7573 746f 6d44 6972 6563 746f  ...customDirecto
-00001df0: 7279 9468 075d 9468 168c 0f63 7573 746f  ry.h.].h...custo
-00001e00: 6d44 6972 6563 746f 7279 9485 9481 947d  mDirectory.....}
-00001e10: 9428 681b 6a86 0200 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00001e20: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00001e30: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00001e40: 682b 6a46 0100 0068 1e4b 3568 1d68 2c68  h+jF...h.K5h.h,h
-00001e50: 1b6a 8202 0000 681c 6803 7562 6816 8c19  .j....h.h.ubh...
-00001e60: 203a 2053 6574 2074 6869 7320 7061 7261   : Set this para
-00001e70: 6d65 7465 7220 746f 2094 8594 8194 7d94  meter to .....}.
-00001e80: 2868 1b6a 8202 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-00001e90: 1e4e 7562 6a47 0100 0029 8194 7d94 2868  .NubjG...)..}.(h
-00001ea0: 058c 0454 7275 6594 6807 5d94 6816 8c04  ...True.h.].h...
-00001eb0: 5472 7565 9485 9481 947d 9428 681b 6a98  True.....}.(h.j.
-00001ec0: 0200 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00001ed0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00001ee0: 9468 275d 9468 295d 9475 682b 6a46 0100  .h'].h)].uh+jF..
-00001ef0: 0068 1e4b 3568 1d68 2c68 1b6a 8202 0000  .h.K5h.h,h.j....
-00001f00: 681c 6803 7562 6816 8c5a 2069 6620 796f  h.h.ubh..Z if yo
-00001f10: 7520 7072 6f76 6964 6520 6120 6675 6c6c  u provide a full
-00001f20: 2070 6174 6820 7768 6963 6820 6973 2064   path which is d
-00001f30: 6966 6665 7265 6e74 2074 6861 6e20 7468  ifferent than th
-00001f40: 6520 6f6e 6520 7370 6563 6966 6965 6420  e one specified 
-00001f50: 696e 2074 6865 2069 6e69 7420 7072 6f63  in the init proc
-00001f60: 6573 732e 9485 9481 947d 9428 681b 6a82  ess......}.(h.j.
-00001f70: 0200 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
-00001f80: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00001f90: 9468 275d 9468 295d 9475 682b 683e 681e  .h'].h)].uh+h>h.
-00001fa0: 4b35 681d 682c 681b 6a7f 0200 0068 1c68  K5h.h,h.j....h.h
-00001fb0: 0375 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
-00001fc0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00001fd0: 6a32 0200 0068 1e4b 3568 1d68 2c68 1b6a  j2...h.K5h.h,h.j
-00001fe0: 4502 0000 681c 6803 7562 6568 1f7d 9428  E...h.h.ubeh.}.(
-00001ff0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00002000: 6829 5d94 8c06 6275 6c6c 6574 948c 012d  h)]...bullet...-
-00002010: 9475 682b 6a2d 0200 0068 1e4b 3468 1d68  .uh+j-...h.K4h.h
-00002020: 2c68 1b6a 3402 0000 681c 6803 7562 6568  ,h.j4...h.h.ubeh
-00002030: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00002040: 6827 5d94 6829 5d94 7568 2b6a 3202 0000  h'].h)].uh+j2...
-00002050: 681e 4b33 681d 682c 681b 6a2f 0200 0068  h.K3h.h,h.j/...h
-00002060: 1c68 0375 626a 3302 0000 2981 947d 9428  .h.ubj3...)..}.(
-00002070: 6805 6806 6807 5d94 2868 3f29 8194 7d94  h.h.h.].(h?)..}.
-00002080: 2868 058c 0b4f 7468 6572 7769 7365 203a  (h...Otherwise :
-00002090: 9468 075d 9468 168c 0b4f 7468 6572 7769  .h.].h...Otherwi
-000020a0: 7365 203a 9485 9481 947d 9428 681b 6ac7  se :.....}.(h.j.
-000020b0: 0200 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-000020c0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-000020d0: 9468 275d 9468 295d 9475 682b 683e 681e  .h'].h)].uh+h>h.
-000020e0: 4b36 681d 682c 681b 6ac4 0200 0068 1c68  K6h.h,h.j....h.h
-000020f0: 0375 626a 2e02 0000 2981 947d 9428 6805  .ubj....)..}.(h.
-00002100: 6806 6807 5d94 286a 3302 0000 2981 947d  h.h.].(j3...)..}
-00002110: 9428 6805 6806 6807 5d94 683f 2981 947d  .(h.h.h.].h?)..}
-00002120: 9428 6805 8c37 6066 696c 654e 616d 6560  .(h..7`fileName`
-00002130: 203a 2046 756c 6c20 7061 7468 2074 6f20   : Full path to 
-00002140: 7468 6520 606d 7a44 6174 612e 786d 6c60  the `mzData.xml`
-00002150: 2066 696c 6520 746f 2072 6561 6494 6807   file to read.h.
-00002160: 5d94 286a 4701 0000 2981 947d 9428 6805  ].(jG...)..}.(h.
-00002170: 8c08 6669 6c65 4e61 6d65 9468 075d 9468  ..fileName.h.].h
-00002180: 168c 0866 696c 654e 616d 6594 8594 8194  ...fileName.....
-00002190: 7d94 2868 1b6a df02 0000 681c 6803 681d  }.(h.j....h.h.h.
-000021a0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-000021b0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000021c0: 7568 2b6a 4601 0000 681e 4b37 681d 682c  uh+jF...h.K7h.h,
-000021d0: 681b 6adb 0200 0068 1c68 0375 6268 168c  h.j....h.h.ubh..
-000021e0: 1420 3a20 4675 6c6c 2070 6174 6820 746f  . : Full path to
-000021f0: 2074 6865 2094 8594 8194 7d94 2868 1b6a   the .....}.(h.j
-00002200: db02 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00002210: 6a47 0100 0029 8194 7d94 2868 058c 0a6d  jG...)..}.(h...m
-00002220: 7a44 6174 612e 786d 6c94 6807 5d94 6816  zData.xml.h.].h.
-00002230: 8c0a 6d7a 4461 7461 2e78 6d6c 9485 9481  ..mzData.xml....
-00002240: 947d 9428 681b 6af1 0200 0068 1c68 0368  .}.(h.j....h.h.h
-00002250: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00002260: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00002270: 9475 682b 6a46 0100 0068 1e4b 3768 1d68  .uh+jF...h.K7h.h
-00002280: 2c68 1b6a db02 0000 681c 6803 7562 6816  ,h.j....h.h.ubh.
-00002290: 8c0d 2066 696c 6520 746f 2072 6561 6494  .. file to read.
-000022a0: 8594 8194 7d94 2868 1b6a db02 0000 681c  ....}.(h.j....h.
-000022b0: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
-000022c0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000022d0: 6829 5d94 7568 2b68 3e68 1e4b 3768 1d68  h)].uh+h>h.K7h.h
-000022e0: 2c68 1b6a d802 0000 681c 6803 7562 6168  ,h.j....h.h.ubah
-000022f0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00002300: 6827 5d94 6829 5d94 7568 2b6a 3202 0000  h'].h)].uh+j2...
-00002310: 681e 4b37 681d 682c 681b 6ad5 0200 0068  h.K7h.h,h.j....h
-00002320: 1c68 0375 626a 3302 0000 2981 947d 9428  .h.ubj3...)..}.(
-00002330: 6805 6806 6807 5d94 683f 2981 947d 9428  h.h.h.].h?)..}.(
-00002340: 6805 8c20 6063 7573 746f 6d44 6972 6563  h.. `customDirec
-00002350: 746f 7279 6020 3a20 446f 6573 206e 6f74  tory` : Does not
-00002360: 6869 6e67 9468 075d 9428 6a47 0100 0029  hing.h.].(jG...)
-00002370: 8194 7d94 2868 058c 0f63 7573 746f 6d44  ..}.(h...customD
-00002380: 6972 6563 746f 7279 9468 075d 9468 168c  irectory.h.].h..
-00002390: 0f63 7573 746f 6d44 6972 6563 746f 7279  .customDirectory
-000023a0: 9485 9481 947d 9428 681b 6a16 0300 0068  .....}.(h.j....h
-000023b0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-000023c0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-000023d0: 9468 295d 9475 682b 6a46 0100 0068 1e4b  .h)].uh+jF...h.K
-000023e0: 3868 1d68 2c68 1b6a 1203 0000 681c 6803  8h.h,h.j....h.h.
-000023f0: 7562 6816 8c0f 203a 2044 6f65 7320 6e6f  ubh... : Does no
-00002400: 7468 696e 6794 8594 8194 7d94 2868 1b6a  thing.....}.(h.j
-00002410: 1203 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00002420: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00002430: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
-00002440: 1e4b 3868 1d68 2c68 1b6a 0f03 0000 681c  .K8h.h,h.j....h.
-00002450: 6803 7562 6168 1f7d 9428 6821 5d94 6823  h.ubah.}.(h!].h#
-00002460: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00002470: 2b6a 3202 0000 681e 4b38 681d 682c 681b  +j2...h.K8h.h,h.
-00002480: 6ad5 0200 0068 1c68 0375 6265 681f 7d94  j....h.h.ubeh.}.
-00002490: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-000024a0: 9468 295d 946a bc02 0000 6abd 0200 0075  .h)].j....j....u
-000024b0: 682b 6a2d 0200 0068 1e4b 3768 1d68 2c68  h+j-...h.K7h.h,h
-000024c0: 1b6a c402 0000 681c 6803 7562 6568 1f7d  .j....h.h.ubeh.}
-000024d0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000024e0: 5d94 6829 5d94 7568 2b6a 3202 0000 681e  ].h)].uh+j2...h.
-000024f0: 4b36 681d 682c 681b 6a2f 0200 0068 1c68  K6h.h,h.j/...h.h
-00002500: 0375 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
-00002510: 9468 255d 9468 275d 9468 295d 946a bc02  .h%].h'].h)].j..
-00002520: 0000 6abd 0200 0075 682b 6a2d 0200 0068  ..j....uh+j-...h
-00002530: 1e4b 3368 1d68 2c68 1b6a dd01 0000 681c  .K3h.h,h.j....h.
-00002540: 6803 7562 683f 2981 947d 9428 6805 8c0e  h.ubh?)..}.(h...
-00002550: 3c75 3e4f 7574 7075 7473 3c2f 753e 9468  <u>Outputs</u>.h
-00002560: 075d 9428 6a03 0200 0029 8194 7d94 2868  .].(j....)..}.(h
-00002570: 058c 033c 753e 9468 075d 9468 168c 033c  ...<u>.h.].h...<
-00002580: 753e 9485 9481 947d 9428 681b 6a4a 0300  u>.....}.(h.jJ..
-00002590: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-000025a0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000025b0: 275d 9468 295d 948c 0666 6f72 6d61 7494  '].h)]...format.
-000025c0: 6a13 0200 0068 7a68 7b75 682b 6a02 0200  j....hzh{uh+j...
-000025d0: 0068 1d68 2c68 1e4b 3a68 1b6a 4603 0000  .h.h,h.K:h.jF...
-000025e0: 681c 6803 7562 6816 8c07 4f75 7470 7574  h.h.ubh...Output
-000025f0: 7394 8594 8194 7d94 2868 1b6a 4603 0000  s.....}.(h.jF...
-00002600: 681c 6803 681d 4e68 1e4e 7562 6a03 0200  h.h.h.Nh.Nubj...
-00002610: 0029 8194 7d94 2868 058c 043c 2f75 3e94  .)..}.(h...</u>.
-00002620: 6807 5d94 6816 8c04 3c2f 753e 9485 9481  h.].h...</u>....
-00002630: 947d 9428 681b 6a5d 0300 0068 1c68 0368  .}.(h.j]...h.h.h
-00002640: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00002650: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00002660: 948c 0666 6f72 6d61 7494 6a13 0200 0068  ...format.j....h
-00002670: 7a68 7b75 682b 6a02 0200 0068 1d68 2c68  zh{uh+j....h.h,h
-00002680: 1e4b 3a68 1b6a 4603 0000 681c 6803 7562  .K:h.jF...h.h.ub
-00002690: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-000026a0: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
-000026b0: 1e4b 3a68 1d68 2c68 1b6a dd01 0000 681c  .K:h.h,h.j....h.
-000026c0: 6803 7562 6a2e 0200 0029 8194 7d94 2868  h.ubj....)..}.(h
-000026d0: 0568 0668 075d 946a 3302 0000 2981 947d  .h.h.].j3...)..}
-000026e0: 9428 6805 6806 6807 5d94 683f 2981 947d  .(h.h.h.].h?)..}
-000026f0: 9428 6805 8c43 4f75 7470 7574 7320 6120  .(h..COutputs a 
-00002700: 606d 7a44 6174 6160 2063 6c61 7373 2063  `mzData` class c
-00002710: 6f6e 7461 696e 696e 6720 7468 6520 636f  ontaining the co
-00002720: 6e74 656e 7420 6f66 2074 6865 2066 696c  ntent of the fil
-00002730: 6520 7061 7273 6564 2e94 6807 5d94 2868  e parsed..h.].(h
-00002740: 168c 0a4f 7574 7075 7473 2061 2094 8594  ...Outputs a ...
-00002750: 8194 7d94 2868 1b6a 7803 0000 681c 6803  ..}.(h.jx...h.h.
-00002760: 681d 4e68 1e4e 7562 6a47 0100 0029 8194  h.Nh.NubjG...)..
-00002770: 7d94 2868 058c 066d 7a44 6174 6194 6807  }.(h...mzData.h.
-00002780: 5d94 6816 8c06 6d7a 4461 7461 9485 9481  ].h...mzData....
-00002790: 947d 9428 681b 6a80 0300 0068 1c68 0368  .}.(h.j....h.h.h
-000027a0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000027b0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-000027c0: 9475 682b 6a46 0100 0068 1e4b 3b68 1d68  .uh+jF...h.K;h.h
-000027d0: 2c68 1b6a 7803 0000 681c 6803 7562 6816  ,h.jx...h.h.ubh.
-000027e0: 8c31 2063 6c61 7373 2063 6f6e 7461 696e  .1 class contain
-000027f0: 696e 6720 7468 6520 636f 6e74 656e 7420  ing the content 
-00002800: 6f66 2074 6865 2066 696c 6520 7061 7273  of the file pars
-00002810: 6564 2e94 8594 8194 7d94 2868 1b6a 7803  ed......}.(h.jx.
-00002820: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
-00002830: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00002840: 6827 5d94 6829 5d94 7568 2b68 3e68 1e4b  h'].h)].uh+h>h.K
-00002850: 3b68 1d68 2c68 1b6a 7503 0000 681c 6803  ;h.h,h.ju...h.h.
-00002860: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00002870: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00002880: 3202 0000 681e 4b3b 681d 682c 681b 6a72  2...h.K;h.h,h.jr
-00002890: 0300 0068 1c68 0375 6261 681f 7d94 2868  ...h.h.ubah.}.(h
-000028a0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000028b0: 295d 946a bc02 0000 6abd 0200 0075 682b  )].j....j....uh+
-000028c0: 6a2d 0200 0068 1e4b 3b68 1d68 2c68 1b6a  j-...h.K;h.h,h.j
-000028d0: dd01 0000 681c 6803 7562 6568 1f7d 9428  ....h.h.ubeh.}.(
-000028e0: 6821 5d94 8c03 6964 3394 6168 235d 9468  h!]...id3.ah#].h
-000028f0: 255d 9468 275d 946a 0901 0000 6168 295d  %].h'].j....ah)]
-00002900: 9475 682b 680a 681e 4b2a 681d 682c 681b  .uh+h.h.K*h.h,h.
-00002910: 6a1c 0100 0068 1c68 0368 564b 0175 6265  j....h.h.hVK.ube
-00002920: 681f 7d94 2868 215d 948c 0d6d 7a64 6174  h.}.(h!]...mzdat
-00002930: 6178 6d6c 7265 6164 9461 6823 5d94 6825  axmlread.ah#].h%
-00002940: 5d94 8c0d 6d7a 6461 7461 786d 6c72 6561  ]...mzdataxmlrea
-00002950: 6494 6168 275d 9468 295d 9475 682b 680a  d.ah'].h)].uh+h.
-00002960: 681e 4b20 681d 682c 681b 6a0b 0100 0068  h.K h.h,h.j....h
-00002970: 1c68 0375 6268 0b29 8194 7d94 2868 0568  .h.ubh.)..}.(h.h
-00002980: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
-00002990: 8c0b 7361 7665 4d61 7466 696c 6594 6807  ..saveMatfile.h.
-000029a0: 5d94 6816 8c0b 7361 7665 4d61 7466 696c  ].h...saveMatfil
-000029b0: 6594 8594 8194 7d94 2868 1b6a b603 0000  e.....}.(h.j....
-000029c0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-000029d0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000029e0: 5d94 6829 5d94 7568 2b68 0f68 1e4b 3d68  ].h)].uh+h.h.K=h
-000029f0: 1d68 2c68 1b6a b303 0000 681c 6803 7562  .h,h.j....h.h.ub
-00002a00: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
-00002a10: 2868 1029 8194 7d94 2868 058c 0c50 7265  (h.)..}.(h...Pre
-00002a20: 7365 6e74 6174 696f 6e94 6807 5d94 6816  sentation.h.].h.
-00002a30: 8c0c 5072 6573 656e 7461 7469 6f6e 9485  ..Presentation..
-00002a40: 9481 947d 9428 681b 6ac7 0300 0068 1c68  ...}.(h.j....h.h
-00002a50: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00002a60: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00002a70: 295d 9475 682b 680f 681e 4b3e 681d 682c  )].uh+h.h.K>h.h,
-00002a80: 681b 6ac4 0300 0068 1c68 0375 6268 3f29  h.j....h.h.ubh?)
-00002a90: 8194 7d94 2868 058c 4553 6176 6573 2061  ..}.(h..ESaves a
-00002aa0: 2060 6d7a 4461 7461 6020 636c 6173 7320   `mzData` class 
-00002ab0: 696e 746f 2061 2060 2e6d 6174 6020 6669  into a `.mat` fi
-00002ac0: 6c65 2077 6974 6820 616c 6c20 6d65 7461  le with all meta
-00002ad0: 6461 7461 2069 6e63 6c75 6465 642e 9468  data included..h
-00002ae0: 075d 9428 6816 8c08 5361 7665 7320 6120  .].(h...Saves a 
-00002af0: 9485 9481 947d 9428 681b 6ad5 0300 0068  .....}.(h.j....h
-00002b00: 1c68 0368 1d4e 681e 4e75 626a 4701 0000  .h.h.Nh.NubjG...
-00002b10: 2981 947d 9428 6805 8c06 6d7a 4461 7461  )..}.(h...mzData
-00002b20: 9468 075d 9468 168c 066d 7a44 6174 6194  .h.].h...mzData.
-00002b30: 8594 8194 7d94 2868 1b6a dd03 0000 681c  ....}.(h.j....h.
-00002b40: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00002b50: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00002b60: 6829 5d94 7568 2b6a 4601 0000 681e 4b3f  h)].uh+jF...h.K?
-00002b70: 681d 682c 681b 6ad5 0300 0068 1c68 0375  h.h,h.j....h.h.u
-00002b80: 6268 168c 0e20 636c 6173 7320 696e 746f  bh... class into
-00002b90: 2061 2094 8594 8194 7d94 2868 1b6a d503   a .....}.(h.j..
-00002ba0: 0000 681c 6803 681d 4e68 1e4e 7562 6a47  ..h.h.h.Nh.NubjG
-00002bb0: 0100 0029 8194 7d94 2868 058c 042e 6d61  ...)..}.(h....ma
-00002bc0: 7494 6807 5d94 6816 8c04 2e6d 6174 9485  t.h.].h....mat..
-00002bd0: 9481 947d 9428 681b 6aef 0300 0068 1c68  ...}.(h.j....h.h
-00002be0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00002bf0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00002c00: 295d 9475 682b 6a46 0100 0068 1e4b 3f68  )].uh+jF...h.K?h
-00002c10: 1d68 2c68 1b6a d503 0000 681c 6803 7562  .h,h.j....h.h.ub
-00002c20: 6816 8c21 2066 696c 6520 7769 7468 2061  h..! file with a
-00002c30: 6c6c 206d 6574 6164 6174 6120 696e 636c  ll metadata incl
-00002c40: 7564 6564 2e94 8594 8194 7d94 2868 1b6a  uded......}.(h.j
-00002c50: d503 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00002c60: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00002c70: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
-00002c80: 1e4b 3f68 1d68 2c68 1b6a c403 0000 681c  .K?h.h,h.j....h.
-00002c90: 6803 7562 6568 1f7d 9428 6821 5d94 8c03  h.ubeh.}.(h!]...
-00002ca0: 6964 3494 6168 235d 9468 255d 9468 275d  id4.ah#].h%].h']
-00002cb0: 948c 0c70 7265 7365 6e74 6174 696f 6e94  ...presentation.
-00002cc0: 6168 295d 9475 682b 680a 681e 4b3e 681d  ah)].uh+h.h.K>h.
-00002cd0: 682c 681b 6ab3 0300 0068 1c68 0368 564b  h,h.j....h.h.hVK
-00002ce0: 0175 6268 0b29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
-00002cf0: 075d 9428 6810 2981 947d 9428 6805 8c0a  .].(h.)..}.(h...
-00002d00: 4465 6669 6e69 7469 6f6e 9468 075d 9468  Definition.h.].h
-00002d10: 168c 0a44 6566 696e 6974 696f 6e94 8594  ...Definition...
-00002d20: 8194 7d94 2868 1b6a 1204 0000 681c 6803  ..}.(h.j....h.h.
-00002d30: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00002d40: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00002d50: 5d94 7568 2b68 0f68 1e4b 4168 1d68 2c68  ].uh+h.h.KAh.h,h
-00002d60: 1b6a 0f04 0000 681c 6803 7562 6869 2981  .j....h.h.ubhi).
-00002d70: 947d 9428 6805 8c79 6465 6620 7361 7665  .}.(h..ydef save
-00002d80: 4d61 7466 696c 6528 7365 6c66 406d 7a44  Matfile(self@mzD
-00002d90: 6174 614d 616e 6167 6572 2c20 6d7a 4461  ataManager, mzDa
-00002da0: 7461 203a 206d 7a44 6174 612c 2072 656d  ta : mzData, rem
-00002db0: 6f76 6520 3a20 626f 6f6c 203d 2046 616c  ove : bool = Fal
-00002dc0: 7365 2c20 6469 7232 5361 7665 203a 2073  se, dir2Save : s
-00002dd0: 7472 203d 204e 6f6e 652c 2066 6f72 6365  tr = None, force
-00002de0: 203a 2062 6f6f 6c20 3d20 4661 6c73 6529   : bool = False)
-00002df0: 0a94 6807 5d94 6816 8c79 6465 6620 7361  ..h.].h..ydef sa
-00002e00: 7665 4d61 7466 696c 6528 7365 6c66 406d  veMatfile(self@m
-00002e10: 7a44 6174 614d 616e 6167 6572 2c20 6d7a  zDataManager, mz
-00002e20: 4461 7461 203a 206d 7a44 6174 612c 2072  Data : mzData, r
-00002e30: 656d 6f76 6520 3a20 626f 6f6c 203d 2046  emove : bool = F
-00002e40: 616c 7365 2c20 6469 7232 5361 7665 203a  alse, dir2Save :
-00002e50: 2073 7472 203d 204e 6f6e 652c 2066 6f72   str = None, for
-00002e60: 6365 203a 2062 6f6f 6c20 3d20 4661 6c73  ce : bool = Fals
-00002e70: 6529 0a94 8594 8194 7d94 681b 6a20 0400  e)......}.h.j ..
-00002e80: 0073 6261 681f 7d94 2868 215d 9468 235d  .sbah.}.(h!].h#]
-00002e90: 9468 255d 9468 275d 9468 295d 948c 086c  .h%].h'].h)]...l
-00002ea0: 616e 6775 6167 6594 8c06 7079 7468 6f6e  anguage...python
-00002eb0: 9468 7a68 7b75 682b 6868 681d 682c 681e  .hzh{uh+hhh.h,h.
-00002ec0: 4b42 681b 6a0f 0400 0068 1c68 0375 6265  KBh.j....h.h.ube
-00002ed0: 681f 7d94 2868 215d 948c 0369 6435 9461  h.}.(h!]...id5.a
-00002ee0: 6823 5d94 6825 5d94 6827 5d94 8c0a 6465  h#].h%].h']...de
-00002ef0: 6669 6e69 7469 6f6e 9461 6829 5d94 7568  finition.ah)].uh
-00002f00: 2b68 0a68 1e4b 4168 1d68 2c68 1b6a b303  +h.h.KAh.h,h.j..
-00002f10: 0000 681c 6803 6856 4b01 7562 680b 2981  ..h.h.hVK.ubh.).
-00002f20: 947d 9428 6805 6806 6807 5d94 2868 1029  .}.(h.h.h.].(h.)
-00002f30: 8194 7d94 2868 058c 0a48 6f77 2074 6f20  ..}.(h...How to 
-00002f40: 7573 6594 6807 5d94 6816 8c0a 486f 7720  use.h.].h...How 
-00002f50: 746f 2075 7365 9485 9481 947d 9428 681b  to use.....}.(h.
-00002f60: 6a3b 0400 0068 1c68 0368 1d4e 681e 4e75  j;...h.h.h.Nh.Nu
-00002f70: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00002f80: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
-00002f90: 681e 4b46 681d 682c 681b 6a38 0400 0068  h.KFh.h,h.j8...h
-00002fa0: 1c68 0375 6268 6929 8194 7d94 2868 058c  .h.ubhi)..}.(h..
-00002fb0: f723 2043 6f6e 7369 6465 7269 6e67 2074  .# Considering t
-00002fc0: 6861 7420 6d7a 4461 7461 4d61 6e61 6765  hat mzDataManage
-00002fd0: 7220 636c 6173 7320 6861 7320 6265 656e  r class has been
-00002fe0: 2069 6e74 6961 6c69 7a65 6420 6265 666f   intialized befo
-00002ff0: 7265 2061 6e64 2073 746f 7265 6420 6173  re and stored as
-00003000: 206d 616e 6167 6572 2076 6172 6961 626c   manager variabl
-00003010: 650a 0a23 2043 6f6e 7369 6465 7269 6e67  e..# Considering
-00003020: 2061 6c73 6f20 7468 6520 7661 7269 6162   also the variab
-00003030: 6c65 2063 6f6e 7465 6e74 2077 6869 6368  le content which
-00003040: 2069 7320 7468 6520 7265 7375 6c74 206f   is the result o
-00003050: 6620 7468 6520 6675 6e63 7469 6f6e 206d  f the function m
-00003060: 7a44 6174 6158 4d4c 7265 6164 2070 7265  zDataXMLread pre
-00003070: 7365 6e74 6564 2061 626f 7665 0a0a 6d61  sented above..ma
-00003080: 6e61 6765 722e 7361 7665 4d61 7446 696c  nager.saveMatFil
-00003090: 6528 0a20 2020 206d 7a44 6174 613d 636f  e(.    mzData=co
-000030a0: 6e74 656e 740a 290a 9468 075d 9468 168c  ntent.)..h.].h..
-000030b0: f723 2043 6f6e 7369 6465 7269 6e67 2074  .# Considering t
-000030c0: 6861 7420 6d7a 4461 7461 4d61 6e61 6765  hat mzDataManage
-000030d0: 7220 636c 6173 7320 6861 7320 6265 656e  r class has been
-000030e0: 2069 6e74 6961 6c69 7a65 6420 6265 666f   intialized befo
-000030f0: 7265 2061 6e64 2073 746f 7265 6420 6173  re and stored as
-00003100: 206d 616e 6167 6572 2076 6172 6961 626c   manager variabl
-00003110: 650a 0a23 2043 6f6e 7369 6465 7269 6e67  e..# Considering
-00003120: 2061 6c73 6f20 7468 6520 7661 7269 6162   also the variab
-00003130: 6c65 2063 6f6e 7465 6e74 2077 6869 6368  le content which
-00003140: 2069 7320 7468 6520 7265 7375 6c74 206f   is the result o
-00003150: 6620 7468 6520 6675 6e63 7469 6f6e 206d  f the function m
-00003160: 7a44 6174 6158 4d4c 7265 6164 2070 7265  zDataXMLread pre
-00003170: 7365 6e74 6564 2061 626f 7665 0a0a 6d61  sented above..ma
-00003180: 6e61 6765 722e 7361 7665 4d61 7446 696c  nager.saveMatFil
-00003190: 6528 0a20 2020 206d 7a44 6174 613d 636f  e(.    mzData=co
-000031a0: 6e74 656e 740a 290a 9485 9481 947d 9468  ntent.)......}.h
-000031b0: 1b6a 4904 0000 7362 6168 1f7d 9428 6821  .jI...sbah.}.(h!
-000031c0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-000031d0: 5d94 8c08 6c61 6e67 7561 6765 948c 0670  ]...language...p
-000031e0: 7974 686f 6e94 687a 687b 7568 2b68 6868  ython.hzh{uh+hhh
-000031f0: 1d68 2c68 1e4b 4768 1b6a 3804 0000 681c  .h,h.KGh.j8...h.
-00003200: 6803 7562 683f 2981 947d 9428 6805 8c11  h.ubh?)..}.(h...
-00003210: 3c75 3e50 6172 616d 6574 6572 733c 2f75  <u>Parameters</u
-00003220: 3e94 6807 5d94 286a 0302 0000 2981 947d  >.h.].(j....)..}
-00003230: 9428 6805 8c03 3c75 3e94 6807 5d94 6816  .(h...<u>.h.].h.
-00003240: 8c03 3c75 3e94 8594 8194 7d94 2868 1b6a  ..<u>.....}.(h.j
-00003250: 5d04 0000 681c 6803 681d 4e68 1e4e 7562  ]...h.h.h.Nh.Nub
-00003260: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00003270: 5d94 6827 5d94 6829 5d94 8c06 666f 726d  ].h'].h)]...form
-00003280: 6174 946a 1302 0000 687a 687b 7568 2b6a  at.j....hzh{uh+j
-00003290: 0202 0000 681d 682c 681e 4b50 681b 6a59  ....h.h,h.KPh.jY
-000032a0: 0400 0068 1c68 0375 6268 168c 0a50 6172  ...h.h.ubh...Par
-000032b0: 616d 6574 6572 7394 8594 8194 7d94 2868  ameters.....}.(h
-000032c0: 1b6a 5904 0000 681c 6803 681d 4e68 1e4e  .jY...h.h.h.Nh.N
-000032d0: 7562 6a03 0200 0029 8194 7d94 2868 058c  ubj....)..}.(h..
-000032e0: 043c 2f75 3e94 6807 5d94 6816 8c04 3c2f  .</u>.h.].h...</
-000032f0: 753e 9485 9481 947d 9428 681b 6a70 0400  u>.....}.(h.jp..
-00003300: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00003310: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00003320: 275d 9468 295d 948c 0666 6f72 6d61 7494  '].h)]...format.
-00003330: 6a13 0200 0068 7a68 7b75 682b 6a02 0200  j....hzh{uh+j...
-00003340: 0068 1d68 2c68 1e4b 5068 1b6a 5904 0000  .h.h,h.KPh.jY...
-00003350: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
-00003360: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00003370: 7568 2b68 3e68 1e4b 5068 1d68 2c68 1b6a  uh+h>h.KPh.h,h.j
-00003380: 3804 0000 681c 6803 7562 6a2e 0200 0029  8...h.h.ubj....)
-00003390: 8194 7d94 2868 0568 0668 075d 9428 6a33  ..}.(h.h.h.].(j3
-000033a0: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-000033b0: 9468 3f29 8194 7d94 2868 058c 7760 6d7a  .h?)..}.(h..w`mz
-000033c0: 4461 7461 6020 3a20 5468 6520 606d 7a44  Data` : The `mzD
-000033d0: 6174 6160 2073 7472 7563 7475 7265 2074  ata` structure t
-000033e0: 6f20 7361 7665 2061 7320 6120 602e 6d61  o save as a `.ma
-000033f0: 7460 2066 696c 652e 2028 5365 6520 5b68  t` file. (See [h
-00003400: 6572 655d 286d 6174 5374 7275 6374 7572  ere](matStructur
-00003410: 652e 6d64 2920 666f 7220 7468 6520 602e  e.md) for the `.
-00003420: 6d61 7460 2066 696c 6520 7374 7275 6374  mat` file struct
-00003430: 7572 6529 9468 075d 9428 6a47 0100 0029  ure).h.].(jG...)
-00003440: 8194 7d94 2868 058c 066d 7a44 6174 6194  ..}.(h...mzData.
-00003450: 6807 5d94 6816 8c06 6d7a 4461 7461 9485  h.].h...mzData..
-00003460: 9481 947d 9428 681b 6a8f 0400 0068 1c68  ...}.(h.j....h.h
-00003470: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00003480: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00003490: 295d 9475 682b 6a46 0100 0068 1e4b 5168  )].uh+jF...h.KQh
-000034a0: 1d68 2c68 1b6a 8b04 0000 681c 6803 7562  .h,h.j....h.h.ub
-000034b0: 6816 8c07 203a 2054 6865 2094 8594 8194  h... : The .....
-000034c0: 7d94 2868 1b6a 8b04 0000 681c 6803 681d  }.(h.j....h.h.h.
-000034d0: 4e68 1e4e 7562 6a47 0100 0029 8194 7d94  Nh.NubjG...)..}.
-000034e0: 2868 058c 066d 7a44 6174 6194 6807 5d94  (h...mzData.h.].
-000034f0: 6816 8c06 6d7a 4461 7461 9485 9481 947d  h...mzData.....}
-00003500: 9428 681b 6aa1 0400 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00003510: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00003520: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00003530: 682b 6a46 0100 0068 1e4b 5168 1d68 2c68  h+jF...h.KQh.h,h
-00003540: 1b6a 8b04 0000 681c 6803 7562 6816 8c18  .j....h.h.ubh...
-00003550: 2073 7472 7563 7475 7265 2074 6f20 7361   structure to sa
-00003560: 7665 2061 7320 6120 9485 9481 947d 9428  ve as a .....}.(
-00003570: 681b 6a8b 0400 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00003580: 4e75 626a 4701 0000 2981 947d 9428 6805  NubjG...)..}.(h.
-00003590: 8c04 2e6d 6174 9468 075d 9468 168c 042e  ...mat.h.].h....
-000035a0: 6d61 7494 8594 8194 7d94 2868 1b6a b304  mat.....}.(h.j..
-000035b0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-000035c0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-000035d0: 6827 5d94 6829 5d94 7568 2b6a 4601 0000  h'].h)].uh+jF...
-000035e0: 681e 4b51 681d 682c 681b 6a8b 0400 0068  h.KQh.h,h.j....h
-000035f0: 1c68 0375 6268 168c 0c20 6669 6c65 2e20  .h.ubh... file. 
-00003600: 2853 6565 2094 8594 8194 7d94 2868 1b6a  (See .....}.(h.j
-00003610: 8b04 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00003620: 6a7f 0100 0029 8194 7d94 2868 0568 0668  j....)..}.(h.h.h
-00003630: 075d 946a 8401 0000 2981 947d 9428 6805  .].j....)..}.(h.
-00003640: 8c04 6865 7265 9468 075d 9468 168c 0468  ..here.h.].h...h
-00003650: 6572 6594 8594 8194 7d94 2868 1b6a c804  ere.....}.(h.j..
-00003660: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00003670: 1f7d 9428 6821 5d94 6823 5d94 286a 9001  .}.(h!].h#].(j..
-00003680: 0000 6a91 0100 0065 6825 5d94 6827 5d94  ..j....eh%].h'].
-00003690: 6829 5d94 7568 2b6a 8301 0000 681b 6ac5  h)].uh+j....h.j.
-000036a0: 0400 0068 1c68 0368 1d68 2c68 1e4b 0075  ...h.h.h.h,h.K.u
-000036b0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-000036c0: 255d 9468 275d 9468 295d 948c 0972 6566  %].h'].h)]...ref
-000036d0: 646f 6d61 696e 946a 9c01 0000 8c09 7265  domain.j......re
-000036e0: 6674 6172 6765 7494 8c0c 6d61 7453 7472  ftarget...matStr
-000036f0: 7563 7475 7265 948c 0b72 6566 7461 7267  ucture...reftarg
-00003700: 6574 6964 944e 8c06 7265 6664 6f63 946a  etid.N..refdoc.j
-00003710: a101 0000 8c07 7265 6674 7970 6594 6a91  ......reftype.j.
-00003720: 0100 008c 0b72 6566 6578 706c 6963 6974  .....refexplicit
-00003730: 9488 7568 2b6a 7e01 0000 681e 4b51 681d  ..uh+j~...h.KQh.
-00003740: 682c 681b 6a8b 0400 0068 1c68 0375 6268  h,h.j....h.h.ubh
-00003750: 168c 0920 666f 7220 7468 6520 9485 9481  ... for the ....
-00003760: 947d 9428 681b 6a8b 0400 0068 1c68 0368  .}.(h.j....h.h.h
-00003770: 1d4e 681e 4e75 626a 4701 0000 2981 947d  .Nh.NubjG...)..}
-00003780: 9428 6805 8c04 2e6d 6174 9468 075d 9468  .(h....mat.h.].h
-00003790: 168c 042e 6d61 7494 8594 8194 7d94 2868  ....mat.....}.(h
-000037a0: 1b6a e704 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-000037b0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-000037c0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-000037d0: 4601 0000 681e 4b51 681d 682c 681b 6a8b  F...h.KQh.h,h.j.
-000037e0: 0400 0068 1c68 0375 6268 168c 1020 6669  ...h.h.ubh... fi
-000037f0: 6c65 2073 7472 7563 7475 7265 2994 8594  le structure)...
-00003800: 8194 7d94 2868 1b6a 8b04 0000 681c 6803  ..}.(h.j....h.h.
-00003810: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
-00003820: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00003830: 5d94 7568 2b68 3e68 1e4b 5168 1d68 2c68  ].uh+h>h.KQh.h,h
-00003840: 1b6a 8804 0000 681c 6803 7562 6168 1f7d  .j....h.h.ubah.}
-00003850: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00003860: 5d94 6829 5d94 7568 2b6a 3202 0000 681e  ].h)].uh+j2...h.
-00003870: 4b51 681d 682c 681b 6a85 0400 0068 1c68  KQh.h,h.j....h.h
-00003880: 0375 626a 3302 0000 2981 947d 9428 6805  .ubj3...)..}.(h.
-00003890: 6806 6807 5d94 683f 2981 947d 9428 6805  h.h.].h?)..}.(h.
-000038a0: 8c6b 6072 656d 6f76 6560 203a 2053 686f  .k`remove` : Sho
-000038b0: 756c 6420 7468 6520 6f72 6967 696e 616c  uld the original
-000038c0: 2066 696c 6520 2873 6f20 7468 6520 6f72   file (so the or
-000038d0: 6967 696e 616c 2060 2e6d 7a44 6174 612e  iginal `.mzData.
-000038e0: 786d 6c60 2066 696c 6529 2062 6520 7265  xml` file) be re
-000038f0: 6d6f 7665 6420 7768 656e 2073 6176 6520  moved when save 
-00003900: 6973 2063 6f6d 706c 6574 6520 3f94 6807  is complete ?.h.
-00003910: 5d94 286a 4701 0000 2981 947d 9428 6805  ].(jG...)..}.(h.
-00003920: 8c06 7265 6d6f 7665 9468 075d 9468 168c  ..remove.h.].h..
-00003930: 0672 656d 6f76 6594 8594 8194 7d94 2868  .remove.....}.(h
-00003940: 1b6a 0c05 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00003950: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00003960: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00003970: 4601 0000 681e 4b52 681d 682c 681b 6a08  F...h.KRh.h,h.j.
-00003980: 0500 0068 1c68 0375 6268 168c 2d20 3a20  ...h.h.ubh..- : 
-00003990: 5368 6f75 6c64 2074 6865 206f 7269 6769  Should the origi
-000039a0: 6e61 6c20 6669 6c65 2028 736f 2074 6865  nal file (so the
-000039b0: 206f 7269 6769 6e61 6c20 9485 9481 947d   original .....}
-000039c0: 9428 681b 6a08 0500 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-000039d0: 681e 4e75 626a 4701 0000 2981 947d 9428  h.NubjG...)..}.(
-000039e0: 6805 8c0b 2e6d 7a44 6174 612e 786d 6c94  h....mzData.xml.
-000039f0: 6807 5d94 6816 8c0b 2e6d 7a44 6174 612e  h.].h....mzData.
-00003a00: 786d 6c94 8594 8194 7d94 2868 1b6a 1e05  xml.....}.(h.j..
-00003a10: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00003a20: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00003a30: 6827 5d94 6829 5d94 7568 2b6a 4601 0000  h'].h)].uh+jF...
-00003a40: 681e 4b52 681d 682c 681b 6a08 0500 0068  h.KRh.h,h.j....h
-00003a50: 1c68 0375 6268 168c 2920 6669 6c65 2920  .h.ubh..) file) 
-00003a60: 6265 2072 656d 6f76 6564 2077 6865 6e20  be removed when 
-00003a70: 7361 7665 2069 7320 636f 6d70 6c65 7465  save is complete
-00003a80: 203f 9485 9481 947d 9428 681b 6a08 0500   ?.....}.(h.j...
-00003a90: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
-00003aa0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00003ab0: 275d 9468 295d 9475 682b 683e 681e 4b52  '].h)].uh+h>h.KR
-00003ac0: 681d 682c 681b 6a05 0500 0068 1c68 0375  h.h,h.j....h.h.u
-00003ad0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00003ae0: 255d 9468 275d 9468 295d 9475 682b 6a32  %].h'].h)].uh+j2
-00003af0: 0200 0068 1e4b 5268 1d68 2c68 1b6a 8504  ...h.KRh.h,h.j..
-00003b00: 0000 681c 6803 7562 6a33 0200 0029 8194  ..h.h.ubj3...)..
-00003b10: 7d94 2868 0568 0668 075d 9468 3f29 8194  }.(h.h.h.].h?)..
-00003b20: 7d94 2868 058c b860 666f 7263 6560 203a  }.(h...`force` :
-00003b30: 2049 6620 6120 602e 6d61 7460 2066 696c   If a `.mat` fil
-00003b40: 6520 616c 7265 6164 7920 6578 6973 7473  e already exists
-00003b50: 2077 6974 6820 7468 6520 7361 6d65 206e   with the same n
-00003b60: 616d 6520 696e 2074 6865 2065 7870 6f72  ame in the expor
-00003b70: 7420 666f 6c64 6572 2c20 7368 6f75 6c64  t folder, should
-00003b80: 2069 7420 6265 2072 6570 6c61 6365 6420   it be replaced 
-00003b90: 3f20 4966 2074 6869 7320 7061 7261 6d65  ? If this parame
-00003ba0: 7465 7220 6973 2073 6574 2074 6f20 6046  ter is set to `F
-00003bb0: 616c 7365 602c 2073 6176 6520 7769 6c6c  alse`, save will
-00003bc0: 2062 6520 6162 6f72 7465 6420 6966 2061   be aborted if a
-00003bd0: 2066 696c 6520 6973 2066 6f75 6e64 2e94   file is found..
-00003be0: 6807 5d94 286a 4701 0000 2981 947d 9428  h.].(jG...)..}.(
-00003bf0: 6805 8c05 666f 7263 6594 6807 5d94 6816  h...force.h.].h.
-00003c00: 8c05 666f 7263 6594 8594 8194 7d94 2868  ..force.....}.(h
-00003c10: 1b6a 4305 0000 681c 6803 681d 4e68 1e4e  .jC...h.h.h.Nh.N
-00003c20: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00003c30: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00003c40: 4601 0000 681e 4b53 681d 682c 681b 6a3f  F...h.KSh.h,h.j?
-00003c50: 0500 0068 1c68 0375 6268 168c 0820 3a20  ...h.h.ubh... : 
-00003c60: 4966 2061 2094 8594 8194 7d94 2868 1b6a  If a .....}.(h.j
-00003c70: 3f05 0000 681c 6803 681d 4e68 1e4e 7562  ?...h.h.h.Nh.Nub
-00003c80: 6a47 0100 0029 8194 7d94 2868 058c 042e  jG...)..}.(h....
-00003c90: 6d61 7494 6807 5d94 6816 8c04 2e6d 6174  mat.h.].h....mat
-00003ca0: 9485 9481 947d 9428 681b 6a55 0500 0068  .....}.(h.jU...h
-00003cb0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-00003cc0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00003cd0: 9468 295d 9475 682b 6a46 0100 0068 1e4b  .h)].uh+jF...h.K
-00003ce0: 5368 1d68 2c68 1b6a 3f05 0000 681c 6803  Sh.h,h.j?...h.h.
-00003cf0: 7562 6816 8c72 2066 696c 6520 616c 7265  ubh..r file alre
-00003d00: 6164 7920 6578 6973 7473 2077 6974 6820  ady exists with 
-00003d10: 7468 6520 7361 6d65 206e 616d 6520 696e  the same name in
-00003d20: 2074 6865 2065 7870 6f72 7420 666f 6c64   the export fold
-00003d30: 6572 2c20 7368 6f75 6c64 2069 7420 6265  er, should it be
-00003d40: 2072 6570 6c61 6365 6420 3f20 4966 2074   replaced ? If t
-00003d50: 6869 7320 7061 7261 6d65 7465 7220 6973  his parameter is
-00003d60: 2073 6574 2074 6f20 9485 9481 947d 9428   set to .....}.(
-00003d70: 681b 6a3f 0500 0068 1c68 0368 1d4e 681e  h.j?...h.h.h.Nh.
-00003d80: 4e75 626a 4701 0000 2981 947d 9428 6805  NubjG...)..}.(h.
-00003d90: 8c05 4661 6c73 6594 6807 5d94 6816 8c05  ..False.h.].h...
-00003da0: 4661 6c73 6594 8594 8194 7d94 2868 1b6a  False.....}.(h.j
-00003db0: 6705 0000 681c 6803 681d 4e68 1e4e 7562  g...h.h.h.Nh.Nub
-00003dc0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00003dd0: 5d94 6827 5d94 6829 5d94 7568 2b6a 4601  ].h'].h)].uh+jF.
-00003de0: 0000 681e 4b53 681d 682c 681b 6a3f 0500  ..h.KSh.h,h.j?..
-00003df0: 0068 1c68 0375 6268 168c 2a2c 2073 6176  .h.h.ubh..*, sav
-00003e00: 6520 7769 6c6c 2062 6520 6162 6f72 7465  e will be aborte
-00003e10: 6420 6966 2061 2066 696c 6520 6973 2066  d if a file is f
-00003e20: 6f75 6e64 2e94 8594 8194 7d94 2868 1b6a  ound......}.(h.j
-00003e30: 3f05 0000 681c 6803 681d 4e68 1e4e 7562  ?...h.h.h.Nh.Nub
-00003e40: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00003e50: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
-00003e60: 1e4b 5368 1d68 2c68 1b6a 3c05 0000 681c  .KSh.h,h.j<...h.
-00003e70: 6803 7562 6168 1f7d 9428 6821 5d94 6823  h.ubah.}.(h!].h#
-00003e80: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00003e90: 2b6a 3202 0000 681e 4b53 681d 682c 681b  +j2...h.KSh.h,h.
-00003ea0: 6a85 0400 0068 1c68 0375 626a 3302 0000  j....h.h.ubj3...
-00003eb0: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
-00003ec0: 3f29 8194 7d94 2868 058c 3549 6620 6469  ?)..}.(h..5If di
-00003ed0: 7265 6374 6f72 6965 7320 7765 7265 206e  rectories were n
-00003ee0: 6f74 2070 726f 7669 6465 6420 6475 7269  ot provided duri
-00003ef0: 6e67 2069 6e69 7420 7072 6f63 6573 733a  ng init process:
-00003f00: 9468 075d 9468 168c 3549 6620 6469 7265  .h.].h..5If dire
-00003f10: 6374 6f72 6965 7320 7765 7265 206e 6f74  ctories were not
-00003f20: 2070 726f 7669 6465 6420 6475 7269 6e67   provided during
-00003f30: 2069 6e69 7420 7072 6f63 6573 733a 9485   init process:..
-00003f40: 9481 947d 9428 681b 6a88 0500 0068 1c68  ...}.(h.j....h.h
-00003f50: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00003f60: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00003f70: 295d 9475 682b 683e 681e 4b54 681d 682c  )].uh+h>h.KTh.h,
-00003f80: 681b 6a85 0500 0068 1c68 0375 626a 2e02  h.j....h.h.ubj..
-00003f90: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
-00003fa0: 6a33 0200 0029 8194 7d94 2868 0568 0668  j3...)..}.(h.h.h
-00003fb0: 075d 9468 3f29 8194 7d94 2868 058c b160  .].h?)..}.(h...`
-00003fc0: 6469 7232 7361 7665 6020 3a20 4675 6c6c  dir2save` : Full
-00003fd0: 2064 6972 6563 746f 7279 2073 7065 6369   directory speci
-00003fe0: 6679 696e 6720 7768 6572 6520 746f 2073  fying where to s
-00003ff0: 6176 6520 7468 6520 636f 6e76 6572 7465  ave the converte
-00004000: 6420 6669 6c65 2e20 4966 2074 6869 7320  d file. If this 
-00004010: 7061 7261 6d65 7465 7220 6973 2073 6574  parameter is set
-00004020: 2077 6869 6c65 2061 2064 6972 6563 746f   while a directo
-00004030: 7279 2077 6173 2073 7065 6369 6669 6564  ry was specified
-00004040: 2069 6e20 7468 6520 696e 6974 2070 726f   in the init pro
-00004050: 6365 7373 2c20 7468 6973 2076 616c 7565  cess, this value
-00004060: 2069 7320 7072 696f 7269 7469 7a65 642e   is prioritized.
-00004070: 9468 075d 9428 6a47 0100 0029 8194 7d94  .h.].(jG...)..}.
-00004080: 2868 058c 0864 6972 3273 6176 6594 6807  (h...dir2save.h.
-00004090: 5d94 6816 8c08 6469 7232 7361 7665 9485  ].h...dir2save..
-000040a0: 9481 947d 9428 681b 6aa0 0500 0068 1c68  ...}.(h.j....h.h
-000040b0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-000040c0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000040d0: 295d 9475 682b 6a46 0100 0068 1e4b 5568  )].uh+jF...h.KUh
-000040e0: 1d68 2c68 1b6a 9c05 0000 681c 6803 7562  .h,h.j....h.h.ub
-000040f0: 6816 8ca7 203a 2046 756c 6c20 6469 7265  h... : Full dire
-00004100: 6374 6f72 7920 7370 6563 6966 7969 6e67  ctory specifying
-00004110: 2077 6865 7265 2074 6f20 7361 7665 2074   where to save t
-00004120: 6865 2063 6f6e 7665 7274 6564 2066 696c  he converted fil
-00004130: 652e 2049 6620 7468 6973 2070 6172 616d  e. If this param
-00004140: 6574 6572 2069 7320 7365 7420 7768 696c  eter is set whil
-00004150: 6520 6120 6469 7265 6374 6f72 7920 7761  e a directory wa
-00004160: 7320 7370 6563 6966 6965 6420 696e 2074  s specified in t
-00004170: 6865 2069 6e69 7420 7072 6f63 6573 732c  he init process,
-00004180: 2074 6869 7320 7661 6c75 6520 6973 2070   this value is p
-00004190: 7269 6f72 6974 697a 6564 2e94 8594 8194  rioritized......
-000041a0: 7d94 2868 1b6a 9c05 0000 681c 6803 681d  }.(h.j....h.h.h.
-000041b0: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
-000041c0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000041d0: 7568 2b68 3e68 1e4b 5568 1d68 2c68 1b6a  uh+h>h.KUh.h,h.j
-000041e0: 9905 0000 681c 6803 7562 6168 1f7d 9428  ....h.h.ubah.}.(
-000041f0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00004200: 6829 5d94 7568 2b6a 3202 0000 681e 4b55  h)].uh+j2...h.KU
-00004210: 681d 682c 681b 6a96 0500 0068 1c68 0375  h.h,h.j....h.h.u
-00004220: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00004230: 255d 9468 275d 9468 295d 946a bc02 0000  %].h'].h)].j....
-00004240: 6abd 0200 0075 682b 6a2d 0200 0068 1e4b  j....uh+j-...h.K
-00004250: 5568 1d68 2c68 1b6a 8505 0000 681c 6803  Uh.h,h.j....h.h.
-00004260: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-00004270: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00004280: 3202 0000 681e 4b54 681d 682c 681b 6a85  2...h.KTh.h,h.j.
-00004290: 0400 0068 1c68 0375 6265 681f 7d94 2868  ...h.h.ubeh.}.(h
-000042a0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000042b0: 295d 946a bc02 0000 6abd 0200 0075 682b  )].j....j....uh+
-000042c0: 6a2d 0200 0068 1e4b 5168 1d68 2c68 1b6a  j-...h.KQh.h,h.j
-000042d0: 3804 0000 681c 6803 7562 683f 2981 947d  8...h.h.ubh?)..}
-000042e0: 9428 6805 8c54 3c75 3e4f 7574 7075 7473  .(h..T<u>Outputs
-000042f0: 3c2f 753e 3c62 723e 0a49 6620 6675 6e63  </u><br>.If func
-00004300: 7469 6f6e 2072 616e 2063 6f72 7265 6374  tion ran correct
-00004310: 6c79 2c20 6e6f 206f 7574 7075 742c 206f  ly, no output, o
-00004320: 7468 6572 7769 7365 2072 6169 7365 7320  therwise raises 
-00004330: 7468 6520 6572 726f 722e 9468 075d 9428  the error..h.].(
-00004340: 6a03 0200 0029 8194 7d94 2868 058c 033c  j....)..}.(h...<
-00004350: 753e 9468 075d 9468 168c 033c 753e 9485  u>.h.].h...<u>..
-00004360: 9481 947d 9428 681b 6ad4 0500 0068 1c68  ...}.(h.j....h.h
-00004370: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00004380: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00004390: 295d 948c 0666 6f72 6d61 7494 6a13 0200  )]...format.j...
-000043a0: 0068 7a68 7b75 682b 6a02 0200 0068 1d68  .hzh{uh+j....h.h
-000043b0: 2c68 1e4b 5768 1b6a d005 0000 681c 6803  ,h.KWh.j....h.h.
-000043c0: 7562 6816 8c07 4f75 7470 7574 7394 8594  ubh...Outputs...
-000043d0: 8194 7d94 2868 1b6a d005 0000 681c 6803  ..}.(h.j....h.h.
-000043e0: 681d 4e68 1e4e 7562 6a03 0200 0029 8194  h.Nh.Nubj....)..
-000043f0: 7d94 2868 058c 043c 2f75 3e94 6807 5d94  }.(h...</u>.h.].
-00004400: 6816 8c04 3c2f 753e 9485 9481 947d 9428  h...</u>.....}.(
-00004410: 681b 6ae7 0500 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00004420: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00004430: 9468 255d 9468 275d 9468 295d 948c 0666  .h%].h'].h)]...f
-00004440: 6f72 6d61 7494 6a13 0200 0068 7a68 7b75  ormat.j....hzh{u
-00004450: 682b 6a02 0200 0068 1d68 2c68 1e4b 5768  h+j....h.h,h.KWh
-00004460: 1b6a d005 0000 681c 6803 7562 6a03 0200  .j....h.h.ubj...
-00004470: 0029 8194 7d94 2868 058c 043c 6272 3e94  .)..}.(h...<br>.
-00004480: 6807 5d94 6816 8c04 3c62 723e 9485 9481  h.].h...<br>....
-00004490: 947d 9428 681b 6af6 0500 0068 1c68 0368  .}.(h.j....h.h.h
-000044a0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000044b0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-000044c0: 948c 0666 6f72 6d61 7494 6a13 0200 0068  ...format.j....h
-000044d0: 7a68 7b75 682b 6a02 0200 0068 1d68 2c68  zh{uh+j....h.h,h
-000044e0: 1e4b 5768 1b6a d005 0000 681c 6803 7562  .KWh.j....h.h.ub
-000044f0: 6816 8c01 0a94 8594 8194 7d94 2868 1b6a  h.........}.(h.j
-00004500: d005 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00004510: 6816 8c41 4966 2066 756e 6374 696f 6e20  h..AIf function 
-00004520: 7261 6e20 636f 7272 6563 746c 792c 206e  ran correctly, n
-00004530: 6f20 6f75 7470 7574 2c20 6f74 6865 7277  o output, otherw
-00004540: 6973 6520 7261 6973 6573 2074 6865 2065  ise raises the e
-00004550: 7272 6f72 2e94 8594 8194 7d94 2868 1b6a  rror......}.(h.j
-00004560: d005 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00004570: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00004580: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
-00004590: 1e4b 5768 1d68 2c68 1b6a 3804 0000 681c  .KWh.h,h.j8...h.
-000045a0: 6803 7562 6568 1f7d 9428 6821 5d94 8c03  h.ubeh.}.(h!]...
-000045b0: 6964 3694 6168 235d 9468 255d 9468 275d  id6.ah#].h%].h']
-000045c0: 948c 0a68 6f77 2074 6f20 7573 6594 6168  ...how to use.ah
-000045d0: 295d 9475 682b 680a 681e 4b46 681d 682c  )].uh+h.h.KFh.h,
-000045e0: 681b 6ab3 0300 0068 1c68 0368 564b 0175  h.j....h.h.hVK.u
-000045f0: 6265 681f 7d94 2868 215d 948c 0b73 6176  beh.}.(h!]...sav
-00004600: 656d 6174 6669 6c65 9461 6823 5d94 6825  ematfile.ah#].h%
-00004610: 5d94 8c0b 7361 7665 6d61 7466 696c 6594  ]...savematfile.
-00004620: 6168 275d 9468 295d 9475 682b 680a 681e  ah'].h)].uh+h.h.
-00004630: 4b3d 681d 682c 681b 6a0b 0100 0068 1c68  K=h.h,h.j....h.h
-00004640: 0375 6268 0b29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
-00004650: 075d 9428 6810 2981 947d 9428 6805 8c0b  .].(h.)..}.(h...
-00004660: 636f 6e76 6572 7446 696c 6594 6807 5d94  convertFile.h.].
-00004670: 6816 8c0b 636f 6e76 6572 7446 696c 6594  h...convertFile.
-00004680: 8594 8194 7d94 2868 1b6a 2606 0000 681c  ....}.(h.j&...h.
-00004690: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-000046a0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000046b0: 6829 5d94 7568 2b68 0f68 1e4b 5a68 1d68  h)].uh+h.h.KZh.h
-000046c0: 2c68 1b6a 2306 0000 681c 6803 7562 680b  ,h.j#...h.h.ubh.
-000046d0: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
-000046e0: 1029 8194 7d94 2868 058c 0c50 7265 7365  .)..}.(h...Prese
-000046f0: 6e74 6174 696f 6e94 6807 5d94 6816 8c0c  ntation.h.].h...
-00004700: 5072 6573 656e 7461 7469 6f6e 9485 9481  Presentation....
-00004710: 947d 9428 681b 6a37 0600 0068 1c68 0368  .}.(h.j7...h.h.h
-00004720: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00004730: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00004740: 9475 682b 680f 681e 4b5b 681d 682c 681b  .uh+h.h.K[h.h,h.
-00004750: 6a34 0600 0068 1c68 0375 6268 3f29 8194  j4...h.h.ubh?)..
-00004760: 7d94 2868 058c 8441 6c6c 2069 6e20 6f6e  }.(h...All in on
-00004770: 6520 6675 6e63 7469 6f6e 2e20 5265 6164  e function. Read
-00004780: 7320 606d 7a44 6174 612e 786d 6c60 2066  s `mzData.xml` f
-00004790: 696c 6520 616e 6420 6175 746f 6d61 7469  ile and automati
-000047a0: 6361 6c6c 7920 7361 7665 7320 6974 2069  cally saves it i
-000047b0: 6e74 6f20 7468 6520 6578 706f 7274 2066  nto the export f
-000047c0: 6f6c 6465 722e 204e 6f20 7472 616e 7369  older. No transi
-000047d0: 7469 6f6e 2074 6f20 7468 6520 606d 7a44  tion to the `mzD
-000047e0: 6174 6160 2063 6c61 7373 2e94 6807 5d94  ata` class..h.].
-000047f0: 2868 168c 1b41 6c6c 2069 6e20 6f6e 6520  (h...All in one 
-00004800: 6675 6e63 7469 6f6e 2e20 5265 6164 7320  function. Reads 
-00004810: 9485 9481 947d 9428 681b 6a45 0600 0068  .....}.(h.jE...h
-00004820: 1c68 0368 1d4e 681e 4e75 626a 4701 0000  .h.h.Nh.NubjG...
-00004830: 2981 947d 9428 6805 8c0a 6d7a 4461 7461  )..}.(h...mzData
-00004840: 2e78 6d6c 9468 075d 9468 168c 0a6d 7a44  .xml.h.].h...mzD
-00004850: 6174 612e 786d 6c94 8594 8194 7d94 2868  ata.xml.....}.(h
-00004860: 1b6a 4d06 0000 681c 6803 681d 4e68 1e4e  .jM...h.h.h.Nh.N
-00004870: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00004880: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00004890: 4601 0000 681e 4b5c 681d 682c 681b 6a45  F...h.K\h.h,h.jE
-000048a0: 0600 0068 1c68 0375 6268 168c 4e20 6669  ...h.h.ubh..N fi
-000048b0: 6c65 2061 6e64 2061 7574 6f6d 6174 6963  le and automatic
-000048c0: 616c 6c79 2073 6176 6573 2069 7420 696e  ally saves it in
-000048d0: 746f 2074 6865 2065 7870 6f72 7420 666f  to the export fo
-000048e0: 6c64 6572 2e20 4e6f 2074 7261 6e73 6974  lder. No transit
-000048f0: 696f 6e20 746f 2074 6865 2094 8594 8194  ion to the .....
-00004900: 7d94 2868 1b6a 4506 0000 681c 6803 681d  }.(h.jE...h.h.h.
-00004910: 4e68 1e4e 7562 6a47 0100 0029 8194 7d94  Nh.NubjG...)..}.
-00004920: 2868 058c 066d 7a44 6174 6194 6807 5d94  (h...mzData.h.].
-00004930: 6816 8c06 6d7a 4461 7461 9485 9481 947d  h...mzData.....}
-00004940: 9428 681b 6a5f 0600 0068 1c68 0368 1d4e  .(h.j_...h.h.h.N
-00004950: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00004960: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00004970: 682b 6a46 0100 0068 1e4b 5c68 1d68 2c68  h+jF...h.K\h.h,h
-00004980: 1b6a 4506 0000 681c 6803 7562 6816 8c07  .jE...h.h.ubh...
-00004990: 2063 6c61 7373 2e94 8594 8194 7d94 2868   class......}.(h
-000049a0: 1b6a 4506 0000 681c 6803 681d 4e68 1e4e  .jE...h.h.h.Nh.N
-000049b0: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-000049c0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-000049d0: 3e68 1e4b 5c68 1d68 2c68 1b6a 3406 0000  >h.K\h.h,h.j4...
-000049e0: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
-000049f0: 8c03 6964 3794 6168 235d 9468 255d 9468  ..id7.ah#].h%].h
-00004a00: 275d 948c 0c70 7265 7365 6e74 6174 696f  ']...presentatio
-00004a10: 6e94 6168 295d 9475 682b 680a 681e 4b5b  n.ah)].uh+h.h.K[
-00004a20: 681d 682c 681b 6a23 0600 0068 1c68 0368  h.h,h.j#...h.h.h
-00004a30: 564b 0175 6268 0b29 8194 7d94 2868 0568  VK.ubh.)..}.(h.h
-00004a40: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
-00004a50: 8c0a 4465 6669 6e69 7469 6f6e 9468 075d  ..Definition.h.]
-00004a60: 9468 168c 0a44 6566 696e 6974 696f 6e94  .h...Definition.
-00004a70: 8594 8194 7d94 2868 1b6a 8206 0000 681c  ....}.(h.j....h.
-00004a80: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00004a90: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00004aa0: 6829 5d94 7568 2b68 0f68 1e4b 5e68 1d68  h)].uh+h.h.K^h.h
-00004ab0: 2c68 1b6a 7f06 0000 681c 6803 7562 6869  ,h.j....h.h.ubhi
-00004ac0: 2981 947d 9428 6805 8c98 6465 6620 636f  )..}.(h...def co
-00004ad0: 6e76 6572 7446 696c 6528 7365 6c66 406d  nvertFile(self@m
-00004ae0: 7a44 6174 614d 616e 6167 6572 2c20 6669  zDataManager, fi
-00004af0: 6c65 4e61 6d65 203a 2073 7472 2c20 6375  leName : str, cu
-00004b00: 7374 6f6d 4469 7265 6374 6f72 7920 3a20  stomDirectory : 
-00004b10: 626f 6f6c 203d 2046 616c 7365 2c20 6469  bool = False, di
-00004b20: 7232 5361 7665 203a 2073 7472 203d 204e  r2Save : str = N
-00004b30: 6f6e 652c 2066 6f72 6365 203a 2062 6f6f  one, force : boo
-00004b40: 6c20 3d20 4661 6c73 652c 2072 656d 6f76  l = False, remov
-00004b50: 6520 3a20 626f 6f6c 203d 2046 616c 7365  e : bool = False
-00004b60: 290a 9468 075d 9468 168c 9864 6566 2063  )..h.].h...def c
-00004b70: 6f6e 7665 7274 4669 6c65 2873 656c 6640  onvertFile(self@
-00004b80: 6d7a 4461 7461 4d61 6e61 6765 722c 2066  mzDataManager, f
-00004b90: 696c 654e 616d 6520 3a20 7374 722c 2063  ileName : str, c
-00004ba0: 7573 746f 6d44 6972 6563 746f 7279 203a  ustomDirectory :
-00004bb0: 2062 6f6f 6c20 3d20 4661 6c73 652c 2064   bool = False, d
-00004bc0: 6972 3253 6176 6520 3a20 7374 7220 3d20  ir2Save : str = 
-00004bd0: 4e6f 6e65 2c20 666f 7263 6520 3a20 626f  None, force : bo
-00004be0: 6f6c 203d 2046 616c 7365 2c20 7265 6d6f  ol = False, remo
-00004bf0: 7665 203a 2062 6f6f 6c20 3d20 4661 6c73  ve : bool = Fals
-00004c00: 6529 0a94 8594 8194 7d94 681b 6a90 0600  e)......}.h.j...
-00004c10: 0073 6261 681f 7d94 2868 215d 9468 235d  .sbah.}.(h!].h#]
-00004c20: 9468 255d 9468 275d 9468 295d 948c 086c  .h%].h'].h)]...l
-00004c30: 616e 6775 6167 6594 8c06 7079 7468 6f6e  anguage...python
-00004c40: 9468 7a68 7b75 682b 6868 681d 682c 681e  .hzh{uh+hhh.h,h.
-00004c50: 4b5f 681b 6a7f 0600 0068 1c68 0375 6265  K_h.j....h.h.ube
-00004c60: 681f 7d94 2868 215d 948c 0369 6438 9461  h.}.(h!]...id8.a
-00004c70: 6823 5d94 6825 5d94 6827 5d94 8c0a 6465  h#].h%].h']...de
-00004c80: 6669 6e69 7469 6f6e 9461 6829 5d94 7568  finition.ah)].uh
-00004c90: 2b68 0a68 1e4b 5e68 1d68 2c68 1b6a 2306  +h.h.K^h.h,h.j#.
-00004ca0: 0000 681c 6803 6856 4b01 7562 680b 2981  ..h.h.hVK.ubh.).
-00004cb0: 947d 9428 6805 6806 6807 5d94 2868 1029  .}.(h.h.h.].(h.)
-00004cc0: 8194 7d94 2868 058c 0a48 6f77 2074 6f20  ..}.(h...How to 
-00004cd0: 7573 6594 6807 5d94 6816 8c0a 486f 7720  use.h.].h...How 
-00004ce0: 746f 2075 7365 9485 9481 947d 9428 681b  to use.....}.(h.
-00004cf0: 6aab 0600 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00004d00: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00004d10: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
-00004d20: 681e 4b63 681d 682c 681b 6aa8 0600 0068  h.Kch.h,h.j....h
-00004d30: 1c68 0375 6268 6929 8194 7d94 2868 058c  .h.ubhi)..}.(h..
-00004d40: 8f23 2043 6f6e 7369 6465 7269 6e67 2074  .# Considering t
-00004d50: 6861 7420 6d7a 4461 7461 4d61 6e61 6765  hat mzDataManage
-00004d60: 7220 636c 6173 7320 6861 7320 6265 656e  r class has been
-00004d70: 2069 6e74 6961 6c69 7a65 6420 6265 666f   intialized befo
-00004d80: 7265 2061 6e64 2073 746f 7265 6420 6173  re and stored as
-00004d90: 206d 616e 6167 6572 2076 6172 6961 626c   manager variabl
-00004da0: 650a 0a6d 616e 6167 6572 2e63 6f6e 7665  e..manager.conve
-00004db0: 7274 4669 6c65 280a 2020 2020 6669 6c65  rtFile(.    file
-00004dc0: 4e61 6d65 3d46 696c 654e 616d 650a 290a  Name=FileName.).
-00004dd0: 9468 075d 9468 168c 8f23 2043 6f6e 7369  .h.].h...# Consi
-00004de0: 6465 7269 6e67 2074 6861 7420 6d7a 4461  dering that mzDa
-00004df0: 7461 4d61 6e61 6765 7220 636c 6173 7320  taManager class 
-00004e00: 6861 7320 6265 656e 2069 6e74 6961 6c69  has been intiali
-00004e10: 7a65 6420 6265 666f 7265 2061 6e64 2073  zed before and s
-00004e20: 746f 7265 6420 6173 206d 616e 6167 6572  tored as manager
-00004e30: 2076 6172 6961 626c 650a 0a6d 616e 6167   variable..manag
-00004e40: 6572 2e63 6f6e 7665 7274 4669 6c65 280a  er.convertFile(.
-00004e50: 2020 2020 6669 6c65 4e61 6d65 3d46 696c      fileName=Fil
-00004e60: 654e 616d 650a 290a 9485 9481 947d 9468  eName.)......}.h
-00004e70: 1b6a b906 0000 7362 6168 1f7d 9428 6821  .j....sbah.}.(h!
-00004e80: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00004e90: 5d94 8c08 6c61 6e67 7561 6765 948c 0670  ]...language...p
-00004ea0: 7974 686f 6e94 687a 687b 7568 2b68 6868  ython.hzh{uh+hhh
-00004eb0: 1d68 2c68 1e4b 6468 1b6a a806 0000 681c  .h,h.Kdh.j....h.
-00004ec0: 6803 7562 683f 2981 947d 9428 6805 8c11  h.ubh?)..}.(h...
-00004ed0: 3c75 3e50 6172 616d 6574 6572 733c 2f75  <u>Parameters</u
-00004ee0: 3e94 6807 5d94 286a 0302 0000 2981 947d  >.h.].(j....)..}
-00004ef0: 9428 6805 8c03 3c75 3e94 6807 5d94 6816  .(h...<u>.h.].h.
-00004f00: 8c03 3c75 3e94 8594 8194 7d94 2868 1b6a  ..<u>.....}.(h.j
-00004f10: cd06 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00004f20: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00004f30: 5d94 6827 5d94 6829 5d94 8c06 666f 726d  ].h'].h)]...form
-00004f40: 6174 946a 1302 0000 687a 687b 7568 2b6a  at.j....hzh{uh+j
-00004f50: 0202 0000 681d 682c 681e 4b6c 681b 6ac9  ....h.h,h.Klh.j.
-00004f60: 0600 0068 1c68 0375 6268 168c 0a50 6172  ...h.h.ubh...Par
-00004f70: 616d 6574 6572 7394 8594 8194 7d94 2868  ameters.....}.(h
-00004f80: 1b6a c906 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00004f90: 7562 6a03 0200 0029 8194 7d94 2868 058c  ubj....)..}.(h..
-00004fa0: 043c 2f75 3e94 6807 5d94 6816 8c04 3c2f  .</u>.h.].h...</
-00004fb0: 753e 9485 9481 947d 9428 681b 6ae0 0600  u>.....}.(h.j...
-00004fc0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00004fd0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00004fe0: 275d 9468 295d 948c 0666 6f72 6d61 7494  '].h)]...format.
-00004ff0: 6a13 0200 0068 7a68 7b75 682b 6a02 0200  j....hzh{uh+j...
-00005000: 0068 1d68 2c68 1e4b 6c68 1b6a c906 0000  .h.h,h.Klh.j....
-00005010: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
-00005020: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00005030: 7568 2b68 3e68 1e4b 6c68 1d68 2c68 1b6a  uh+h>h.Klh.h,h.j
-00005040: a806 0000 681c 6803 7562 6a2e 0200 0029  ....h.h.ubj....)
-00005050: 8194 7d94 2868 0568 0668 075d 9428 6a33  ..}.(h.h.h.].(j3
-00005060: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-00005070: 9428 683f 2981 947d 9428 6805 8c10 6066  .(h?)..}.(h...`f
-00005080: 696c 654e 616d 6560 203a 3c62 723e 9468  ileName` :<br>.h
-00005090: 075d 9428 6a47 0100 0029 8194 7d94 2868  .].(jG...)..}.(h
-000050a0: 058c 0866 696c 654e 616d 6594 6807 5d94  ...fileName.h.].
-000050b0: 6816 8c08 6669 6c65 4e61 6d65 9485 9481  h...fileName....
-000050c0: 947d 9428 681b 6aff 0600 0068 1c68 0368  .}.(h.j....h.h.h
-000050d0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000050e0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-000050f0: 9475 682b 6a46 0100 0068 1e4b 6d68 1d68  .uh+jF...h.Kmh.h
-00005100: 2c68 1b6a fb06 0000 681c 6803 7562 6816  ,h.j....h.h.ubh.
-00005110: 8c02 203a 9485 9481 947d 9428 681b 6afb  .. :.....}.(h.j.
-00005120: 0600 0068 1c68 0368 1d4e 681e 4e75 626a  ...h.h.h.Nh.Nubj
-00005130: 0302 0000 2981 947d 9428 6805 8c04 3c62  ....)..}.(h...<b
-00005140: 723e 9468 075d 9468 168c 043c 6272 3e94  r>.h.].h...<br>.
-00005150: 8594 8194 7d94 2868 1b6a 1107 0000 681c  ....}.(h.j....h.
-00005160: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00005170: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00005180: 6829 5d94 8c06 666f 726d 6174 946a 1302  h)]...format.j..
-00005190: 0000 687a 687b 7568 2b6a 0202 0000 681d  ..hzh{uh+j....h.
-000051a0: 682c 681e 4b6d 681b 6afb 0600 0068 1c68  h,h.Kmh.j....h.h
-000051b0: 0375 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
-000051c0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-000051d0: 683e 681e 4b6d 681d 682c 681b 6af8 0600  h>h.Kmh.h,h.j...
-000051e0: 0068 1c68 0375 626a 2e02 0000 2981 947d  .h.h.ubj....)..}
-000051f0: 9428 6805 6806 6807 5d94 286a 3302 0000  .(h.h.h.].(j3...
-00005200: 2981 947d 9428 6805 6806 6807 5d94 683f  )..}.(h.h.h.].h?
-00005210: 2981 947d 9428 6805 8c92 5368 6f75 6c64  )..}.(h...Should
-00005220: 2062 6520 7468 6520 6675 6c6c 2070 6174   be the full pat
-00005230: 6820 746f 2074 6865 2066 696c 6520 616e  h to the file an
-00005240: 6420 6974 2773 2065 7874 656e 7369 6f6e  d it's extension
-00005250: 2028 2e6d 7a64 6174 612e 786d 6c29 2074   (.mzdata.xml) t
-00005260: 6f20 636f 6e76 6572 7420 6966 206e 6f20  o convert if no 
-00005270: 7661 6c75 6520 7761 7320 6769 7665 6e20  value was given 
-00005280: 746f 2060 6d7a 4461 7461 5061 7468 6020  to `mzDataPath` 
-00005290: 7768 656e 2069 6e69 7469 616c 697a 696e  when initializin
-000052a0: 6720 7468 6520 636c 6173 732e 9468 075d  g the class..h.]
-000052b0: 9428 6816 8c6b 5368 6f75 6c64 2062 6520  .(h..kShould be 
-000052c0: 7468 6520 6675 6c6c 2070 6174 6820 746f  the full path to
-000052d0: 2074 6865 2066 696c 6520 616e 6420 6974   the file and it
-000052e0: e280 9973 2065 7874 656e 7369 6f6e 2028  ...s extension (
-000052f0: 2e6d 7a64 6174 612e 786d 6c29 2074 6f20  .mzdata.xml) to 
-00005300: 636f 6e76 6572 7420 6966 206e 6f20 7661  convert if no va
-00005310: 6c75 6520 7761 7320 6769 7665 6e20 746f  lue was given to
-00005320: 2094 8594 8194 7d94 2868 1b6a 2c07 0000   .....}.(h.j,...
-00005330: 681c 6803 681d 4e68 1e4e 7562 6a47 0100  h.h.h.Nh.NubjG..
-00005340: 0029 8194 7d94 2868 058c 0a6d 7a44 6174  .)..}.(h...mzDat
-00005350: 6150 6174 6894 6807 5d94 6816 8c0a 6d7a  aPath.h.].h...mz
-00005360: 4461 7461 5061 7468 9485 9481 947d 9428  DataPath.....}.(
-00005370: 681b 6a34 0700 0068 1c68 0368 1d4e 681e  h.j4...h.h.h.Nh.
-00005380: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00005390: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-000053a0: 6a46 0100 0068 1e4b 6e68 1d68 2c68 1b6a  jF...h.Knh.h,h.j
-000053b0: 2c07 0000 681c 6803 7562 6816 8c1d 2077  ,...h.h.ubh... w
-000053c0: 6865 6e20 696e 6974 6961 6c69 7a69 6e67  hen initializing
-000053d0: 2074 6865 2063 6c61 7373 2e94 8594 8194   the class......
-000053e0: 7d94 2868 1b6a 2c07 0000 681c 6803 681d  }.(h.j,...h.h.h.
-000053f0: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
-00005400: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00005410: 7568 2b68 3e68 1e4b 6e68 1d68 2c68 1b6a  uh+h>h.Knh.h,h.j
-00005420: 2907 0000 681c 6803 7562 6168 1f7d 9428  )...h.h.ubah.}.(
-00005430: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00005440: 6829 5d94 7568 2b6a 3202 0000 681e 4b6e  h)].uh+j2...h.Kn
-00005450: 681d 682c 681b 6a26 0700 0068 1c68 0375  h.h,h.j&...h.h.u
-00005460: 626a 3302 0000 2981 947d 9428 6805 6806  bj3...)..}.(h.h.
-00005470: 6807 5d94 683f 2981 947d 9428 6805 8c45  h.].h?)..}.(h..E
-00005480: 4f74 6865 7277 6973 652c 2074 6865 2066  Otherwise, the f
-00005490: 696c 6527 7320 7265 6c61 7469 7665 2070  ile's relative p
-000054a0: 6174 6820 7769 7468 2069 7427 7320 6578  ath with it's ex
-000054b0: 7465 6e73 696f 6e20 282e 6d7a 6461 7461  tension (.mzdata
-000054c0: 2e78 6d6c 2994 6807 5d94 6816 8c49 4f74  .xml).h.].h..IOt
-000054d0: 6865 7277 6973 652c 2074 6865 2066 696c  herwise, the fil
-000054e0: 65e2 8099 7320 7265 6c61 7469 7665 2070  e...s relative p
-000054f0: 6174 6820 7769 7468 2069 74e2 8099 7320  ath with it...s 
-00005500: 6578 7465 6e73 696f 6e20 282e 6d7a 6461  extension (.mzda
-00005510: 7461 2e78 6d6c 2994 8594 8194 7d94 2868  ta.xml).....}.(h
-00005520: 1b6a 5507 0000 681c 6803 681d 4e68 1e4e  .jU...h.h.h.Nh.N
-00005530: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00005540: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-00005550: 3e68 1e4b 6f68 1d68 2c68 1b6a 5207 0000  >h.Koh.h,h.jR...
-00005560: 681c 6803 7562 6168 1f7d 9428 6821 5d94  h.h.ubah.}.(h!].
-00005570: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00005580: 7568 2b6a 3202 0000 681e 4b6f 681d 682c  uh+j2...h.Koh.h,
-00005590: 681b 6a26 0700 0068 1c68 0375 6265 681f  h.j&...h.h.ubeh.
-000055a0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000055b0: 275d 9468 295d 946a bc02 0000 6abd 0200  '].h)].j....j...
-000055c0: 0075 682b 6a2d 0200 0068 1e4b 6e68 1d68  .uh+j-...h.Knh.h
-000055d0: 2c68 1b6a f806 0000 681c 6803 7562 6568  ,h.j....h.h.ubeh
-000055e0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-000055f0: 6827 5d94 6829 5d94 7568 2b6a 3202 0000  h'].h)].uh+j2...
-00005600: 681e 4b6d 681d 682c 681b 6af5 0600 0068  h.Kmh.h,h.j....h
-00005610: 1c68 0375 626a 3302 0000 2981 947d 9428  .h.ubj3...)..}.(
-00005620: 6805 6806 6807 5d94 683f 2981 947d 9428  h.h.h.].h?)..}.(
-00005630: 6805 8c7e 6063 7573 746f 6d44 6972 6563  h..~`customDirec
-00005640: 746f 7279 6020 3a20 5365 7420 7468 6973  tory` : Set this
-00005650: 2070 6172 616d 6574 6572 2074 6f20 6054   parameter to `T
-00005660: 7275 6560 2069 6620 7468 6520 6066 696c  rue` if the `fil
-00005670: 654e 616d 6560 2069 7320 696e 2061 2064  eName` is in a d
-00005680: 6966 6665 7265 6e74 2070 6174 6820 7468  ifferent path th
-00005690: 616e 2074 6865 206f 6e65 2067 6976 656e  an the one given
-000056a0: 2069 6e20 636f 6e66 6967 7572 6174 696f   in configuratio
-000056b0: 6e2e 9468 075d 9428 6a47 0100 0029 8194  n..h.].(jG...)..
-000056c0: 7d94 2868 058c 0f63 7573 746f 6d44 6972  }.(h...customDir
-000056d0: 6563 746f 7279 9468 075d 9468 168c 0f63  ectory.h.].h...c
-000056e0: 7573 746f 6d44 6972 6563 746f 7279 9485  ustomDirectory..
-000056f0: 9481 947d 9428 681b 6a7c 0700 0068 1c68  ...}.(h.j|...h.h
-00005700: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00005710: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00005720: 295d 9475 682b 6a46 0100 0068 1e4b 7068  )].uh+jF...h.Kph
-00005730: 1d68 2c68 1b6a 7807 0000 681c 6803 7562  .h,h.jx...h.h.ub
-00005740: 6816 8c19 203a 2053 6574 2074 6869 7320  h... : Set this 
-00005750: 7061 7261 6d65 7465 7220 746f 2094 8594  parameter to ...
-00005760: 8194 7d94 2868 1b6a 7807 0000 681c 6803  ..}.(h.jx...h.h.
-00005770: 681d 4e68 1e4e 7562 6a47 0100 0029 8194  h.Nh.NubjG...)..
-00005780: 7d94 2868 058c 0454 7275 6594 6807 5d94  }.(h...True.h.].
-00005790: 6816 8c04 5472 7565 9485 9481 947d 9428  h...True.....}.(
-000057a0: 681b 6a8e 0700 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-000057b0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-000057c0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-000057d0: 6a46 0100 0068 1e4b 7068 1d68 2c68 1b6a  jF...h.Kph.h,h.j
-000057e0: 7807 0000 681c 6803 7562 6816 8c08 2069  x...h.h.ubh... i
-000057f0: 6620 7468 6520 9485 9481 947d 9428 681b  f the .....}.(h.
-00005800: 6a78 0700 0068 1c68 0368 1d4e 681e 4e75  jx...h.h.h.Nh.Nu
-00005810: 626a 4701 0000 2981 947d 9428 6805 8c08  bjG...)..}.(h...
-00005820: 6669 6c65 4e61 6d65 9468 075d 9468 168c  fileName.h.].h..
-00005830: 0866 696c 654e 616d 6594 8594 8194 7d94  .fileName.....}.
-00005840: 2868 1b6a a007 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-00005850: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00005860: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00005870: 2b6a 4601 0000 681e 4b70 681d 682c 681b  +jF...h.Kph.h,h.
-00005880: 6a78 0700 0068 1c68 0375 6268 168c 3c20  jx...h.h.ubh..< 
-00005890: 6973 2069 6e20 6120 6469 6666 6572 656e  is in a differen
-000058a0: 7420 7061 7468 2074 6861 6e20 7468 6520  t path than the 
-000058b0: 6f6e 6520 6769 7665 6e20 696e 2063 6f6e  one given in con
-000058c0: 6669 6775 7261 7469 6f6e 2e94 8594 8194  figuration......
-000058d0: 7d94 2868 1b6a 7807 0000 681c 6803 681d  }.(h.jx...h.h.h.
-000058e0: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
-000058f0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00005900: 7568 2b68 3e68 1e4b 7068 1d68 2c68 1b6a  uh+h>h.Kph.h,h.j
-00005910: 7507 0000 681c 6803 7562 6168 1f7d 9428  u...h.h.ubah.}.(
-00005920: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00005930: 6829 5d94 7568 2b6a 3202 0000 681e 4b70  h)].uh+j2...h.Kp
-00005940: 681d 682c 681b 6af5 0600 0068 1c68 0375  h.h,h.j....h.h.u
-00005950: 626a 3302 0000 2981 947d 9428 6805 6806  bj3...)..}.(h.h.
-00005960: 6807 5d94 683f 2981 947d 9428 6805 8cbc  h.].h?)..}.(h...
-00005970: 6064 6972 3253 6176 6560 2020 203a 2053  `dir2Save`   : S
-00005980: 6176 6520 6469 7265 6374 6f72 7920 746f  ave directory to
-00005990: 2073 6176 6520 7468 6520 2e6d 6174 2066   save the .mat f
-000059a0: 696c 652e 2049 6620 7061 7468 2077 6173  ile. If path was
-000059b0: 2067 6976 656e 2069 6e20 636f 6e66 6967   given in config
-000059c0: 7572 6174 696f 6e2c 2069 7420 6973 206e  uration, it is n
-000059d0: 6f74 206e 6565 6465 642e 2054 6869 7320  ot needed. This 
-000059e0: 7061 7261 6d65 7465 7220 7769 6c6c 2062  parameter will b
-000059f0: 6520 7072 696f 7269 7469 7365 6420 6f76  e prioritised ov
-00005a00: 6572 2074 6865 2070 6174 6820 6769 7665  er the path give
-00005a10: 6e20 696e 2063 6f6e 6669 6775 7261 7469  n in configurati
-00005a20: 6f6e 2028 6966 2061 6e79 292e 9468 075d  on (if any)..h.]
-00005a30: 9428 6a47 0100 0029 8194 7d94 2868 058c  .(jG...)..}.(h..
-00005a40: 0864 6972 3253 6176 6594 6807 5d94 6816  .dir2Save.h.].h.
-00005a50: 8c08 6469 7232 5361 7665 9485 9481 947d  ..dir2Save.....}
-00005a60: 9428 681b 6ac5 0700 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00005a70: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00005a80: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00005a90: 682b 6a46 0100 0068 1e4b 7168 1d68 2c68  h+jF...h.Kqh.h,h
-00005aa0: 1b6a c107 0000 681c 6803 7562 6816 8cb2  .j....h.h.ubh...
-00005ab0: 2020 203a 2053 6176 6520 6469 7265 6374     : Save direct
-00005ac0: 6f72 7920 746f 2073 6176 6520 7468 6520  ory to save the 
-00005ad0: 2e6d 6174 2066 696c 652e 2049 6620 7061  .mat file. If pa
-00005ae0: 7468 2077 6173 2067 6976 656e 2069 6e20  th was given in 
-00005af0: 636f 6e66 6967 7572 6174 696f 6e2c 2069  configuration, i
-00005b00: 7420 6973 206e 6f74 206e 6565 6465 642e  t is not needed.
-00005b10: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
-00005b20: 7769 6c6c 2062 6520 7072 696f 7269 7469  will be prioriti
-00005b30: 7365 6420 6f76 6572 2074 6865 2070 6174  sed over the pat
-00005b40: 6820 6769 7665 6e20 696e 2063 6f6e 6669  h given in confi
-00005b50: 6775 7261 7469 6f6e 2028 6966 2061 6e79  guration (if any
-00005b60: 292e 9485 9481 947d 9428 681b 6ac1 0700  )......}.(h.j...
-00005b70: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
-00005b80: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00005b90: 275d 9468 295d 9475 682b 683e 681e 4b71  '].h)].uh+h>h.Kq
-00005ba0: 681d 682c 681b 6abe 0700 0068 1c68 0375  h.h,h.j....h.h.u
-00005bb0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00005bc0: 255d 9468 275d 9468 295d 9475 682b 6a32  %].h'].h)].uh+j2
-00005bd0: 0200 0068 1e4b 7168 1d68 2c68 1b6a f506  ...h.Kqh.h,h.j..
-00005be0: 0000 681c 6803 7562 6a33 0200 0029 8194  ..h.h.ubj3...)..
-00005bf0: 7d94 2868 0568 0668 075d 9468 3f29 8194  }.(h.h.h.].h?)..
-00005c00: 7d94 2868 058c ba60 666f 7263 6560 2020  }.(h...`force`  
-00005c10: 2020 2020 3a20 4966 2061 2066 696c 6520      : If a file 
-00005c20: 6861 7320 7468 6520 7361 6d65 206e 616d  has the same nam
-00005c30: 6520 696e 2074 6865 2063 6f6e 7665 7274  e in the convert
-00005c40: 6564 2066 6f6c 6465 722c 2073 686f 756c  ed folder, shoul
-00005c50: 6420 6974 2062 6520 7265 706c 6163 6564  d it be replaced
-00005c60: 203f 2028 4669 6c65 2077 696c 6c20 6e6f   ? (File will no
-00005c70: 7420 6265 2073 6176 6564 2069 6620 7369  t be saved if si
-00005c80: 626c 696e 6720 666f 756e 6420 696e 2063  bling found in c
-00005c90: 6f6e 7665 7274 2066 6f6c 6465 7220 616e  onvert folder an
-00005ca0: 6420 7468 6973 2070 6172 616d 6574 6572  d this parameter
-00005cb0: 2073 6574 2074 6f20 6046 616c 7365 602e   set to `False`.
-00005cc0: 2994 6807 5d94 286a 4701 0000 2981 947d  ).h.].(jG...)..}
-00005cd0: 9428 6805 8c05 666f 7263 6594 6807 5d94  .(h...force.h.].
-00005ce0: 6816 8c05 666f 7263 6594 8594 8194 7d94  h...force.....}.
-00005cf0: 2868 1b6a ea07 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-00005d00: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00005d10: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00005d20: 2b6a 4601 0000 681e 4b72 681d 682c 681b  +jF...h.Krh.h,h.
-00005d30: 6ae6 0700 0068 1c68 0375 6268 168c aa20  j....h.h.ubh... 
-00005d40: 2020 2020 203a 2049 6620 6120 6669 6c65       : If a file
-00005d50: 2068 6173 2074 6865 2073 616d 6520 6e61   has the same na
-00005d60: 6d65 2069 6e20 7468 6520 636f 6e76 6572  me in the conver
-00005d70: 7465 6420 666f 6c64 6572 2c20 7368 6f75  ted folder, shou
-00005d80: 6c64 2069 7420 6265 2072 6570 6c61 6365  ld it be replace
-00005d90: 6420 3f20 2846 696c 6520 7769 6c6c 206e  d ? (File will n
-00005da0: 6f74 2062 6520 7361 7665 6420 6966 2073  ot be saved if s
-00005db0: 6962 6c69 6e67 2066 6f75 6e64 2069 6e20  ibling found in 
-00005dc0: 636f 6e76 6572 7420 666f 6c64 6572 2061  convert folder a
-00005dd0: 6e64 2074 6869 7320 7061 7261 6d65 7465  nd this paramete
-00005de0: 7220 7365 7420 746f 2094 8594 8194 7d94  r set to .....}.
-00005df0: 2868 1b6a e607 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-00005e00: 1e4e 7562 6a47 0100 0029 8194 7d94 2868  .NubjG...)..}.(h
-00005e10: 058c 0546 616c 7365 9468 075d 9468 168c  ...False.h.].h..
-00005e20: 0546 616c 7365 9485 9481 947d 9428 681b  .False.....}.(h.
-00005e30: 6afc 0700 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00005e40: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00005e50: 255d 9468 275d 9468 295d 9475 682b 6a46  %].h'].h)].uh+jF
-00005e60: 0100 0068 1e4b 7268 1d68 2c68 1b6a e607  ...h.Krh.h,h.j..
-00005e70: 0000 681c 6803 7562 6816 8c02 2e29 9485  ..h.h.ubh....)..
-00005e80: 9481 947d 9428 681b 6ae6 0700 0068 1c68  ...}.(h.j....h.h
-00005e90: 0368 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
-00005ea0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00005eb0: 295d 9475 682b 683e 681e 4b72 681d 682c  )].uh+h>h.Krh.h,
-00005ec0: 681b 6ae3 0700 0068 1c68 0375 6261 681f  h.j....h.h.ubah.
-00005ed0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00005ee0: 275d 9468 295d 9475 682b 6a32 0200 0068  '].h)].uh+j2...h
-00005ef0: 1e4b 7268 1d68 2c68 1b6a f506 0000 681c  .Krh.h,h.j....h.
-00005f00: 6803 7562 6a33 0200 0029 8194 7d94 2868  h.ubj3...)..}.(h
-00005f10: 0568 0668 075d 9468 3f29 8194 7d94 2868  .h.h.].h?)..}.(h
-00005f20: 058c 5460 7265 6d6f 7665 6020 2020 2020  ..T`remove`     
-00005f30: 3a20 5368 6f75 6c64 2074 6865 206f 7269  : Should the ori
-00005f40: 6769 6e61 6c20 6669 6c65 2062 6520 7265  ginal file be re
-00005f50: 6d6f 7665 6420 7768 656e 2069 7420 6973  moved when it is
-00005f60: 2073 6176 6564 2061 7320 602e 6d61 7460   saved as `.mat`
-00005f70: 2066 696c 6520 3f94 6807 5d94 286a 4701   file ?.h.].(jG.
-00005f80: 0000 2981 947d 9428 6805 8c06 7265 6d6f  ..)..}.(h...remo
-00005f90: 7665 9468 075d 9468 168c 0672 656d 6f76  ve.h.].h...remov
-00005fa0: 6594 8594 8194 7d94 2868 1b6a 2108 0000  e.....}.(h.j!...
-00005fb0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00005fc0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00005fd0: 5d94 6829 5d94 7568 2b6a 4601 0000 681e  ].h)].uh+jF...h.
-00005fe0: 4b73 681d 682c 681b 6a1d 0800 0068 1c68  Ksh.h,h.j....h.h
-00005ff0: 0375 6268 168c 3f20 2020 2020 3a20 5368  .ubh..?     : Sh
-00006000: 6f75 6c64 2074 6865 206f 7269 6769 6e61  ould the origina
-00006010: 6c20 6669 6c65 2062 6520 7265 6d6f 7665  l file be remove
-00006020: 6420 7768 656e 2069 7420 6973 2073 6176  d when it is sav
-00006030: 6564 2061 7320 9485 9481 947d 9428 681b  ed as .....}.(h.
-00006040: 6a1d 0800 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00006050: 626a 4701 0000 2981 947d 9428 6805 8c04  bjG...)..}.(h...
-00006060: 2e6d 6174 9468 075d 9468 168c 042e 6d61  .mat.h.].h....ma
-00006070: 7494 8594 8194 7d94 2868 1b6a 3308 0000  t.....}.(h.j3...
-00006080: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00006090: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000060a0: 5d94 6829 5d94 7568 2b6a 4601 0000 681e  ].h)].uh+jF...h.
-000060b0: 4b73 681d 682c 681b 6a1d 0800 0068 1c68  Ksh.h,h.j....h.h
-000060c0: 0375 6268 168c 0720 6669 6c65 203f 9485  .ubh... file ?..
-000060d0: 9481 947d 9428 681b 6a1d 0800 0068 1c68  ...}.(h.j....h.h
-000060e0: 0368 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
-000060f0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00006100: 295d 9475 682b 683e 681e 4b73 681d 682c  )].uh+h>h.Ksh.h,
-00006110: 681b 6a1a 0800 0068 1c68 0375 6261 681f  h.j....h.h.ubah.
-00006120: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00006130: 275d 9468 295d 9475 682b 6a32 0200 0068  '].h)].uh+j2...h
-00006140: 1e4b 7368 1d68 2c68 1b6a f506 0000 681c  .Ksh.h,h.j....h.
-00006150: 6803 7562 6568 1f7d 9428 6821 5d94 6823  h.ubeh.}.(h!].h#
-00006160: 5d94 6825 5d94 6827 5d94 6829 5d94 6abc  ].h%].h'].h)].j.
-00006170: 0200 006a bd02 0000 7568 2b6a 2d02 0000  ...j....uh+j-...
-00006180: 681e 4b6d 681d 682c 681b 6aa8 0600 0068  h.Kmh.h,h.j....h
-00006190: 1c68 0375 6268 3f29 8194 7d94 2868 058c  .h.ubh?)..}.(h..
-000061a0: 1d3c 753e 4f75 7470 7574 733c 2f75 3e3c  .<u>Outputs</u><
-000061b0: 6272 3e0a 4e6f 206f 7574 7075 7473 9468  br>.No outputs.h
-000061c0: 075d 9428 6a03 0200 0029 8194 7d94 2868  .].(j....)..}.(h
-000061d0: 058c 033c 753e 9468 075d 9468 168c 033c  ...<u>.h.].h...<
-000061e0: 753e 9485 9481 947d 9428 681b 6a5b 0800  u>.....}.(h.j[..
-000061f0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00006200: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00006210: 275d 9468 295d 948c 0666 6f72 6d61 7494  '].h)]...format.
-00006220: 6a13 0200 0068 7a68 7b75 682b 6a02 0200  j....hzh{uh+j...
-00006230: 0068 1d68 2c68 1e4b 7568 1b6a 5708 0000  .h.h,h.Kuh.jW...
-00006240: 681c 6803 7562 6816 8c07 4f75 7470 7574  h.h.ubh...Output
-00006250: 7394 8594 8194 7d94 2868 1b6a 5708 0000  s.....}.(h.jW...
-00006260: 681c 6803 681d 4e68 1e4e 7562 6a03 0200  h.h.h.Nh.Nubj...
-00006270: 0029 8194 7d94 2868 058c 043c 2f75 3e94  .)..}.(h...</u>.
-00006280: 6807 5d94 6816 8c04 3c2f 753e 9485 9481  h.].h...</u>....
-00006290: 947d 9428 681b 6a6e 0800 0068 1c68 0368  .}.(h.jn...h.h.h
-000062a0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000062b0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-000062c0: 948c 0666 6f72 6d61 7494 6a13 0200 0068  ...format.j....h
-000062d0: 7a68 7b75 682b 6a02 0200 0068 1d68 2c68  zh{uh+j....h.h,h
-000062e0: 1e4b 7568 1b6a 5708 0000 681c 6803 7562  .Kuh.jW...h.h.ub
-000062f0: 6a03 0200 0029 8194 7d94 2868 058c 043c  j....)..}.(h...<
-00006300: 6272 3e94 6807 5d94 6816 8c04 3c62 723e  br>.h.].h...<br>
-00006310: 9485 9481 947d 9428 681b 6a7d 0800 0068  .....}.(h.j}...h
-00006320: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-00006330: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00006340: 9468 295d 948c 0666 6f72 6d61 7494 6a13  .h)]...format.j.
-00006350: 0200 0068 7a68 7b75 682b 6a02 0200 0068  ...hzh{uh+j....h
-00006360: 1d68 2c68 1e4b 7568 1b6a 5708 0000 681c  .h,h.Kuh.jW...h.
-00006370: 6803 7562 6816 8c01 0a94 8594 8194 7d94  h.ubh.........}.
-00006380: 2868 1b6a 5708 0000 681c 6803 681d 4e68  (h.jW...h.h.h.Nh
-00006390: 1e4e 7562 6816 8c0a 4e6f 206f 7574 7075  .Nubh...No outpu
-000063a0: 7473 9485 9481 947d 9428 681b 6a57 0800  ts.....}.(h.jW..
-000063b0: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
-000063c0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000063d0: 275d 9468 295d 9475 682b 683e 681e 4b75  '].h)].uh+h>h.Ku
-000063e0: 681d 682c 681b 6aa8 0600 0068 1c68 0375  h.h,h.j....h.h.u
-000063f0: 6265 681f 7d94 2868 215d 948c 0369 6439  beh.}.(h!]...id9
-00006400: 9461 6823 5d94 6825 5d94 6827 5d94 8c0a  .ah#].h%].h']...
-00006410: 686f 7720 746f 2075 7365 9461 6829 5d94  how to use.ah)].
-00006420: 7568 2b68 0a68 1e4b 6368 1d68 2c68 1b6a  uh+h.h.Kch.h,h.j
-00006430: 2306 0000 681c 6803 6856 4b01 7562 6568  #...h.h.hVK.ubeh
-00006440: 1f7d 9428 6821 5d94 8c0b 636f 6e76 6572  .}.(h!]...conver
-00006450: 7466 696c 6594 6168 235d 9468 255d 948c  tfile.ah#].h%]..
-00006460: 0b63 6f6e 7665 7274 6669 6c65 9461 6827  .convertfile.ah'
-00006470: 5d94 6829 5d94 7568 2b68 0a68 1e4b 5a68  ].h)].uh+h.h.KZh
-00006480: 1d68 2c68 1b6a 0b01 0000 681c 6803 7562  .h,h.j....h.h.ub
-00006490: 6568 1f7d 9428 6821 5d94 8c09 6675 6e63  eh.}.(h!]...func
-000064a0: 7469 6f6e 7394 6168 235d 9468 255d 948c  tions.ah#].h%]..
-000064b0: 0966 756e 6374 696f 6e73 9461 6827 5d94  .functions.ah'].
-000064c0: 6829 5d94 7568 2b68 0a68 1e4b 1e68 1d68  h)].uh+h.h.K.h.h
-000064d0: 2c68 1b68 0c68 1c68 0375 6265 681f 7d94  ,h.h.h.h.ubeh.}.
-000064e0: 2868 215d 948c 0d6d 7a64 6174 616d 616e  (h!]...mzdataman
-000064f0: 6167 6572 9461 6823 5d94 6825 5d94 8c0d  ager.ah#].h%]...
-00006500: 6d7a 6461 7461 6d61 6e61 6765 7294 6168  mzdatamanager.ah
-00006510: 275d 9468 295d 9475 682b 680a 681e 4b01  '].h)].uh+h.h.K.
-00006520: 681d 682c 681b 6803 681c 6803 7562 6168  h.h,h.h.h.h.ubah
-00006530: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00006540: 6827 5d94 6829 5d94 8c06 736f 7572 6365  h'].h)]...source
-00006550: 9468 2c8c 1474 7261 6e73 6c61 7469 6f6e  .h,..translation
-00006560: 5f70 726f 6772 6573 7394 7d94 288c 0574  _progress.}.(..t
-00006570: 6f74 616c 944b 008c 0a74 7261 6e73 6c61  otal.K...transla
-00006580: 7465 6494 4b00 7575 682b 6801 8c0e 6375  ted.K.uuh+h...cu
-00006590: 7272 656e 745f 736f 7572 6365 944e 8c0c  rrent_source.N..
-000065a0: 6375 7272 656e 745f 6c69 6e65 944e 8c08  current_line.N..
-000065b0: 7365 7474 696e 6773 948c 1164 6f63 7574  settings...docut
-000065c0: 696c 732e 6672 6f6e 7465 6e64 948c 0656  ils.frontend...V
-000065d0: 616c 7565 7394 9394 2981 947d 9428 680f  alues...)..}.(h.
-000065e0: 4e8c 0967 656e 6572 6174 6f72 944e 8c09  N..generator.N..
-000065f0: 6461 7465 7374 616d 7094 4e8c 0b73 6f75  datestamp.N..sou
-00006600: 7263 655f 6c69 6e6b 944e 8c0a 736f 7572  rce_link.N..sour
-00006610: 6365 5f75 726c 944e 8c0d 746f 635f 6261  ce_url.N..toc_ba
-00006620: 636b 6c69 6e6b 7394 8c05 656e 7472 7994  cklinks...entry.
-00006630: 8c12 666f 6f74 6e6f 7465 5f62 6163 6b6c  ..footnote_backl
-00006640: 696e 6b73 944b 018c 0d73 6563 746e 756d  inks.K...sectnum
-00006650: 5f78 666f 726d 944b 018c 0e73 7472 6970  _xform.K...strip
-00006660: 5f63 6f6d 6d65 6e74 7394 4e8c 1b73 7472  _comments.N..str
-00006670: 6970 5f65 6c65 6d65 6e74 735f 7769 7468  ip_elements_with
-00006680: 5f63 6c61 7373 6573 944e 8c0d 7374 7269  _classes.N..stri
-00006690: 705f 636c 6173 7365 7394 4e8c 0c72 6570  p_classes.N..rep
-000066a0: 6f72 745f 6c65 7665 6c94 4b02 8c0a 6861  ort_level.K...ha
-000066b0: 6c74 5f6c 6576 656c 944b 058c 1165 7869  lt_level.K...exi
-000066c0: 745f 7374 6174 7573 5f6c 6576 656c 944b  t_status_level.K
-000066d0: 058c 0564 6562 7567 944e 8c0e 7761 726e  ...debug.N..warn
-000066e0: 696e 675f 7374 7265 616d 944e 8c09 7472  ing_stream.N..tr
-000066f0: 6163 6562 6163 6b94 888c 0e69 6e70 7574  aceback....input
-00006700: 5f65 6e63 6f64 696e 6794 8c09 7574 662d  _encoding...utf-
-00006710: 382d 7369 6794 8c1c 696e 7075 745f 656e  8-sig...input_en
-00006720: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
-00006730: 646c 6572 948c 0673 7472 6963 7494 8c0f  dler...strict...
-00006740: 6f75 7470 7574 5f65 6e63 6f64 696e 6794  output_encoding.
-00006750: 8c05 7574 662d 3894 8c1d 6f75 7470 7574  ..utf-8...output
-00006760: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
-00006770: 6861 6e64 6c65 7294 6ae1 0800 008c 0e65  handler.j......e
-00006780: 7272 6f72 5f65 6e63 6f64 696e 6794 8c05  rror_encoding...
-00006790: 7574 662d 3894 8c1c 6572 726f 725f 656e  utf-8...error_en
-000067a0: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
-000067b0: 646c 6572 948c 1062 6163 6b73 6c61 7368  dler...backslash
-000067c0: 7265 706c 6163 6594 8c0d 6c61 6e67 7561  replace...langua
-000067d0: 6765 5f63 6f64 6594 8c02 656e 948c 1372  ge_code...en...r
-000067e0: 6563 6f72 645f 6465 7065 6e64 656e 6369  ecord_dependenci
-000067f0: 6573 944e 8c06 636f 6e66 6967 944e 8c09  es.N..config.N..
-00006800: 6964 5f70 7265 6669 7894 6806 8c0e 6175  id_prefix.h...au
-00006810: 746f 5f69 645f 7072 6566 6978 948c 0269  to_id_prefix...i
-00006820: 6494 8c0d 6475 6d70 5f73 6574 7469 6e67  d...dump_setting
-00006830: 7394 4e8c 0e64 756d 705f 696e 7465 726e  s.N..dump_intern
-00006840: 616c 7394 4e8c 0f64 756d 705f 7472 616e  als.N..dump_tran
-00006850: 7366 6f72 6d73 944e 8c0f 6475 6d70 5f70  sforms.N..dump_p
-00006860: 7365 7564 6f5f 786d 6c94 4e8c 1065 7870  seudo_xml.N..exp
-00006870: 6f73 655f 696e 7465 726e 616c 7394 4e8c  ose_internals.N.
-00006880: 0e73 7472 6963 745f 7669 7369 746f 7294  .strict_visitor.
-00006890: 4e8c 0f5f 6469 7361 626c 655f 636f 6e66  N.._disable_conf
-000068a0: 6967 944e 8c07 5f73 6f75 7263 6594 682c  ig.N.._source.h,
-000068b0: 8c0c 5f64 6573 7469 6e61 7469 6f6e 944e  .._destination.N
-000068c0: 8c0d 5f63 6f6e 6669 675f 6669 6c65 7394  .._config_files.
-000068d0: 5d94 8c16 6669 6c65 5f69 6e73 6572 7469  ]...file_inserti
-000068e0: 6f6e 5f65 6e61 626c 6564 9488 8c0b 7261  on_enabled....ra
-000068f0: 775f 656e 6162 6c65 6494 4b01 8c11 6c69  w_enabled.K...li
-00006900: 6e65 5f6c 656e 6774 685f 6c69 6d69 7494  ne_length_limit.
-00006910: 4d10 278c 0e70 6570 5f72 6566 6572 656e  M.'..pep_referen
-00006920: 6365 7394 4e8c 0c70 6570 5f62 6173 655f  ces.N..pep_base_
-00006930: 7572 6c94 8c18 6874 7470 733a 2f2f 7065  url...https://pe
-00006940: 7073 2e70 7974 686f 6e2e 6f72 672f 948c  ps.python.org/..
-00006950: 1570 6570 5f66 696c 655f 7572 6c5f 7465  .pep_file_url_te
-00006960: 6d70 6c61 7465 948c 0870 6570 2d25 3034  mplate...pep-%04
-00006970: 6494 8c0e 7266 635f 7265 6665 7265 6e63  d...rfc_referenc
-00006980: 6573 944e 8c0c 7266 635f 6261 7365 5f75  es.N..rfc_base_u
-00006990: 726c 948c 2668 7474 7073 3a2f 2f64 6174  rl..&https://dat
-000069a0: 6174 7261 636b 6572 2e69 6574 662e 6f72  atracker.ietf.or
-000069b0: 672f 646f 632f 6874 6d6c 2f94 8c09 7461  g/doc/html/...ta
-000069c0: 625f 7769 6474 6894 4b08 8c1d 7472 696d  b_width.K...trim
-000069d0: 5f66 6f6f 746e 6f74 655f 7265 6665 7265  _footnote_refere
-000069e0: 6e63 655f 7370 6163 6594 898c 1073 796e  nce_space....syn
-000069f0: 7461 785f 6869 6768 6c69 6768 7494 8c04  tax_highlight...
-00006a00: 6c6f 6e67 948c 0c73 6d61 7274 5f71 756f  long...smart_quo
-00006a10: 7465 7394 888c 1373 6d61 7274 7175 6f74  tes....smartquot
-00006a20: 6573 5f6c 6f63 616c 6573 945d 948c 1d63  es_locales.]...c
-00006a30: 6861 7261 6374 6572 5f6c 6576 656c 5f69  haracter_level_i
-00006a40: 6e6c 696e 655f 6d61 726b 7570 9489 8c0e  nline_markup....
-00006a50: 646f 6374 6974 6c65 5f78 666f 726d 9489  doctitle_xform..
-00006a60: 8c0d 646f 6369 6e66 6f5f 7866 6f72 6d94  ..docinfo_xform.
-00006a70: 4b01 8c12 7365 6374 7375 6274 6974 6c65  K...sectsubtitle
-00006a80: 5f78 666f 726d 9489 8c0d 696d 6167 655f  _xform....image_
-00006a90: 6c6f 6164 696e 6794 8c04 6c69 6e6b 948c  loading...link..
-00006aa0: 1065 6d62 6564 5f73 7479 6c65 7368 6565  .embed_styleshee
-00006ab0: 7494 898c 1563 6c6f 616b 5f65 6d61 696c  t....cloak_email
-00006ac0: 5f61 6464 7265 7373 6573 9488 8c11 7365  _addresses....se
-00006ad0: 6374 696f 6e5f 7365 6c66 5f6c 696e 6b94  ction_self_link.
-00006ae0: 898c 0365 6e76 944e 7562 8c08 7265 706f  ...env.Nub..repo
-00006af0: 7274 6572 944e 8c10 696e 6469 7265 6374  rter.N..indirect
-00006b00: 5f74 6172 6765 7473 945d 948c 1173 7562  _targets.]...sub
-00006b10: 7374 6974 7574 696f 6e5f 6465 6673 947d  stitution_defs.}
-00006b20: 9428 8c0f 776f 7264 636f 756e 742d 776f  .(..wordcount-wo
-00006b30: 7264 7394 6809 8c17 7375 6273 7469 7475  rds.h...substitu
-00006b40: 7469 6f6e 5f64 6566 696e 6974 696f 6e94  tion_definition.
-00006b50: 9394 2981 947d 9428 6805 8c03 3433 3594  ..)..}.(h...435.
-00006b60: 6807 5d94 6816 8c03 3433 3594 8594 8194  h.].h...435.....
-00006b70: 7d94 681b 6a1f 0900 0073 6261 681f 7d94  }.h.j....sbah.}.
-00006b80: 2868 215d 9468 235d 9468 255d 948c 0f77  (h!].h#].h%]...w
-00006b90: 6f72 6463 6f75 6e74 2d77 6f72 6473 9461  ordcount-words.a
-00006ba0: 6827 5d94 6829 5d94 7568 2b6a 1d09 0000  h'].h)].uh+j....
-00006bb0: 681d 682c 7562 8c11 776f 7264 636f 756e  h.h,ub..wordcoun
-00006bc0: 742d 6d69 6e75 7465 7394 6a1e 0900 0029  t-minutes.j....)
-00006bd0: 8194 7d94 2868 058c 0132 9468 075d 9468  ..}.(h...2.h.].h
-00006be0: 168c 0132 9485 9481 947d 9468 1b6a 2f09  ...2.....}.h.j/.
-00006bf0: 0000 7362 6168 1f7d 9428 6821 5d94 6823  ..sbah.}.(h!].h#
-00006c00: 5d94 6825 5d94 8c11 776f 7264 636f 756e  ].h%]...wordcoun
-00006c10: 742d 6d69 6e75 7465 7394 6168 275d 9468  t-minutes.ah'].h
-00006c20: 295d 9475 682b 6a1d 0900 0068 1d68 2c75  )].uh+j....h.h,u
-00006c30: 6275 8c12 7375 6273 7469 7475 7469 6f6e  bu..substitution
-00006c40: 5f6e 616d 6573 947d 9428 8c0f 776f 7264  _names.}.(..word
-00006c50: 636f 756e 742d 776f 7264 7394 6a1c 0900  count-words.j...
-00006c60: 008c 1177 6f72 6463 6f75 6e74 2d6d 696e  ...wordcount-min
-00006c70: 7574 6573 946a 2e09 0000 758c 0872 6566  utes.j....u..ref
-00006c80: 6e61 6d65 7394 7d94 8c06 7265 6669 6473  names.}...refids
-00006c90: 947d 948c 076e 616d 6569 6473 947d 9428  .}...nameids.}.(
-00006ca0: 6ab7 0800 006a b408 0000 8c0c 7072 6573  j....j......pres
-00006cb0: 656e 7461 7469 6f6e 944e 8c0a 6465 6669  entation.N..defi
-00006cc0: 6e69 7469 6f6e 944e 8c0a 686f 7720 746f  nition.N..how to
-00006cd0: 2075 7365 944e 68c9 68c6 6a00 0100 0068   use.Nh.h.j....h
-00006ce0: fd6a af08 0000 6aac 0800 006a b003 0000  .j....j....j....
-00006cf0: 6aad 0300 006a 2006 0000 6a1d 0600 006a  j....j ...j....j
-00006d00: a708 0000 6aa4 0800 0075 8c09 6e61 6d65  ....j....u..name
-00006d10: 7479 7065 7394 7d94 286a b708 0000 896a  types.}.(j.....j
-00006d20: 4809 0000 896a 4909 0000 896a 4a09 0000  H....jI....jJ...
-00006d30: 8968 c989 6a00 0100 0089 6aaf 0800 0089  .h..j.....j.....
-00006d40: 6ab0 0300 0089 6a20 0600 0089 6aa7 0800  j.....j ....j...
-00006d50: 0089 7568 217d 9428 6ab4 0800 0068 0c68  ..uh!}.(j....h.h
-00006d60: 5068 2d68 7e68 576a 0501 0000 6884 68c6  Ph-h~hWj....h.h.
-00006d70: 6895 68fd 68cc 6aac 0800 006a 0b01 0000  h.h.h.j....j....
-00006d80: 6aad 0300 006a 1c01 0000 6ab0 0100 006a  j....j....j....j
-00006d90: 2d01 0000 6ad8 0100 006a b501 0000 6aa6  -...j....j....j.
-00006da0: 0300 006a dd01 0000 6a1d 0600 006a b303  ...j....j....j..
-00006db0: 0000 6a09 0400 006a c403 0000 6a32 0400  ..j....j....j2..
-00006dc0: 006a 0f04 0000 6a15 0600 006a 3804 0000  .j....j....j8...
-00006dd0: 6aa4 0800 006a 2306 0000 6a79 0600 006a  j....j#...jy...j
-00006de0: 3406 0000 6aa2 0600 006a 7f06 0000 6a9c  4...j....j....j.
-00006df0: 0800 006a a806 0000 758c 0d66 6f6f 746e  ...j....u..footn
-00006e00: 6f74 655f 7265 6673 947d 948c 0d63 6974  ote_refs.}...cit
-00006e10: 6174 696f 6e5f 7265 6673 947d 948c 0d61  ation_refs.}...a
-00006e20: 7574 6f66 6f6f 746e 6f74 6573 945d 948c  utofootnotes.]..
-00006e30: 1161 7574 6f66 6f6f 746e 6f74 655f 7265  .autofootnote_re
-00006e40: 6673 945d 948c 1073 796d 626f 6c5f 666f  fs.]...symbol_fo
-00006e50: 6f74 6e6f 7465 7394 5d94 8c14 7379 6d62  otnotes.]...symb
-00006e60: 6f6c 5f66 6f6f 746e 6f74 655f 7265 6673  ol_footnote_refs
-00006e70: 945d 948c 0966 6f6f 746e 6f74 6573 945d  .]...footnotes.]
-00006e80: 948c 0963 6974 6174 696f 6e73 945d 948c  ...citations.]..
-00006e90: 1261 7574 6f66 6f6f 746e 6f74 655f 7374  .autofootnote_st
-00006ea0: 6172 7494 4b01 8c15 7379 6d62 6f6c 5f66  art.K...symbol_f
-00006eb0: 6f6f 746e 6f74 655f 7374 6172 7494 4b00  ootnote_start.K.
-00006ec0: 8c0a 6964 5f63 6f75 6e74 6572 948c 0b63  ..id_counter...c
-00006ed0: 6f6c 6c65 6374 696f 6e73 948c 0743 6f75  ollections...Cou
-00006ee0: 6e74 6572 9493 947d 946a ef08 0000 4b09  nter...}.j....K.
-00006ef0: 7385 9452 948c 0e70 6172 7365 5f6d 6573  s..R...parse_mes
-00006f00: 7361 6765 7394 5d94 8c12 7472 616e 7366  sages.]...transf
-00006f10: 6f72 6d5f 6d65 7373 6167 6573 945d 948c  orm_messages.]..
-00006f20: 0b74 7261 6e73 666f 726d 6572 944e 8c0b  .transformer.N..
-00006f30: 696e 636c 7564 655f 6c6f 6794 5d94 8c0a  include_log.]...
-00006f40: 6465 636f 7261 7469 6f6e 944e 681c 6803  decoration.Nh.h.
-00006f50: 8c0a 6d79 7374 5f73 6c75 6773 947d 9475  ..myst_slugs.}.u
-00006f60: 622e                                     b.
+00000140: 6d65 9468 0f68 1e4b 0168 1d8c 5c43 3a5c  me.h.h.K.h..\C:\
+00000150: 5573 6572 735c 6d61 7869 6d5c 4f6e 6544  Users\maxim\OneD
+00000160: 7269 7665 5c44 6f63 756d 656e 7473 5c50  rive\Documents\P
+00000170: 7974 686f 6e5c 5061 636b 6167 6573 5c6d  ython\Packages\m
+00000180: 7a44 6174 6158 4d4c 324d 6174 5c64 6f63  zDataXML2Mat\doc
+00000190: 735c 736f 7572 6365 5c6d 7a44 6174 614d  s\source\mzDataM
+000001a0: 616e 6167 6572 2e6d 6494 681b 680c 681c  anager.md.h.h.h.
+000001b0: 6803 7562 680b 2981 947d 9428 6805 6806  h.ubh.)..}.(h.h.
+000001c0: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
+000001d0: 0c50 7265 7365 6e74 6174 696f 6e94 6807  .Presentation.h.
+000001e0: 5d94 6816 8c0c 5072 6573 656e 7461 7469  ].h...Presentati
+000001f0: 6f6e 9485 9481 947d 9428 681b 6830 681c  on.....}.(h.h0h.
+00000200: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+00000210: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00000220: 6829 5d94 7568 2b68 0f68 1e4b 0368 1d68  h)].uh+h.h.K.h.h
+00000230: 2c68 1b68 2d68 1c68 0375 6268 098c 0970  ,h.h-h.h.ubh...p
+00000240: 6172 6167 7261 7068 9493 9429 8194 7d94  aragraph...)..}.
+00000250: 2868 058c 3e4d 6169 6e20 636c 6173 7320  (h..>Main class 
+00000260: 7573 6564 2066 6f72 2063 6f6e 7665 7274  used for convert
+00000270: 696e 6720 6d7a 4461 7461 2066 696c 6573  ing mzData files
+00000280: 2069 6e74 6f20 6d61 746c 6162 2066 696c   into matlab fil
+00000290: 6573 2e94 6807 5d94 6816 8c3e 4d61 696e  es..h.].h..>Main
+000002a0: 2063 6c61 7373 2075 7365 6420 666f 7220   class used for 
+000002b0: 636f 6e76 6572 7469 6e67 206d 7a44 6174  converting mzDat
+000002c0: 6120 6669 6c65 7320 696e 746f 206d 6174  a files into mat
+000002d0: 6c61 6220 6669 6c65 732e 9485 9481 947d  lab files......}
+000002e0: 9428 681b 6840 681c 6803 681d 4e68 1e4e  .(h.h@h.h.h.Nh.N
+000002f0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00000300: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00000310: 3e68 1e4b 0468 1d68 2c68 1b68 2d68 1c68  >h.K.h.h,h.h-h.h
+00000320: 0375 6265 681f 7d94 2868 215d 948c 0c70  .ubeh.}.(h!]...p
+00000330: 7265 7365 6e74 6174 696f 6e94 6168 235d  resentation.ah#]
+00000340: 9468 255d 9468 275d 948c 0c70 7265 7365  .h%].h']...prese
+00000350: 6e74 6174 696f 6e94 6168 295d 9475 682b  ntation.ah)].uh+
+00000360: 680a 681e 4b03 681d 682c 681b 680c 681c  h.h.K.h.h,h.h.h.
+00000370: 6803 8c0a 7265 6665 7265 6e63 6564 944b  h...referenced.K
+00000380: 0175 6268 0b29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
+00000390: 075d 9428 6810 2981 947d 9428 6805 8c0a  .].(h.)..}.(h...
+000003a0: 4465 6669 6e69 7469 6f6e 9468 075d 9468  Definition.h.].h
+000003b0: 168c 0a44 6566 696e 6974 696f 6e94 8594  ...Definition...
+000003c0: 8194 7d94 2868 1b68 5a68 1c68 0368 1d4e  ..}.(h.hZh.h.h.N
+000003d0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+000003e0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+000003f0: 682b 680f 681e 4b06 681d 682c 681b 6857  h+h.h.K.h.h,h.hW
+00000400: 681c 6803 7562 6809 8c0d 6c69 7465 7261  h.h.ubh...litera
+00000410: 6c5f 626c 6f63 6b94 9394 2981 947d 9428  l_block...)..}.(
+00000420: 6805 8c77 636c 6173 7320 6d7a 4461 7461  h..wclass mzData
+00000430: 4d61 6e61 6765 7228 4261 7365 4d6f 6465  Manager(BaseMode
+00000440: 6c29 3a0a 2020 2020 6d7a 4461 7461 5061  l):.    mzDataPa
+00000450: 7468 203a 2073 7472 203d 204e 6f6e 650a  th : str = None.
+00000460: 2020 2020 6578 706f 7274 5061 7468 203a      exportPath :
+00000470: 2073 7472 203d 204e 6f6e 650a 2020 2020   str = None.    
+00000480: 7573 6544 6972 6563 746f 7279 203a 2062  useDirectory : b
+00000490: 6f6f 6c20 3d20 5472 7565 0a94 6807 5d94  ool = True..h.].
+000004a0: 6816 8c77 636c 6173 7320 6d7a 4461 7461  h..wclass mzData
+000004b0: 4d61 6e61 6765 7228 4261 7365 4d6f 6465  Manager(BaseMode
+000004c0: 6c29 3a0a 2020 2020 6d7a 4461 7461 5061  l):.    mzDataPa
+000004d0: 7468 203a 2073 7472 203d 204e 6f6e 650a  th : str = None.
+000004e0: 2020 2020 6578 706f 7274 5061 7468 203a      exportPath :
+000004f0: 2073 7472 203d 204e 6f6e 650a 2020 2020   str = None.    
+00000500: 7573 6544 6972 6563 746f 7279 203a 2062  useDirectory : b
+00000510: 6f6f 6c20 3d20 5472 7565 0a94 8594 8194  ool = True......
+00000520: 7d94 681b 686a 7362 6168 1f7d 9428 6821  }.h.hjsbah.}.(h!
+00000530: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00000540: 5d94 8c08 6c61 6e67 7561 6765 948c 0670  ]...language...p
+00000550: 7974 686f 6e94 8c09 786d 6c3a 7370 6163  ython...xml:spac
+00000560: 6594 8c08 7072 6573 6572 7665 9475 682b  e...preserve.uh+
+00000570: 6868 681d 682c 681e 4b07 681b 6857 681c  hhh.h,h.K.h.hWh.
+00000580: 6803 7562 6568 1f7d 9428 6821 5d94 8c0a  h.ubeh.}.(h!]...
+00000590: 6465 6669 6e69 7469 6f6e 9461 6823 5d94  definition.ah#].
+000005a0: 6825 5d94 6827 5d94 8c0a 6465 6669 6e69  h%].h']...defini
+000005b0: 7469 6f6e 9461 6829 5d94 7568 2b68 0a68  tion.ah)].uh+h.h
+000005c0: 1e4b 0668 1d68 2c68 1b68 0c68 1c68 0368  .K.h.h,h.h.h.h.h
+000005d0: 564b 0175 6268 0b29 8194 7d94 2868 0568  VK.ubh.)..}.(h.h
+000005e0: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
+000005f0: 8c0a 486f 7720 746f 2075 7365 9468 075d  ..How to use.h.]
+00000600: 9468 168c 0a48 6f77 2074 6f20 7573 6594  .h...How to use.
+00000610: 8594 8194 7d94 2868 1b68 8768 1c68 0368  ....}.(h.h.h.h.h
+00000620: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00000630: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00000640: 9475 682b 680f 681e 4b0e 681d 682c 681b  .uh+h.h.K.h.h,h.
+00000650: 6884 681c 6803 7562 680b 2981 947d 9428  h.h.h.ubh.)..}.(
+00000660: 6805 6806 6807 5d94 2868 1029 8194 7d94  h.h.h.].(h.)..}.
+00000670: 2868 058c 0957 6974 6820 7061 7468 9468  (h...With path.h
+00000680: 075d 9468 168c 0957 6974 6820 7061 7468  .].h...With path
+00000690: 9485 9481 947d 9428 681b 6898 681c 6803  .....}.(h.h.h.h.
+000006a0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000006b0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000006c0: 5d94 7568 2b68 0f68 1e4b 0f68 1d68 2c68  ].uh+h.h.K.h.h,h
+000006d0: 1b68 9568 1c68 0375 6268 6929 8194 7d94  .h.h.h.ubhi)..}.
+000006e0: 2868 058c 5e6d 616e 6167 6572 203d 206d  (h..^manager = m
+000006f0: 7a44 6174 614d 616e 6167 6572 280a 2020  zDataManager(.  
+00000700: 2020 6d7a 4461 7461 5061 7468 203d 2022    mzDataPath = "
+00000710: 536f 6d65 2f50 6174 6822 2c0a 2020 2020  Some/Path",.    
+00000720: 6578 706f 7274 5061 7468 203d 2022 536f  exportPath = "So
+00000730: 6d65 2f45 7870 6f72 742f 5061 7468 222c  me/Export/Path",
+00000740: 0a29 0a94 6807 5d94 6816 8c5e 6d61 6e61  .)..h.].h..^mana
+00000750: 6765 7220 3d20 6d7a 4461 7461 4d61 6e61  ger = mzDataMana
+00000760: 6765 7228 0a20 2020 206d 7a44 6174 6150  ger(.    mzDataP
+00000770: 6174 6820 3d20 2253 6f6d 652f 5061 7468  ath = "Some/Path
+00000780: 222c 0a20 2020 2065 7870 6f72 7450 6174  ",.    exportPat
+00000790: 6820 3d20 2253 6f6d 652f 4578 706f 7274  h = "Some/Export
+000007a0: 2f50 6174 6822 2c0a 290a 9485 9481 947d  /Path",.)......}
+000007b0: 9468 1b68 a673 6261 681f 7d94 2868 215d  .h.h.sbah.}.(h!]
+000007c0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000007d0: 948c 086c 616e 6775 6167 6594 8c06 7079  ...language...py
+000007e0: 7468 6f6e 9468 7a68 7b75 682b 6868 681d  thon.hzh{uh+hhh.
+000007f0: 682c 681e 4b10 681b 6895 681c 6803 7562  h,h.K.h.h.h.h.ub
+00000800: 683f 2981 947d 9428 6805 8ca6 5468 6520  h?)..}.(h...The 
+00000810: 7061 7468 2079 6f75 2073 7065 6369 6679  path you specify
+00000820: 2069 6e20 7468 6f73 6520 6172 6775 6d65   in those argume
+00000830: 6e74 7320 7769 6c6c 2062 6520 7374 6f72  nts will be stor
+00000840: 6564 2069 6e20 7468 6520 636c 6173 732c  ed in the class,
+00000850: 2073 6f20 7768 656e 2079 6f75 2075 7365   so when you use
+00000860: 2074 6865 2069 6e74 6567 7261 7465 6420   the integrated 
+00000870: 6675 6e63 7469 6f6e 732c 2079 6f75 206f  functions, you o
+00000880: 6e6c 7920 6e65 6564 2074 6f20 7370 6563  nly need to spec
+00000890: 6966 7920 7468 6520 7265 6c61 7469 7665  ify the relative
+000008a0: 2070 6174 6820 746f 2074 6865 2066 696c   path to the fil
+000008b0: 652e 9468 075d 9468 168c a654 6865 2070  e..h.].h...The p
+000008c0: 6174 6820 796f 7520 7370 6563 6966 7920  ath you specify 
+000008d0: 696e 2074 686f 7365 2061 7267 756d 656e  in those argumen
+000008e0: 7473 2077 696c 6c20 6265 2073 746f 7265  ts will be store
+000008f0: 6420 696e 2074 6865 2063 6c61 7373 2c20  d in the class, 
+00000900: 736f 2077 6865 6e20 796f 7520 7573 6520  so when you use 
+00000910: 7468 6520 696e 7465 6772 6174 6564 2066  the integrated f
+00000920: 756e 6374 696f 6e73 2c20 796f 7520 6f6e  unctions, you on
+00000930: 6c79 206e 6565 6420 746f 2073 7065 6369  ly need to speci
+00000940: 6679 2074 6865 2072 656c 6174 6976 6520  fy the relative 
+00000950: 7061 7468 2074 6f20 7468 6520 6669 6c65  path to the file
+00000960: 2e94 8594 8194 7d94 2868 1b68 b668 1c68  ......}.(h.h.h.h
+00000970: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00000980: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00000990: 295d 9475 682b 683e 681e 4b16 681d 682c  )].uh+h>h.K.h.h,
+000009a0: 681b 6895 681c 6803 7562 6568 1f7d 9428  h.h.h.h.ubeh.}.(
+000009b0: 6821 5d94 8c09 7769 7468 2d70 6174 6894  h!]...with-path.
+000009c0: 6168 235d 9468 255d 948c 0977 6974 6820  ah#].h%]...with 
+000009d0: 7061 7468 9461 6827 5d94 6829 5d94 7568  path.ah'].h)].uh
+000009e0: 2b68 0a68 1e4b 0f68 1d68 2c68 1b68 8468  +h.h.K.h.h,h.h.h
+000009f0: 1c68 0375 6268 0b29 8194 7d94 2868 0568  .h.ubh.)..}.(h.h
+00000a00: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
+00000a10: 8c0c 5769 7468 6f75 7420 7061 7468 9468  ..Without path.h
+00000a20: 075d 9468 168c 0c57 6974 686f 7574 2070  .].h...Without p
+00000a30: 6174 6894 8594 8194 7d94 2868 1b68 cf68  ath.....}.(h.h.h
+00000a40: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00000a50: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00000a60: 9468 295d 9475 682b 680f 681e 4b18 681d  .h)].uh+h.h.K.h.
+00000a70: 682c 681b 68cc 681c 6803 7562 6869 2981  h,h.h.h.h.ubhi).
+00000a80: 947d 9428 6805 8c2c 6d61 6e61 6765 7220  .}.(h..,manager 
+00000a90: 3d20 6d7a 4461 7461 4d61 6e61 6765 7228  = mzDataManager(
+00000aa0: 7573 6544 6972 6563 746f 7279 3d46 616c  useDirectory=Fal
+00000ab0: 7365 290a 9468 075d 9468 168c 2c6d 616e  se)..h.].h..,man
+00000ac0: 6167 6572 203d 206d 7a44 6174 614d 616e  ager = mzDataMan
+00000ad0: 6167 6572 2875 7365 4469 7265 6374 6f72  ager(useDirector
+00000ae0: 793d 4661 6c73 6529 0a94 8594 8194 7d94  y=False)......}.
+00000af0: 681b 68dd 7362 6168 1f7d 9428 6821 5d94  h.h.sbah.}.(h!].
+00000b00: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00000b10: 8c08 6c61 6e67 7561 6765 948c 0670 7974  ..language...pyt
+00000b20: 686f 6e94 687a 687b 7568 2b68 6868 1d68  hon.hzh{uh+hhh.h
+00000b30: 2c68 1e4b 1968 1b68 cc68 1c68 0375 6268  ,h.K.h.h.h.h.ubh
+00000b40: 3f29 8194 7d94 2868 058c 8353 6574 7469  ?)..}.(h...Setti
+00000b50: 6e67 2075 7020 7468 6520 636c 6173 7320  ng up the class 
+00000b60: 7468 6973 2077 6179 2077 696c 6c20 7265  this way will re
+00000b70: 7175 6972 6520 746f 2073 7065 6369 6679  quire to specify
+00000b80: 2065 6163 6820 7469 6d65 2079 6f75 2063   each time you c
+00000b90: 616c 6c20 6120 6675 6e63 7469 6f6e 2074  all a function t
+00000ba0: 6f20 6769 7665 2074 6865 2066 756c 6c20  o give the full 
+00000bb0: 7061 7468 2061 6e64 2074 6865 2065 7870  path and the exp
+00000bc0: 6f72 7420 6469 7265 6374 6f72 792e 9468  ort directory..h
+00000bd0: 075d 9468 168c 8353 6574 7469 6e67 2075  .].h...Setting u
+00000be0: 7020 7468 6520 636c 6173 7320 7468 6973  p the class this
+00000bf0: 2077 6179 2077 696c 6c20 7265 7175 6972   way will requir
+00000c00: 6520 746f 2073 7065 6369 6679 2065 6163  e to specify eac
+00000c10: 6820 7469 6d65 2079 6f75 2063 616c 6c20  h time you call 
+00000c20: 6120 6675 6e63 7469 6f6e 2074 6f20 6769  a function to gi
+00000c30: 7665 2074 6865 2066 756c 6c20 7061 7468  ve the full path
+00000c40: 2061 6e64 2074 6865 2065 7870 6f72 7420   and the export 
+00000c50: 6469 7265 6374 6f72 792e 9485 9481 947d  directory......}
+00000c60: 9428 681b 68ed 681c 6803 681d 4e68 1e4e  .(h.h.h.h.h.Nh.N
+00000c70: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00000c80: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00000c90: 3e68 1e4b 1c68 1d68 2c68 1b68 cc68 1c68  >h.K.h.h,h.h.h.h
+00000ca0: 0375 6265 681f 7d94 2868 215d 948c 0c77  .ubeh.}.(h!]...w
+00000cb0: 6974 686f 7574 2d70 6174 6894 6168 235d  ithout-path.ah#]
+00000cc0: 9468 255d 948c 0c77 6974 686f 7574 2070  .h%]...without p
+00000cd0: 6174 6894 6168 275d 9468 295d 9475 682b  ath.ah'].h)].uh+
+00000ce0: 680a 681e 4b18 681d 682c 681b 6884 681c  h.h.K.h.h,h.h.h.
+00000cf0: 6803 7562 6568 1f7d 9428 6821 5d94 8c0a  h.ubeh.}.(h!]...
+00000d00: 686f 772d 746f 2d75 7365 9461 6823 5d94  how-to-use.ah#].
+00000d10: 6825 5d94 6827 5d94 8c0a 686f 7720 746f  h%].h']...how to
+00000d20: 2075 7365 9461 6829 5d94 7568 2b68 0a68   use.ah)].uh+h.h
+00000d30: 1e4b 0e68 1d68 2c68 1b68 0c68 1c68 0368  .K.h.h,h.h.h.h.h
+00000d40: 564b 0175 6268 0b29 8194 7d94 2868 0568  VK.ubh.)..}.(h.h
+00000d50: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
+00000d60: 8c09 4675 6e63 7469 6f6e 7394 6807 5d94  ..Functions.h.].
+00000d70: 6816 8c09 4675 6e63 7469 6f6e 7394 8594  h...Functions...
+00000d80: 8194 7d94 2868 1b6a 0e01 0000 681c 6803  ..}.(h.j....h.h.
+00000d90: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00000da0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00000db0: 5d94 7568 2b68 0f68 1e4b 1e68 1d68 2c68  ].uh+h.h.K.h.h,h
+00000dc0: 1b6a 0b01 0000 681c 6803 7562 680b 2981  .j....h.h.ubh.).
+00000dd0: 947d 9428 6805 6806 6807 5d94 2868 1029  .}.(h.h.h.].(h.)
+00000de0: 8194 7d94 2868 058c 0d6d 7a44 6174 6158  ..}.(h...mzDataX
+00000df0: 4d4c 7265 6164 9468 075d 9468 168c 0d6d  MLread.h.].h...m
+00000e00: 7a44 6174 6158 4d4c 7265 6164 9485 9481  zDataXMLread....
+00000e10: 947d 9428 681b 6a1f 0100 0068 1c68 0368  .}.(h.j....h.h.h
+00000e20: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00000e30: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00000e40: 9475 682b 680f 681e 4b20 681d 682c 681b  .uh+h.h.K h.h,h.
+00000e50: 6a1c 0100 0068 1c68 0375 6268 0b29 8194  j....h.h.ubh.)..
+00000e60: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
+00000e70: 947d 9428 6805 8c0c 5072 6573 656e 7461  .}.(h...Presenta
+00000e80: 7469 6f6e 9468 075d 9468 168c 0c50 7265  tion.h.].h...Pre
+00000e90: 7365 6e74 6174 696f 6e94 8594 8194 7d94  sentation.....}.
+00000ea0: 2868 1b6a 3001 0000 681c 6803 681d 4e68  (h.j0...h.h.h.Nh
+00000eb0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00000ec0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00000ed0: 2b68 0f68 1e4b 2268 1d68 2c68 1b6a 2d01  +h.h.K"h.h,h.j-.
+00000ee0: 0000 681c 6803 7562 683f 2981 947d 9428  ..h.h.ubh?)..}.(
+00000ef0: 6805 8cbd 5468 6973 2066 756e 6374 696f  h...This functio
+00000f00: 6e20 7265 6164 7320 6120 602e 6d7a 4461  n reads a `.mzDa
+00000f10: 7461 2e78 6d6c 6020 6669 6c65 2061 6e64  ta.xml` file and
+00000f20: 2072 6574 7572 6e73 2061 2060 6d7a 4461   returns a `mzDa
+00000f30: 7461 6020 7374 7275 6374 7572 6520 7768  ta` structure wh
+00000f40: 6963 6820 6361 6e20 6265 206d 6f64 6966  ich can be modif
+00000f50: 6965 6420 6265 666f 7265 2073 6176 696e  ied before savin
+00000f60: 6720 6974 2773 2064 6174 6120 746f 2061  g it's data to a
+00000f70: 2060 2e6d 6174 6020 6669 6c65 2028 5365   `.mat` file (Se
+00000f80: 6520 5b6d 7a44 6174 615d 286d 7a44 6174  e [mzData](mzDat
+00000f90: 612e 6d64 2920 636c 6173 7320 666f 7220  a.md) class for 
+00000fa0: 6675 7274 6865 7220 6465 7461 696c 7329  further details)
+00000fb0: 2e94 6807 5d94 2868 168c 1654 6869 7320  ..h.].(h...This 
+00000fc0: 6675 6e63 7469 6f6e 2072 6561 6473 2061  function reads a
+00000fd0: 2094 8594 8194 7d94 2868 1b6a 3e01 0000   .....}.(h.j>...
+00000fe0: 681c 6803 681d 4e68 1e4e 7562 6809 8c07  h.h.h.Nh.Nubh...
+00000ff0: 6c69 7465 7261 6c94 9394 2981 947d 9428  literal...)..}.(
+00001000: 6805 8c0b 2e6d 7a44 6174 612e 786d 6c94  h....mzData.xml.
+00001010: 6807 5d94 6816 8c0b 2e6d 7a44 6174 612e  h.].h....mzData.
+00001020: 786d 6c94 8594 8194 7d94 2868 1b6a 4801  xml.....}.(h.jH.
+00001030: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+00001040: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00001050: 6827 5d94 6829 5d94 7568 2b6a 4601 0000  h'].h)].uh+jF...
+00001060: 681e 4b23 681d 682c 681b 6a3e 0100 0068  h.K#h.h,h.j>...h
+00001070: 1c68 0375 6268 168c 1420 6669 6c65 2061  .h.ubh... file a
+00001080: 6e64 2072 6574 7572 6e73 2061 2094 8594  nd returns a ...
+00001090: 8194 7d94 2868 1b6a 3e01 0000 681c 6803  ..}.(h.j>...h.h.
+000010a0: 681d 4e68 1e4e 7562 6a47 0100 0029 8194  h.Nh.NubjG...)..
+000010b0: 7d94 2868 058c 066d 7a44 6174 6194 6807  }.(h...mzData.h.
+000010c0: 5d94 6816 8c06 6d7a 4461 7461 9485 9481  ].h...mzData....
+000010d0: 947d 9428 681b 6a5a 0100 0068 1c68 0368  .}.(h.jZ...h.h.h
+000010e0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+000010f0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00001100: 9475 682b 6a46 0100 0068 1e4b 2368 1d68  .uh+jF...h.K#h.h
+00001110: 2c68 1b6a 3e01 0000 681c 6803 7562 6816  ,h.j>...h.h.ubh.
+00001120: 8c40 2073 7472 7563 7475 7265 2077 6869  .@ structure whi
+00001130: 6368 2063 616e 2062 6520 6d6f 6469 6669  ch can be modifi
+00001140: 6564 2062 6566 6f72 6520 7361 7669 6e67  ed before saving
+00001150: 2069 74e2 8099 7320 6461 7461 2074 6f20   it...s data to 
+00001160: 6120 9485 9481 947d 9428 681b 6a3e 0100  a .....}.(h.j>..
+00001170: 0068 1c68 0368 1d4e 681e 4e75 626a 4701  .h.h.h.Nh.NubjG.
+00001180: 0000 2981 947d 9428 6805 8c04 2e6d 6174  ..)..}.(h....mat
+00001190: 9468 075d 9468 168c 042e 6d61 7494 8594  .h.].h....mat...
+000011a0: 8194 7d94 2868 1b6a 6c01 0000 681c 6803  ..}.(h.jl...h.h.
+000011b0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000011c0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000011d0: 5d94 7568 2b6a 4601 0000 681e 4b23 681d  ].uh+jF...h.K#h.
+000011e0: 682c 681b 6a3e 0100 0068 1c68 0375 6268  h,h.j>...h.h.ubh
+000011f0: 168c 0b20 6669 6c65 2028 5365 6520 9485  ... file (See ..
+00001200: 9481 947d 9428 681b 6a3e 0100 0068 1c68  ...}.(h.j>...h.h
+00001210: 0368 1d4e 681e 4e75 6268 008c 0c70 656e  .h.Nh.Nubh...pen
+00001220: 6469 6e67 5f78 7265 6694 9394 2981 947d  ding_xref...)..}
+00001230: 9428 6805 6806 6807 5d94 6809 8c06 696e  .(h.h.h.].h...in
+00001240: 6c69 6e65 9493 9429 8194 7d94 2868 058c  line...)..}.(h..
+00001250: 066d 7a44 6174 6194 6807 5d94 6816 8c06  .mzData.h.].h...
+00001260: 6d7a 4461 7461 9485 9481 947d 9428 681b  mzData.....}.(h.
+00001270: 6a85 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00001280: 6261 681f 7d94 2868 215d 9468 235d 9428  bah.}.(h!].h#].(
+00001290: 8c04 7872 6566 948c 046d 7973 7494 6568  ..xref...myst.eh
+000012a0: 255d 9468 275d 9468 295d 9475 682b 6a83  %].h'].h)].uh+j.
+000012b0: 0100 0068 1b6a 8001 0000 681c 6803 681d  ...h.j....h.h.h.
+000012c0: 682c 681e 4b00 7562 6168 1f7d 9428 6821  h,h.K.ubah.}.(h!
+000012d0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000012e0: 5d94 8c09 7265 6664 6f6d 6169 6e94 8c03  ]...refdomain...
+000012f0: 646f 6394 8c09 7265 6674 6172 6765 7494  doc...reftarget.
+00001300: 8c06 6d7a 4461 7461 948c 0b72 6566 7461  ..mzData...refta
+00001310: 7267 6574 6964 944e 8c06 7265 6664 6f63  rgetid.N..refdoc
+00001320: 948c 0d6d 7a44 6174 614d 616e 6167 6572  ...mzDataManager
+00001330: 948c 0772 6566 7479 7065 946a 9101 0000  ...reftype.j....
+00001340: 8c0b 7265 6665 7870 6c69 6369 7494 8875  ..refexplicit..u
+00001350: 682b 6a7e 0100 0068 1e4b 2368 1d68 2c68  h+j~...h.K#h.h,h
+00001360: 1b6a 3e01 0000 681c 6803 7562 6816 8c1c  .j>...h.h.ubh...
+00001370: 2063 6c61 7373 2066 6f72 2066 7572 7468   class for furth
+00001380: 6572 2064 6574 6169 6c73 292e 9485 9481  er details).....
+00001390: 947d 9428 681b 6a3e 0100 0068 1c68 0368  .}.(h.j>...h.h.h
+000013a0: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
+000013b0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000013c0: 9475 682b 683e 681e 4b23 681d 682c 681b  .uh+h>h.K#h.h,h.
+000013d0: 6a2d 0100 0068 1c68 0375 6265 681f 7d94  j-...h.h.ubeh.}.
+000013e0: 2868 215d 948c 0369 6431 9461 6823 5d94  (h!]...id1.ah#].
+000013f0: 6825 5d94 6827 5d94 6854 6168 295d 9475  h%].h'].hTah)].u
+00001400: 682b 680a 681e 4b22 681d 682c 681b 6a1c  h+h.h.K"h.h,h.j.
+00001410: 0100 0068 1c68 0368 564b 0175 6268 0b29  ...h.h.hVK.ubh.)
+00001420: 8194 7d94 2868 0568 0668 075d 9428 6810  ..}.(h.h.h.].(h.
+00001430: 2981 947d 9428 6805 8c0a 4465 6669 6e69  )..}.(h...Defini
+00001440: 7469 6f6e 9468 075d 9468 168c 0a44 6566  tion.h.].h...Def
+00001450: 696e 6974 696f 6e94 8594 8194 7d94 2868  inition.....}.(h
+00001460: 1b6a b801 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00001470: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001480: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00001490: 0f68 1e4b 2568 1d68 2c68 1b6a b501 0000  .h.K%h.h,h.j....
+000014a0: 681c 6803 7562 6869 2981 947d 9428 6805  h.h.ubhi)..}.(h.
+000014b0: 8c56 6465 6620 6d7a 4461 7461 584d 4c72  .Vdef mzDataXMLr
+000014c0: 6561 6428 7365 6c66 406d 7a44 6174 614d  ead(self@mzDataM
+000014d0: 616e 6167 6572 2c20 6669 6c65 4e61 6d65  anager, fileName
+000014e0: 203a 2073 7472 2c20 6375 7374 6f6d 4469   : str, customDi
+000014f0: 7265 6374 6f72 7920 3a20 626f 6f6c 203d  rectory : bool =
+00001500: 2046 616c 7365 290a 9468 075d 9468 168c   False)..h.].h..
+00001510: 5664 6566 206d 7a44 6174 6158 4d4c 7265  Vdef mzDataXMLre
+00001520: 6164 2873 656c 6640 6d7a 4461 7461 4d61  ad(self@mzDataMa
+00001530: 6e61 6765 722c 2066 696c 654e 616d 6520  nager, fileName 
+00001540: 3a20 7374 722c 2063 7573 746f 6d44 6972  : str, customDir
+00001550: 6563 746f 7279 203a 2062 6f6f 6c20 3d20  ectory : bool = 
+00001560: 4661 6c73 6529 0a94 8594 8194 7d94 681b  False)......}.h.
+00001570: 6ac6 0100 0073 6261 681f 7d94 2868 215d  j....sbah.}.(h!]
+00001580: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00001590: 948c 086c 616e 6775 6167 6594 8c06 7079  ...language...py
+000015a0: 7468 6f6e 9468 7a68 7b75 682b 6868 681d  thon.hzh{uh+hhh.
+000015b0: 682c 681e 4b26 681b 6ab5 0100 0068 1c68  h,h.K&h.j....h.h
+000015c0: 0375 6265 681f 7d94 2868 215d 948c 0369  .ubeh.}.(h!]...i
+000015d0: 6432 9461 6823 5d94 6825 5d94 6827 5d94  d2.ah#].h%].h'].
+000015e0: 6882 6168 295d 9475 682b 680a 681e 4b25  h.ah)].uh+h.h.K%
+000015f0: 681d 682c 681b 6a1c 0100 0068 1c68 0368  h.h,h.j....h.h.h
+00001600: 564b 0175 6268 0b29 8194 7d94 2868 0568  VK.ubh.)..}.(h.h
+00001610: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
+00001620: 8c0a 486f 7720 746f 2075 7365 9468 075d  ..How to use.h.]
+00001630: 9468 168c 0a48 6f77 2074 6f20 7573 6594  .h...How to use.
+00001640: 8594 8194 7d94 2868 1b6a e001 0000 681c  ....}.(h.j....h.
+00001650: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+00001660: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00001670: 6829 5d94 7568 2b68 0f68 1e4b 2a68 1d68  h)].uh+h.h.K*h.h
+00001680: 2c68 1b6a dd01 0000 681c 6803 7562 6869  ,h.j....h.h.ubhi
+00001690: 2981 947d 9428 6805 8c9c 2320 436f 6e73  )..}.(h...# Cons
+000016a0: 6964 6572 696e 6720 7468 6174 206d 7a44  idering that mzD
+000016b0: 6174 614d 616e 6167 6572 2063 6c61 7373  ataManager class
+000016c0: 2068 6173 2062 6565 6e20 696e 7469 616c   has been intial
+000016d0: 697a 6564 2062 6566 6f72 6520 616e 6420  ized before and 
+000016e0: 7374 6f72 6564 2061 7320 6d61 6e61 6765  stored as manage
+000016f0: 7220 7661 7269 6162 6c65 0a0a 636f 6e74  r variable..cont
+00001700: 656e 7420 3d20 6d61 6e61 6765 722e 6d7a  ent = manager.mz
+00001710: 4461 7461 584d 4c72 6561 6428 0a20 2020  DataXMLread(.   
+00001720: 2066 696c 654e 616d 653d 5061 7468 3246   fileName=Path2F
+00001730: 696c 650a 290a 9468 075d 9468 168c 9c23  ile.)..h.].h...#
+00001740: 2043 6f6e 7369 6465 7269 6e67 2074 6861   Considering tha
+00001750: 7420 6d7a 4461 7461 4d61 6e61 6765 7220  t mzDataManager 
+00001760: 636c 6173 7320 6861 7320 6265 656e 2069  class has been i
+00001770: 6e74 6961 6c69 7a65 6420 6265 666f 7265  ntialized before
+00001780: 2061 6e64 2073 746f 7265 6420 6173 206d   and stored as m
+00001790: 616e 6167 6572 2076 6172 6961 626c 650a  anager variable.
+000017a0: 0a63 6f6e 7465 6e74 203d 206d 616e 6167  .content = manag
+000017b0: 6572 2e6d 7a44 6174 6158 4d4c 7265 6164  er.mzDataXMLread
+000017c0: 280a 2020 2020 6669 6c65 4e61 6d65 3d50  (.    fileName=P
+000017d0: 6174 6832 4669 6c65 0a29 0a94 8594 8194  ath2File.)......
+000017e0: 7d94 681b 6aee 0100 0073 6261 681f 7d94  }.h.j....sbah.}.
+000017f0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001800: 9468 295d 948c 086c 616e 6775 6167 6594  .h)]...language.
+00001810: 8c06 7079 7468 6f6e 9468 7a68 7b75 682b  ..python.hzh{uh+
+00001820: 6868 681d 682c 681e 4b2b 681b 6add 0100  hhh.h,h.K+h.j...
+00001830: 0068 1c68 0375 6268 3f29 8194 7d94 2868  .h.h.ubh?)..}.(h
+00001840: 058c 113c 753e 5061 7261 6d65 7465 7273  ...<u>Parameters
+00001850: 3c2f 753e 9468 075d 9428 6809 8c03 7261  </u>.h.].(h...ra
+00001860: 7794 9394 2981 947d 9428 6805 8c03 3c75  w...)..}.(h...<u
+00001870: 3e94 6807 5d94 6816 8c03 3c75 3e94 8594  >.h.].h...<u>...
+00001880: 8194 7d94 2868 1b6a 0402 0000 681c 6803  ..}.(h.j....h.h.
+00001890: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000018a0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000018b0: 5d94 8c06 666f 726d 6174 948c 0468 746d  ]...format...htm
+000018c0: 6c94 687a 687b 7568 2b6a 0202 0000 681d  l.hzh{uh+j....h.
+000018d0: 682c 681e 4b32 681b 6afe 0100 0068 1c68  h,h.K2h.j....h.h
+000018e0: 0375 6268 168c 0a50 6172 616d 6574 6572  .ubh...Parameter
+000018f0: 7394 8594 8194 7d94 2868 1b6a fe01 0000  s.....}.(h.j....
+00001900: 681c 6803 681d 4e68 1e4e 7562 6a03 0200  h.h.h.Nh.Nubj...
+00001910: 0029 8194 7d94 2868 058c 043c 2f75 3e94  .)..}.(h...</u>.
+00001920: 6807 5d94 6816 8c04 3c2f 753e 9485 9481  h.].h...</u>....
+00001930: 947d 9428 681b 6a18 0200 0068 1c68 0368  .}.(h.j....h.h.h
+00001940: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00001950: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00001960: 948c 0666 6f72 6d61 7494 6a13 0200 0068  ...format.j....h
+00001970: 7a68 7b75 682b 6a02 0200 0068 1d68 2c68  zh{uh+j....h.h,h
+00001980: 1e4b 3268 1b6a fe01 0000 681c 6803 7562  .K2h.j....h.h.ub
+00001990: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
+000019a0: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
+000019b0: 1e4b 3268 1d68 2c68 1b6a dd01 0000 681c  .K2h.h,h.j....h.
+000019c0: 6803 7562 6809 8c0b 6275 6c6c 6574 5f6c  h.ubh...bullet_l
+000019d0: 6973 7494 9394 2981 947d 9428 6805 6806  ist...)..}.(h.h.
+000019e0: 6807 5d94 2868 098c 096c 6973 745f 6974  h.].(h...list_it
+000019f0: 656d 9493 9429 8194 7d94 2868 0568 0668  em...)..}.(h.h.h
+00001a00: 075d 9428 683f 2981 947d 9428 6805 8c32  .].(h?)..}.(h..2
+00001a10: 4966 2064 6972 6563 746f 7269 6573 2077  If directories w
+00001a20: 6572 6520 7072 6f76 6964 6564 2069 6e20  ere provided in 
+00001a30: 7468 6520 696e 6974 2070 726f 6365 7373  the init process
+00001a40: 203a 9468 075d 9468 168c 3249 6620 6469   :.h.].h..2If di
+00001a50: 7265 6374 6f72 6965 7320 7765 7265 2070  rectories were p
+00001a60: 726f 7669 6465 6420 696e 2074 6865 2069  rovided in the i
+00001a70: 6e69 7420 7072 6f63 6573 7320 3a94 8594  nit process :...
+00001a80: 8194 7d94 2868 1b6a 3702 0000 681c 6803  ..}.(h.j7...h.h.
+00001a90: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00001aa0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00001ab0: 5d94 7568 2b68 3e68 1e4b 3368 1d68 2c68  ].uh+h>h.K3h.h,h
+00001ac0: 1b6a 3402 0000 681c 6803 7562 6a2e 0200  .j4...h.h.ubj...
+00001ad0: 0029 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+00001ae0: 6a33 0200 0029 8194 7d94 2868 0568 0668  j3...)..}.(h.h.h
+00001af0: 075d 9468 3f29 8194 7d94 2868 058c 3b60  .].h?)..}.(h..;`
+00001b00: 6669 6c65 4e61 6d65 6020 3a20 5265 6c61  fileName` : Rela
+00001b10: 7469 7665 2070 6174 6820 6f66 2074 6865  tive path of the
+00001b20: 2060 6d7a 4461 7461 2e78 6d6c 6020 6669   `mzData.xml` fi
+00001b30: 6c65 2074 6f20 7265 6164 9468 075d 9428  le to read.h.].(
+00001b40: 6a47 0100 0029 8194 7d94 2868 058c 0866  jG...)..}.(h...f
+00001b50: 696c 654e 616d 6594 6807 5d94 6816 8c08  ileName.h.].h...
+00001b60: 6669 6c65 4e61 6d65 9485 9481 947d 9428  fileName.....}.(
+00001b70: 681b 6a4f 0200 0068 1c68 0368 1d4e 681e  h.jO...h.h.h.Nh.
+00001b80: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00001b90: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00001ba0: 6a46 0100 0068 1e4b 3468 1d68 2c68 1b6a  jF...h.K4h.h,h.j
+00001bb0: 4b02 0000 681c 6803 7562 6816 8c18 203a  K...h.h.ubh... :
+00001bc0: 2052 656c 6174 6976 6520 7061 7468 206f   Relative path o
+00001bd0: 6620 7468 6520 9485 9481 947d 9428 681b  f the .....}.(h.
+00001be0: 6a4b 0200 0068 1c68 0368 1d4e 681e 4e75  jK...h.h.h.Nh.Nu
+00001bf0: 626a 4701 0000 2981 947d 9428 6805 8c0a  bjG...)..}.(h...
+00001c00: 6d7a 4461 7461 2e78 6d6c 9468 075d 9468  mzData.xml.h.].h
+00001c10: 168c 0a6d 7a44 6174 612e 786d 6c94 8594  ...mzData.xml...
+00001c20: 8194 7d94 2868 1b6a 6102 0000 681c 6803  ..}.(h.ja...h.h.
+00001c30: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00001c40: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00001c50: 5d94 7568 2b6a 4601 0000 681e 4b34 681d  ].uh+jF...h.K4h.
+00001c60: 682c 681b 6a4b 0200 0068 1c68 0375 6268  h,h.jK...h.h.ubh
+00001c70: 168c 0d20 6669 6c65 2074 6f20 7265 6164  ... file to read
+00001c80: 9485 9481 947d 9428 681b 6a4b 0200 0068  .....}.(h.jK...h
+00001c90: 1c68 0368 1d4e 681e 4e75 6265 681f 7d94  .h.h.Nh.Nubeh.}.
+00001ca0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001cb0: 9468 295d 9475 682b 683e 681e 4b34 681d  .h)].uh+h>h.K4h.
+00001cc0: 682c 681b 6a48 0200 0068 1c68 0375 6261  h,h.jH...h.h.uba
+00001cd0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00001ce0: 9468 275d 9468 295d 9475 682b 6a32 0200  .h'].h)].uh+j2..
+00001cf0: 0068 1e4b 3468 1d68 2c68 1b6a 4502 0000  .h.K4h.h,h.jE...
+00001d00: 681c 6803 7562 6a33 0200 0029 8194 7d94  h.h.ubj3...)..}.
+00001d10: 2868 0568 0668 075d 9468 3f29 8194 7d94  (h.h.h.].h?)..}.
+00001d20: 2868 058c 8a60 6375 7374 6f6d 4469 7265  (h...`customDire
+00001d30: 6374 6f72 7960 203a 2053 6574 2074 6869  ctory` : Set thi
+00001d40: 7320 7061 7261 6d65 7465 7220 746f 2060  s parameter to `
+00001d50: 5472 7565 6020 6966 2079 6f75 2070 726f  True` if you pro
+00001d60: 7669 6465 2061 2066 756c 6c20 7061 7468  vide a full path
+00001d70: 2077 6869 6368 2069 7320 6469 6666 6572   which is differ
+00001d80: 656e 7420 7468 616e 2074 6865 206f 6e65  ent than the one
+00001d90: 2073 7065 6369 6669 6564 2069 6e20 7468   specified in th
+00001da0: 6520 696e 6974 2070 726f 6365 7373 2e94  e init process..
+00001db0: 6807 5d94 286a 4701 0000 2981 947d 9428  h.].(jG...)..}.(
+00001dc0: 6805 8c0f 6375 7374 6f6d 4469 7265 6374  h...customDirect
+00001dd0: 6f72 7994 6807 5d94 6816 8c0f 6375 7374  ory.h.].h...cust
+00001de0: 6f6d 4469 7265 6374 6f72 7994 8594 8194  omDirectory.....
+00001df0: 7d94 2868 1b6a 8602 0000 681c 6803 681d  }.(h.j....h.h.h.
+00001e00: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00001e10: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00001e20: 7568 2b6a 4601 0000 681e 4b35 681d 682c  uh+jF...h.K5h.h,
+00001e30: 681b 6a82 0200 0068 1c68 0375 6268 168c  h.j....h.h.ubh..
+00001e40: 1920 3a20 5365 7420 7468 6973 2070 6172  . : Set this par
+00001e50: 616d 6574 6572 2074 6f20 9485 9481 947d  ameter to .....}
+00001e60: 9428 681b 6a82 0200 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00001e70: 681e 4e75 626a 4701 0000 2981 947d 9428  h.NubjG...)..}.(
+00001e80: 6805 8c04 5472 7565 9468 075d 9468 168c  h...True.h.].h..
+00001e90: 0454 7275 6594 8594 8194 7d94 2868 1b6a  .True.....}.(h.j
+00001ea0: 9802 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00001eb0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00001ec0: 5d94 6827 5d94 6829 5d94 7568 2b6a 4601  ].h'].h)].uh+jF.
+00001ed0: 0000 681e 4b35 681d 682c 681b 6a82 0200  ..h.K5h.h,h.j...
+00001ee0: 0068 1c68 0375 6268 168c 5a20 6966 2079  .h.h.ubh..Z if y
+00001ef0: 6f75 2070 726f 7669 6465 2061 2066 756c  ou provide a ful
+00001f00: 6c20 7061 7468 2077 6869 6368 2069 7320  l path which is 
+00001f10: 6469 6666 6572 656e 7420 7468 616e 2074  different than t
+00001f20: 6865 206f 6e65 2073 7065 6369 6669 6564  he one specified
+00001f30: 2069 6e20 7468 6520 696e 6974 2070 726f   in the init pro
+00001f40: 6365 7373 2e94 8594 8194 7d94 2868 1b6a  cess......}.(h.j
+00001f50: 8202 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00001f60: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
+00001f70: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
+00001f80: 1e4b 3568 1d68 2c68 1b6a 7f02 0000 681c  .K5h.h,h.j....h.
+00001f90: 6803 7562 6168 1f7d 9428 6821 5d94 6823  h.ubah.}.(h!].h#
+00001fa0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00001fb0: 2b6a 3202 0000 681e 4b35 681d 682c 681b  +j2...h.K5h.h,h.
+00001fc0: 6a45 0200 0068 1c68 0375 6265 681f 7d94  jE...h.h.ubeh.}.
+00001fd0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001fe0: 9468 295d 948c 0662 756c 6c65 7494 8c01  .h)]...bullet...
+00001ff0: 2d94 7568 2b6a 2d02 0000 681e 4b34 681d  -.uh+j-...h.K4h.
+00002000: 682c 681b 6a34 0200 0068 1c68 0375 6265  h,h.j4...h.h.ube
+00002010: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00002020: 9468 275d 9468 295d 9475 682b 6a32 0200  .h'].h)].uh+j2..
+00002030: 0068 1e4b 3368 1d68 2c68 1b6a 2f02 0000  .h.K3h.h,h.j/...
+00002040: 681c 6803 7562 6a33 0200 0029 8194 7d94  h.h.ubj3...)..}.
+00002050: 2868 0568 0668 075d 9428 683f 2981 947d  (h.h.h.].(h?)..}
+00002060: 9428 6805 8c0b 4f74 6865 7277 6973 6520  .(h...Otherwise 
+00002070: 3a94 6807 5d94 6816 8c0b 4f74 6865 7277  :.h.].h...Otherw
+00002080: 6973 6520 3a94 8594 8194 7d94 2868 1b6a  ise :.....}.(h.j
+00002090: c702 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+000020a0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000020b0: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
+000020c0: 1e4b 3668 1d68 2c68 1b6a c402 0000 681c  .K6h.h,h.j....h.
+000020d0: 6803 7562 6a2e 0200 0029 8194 7d94 2868  h.ubj....)..}.(h
+000020e0: 0568 0668 075d 9428 6a33 0200 0029 8194  .h.h.].(j3...)..
+000020f0: 7d94 2868 0568 0668 075d 9468 3f29 8194  }.(h.h.h.].h?)..
+00002100: 7d94 2868 058c 3760 6669 6c65 4e61 6d65  }.(h..7`fileName
+00002110: 6020 3a20 4675 6c6c 2070 6174 6820 746f  ` : Full path to
+00002120: 2074 6865 2060 6d7a 4461 7461 2e78 6d6c   the `mzData.xml
+00002130: 6020 6669 6c65 2074 6f20 7265 6164 9468  ` file to read.h
+00002140: 075d 9428 6a47 0100 0029 8194 7d94 2868  .].(jG...)..}.(h
+00002150: 058c 0866 696c 654e 616d 6594 6807 5d94  ...fileName.h.].
+00002160: 6816 8c08 6669 6c65 4e61 6d65 9485 9481  h...fileName....
+00002170: 947d 9428 681b 6adf 0200 0068 1c68 0368  .}.(h.j....h.h.h
+00002180: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00002190: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000021a0: 9475 682b 6a46 0100 0068 1e4b 3768 1d68  .uh+jF...h.K7h.h
+000021b0: 2c68 1b6a db02 0000 681c 6803 7562 6816  ,h.j....h.h.ubh.
+000021c0: 8c14 203a 2046 756c 6c20 7061 7468 2074  .. : Full path t
+000021d0: 6f20 7468 6520 9485 9481 947d 9428 681b  o the .....}.(h.
+000021e0: 6adb 0200 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+000021f0: 626a 4701 0000 2981 947d 9428 6805 8c0a  bjG...)..}.(h...
+00002200: 6d7a 4461 7461 2e78 6d6c 9468 075d 9468  mzData.xml.h.].h
+00002210: 168c 0a6d 7a44 6174 612e 786d 6c94 8594  ...mzData.xml...
+00002220: 8194 7d94 2868 1b6a f102 0000 681c 6803  ..}.(h.j....h.h.
+00002230: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00002240: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002250: 5d94 7568 2b6a 4601 0000 681e 4b37 681d  ].uh+jF...h.K7h.
+00002260: 682c 681b 6adb 0200 0068 1c68 0375 6268  h,h.j....h.h.ubh
+00002270: 168c 0d20 6669 6c65 2074 6f20 7265 6164  ... file to read
+00002280: 9485 9481 947d 9428 681b 6adb 0200 0068  .....}.(h.j....h
+00002290: 1c68 0368 1d4e 681e 4e75 6265 681f 7d94  .h.h.Nh.Nubeh.}.
+000022a0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000022b0: 9468 295d 9475 682b 683e 681e 4b37 681d  .h)].uh+h>h.K7h.
+000022c0: 682c 681b 6ad8 0200 0068 1c68 0375 6261  h,h.j....h.h.uba
+000022d0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000022e0: 9468 275d 9468 295d 9475 682b 6a32 0200  .h'].h)].uh+j2..
+000022f0: 0068 1e4b 3768 1d68 2c68 1b6a d502 0000  .h.K7h.h,h.j....
+00002300: 681c 6803 7562 6a33 0200 0029 8194 7d94  h.h.ubj3...)..}.
+00002310: 2868 0568 0668 075d 9468 3f29 8194 7d94  (h.h.h.].h?)..}.
+00002320: 2868 058c 2060 6375 7374 6f6d 4469 7265  (h.. `customDire
+00002330: 6374 6f72 7960 203a 2044 6f65 7320 6e6f  ctory` : Does no
+00002340: 7468 696e 6794 6807 5d94 286a 4701 0000  thing.h.].(jG...
+00002350: 2981 947d 9428 6805 8c0f 6375 7374 6f6d  )..}.(h...custom
+00002360: 4469 7265 6374 6f72 7994 6807 5d94 6816  Directory.h.].h.
+00002370: 8c0f 6375 7374 6f6d 4469 7265 6374 6f72  ..customDirector
+00002380: 7994 8594 8194 7d94 2868 1b6a 1603 0000  y.....}.(h.j....
+00002390: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+000023a0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+000023b0: 5d94 6829 5d94 7568 2b6a 4601 0000 681e  ].h)].uh+jF...h.
+000023c0: 4b38 681d 682c 681b 6a12 0300 0068 1c68  K8h.h,h.j....h.h
+000023d0: 0375 6268 168c 0f20 3a20 446f 6573 206e  .ubh... : Does n
+000023e0: 6f74 6869 6e67 9485 9481 947d 9428 681b  othing.....}.(h.
+000023f0: 6a12 0300 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00002400: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00002410: 255d 9468 275d 9468 295d 9475 682b 683e  %].h'].h)].uh+h>
+00002420: 681e 4b38 681d 682c 681b 6a0f 0300 0068  h.K8h.h,h.j....h
+00002430: 1c68 0375 6261 681f 7d94 2868 215d 9468  .h.ubah.}.(h!].h
+00002440: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00002450: 682b 6a32 0200 0068 1e4b 3868 1d68 2c68  h+j2...h.K8h.h,h
+00002460: 1b6a d502 0000 681c 6803 7562 6568 1f7d  .j....h.h.ubeh.}
+00002470: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00002480: 5d94 6829 5d94 6abc 0200 006a bd02 0000  ].h)].j....j....
+00002490: 7568 2b6a 2d02 0000 681e 4b37 681d 682c  uh+j-...h.K7h.h,
+000024a0: 681b 6ac4 0200 0068 1c68 0375 6265 681f  h.j....h.h.ubeh.
+000024b0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+000024c0: 275d 9468 295d 9475 682b 6a32 0200 0068  '].h)].uh+j2...h
+000024d0: 1e4b 3668 1d68 2c68 1b6a 2f02 0000 681c  .K6h.h,h.j/...h.
+000024e0: 6803 7562 6568 1f7d 9428 6821 5d94 6823  h.ubeh.}.(h!].h#
+000024f0: 5d94 6825 5d94 6827 5d94 6829 5d94 6abc  ].h%].h'].h)].j.
+00002500: 0200 006a bd02 0000 7568 2b6a 2d02 0000  ...j....uh+j-...
+00002510: 681e 4b33 681d 682c 681b 6add 0100 0068  h.K3h.h,h.j....h
+00002520: 1c68 0375 6268 3f29 8194 7d94 2868 058c  .h.ubh?)..}.(h..
+00002530: 0e3c 753e 4f75 7470 7574 733c 2f75 3e94  .<u>Outputs</u>.
+00002540: 6807 5d94 286a 0302 0000 2981 947d 9428  h.].(j....)..}.(
+00002550: 6805 8c03 3c75 3e94 6807 5d94 6816 8c03  h...<u>.h.].h...
+00002560: 3c75 3e94 8594 8194 7d94 2868 1b6a 4a03  <u>.....}.(h.jJ.
+00002570: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+00002580: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00002590: 6827 5d94 6829 5d94 8c06 666f 726d 6174  h'].h)]...format
+000025a0: 946a 1302 0000 687a 687b 7568 2b6a 0202  .j....hzh{uh+j..
+000025b0: 0000 681d 682c 681e 4b3a 681b 6a46 0300  ..h.h,h.K:h.jF..
+000025c0: 0068 1c68 0375 6268 168c 074f 7574 7075  .h.h.ubh...Outpu
+000025d0: 7473 9485 9481 947d 9428 681b 6a46 0300  ts.....}.(h.jF..
+000025e0: 0068 1c68 0368 1d4e 681e 4e75 626a 0302  .h.h.h.Nh.Nubj..
+000025f0: 0000 2981 947d 9428 6805 8c04 3c2f 753e  ..)..}.(h...</u>
+00002600: 9468 075d 9468 168c 043c 2f75 3e94 8594  .h.].h...</u>...
+00002610: 8194 7d94 2868 1b6a 5d03 0000 681c 6803  ..}.(h.j]...h.h.
+00002620: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00002630: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002640: 5d94 8c06 666f 726d 6174 946a 1302 0000  ]...format.j....
+00002650: 687a 687b 7568 2b6a 0202 0000 681d 682c  hzh{uh+j....h.h,
+00002660: 681e 4b3a 681b 6a46 0300 0068 1c68 0375  h.K:h.jF...h.h.u
+00002670: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00002680: 255d 9468 275d 9468 295d 9475 682b 683e  %].h'].h)].uh+h>
+00002690: 681e 4b3a 681d 682c 681b 6add 0100 0068  h.K:h.h,h.j....h
+000026a0: 1c68 0375 626a 2e02 0000 2981 947d 9428  .h.ubj....)..}.(
+000026b0: 6805 6806 6807 5d94 6a33 0200 0029 8194  h.h.h.].j3...)..
+000026c0: 7d94 2868 0568 0668 075d 9468 3f29 8194  }.(h.h.h.].h?)..
+000026d0: 7d94 2868 058c 434f 7574 7075 7473 2061  }.(h..COutputs a
+000026e0: 2060 6d7a 4461 7461 6020 636c 6173 7320   `mzData` class 
+000026f0: 636f 6e74 6169 6e69 6e67 2074 6865 2063  containing the c
+00002700: 6f6e 7465 6e74 206f 6620 7468 6520 6669  ontent of the fi
+00002710: 6c65 2070 6172 7365 642e 9468 075d 9428  le parsed..h.].(
+00002720: 6816 8c0a 4f75 7470 7574 7320 6120 9485  h...Outputs a ..
+00002730: 9481 947d 9428 681b 6a78 0300 0068 1c68  ...}.(h.jx...h.h
+00002740: 0368 1d4e 681e 4e75 626a 4701 0000 2981  .h.Nh.NubjG...).
+00002750: 947d 9428 6805 8c06 6d7a 4461 7461 9468  .}.(h...mzData.h
+00002760: 075d 9468 168c 066d 7a44 6174 6194 8594  .].h...mzData...
+00002770: 8194 7d94 2868 1b6a 8003 0000 681c 6803  ..}.(h.j....h.h.
+00002780: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00002790: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000027a0: 5d94 7568 2b6a 4601 0000 681e 4b3b 681d  ].uh+jF...h.K;h.
+000027b0: 682c 681b 6a78 0300 0068 1c68 0375 6268  h,h.jx...h.h.ubh
+000027c0: 168c 3120 636c 6173 7320 636f 6e74 6169  ..1 class contai
+000027d0: 6e69 6e67 2074 6865 2063 6f6e 7465 6e74  ning the content
+000027e0: 206f 6620 7468 6520 6669 6c65 2070 6172   of the file par
+000027f0: 7365 642e 9485 9481 947d 9428 681b 6a78  sed......}.(h.jx
+00002800: 0300 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
+00002810: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00002820: 9468 275d 9468 295d 9475 682b 683e 681e  .h'].h)].uh+h>h.
+00002830: 4b3b 681d 682c 681b 6a75 0300 0068 1c68  K;h.h,h.ju...h.h
+00002840: 0375 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
+00002850: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00002860: 6a32 0200 0068 1e4b 3b68 1d68 2c68 1b6a  j2...h.K;h.h,h.j
+00002870: 7203 0000 681c 6803 7562 6168 1f7d 9428  r...h.h.ubah.}.(
+00002880: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00002890: 6829 5d94 6abc 0200 006a bd02 0000 7568  h)].j....j....uh
+000028a0: 2b6a 2d02 0000 681e 4b3b 681d 682c 681b  +j-...h.K;h.h,h.
+000028b0: 6add 0100 0068 1c68 0375 6268 098c 0674  j....h.h.ubh...t
+000028c0: 6172 6765 7494 9394 2981 947d 9428 6805  arget...)..}.(h.
+000028d0: 8c0b 7361 7665 6d61 7466 696c 6594 6807  ..savematfile.h.
+000028e0: 5d94 681f 7d94 2868 215d 9468 235d 9468  ].h.}.(h!].h#].h
+000028f0: 255d 9468 275d 9468 295d 948c 0572 6566  %].h'].h)]...ref
+00002900: 6964 948c 0b73 6176 656d 6174 6669 6c65  id...savematfile
+00002910: 9475 682b 6aa4 0300 0068 1e4b 3d68 1d68  .uh+j....h.K=h.h
+00002920: 2c68 1b6a dd01 0000 681c 6803 7562 6568  ,h.j....h.h.ubeh
+00002930: 1f7d 9428 6821 5d94 8c03 6964 3394 6168  .}.(h!]...id3.ah
+00002940: 235d 9468 255d 9468 275d 946a 0901 0000  #].h%].h'].j....
+00002950: 6168 295d 9475 682b 680a 681e 4b2a 681d  ah)].uh+h.h.K*h.
+00002960: 682c 681b 6a1c 0100 0068 1c68 0368 564b  h,h.j....h.h.hVK
+00002970: 0175 6265 681f 7d94 2868 215d 948c 0d6d  .ubeh.}.(h!]...m
+00002980: 7a64 6174 6178 6d6c 7265 6164 9461 6823  zdataxmlread.ah#
+00002990: 5d94 6825 5d94 8c0d 6d7a 6461 7461 786d  ].h%]...mzdataxm
+000029a0: 6c72 6561 6494 6168 275d 9468 295d 9475  lread.ah'].h)].u
+000029b0: 682b 680a 681e 4b20 681d 682c 681b 6a0b  h+h.h.K h.h,h.j.
+000029c0: 0100 0068 1c68 0375 6268 0b29 8194 7d94  ...h.h.ubh.)..}.
+000029d0: 2868 0568 0668 075d 9428 6810 2981 947d  (h.h.h.].(h.)..}
+000029e0: 9428 6805 8c0b 7361 7665 4d61 7466 696c  .(h...saveMatfil
+000029f0: 6594 6807 5d94 6816 8c0b 7361 7665 4d61  e.h.].h...saveMa
+00002a00: 7466 696c 6594 8594 8194 7d94 2868 1b6a  tfile.....}.(h.j
+00002a10: c403 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00002a20: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00002a30: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
+00002a40: 1e4b 3e68 1d68 2c68 1b6a c103 0000 681c  .K>h.h,h.j....h.
+00002a50: 6803 7562 680b 2981 947d 9428 6805 6806  h.ubh.)..}.(h.h.
+00002a60: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
+00002a70: 0c50 7265 7365 6e74 6174 696f 6e94 6807  .Presentation.h.
+00002a80: 5d94 6816 8c0c 5072 6573 656e 7461 7469  ].h...Presentati
+00002a90: 6f6e 9485 9481 947d 9428 681b 6ad5 0300  on.....}.(h.j...
+00002aa0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00002ab0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00002ac0: 275d 9468 295d 9475 682b 680f 681e 4b3f  '].h)].uh+h.h.K?
+00002ad0: 681d 682c 681b 6ad2 0300 0068 1c68 0375  h.h,h.j....h.h.u
+00002ae0: 6268 3f29 8194 7d94 2868 058c 4553 6176  bh?)..}.(h..ESav
+00002af0: 6573 2061 2060 6d7a 4461 7461 6020 636c  es a `mzData` cl
+00002b00: 6173 7320 696e 746f 2061 2060 2e6d 6174  ass into a `.mat
+00002b10: 6020 6669 6c65 2077 6974 6820 616c 6c20  ` file with all 
+00002b20: 6d65 7461 6461 7461 2069 6e63 6c75 6465  metadata include
+00002b30: 642e 9468 075d 9428 6816 8c08 5361 7665  d..h.].(h...Save
+00002b40: 7320 6120 9485 9481 947d 9428 681b 6ae3  s a .....}.(h.j.
+00002b50: 0300 0068 1c68 0368 1d4e 681e 4e75 626a  ...h.h.h.Nh.Nubj
+00002b60: 4701 0000 2981 947d 9428 6805 8c06 6d7a  G...)..}.(h...mz
+00002b70: 4461 7461 9468 075d 9468 168c 066d 7a44  Data.h.].h...mzD
+00002b80: 6174 6194 8594 8194 7d94 2868 1b6a eb03  ata.....}.(h.j..
+00002b90: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+00002ba0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00002bb0: 6827 5d94 6829 5d94 7568 2b6a 4601 0000  h'].h)].uh+jF...
+00002bc0: 681e 4b40 681d 682c 681b 6ae3 0300 0068  h.K@h.h,h.j....h
+00002bd0: 1c68 0375 6268 168c 0e20 636c 6173 7320  .h.ubh... class 
+00002be0: 696e 746f 2061 2094 8594 8194 7d94 2868  into a .....}.(h
+00002bf0: 1b6a e303 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00002c00: 7562 6a47 0100 0029 8194 7d94 2868 058c  ubjG...)..}.(h..
+00002c10: 042e 6d61 7494 6807 5d94 6816 8c04 2e6d  ..mat.h.].h....m
+00002c20: 6174 9485 9481 947d 9428 681b 6afd 0300  at.....}.(h.j...
+00002c30: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00002c40: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00002c50: 275d 9468 295d 9475 682b 6a46 0100 0068  '].h)].uh+jF...h
+00002c60: 1e4b 4068 1d68 2c68 1b6a e303 0000 681c  .K@h.h,h.j....h.
+00002c70: 6803 7562 6816 8c21 2066 696c 6520 7769  h.ubh..! file wi
+00002c80: 7468 2061 6c6c 206d 6574 6164 6174 6120  th all metadata 
+00002c90: 696e 636c 7564 6564 2e94 8594 8194 7d94  included......}.
+00002ca0: 2868 1b6a e303 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00002cb0: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
+00002cc0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00002cd0: 2b68 3e68 1e4b 4068 1d68 2c68 1b6a d203  +h>h.K@h.h,h.j..
+00002ce0: 0000 681c 6803 7562 6568 1f7d 9428 6821  ..h.h.ubeh.}.(h!
+00002cf0: 5d94 8c03 6964 3594 6168 235d 9468 255d  ]...id5.ah#].h%]
+00002d00: 9468 275d 948c 0c70 7265 7365 6e74 6174  .h']...presentat
+00002d10: 696f 6e94 6168 295d 9475 682b 680a 681e  ion.ah)].uh+h.h.
+00002d20: 4b3f 681d 682c 681b 6ac1 0300 0068 1c68  K?h.h,h.j....h.h
+00002d30: 0368 564b 0175 6268 0b29 8194 7d94 2868  .hVK.ubh.)..}.(h
+00002d40: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
+00002d50: 6805 8c0a 4465 6669 6e69 7469 6f6e 9468  h...Definition.h
+00002d60: 075d 9468 168c 0a44 6566 696e 6974 696f  .].h...Definitio
+00002d70: 6e94 8594 8194 7d94 2868 1b6a 2004 0000  n.....}.(h.j ...
+00002d80: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00002d90: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00002da0: 5d94 6829 5d94 7568 2b68 0f68 1e4b 4268  ].h)].uh+h.h.KBh
+00002db0: 1d68 2c68 1b6a 1d04 0000 681c 6803 7562  .h,h.j....h.h.ub
+00002dc0: 6869 2981 947d 9428 6805 8c79 6465 6620  hi)..}.(h..ydef 
+00002dd0: 7361 7665 4d61 7466 696c 6528 7365 6c66  saveMatfile(self
+00002de0: 406d 7a44 6174 614d 616e 6167 6572 2c20  @mzDataManager, 
+00002df0: 6d7a 4461 7461 203a 206d 7a44 6174 612c  mzData : mzData,
+00002e00: 2072 656d 6f76 6520 3a20 626f 6f6c 203d   remove : bool =
+00002e10: 2046 616c 7365 2c20 6469 7232 5361 7665   False, dir2Save
+00002e20: 203a 2073 7472 203d 204e 6f6e 652c 2066   : str = None, f
+00002e30: 6f72 6365 203a 2062 6f6f 6c20 3d20 4661  orce : bool = Fa
+00002e40: 6c73 6529 0a94 6807 5d94 6816 8c79 6465  lse)..h.].h..yde
+00002e50: 6620 7361 7665 4d61 7466 696c 6528 7365  f saveMatfile(se
+00002e60: 6c66 406d 7a44 6174 614d 616e 6167 6572  lf@mzDataManager
+00002e70: 2c20 6d7a 4461 7461 203a 206d 7a44 6174  , mzData : mzDat
+00002e80: 612c 2072 656d 6f76 6520 3a20 626f 6f6c  a, remove : bool
+00002e90: 203d 2046 616c 7365 2c20 6469 7232 5361   = False, dir2Sa
+00002ea0: 7665 203a 2073 7472 203d 204e 6f6e 652c  ve : str = None,
+00002eb0: 2066 6f72 6365 203a 2062 6f6f 6c20 3d20   force : bool = 
+00002ec0: 4661 6c73 6529 0a94 8594 8194 7d94 681b  False)......}.h.
+00002ed0: 6a2e 0400 0073 6261 681f 7d94 2868 215d  j....sbah.}.(h!]
+00002ee0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00002ef0: 948c 086c 616e 6775 6167 6594 8c06 7079  ...language...py
+00002f00: 7468 6f6e 9468 7a68 7b75 682b 6868 681d  thon.hzh{uh+hhh.
+00002f10: 682c 681e 4b43 681b 6a1d 0400 0068 1c68  h,h.KCh.j....h.h
+00002f20: 0375 6265 681f 7d94 2868 215d 948c 0369  .ubeh.}.(h!]...i
+00002f30: 6436 9461 6823 5d94 6825 5d94 6827 5d94  d6.ah#].h%].h'].
+00002f40: 8c0a 6465 6669 6e69 7469 6f6e 9461 6829  ..definition.ah)
+00002f50: 5d94 7568 2b68 0a68 1e4b 4268 1d68 2c68  ].uh+h.h.KBh.h,h
+00002f60: 1b6a c103 0000 681c 6803 6856 4b01 7562  .j....h.h.hVK.ub
+00002f70: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
+00002f80: 2868 1029 8194 7d94 2868 058c 0a48 6f77  (h.)..}.(h...How
+00002f90: 2074 6f20 7573 6594 6807 5d94 6816 8c0a   to use.h.].h...
+00002fa0: 486f 7720 746f 2075 7365 9485 9481 947d  How to use.....}
+00002fb0: 9428 681b 6a49 0400 0068 1c68 0368 1d4e  .(h.jI...h.h.h.N
+00002fc0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00002fd0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00002fe0: 682b 680f 681e 4b47 681d 682c 681b 6a46  h+h.h.KGh.h,h.jF
+00002ff0: 0400 0068 1c68 0375 6268 6929 8194 7d94  ...h.h.ubhi)..}.
+00003000: 2868 058c f723 2043 6f6e 7369 6465 7269  (h...# Consideri
+00003010: 6e67 2074 6861 7420 6d7a 4461 7461 4d61  ng that mzDataMa
+00003020: 6e61 6765 7220 636c 6173 7320 6861 7320  nager class has 
+00003030: 6265 656e 2069 6e74 6961 6c69 7a65 6420  been intialized 
+00003040: 6265 666f 7265 2061 6e64 2073 746f 7265  before and store
+00003050: 6420 6173 206d 616e 6167 6572 2076 6172  d as manager var
+00003060: 6961 626c 650a 0a23 2043 6f6e 7369 6465  iable..# Conside
+00003070: 7269 6e67 2061 6c73 6f20 7468 6520 7661  ring also the va
+00003080: 7269 6162 6c65 2063 6f6e 7465 6e74 2077  riable content w
+00003090: 6869 6368 2069 7320 7468 6520 7265 7375  hich is the resu
+000030a0: 6c74 206f 6620 7468 6520 6675 6e63 7469  lt of the functi
+000030b0: 6f6e 206d 7a44 6174 6158 4d4c 7265 6164  on mzDataXMLread
+000030c0: 2070 7265 7365 6e74 6564 2061 626f 7665   presented above
+000030d0: 0a0a 6d61 6e61 6765 722e 7361 7665 4d61  ..manager.saveMa
+000030e0: 7446 696c 6528 0a20 2020 206d 7a44 6174  tFile(.    mzDat
+000030f0: 613d 636f 6e74 656e 740a 290a 9468 075d  a=content.)..h.]
+00003100: 9468 168c f723 2043 6f6e 7369 6465 7269  .h...# Consideri
+00003110: 6e67 2074 6861 7420 6d7a 4461 7461 4d61  ng that mzDataMa
+00003120: 6e61 6765 7220 636c 6173 7320 6861 7320  nager class has 
+00003130: 6265 656e 2069 6e74 6961 6c69 7a65 6420  been intialized 
+00003140: 6265 666f 7265 2061 6e64 2073 746f 7265  before and store
+00003150: 6420 6173 206d 616e 6167 6572 2076 6172  d as manager var
+00003160: 6961 626c 650a 0a23 2043 6f6e 7369 6465  iable..# Conside
+00003170: 7269 6e67 2061 6c73 6f20 7468 6520 7661  ring also the va
+00003180: 7269 6162 6c65 2063 6f6e 7465 6e74 2077  riable content w
+00003190: 6869 6368 2069 7320 7468 6520 7265 7375  hich is the resu
+000031a0: 6c74 206f 6620 7468 6520 6675 6e63 7469  lt of the functi
+000031b0: 6f6e 206d 7a44 6174 6158 4d4c 7265 6164  on mzDataXMLread
+000031c0: 2070 7265 7365 6e74 6564 2061 626f 7665   presented above
+000031d0: 0a0a 6d61 6e61 6765 722e 7361 7665 4d61  ..manager.saveMa
+000031e0: 7446 696c 6528 0a20 2020 206d 7a44 6174  tFile(.    mzDat
+000031f0: 613d 636f 6e74 656e 740a 290a 9485 9481  a=content.).....
+00003200: 947d 9468 1b6a 5704 0000 7362 6168 1f7d  .}.h.jW...sbah.}
+00003210: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00003220: 5d94 6829 5d94 8c08 6c61 6e67 7561 6765  ].h)]...language
+00003230: 948c 0670 7974 686f 6e94 687a 687b 7568  ...python.hzh{uh
+00003240: 2b68 6868 1d68 2c68 1e4b 4868 1b6a 4604  +hhh.h,h.KHh.jF.
+00003250: 0000 681c 6803 7562 683f 2981 947d 9428  ..h.h.ubh?)..}.(
+00003260: 6805 8c11 3c75 3e50 6172 616d 6574 6572  h...<u>Parameter
+00003270: 733c 2f75 3e94 6807 5d94 286a 0302 0000  s</u>.h.].(j....
+00003280: 2981 947d 9428 6805 8c03 3c75 3e94 6807  )..}.(h...<u>.h.
+00003290: 5d94 6816 8c03 3c75 3e94 8594 8194 7d94  ].h...<u>.....}.
+000032a0: 2868 1b6a 6b04 0000 681c 6803 681d 4e68  (h.jk...h.h.h.Nh
+000032b0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+000032c0: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
+000032d0: 666f 726d 6174 946a 1302 0000 687a 687b  format.j....hzh{
+000032e0: 7568 2b6a 0202 0000 681d 682c 681e 4b51  uh+j....h.h,h.KQ
+000032f0: 681b 6a67 0400 0068 1c68 0375 6268 168c  h.jg...h.h.ubh..
+00003300: 0a50 6172 616d 6574 6572 7394 8594 8194  .Parameters.....
+00003310: 7d94 2868 1b6a 6704 0000 681c 6803 681d  }.(h.jg...h.h.h.
+00003320: 4e68 1e4e 7562 6a03 0200 0029 8194 7d94  Nh.Nubj....)..}.
+00003330: 2868 058c 043c 2f75 3e94 6807 5d94 6816  (h...</u>.h.].h.
+00003340: 8c04 3c2f 753e 9485 9481 947d 9428 681b  ..</u>.....}.(h.
+00003350: 6a7e 0400 0068 1c68 0368 1d4e 681e 4e75  j~...h.h.h.Nh.Nu
+00003360: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00003370: 255d 9468 275d 9468 295d 948c 0666 6f72  %].h'].h)]...for
+00003380: 6d61 7494 6a13 0200 0068 7a68 7b75 682b  mat.j....hzh{uh+
+00003390: 6a02 0200 0068 1d68 2c68 1e4b 5168 1b6a  j....h.h,h.KQh.j
+000033a0: 6704 0000 681c 6803 7562 6568 1f7d 9428  g...h.h.ubeh.}.(
+000033b0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000033c0: 6829 5d94 7568 2b68 3e68 1e4b 5168 1d68  h)].uh+h>h.KQh.h
+000033d0: 2c68 1b6a 4604 0000 681c 6803 7562 6a2e  ,h.jF...h.h.ubj.
+000033e0: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+000033f0: 9428 6a33 0200 0029 8194 7d94 2868 0568  .(j3...)..}.(h.h
+00003400: 0668 075d 9468 3f29 8194 7d94 2868 058c  .h.].h?)..}.(h..
+00003410: 7460 6d7a 4461 7461 6020 3a20 5468 6520  t`mzData` : The 
+00003420: 606d 7a44 6174 6160 2073 7472 7563 7475  `mzData` structu
+00003430: 7265 2074 6f20 7361 7665 2061 7320 6120  re to save as a 
+00003440: 602e 6d61 7460 2066 696c 652e 2028 5365  `.mat` file. (Se
+00003450: 6520 5b68 6572 655d 286d 6174 5374 7275  e [here](matStru
+00003460: 6374 2e6d 6429 2066 6f72 2074 6865 2060  ct.md) for the `
+00003470: 2e6d 6174 6020 6669 6c65 2073 7472 7563  .mat` file struc
+00003480: 7475 7265 2994 6807 5d94 286a 4701 0000  ture).h.].(jG...
+00003490: 2981 947d 9428 6805 8c06 6d7a 4461 7461  )..}.(h...mzData
+000034a0: 9468 075d 9468 168c 066d 7a44 6174 6194  .h.].h...mzData.
+000034b0: 8594 8194 7d94 2868 1b6a 9d04 0000 681c  ....}.(h.j....h.
+000034c0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+000034d0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000034e0: 6829 5d94 7568 2b6a 4601 0000 681e 4b52  h)].uh+jF...h.KR
+000034f0: 681d 682c 681b 6a99 0400 0068 1c68 0375  h.h,h.j....h.h.u
+00003500: 6268 168c 0720 3a20 5468 6520 9485 9481  bh... : The ....
+00003510: 947d 9428 681b 6a99 0400 0068 1c68 0368  .}.(h.j....h.h.h
+00003520: 1d4e 681e 4e75 626a 4701 0000 2981 947d  .Nh.NubjG...)..}
+00003530: 9428 6805 8c06 6d7a 4461 7461 9468 075d  .(h...mzData.h.]
+00003540: 9468 168c 066d 7a44 6174 6194 8594 8194  .h...mzData.....
+00003550: 7d94 2868 1b6a af04 0000 681c 6803 681d  }.(h.j....h.h.h.
+00003560: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00003570: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00003580: 7568 2b6a 4601 0000 681e 4b52 681d 682c  uh+jF...h.KRh.h,
+00003590: 681b 6a99 0400 0068 1c68 0375 6268 168c  h.j....h.h.ubh..
+000035a0: 1820 7374 7275 6374 7572 6520 746f 2073  . structure to s
+000035b0: 6176 6520 6173 2061 2094 8594 8194 7d94  ave as a .....}.
+000035c0: 2868 1b6a 9904 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+000035d0: 1e4e 7562 6a47 0100 0029 8194 7d94 2868  .NubjG...)..}.(h
+000035e0: 058c 042e 6d61 7494 6807 5d94 6816 8c04  ....mat.h.].h...
+000035f0: 2e6d 6174 9485 9481 947d 9428 681b 6ac1  .mat.....}.(h.j.
+00003600: 0400 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00003610: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00003620: 9468 275d 9468 295d 9475 682b 6a46 0100  .h'].h)].uh+jF..
+00003630: 0068 1e4b 5268 1d68 2c68 1b6a 9904 0000  .h.KRh.h,h.j....
+00003640: 681c 6803 7562 6816 8c0c 2066 696c 652e  h.h.ubh... file.
+00003650: 2028 5365 6520 9485 9481 947d 9428 681b   (See .....}.(h.
+00003660: 6a99 0400 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00003670: 626a 7f01 0000 2981 947d 9428 6805 6806  bj....)..}.(h.h.
+00003680: 6807 5d94 6a84 0100 0029 8194 7d94 2868  h.].j....)..}.(h
+00003690: 058c 0468 6572 6594 6807 5d94 6816 8c04  ...here.h.].h...
+000036a0: 6865 7265 9485 9481 947d 9428 681b 6ad6  here.....}.(h.j.
+000036b0: 0400 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+000036c0: 681f 7d94 2868 215d 9468 235d 9428 6a90  h.}.(h!].h#].(j.
+000036d0: 0100 006a 9101 0000 6568 255d 9468 275d  ...j....eh%].h']
+000036e0: 9468 295d 9475 682b 6a83 0100 0068 1b6a  .h)].uh+j....h.j
+000036f0: d304 0000 681c 6803 681d 682c 681e 4b00  ....h.h.h.h,h.K.
+00003700: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00003710: 6825 5d94 6827 5d94 6829 5d94 8c09 7265  h%].h'].h)]...re
+00003720: 6664 6f6d 6169 6e94 6a9c 0100 008c 0972  fdomain.j......r
+00003730: 6566 7461 7267 6574 948c 096d 6174 5374  eftarget...matSt
+00003740: 7275 6374 948c 0b72 6566 7461 7267 6574  ruct...reftarget
+00003750: 6964 944e 8c06 7265 6664 6f63 946a a101  id.N..refdoc.j..
+00003760: 0000 8c07 7265 6674 7970 6594 6a91 0100  ....reftype.j...
+00003770: 008c 0b72 6566 6578 706c 6963 6974 9488  ...refexplicit..
+00003780: 7568 2b6a 7e01 0000 681e 4b52 681d 682c  uh+j~...h.KRh.h,
+00003790: 681b 6a99 0400 0068 1c68 0375 6268 168c  h.j....h.h.ubh..
+000037a0: 0920 666f 7220 7468 6520 9485 9481 947d  . for the .....}
+000037b0: 9428 681b 6a99 0400 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+000037c0: 681e 4e75 626a 4701 0000 2981 947d 9428  h.NubjG...)..}.(
+000037d0: 6805 8c04 2e6d 6174 9468 075d 9468 168c  h....mat.h.].h..
+000037e0: 042e 6d61 7494 8594 8194 7d94 2868 1b6a  ..mat.....}.(h.j
+000037f0: f504 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00003800: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00003810: 5d94 6827 5d94 6829 5d94 7568 2b6a 4601  ].h'].h)].uh+jF.
+00003820: 0000 681e 4b52 681d 682c 681b 6a99 0400  ..h.KRh.h,h.j...
+00003830: 0068 1c68 0375 6268 168c 1020 6669 6c65  .h.h.ubh... file
+00003840: 2073 7472 7563 7475 7265 2994 8594 8194   structure).....
+00003850: 7d94 2868 1b6a 9904 0000 681c 6803 681d  }.(h.j....h.h.h.
+00003860: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
+00003870: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00003880: 7568 2b68 3e68 1e4b 5268 1d68 2c68 1b6a  uh+h>h.KRh.h,h.j
+00003890: 9604 0000 681c 6803 7562 6168 1f7d 9428  ....h.h.ubah.}.(
+000038a0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000038b0: 6829 5d94 7568 2b6a 3202 0000 681e 4b52  h)].uh+j2...h.KR
+000038c0: 681d 682c 681b 6a93 0400 0068 1c68 0375  h.h,h.j....h.h.u
+000038d0: 626a 3302 0000 2981 947d 9428 6805 6806  bj3...)..}.(h.h.
+000038e0: 6807 5d94 683f 2981 947d 9428 6805 8c6b  h.].h?)..}.(h..k
+000038f0: 6072 656d 6f76 6560 203a 2053 686f 756c  `remove` : Shoul
+00003900: 6420 7468 6520 6f72 6967 696e 616c 2066  d the original f
+00003910: 696c 6520 2873 6f20 7468 6520 6f72 6967  ile (so the orig
+00003920: 696e 616c 2060 2e6d 7a44 6174 612e 786d  inal `.mzData.xm
+00003930: 6c60 2066 696c 6529 2062 6520 7265 6d6f  l` file) be remo
+00003940: 7665 6420 7768 656e 2073 6176 6520 6973  ved when save is
+00003950: 2063 6f6d 706c 6574 6520 3f94 6807 5d94   complete ?.h.].
+00003960: 286a 4701 0000 2981 947d 9428 6805 8c06  (jG...)..}.(h...
+00003970: 7265 6d6f 7665 9468 075d 9468 168c 0672  remove.h.].h...r
+00003980: 656d 6f76 6594 8594 8194 7d94 2868 1b6a  emove.....}.(h.j
+00003990: 1a05 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+000039a0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000039b0: 5d94 6827 5d94 6829 5d94 7568 2b6a 4601  ].h'].h)].uh+jF.
+000039c0: 0000 681e 4b53 681d 682c 681b 6a16 0500  ..h.KSh.h,h.j...
+000039d0: 0068 1c68 0375 6268 168c 2d20 3a20 5368  .h.h.ubh..- : Sh
+000039e0: 6f75 6c64 2074 6865 206f 7269 6769 6e61  ould the origina
+000039f0: 6c20 6669 6c65 2028 736f 2074 6865 206f  l file (so the o
+00003a00: 7269 6769 6e61 6c20 9485 9481 947d 9428  riginal .....}.(
+00003a10: 681b 6a16 0500 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00003a20: 4e75 626a 4701 0000 2981 947d 9428 6805  NubjG...)..}.(h.
+00003a30: 8c0b 2e6d 7a44 6174 612e 786d 6c94 6807  ...mzData.xml.h.
+00003a40: 5d94 6816 8c0b 2e6d 7a44 6174 612e 786d  ].h....mzData.xm
+00003a50: 6c94 8594 8194 7d94 2868 1b6a 2c05 0000  l.....}.(h.j,...
+00003a60: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00003a70: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00003a80: 5d94 6829 5d94 7568 2b6a 4601 0000 681e  ].h)].uh+jF...h.
+00003a90: 4b53 681d 682c 681b 6a16 0500 0068 1c68  KSh.h,h.j....h.h
+00003aa0: 0375 6268 168c 2920 6669 6c65 2920 6265  .ubh..) file) be
+00003ab0: 2072 656d 6f76 6564 2077 6865 6e20 7361   removed when sa
+00003ac0: 7665 2069 7320 636f 6d70 6c65 7465 203f  ve is complete ?
+00003ad0: 9485 9481 947d 9428 681b 6a16 0500 0068  .....}.(h.j....h
+00003ae0: 1c68 0368 1d4e 681e 4e75 6265 681f 7d94  .h.h.Nh.Nubeh.}.
+00003af0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00003b00: 9468 295d 9475 682b 683e 681e 4b53 681d  .h)].uh+h>h.KSh.
+00003b10: 682c 681b 6a13 0500 0068 1c68 0375 6261  h,h.j....h.h.uba
+00003b20: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00003b30: 9468 275d 9468 295d 9475 682b 6a32 0200  .h'].h)].uh+j2..
+00003b40: 0068 1e4b 5368 1d68 2c68 1b6a 9304 0000  .h.KSh.h,h.j....
+00003b50: 681c 6803 7562 6a33 0200 0029 8194 7d94  h.h.ubj3...)..}.
+00003b60: 2868 0568 0668 075d 9468 3f29 8194 7d94  (h.h.h.].h?)..}.
+00003b70: 2868 058c b860 666f 7263 6560 203a 2049  (h...`force` : I
+00003b80: 6620 6120 602e 6d61 7460 2066 696c 6520  f a `.mat` file 
+00003b90: 616c 7265 6164 7920 6578 6973 7473 2077  already exists w
+00003ba0: 6974 6820 7468 6520 7361 6d65 206e 616d  ith the same nam
+00003bb0: 6520 696e 2074 6865 2065 7870 6f72 7420  e in the export 
+00003bc0: 666f 6c64 6572 2c20 7368 6f75 6c64 2069  folder, should i
+00003bd0: 7420 6265 2072 6570 6c61 6365 6420 3f20  t be replaced ? 
+00003be0: 4966 2074 6869 7320 7061 7261 6d65 7465  If this paramete
+00003bf0: 7220 6973 2073 6574 2074 6f20 6046 616c  r is set to `Fal
+00003c00: 7365 602c 2073 6176 6520 7769 6c6c 2062  se`, save will b
+00003c10: 6520 6162 6f72 7465 6420 6966 2061 2066  e aborted if a f
+00003c20: 696c 6520 6973 2066 6f75 6e64 2e94 6807  ile is found..h.
+00003c30: 5d94 286a 4701 0000 2981 947d 9428 6805  ].(jG...)..}.(h.
+00003c40: 8c05 666f 7263 6594 6807 5d94 6816 8c05  ..force.h.].h...
+00003c50: 666f 7263 6594 8594 8194 7d94 2868 1b6a  force.....}.(h.j
+00003c60: 5105 0000 681c 6803 681d 4e68 1e4e 7562  Q...h.h.h.Nh.Nub
+00003c70: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00003c80: 5d94 6827 5d94 6829 5d94 7568 2b6a 4601  ].h'].h)].uh+jF.
+00003c90: 0000 681e 4b54 681d 682c 681b 6a4d 0500  ..h.KTh.h,h.jM..
+00003ca0: 0068 1c68 0375 6268 168c 0820 3a20 4966  .h.h.ubh... : If
+00003cb0: 2061 2094 8594 8194 7d94 2868 1b6a 4d05   a .....}.(h.jM.
+00003cc0: 0000 681c 6803 681d 4e68 1e4e 7562 6a47  ..h.h.h.Nh.NubjG
+00003cd0: 0100 0029 8194 7d94 2868 058c 042e 6d61  ...)..}.(h....ma
+00003ce0: 7494 6807 5d94 6816 8c04 2e6d 6174 9485  t.h.].h....mat..
+00003cf0: 9481 947d 9428 681b 6a63 0500 0068 1c68  ...}.(h.jc...h.h
+00003d00: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00003d10: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00003d20: 295d 9475 682b 6a46 0100 0068 1e4b 5468  )].uh+jF...h.KTh
+00003d30: 1d68 2c68 1b6a 4d05 0000 681c 6803 7562  .h,h.jM...h.h.ub
+00003d40: 6816 8c72 2066 696c 6520 616c 7265 6164  h..r file alread
+00003d50: 7920 6578 6973 7473 2077 6974 6820 7468  y exists with th
+00003d60: 6520 7361 6d65 206e 616d 6520 696e 2074  e same name in t
+00003d70: 6865 2065 7870 6f72 7420 666f 6c64 6572  he export folder
+00003d80: 2c20 7368 6f75 6c64 2069 7420 6265 2072  , should it be r
+00003d90: 6570 6c61 6365 6420 3f20 4966 2074 6869  eplaced ? If thi
+00003da0: 7320 7061 7261 6d65 7465 7220 6973 2073  s parameter is s
+00003db0: 6574 2074 6f20 9485 9481 947d 9428 681b  et to .....}.(h.
+00003dc0: 6a4d 0500 0068 1c68 0368 1d4e 681e 4e75  jM...h.h.h.Nh.Nu
+00003dd0: 626a 4701 0000 2981 947d 9428 6805 8c05  bjG...)..}.(h...
+00003de0: 4661 6c73 6594 6807 5d94 6816 8c05 4661  False.h.].h...Fa
+00003df0: 6c73 6594 8594 8194 7d94 2868 1b6a 7505  lse.....}.(h.ju.
+00003e00: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+00003e10: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00003e20: 6827 5d94 6829 5d94 7568 2b6a 4601 0000  h'].h)].uh+jF...
+00003e30: 681e 4b54 681d 682c 681b 6a4d 0500 0068  h.KTh.h,h.jM...h
+00003e40: 1c68 0375 6268 168c 2a2c 2073 6176 6520  .h.ubh..*, save 
+00003e50: 7769 6c6c 2062 6520 6162 6f72 7465 6420  will be aborted 
+00003e60: 6966 2061 2066 696c 6520 6973 2066 6f75  if a file is fou
+00003e70: 6e64 2e94 8594 8194 7d94 2868 1b6a 4d05  nd......}.(h.jM.
+00003e80: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
+00003e90: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00003ea0: 6827 5d94 6829 5d94 7568 2b68 3e68 1e4b  h'].h)].uh+h>h.K
+00003eb0: 5468 1d68 2c68 1b6a 4a05 0000 681c 6803  Th.h,h.jJ...h.h.
+00003ec0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00003ed0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00003ee0: 3202 0000 681e 4b54 681d 682c 681b 6a93  2...h.KTh.h,h.j.
+00003ef0: 0400 0068 1c68 0375 626a 3302 0000 2981  ...h.h.ubj3...).
+00003f00: 947d 9428 6805 6806 6807 5d94 2868 3f29  .}.(h.h.h.].(h?)
+00003f10: 8194 7d94 2868 058c 3549 6620 6469 7265  ..}.(h..5If dire
+00003f20: 6374 6f72 6965 7320 7765 7265 206e 6f74  ctories were not
+00003f30: 2070 726f 7669 6465 6420 6475 7269 6e67   provided during
+00003f40: 2069 6e69 7420 7072 6f63 6573 733a 9468   init process:.h
+00003f50: 075d 9468 168c 3549 6620 6469 7265 6374  .].h..5If direct
+00003f60: 6f72 6965 7320 7765 7265 206e 6f74 2070  ories were not p
+00003f70: 726f 7669 6465 6420 6475 7269 6e67 2069  rovided during i
+00003f80: 6e69 7420 7072 6f63 6573 733a 9485 9481  nit process:....
+00003f90: 947d 9428 681b 6a96 0500 0068 1c68 0368  .}.(h.j....h.h.h
+00003fa0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00003fb0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00003fc0: 9475 682b 683e 681e 4b55 681d 682c 681b  .uh+h>h.KUh.h,h.
+00003fd0: 6a93 0500 0068 1c68 0375 626a 2e02 0000  j....h.h.ubj....
+00003fe0: 2981 947d 9428 6805 6806 6807 5d94 6a33  )..}.(h.h.h.].j3
+00003ff0: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+00004000: 9468 3f29 8194 7d94 2868 058c b160 6469  .h?)..}.(h...`di
+00004010: 7232 7361 7665 6020 3a20 4675 6c6c 2064  r2save` : Full d
+00004020: 6972 6563 746f 7279 2073 7065 6369 6679  irectory specify
+00004030: 696e 6720 7768 6572 6520 746f 2073 6176  ing where to sav
+00004040: 6520 7468 6520 636f 6e76 6572 7465 6420  e the converted 
+00004050: 6669 6c65 2e20 4966 2074 6869 7320 7061  file. If this pa
+00004060: 7261 6d65 7465 7220 6973 2073 6574 2077  rameter is set w
+00004070: 6869 6c65 2061 2064 6972 6563 746f 7279  hile a directory
+00004080: 2077 6173 2073 7065 6369 6669 6564 2069   was specified i
+00004090: 6e20 7468 6520 696e 6974 2070 726f 6365  n the init proce
+000040a0: 7373 2c20 7468 6973 2076 616c 7565 2069  ss, this value i
+000040b0: 7320 7072 696f 7269 7469 7a65 642e 9468  s prioritized..h
+000040c0: 075d 9428 6a47 0100 0029 8194 7d94 2868  .].(jG...)..}.(h
+000040d0: 058c 0864 6972 3273 6176 6594 6807 5d94  ...dir2save.h.].
+000040e0: 6816 8c08 6469 7232 7361 7665 9485 9481  h...dir2save....
+000040f0: 947d 9428 681b 6aae 0500 0068 1c68 0368  .}.(h.j....h.h.h
+00004100: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00004110: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00004120: 9475 682b 6a46 0100 0068 1e4b 5668 1d68  .uh+jF...h.KVh.h
+00004130: 2c68 1b6a aa05 0000 681c 6803 7562 6816  ,h.j....h.h.ubh.
+00004140: 8ca7 203a 2046 756c 6c20 6469 7265 6374  .. : Full direct
+00004150: 6f72 7920 7370 6563 6966 7969 6e67 2077  ory specifying w
+00004160: 6865 7265 2074 6f20 7361 7665 2074 6865  here to save the
+00004170: 2063 6f6e 7665 7274 6564 2066 696c 652e   converted file.
+00004180: 2049 6620 7468 6973 2070 6172 616d 6574   If this paramet
+00004190: 6572 2069 7320 7365 7420 7768 696c 6520  er is set while 
+000041a0: 6120 6469 7265 6374 6f72 7920 7761 7320  a directory was 
+000041b0: 7370 6563 6966 6965 6420 696e 2074 6865  specified in the
+000041c0: 2069 6e69 7420 7072 6f63 6573 732c 2074   init process, t
+000041d0: 6869 7320 7661 6c75 6520 6973 2070 7269  his value is pri
+000041e0: 6f72 6974 697a 6564 2e94 8594 8194 7d94  oritized......}.
+000041f0: 2868 1b6a aa05 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00004200: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
+00004210: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00004220: 2b68 3e68 1e4b 5668 1d68 2c68 1b6a a705  +h>h.KVh.h,h.j..
+00004230: 0000 681c 6803 7562 6168 1f7d 9428 6821  ..h.h.ubah.}.(h!
+00004240: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00004250: 5d94 7568 2b6a 3202 0000 681e 4b56 681d  ].uh+j2...h.KVh.
+00004260: 682c 681b 6aa4 0500 0068 1c68 0375 6261  h,h.j....h.h.uba
+00004270: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00004280: 9468 275d 9468 295d 946a bc02 0000 6abd  .h'].h)].j....j.
+00004290: 0200 0075 682b 6a2d 0200 0068 1e4b 5668  ...uh+j-...h.KVh
+000042a0: 1d68 2c68 1b6a 9305 0000 681c 6803 7562  .h,h.j....h.h.ub
+000042b0: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
+000042c0: 5d94 6827 5d94 6829 5d94 7568 2b6a 3202  ].h'].h)].uh+j2.
+000042d0: 0000 681e 4b55 681d 682c 681b 6a93 0400  ..h.KUh.h,h.j...
+000042e0: 0068 1c68 0375 6265 681f 7d94 2868 215d  .h.h.ubeh.}.(h!]
+000042f0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00004300: 946a bc02 0000 6abd 0200 0075 682b 6a2d  .j....j....uh+j-
+00004310: 0200 0068 1e4b 5268 1d68 2c68 1b6a 4604  ...h.KRh.h,h.jF.
+00004320: 0000 681c 6803 7562 683f 2981 947d 9428  ..h.h.ubh?)..}.(
+00004330: 6805 8c54 3c75 3e4f 7574 7075 7473 3c2f  h..T<u>Outputs</
+00004340: 753e 3c62 723e 0a49 6620 6675 6e63 7469  u><br>.If functi
+00004350: 6f6e 2072 616e 2063 6f72 7265 6374 6c79  on ran correctly
+00004360: 2c20 6e6f 206f 7574 7075 742c 206f 7468  , no output, oth
+00004370: 6572 7769 7365 2072 6169 7365 7320 7468  erwise raises th
+00004380: 6520 6572 726f 722e 9468 075d 9428 6a03  e error..h.].(j.
+00004390: 0200 0029 8194 7d94 2868 058c 033c 753e  ...)..}.(h...<u>
+000043a0: 9468 075d 9468 168c 033c 753e 9485 9481  .h.].h...<u>....
+000043b0: 947d 9428 681b 6ae2 0500 0068 1c68 0368  .}.(h.j....h.h.h
+000043c0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+000043d0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000043e0: 948c 0666 6f72 6d61 7494 6a13 0200 0068  ...format.j....h
+000043f0: 7a68 7b75 682b 6a02 0200 0068 1d68 2c68  zh{uh+j....h.h,h
+00004400: 1e4b 5868 1b6a de05 0000 681c 6803 7562  .KXh.j....h.h.ub
+00004410: 6816 8c07 4f75 7470 7574 7394 8594 8194  h...Outputs.....
+00004420: 7d94 2868 1b6a de05 0000 681c 6803 681d  }.(h.j....h.h.h.
+00004430: 4e68 1e4e 7562 6a03 0200 0029 8194 7d94  Nh.Nubj....)..}.
+00004440: 2868 058c 043c 2f75 3e94 6807 5d94 6816  (h...</u>.h.].h.
+00004450: 8c04 3c2f 753e 9485 9481 947d 9428 681b  ..</u>.....}.(h.
+00004460: 6af5 0500 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00004470: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00004480: 255d 9468 275d 9468 295d 948c 0666 6f72  %].h'].h)]...for
+00004490: 6d61 7494 6a13 0200 0068 7a68 7b75 682b  mat.j....hzh{uh+
+000044a0: 6a02 0200 0068 1d68 2c68 1e4b 5868 1b6a  j....h.h,h.KXh.j
+000044b0: de05 0000 681c 6803 7562 6a03 0200 0029  ....h.h.ubj....)
+000044c0: 8194 7d94 2868 058c 043c 6272 3e94 6807  ..}.(h...<br>.h.
+000044d0: 5d94 6816 8c04 3c62 723e 9485 9481 947d  ].h...<br>.....}
+000044e0: 9428 681b 6a04 0600 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+000044f0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00004500: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00004510: 0666 6f72 6d61 7494 6a13 0200 0068 7a68  .format.j....hzh
+00004520: 7b75 682b 6a02 0200 0068 1d68 2c68 1e4b  {uh+j....h.h,h.K
+00004530: 5868 1b6a de05 0000 681c 6803 7562 6816  Xh.j....h.h.ubh.
+00004540: 8c01 0a94 8594 8194 7d94 2868 1b6a de05  ........}.(h.j..
+00004550: 0000 681c 6803 681d 4e68 1e4e 7562 6816  ..h.h.h.Nh.Nubh.
+00004560: 8c41 4966 2066 756e 6374 696f 6e20 7261  .AIf function ra
+00004570: 6e20 636f 7272 6563 746c 792c 206e 6f20  n correctly, no 
+00004580: 6f75 7470 7574 2c20 6f74 6865 7277 6973  output, otherwis
+00004590: 6520 7261 6973 6573 2074 6865 2065 7272  e raises the err
+000045a0: 6f72 2e94 8594 8194 7d94 2868 1b6a de05  or......}.(h.j..
+000045b0: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
+000045c0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000045d0: 6827 5d94 6829 5d94 7568 2b68 3e68 1e4b  h'].h)].uh+h>h.K
+000045e0: 5868 1d68 2c68 1b6a 4604 0000 681c 6803  Xh.h,h.jF...h.h.
+000045f0: 7562 6568 1f7d 9428 6821 5d94 8c03 6964  ubeh.}.(h!]...id
+00004600: 3794 6168 235d 9468 255d 9468 275d 948c  7.ah#].h%].h']..
+00004610: 0a68 6f77 2074 6f20 7573 6594 6168 295d  .how to use.ah)]
+00004620: 9475 682b 680a 681e 4b47 681d 682c 681b  .uh+h.h.KGh.h,h.
+00004630: 6ac1 0300 0068 1c68 0368 564b 0175 6265  j....h.h.hVK.ube
+00004640: 681f 7d94 2868 215d 9428 6ab1 0300 008c  h.}.(h!].(j.....
+00004650: 0369 6434 9465 6823 5d94 6825 5d94 8c0b  .id4.eh#].h%]...
+00004660: 7361 7665 6d61 7466 696c 6594 6168 275d  savematfile.ah']
+00004670: 948c 0b73 6176 656d 6174 6669 6c65 9461  ...savematfile.a
+00004680: 6829 5d94 7568 2b68 0a68 1e4b 3e68 1d68  h)].uh+h.h.K>h.h
+00004690: 2c68 1b6a 0b01 0000 681c 6803 6856 4b01  ,h.j....h.h.hVK.
+000046a0: 8c19 6578 7065 6374 5f72 6566 6572 656e  ..expect_referen
+000046b0: 6365 645f 6279 5f6e 616d 6594 7d94 6a2e  ced_by_name.}.j.
+000046c0: 0600 006a a603 0000 738c 1765 7870 6563  ...j....s..expec
+000046d0: 745f 7265 6665 7265 6e63 6564 5f62 795f  t_referenced_by_
+000046e0: 6964 947d 946a b103 0000 6aa6 0300 0073  id.}.j....j....s
+000046f0: 7562 680b 2981 947d 9428 6805 6806 6807  ubh.)..}.(h.h.h.
+00004700: 5d94 2868 1029 8194 7d94 2868 058c 0b63  ].(h.)..}.(h...c
+00004710: 6f6e 7665 7274 4669 6c65 9468 075d 9468  onvertFile.h.].h
+00004720: 168c 0b63 6f6e 7665 7274 4669 6c65 9485  ...convertFile..
+00004730: 9481 947d 9428 681b 6a39 0600 0068 1c68  ...}.(h.j9...h.h
+00004740: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00004750: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00004760: 295d 9475 682b 680f 681e 4b5b 681d 682c  )].uh+h.h.K[h.h,
+00004770: 681b 6a36 0600 0068 1c68 0375 6268 0b29  h.j6...h.h.ubh.)
+00004780: 8194 7d94 2868 0568 0668 075d 9428 6810  ..}.(h.h.h.].(h.
+00004790: 2981 947d 9428 6805 8c0c 5072 6573 656e  )..}.(h...Presen
+000047a0: 7461 7469 6f6e 9468 075d 9468 168c 0c50  tation.h.].h...P
+000047b0: 7265 7365 6e74 6174 696f 6e94 8594 8194  resentation.....
+000047c0: 7d94 2868 1b6a 4a06 0000 681c 6803 681d  }.(h.jJ...h.h.h.
+000047d0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+000047e0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000047f0: 7568 2b68 0f68 1e4b 5c68 1d68 2c68 1b6a  uh+h.h.K\h.h,h.j
+00004800: 4706 0000 681c 6803 7562 683f 2981 947d  G...h.h.ubh?)..}
+00004810: 9428 6805 8c84 416c 6c20 696e 206f 6e65  .(h...All in one
+00004820: 2066 756e 6374 696f 6e2e 2052 6561 6473   function. Reads
+00004830: 2060 6d7a 4461 7461 2e78 6d6c 6020 6669   `mzData.xml` fi
+00004840: 6c65 2061 6e64 2061 7574 6f6d 6174 6963  le and automatic
+00004850: 616c 6c79 2073 6176 6573 2069 7420 696e  ally saves it in
+00004860: 746f 2074 6865 2065 7870 6f72 7420 666f  to the export fo
+00004870: 6c64 6572 2e20 4e6f 2074 7261 6e73 6974  lder. No transit
+00004880: 696f 6e20 746f 2074 6865 2060 6d7a 4461  ion to the `mzDa
+00004890: 7461 6020 636c 6173 732e 9468 075d 9428  ta` class..h.].(
+000048a0: 6816 8c1b 416c 6c20 696e 206f 6e65 2066  h...All in one f
+000048b0: 756e 6374 696f 6e2e 2052 6561 6473 2094  unction. Reads .
+000048c0: 8594 8194 7d94 2868 1b6a 5806 0000 681c  ....}.(h.jX...h.
+000048d0: 6803 681d 4e68 1e4e 7562 6a47 0100 0029  h.h.Nh.NubjG...)
+000048e0: 8194 7d94 2868 058c 0a6d 7a44 6174 612e  ..}.(h...mzData.
+000048f0: 786d 6c94 6807 5d94 6816 8c0a 6d7a 4461  xml.h.].h...mzDa
+00004900: 7461 2e78 6d6c 9485 9481 947d 9428 681b  ta.xml.....}.(h.
+00004910: 6a60 0600 0068 1c68 0368 1d4e 681e 4e75  j`...h.h.h.Nh.Nu
+00004920: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00004930: 255d 9468 275d 9468 295d 9475 682b 6a46  %].h'].h)].uh+jF
+00004940: 0100 0068 1e4b 5d68 1d68 2c68 1b6a 5806  ...h.K]h.h,h.jX.
+00004950: 0000 681c 6803 7562 6816 8c4e 2066 696c  ..h.h.ubh..N fil
+00004960: 6520 616e 6420 6175 746f 6d61 7469 6361  e and automatica
+00004970: 6c6c 7920 7361 7665 7320 6974 2069 6e74  lly saves it int
+00004980: 6f20 7468 6520 6578 706f 7274 2066 6f6c  o the export fol
+00004990: 6465 722e 204e 6f20 7472 616e 7369 7469  der. No transiti
+000049a0: 6f6e 2074 6f20 7468 6520 9485 9481 947d  on to the .....}
+000049b0: 9428 681b 6a58 0600 0068 1c68 0368 1d4e  .(h.jX...h.h.h.N
+000049c0: 681e 4e75 626a 4701 0000 2981 947d 9428  h.NubjG...)..}.(
+000049d0: 6805 8c06 6d7a 4461 7461 9468 075d 9468  h...mzData.h.].h
+000049e0: 168c 066d 7a44 6174 6194 8594 8194 7d94  ...mzData.....}.
+000049f0: 2868 1b6a 7206 0000 681c 6803 681d 4e68  (h.jr...h.h.h.Nh
+00004a00: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00004a10: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00004a20: 2b6a 4601 0000 681e 4b5d 681d 682c 681b  +jF...h.K]h.h,h.
+00004a30: 6a58 0600 0068 1c68 0375 6268 168c 0720  jX...h.h.ubh... 
+00004a40: 636c 6173 732e 9485 9481 947d 9428 681b  class......}.(h.
+00004a50: 6a58 0600 0068 1c68 0368 1d4e 681e 4e75  jX...h.h.h.Nh.Nu
+00004a60: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00004a70: 255d 9468 275d 9468 295d 9475 682b 683e  %].h'].h)].uh+h>
+00004a80: 681e 4b5d 681d 682c 681b 6a47 0600 0068  h.K]h.h,h.jG...h
+00004a90: 1c68 0375 6265 681f 7d94 2868 215d 948c  .h.ubeh.}.(h!]..
+00004aa0: 0369 6438 9461 6823 5d94 6825 5d94 6827  .id8.ah#].h%].h'
+00004ab0: 5d94 8c0c 7072 6573 656e 7461 7469 6f6e  ]...presentation
+00004ac0: 9461 6829 5d94 7568 2b68 0a68 1e4b 5c68  .ah)].uh+h.h.K\h
+00004ad0: 1d68 2c68 1b6a 3606 0000 681c 6803 6856  .h,h.j6...h.h.hV
+00004ae0: 4b01 7562 680b 2981 947d 9428 6805 6806  K.ubh.)..}.(h.h.
+00004af0: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
+00004b00: 0a44 6566 696e 6974 696f 6e94 6807 5d94  .Definition.h.].
+00004b10: 6816 8c0a 4465 6669 6e69 7469 6f6e 9485  h...Definition..
+00004b20: 9481 947d 9428 681b 6a95 0600 0068 1c68  ...}.(h.j....h.h
+00004b30: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00004b40: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00004b50: 295d 9475 682b 680f 681e 4b5f 681d 682c  )].uh+h.h.K_h.h,
+00004b60: 681b 6a92 0600 0068 1c68 0375 6268 6929  h.j....h.h.ubhi)
+00004b70: 8194 7d94 2868 058c 9864 6566 2063 6f6e  ..}.(h...def con
+00004b80: 7665 7274 4669 6c65 2873 656c 6640 6d7a  vertFile(self@mz
+00004b90: 4461 7461 4d61 6e61 6765 722c 2066 696c  DataManager, fil
+00004ba0: 654e 616d 6520 3a20 7374 722c 2063 7573  eName : str, cus
+00004bb0: 746f 6d44 6972 6563 746f 7279 203a 2062  tomDirectory : b
+00004bc0: 6f6f 6c20 3d20 4661 6c73 652c 2064 6972  ool = False, dir
+00004bd0: 3253 6176 6520 3a20 7374 7220 3d20 4e6f  2Save : str = No
+00004be0: 6e65 2c20 666f 7263 6520 3a20 626f 6f6c  ne, force : bool
+00004bf0: 203d 2046 616c 7365 2c20 7265 6d6f 7665   = False, remove
+00004c00: 203a 2062 6f6f 6c20 3d20 4661 6c73 6529   : bool = False)
+00004c10: 0a94 6807 5d94 6816 8c98 6465 6620 636f  ..h.].h...def co
+00004c20: 6e76 6572 7446 696c 6528 7365 6c66 406d  nvertFile(self@m
+00004c30: 7a44 6174 614d 616e 6167 6572 2c20 6669  zDataManager, fi
+00004c40: 6c65 4e61 6d65 203a 2073 7472 2c20 6375  leName : str, cu
+00004c50: 7374 6f6d 4469 7265 6374 6f72 7920 3a20  stomDirectory : 
+00004c60: 626f 6f6c 203d 2046 616c 7365 2c20 6469  bool = False, di
+00004c70: 7232 5361 7665 203a 2073 7472 203d 204e  r2Save : str = N
+00004c80: 6f6e 652c 2066 6f72 6365 203a 2062 6f6f  one, force : boo
+00004c90: 6c20 3d20 4661 6c73 652c 2072 656d 6f76  l = False, remov
+00004ca0: 6520 3a20 626f 6f6c 203d 2046 616c 7365  e : bool = False
+00004cb0: 290a 9485 9481 947d 9468 1b6a a306 0000  )......}.h.j....
+00004cc0: 7362 6168 1f7d 9428 6821 5d94 6823 5d94  sbah.}.(h!].h#].
+00004cd0: 6825 5d94 6827 5d94 6829 5d94 8c08 6c61  h%].h'].h)]...la
+00004ce0: 6e67 7561 6765 948c 0670 7974 686f 6e94  nguage...python.
+00004cf0: 687a 687b 7568 2b68 6868 1d68 2c68 1e4b  hzh{uh+hhh.h,h.K
+00004d00: 6068 1b6a 9206 0000 681c 6803 7562 6568  `h.j....h.h.ubeh
+00004d10: 1f7d 9428 6821 5d94 8c03 6964 3994 6168  .}.(h!]...id9.ah
+00004d20: 235d 9468 255d 9468 275d 948c 0a64 6566  #].h%].h']...def
+00004d30: 696e 6974 696f 6e94 6168 295d 9475 682b  inition.ah)].uh+
+00004d40: 680a 681e 4b5f 681d 682c 681b 6a36 0600  h.h.K_h.h,h.j6..
+00004d50: 0068 1c68 0368 564b 0175 6268 0b29 8194  .h.h.hVK.ubh.)..
+00004d60: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
+00004d70: 947d 9428 6805 8c0a 486f 7720 746f 2075  .}.(h...How to u
+00004d80: 7365 9468 075d 9468 168c 0a48 6f77 2074  se.h.].h...How t
+00004d90: 6f20 7573 6594 8594 8194 7d94 2868 1b6a  o use.....}.(h.j
+00004da0: be06 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00004db0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00004dc0: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
+00004dd0: 1e4b 6468 1d68 2c68 1b6a bb06 0000 681c  .Kdh.h,h.j....h.
+00004de0: 6803 7562 6869 2981 947d 9428 6805 8c8f  h.ubhi)..}.(h...
+00004df0: 2320 436f 6e73 6964 6572 696e 6720 7468  # Considering th
+00004e00: 6174 206d 7a44 6174 614d 616e 6167 6572  at mzDataManager
+00004e10: 2063 6c61 7373 2068 6173 2062 6565 6e20   class has been 
+00004e20: 696e 7469 616c 697a 6564 2062 6566 6f72  intialized befor
+00004e30: 6520 616e 6420 7374 6f72 6564 2061 7320  e and stored as 
+00004e40: 6d61 6e61 6765 7220 7661 7269 6162 6c65  manager variable
+00004e50: 0a0a 6d61 6e61 6765 722e 636f 6e76 6572  ..manager.conver
+00004e60: 7446 696c 6528 0a20 2020 2066 696c 654e  tFile(.    fileN
+00004e70: 616d 653d 4669 6c65 4e61 6d65 0a29 0a94  ame=FileName.)..
+00004e80: 6807 5d94 6816 8c8f 2320 436f 6e73 6964  h.].h...# Consid
+00004e90: 6572 696e 6720 7468 6174 206d 7a44 6174  ering that mzDat
+00004ea0: 614d 616e 6167 6572 2063 6c61 7373 2068  aManager class h
+00004eb0: 6173 2062 6565 6e20 696e 7469 616c 697a  as been intializ
+00004ec0: 6564 2062 6566 6f72 6520 616e 6420 7374  ed before and st
+00004ed0: 6f72 6564 2061 7320 6d61 6e61 6765 7220  ored as manager 
+00004ee0: 7661 7269 6162 6c65 0a0a 6d61 6e61 6765  variable..manage
+00004ef0: 722e 636f 6e76 6572 7446 696c 6528 0a20  r.convertFile(. 
+00004f00: 2020 2066 696c 654e 616d 653d 4669 6c65     fileName=File
+00004f10: 4e61 6d65 0a29 0a94 8594 8194 7d94 681b  Name.)......}.h.
+00004f20: 6acc 0600 0073 6261 681f 7d94 2868 215d  j....sbah.}.(h!]
+00004f30: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00004f40: 948c 086c 616e 6775 6167 6594 8c06 7079  ...language...py
+00004f50: 7468 6f6e 9468 7a68 7b75 682b 6868 681d  thon.hzh{uh+hhh.
+00004f60: 682c 681e 4b65 681b 6abb 0600 0068 1c68  h,h.Keh.j....h.h
+00004f70: 0375 6268 3f29 8194 7d94 2868 058c 113c  .ubh?)..}.(h...<
+00004f80: 753e 5061 7261 6d65 7465 7273 3c2f 753e  u>Parameters</u>
+00004f90: 9468 075d 9428 6a03 0200 0029 8194 7d94  .h.].(j....)..}.
+00004fa0: 2868 058c 033c 753e 9468 075d 9468 168c  (h...<u>.h.].h..
+00004fb0: 033c 753e 9485 9481 947d 9428 681b 6ae0  .<u>.....}.(h.j.
+00004fc0: 0600 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00004fd0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00004fe0: 9468 275d 9468 295d 948c 0666 6f72 6d61  .h'].h)]...forma
+00004ff0: 7494 6a13 0200 0068 7a68 7b75 682b 6a02  t.j....hzh{uh+j.
+00005000: 0200 0068 1d68 2c68 1e4b 6d68 1b6a dc06  ...h.h,h.Kmh.j..
+00005010: 0000 681c 6803 7562 6816 8c0a 5061 7261  ..h.h.ubh...Para
+00005020: 6d65 7465 7273 9485 9481 947d 9428 681b  meters.....}.(h.
+00005030: 6adc 0600 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00005040: 626a 0302 0000 2981 947d 9428 6805 8c04  bj....)..}.(h...
+00005050: 3c2f 753e 9468 075d 9468 168c 043c 2f75  </u>.h.].h...</u
+00005060: 3e94 8594 8194 7d94 2868 1b6a f306 0000  >.....}.(h.j....
+00005070: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00005080: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00005090: 5d94 6829 5d94 8c06 666f 726d 6174 946a  ].h)]...format.j
+000050a0: 1302 0000 687a 687b 7568 2b6a 0202 0000  ....hzh{uh+j....
+000050b0: 681d 682c 681e 4b6d 681b 6adc 0600 0068  h.h,h.Kmh.j....h
+000050c0: 1c68 0375 6265 681f 7d94 2868 215d 9468  .h.ubeh.}.(h!].h
+000050d0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+000050e0: 682b 683e 681e 4b6d 681d 682c 681b 6abb  h+h>h.Kmh.h,h.j.
+000050f0: 0600 0068 1c68 0375 626a 2e02 0000 2981  ...h.h.ubj....).
+00005100: 947d 9428 6805 6806 6807 5d94 286a 3302  .}.(h.h.h.].(j3.
+00005110: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00005120: 2868 3f29 8194 7d94 2868 058c 1060 6669  (h?)..}.(h...`fi
+00005130: 6c65 4e61 6d65 6020 3a3c 6272 3e94 6807  leName` :<br>.h.
+00005140: 5d94 286a 4701 0000 2981 947d 9428 6805  ].(jG...)..}.(h.
+00005150: 8c08 6669 6c65 4e61 6d65 9468 075d 9468  ..fileName.h.].h
+00005160: 168c 0866 696c 654e 616d 6594 8594 8194  ...fileName.....
+00005170: 7d94 2868 1b6a 1207 0000 681c 6803 681d  }.(h.j....h.h.h.
+00005180: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00005190: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000051a0: 7568 2b6a 4601 0000 681e 4b6e 681d 682c  uh+jF...h.Knh.h,
+000051b0: 681b 6a0e 0700 0068 1c68 0375 6268 168c  h.j....h.h.ubh..
+000051c0: 0220 3a94 8594 8194 7d94 2868 1b6a 0e07  . :.....}.(h.j..
+000051d0: 0000 681c 6803 681d 4e68 1e4e 7562 6a03  ..h.h.h.Nh.Nubj.
+000051e0: 0200 0029 8194 7d94 2868 058c 043c 6272  ...)..}.(h...<br
+000051f0: 3e94 6807 5d94 6816 8c04 3c62 723e 9485  >.h.].h...<br>..
+00005200: 9481 947d 9428 681b 6a24 0700 0068 1c68  ...}.(h.j$...h.h
+00005210: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00005220: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00005230: 295d 948c 0666 6f72 6d61 7494 6a13 0200  )]...format.j...
+00005240: 0068 7a68 7b75 682b 6a02 0200 0068 1d68  .hzh{uh+j....h.h
+00005250: 2c68 1e4b 6e68 1b6a 0e07 0000 681c 6803  ,h.Knh.j....h.h.
+00005260: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+00005270: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00005280: 3e68 1e4b 6e68 1d68 2c68 1b6a 0b07 0000  >h.Knh.h,h.j....
+00005290: 681c 6803 7562 6a2e 0200 0029 8194 7d94  h.h.ubj....)..}.
+000052a0: 2868 0568 0668 075d 9428 6a33 0200 0029  (h.h.h.].(j3...)
+000052b0: 8194 7d94 2868 0568 0668 075d 9468 3f29  ..}.(h.h.h.].h?)
+000052c0: 8194 7d94 2868 058c 9253 686f 756c 6420  ..}.(h...Should 
+000052d0: 6265 2074 6865 2066 756c 6c20 7061 7468  be the full path
+000052e0: 2074 6f20 7468 6520 6669 6c65 2061 6e64   to the file and
+000052f0: 2069 7427 7320 6578 7465 6e73 696f 6e20   it's extension 
+00005300: 282e 6d7a 6461 7461 2e78 6d6c 2920 746f  (.mzdata.xml) to
+00005310: 2063 6f6e 7665 7274 2069 6620 6e6f 2076   convert if no v
+00005320: 616c 7565 2077 6173 2067 6976 656e 2074  alue was given t
+00005330: 6f20 606d 7a44 6174 6150 6174 6860 2077  o `mzDataPath` w
+00005340: 6865 6e20 696e 6974 6961 6c69 7a69 6e67  hen initializing
+00005350: 2074 6865 2063 6c61 7373 2e94 6807 5d94   the class..h.].
+00005360: 2868 168c 6b53 686f 756c 6420 6265 2074  (h..kShould be t
+00005370: 6865 2066 756c 6c20 7061 7468 2074 6f20  he full path to 
+00005380: 7468 6520 6669 6c65 2061 6e64 2069 74e2  the file and it.
+00005390: 8099 7320 6578 7465 6e73 696f 6e20 282e  ..s extension (.
+000053a0: 6d7a 6461 7461 2e78 6d6c 2920 746f 2063  mzdata.xml) to c
+000053b0: 6f6e 7665 7274 2069 6620 6e6f 2076 616c  onvert if no val
+000053c0: 7565 2077 6173 2067 6976 656e 2074 6f20  ue was given to 
+000053d0: 9485 9481 947d 9428 681b 6a3f 0700 0068  .....}.(h.j?...h
+000053e0: 1c68 0368 1d4e 681e 4e75 626a 4701 0000  .h.h.Nh.NubjG...
+000053f0: 2981 947d 9428 6805 8c0a 6d7a 4461 7461  )..}.(h...mzData
+00005400: 5061 7468 9468 075d 9468 168c 0a6d 7a44  Path.h.].h...mzD
+00005410: 6174 6150 6174 6894 8594 8194 7d94 2868  ataPath.....}.(h
+00005420: 1b6a 4707 0000 681c 6803 681d 4e68 1e4e  .jG...h.h.h.Nh.N
+00005430: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00005440: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00005450: 4601 0000 681e 4b6f 681d 682c 681b 6a3f  F...h.Koh.h,h.j?
+00005460: 0700 0068 1c68 0375 6268 168c 1d20 7768  ...h.h.ubh... wh
+00005470: 656e 2069 6e69 7469 616c 697a 696e 6720  en initializing 
+00005480: 7468 6520 636c 6173 732e 9485 9481 947d  the class......}
+00005490: 9428 681b 6a3f 0700 0068 1c68 0368 1d4e  .(h.j?...h.h.h.N
+000054a0: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
+000054b0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+000054c0: 682b 683e 681e 4b6f 681d 682c 681b 6a3c  h+h>h.Koh.h,h.j<
+000054d0: 0700 0068 1c68 0375 6261 681f 7d94 2868  ...h.h.ubah.}.(h
+000054e0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000054f0: 295d 9475 682b 6a32 0200 0068 1e4b 6f68  )].uh+j2...h.Koh
+00005500: 1d68 2c68 1b6a 3907 0000 681c 6803 7562  .h,h.j9...h.h.ub
+00005510: 6a33 0200 0029 8194 7d94 2868 0568 0668  j3...)..}.(h.h.h
+00005520: 075d 9468 3f29 8194 7d94 2868 058c 454f  .].h?)..}.(h..EO
+00005530: 7468 6572 7769 7365 2c20 7468 6520 6669  therwise, the fi
+00005540: 6c65 2773 2072 656c 6174 6976 6520 7061  le's relative pa
+00005550: 7468 2077 6974 6820 6974 2773 2065 7874  th with it's ext
+00005560: 656e 7369 6f6e 2028 2e6d 7a64 6174 612e  ension (.mzdata.
+00005570: 786d 6c29 9468 075d 9468 168c 494f 7468  xml).h.].h..IOth
+00005580: 6572 7769 7365 2c20 7468 6520 6669 6c65  erwise, the file
+00005590: e280 9973 2072 656c 6174 6976 6520 7061  ...s relative pa
+000055a0: 7468 2077 6974 6820 6974 e280 9973 2065  th with it...s e
+000055b0: 7874 656e 7369 6f6e 2028 2e6d 7a64 6174  xtension (.mzdat
+000055c0: 612e 786d 6c29 9485 9481 947d 9428 681b  a.xml).....}.(h.
+000055d0: 6a68 0700 0068 1c68 0368 1d4e 681e 4e75  jh...h.h.h.Nh.Nu
+000055e0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+000055f0: 255d 9468 275d 9468 295d 9475 682b 683e  %].h'].h)].uh+h>
+00005600: 681e 4b70 681d 682c 681b 6a65 0700 0068  h.Kph.h,h.je...h
+00005610: 1c68 0375 6261 681f 7d94 2868 215d 9468  .h.ubah.}.(h!].h
+00005620: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00005630: 682b 6a32 0200 0068 1e4b 7068 1d68 2c68  h+j2...h.Kph.h,h
+00005640: 1b6a 3907 0000 681c 6803 7562 6568 1f7d  .j9...h.h.ubeh.}
+00005650: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00005660: 5d94 6829 5d94 6abc 0200 006a bd02 0000  ].h)].j....j....
+00005670: 7568 2b6a 2d02 0000 681e 4b6f 681d 682c  uh+j-...h.Koh.h,
+00005680: 681b 6a0b 0700 0068 1c68 0375 6265 681f  h.j....h.h.ubeh.
+00005690: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+000056a0: 275d 9468 295d 9475 682b 6a32 0200 0068  '].h)].uh+j2...h
+000056b0: 1e4b 6e68 1d68 2c68 1b6a 0807 0000 681c  .Knh.h,h.j....h.
+000056c0: 6803 7562 6a33 0200 0029 8194 7d94 2868  h.ubj3...)..}.(h
+000056d0: 0568 0668 075d 9468 3f29 8194 7d94 2868  .h.h.].h?)..}.(h
+000056e0: 058c 7e60 6375 7374 6f6d 4469 7265 6374  ..~`customDirect
+000056f0: 6f72 7960 203a 2053 6574 2074 6869 7320  ory` : Set this 
+00005700: 7061 7261 6d65 7465 7220 746f 2060 5472  parameter to `Tr
+00005710: 7565 6020 6966 2074 6865 2060 6669 6c65  ue` if the `file
+00005720: 4e61 6d65 6020 6973 2069 6e20 6120 6469  Name` is in a di
+00005730: 6666 6572 656e 7420 7061 7468 2074 6861  fferent path tha
+00005740: 6e20 7468 6520 6f6e 6520 6769 7665 6e20  n the one given 
+00005750: 696e 2063 6f6e 6669 6775 7261 7469 6f6e  in configuration
+00005760: 2e94 6807 5d94 286a 4701 0000 2981 947d  ..h.].(jG...)..}
+00005770: 9428 6805 8c0f 6375 7374 6f6d 4469 7265  .(h...customDire
+00005780: 6374 6f72 7994 6807 5d94 6816 8c0f 6375  ctory.h.].h...cu
+00005790: 7374 6f6d 4469 7265 6374 6f72 7994 8594  stomDirectory...
+000057a0: 8194 7d94 2868 1b6a 8f07 0000 681c 6803  ..}.(h.j....h.h.
+000057b0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000057c0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000057d0: 5d94 7568 2b6a 4601 0000 681e 4b71 681d  ].uh+jF...h.Kqh.
+000057e0: 682c 681b 6a8b 0700 0068 1c68 0375 6268  h,h.j....h.h.ubh
+000057f0: 168c 1920 3a20 5365 7420 7468 6973 2070  ... : Set this p
+00005800: 6172 616d 6574 6572 2074 6f20 9485 9481  arameter to ....
+00005810: 947d 9428 681b 6a8b 0700 0068 1c68 0368  .}.(h.j....h.h.h
+00005820: 1d4e 681e 4e75 626a 4701 0000 2981 947d  .Nh.NubjG...)..}
+00005830: 9428 6805 8c04 5472 7565 9468 075d 9468  .(h...True.h.].h
+00005840: 168c 0454 7275 6594 8594 8194 7d94 2868  ...True.....}.(h
+00005850: 1b6a a107 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00005860: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00005870: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00005880: 4601 0000 681e 4b71 681d 682c 681b 6a8b  F...h.Kqh.h,h.j.
+00005890: 0700 0068 1c68 0375 6268 168c 0820 6966  ...h.h.ubh... if
+000058a0: 2074 6865 2094 8594 8194 7d94 2868 1b6a   the .....}.(h.j
+000058b0: 8b07 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+000058c0: 6a47 0100 0029 8194 7d94 2868 058c 0866  jG...)..}.(h...f
+000058d0: 696c 654e 616d 6594 6807 5d94 6816 8c08  ileName.h.].h...
+000058e0: 6669 6c65 4e61 6d65 9485 9481 947d 9428  fileName.....}.(
+000058f0: 681b 6ab3 0700 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00005900: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00005910: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00005920: 6a46 0100 0068 1e4b 7168 1d68 2c68 1b6a  jF...h.Kqh.h,h.j
+00005930: 8b07 0000 681c 6803 7562 6816 8c3c 2069  ....h.h.ubh..< i
+00005940: 7320 696e 2061 2064 6966 6665 7265 6e74  s in a different
+00005950: 2070 6174 6820 7468 616e 2074 6865 206f   path than the o
+00005960: 6e65 2067 6976 656e 2069 6e20 636f 6e66  ne given in conf
+00005970: 6967 7572 6174 696f 6e2e 9485 9481 947d  iguration......}
+00005980: 9428 681b 6a8b 0700 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00005990: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
+000059a0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+000059b0: 682b 683e 681e 4b71 681d 682c 681b 6a88  h+h>h.Kqh.h,h.j.
+000059c0: 0700 0068 1c68 0375 6261 681f 7d94 2868  ...h.h.ubah.}.(h
+000059d0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000059e0: 295d 9475 682b 6a32 0200 0068 1e4b 7168  )].uh+j2...h.Kqh
+000059f0: 1d68 2c68 1b6a 0807 0000 681c 6803 7562  .h,h.j....h.h.ub
+00005a00: 6a33 0200 0029 8194 7d94 2868 0568 0668  j3...)..}.(h.h.h
+00005a10: 075d 9468 3f29 8194 7d94 2868 058c bc60  .].h?)..}.(h...`
+00005a20: 6469 7232 5361 7665 6020 2020 3a20 5361  dir2Save`   : Sa
+00005a30: 7665 2064 6972 6563 746f 7279 2074 6f20  ve directory to 
+00005a40: 7361 7665 2074 6865 202e 6d61 7420 6669  save the .mat fi
+00005a50: 6c65 2e20 4966 2070 6174 6820 7761 7320  le. If path was 
+00005a60: 6769 7665 6e20 696e 2063 6f6e 6669 6775  given in configu
+00005a70: 7261 7469 6f6e 2c20 6974 2069 7320 6e6f  ration, it is no
+00005a80: 7420 6e65 6564 6564 2e20 5468 6973 2070  t needed. This p
+00005a90: 6172 616d 6574 6572 2077 696c 6c20 6265  arameter will be
+00005aa0: 2070 7269 6f72 6974 6973 6564 206f 7665   prioritised ove
+00005ab0: 7220 7468 6520 7061 7468 2067 6976 656e  r the path given
+00005ac0: 2069 6e20 636f 6e66 6967 7572 6174 696f   in configuratio
+00005ad0: 6e20 2869 6620 616e 7929 2e94 6807 5d94  n (if any)..h.].
+00005ae0: 286a 4701 0000 2981 947d 9428 6805 8c08  (jG...)..}.(h...
+00005af0: 6469 7232 5361 7665 9468 075d 9468 168c  dir2Save.h.].h..
+00005b00: 0864 6972 3253 6176 6594 8594 8194 7d94  .dir2Save.....}.
+00005b10: 2868 1b6a d807 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00005b20: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00005b30: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00005b40: 2b6a 4601 0000 681e 4b72 681d 682c 681b  +jF...h.Krh.h,h.
+00005b50: 6ad4 0700 0068 1c68 0375 6268 168c b220  j....h.h.ubh... 
+00005b60: 2020 3a20 5361 7665 2064 6972 6563 746f    : Save directo
+00005b70: 7279 2074 6f20 7361 7665 2074 6865 202e  ry to save the .
+00005b80: 6d61 7420 6669 6c65 2e20 4966 2070 6174  mat file. If pat
+00005b90: 6820 7761 7320 6769 7665 6e20 696e 2063  h was given in c
+00005ba0: 6f6e 6669 6775 7261 7469 6f6e 2c20 6974  onfiguration, it
+00005bb0: 2069 7320 6e6f 7420 6e65 6564 6564 2e20   is not needed. 
+00005bc0: 5468 6973 2070 6172 616d 6574 6572 2077  This parameter w
+00005bd0: 696c 6c20 6265 2070 7269 6f72 6974 6973  ill be prioritis
+00005be0: 6564 206f 7665 7220 7468 6520 7061 7468  ed over the path
+00005bf0: 2067 6976 656e 2069 6e20 636f 6e66 6967   given in config
+00005c00: 7572 6174 696f 6e20 2869 6620 616e 7929  uration (if any)
+00005c10: 2e94 8594 8194 7d94 2868 1b6a d407 0000  ......}.(h.j....
+00005c20: 681c 6803 681d 4e68 1e4e 7562 6568 1f7d  h.h.h.Nh.Nubeh.}
+00005c30: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00005c40: 5d94 6829 5d94 7568 2b68 3e68 1e4b 7268  ].h)].uh+h>h.Krh
+00005c50: 1d68 2c68 1b6a d107 0000 681c 6803 7562  .h,h.j....h.h.ub
+00005c60: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00005c70: 5d94 6827 5d94 6829 5d94 7568 2b6a 3202  ].h'].h)].uh+j2.
+00005c80: 0000 681e 4b72 681d 682c 681b 6a08 0700  ..h.Krh.h,h.j...
+00005c90: 0068 1c68 0375 626a 3302 0000 2981 947d  .h.h.ubj3...)..}
+00005ca0: 9428 6805 6806 6807 5d94 683f 2981 947d  .(h.h.h.].h?)..}
+00005cb0: 9428 6805 8cba 6066 6f72 6365 6020 2020  .(h...`force`   
+00005cc0: 2020 203a 2049 6620 6120 6669 6c65 2068     : If a file h
+00005cd0: 6173 2074 6865 2073 616d 6520 6e61 6d65  as the same name
+00005ce0: 2069 6e20 7468 6520 636f 6e76 6572 7465   in the converte
+00005cf0: 6420 666f 6c64 6572 2c20 7368 6f75 6c64  d folder, should
+00005d00: 2069 7420 6265 2072 6570 6c61 6365 6420   it be replaced 
+00005d10: 3f20 2846 696c 6520 7769 6c6c 206e 6f74  ? (File will not
+00005d20: 2062 6520 7361 7665 6420 6966 2073 6962   be saved if sib
+00005d30: 6c69 6e67 2066 6f75 6e64 2069 6e20 636f  ling found in co
+00005d40: 6e76 6572 7420 666f 6c64 6572 2061 6e64  nvert folder and
+00005d50: 2074 6869 7320 7061 7261 6d65 7465 7220   this parameter 
+00005d60: 7365 7420 746f 2060 4661 6c73 6560 2e29  set to `False`.)
+00005d70: 9468 075d 9428 6a47 0100 0029 8194 7d94  .h.].(jG...)..}.
+00005d80: 2868 058c 0566 6f72 6365 9468 075d 9468  (h...force.h.].h
+00005d90: 168c 0566 6f72 6365 9485 9481 947d 9428  ...force.....}.(
+00005da0: 681b 6afd 0700 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00005db0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00005dc0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00005dd0: 6a46 0100 0068 1e4b 7368 1d68 2c68 1b6a  jF...h.Ksh.h,h.j
+00005de0: f907 0000 681c 6803 7562 6816 8caa 2020  ....h.h.ubh...  
+00005df0: 2020 2020 3a20 4966 2061 2066 696c 6520      : If a file 
+00005e00: 6861 7320 7468 6520 7361 6d65 206e 616d  has the same nam
+00005e10: 6520 696e 2074 6865 2063 6f6e 7665 7274  e in the convert
+00005e20: 6564 2066 6f6c 6465 722c 2073 686f 756c  ed folder, shoul
+00005e30: 6420 6974 2062 6520 7265 706c 6163 6564  d it be replaced
+00005e40: 203f 2028 4669 6c65 2077 696c 6c20 6e6f   ? (File will no
+00005e50: 7420 6265 2073 6176 6564 2069 6620 7369  t be saved if si
+00005e60: 626c 696e 6720 666f 756e 6420 696e 2063  bling found in c
+00005e70: 6f6e 7665 7274 2066 6f6c 6465 7220 616e  onvert folder an
+00005e80: 6420 7468 6973 2070 6172 616d 6574 6572  d this parameter
+00005e90: 2073 6574 2074 6f20 9485 9481 947d 9428   set to .....}.(
+00005ea0: 681b 6af9 0700 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00005eb0: 4e75 626a 4701 0000 2981 947d 9428 6805  NubjG...)..}.(h.
+00005ec0: 8c05 4661 6c73 6594 6807 5d94 6816 8c05  ..False.h.].h...
+00005ed0: 4661 6c73 6594 8594 8194 7d94 2868 1b6a  False.....}.(h.j
+00005ee0: 0f08 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00005ef0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00005f00: 5d94 6827 5d94 6829 5d94 7568 2b6a 4601  ].h'].h)].uh+jF.
+00005f10: 0000 681e 4b73 681d 682c 681b 6af9 0700  ..h.Ksh.h,h.j...
+00005f20: 0068 1c68 0375 6268 168c 022e 2994 8594  .h.h.ubh....)...
+00005f30: 8194 7d94 2868 1b6a f907 0000 681c 6803  ..}.(h.j....h.h.
+00005f40: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
+00005f50: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00005f60: 5d94 7568 2b68 3e68 1e4b 7368 1d68 2c68  ].uh+h>h.Ksh.h,h
+00005f70: 1b6a f607 0000 681c 6803 7562 6168 1f7d  .j....h.h.ubah.}
+00005f80: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00005f90: 5d94 6829 5d94 7568 2b6a 3202 0000 681e  ].h)].uh+j2...h.
+00005fa0: 4b73 681d 682c 681b 6a08 0700 0068 1c68  Ksh.h,h.j....h.h
+00005fb0: 0375 626a 3302 0000 2981 947d 9428 6805  .ubj3...)..}.(h.
+00005fc0: 6806 6807 5d94 683f 2981 947d 9428 6805  h.h.].h?)..}.(h.
+00005fd0: 8c54 6072 656d 6f76 6560 2020 2020 203a  .T`remove`     :
+00005fe0: 2053 686f 756c 6420 7468 6520 6f72 6967   Should the orig
+00005ff0: 696e 616c 2066 696c 6520 6265 2072 656d  inal file be rem
+00006000: 6f76 6564 2077 6865 6e20 6974 2069 7320  oved when it is 
+00006010: 7361 7665 6420 6173 2060 2e6d 6174 6020  saved as `.mat` 
+00006020: 6669 6c65 203f 9468 075d 9428 6a47 0100  file ?.h.].(jG..
+00006030: 0029 8194 7d94 2868 058c 0672 656d 6f76  .)..}.(h...remov
+00006040: 6594 6807 5d94 6816 8c06 7265 6d6f 7665  e.h.].h...remove
+00006050: 9485 9481 947d 9428 681b 6a34 0800 0068  .....}.(h.j4...h
+00006060: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00006070: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00006080: 9468 295d 9475 682b 6a46 0100 0068 1e4b  .h)].uh+jF...h.K
+00006090: 7468 1d68 2c68 1b6a 3008 0000 681c 6803  th.h,h.j0...h.h.
+000060a0: 7562 6816 8c3f 2020 2020 203a 2053 686f  ubh..?     : Sho
+000060b0: 756c 6420 7468 6520 6f72 6967 696e 616c  uld the original
+000060c0: 2066 696c 6520 6265 2072 656d 6f76 6564   file be removed
+000060d0: 2077 6865 6e20 6974 2069 7320 7361 7665   when it is save
+000060e0: 6420 6173 2094 8594 8194 7d94 2868 1b6a  d as .....}.(h.j
+000060f0: 3008 0000 681c 6803 681d 4e68 1e4e 7562  0...h.h.h.Nh.Nub
+00006100: 6a47 0100 0029 8194 7d94 2868 058c 042e  jG...)..}.(h....
+00006110: 6d61 7494 6807 5d94 6816 8c04 2e6d 6174  mat.h.].h....mat
+00006120: 9485 9481 947d 9428 681b 6a46 0800 0068  .....}.(h.jF...h
+00006130: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00006140: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00006150: 9468 295d 9475 682b 6a46 0100 0068 1e4b  .h)].uh+jF...h.K
+00006160: 7468 1d68 2c68 1b6a 3008 0000 681c 6803  th.h,h.j0...h.h.
+00006170: 7562 6816 8c07 2066 696c 6520 3f94 8594  ubh... file ?...
+00006180: 8194 7d94 2868 1b6a 3008 0000 681c 6803  ..}.(h.j0...h.h.
+00006190: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
+000061a0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000061b0: 5d94 7568 2b68 3e68 1e4b 7468 1d68 2c68  ].uh+h>h.Kth.h,h
+000061c0: 1b6a 2d08 0000 681c 6803 7562 6168 1f7d  .j-...h.h.ubah.}
+000061d0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+000061e0: 5d94 6829 5d94 7568 2b6a 3202 0000 681e  ].h)].uh+j2...h.
+000061f0: 4b74 681d 682c 681b 6a08 0700 0068 1c68  Kth.h,h.j....h.h
+00006200: 0375 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
+00006210: 9468 255d 9468 275d 9468 295d 946a bc02  .h%].h'].h)].j..
+00006220: 0000 6abd 0200 0075 682b 6a2d 0200 0068  ..j....uh+j-...h
+00006230: 1e4b 6e68 1d68 2c68 1b6a bb06 0000 681c  .Knh.h,h.j....h.
+00006240: 6803 7562 683f 2981 947d 9428 6805 8c1d  h.ubh?)..}.(h...
+00006250: 3c75 3e4f 7574 7075 7473 3c2f 753e 3c62  <u>Outputs</u><b
+00006260: 723e 0a4e 6f20 6f75 7470 7574 7394 6807  r>.No outputs.h.
+00006270: 5d94 286a 0302 0000 2981 947d 9428 6805  ].(j....)..}.(h.
+00006280: 8c03 3c75 3e94 6807 5d94 6816 8c03 3c75  ..<u>.h.].h...<u
+00006290: 3e94 8594 8194 7d94 2868 1b6a 6e08 0000  >.....}.(h.jn...
+000062a0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+000062b0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+000062c0: 5d94 6829 5d94 8c06 666f 726d 6174 946a  ].h)]...format.j
+000062d0: 1302 0000 687a 687b 7568 2b6a 0202 0000  ....hzh{uh+j....
+000062e0: 681d 682c 681e 4b76 681b 6a6a 0800 0068  h.h,h.Kvh.jj...h
+000062f0: 1c68 0375 6268 168c 074f 7574 7075 7473  .h.ubh...Outputs
+00006300: 9485 9481 947d 9428 681b 6a6a 0800 0068  .....}.(h.jj...h
+00006310: 1c68 0368 1d4e 681e 4e75 626a 0302 0000  .h.h.Nh.Nubj....
+00006320: 2981 947d 9428 6805 8c04 3c2f 753e 9468  )..}.(h...</u>.h
+00006330: 075d 9468 168c 043c 2f75 3e94 8594 8194  .].h...</u>.....
+00006340: 7d94 2868 1b6a 8108 0000 681c 6803 681d  }.(h.j....h.h.h.
+00006350: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00006360: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00006370: 8c06 666f 726d 6174 946a 1302 0000 687a  ..format.j....hz
+00006380: 687b 7568 2b6a 0202 0000 681d 682c 681e  h{uh+j....h.h,h.
+00006390: 4b76 681b 6a6a 0800 0068 1c68 0375 626a  Kvh.jj...h.h.ubj
+000063a0: 0302 0000 2981 947d 9428 6805 8c04 3c62  ....)..}.(h...<b
+000063b0: 723e 9468 075d 9468 168c 043c 6272 3e94  r>.h.].h...<br>.
+000063c0: 8594 8194 7d94 2868 1b6a 9008 0000 681c  ....}.(h.j....h.
+000063d0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+000063e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000063f0: 6829 5d94 8c06 666f 726d 6174 946a 1302  h)]...format.j..
+00006400: 0000 687a 687b 7568 2b6a 0202 0000 681d  ..hzh{uh+j....h.
+00006410: 682c 681e 4b76 681b 6a6a 0800 0068 1c68  h,h.Kvh.jj...h.h
+00006420: 0375 6268 168c 010a 9485 9481 947d 9428  .ubh.........}.(
+00006430: 681b 6a6a 0800 0068 1c68 0368 1d4e 681e  h.jj...h.h.h.Nh.
+00006440: 4e75 6268 168c 0a4e 6f20 6f75 7470 7574  Nubh...No output
+00006450: 7394 8594 8194 7d94 2868 1b6a 6a08 0000  s.....}.(h.jj...
+00006460: 681c 6803 681d 4e68 1e4e 7562 6568 1f7d  h.h.h.Nh.Nubeh.}
+00006470: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00006480: 5d94 6829 5d94 7568 2b68 3e68 1e4b 7668  ].h)].uh+h>h.Kvh
+00006490: 1d68 2c68 1b6a bb06 0000 681c 6803 7562  .h,h.j....h.h.ub
+000064a0: 6568 1f7d 9428 6821 5d94 8c04 6964 3130  eh.}.(h!]...id10
+000064b0: 9461 6823 5d94 6825 5d94 6827 5d94 8c0a  .ah#].h%].h']...
+000064c0: 686f 7720 746f 2075 7365 9461 6829 5d94  how to use.ah)].
+000064d0: 7568 2b68 0a68 1e4b 6468 1d68 2c68 1b6a  uh+h.h.Kdh.h,h.j
+000064e0: 3606 0000 681c 6803 6856 4b01 7562 6568  6...h.h.hVK.ubeh
+000064f0: 1f7d 9428 6821 5d94 8c0b 636f 6e76 6572  .}.(h!]...conver
+00006500: 7466 696c 6594 6168 235d 9468 255d 948c  tfile.ah#].h%]..
+00006510: 0b63 6f6e 7665 7274 6669 6c65 9461 6827  .convertfile.ah'
+00006520: 5d94 6829 5d94 7568 2b68 0a68 1e4b 5b68  ].h)].uh+h.h.K[h
+00006530: 1d68 2c68 1b6a 0b01 0000 681c 6803 7562  .h,h.j....h.h.ub
+00006540: 6568 1f7d 9428 6821 5d94 8c09 6675 6e63  eh.}.(h!]...func
+00006550: 7469 6f6e 7394 6168 235d 9468 255d 948c  tions.ah#].h%]..
+00006560: 0966 756e 6374 696f 6e73 9461 6827 5d94  .functions.ah'].
+00006570: 6829 5d94 7568 2b68 0a68 1e4b 1e68 1d68  h)].uh+h.h.K.h.h
+00006580: 2c68 1b68 0c68 1c68 0375 6265 681f 7d94  ,h.h.h.h.ubeh.}.
+00006590: 2868 215d 948c 0d6d 7a64 6174 616d 616e  (h!]...mzdataman
+000065a0: 6167 6572 9461 6823 5d94 6825 5d94 8c0d  ager.ah#].h%]...
+000065b0: 6d7a 6461 7461 6d61 6e61 6765 7294 6168  mzdatamanager.ah
+000065c0: 275d 9468 295d 9475 682b 680a 681e 4b01  '].h)].uh+h.h.K.
+000065d0: 681d 682c 681b 6803 681c 6803 7562 6168  h.h,h.h.h.h.ubah
+000065e0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000065f0: 6827 5d94 6829 5d94 8c06 736f 7572 6365  h'].h)]...source
+00006600: 9468 2c8c 1474 7261 6e73 6c61 7469 6f6e  .h,..translation
+00006610: 5f70 726f 6772 6573 7394 7d94 288c 0574  _progress.}.(..t
+00006620: 6f74 616c 944b 008c 0a74 7261 6e73 6c61  otal.K...transla
+00006630: 7465 6494 4b00 7575 682b 6801 8c0e 6375  ted.K.uuh+h...cu
+00006640: 7272 656e 745f 736f 7572 6365 944e 8c0c  rrent_source.N..
+00006650: 6375 7272 656e 745f 6c69 6e65 944e 8c08  current_line.N..
+00006660: 7365 7474 696e 6773 948c 1164 6f63 7574  settings...docut
+00006670: 696c 732e 6672 6f6e 7465 6e64 948c 0656  ils.frontend...V
+00006680: 616c 7565 7394 9394 2981 947d 9428 8c06  alues...)..}.(..
+00006690: 6f75 7470 7574 944e 680f 4e8c 0967 656e  output.Nh.N..gen
+000066a0: 6572 6174 6f72 944e 8c09 6461 7465 7374  erator.N..datest
+000066b0: 616d 7094 4e8c 0b73 6f75 7263 655f 6c69  amp.N..source_li
+000066c0: 6e6b 944e 8c0a 736f 7572 6365 5f75 726c  nk.N..source_url
+000066d0: 944e 8c0d 746f 635f 6261 636b 6c69 6e6b  .N..toc_backlink
+000066e0: 7394 8c05 656e 7472 7994 8c12 666f 6f74  s...entry...foot
+000066f0: 6e6f 7465 5f62 6163 6b6c 696e 6b73 944b  note_backlinks.K
+00006700: 018c 0d73 6563 746e 756d 5f78 666f 726d  ...sectnum_xform
+00006710: 944b 018c 0e73 7472 6970 5f63 6f6d 6d65  .K...strip_comme
+00006720: 6e74 7394 4e8c 1b73 7472 6970 5f65 6c65  nts.N..strip_ele
+00006730: 6d65 6e74 735f 7769 7468 5f63 6c61 7373  ments_with_class
+00006740: 6573 944e 8c0d 7374 7269 705f 636c 6173  es.N..strip_clas
+00006750: 7365 7394 4e8c 0c72 6570 6f72 745f 6c65  ses.N..report_le
+00006760: 7665 6c94 4b02 8c0a 6861 6c74 5f6c 6576  vel.K...halt_lev
+00006770: 656c 944b 058c 1165 7869 745f 7374 6174  el.K...exit_stat
+00006780: 7573 5f6c 6576 656c 944b 058c 0564 6562  us_level.K...deb
+00006790: 7567 944e 8c0e 7761 726e 696e 675f 7374  ug.N..warning_st
+000067a0: 7265 616d 944e 8c09 7472 6163 6562 6163  ream.N..tracebac
+000067b0: 6b94 888c 0e69 6e70 7574 5f65 6e63 6f64  k....input_encod
+000067c0: 696e 6794 8c09 7574 662d 382d 7369 6794  ing...utf-8-sig.
+000067d0: 8c1c 696e 7075 745f 656e 636f 6469 6e67  ..input_encoding
+000067e0: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+000067f0: 0673 7472 6963 7494 8c0f 6f75 7470 7574  .strict...output
+00006800: 5f65 6e63 6f64 696e 6794 8c05 7574 662d  _encoding...utf-
+00006810: 3894 8c1d 6f75 7470 7574 5f65 6e63 6f64  8...output_encod
+00006820: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
+00006830: 7294 6af5 0800 008c 0e65 7272 6f72 5f65  r.j......error_e
+00006840: 6e63 6f64 696e 6794 8c05 7574 662d 3894  ncoding...utf-8.
+00006850: 8c1c 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
+00006860: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+00006870: 1062 6163 6b73 6c61 7368 7265 706c 6163  .backslashreplac
+00006880: 6594 8c0d 6c61 6e67 7561 6765 5f63 6f64  e...language_cod
+00006890: 6594 8c02 656e 948c 1372 6563 6f72 645f  e...en...record_
+000068a0: 6465 7065 6e64 656e 6369 6573 944e 8c06  dependencies.N..
+000068b0: 636f 6e66 6967 944e 8c09 6964 5f70 7265  config.N..id_pre
+000068c0: 6669 7894 6806 8c0e 6175 746f 5f69 645f  fix.h...auto_id_
+000068d0: 7072 6566 6978 948c 0269 6494 8c0d 6475  prefix...id...du
+000068e0: 6d70 5f73 6574 7469 6e67 7394 4e8c 0e64  mp_settings.N..d
+000068f0: 756d 705f 696e 7465 726e 616c 7394 4e8c  ump_internals.N.
+00006900: 0f64 756d 705f 7472 616e 7366 6f72 6d73  .dump_transforms
+00006910: 944e 8c0f 6475 6d70 5f70 7365 7564 6f5f  .N..dump_pseudo_
+00006920: 786d 6c94 4e8c 1065 7870 6f73 655f 696e  xml.N..expose_in
+00006930: 7465 726e 616c 7394 4e8c 0e73 7472 6963  ternals.N..stric
+00006940: 745f 7669 7369 746f 7294 4e8c 0f5f 6469  t_visitor.N.._di
+00006950: 7361 626c 655f 636f 6e66 6967 944e 8c07  sable_config.N..
+00006960: 5f73 6f75 7263 6594 682c 8c0c 5f64 6573  _source.h,.._des
+00006970: 7469 6e61 7469 6f6e 944e 8c0d 5f63 6f6e  tination.N.._con
+00006980: 6669 675f 6669 6c65 7394 5d94 8c16 6669  fig_files.]...fi
+00006990: 6c65 5f69 6e73 6572 7469 6f6e 5f65 6e61  le_insertion_ena
+000069a0: 626c 6564 9488 8c0b 7261 775f 656e 6162  bled....raw_enab
+000069b0: 6c65 6494 4b01 8c11 6c69 6e65 5f6c 656e  led.K...line_len
+000069c0: 6774 685f 6c69 6d69 7494 4d10 278c 0e70  gth_limit.M.'..p
+000069d0: 6570 5f72 6566 6572 656e 6365 7394 4e8c  ep_references.N.
+000069e0: 0c70 6570 5f62 6173 655f 7572 6c94 8c18  .pep_base_url...
+000069f0: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
+00006a00: 686f 6e2e 6f72 672f 948c 1570 6570 5f66  hon.org/...pep_f
+00006a10: 696c 655f 7572 6c5f 7465 6d70 6c61 7465  ile_url_template
+00006a20: 948c 0870 6570 2d25 3034 6494 8c0e 7266  ...pep-%04d...rf
+00006a30: 635f 7265 6665 7265 6e63 6573 944e 8c0c  c_references.N..
+00006a40: 7266 635f 6261 7365 5f75 726c 948c 2668  rfc_base_url..&h
+00006a50: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
+00006a60: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
+00006a70: 6874 6d6c 2f94 8c09 7461 625f 7769 6474  html/...tab_widt
+00006a80: 6894 4b08 8c1d 7472 696d 5f66 6f6f 746e  h.K...trim_footn
+00006a90: 6f74 655f 7265 6665 7265 6e63 655f 7370  ote_reference_sp
+00006aa0: 6163 6594 898c 1073 796e 7461 785f 6869  ace....syntax_hi
+00006ab0: 6768 6c69 6768 7494 8c04 6c6f 6e67 948c  ghlight...long..
+00006ac0: 0c73 6d61 7274 5f71 756f 7465 7394 888c  .smart_quotes...
+00006ad0: 1373 6d61 7274 7175 6f74 6573 5f6c 6f63  .smartquotes_loc
+00006ae0: 616c 6573 945d 948c 1d63 6861 7261 6374  ales.]...charact
+00006af0: 6572 5f6c 6576 656c 5f69 6e6c 696e 655f  er_level_inline_
+00006b00: 6d61 726b 7570 9489 8c0e 646f 6374 6974  markup....doctit
+00006b10: 6c65 5f78 666f 726d 9489 8c0d 646f 6369  le_xform....doci
+00006b20: 6e66 6f5f 7866 6f72 6d94 4b01 8c12 7365  nfo_xform.K...se
+00006b30: 6374 7375 6274 6974 6c65 5f78 666f 726d  ctsubtitle_xform
+00006b40: 9489 8c0d 696d 6167 655f 6c6f 6164 696e  ....image_loadin
+00006b50: 6794 8c04 6c69 6e6b 948c 1065 6d62 6564  g...link...embed
+00006b60: 5f73 7479 6c65 7368 6565 7494 898c 1563  _stylesheet....c
+00006b70: 6c6f 616b 5f65 6d61 696c 5f61 6464 7265  loak_email_addre
+00006b80: 7373 6573 9488 8c11 7365 6374 696f 6e5f  sses....section_
+00006b90: 7365 6c66 5f6c 696e 6b94 898c 0365 6e76  self_link....env
+00006ba0: 944e 7562 8c08 7265 706f 7274 6572 944e  .Nub..reporter.N
+00006bb0: 8c10 696e 6469 7265 6374 5f74 6172 6765  ..indirect_targe
+00006bc0: 7473 945d 948c 1173 7562 7374 6974 7574  ts.]...substitut
+00006bd0: 696f 6e5f 6465 6673 947d 9428 8c0f 776f  ion_defs.}.(..wo
+00006be0: 7264 636f 756e 742d 776f 7264 7394 6809  rdcount-words.h.
+00006bf0: 8c17 7375 6273 7469 7475 7469 6f6e 5f64  ..substitution_d
+00006c00: 6566 696e 6974 696f 6e94 9394 2981 947d  efinition...)..}
+00006c10: 9428 6805 8c03 3433 3594 6807 5d94 6816  .(h...435.h.].h.
+00006c20: 8c03 3433 3594 8594 8194 7d94 681b 6a33  ..435.....}.h.j3
+00006c30: 0900 0073 6261 681f 7d94 2868 215d 9468  ...sbah.}.(h!].h
+00006c40: 235d 9468 255d 948c 0f77 6f72 6463 6f75  #].h%]...wordcou
+00006c50: 6e74 2d77 6f72 6473 9461 6827 5d94 6829  nt-words.ah'].h)
+00006c60: 5d94 7568 2b6a 3109 0000 681d 682c 7562  ].uh+j1...h.h,ub
+00006c70: 8c11 776f 7264 636f 756e 742d 6d69 6e75  ..wordcount-minu
+00006c80: 7465 7394 6a32 0900 0029 8194 7d94 2868  tes.j2...)..}.(h
+00006c90: 058c 0132 9468 075d 9468 168c 0132 9485  ...2.h.].h...2..
+00006ca0: 9481 947d 9468 1b6a 4309 0000 7362 6168  ...}.h.jC...sbah
+00006cb0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00006cc0: 8c11 776f 7264 636f 756e 742d 6d69 6e75  ..wordcount-minu
+00006cd0: 7465 7394 6168 275d 9468 295d 9475 682b  tes.ah'].h)].uh+
+00006ce0: 6a31 0900 0068 1d68 2c75 6275 8c12 7375  j1...h.h,ubu..su
+00006cf0: 6273 7469 7475 7469 6f6e 5f6e 616d 6573  bstitution_names
+00006d00: 947d 9428 8c0f 776f 7264 636f 756e 742d  .}.(..wordcount-
+00006d10: 776f 7264 7394 6a30 0900 008c 1177 6f72  words.j0.....wor
+00006d20: 6463 6f75 6e74 2d6d 696e 7574 6573 946a  dcount-minutes.j
+00006d30: 4209 0000 758c 0872 6566 6e61 6d65 7394  B...u..refnames.
+00006d40: 7d94 8c06 7265 6669 6473 947d 946a b103  }...refids.}.j..
+00006d50: 0000 5d94 6aa6 0300 0061 738c 076e 616d  ..].j....as..nam
+00006d60: 6569 6473 947d 9428 6aca 0800 006a c708  eids.}.(j....j..
+00006d70: 0000 8c0c 7072 6573 656e 7461 7469 6f6e  ....presentation
+00006d80: 944e 8c0a 6465 6669 6e69 7469 6f6e 944e  .N..definition.N
+00006d90: 8c0a 686f 7720 746f 2075 7365 944e 68c9  ..how to use.Nh.
+00006da0: 68c6 6a00 0100 0068 fd6a c208 0000 6abf  h.j....h.j....j.
+00006db0: 0800 006a be03 0000 6abb 0300 006a 2e06  ...j....j....j..
+00006dc0: 0000 6ab1 0300 006a ba08 0000 6ab7 0800  ..j....j....j...
+00006dd0: 0075 8c09 6e61 6d65 7479 7065 7394 7d94  .u..nametypes.}.
+00006de0: 286a ca08 0000 896a 5d09 0000 896a 5e09  (j.....j]....j^.
+00006df0: 0000 896a 5f09 0000 8968 c989 6a00 0100  ...j_....h..j...
+00006e00: 0089 6ac2 0800 0089 6abe 0300 0089 6a2e  ..j.....j.....j.
+00006e10: 0600 0088 6aba 0800 0089 7568 217d 9428  ....j.....uh!}.(
+00006e20: 6ac7 0800 0068 0c68 5068 2d68 7e68 576a  j....h.hPh-h~hWj
+00006e30: 0501 0000 6884 68c6 6895 68fd 68cc 6abf  ....h.h.h.h.h.j.
+00006e40: 0800 006a 0b01 0000 6abb 0300 006a 1c01  ...j....j....j..
+00006e50: 0000 6ab0 0100 006a 2d01 0000 6ad8 0100  ..j....j-...j...
+00006e60: 006a b501 0000 6ab4 0300 006a dd01 0000  .j....j....j....
+00006e70: 6ab1 0300 006a c103 0000 6a2b 0600 006a  j....j....j+...j
+00006e80: c103 0000 6a17 0400 006a d203 0000 6a40  ....j....j....j@
+00006e90: 0400 006a 1d04 0000 6a23 0600 006a 4604  ...j....j#...jF.
+00006ea0: 0000 6ab7 0800 006a 3606 0000 6a8c 0600  ..j....j6...j...
+00006eb0: 006a 4706 0000 6ab5 0600 006a 9206 0000  .jG...j....j....
+00006ec0: 6aaf 0800 006a bb06 0000 758c 0d66 6f6f  j....j....u..foo
+00006ed0: 746e 6f74 655f 7265 6673 947d 948c 0d63  tnote_refs.}...c
+00006ee0: 6974 6174 696f 6e5f 7265 6673 947d 948c  itation_refs.}..
+00006ef0: 0d61 7574 6f66 6f6f 746e 6f74 6573 945d  .autofootnotes.]
+00006f00: 948c 1161 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+00006f10: 7265 6673 945d 948c 1073 796d 626f 6c5f  refs.]...symbol_
+00006f20: 666f 6f74 6e6f 7465 7394 5d94 8c14 7379  footnotes.]...sy
+00006f30: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7265  mbol_footnote_re
+00006f40: 6673 945d 948c 0966 6f6f 746e 6f74 6573  fs.]...footnotes
+00006f50: 945d 948c 0963 6974 6174 696f 6e73 945d  .]...citations.]
+00006f60: 948c 1261 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+00006f70: 7374 6172 7494 4b01 8c15 7379 6d62 6f6c  start.K...symbol
+00006f80: 5f66 6f6f 746e 6f74 655f 7374 6172 7494  _footnote_start.
+00006f90: 4b00 8c0a 6964 5f63 6f75 6e74 6572 948c  K...id_counter..
+00006fa0: 0b63 6f6c 6c65 6374 696f 6e73 948c 0743  .collections...C
+00006fb0: 6f75 6e74 6572 9493 947d 946a 0309 0000  ounter...}.j....
+00006fc0: 4b0a 7385 9452 948c 0e70 6172 7365 5f6d  K.s..R...parse_m
+00006fd0: 6573 7361 6765 7394 5d94 8c12 7472 616e  essages.]...tran
+00006fe0: 7366 6f72 6d5f 6d65 7373 6167 6573 945d  sform_messages.]
+00006ff0: 9468 098c 0e73 7973 7465 6d5f 6d65 7373  .h...system_mess
+00007000: 6167 6594 9394 2981 947d 9428 6805 6806  age...)..}.(h.h.
+00007010: 6807 5d94 683f 2981 947d 9428 6805 6806  h.].h?)..}.(h.h.
+00007020: 6807 5d94 6816 8c31 4879 7065 726c 696e  h.].h..1Hyperlin
+00007030: 6b20 7461 7267 6574 2022 7361 7665 6d61  k target "savema
+00007040: 7466 696c 6522 2069 7320 6e6f 7420 7265  tfile" is not re
+00007050: 6665 7265 6e63 6564 2e94 8594 8194 7d94  ferenced......}.
+00007060: 681b 6a85 0900 0073 6261 681f 7d94 2868  h.j....sbah.}.(h
+00007070: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00007080: 295d 9475 682b 683e 681b 6a82 0900 0075  )].uh+h>h.j....u
+00007090: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+000070a0: 255d 9468 275d 9468 295d 948c 056c 6576  %].h'].h)]...lev
+000070b0: 656c 944b 018c 0474 7970 6594 8c04 494e  el.K...type...IN
+000070c0: 464f 948c 0673 6f75 7263 6594 682c 8c04  FO...source.h,..
+000070d0: 6c69 6e65 944b 3d75 682b 6a80 0900 0075  line.K=uh+j....u
+000070e0: 6261 8c0b 7472 616e 7366 6f72 6d65 7294  ba..transformer.
+000070f0: 4e8c 0b69 6e63 6c75 6465 5f6c 6f67 945d  N..include_log.]
+00007100: 948c 0a64 6563 6f72 6174 696f 6e94 4e68  ...decoration.Nh
+00007110: 1c68 038c 0a6d 7973 745f 736c 7567 7394  .h...myst_slugs.
+00007120: 7d94 7562 2e                             }.ub.
```

### Comparing `mzdata2mat-0.1.1/docs/build/doctrees/mzDataXMLStruct.doctree` & `mzdata2mat-0.2.0/docs/build/doctrees/mzdata2mat-verify.doctree`

 * *Files 26% similar despite different names*

```diff
@@ -1,412 +1,400 @@
-00000000: 8005 95b4 1900 0000 0000 008c 0f73 7068  .............sph
+00000000: 8005 95ea 1800 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
-00000080: 6594 9394 2981 947d 9428 6805 8c0f 6d7a  e...)..}.(h...mz
-00000090: 4461 7461 584d 4c53 7472 7563 7494 6807  DataXMLStruct.h.
-000000a0: 5d94 6809 8c04 5465 7874 9493 948c 0f6d  ].h...Text.....m
-000000b0: 7a44 6174 6158 4d4c 5374 7275 6374 9485  zDataXMLStruct..
-000000c0: 9481 947d 9428 8c06 7061 7265 6e74 9468  ...}.(..parent.h
-000000d0: 118c 095f 646f 6375 6d65 6e74 9468 038c  ..._document.h..
-000000e0: 0673 6f75 7263 6594 4e8c 046c 696e 6594  .source.N..line.
-000000f0: 4e75 6261 8c0a 6174 7472 6962 7574 6573  Nuba..attributes
-00000100: 947d 9428 8c03 6964 7394 5d94 8c07 636c  .}.(..ids.]...cl
-00000110: 6173 7365 7394 5d94 8c05 6e61 6d65 7394  asses.]...names.
-00000120: 5d94 8c08 6475 706e 616d 6573 945d 948c  ]...dupnames.]..
-00000130: 0862 6163 6b72 6566 7394 5d94 758c 0774  .backrefs.].u..t
-00000140: 6167 6e61 6d65 9468 0f68 1e4b 0168 1d8c  agname.h.h.K.h..
-00000150: 7d2f 5573 6572 732f 6c69 6368 3931 312f  }/Users/lich911/
-00000160: 4c69 6272 6172 792f 436c 6f75 6453 746f  Library/CloudSto
-00000170: 7261 6765 2f4f 6e65 4472 6976 652d 5065  rage/OneDrive-Pe
-00000180: 7273 6f6e 6e65 6c2f 446f 6375 6d65 6e74  rsonnel/Document
-00000190: 732f 5079 7468 6f6e 2f50 6163 6b61 6765  s/Python/Package
-000001a0: 732f 6d7a 4461 7461 584d 4c32 4d61 742f  s/mzDataXML2Mat/
-000001b0: 646f 6373 2f73 6f75 7263 652f 6d7a 4461  docs/source/mzDa
-000001c0: 7461 584d 4c53 7472 7563 742e 6d64 9468  taXMLStruct.md.h
-000001d0: 1b68 0c68 1c68 0375 6268 0b29 8194 7d94  .h.h.h.ubh.)..}.
-000001e0: 2868 0568 0668 075d 9428 6810 2981 947d  (h.h.h.].(h.)..}
-000001f0: 9428 6805 8c0c 5072 6573 656e 7461 7469  .(h...Presentati
-00000200: 6f6e 9468 075d 9468 168c 0c50 7265 7365  on.h.].h...Prese
-00000210: 6e74 6174 696f 6e94 8594 8194 7d94 2868  ntation.....}.(h
-00000220: 1b68 3068 1c68 0368 1d4e 681e 4e75 6261  .h0h.h.h.Nh.Nuba
-00000230: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00000240: 9468 275d 9468 295d 9475 682b 680f 681e  .h'].h)].uh+h.h.
-00000250: 4b03 681d 682c 681b 682d 681c 6803 7562  K.h.h,h.h-h.h.ub
-00000260: 6809 8c09 7061 7261 6772 6170 6894 9394  h...paragraph...
-00000270: 2981 947d 9428 6805 8c5e 496e 7465 726e  )..}.(h..^Intern
-00000280: 616c 2063 6c61 7373 2c20 646f 206e 6f74  al class, do not
-00000290: 2075 7365 2069 7420 746f 2073 746f 7265   use it to store
-000002a0: 2064 6174 612e 2043 6f6e 7369 6465 7220   data. Consider 
-000002b0: 7573 696e 6720 5b6d 7a44 6174 615d 286d  using [mzData](m
-000002c0: 7a44 6174 612e 6d64 2920 636c 6173 7320  zData.md) class 
-000002d0: 696e 7374 6561 642e 9468 075d 9428 6816  instead..h.].(h.
-000002e0: 8c3c 496e 7465 726e 616c 2063 6c61 7373  .<Internal class
-000002f0: 2c20 646f 206e 6f74 2075 7365 2069 7420  , do not use it 
-00000300: 746f 2073 746f 7265 2064 6174 612e 2043  to store data. C
-00000310: 6f6e 7369 6465 7220 7573 696e 6720 9485  onsider using ..
-00000320: 9481 947d 9428 681b 6840 681c 6803 681d  ...}.(h.h@h.h.h.
-00000330: 4e68 1e4e 7562 6800 8c0c 7065 6e64 696e  Nh.Nubh...pendin
-00000340: 675f 7872 6566 9493 9429 8194 7d94 2868  g_xref...)..}.(h
-00000350: 0568 0668 075d 9468 098c 0669 6e6c 696e  .h.h.].h...inlin
-00000360: 6594 9394 2981 947d 9428 6805 8c06 6d7a  e...)..}.(h...mz
-00000370: 4461 7461 9468 075d 9468 168c 066d 7a44  Data.h.].h...mzD
-00000380: 6174 6194 8594 8194 7d94 2868 1b68 4f68  ata.....}.(h.hOh
-00000390: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-000003a0: 2868 215d 9468 235d 9428 8c04 7872 6566  (h!].h#].(..xref
-000003b0: 948c 046d 7973 7494 6568 255d 9468 275d  ...myst.eh%].h']
-000003c0: 9468 295d 9475 682b 684d 681b 684a 681c  .h)].uh+hMh.hJh.
-000003d0: 6803 681d 682c 681e 4b00 7562 6168 1f7d  h.h.h,h.K.ubah.}
-000003e0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000003f0: 5d94 6829 5d94 8c09 7265 6664 6f6d 6169  ].h)]...refdomai
-00000400: 6e94 8c03 646f 6394 8c09 7265 6674 6172  n...doc...reftar
-00000410: 6765 7494 8c06 6d7a 4461 7461 948c 0b72  get...mzData...r
-00000420: 6566 7461 7267 6574 6964 944e 8c06 7265  eftargetid.N..re
-00000430: 6664 6f63 948c 0f6d 7a44 6174 6158 4d4c  fdoc...mzDataXML
-00000440: 5374 7275 6374 948c 0772 6566 7479 7065  Struct...reftype
-00000450: 9468 5b8c 0b72 6566 6578 706c 6963 6974  .h[..refexplicit
-00000460: 9488 7568 2b68 4868 1e4b 0468 1d68 2c68  ..uh+hHh.K.h.h,h
-00000470: 1b68 4068 1c68 0375 6268 168c 0f20 636c  .h@h.h.ubh... cl
-00000480: 6173 7320 696e 7374 6561 642e 9485 9481  ass instead.....
-00000490: 947d 9428 681b 6840 681c 6803 681d 4e68  .}.(h.h@h.h.h.Nh
-000004a0: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
-000004b0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-000004c0: 2b68 3e68 1e4b 0468 1d68 2c68 1b68 2d68  +h>h.K.h.h,h.h-h
-000004d0: 1c68 0375 6265 681f 7d94 2868 215d 948c  .h.ubeh.}.(h!]..
-000004e0: 0c70 7265 7365 6e74 6174 696f 6e94 6168  .presentation.ah
-000004f0: 235d 9468 255d 948c 0c70 7265 7365 6e74  #].h%]...present
-00000500: 6174 696f 6e94 6168 275d 9468 295d 9475  ation.ah'].h)].u
-00000510: 682b 680a 681e 4b03 681d 682c 681b 680c  h+h.h.K.h.h,h.h.
-00000520: 681c 6803 7562 680b 2981 947d 9428 6805  h.h.ubh.)..}.(h.
-00000530: 6806 6807 5d94 2868 1029 8194 7d94 2868  h.h.].(h.)..}.(h
-00000540: 058c 0a44 6566 696e 6974 696f 6e94 6807  ...Definition.h.
-00000550: 5d94 6816 8c0a 4465 6669 6e69 7469 6f6e  ].h...Definition
-00000560: 9485 9481 947d 9428 681b 6883 681c 6803  .....}.(h.h.h.h.
-00000570: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00000580: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00000590: 5d94 7568 2b68 0f68 1e4b 0668 1d68 2c68  ].uh+h.h.K.h.h,h
-000005a0: 1b68 8068 1c68 0375 6268 098c 0d6c 6974  .h.h.h.ubh...lit
-000005b0: 6572 616c 5f62 6c6f 636b 9493 9429 8194  eral_block...)..
-000005c0: 7d94 2868 058c 5f63 6c61 7373 206d 7a44  }.(h.._class mzD
-000005d0: 6174 6158 4d4c 5374 7275 6374 2842 6173  ataXMLStruct(Bas
-000005e0: 654d 6f64 656c 293a 0a20 2020 206d 6574  eModel):.    met
-000005f0: 6164 6174 6120 3a20 6469 6374 0a20 2020  adata : dict.   
-00000600: 2074 696d 6573 203a 206c 6973 745b 666c   times : list[fl
-00000610: 6f61 745d 0a20 2020 2073 6572 6965 7320  oat].    series 
-00000620: 3a20 416e 790a 9468 075d 9468 168c 5f63  : Any..h.].h.._c
-00000630: 6c61 7373 206d 7a44 6174 6158 4d4c 5374  lass mzDataXMLSt
-00000640: 7275 6374 2842 6173 654d 6f64 656c 293a  ruct(BaseModel):
-00000650: 0a20 2020 206d 6574 6164 6174 6120 3a20  .    metadata : 
-00000660: 6469 6374 0a20 2020 2074 696d 6573 203a  dict.    times :
-00000670: 206c 6973 745b 666c 6f61 745d 0a20 2020   list[float].   
-00000680: 2073 6572 6965 7320 3a20 416e 790a 9485   series : Any...
-00000690: 9481 947d 9468 1b68 9373 6261 681f 7d94  ...}.h.h.sbah.}.
-000006a0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-000006b0: 9468 295d 948c 086c 616e 6775 6167 6594  .h)]...language.
-000006c0: 8c06 7079 7468 6f6e 948c 0978 6d6c 3a73  ..python...xml:s
-000006d0: 7061 6365 948c 0870 7265 7365 7276 6594  pace...preserve.
-000006e0: 7568 2b68 9168 1d68 2c68 1e4b 0768 1b68  uh+h.h.h,h.K.h.h
-000006f0: 8068 1c68 0375 6265 681f 7d94 2868 215d  .h.h.ubeh.}.(h!]
-00000700: 948c 0a64 6566 696e 6974 696f 6e94 6168  ...definition.ah
-00000710: 235d 9468 255d 948c 0a64 6566 696e 6974  #].h%]...definit
-00000720: 696f 6e94 6168 275d 9468 295d 9475 682b  ion.ah'].h)].uh+
-00000730: 680a 681e 4b06 681d 682c 681b 680c 681c  h.h.K.h.h,h.h.h.
-00000740: 6803 7562 680b 2981 947d 9428 6805 6806  h.ubh.)..}.(h.h.
-00000750: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
-00000760: 0a48 6f77 2074 6f20 7573 6594 6807 5d94  .How to use.h.].
-00000770: 6816 8c0a 486f 7720 746f 2075 7365 9485  h...How to use..
-00000780: 9481 947d 9428 681b 68b0 681c 6803 681d  ...}.(h.h.h.h.h.
-00000790: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-000007a0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000007b0: 7568 2b68 0f68 1e4b 0d68 1d68 2c68 1b68  uh+h.h.K.h.h,h.h
-000007c0: ad68 1c68 0375 6268 9229 8194 7d94 2868  .h.h.ubh.)..}.(h
-000007d0: 058c 6176 616c 7565 203d 206d 7a44 6174  ..avalue = mzDat
-000007e0: 6158 4d4c 5374 7275 6374 280a 2020 2020  aXMLStruct(.    
-000007f0: 6d65 7461 6461 7461 203d 2073 6f6d 6544  metadata = someD
-00000800: 6963 742c 0a20 2020 2074 696d 6573 203d  ict,.    times =
-00000810: 206c 6973 744f 6654 696d 6573 2c0a 2020   listOfTimes,.  
-00000820: 2020 7365 7269 6573 203d 2073 6572 6965    series = serie
-00000830: 730a 290a 9468 075d 9468 168c 6176 616c  s.)..h.].h..aval
-00000840: 7565 203d 206d 7a44 6174 6158 4d4c 5374  ue = mzDataXMLSt
-00000850: 7275 6374 280a 2020 2020 6d65 7461 6461  ruct(.    metada
-00000860: 7461 203d 2073 6f6d 6544 6963 742c 0a20  ta = someDict,. 
-00000870: 2020 2074 696d 6573 203d 206c 6973 744f     times = listO
-00000880: 6654 696d 6573 2c0a 2020 2020 7365 7269  fTimes,.    seri
-00000890: 6573 203d 2073 6572 6965 730a 290a 9485  es = series.)...
-000008a0: 9481 947d 9468 1b68 be73 6261 681f 7d94  ...}.h.h.sbah.}.
-000008b0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-000008c0: 9468 295d 948c 086c 616e 6775 6167 6594  .h)]...language.
-000008d0: 8c06 7079 7468 6f6e 9468 a368 a475 682b  ..python.h.h.uh+
-000008e0: 6891 681d 682c 681e 4b0e 681b 68ad 681c  h.h.h,h.K.h.h.h.
-000008f0: 6803 7562 6568 1f7d 9428 6821 5d94 8c0a  h.ubeh.}.(h!]...
-00000900: 686f 772d 746f 2d75 7365 9461 6823 5d94  how-to-use.ah#].
-00000910: 6825 5d94 8c0a 686f 7720 746f 2075 7365  h%]...how to use
-00000920: 9461 6827 5d94 6829 5d94 7568 2b68 0a68  .ah'].h)].uh+h.h
-00000930: 1e4b 0d68 1d68 2c68 1b68 0c68 1c68 0375  .K.h.h,h.h.h.h.u
-00000940: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
-00000950: 9428 6810 2981 947d 9428 6805 8c09 4675  .(h.)..}.(h...Fu
-00000960: 6e63 7469 6f6e 7394 6807 5d94 6816 8c09  nctions.h.].h...
-00000970: 4675 6e63 7469 6f6e 7394 8594 8194 7d94  Functions.....}.
-00000980: 2868 1b68 d968 1c68 0368 1d4e 681e 4e75  (h.h.h.h.h.Nh.Nu
-00000990: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-000009a0: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
-000009b0: 681e 4b16 681d 682c 681b 68d6 681c 6803  h.K.h.h,h.h.h.h.
-000009c0: 7562 683f 2981 947d 9428 6805 8c04 4e6f  ubh?)..}.(h...No
-000009d0: 6e65 9468 075d 9468 168c 044e 6f6e 6594  ne.h.].h...None.
-000009e0: 8594 8194 7d94 2868 1b68 e768 1c68 0368  ....}.(h.h.h.h.h
-000009f0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00000a00: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00000a10: 9475 682b 683e 681e 4b17 681d 682c 681b  .uh+h>h.K.h.h,h.
-00000a20: 68d6 681c 6803 7562 6568 1f7d 9428 6821  h.h.h.ubeh.}.(h!
-00000a30: 5d94 8c09 6675 6e63 7469 6f6e 7394 6168  ]...functions.ah
-00000a40: 235d 9468 255d 948c 0966 756e 6374 696f  #].h%]...functio
-00000a50: 6e73 9461 6827 5d94 6829 5d94 7568 2b68  ns.ah'].h)].uh+h
-00000a60: 0a68 1e4b 1668 1d68 2c68 1b68 0c68 1c68  .h.K.h.h,h.h.h.h
-00000a70: 0375 6268 0b29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
-00000a80: 075d 9428 6810 2981 947d 9428 6805 8c05  .].(h.)..}.(h...
-00000a90: 4e6f 7465 7394 6807 5d94 6816 8c05 4e6f  Notes.h.].h...No
-00000aa0: 7465 7394 8594 8194 7d94 2868 1b6a 0001  tes.....}.(h.j..
-00000ab0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00000ac0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00000ad0: 6827 5d94 6829 5d94 7568 2b68 0f68 1e4b  h'].h)].uh+h.h.K
-00000ae0: 1968 1d68 2c68 1b68 fd68 1c68 0375 6268  .h.h,h.h.h.h.ubh
-00000af0: 3f29 8194 7d94 2868 058c 9f54 6869 7320  ?)..}.(h...This 
-00000b00: 6973 2061 6e20 5f5f 696e 7465 726e 616c  is an __internal
-00000b10: 5f5f 2063 6c61 7373 2c20 6974 2073 686f  __ class, it sho
-00000b20: 756c 646e 2774 2062 6520 7573 6564 2074  uldn't be used t
-00000b30: 6f20 7374 6f72 6520 6d7a 2076 616c 7565  o store mz value
-00000b40: 732e 2054 6869 7320 636c 6173 7320 6973  s. This class is
-00000b50: 2061 7574 6f6d 6174 6963 616c 6c79 2070   automatically p
-00000b60: 6f70 756c 6174 6564 2077 6865 6e20 7061  opulated when pa
-00000b70: 7273 696e 6720 6120 602e 6d7a 4461 7461  rsing a `.mzData
-00000b80: 2e78 6d6c 6020 6669 6c65 2061 6e64 2069  .xml` file and i
-00000b90: 7320 7072 6976 6174 652e 9468 075d 9428  s private..h.].(
-00000ba0: 6816 8c0b 5468 6973 2069 7320 616e 2094  h...This is an .
-00000bb0: 8594 8194 7d94 2868 1b6a 0e01 0000 681c  ....}.(h.j....h.
-00000bc0: 6803 681d 4e68 1e4e 7562 6809 8c06 7374  h.h.Nh.Nubh...st
-00000bd0: 726f 6e67 9493 9429 8194 7d94 2868 058c  rong...)..}.(h..
-00000be0: 0869 6e74 6572 6e61 6c94 6807 5d94 6816  .internal.h.].h.
-00000bf0: 8c08 696e 7465 726e 616c 9485 9481 947d  ..internal.....}
-00000c00: 9428 681b 6a18 0100 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00000c10: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00000c20: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00000c30: 682b 6a16 0100 0068 1e4b 1a68 1d68 2c68  h+j....h.K.h.h,h
-00000c40: 1b6a 0e01 0000 681c 6803 7562 6816 8c68  .j....h.h.ubh..h
-00000c50: 2063 6c61 7373 2c20 6974 2073 686f 756c   class, it shoul
-00000c60: 646e e280 9974 2062 6520 7573 6564 2074  dn...t be used t
-00000c70: 6f20 7374 6f72 6520 6d7a 2076 616c 7565  o store mz value
-00000c80: 732e 2054 6869 7320 636c 6173 7320 6973  s. This class is
-00000c90: 2061 7574 6f6d 6174 6963 616c 6c79 2070   automatically p
-00000ca0: 6f70 756c 6174 6564 2077 6865 6e20 7061  opulated when pa
-00000cb0: 7273 696e 6720 6120 9485 9481 947d 9428  rsing a .....}.(
-00000cc0: 681b 6a0e 0100 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00000cd0: 4e75 6268 098c 076c 6974 6572 616c 9493  Nubh...literal..
-00000ce0: 9429 8194 7d94 2868 058c 0b2e 6d7a 4461  .)..}.(h....mzDa
-00000cf0: 7461 2e78 6d6c 9468 075d 9468 168c 0b2e  ta.xml.h.].h....
-00000d00: 6d7a 4461 7461 2e78 6d6c 9485 9481 947d  mzData.xml.....}
-00000d10: 9428 681b 6a2c 0100 0068 1c68 0368 1d4e  .(h.j,...h.h.h.N
-00000d20: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00000d30: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00000d40: 682b 6a2a 0100 0068 1e4b 1a68 1d68 2c68  h+j*...h.K.h.h,h
-00000d50: 1b6a 0e01 0000 681c 6803 7562 6816 8c15  .j....h.h.ubh...
-00000d60: 2066 696c 6520 616e 6420 6973 2070 7269   file and is pri
-00000d70: 7661 7465 2e94 8594 8194 7d94 2868 1b6a  vate......}.(h.j
-00000d80: 0e01 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00000d90: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00000da0: 5d94 6827 5d94 6829 5d94 7568 2b68 3e68  ].h'].h)].uh+h>h
-00000db0: 1e4b 1a68 1d68 2c68 1b68 fd68 1c68 0375  .K.h.h,h.h.h.h.u
-00000dc0: 6268 3f29 8194 7d94 2868 058c 5143 6f6e  bh?)..}.(h..QCon
-00000dd0: 7369 6465 7220 7573 696e 6720 5b6d 7a44  sider using [mzD
-00000de0: 6174 615d 286d 7a44 6174 612e 6d64 2920  ata](mzData.md) 
-00000df0: 636c 6173 7320 746f 2073 746f 7265 2079  class to store y
-00000e00: 6f75 7220 6d7a 2061 6e64 2069 6e74 656e  our mz and inten
-00000e10: 7369 7469 6573 2076 616c 7565 732e 9468  sities values..h
-00000e20: 075d 9428 6816 8c0f 436f 6e73 6964 6572  .].(h...Consider
-00000e30: 2075 7369 6e67 2094 8594 8194 7d94 2868   using .....}.(h
-00000e40: 1b6a 4401 0000 681c 6803 681d 4e68 1e4e  .jD...h.h.h.Nh.N
-00000e50: 7562 6849 2981 947d 9428 6805 6806 6807  ubhI)..}.(h.h.h.
-00000e60: 5d94 684e 2981 947d 9428 6805 8c06 6d7a  ].hN)..}.(h...mz
-00000e70: 4461 7461 9468 075d 9468 168c 066d 7a44  Data.h.].h...mzD
-00000e80: 6174 6194 8594 8194 7d94 2868 1b6a 4f01  ata.....}.(h.jO.
-00000e90: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00000ea0: 1f7d 9428 6821 5d94 6823 5d94 2868 5a68  .}.(h!].h#].(hZh
-00000eb0: 5b65 6825 5d94 6827 5d94 6829 5d94 7568  [eh%].h'].h)].uh
-00000ec0: 2b68 4d68 1b6a 4c01 0000 681c 6803 681d  +hMh.jL...h.h.h.
-00000ed0: 682c 681e 4b00 7562 6168 1f7d 9428 6821  h,h.K.ubah.}.(h!
-00000ee0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00000ef0: 5d94 8c09 7265 6664 6f6d 6169 6e94 6866  ]...refdomain.hf
-00000f00: 8c09 7265 6674 6172 6765 7494 8c06 6d7a  ..reftarget...mz
-00000f10: 4461 7461 948c 0b72 6566 7461 7267 6574  Data...reftarget
-00000f20: 6964 944e 8c06 7265 6664 6f63 9468 6b8c  id.N..refdoc.hk.
-00000f30: 0772 6566 7479 7065 9468 5b8c 0b72 6566  .reftype.h[..ref
-00000f40: 6578 706c 6963 6974 9488 7568 2b68 4868  explicit..uh+hHh
-00000f50: 1e4b 1c68 1d68 2c68 1b6a 4401 0000 681c  .K.h.h,h.jD...h.
-00000f60: 6803 7562 6816 8c2f 2063 6c61 7373 2074  h.ubh../ class t
-00000f70: 6f20 7374 6f72 6520 796f 7572 206d 7a20  o store your mz 
-00000f80: 616e 6420 696e 7465 6e73 6974 6965 7320  and intensities 
-00000f90: 7661 6c75 6573 2e94 8594 8194 7d94 2868  values......}.(h
-00000fa0: 1b6a 4401 0000 681c 6803 681d 4e68 1e4e  .jD...h.h.h.Nh.N
-00000fb0: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-00000fc0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-00000fd0: 3e68 1e4b 1c68 1d68 2c68 1b68 fd68 1c68  >h.K.h.h,h.h.h.h
-00000fe0: 0375 6265 681f 7d94 2868 215d 948c 056e  .ubeh.}.(h!]...n
-00000ff0: 6f74 6573 9461 6823 5d94 6825 5d94 8c05  otes.ah#].h%]...
-00001000: 6e6f 7465 7394 6168 275d 9468 295d 9475  notes.ah'].h)].u
-00001010: 682b 680a 681e 4b19 681d 682c 681b 680c  h+h.h.K.h.h,h.h.
-00001020: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
-00001030: 8c0f 6d7a 6461 7461 786d 6c73 7472 7563  ..mzdataxmlstruc
-00001040: 7494 6168 235d 9468 255d 948c 0f6d 7a64  t.ah#].h%]...mzd
-00001050: 6174 6178 6d6c 7374 7275 6374 9461 6827  ataxmlstruct.ah'
-00001060: 5d94 6829 5d94 7568 2b68 0a68 1e4b 0168  ].h)].uh+h.h.K.h
-00001070: 1d68 2c68 1b68 0368 1c68 0375 6261 681f  .h,h.h.h.h.ubah.
-00001080: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00001090: 275d 9468 295d 948c 0673 6f75 7263 6594  '].h)]...source.
-000010a0: 682c 8c14 7472 616e 736c 6174 696f 6e5f  h,..translation_
-000010b0: 7072 6f67 7265 7373 947d 9428 8c05 746f  progress.}.(..to
-000010c0: 7461 6c94 4b00 8c0a 7472 616e 736c 6174  tal.K...translat
-000010d0: 6564 944b 0075 7568 2b68 018c 0e63 7572  ed.K.uuh+h...cur
-000010e0: 7265 6e74 5f73 6f75 7263 6594 4e8c 0c63  rent_source.N..c
-000010f0: 7572 7265 6e74 5f6c 696e 6594 4e8c 0873  urrent_line.N..s
-00001100: 6574 7469 6e67 7394 8c11 646f 6375 7469  ettings...docuti
-00001110: 6c73 2e66 726f 6e74 656e 6494 8c06 5661  ls.frontend...Va
-00001120: 6c75 6573 9493 9429 8194 7d94 2868 0f4e  lues...)..}.(h.N
-00001130: 8c09 6765 6e65 7261 746f 7294 4e8c 0964  ..generator.N..d
-00001140: 6174 6573 7461 6d70 944e 8c0b 736f 7572  atestamp.N..sour
-00001150: 6365 5f6c 696e 6b94 4e8c 0a73 6f75 7263  ce_link.N..sourc
-00001160: 655f 7572 6c94 4e8c 0d74 6f63 5f62 6163  e_url.N..toc_bac
-00001170: 6b6c 696e 6b73 948c 0565 6e74 7279 948c  klinks...entry..
-00001180: 1266 6f6f 746e 6f74 655f 6261 636b 6c69  .footnote_backli
-00001190: 6e6b 7394 4b01 8c0d 7365 6374 6e75 6d5f  nks.K...sectnum_
-000011a0: 7866 6f72 6d94 4b01 8c0e 7374 7269 705f  xform.K...strip_
-000011b0: 636f 6d6d 656e 7473 944e 8c1b 7374 7269  comments.N..stri
-000011c0: 705f 656c 656d 656e 7473 5f77 6974 685f  p_elements_with_
-000011d0: 636c 6173 7365 7394 4e8c 0d73 7472 6970  classes.N..strip
-000011e0: 5f63 6c61 7373 6573 944e 8c0c 7265 706f  _classes.N..repo
-000011f0: 7274 5f6c 6576 656c 944b 028c 0a68 616c  rt_level.K...hal
-00001200: 745f 6c65 7665 6c94 4b05 8c11 6578 6974  t_level.K...exit
-00001210: 5f73 7461 7475 735f 6c65 7665 6c94 4b05  _status_level.K.
-00001220: 8c05 6465 6275 6794 4e8c 0e77 6172 6e69  ..debug.N..warni
-00001230: 6e67 5f73 7472 6561 6d94 4e8c 0974 7261  ng_stream.N..tra
-00001240: 6365 6261 636b 9488 8c0e 696e 7075 745f  ceback....input_
-00001250: 656e 636f 6469 6e67 948c 0975 7466 2d38  encoding...utf-8
-00001260: 2d73 6967 948c 1c69 6e70 7574 5f65 6e63  -sig...input_enc
-00001270: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-00001280: 6c65 7294 8c06 7374 7269 6374 948c 0f6f  ler...strict...o
-00001290: 7574 7075 745f 656e 636f 6469 6e67 948c  utput_encoding..
-000012a0: 0575 7466 2d38 948c 1d6f 7574 7075 745f  .utf-8...output_
-000012b0: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
-000012c0: 616e 646c 6572 946a ab01 0000 8c0e 6572  andler.j......er
-000012d0: 726f 725f 656e 636f 6469 6e67 948c 0575  ror_encoding...u
-000012e0: 7466 2d38 948c 1c65 7272 6f72 5f65 6e63  tf-8...error_enc
-000012f0: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-00001300: 6c65 7294 8c10 6261 636b 736c 6173 6872  ler...backslashr
-00001310: 6570 6c61 6365 948c 0d6c 616e 6775 6167  eplace...languag
-00001320: 655f 636f 6465 948c 0265 6e94 8c13 7265  e_code...en...re
-00001330: 636f 7264 5f64 6570 656e 6465 6e63 6965  cord_dependencie
-00001340: 7394 4e8c 0663 6f6e 6669 6794 4e8c 0969  s.N..config.N..i
-00001350: 645f 7072 6566 6978 9468 068c 0e61 7574  d_prefix.h...aut
-00001360: 6f5f 6964 5f70 7265 6669 7894 8c02 6964  o_id_prefix...id
-00001370: 948c 0d64 756d 705f 7365 7474 696e 6773  ...dump_settings
-00001380: 944e 8c0e 6475 6d70 5f69 6e74 6572 6e61  .N..dump_interna
-00001390: 6c73 944e 8c0f 6475 6d70 5f74 7261 6e73  ls.N..dump_trans
-000013a0: 666f 726d 7394 4e8c 0f64 756d 705f 7073  forms.N..dump_ps
-000013b0: 6575 646f 5f78 6d6c 944e 8c10 6578 706f  eudo_xml.N..expo
-000013c0: 7365 5f69 6e74 6572 6e61 6c73 944e 8c0e  se_internals.N..
-000013d0: 7374 7269 6374 5f76 6973 6974 6f72 944e  strict_visitor.N
-000013e0: 8c0f 5f64 6973 6162 6c65 5f63 6f6e 6669  .._disable_confi
-000013f0: 6794 4e8c 075f 736f 7572 6365 9468 2c8c  g.N.._source.h,.
-00001400: 0c5f 6465 7374 696e 6174 696f 6e94 4e8c  ._destination.N.
-00001410: 0d5f 636f 6e66 6967 5f66 696c 6573 945d  ._config_files.]
-00001420: 948c 1666 696c 655f 696e 7365 7274 696f  ...file_insertio
-00001430: 6e5f 656e 6162 6c65 6494 888c 0b72 6177  n_enabled....raw
-00001440: 5f65 6e61 626c 6564 944b 018c 116c 696e  _enabled.K...lin
-00001450: 655f 6c65 6e67 7468 5f6c 696d 6974 944d  e_length_limit.M
-00001460: 1027 8c0e 7065 705f 7265 6665 7265 6e63  .'..pep_referenc
-00001470: 6573 944e 8c0c 7065 705f 6261 7365 5f75  es.N..pep_base_u
-00001480: 726c 948c 1868 7474 7073 3a2f 2f70 6570  rl...https://pep
-00001490: 732e 7079 7468 6f6e 2e6f 7267 2f94 8c15  s.python.org/...
-000014a0: 7065 705f 6669 6c65 5f75 726c 5f74 656d  pep_file_url_tem
-000014b0: 706c 6174 6594 8c08 7065 702d 2530 3464  plate...pep-%04d
-000014c0: 948c 0e72 6663 5f72 6566 6572 656e 6365  ...rfc_reference
-000014d0: 7394 4e8c 0c72 6663 5f62 6173 655f 7572  s.N..rfc_base_ur
-000014e0: 6c94 8c26 6874 7470 733a 2f2f 6461 7461  l..&https://data
-000014f0: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
-00001500: 2f64 6f63 2f68 746d 6c2f 948c 0974 6162  /doc/html/...tab
-00001510: 5f77 6964 7468 944b 088c 1d74 7269 6d5f  _width.K...trim_
-00001520: 666f 6f74 6e6f 7465 5f72 6566 6572 656e  footnote_referen
-00001530: 6365 5f73 7061 6365 9489 8c10 7379 6e74  ce_space....synt
-00001540: 6178 5f68 6967 686c 6967 6874 948c 046c  ax_highlight...l
-00001550: 6f6e 6794 8c0c 736d 6172 745f 7175 6f74  ong...smart_quot
-00001560: 6573 9488 8c13 736d 6172 7471 756f 7465  es....smartquote
-00001570: 735f 6c6f 6361 6c65 7394 5d94 8c1d 6368  s_locales.]...ch
-00001580: 6172 6163 7465 725f 6c65 7665 6c5f 696e  aracter_level_in
-00001590: 6c69 6e65 5f6d 6172 6b75 7094 898c 0e64  line_markup....d
-000015a0: 6f63 7469 746c 655f 7866 6f72 6d94 898c  octitle_xform...
-000015b0: 0d64 6f63 696e 666f 5f78 666f 726d 944b  .docinfo_xform.K
-000015c0: 018c 1273 6563 7473 7562 7469 746c 655f  ...sectsubtitle_
-000015d0: 7866 6f72 6d94 898c 0d69 6d61 6765 5f6c  xform....image_l
-000015e0: 6f61 6469 6e67 948c 046c 696e 6b94 8c10  oading...link...
-000015f0: 656d 6265 645f 7374 796c 6573 6865 6574  embed_stylesheet
-00001600: 9489 8c15 636c 6f61 6b5f 656d 6169 6c5f  ....cloak_email_
-00001610: 6164 6472 6573 7365 7394 888c 1173 6563  addresses....sec
-00001620: 7469 6f6e 5f73 656c 665f 6c69 6e6b 9489  tion_self_link..
-00001630: 8c03 656e 7694 4e75 628c 0872 6570 6f72  ..env.Nub..repor
-00001640: 7465 7294 4e8c 1069 6e64 6972 6563 745f  ter.N..indirect_
-00001650: 7461 7267 6574 7394 5d94 8c11 7375 6273  targets.]...subs
-00001660: 7469 7475 7469 6f6e 5f64 6566 7394 7d94  titution_defs.}.
-00001670: 288c 0f77 6f72 6463 6f75 6e74 2d77 6f72  (..wordcount-wor
-00001680: 6473 9468 098c 1773 7562 7374 6974 7574  ds.h...substitut
-00001690: 696f 6e5f 6465 6669 6e69 7469 6f6e 9493  ion_definition..
-000016a0: 9429 8194 7d94 2868 058c 0235 3894 6807  .)..}.(h...58.h.
-000016b0: 5d94 6816 8c02 3538 9485 9481 947d 9468  ].h...58.....}.h
-000016c0: 1b6a e901 0000 7362 6168 1f7d 9428 6821  .j....sbah.}.(h!
-000016d0: 5d94 6823 5d94 6825 5d94 8c0f 776f 7264  ].h#].h%]...word
-000016e0: 636f 756e 742d 776f 7264 7394 6168 275d  count-words.ah']
-000016f0: 9468 295d 9475 682b 6ae7 0100 0068 1d68  .h)].uh+j....h.h
-00001700: 2c75 628c 1177 6f72 6463 6f75 6e74 2d6d  ,ub..wordcount-m
-00001710: 696e 7574 6573 946a e801 0000 2981 947d  inutes.j....)..}
-00001720: 9428 6805 8c01 3094 6807 5d94 6816 8c01  .(h...0.h.].h...
-00001730: 3094 8594 8194 7d94 681b 6af9 0100 0073  0.....}.h.j....s
-00001740: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00001750: 255d 948c 1177 6f72 6463 6f75 6e74 2d6d  %]...wordcount-m
-00001760: 696e 7574 6573 9461 6827 5d94 6829 5d94  inutes.ah'].h)].
-00001770: 7568 2b6a e701 0000 681d 682c 7562 758c  uh+j....h.h,ubu.
-00001780: 1273 7562 7374 6974 7574 696f 6e5f 6e61  .substitution_na
-00001790: 6d65 7394 7d94 288c 0f77 6f72 6463 6f75  mes.}.(..wordcou
-000017a0: 6e74 2d77 6f72 6473 946a e601 0000 8c11  nt-words.j......
-000017b0: 776f 7264 636f 756e 742d 6d69 6e75 7465  wordcount-minute
-000017c0: 7394 6af8 0100 0075 8c08 7265 666e 616d  s.j....u..refnam
-000017d0: 6573 947d 948c 0672 6566 6964 7394 7d94  es.}...refids.}.
-000017e0: 8c07 6e61 6d65 6964 7394 7d94 286a 8101  ..nameids.}.(j..
-000017f0: 0000 6a7e 0100 0068 7d68 7a68 aa68 a768  ..j~...h}hzh.h.h
-00001800: d368 d068 fa68 f76a 7901 0000 6a76 0100  .h.h.h.jy...jv..
-00001810: 0075 8c09 6e61 6d65 7479 7065 7394 7d94  .u..nametypes.}.
-00001820: 286a 8101 0000 8968 7d89 68aa 8968 d389  (j.....h}.h..h..
-00001830: 68fa 896a 7901 0000 8975 6821 7d94 286a  h..jy....uh!}.(j
-00001840: 7e01 0000 680c 687a 682d 68a7 6880 68d0  ~...h.hzh-h.h.h.
-00001850: 68ad 68f7 68d6 6a76 0100 0068 fd75 8c0d  h.h.h.jv...h.u..
-00001860: 666f 6f74 6e6f 7465 5f72 6566 7394 7d94  footnote_refs.}.
-00001870: 8c0d 6369 7461 7469 6f6e 5f72 6566 7394  ..citation_refs.
-00001880: 7d94 8c0d 6175 746f 666f 6f74 6e6f 7465  }...autofootnote
-00001890: 7394 5d94 8c11 6175 746f 666f 6f74 6e6f  s.]...autofootno
-000018a0: 7465 5f72 6566 7394 5d94 8c10 7379 6d62  te_refs.]...symb
-000018b0: 6f6c 5f66 6f6f 746e 6f74 6573 945d 948c  ol_footnotes.]..
-000018c0: 1473 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
-000018d0: 5f72 6566 7394 5d94 8c09 666f 6f74 6e6f  _refs.]...footno
-000018e0: 7465 7394 5d94 8c09 6369 7461 7469 6f6e  tes.]...citation
-000018f0: 7394 5d94 8c12 6175 746f 666f 6f74 6e6f  s.]...autofootno
-00001900: 7465 5f73 7461 7274 944b 018c 1573 796d  te_start.K...sym
-00001910: 626f 6c5f 666f 6f74 6e6f 7465 5f73 7461  bol_footnote_sta
-00001920: 7274 944b 008c 0a69 645f 636f 756e 7465  rt.K...id_counte
-00001930: 7294 8c0b 636f 6c6c 6563 7469 6f6e 7394  r...collections.
-00001940: 8c07 436f 756e 7465 7294 9394 7d94 8594  ..Counter...}...
-00001950: 5294 8c0e 7061 7273 655f 6d65 7373 6167  R...parse_messag
-00001960: 6573 945d 948c 1274 7261 6e73 666f 726d  es.]...transform
-00001970: 5f6d 6573 7361 6765 7394 5d94 8c0b 7472  _messages.]...tr
-00001980: 616e 7366 6f72 6d65 7294 4e8c 0b69 6e63  ansformer.N..inc
-00001990: 6c75 6465 5f6c 6f67 945d 948c 0a64 6563  lude_log.]...dec
-000019a0: 6f72 6174 696f 6e94 4e68 1c68 038c 0a6d  oration.Nh.h...m
-000019b0: 7973 745f 736c 7567 7394 7d94 7562 2e    yst_slugs.}.ub.
+00000080: 6594 9394 2981 947d 9428 6805 8c11 6d7a  e...)..}.(h...mz
+00000090: 6461 7461 326d 6174 2d76 6572 6966 7994  data2mat-verify.
+000000a0: 6807 5d94 6809 8c04 5465 7874 9493 948c  h.].h...Text....
+000000b0: 116d 7a64 6174 6132 6d61 742d 7665 7269  .mzdata2mat-veri
+000000c0: 6679 9485 9481 947d 9428 8c06 7061 7265  fy.....}.(..pare
+000000d0: 6e74 9468 118c 095f 646f 6375 6d65 6e74  nt.h..._document
+000000e0: 9468 038c 0673 6f75 7263 6594 4e8c 046c  .h...source.N..l
+000000f0: 696e 6594 4e75 6261 8c0a 6174 7472 6962  ine.Nuba..attrib
+00000100: 7574 6573 947d 9428 8c03 6964 7394 5d94  utes.}.(..ids.].
+00000110: 8c07 636c 6173 7365 7394 5d94 8c05 6e61  ..classes.]...na
+00000120: 6d65 7394 5d94 8c08 6475 706e 616d 6573  mes.]...dupnames
+00000130: 945d 948c 0862 6163 6b72 6566 7394 5d94  .]...backrefs.].
+00000140: 758c 0774 6167 6e61 6d65 9468 0f68 1e4b  u..tagname.h.h.K
+00000150: 0168 1d8c 6043 3a5c 5573 6572 735c 6d61  .h..`C:\Users\ma
+00000160: 7869 6d5c 4f6e 6544 7269 7665 5c44 6f63  xim\OneDrive\Doc
+00000170: 756d 656e 7473 5c50 7974 686f 6e5c 5061  uments\Python\Pa
+00000180: 636b 6167 6573 5c6d 7a44 6174 6158 4d4c  ckages\mzDataXML
+00000190: 324d 6174 5c64 6f63 735c 736f 7572 6365  2Mat\docs\source
+000001a0: 5c6d 7a64 6174 6132 6d61 742d 7665 7269  \mzdata2mat-veri
+000001b0: 6679 2e6d 6494 681b 680c 681c 6803 7562  fy.md.h.h.h.h.ub
+000001c0: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
+000001d0: 2868 1029 8194 7d94 2868 058c 0c50 7265  (h.)..}.(h...Pre
+000001e0: 7365 6e74 6174 696f 6e94 6807 5d94 6816  sentation.h.].h.
+000001f0: 8c0c 5072 6573 656e 7461 7469 6f6e 9485  ..Presentation..
+00000200: 9481 947d 9428 681b 6830 681c 6803 681d  ...}.(h.h0h.h.h.
+00000210: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00000220: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00000230: 7568 2b68 0f68 1e4b 0368 1d68 2c68 1b68  uh+h.h.K.h.h,h.h
+00000240: 2d68 1c68 0375 6268 098c 0970 6172 6167  -h.h.ubh...parag
+00000250: 7261 7068 9493 9429 8194 7d94 2868 058c  raph...)..}.(h..
+00000260: 9e54 6869 7320 6973 2061 2043 6f6d 6d61  .This is a Comma
+00000270: 6e64 204c 696e 6520 546f 6f6c 2028 434c  nd Line Tool (CL
+00000280: 4929 2077 6869 6368 2074 7269 6573 2074  I) which tries t
+00000290: 6f20 636f 6e76 6572 7420 616e 2065 7861  o convert an exa
+000002a0: 6d70 6c65 2066 696c 6520 696e 2074 6865  mple file in the
+000002b0: 2063 7572 7265 6e74 2064 6972 6563 746f   current directo
+000002c0: 7279 2e20 4974 2069 7320 6175 746f 6d61  ry. It is automa
+000002d0: 7469 6361 6c6c 7920 696e 7374 616c 6c65  tically installe
+000002e0: 6420 7768 656e 2079 6f75 2069 6e73 7461  d when you insta
+000002f0: 6c6c 2074 6865 2070 6163 6b61 6765 2e94  ll the package..
+00000300: 6807 5d94 6816 8c9e 5468 6973 2069 7320  h.].h...This is 
+00000310: 6120 436f 6d6d 616e 6420 4c69 6e65 2054  a Command Line T
+00000320: 6f6f 6c20 2843 4c49 2920 7768 6963 6820  ool (CLI) which 
+00000330: 7472 6965 7320 746f 2063 6f6e 7665 7274  tries to convert
+00000340: 2061 6e20 6578 616d 706c 6520 6669 6c65   an example file
+00000350: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+00000360: 6469 7265 6374 6f72 792e 2049 7420 6973  directory. It is
+00000370: 2061 7574 6f6d 6174 6963 616c 6c79 2069   automatically i
+00000380: 6e73 7461 6c6c 6564 2077 6865 6e20 796f  nstalled when yo
+00000390: 7520 696e 7374 616c 6c20 7468 6520 7061  u install the pa
+000003a0: 636b 6167 652e 9485 9481 947d 9428 681b  ckage......}.(h.
+000003b0: 6840 681c 6803 681d 4e68 1e4e 7562 6168  h@h.h.h.Nh.Nubah
+000003c0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000003d0: 6827 5d94 6829 5d94 7568 2b68 3e68 1e4b  h'].h)].uh+h>h.K
+000003e0: 0468 1d68 2c68 1b68 2d68 1c68 0375 6265  .h.h,h.h-h.h.ube
+000003f0: 681f 7d94 2868 215d 948c 0c70 7265 7365  h.}.(h!]...prese
+00000400: 6e74 6174 696f 6e94 6168 235d 9468 255d  ntation.ah#].h%]
+00000410: 948c 0c70 7265 7365 6e74 6174 696f 6e94  ...presentation.
+00000420: 6168 275d 9468 295d 9475 682b 680a 681e  ah'].h)].uh+h.h.
+00000430: 4b03 681d 682c 681b 680c 681c 6803 7562  K.h.h,h.h.h.h.ub
+00000440: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
+00000450: 2868 1029 8194 7d94 2868 058c 0d48 6f77  (h.)..}.(h...How
+00000460: 2074 6f20 7275 6e20 6974 9468 075d 9468   to run it.h.].h
+00000470: 168c 0d48 6f77 2074 6f20 7275 6e20 6974  ...How to run it
+00000480: 9485 9481 947d 9428 681b 6859 681c 6803  .....}.(h.hYh.h.
+00000490: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000004a0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000004b0: 5d94 7568 2b68 0f68 1e4b 0668 1d68 2c68  ].uh+h.h.K.h.h,h
+000004c0: 1b68 5668 1c68 0375 6268 3f29 8194 7d94  .hVh.h.ubh?)..}.
+000004d0: 2868 058c 6e49 7420 6973 2072 6561 6c6c  (h..nIt is reall
+000004e0: 7920 7369 6d70 6c65 2c20 746f 2072 756e  y simple, to run
+000004f0: 2069 742c 206f 7065 6e20 6120 7465 726d   it, open a term
+00000500: 696e 616c 2077 696e 646f 7720 696e 2061  inal window in a
+00000510: 6e79 2066 6f6c 6465 7220 796f 7520 7761  ny folder you wa
+00000520: 6e74 2061 6e64 2074 7970 6520 7468 6520  nt and type the 
+00000530: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+00000540: 6420 3a94 6807 5d94 6816 8c6e 4974 2069  d :.h.].h..nIt i
+00000550: 7320 7265 616c 6c79 2073 696d 706c 652c  s really simple,
+00000560: 2074 6f20 7275 6e20 6974 2c20 6f70 656e   to run it, open
+00000570: 2061 2074 6572 6d69 6e61 6c20 7769 6e64   a terminal wind
+00000580: 6f77 2069 6e20 616e 7920 666f 6c64 6572  ow in any folder
+00000590: 2079 6f75 2077 616e 7420 616e 6420 7479   you want and ty
+000005a0: 7065 2074 6865 2066 6f6c 6c6f 7769 6e67  pe the following
+000005b0: 2063 6f6d 6d61 6e64 203a 9485 9481 947d   command :.....}
+000005c0: 9428 681b 6867 681c 6803 681d 4e68 1e4e  .(h.hgh.h.h.Nh.N
+000005d0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+000005e0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+000005f0: 3e68 1e4b 0768 1d68 2c68 1b68 5668 1c68  >h.K.h.h,h.hVh.h
+00000600: 0375 6268 098c 0d6c 6974 6572 616c 5f62  .ubh...literal_b
+00000610: 6c6f 636b 9493 9429 8194 7d94 2868 058c  lock...)..}.(h..
+00000620: 1424 206d 7a64 6174 6132 6d61 742d 7665  .$ mzdata2mat-ve
+00000630: 7269 6679 0a94 6807 5d94 6816 8c14 2420  rify..h.].h...$ 
+00000640: 6d7a 6461 7461 326d 6174 2d76 6572 6966  mzdata2mat-verif
+00000650: 790a 9485 9481 947d 9468 1b68 7773 6261  y......}.h.hwsba
+00000660: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00000670: 9468 275d 9468 295d 948c 086c 616e 6775  .h'].h)]...langu
+00000680: 6167 6594 8c05 7368 656c 6c94 8c09 786d  age...shell...xm
+00000690: 6c3a 7370 6163 6594 8c08 7072 6573 6572  l:space...preser
+000006a0: 7665 9475 682b 6875 681d 682c 681e 4b08  ve.uh+huh.h,h.K.
+000006b0: 681b 6856 681c 6803 7562 683f 2981 947d  h.hVh.h.ubh?)..}
+000006c0: 9428 6805 8cfe 4966 2074 6865 2070 6163  .(h...If the pac
+000006d0: 6b61 6765 2069 7320 636f 7272 6563 746c  kage is correctl
+000006e0: 7920 696e 7374 616c 6c65 642c 2079 6f75  y installed, you
+000006f0: 2077 696c 6c20 7365 6520 736f 6d65 206c   will see some l
+00000700: 696e 6573 2062 6569 6e67 2070 7269 6e74  ines being print
+00000710: 6564 2069 6e20 7468 6520 7465 726d 696e  ed in the termin
+00000720: 616c 2e20 4966 2069 7420 6973 2074 6865  al. If it is the
+00000730: 2066 6972 7374 2074 696d 6520 796f 7520   first time you 
+00000740: 6172 6520 7275 6e6e 696e 6720 6974 2c20  are running it, 
+00000750: 736f 6d65 206a 6176 6173 6372 6970 7420  some javascript 
+00000760: 6465 7065 6e64 656e 6369 6573 2077 696c  dependencies wil
+00000770: 6c20 6265 2069 6e73 7461 6c6c 6564 206f  l be installed o
+00000780: 6e20 796f 7572 2073 7973 7465 6d2e 2057  n your system. W
+00000790: 6865 6e20 616c 6c20 6f66 2074 6869 7320  hen all of this 
+000007a0: 6973 2064 6f6e 652c 2079 6f75 2077 696c  is done, you wil
+000007b0: 6c20 6765 7420 7468 6973 206d 6573 7361  l get this messa
+000007c0: 6765 203a 9468 075d 9468 168c fe49 6620  ge :.h.].h...If 
+000007d0: 7468 6520 7061 636b 6167 6520 6973 2063  the package is c
+000007e0: 6f72 7265 6374 6c79 2069 6e73 7461 6c6c  orrectly install
+000007f0: 6564 2c20 796f 7520 7769 6c6c 2073 6565  ed, you will see
+00000800: 2073 6f6d 6520 6c69 6e65 7320 6265 696e   some lines bein
+00000810: 6720 7072 696e 7465 6420 696e 2074 6865  g printed in the
+00000820: 2074 6572 6d69 6e61 6c2e 2049 6620 6974   terminal. If it
+00000830: 2069 7320 7468 6520 6669 7273 7420 7469   is the first ti
+00000840: 6d65 2079 6f75 2061 7265 2072 756e 6e69  me you are runni
+00000850: 6e67 2069 742c 2073 6f6d 6520 6a61 7661  ng it, some java
+00000860: 7363 7269 7074 2064 6570 656e 6465 6e63  script dependenc
+00000870: 6965 7320 7769 6c6c 2062 6520 696e 7374  ies will be inst
+00000880: 616c 6c65 6420 6f6e 2079 6f75 7220 7379  alled on your sy
+00000890: 7374 656d 2e20 5768 656e 2061 6c6c 206f  stem. When all o
+000008a0: 6620 7468 6973 2069 7320 646f 6e65 2c20  f this is done, 
+000008b0: 796f 7520 7769 6c6c 2067 6574 2074 6869  you will get thi
+000008c0: 7320 6d65 7373 6167 6520 3a94 8594 8194  s message :.....
+000008d0: 7d94 2868 1b68 8968 1c68 0368 1d4e 681e  }.(h.h.h.h.h.Nh.
+000008e0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+000008f0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00000900: 683e 681e 4b0c 681d 682c 681b 6856 681c  h>h.K.h.h,h.hVh.
+00000910: 6803 7562 6876 2981 947d 9428 6805 8c1e  h.ubhv)..}.(h...
+00000920: 2420 6d7a 6461 7461 326d 6174 202d 2052  $ mzdata2mat - R
+00000930: 6561 6479 2074 6f20 7573 6520 210a 9468  eady to use !..h
+00000940: 075d 9468 168c 1e24 206d 7a64 6174 6132  .].h...$ mzdata2
+00000950: 6d61 7420 2d20 5265 6164 7920 746f 2075  mat - Ready to u
+00000960: 7365 2021 0a94 8594 8194 7d94 681b 6897  se !......}.h.h.
+00000970: 7362 6168 1f7d 9428 6821 5d94 6823 5d94  sbah.}.(h!].h#].
+00000980: 6825 5d94 6827 5d94 6829 5d94 8c08 6c61  h%].h'].h)]...la
+00000990: 6e67 7561 6765 948c 0573 6865 6c6c 9468  nguage...shell.h
+000009a0: 8768 8875 682b 6875 681d 682c 681e 4b0d  .h.uh+huh.h,h.K.
+000009b0: 681b 6856 681c 6803 7562 6568 1f7d 9428  h.hVh.h.ubeh.}.(
+000009c0: 6821 5d94 8c0d 686f 772d 746f 2d72 756e  h!]...how-to-run
+000009d0: 2d69 7494 6168 235d 9468 255d 948c 0d68  -it.ah#].h%]...h
+000009e0: 6f77 2074 6f20 7275 6e20 6974 9461 6827  ow to run it.ah'
+000009f0: 5d94 6829 5d94 7568 2b68 0a68 1e4b 0668  ].h)].uh+h.h.K.h
+00000a00: 1d68 2c68 1b68 0c68 1c68 0375 6268 0b29  .h,h.h.h.h.ubh.)
+00000a10: 8194 7d94 2868 0568 0668 075d 9428 6810  ..}.(h.h.h.].(h.
+00000a20: 2981 947d 9428 6805 8c0b 4966 2069 7420  )..}.(h...If it 
+00000a30: 6661 696c 7394 6807 5d94 6816 8c0b 4966  fails.h.].h...If
+00000a40: 2069 7420 6661 696c 7394 8594 8194 7d94   it fails.....}.
+00000a50: 2868 1b68 b268 1c68 0368 1d4e 681e 4e75  (h.h.h.h.h.Nh.Nu
+00000a60: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00000a70: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
+00000a80: 681e 4b11 681d 682c 681b 68af 681c 6803  h.K.h.h,h.h.h.h.
+00000a90: 7562 683f 2981 947d 9428 6805 583d 0100  ubh?)..}.(h.X=..
+00000aa0: 0049 6620 796f 7520 6765 7420 616e 2065  .If you get an e
+00000ab0: 7272 6f72 206d 6573 7361 6765 2c20 6974  rror message, it
+00000ac0: 2070 726f 6261 626c 7920 6d65 616e 7320   probably means 
+00000ad0: 7468 6174 2079 6f75 2064 6f6e 2774 2068  that you don't h
+00000ae0: 6176 6520 5f5f 6e6f 6465 2e6a 735f 5f20  ave __node.js__ 
+00000af0: 696e 7374 616c 6c65 6420 6f6e 2079 6f75  installed on you
+00000b00: 7220 636f 6d70 7574 6572 2e20 596f 7520  r computer. You 
+00000b10: 6361 6e20 6765 7420 6974 2066 6f72 2066  can get it for f
+00000b20: 7265 6520 6174 205b 6e6f 6465 6a73 2e6f  ree at [nodejs.o
+00000b30: 7267 5d28 6874 7470 733a 2f2f 6e6f 6465  rg](https://node
+00000b40: 6a73 2e6f 7267 2f65 6e2f 292e 2049 6620  js.org/en/). If 
+00000b50: 796f 7520 7374 696c 6c20 6861 7665 2061  you still have a
+00000b60: 6e20 6572 726f 722c 206f 7065 6e20 6120  n error, open a 
+00000b70: 6e65 7720 6973 7375 6520 6f6e 205b 4769  new issue on [Gi
+00000b80: 7448 7562 5d28 6874 7470 733a 2f2f 6769  tHub](https://gi
+00000b90: 7468 7562 2e63 6f6d 2f4d 6178 696d 654c  thub.com/MaximeL
+00000ba0: 654d 6167 6963 6965 6e2f 6d7a 6461 7461  eMagicien/mzdata
+00000bb0: 326d 6174 2f69 7373 7565 7329 2c20 7765  2mat/issues), we
+00000bc0: 2077 696c 6c20 6265 2068 6170 7079 2074   will be happy t
+00000bd0: 6f20 616e 7377 6572 2079 6f75 2021 9468  o answer you !.h
+00000be0: 075d 9428 6816 8c45 4966 2079 6f75 2067  .].(h..EIf you g
+00000bf0: 6574 2061 6e20 6572 726f 7220 6d65 7373  et an error mess
+00000c00: 6167 652c 2069 7420 7072 6f62 6162 6c79  age, it probably
+00000c10: 206d 6561 6e73 2074 6861 7420 796f 7520   means that you 
+00000c20: 646f 6ee2 8099 7420 6861 7665 2094 8594  don...t have ...
+00000c30: 8194 7d94 2868 1b68 c068 1c68 0368 1d4e  ..}.(h.h.h.h.h.N
+00000c40: 681e 4e75 6268 098c 0673 7472 6f6e 6794  h.Nubh...strong.
+00000c50: 9394 2981 947d 9428 6805 8c07 6e6f 6465  ..)..}.(h...node
+00000c60: 2e6a 7394 6807 5d94 6816 8c07 6e6f 6465  .js.h.].h...node
+00000c70: 2e6a 7394 8594 8194 7d94 2868 1b68 ca68  .js.....}.(h.h.h
+00000c80: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00000c90: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00000ca0: 9468 295d 9475 682b 68c8 681e 4b12 681d  .h)].uh+h.h.K.h.
+00000cb0: 682c 681b 68c0 681c 6803 7562 6816 8c38  h,h.h.h.h.ubh..8
+00000cc0: 2069 6e73 7461 6c6c 6564 206f 6e20 796f   installed on yo
+00000cd0: 7572 2063 6f6d 7075 7465 722e 2059 6f75  ur computer. You
+00000ce0: 2063 616e 2067 6574 2069 7420 666f 7220   can get it for 
+00000cf0: 6672 6565 2061 7420 9485 9481 947d 9428  free at .....}.(
+00000d00: 681b 68c0 681c 6803 681d 4e68 1e4e 7562  h.h.h.h.h.Nh.Nub
+00000d10: 6809 8c09 7265 6665 7265 6e63 6594 9394  h...reference...
+00000d20: 2981 947d 9428 6805 8c0a 6e6f 6465 6a73  )..}.(h...nodejs
+00000d30: 2e6f 7267 9468 075d 9468 168c 0a6e 6f64  .org.h.].h...nod
+00000d40: 656a 732e 6f72 6794 8594 8194 7d94 2868  ejs.org.....}.(h
+00000d50: 1b68 de68 1c68 0368 1d4e 681e 4e75 6261  .h.h.h.h.Nh.Nuba
+00000d60: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00000d70: 9468 275d 9468 295d 948c 0672 6566 7572  .h'].h)]...refur
+00000d80: 6994 8c16 6874 7470 733a 2f2f 6e6f 6465  i...https://node
+00000d90: 6a73 2e6f 7267 2f65 6e2f 9475 682b 68dc  js.org/en/.uh+h.
+00000da0: 681e 4b12 681d 682c 681b 68c0 681c 6803  h.K.h.h,h.h.h.h.
+00000db0: 7562 6816 8c32 2e20 4966 2079 6f75 2073  ubh..2. If you s
+00000dc0: 7469 6c6c 2068 6176 6520 616e 2065 7272  till have an err
+00000dd0: 6f72 2c20 6f70 656e 2061 206e 6577 2069  or, open a new i
+00000de0: 7373 7565 206f 6e20 9485 9481 947d 9428  ssue on .....}.(
+00000df0: 681b 68c0 681c 6803 681d 4e68 1e4e 7562  h.h.h.h.h.Nh.Nub
+00000e00: 68dd 2981 947d 9428 6805 8c06 4769 7448  h.)..}.(h...GitH
+00000e10: 7562 9468 075d 9468 168c 0647 6974 4875  ub.h.].h...GitHu
+00000e20: 6294 8594 8194 7d94 2868 1b68 f268 1c68  b.....}.(h.h.h.h
+00000e30: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00000e40: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00000e50: 295d 9468 ec8c 3568 7474 7073 3a2f 2f67  )].h..5https://g
+00000e60: 6974 6875 622e 636f 6d2f 4d61 7869 6d65  ithub.com/Maxime
+00000e70: 4c65 4d61 6769 6369 656e 2f6d 7a64 6174  LeMagicien/mzdat
+00000e80: 6132 6d61 742f 6973 7375 6573 9475 682b  a2mat/issues.uh+
+00000e90: 68dc 681e 4b12 681d 682c 681b 68c0 681c  h.h.K.h.h,h.h.h.
+00000ea0: 6803 7562 6816 8c22 2c20 7765 2077 696c  h.ubh..", we wil
+00000eb0: 6c20 6265 2068 6170 7079 2074 6f20 616e  l be happy to an
+00000ec0: 7377 6572 2079 6f75 2021 9485 9481 947d  swer you !.....}
+00000ed0: 9428 681b 68c0 681c 6803 681d 4e68 1e4e  .(h.h.h.h.h.Nh.N
+00000ee0: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+00000ef0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00000f00: 3e68 1e4b 1268 1d68 2c68 1b68 af68 1c68  >h.K.h.h,h.h.h.h
+00000f10: 0375 6265 681f 7d94 2868 215d 948c 0b69  .ubeh.}.(h!]...i
+00000f20: 662d 6974 2d66 6169 6c73 9461 6823 5d94  f-it-fails.ah#].
+00000f30: 6825 5d94 8c0b 6966 2069 7420 6661 696c  h%]...if it fail
+00000f40: 7394 6168 275d 9468 295d 9475 682b 680a  s.ah'].h)].uh+h.
+00000f50: 681e 4b11 681d 682c 681b 680c 681c 6803  h.K.h.h,h.h.h.h.
+00000f60: 7562 6568 1f7d 9428 6821 5d94 8c11 6d7a  ubeh.}.(h!]...mz
+00000f70: 6461 7461 326d 6174 2d76 6572 6966 7994  data2mat-verify.
+00000f80: 6168 235d 9468 255d 948c 116d 7a64 6174  ah#].h%]...mzdat
+00000f90: 6132 6d61 742d 7665 7269 6679 9461 6827  a2mat-verify.ah'
+00000fa0: 5d94 6829 5d94 7568 2b68 0a68 1e4b 0168  ].h)].uh+h.h.K.h
+00000fb0: 1d68 2c68 1b68 0368 1c68 0375 6261 681f  .h,h.h.h.h.ubah.
+00000fc0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00000fd0: 275d 9468 295d 948c 0673 6f75 7263 6594  '].h)]...source.
+00000fe0: 682c 8c14 7472 616e 736c 6174 696f 6e5f  h,..translation_
+00000ff0: 7072 6f67 7265 7373 947d 9428 8c05 746f  progress.}.(..to
+00001000: 7461 6c94 4b00 8c0a 7472 616e 736c 6174  tal.K...translat
+00001010: 6564 944b 0075 7568 2b68 018c 0e63 7572  ed.K.uuh+h...cur
+00001020: 7265 6e74 5f73 6f75 7263 6594 4e8c 0c63  rent_source.N..c
+00001030: 7572 7265 6e74 5f6c 696e 6594 4e8c 0873  urrent_line.N..s
+00001040: 6574 7469 6e67 7394 8c11 646f 6375 7469  ettings...docuti
+00001050: 6c73 2e66 726f 6e74 656e 6494 8c06 5661  ls.frontend...Va
+00001060: 6c75 6573 9493 9429 8194 7d94 288c 066f  lues...)..}.(..o
+00001070: 7574 7075 7494 4e68 0f4e 8c09 6765 6e65  utput.Nh.N..gene
+00001080: 7261 746f 7294 4e8c 0964 6174 6573 7461  rator.N..datesta
+00001090: 6d70 944e 8c0b 736f 7572 6365 5f6c 696e  mp.N..source_lin
+000010a0: 6b94 4e8c 0a73 6f75 7263 655f 7572 6c94  k.N..source_url.
+000010b0: 4e8c 0d74 6f63 5f62 6163 6b6c 696e 6b73  N..toc_backlinks
+000010c0: 948c 0565 6e74 7279 948c 1266 6f6f 746e  ...entry...footn
+000010d0: 6f74 655f 6261 636b 6c69 6e6b 7394 4b01  ote_backlinks.K.
+000010e0: 8c0d 7365 6374 6e75 6d5f 7866 6f72 6d94  ..sectnum_xform.
+000010f0: 4b01 8c0e 7374 7269 705f 636f 6d6d 656e  K...strip_commen
+00001100: 7473 944e 8c1b 7374 7269 705f 656c 656d  ts.N..strip_elem
+00001110: 656e 7473 5f77 6974 685f 636c 6173 7365  ents_with_classe
+00001120: 7394 4e8c 0d73 7472 6970 5f63 6c61 7373  s.N..strip_class
+00001130: 6573 944e 8c0c 7265 706f 7274 5f6c 6576  es.N..report_lev
+00001140: 656c 944b 028c 0a68 616c 745f 6c65 7665  el.K...halt_leve
+00001150: 6c94 4b05 8c11 6578 6974 5f73 7461 7475  l.K...exit_statu
+00001160: 735f 6c65 7665 6c94 4b05 8c05 6465 6275  s_level.K...debu
+00001170: 6794 4e8c 0e77 6172 6e69 6e67 5f73 7472  g.N..warning_str
+00001180: 6561 6d94 4e8c 0974 7261 6365 6261 636b  eam.N..traceback
+00001190: 9488 8c0e 696e 7075 745f 656e 636f 6469  ....input_encodi
+000011a0: 6e67 948c 0975 7466 2d38 2d73 6967 948c  ng...utf-8-sig..
+000011b0: 1c69 6e70 7574 5f65 6e63 6f64 696e 675f  .input_encoding_
+000011c0: 6572 726f 725f 6861 6e64 6c65 7294 8c06  error_handler...
+000011d0: 7374 7269 6374 948c 0f6f 7574 7075 745f  strict...output_
+000011e0: 656e 636f 6469 6e67 948c 0575 7466 2d38  encoding...utf-8
+000011f0: 948c 1d6f 7574 7075 745f 656e 636f 6469  ...output_encodi
+00001200: 6e67 5f65 7272 6f72 5f68 616e 646c 6572  ng_error_handler
+00001210: 946a 4301 0000 8c0e 6572 726f 725f 656e  .jC.....error_en
+00001220: 636f 6469 6e67 948c 0575 7466 2d38 948c  coding...utf-8..
+00001230: 1c65 7272 6f72 5f65 6e63 6f64 696e 675f  .error_encoding_
+00001240: 6572 726f 725f 6861 6e64 6c65 7294 8c10  error_handler...
+00001250: 6261 636b 736c 6173 6872 6570 6c61 6365  backslashreplace
+00001260: 948c 0d6c 616e 6775 6167 655f 636f 6465  ...language_code
+00001270: 948c 0265 6e94 8c13 7265 636f 7264 5f64  ...en...record_d
+00001280: 6570 656e 6465 6e63 6965 7394 4e8c 0663  ependencies.N..c
+00001290: 6f6e 6669 6794 4e8c 0969 645f 7072 6566  onfig.N..id_pref
+000012a0: 6978 9468 068c 0e61 7574 6f5f 6964 5f70  ix.h...auto_id_p
+000012b0: 7265 6669 7894 8c02 6964 948c 0d64 756d  refix...id...dum
+000012c0: 705f 7365 7474 696e 6773 944e 8c0e 6475  p_settings.N..du
+000012d0: 6d70 5f69 6e74 6572 6e61 6c73 944e 8c0f  mp_internals.N..
+000012e0: 6475 6d70 5f74 7261 6e73 666f 726d 7394  dump_transforms.
+000012f0: 4e8c 0f64 756d 705f 7073 6575 646f 5f78  N..dump_pseudo_x
+00001300: 6d6c 944e 8c10 6578 706f 7365 5f69 6e74  ml.N..expose_int
+00001310: 6572 6e61 6c73 944e 8c0e 7374 7269 6374  ernals.N..strict
+00001320: 5f76 6973 6974 6f72 944e 8c0f 5f64 6973  _visitor.N.._dis
+00001330: 6162 6c65 5f63 6f6e 6669 6794 4e8c 075f  able_config.N.._
+00001340: 736f 7572 6365 9468 2c8c 0c5f 6465 7374  source.h,.._dest
+00001350: 696e 6174 696f 6e94 4e8c 0d5f 636f 6e66  ination.N.._conf
+00001360: 6967 5f66 696c 6573 945d 948c 1666 696c  ig_files.]...fil
+00001370: 655f 696e 7365 7274 696f 6e5f 656e 6162  e_insertion_enab
+00001380: 6c65 6494 888c 0b72 6177 5f65 6e61 626c  led....raw_enabl
+00001390: 6564 944b 018c 116c 696e 655f 6c65 6e67  ed.K...line_leng
+000013a0: 7468 5f6c 696d 6974 944d 1027 8c0e 7065  th_limit.M.'..pe
+000013b0: 705f 7265 6665 7265 6e63 6573 944e 8c0c  p_references.N..
+000013c0: 7065 705f 6261 7365 5f75 726c 948c 1868  pep_base_url...h
+000013d0: 7474 7073 3a2f 2f70 6570 732e 7079 7468  ttps://peps.pyth
+000013e0: 6f6e 2e6f 7267 2f94 8c15 7065 705f 6669  on.org/...pep_fi
+000013f0: 6c65 5f75 726c 5f74 656d 706c 6174 6594  le_url_template.
+00001400: 8c08 7065 702d 2530 3464 948c 0e72 6663  ..pep-%04d...rfc
+00001410: 5f72 6566 6572 656e 6365 7394 4e8c 0c72  _references.N..r
+00001420: 6663 5f62 6173 655f 7572 6c94 8c26 6874  fc_base_url..&ht
+00001430: 7470 733a 2f2f 6461 7461 7472 6163 6b65  tps://datatracke
+00001440: 722e 6965 7466 2e6f 7267 2f64 6f63 2f68  r.ietf.org/doc/h
+00001450: 746d 6c2f 948c 0974 6162 5f77 6964 7468  tml/...tab_width
+00001460: 944b 088c 1d74 7269 6d5f 666f 6f74 6e6f  .K...trim_footno
+00001470: 7465 5f72 6566 6572 656e 6365 5f73 7061  te_reference_spa
+00001480: 6365 9489 8c10 7379 6e74 6178 5f68 6967  ce....syntax_hig
+00001490: 686c 6967 6874 948c 046c 6f6e 6794 8c0c  hlight...long...
+000014a0: 736d 6172 745f 7175 6f74 6573 9488 8c13  smart_quotes....
+000014b0: 736d 6172 7471 756f 7465 735f 6c6f 6361  smartquotes_loca
+000014c0: 6c65 7394 5d94 8c1d 6368 6172 6163 7465  les.]...characte
+000014d0: 725f 6c65 7665 6c5f 696e 6c69 6e65 5f6d  r_level_inline_m
+000014e0: 6172 6b75 7094 898c 0e64 6f63 7469 746c  arkup....doctitl
+000014f0: 655f 7866 6f72 6d94 898c 0d64 6f63 696e  e_xform....docin
+00001500: 666f 5f78 666f 726d 944b 018c 1273 6563  fo_xform.K...sec
+00001510: 7473 7562 7469 746c 655f 7866 6f72 6d94  tsubtitle_xform.
+00001520: 898c 0d69 6d61 6765 5f6c 6f61 6469 6e67  ...image_loading
+00001530: 948c 046c 696e 6b94 8c10 656d 6265 645f  ...link...embed_
+00001540: 7374 796c 6573 6865 6574 9489 8c15 636c  stylesheet....cl
+00001550: 6f61 6b5f 656d 6169 6c5f 6164 6472 6573  oak_email_addres
+00001560: 7365 7394 888c 1173 6563 7469 6f6e 5f73  ses....section_s
+00001570: 656c 665f 6c69 6e6b 9489 8c03 656e 7694  elf_link....env.
+00001580: 4e75 628c 0872 6570 6f72 7465 7294 4e8c  Nub..reporter.N.
+00001590: 1069 6e64 6972 6563 745f 7461 7267 6574  .indirect_target
+000015a0: 7394 5d94 8c11 7375 6273 7469 7475 7469  s.]...substituti
+000015b0: 6f6e 5f64 6566 7394 7d94 288c 0f77 6f72  on_defs.}.(..wor
+000015c0: 6463 6f75 6e74 2d77 6f72 6473 9468 098c  dcount-words.h..
+000015d0: 1773 7562 7374 6974 7574 696f 6e5f 6465  .substitution_de
+000015e0: 6669 6e69 7469 6f6e 9493 9429 8194 7d94  finition...)..}.
+000015f0: 2868 058c 0331 3434 9468 075d 9468 168c  (h...144.h.].h..
+00001600: 0331 3434 9485 9481 947d 9468 1b6a 8101  .144.....}.h.j..
+00001610: 0000 7362 6168 1f7d 9428 6821 5d94 6823  ..sbah.}.(h!].h#
+00001620: 5d94 6825 5d94 8c0f 776f 7264 636f 756e  ].h%]...wordcoun
+00001630: 742d 776f 7264 7394 6168 275d 9468 295d  t-words.ah'].h)]
+00001640: 9475 682b 6a7f 0100 0068 1d68 2c75 628c  .uh+j....h.h,ub.
+00001650: 1177 6f72 6463 6f75 6e74 2d6d 696e 7574  .wordcount-minut
+00001660: 6573 946a 8001 0000 2981 947d 9428 6805  es.j....)..}.(h.
+00001670: 8c01 3194 6807 5d94 6816 8c01 3194 8594  ..1.h.].h...1...
+00001680: 8194 7d94 681b 6a91 0100 0073 6261 681f  ..}.h.j....sbah.
+00001690: 7d94 2868 215d 9468 235d 9468 255d 948c  }.(h!].h#].h%]..
+000016a0: 1177 6f72 6463 6f75 6e74 2d6d 696e 7574  .wordcount-minut
+000016b0: 6573 9461 6827 5d94 6829 5d94 7568 2b6a  es.ah'].h)].uh+j
+000016c0: 7f01 0000 681d 682c 7562 758c 1273 7562  ....h.h,ubu..sub
+000016d0: 7374 6974 7574 696f 6e5f 6e61 6d65 7394  stitution_names.
+000016e0: 7d94 288c 0f77 6f72 6463 6f75 6e74 2d77  }.(..wordcount-w
+000016f0: 6f72 6473 946a 7e01 0000 8c11 776f 7264  ords.j~.....word
+00001700: 636f 756e 742d 6d69 6e75 7465 7394 6a90  count-minutes.j.
+00001710: 0100 0075 8c08 7265 666e 616d 6573 947d  ...u..refnames.}
+00001720: 948c 0672 6566 6964 7394 7d94 8c07 6e61  ...refids.}...na
+00001730: 6d65 6964 7394 7d94 286a 1801 0000 6a15  meids.}.(j....j.
+00001740: 0100 0068 5368 5068 ac68 a96a 1001 0000  ...hShPh.h.j....
+00001750: 6a0d 0100 0075 8c09 6e61 6d65 7479 7065  j....u..nametype
+00001760: 7394 7d94 286a 1801 0000 8968 5389 68ac  s.}.(j.....hS.h.
+00001770: 896a 1001 0000 8975 6821 7d94 286a 1501  .j.....uh!}.(j..
+00001780: 0000 680c 6850 682d 68a9 6856 6a0d 0100  ..h.hPh-h.hVj...
+00001790: 0068 af75 8c0d 666f 6f74 6e6f 7465 5f72  .h.u..footnote_r
+000017a0: 6566 7394 7d94 8c0d 6369 7461 7469 6f6e  efs.}...citation
+000017b0: 5f72 6566 7394 7d94 8c0d 6175 746f 666f  _refs.}...autofo
+000017c0: 6f74 6e6f 7465 7394 5d94 8c11 6175 746f  otnotes.]...auto
+000017d0: 666f 6f74 6e6f 7465 5f72 6566 7394 5d94  footnote_refs.].
+000017e0: 8c10 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
+000017f0: 6573 945d 948c 1473 796d 626f 6c5f 666f  es.]...symbol_fo
+00001800: 6f74 6e6f 7465 5f72 6566 7394 5d94 8c09  otnote_refs.]...
+00001810: 666f 6f74 6e6f 7465 7394 5d94 8c09 6369  footnotes.]...ci
+00001820: 7461 7469 6f6e 7394 5d94 8c12 6175 746f  tations.]...auto
+00001830: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
+00001840: 018c 1573 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
+00001850: 7465 5f73 7461 7274 944b 008c 0a69 645f  te_start.K...id_
+00001860: 636f 756e 7465 7294 8c0b 636f 6c6c 6563  counter...collec
+00001870: 7469 6f6e 7394 8c07 436f 756e 7465 7294  tions...Counter.
+00001880: 9394 7d94 8594 5294 8c0e 7061 7273 655f  ..}...R...parse_
+00001890: 6d65 7373 6167 6573 945d 948c 1274 7261  messages.]...tra
+000018a0: 6e73 666f 726d 5f6d 6573 7361 6765 7394  nsform_messages.
+000018b0: 5d94 8c0b 7472 616e 7366 6f72 6d65 7294  ]...transformer.
+000018c0: 4e8c 0b69 6e63 6c75 6465 5f6c 6f67 945d  N..include_log.]
+000018d0: 948c 0a64 6563 6f72 6174 696f 6e94 4e68  ...decoration.Nh
+000018e0: 1c68 038c 0a6d 7973 745f 736c 7567 7394  .h...myst_slugs.
+000018f0: 7d94 7562 2e                             }.ub.
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/code-example.html` & `mzdata2mat-0.2.0/docs/build/html/code-example.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,162 +1,169 @@
-<!DOCTYPE html>
-<html class="writer-html5" lang="en" data-content_root="./">
-<head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Example Code &mdash; mzdata2mat 0.1.0 documentation</title>
-      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
-      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
-
-  
-  <!--[if lt IE 9]>
-    <script src="_static/js/html5shiv.min.js"></script>
-  <![endif]-->
-  
-        <script src="_static/jquery.js?v=5d32c60e"></script>
-        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="_static/documentation_options.js?v=01f34227"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
-        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
-    <script src="_static/js/theme.js"></script>
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="mzDataManager" href="mzDataManager.html" />
-    <link rel="prev" title="Installation" href="installation.html" /> 
-</head>
-
-<body class="wy-body-for-nav"> 
-  <div class="wy-grid-for-nav">
-    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
-      <div class="wy-side-scroll">
-        <div class="wy-side-nav-search" >
-
-          
-          
-          <a href="index.html" class="icon icon-home">
-            mzdata2mat
-          </a>
-<div role="search">
-  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
-    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
-    <input type="hidden" name="check_keywords" value="yes" />
-    <input type="hidden" name="area" value="default" />
-  </form>
-</div>
-        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
-<ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
-<li class="toctree-l1 current"><a class="current reference internal" href="#">Example Code</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#in-two-lines">In two lines</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#more-detailled-example">More detailled example</a></li>
-</ul>
-</li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
-<li class="toctree-l1"><a class="reference internal" href="matStructure.html">Matlab saving structure</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
-</ul>
-
-        </div>
-      </div>
-    </nav>
-
-    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
-          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
-          <a href="index.html">mzdata2mat</a>
-      </nav>
-
-      <div class="wy-nav-content">
-        <div class="rst-content">
-          <div role="navigation" aria-label="Page navigation">
-  <ul class="wy-breadcrumbs">
-      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
-      <li class="breadcrumb-item active">Example Code</li>
-      <li class="wy-breadcrumbs-aside">
-            <a href="_sources/code-example.md.txt" rel="nofollow"> View page source</a>
-      </li>
-  </ul>
-  <hr/>
-</div>
-          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
-           <div itemprop="articleBody">
-             
-  <section id="example-code">
-<h1>Example Code<a class="headerlink" href="#example-code" title="Link to this heading"></a></h1>
-<p>This page gives two examples on how to use the package. More examples will be added in the future.</p>
-<section id="in-two-lines">
-<h2>In two lines<a class="headerlink" href="#in-two-lines" title="Link to this heading"></a></h2>
-<p>You can acheive the conversion with only two lines of code :</p>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">mzdata2mat</span> <span class="kn">import</span> <span class="n">mzDataManager</span>
-
-<span class="n">mzDataManager</span><span class="p">(</span><span class="n">useDirectory</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">convertFile</span><span class="p">(</span><span class="o">&lt;</span><span class="n">path2mzDataFile</span><span class="o">&gt;</span><span class="p">,</span> <span class="o">&lt;</span><span class="n">path2folder2save</span><span class="o">&gt;</span><span class="p">)</span>
-
-</pre></div>
-</div>
-</section>
-<section id="more-detailled-example">
-<h2>More detailled example<a class="headerlink" href="#more-detailled-example" title="Link to this heading"></a></h2>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span>
-<span class="c1"># Here we import the main class used for the conversion.</span>
-<span class="mi">1</span> <span class="kn">from</span> <span class="nn">mzdata2mat</span> <span class="kn">import</span> <span class="n">mzDataManager</span>
-
-<span class="c1"># We initialize the class</span>
-<span class="c1"># If all mzData files are stored in the same directory, we can specify the parameter `mzDataPath` instead of `useDirectory`.</span>
-<span class="mi">2</span> <span class="n">converterAgent</span> <span class="o">=</span> <span class="n">mzDataManager</span><span class="p">(</span><span class="n">useDirectory</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-
-<span class="mi">3</span> <span class="n">path2mzDataFile</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;path/to/stored/files&quot;</span>
-
-<span class="mi">4</span> <span class="n">someDirectory</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;path/to/save/file/&quot;</span>
-
-<span class="c1"># Now we can call the mzDataXMLread function to read the .mzData.xml file:</span>
-<span class="mi">5</span> <span class="n">data</span> <span class="o">=</span> <span class="n">converterAgent</span><span class="o">.</span><span class="n">mzDataXMLread</span><span class="p">(</span><span class="n">fileName</span><span class="o">=</span><span class="n">path2mzDataFile</span><span class="p">)</span>
-
-<span class="c1"># The data we&#39;ve got from the previous function can be saved to a .mat file with the saveMatfile funtion:</span>
-<span class="mi">6</span> <span class="n">converterAgent</span><span class="o">.</span><span class="n">saveMatfile</span><span class="p">(</span><span class="n">mzData</span><span class="o">=</span><span class="n">data</span><span class="p">,</span> <span class="n">dir2save</span><span class="o">=</span><span class="n">someDirectory</span><span class="p">)</span>
-
-</pre></div>
-</div>
-</section>
-</section>
-
-
-           </div>
-          </div>
-          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="installation.html" class="btn btn-neutral float-left" title="Installation" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="mzDataManager.html" class="btn btn-neutral float-right" title="mzDataManager" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
-    </div>
-
-  <hr/>
-
-  <div role="contentinfo">
-    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
-  </div>
-
-  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
-    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
-    provided by <a href="https://readthedocs.org">Read the Docs</a>.
-   
-
-</footer>
-        </div>
-      </div>
-    </section>
-  </div>
-  <script>
-      jQuery(function () {
-          SphinxRtdTheme.Navigation.enable(true);
-      });
-  </script> 
-
-</body>
+<!DOCTYPE html>
+<html class="writer-html5" lang="en" data-content_root="./">
+<head>
+  <meta charset="utf-8" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>Example Code &mdash; mzdata2mat 0.2.0 documentation</title>
+      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
+      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
+
+  
+  <!--[if lt IE 9]>
+    <script src="_static/js/html5shiv.min.js"></script>
+  <![endif]-->
+  
+        <script src="_static/jquery.js?v=5d32c60e"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
+        <script src="_static/documentation_options.js?v=938c9ccc"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
+        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
+    <script src="_static/js/theme.js"></script>
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="Advanced load and save logic" href="advancedLoadSaveLogic.html" />
+    <link rel="prev" title="Installation" href="installation.html" /> 
+</head>
+
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
+
+          
+          
+          <a href="index.html" class="icon icon-home">
+            mzdata2mat
+          </a>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
+<ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
+<li class="toctree-l1 current"><a class="current reference internal" href="#">Example Code</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="#in-two-lines">In two lines</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#more-detailled-example">More detailled example</a></li>
+</ul>
+</li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Advanced</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="advancedLoadSaveLogic.html">Advanced load and save logic</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
+<li class="toctree-l1"><a class="reference internal" href="matStruct.html">matStruct</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">CLI</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
+</ul>
+
+        </div>
+      </div>
+    </nav>
+
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">mzdata2mat</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Example Code</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/code-example.md.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+  <section id="example-code">
+<h1>Example Code<a class="headerlink" href="#example-code" title="Link to this heading"></a></h1>
+<p>This page gives two examples on how to use the package. More examples will be added in the future.</p>
+<section id="in-two-lines">
+<h2>In two lines<a class="headerlink" href="#in-two-lines" title="Link to this heading"></a></h2>
+<p>You can acheive the conversion with only two lines of code :</p>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">mzdata2mat</span> <span class="kn">import</span> <span class="n">mzDataManager</span>
+
+<span class="n">mzDataManager</span><span class="p">(</span><span class="n">useDirectory</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">convertFile</span><span class="p">(</span><span class="o">&lt;</span><span class="n">path2mzDataFile</span><span class="o">&gt;</span><span class="p">,</span> <span class="o">&lt;</span><span class="n">path2folder2save</span><span class="o">&gt;</span><span class="p">)</span>
+
+</pre></div>
+</div>
+</section>
+<section id="more-detailled-example">
+<h2>More detailled example<a class="headerlink" href="#more-detailled-example" title="Link to this heading"></a></h2>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span>
+<span class="c1"># Here we import the main class used for the conversion.</span>
+<span class="mi">1</span> <span class="kn">from</span> <span class="nn">mzdata2mat</span> <span class="kn">import</span> <span class="n">mzDataManager</span>
+
+<span class="c1"># We initialize the class</span>
+<span class="c1"># If all mzData files are stored in the same directory, we can specify the parameter `mzDataPath` instead of `useDirectory`.</span>
+<span class="mi">2</span> <span class="n">converterAgent</span> <span class="o">=</span> <span class="n">mzDataManager</span><span class="p">(</span><span class="n">useDirectory</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+
+<span class="mi">3</span> <span class="n">path2mzDataFile</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;path/to/stored/files&quot;</span>
+
+<span class="mi">4</span> <span class="n">someDirectory</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;path/to/save/file/&quot;</span>
+
+<span class="c1"># Now we can call the mzDataXMLread function to read the .mzData.xml file:</span>
+<span class="mi">5</span> <span class="n">data</span> <span class="o">=</span> <span class="n">converterAgent</span><span class="o">.</span><span class="n">mzDataXMLread</span><span class="p">(</span><span class="n">fileName</span><span class="o">=</span><span class="n">path2mzDataFile</span><span class="p">)</span>
+
+<span class="c1"># The data we&#39;ve got from the previous function can be saved to a .mat file with the saveMatfile funtion:</span>
+<span class="mi">6</span> <span class="n">converterAgent</span><span class="o">.</span><span class="n">saveMatfile</span><span class="p">(</span><span class="n">mzData</span><span class="o">=</span><span class="n">data</span><span class="p">,</span> <span class="n">dir2save</span><span class="o">=</span><span class="n">someDirectory</span><span class="p">)</span>
+
+</pre></div>
+</div>
+</section>
+</section>
+
+
+           </div>
+          </div>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="installation.html" class="btn btn-neutral float-left" title="Installation" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="advancedLoadSaveLogic.html" class="btn btn-neutral float-right" title="Advanced load and save logic" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+    </div>
+
+  <hr/>
+
+  <div role="contentinfo">
+    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
+
+</footer>
+        </div>
+      </div>
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
+
+</body>
 </html>
```

#### html2text {}

```diff
@@ -3,20 +3,23 @@
 Infos
     * _C_h_a_n_g_e_l_o_g
 Quickstart
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _E_x_a_m_p_l_e_ _C_o_d_e
           o _I_n_ _t_w_o_ _l_i_n_e_s
           o _M_o_r_e_ _d_e_t_a_i_l_l_e_d_ _e_x_a_m_p_l_e
+Advanced
+    * _A_d_v_a_n_c_e_d_ _l_o_a_d_ _a_n_d_ _s_a_v_e_ _l_o_g_i_c
 API Reference
     * _m_z_D_a_t_a_M_a_n_a_g_e_r
-    * _M_a_t_l_a_b_ _s_a_v_i_n_g_ _s_t_r_u_c_t_u_r_e
+    * _m_a_t_S_t_r_u_c_t
     * _m_z_D_a_t_a
-    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
     * _m_z_D_a_t_a_X_M_L_S_t_r_u_c_t
+CLI
+    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
 _m_z_d_a_t_a_2_m_a_t
     * Example Code
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ EExxaammppllee CCooddee_? ************
 This page gives two examples on how to use the package. More examples will be
 added in the future.
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/genindex.html` & `mzdata2mat-0.2.0/docs/build/html/genindex.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,127 @@
-<!DOCTYPE html>
-<html class="writer-html5" lang="en" data-content_root="./">
-<head>
-  <meta charset="utf-8" />
-  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; mzdata2mat 0.1.0 documentation</title>
-      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
-      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
-
-  
-  <!--[if lt IE 9]>
-    <script src="_static/js/html5shiv.min.js"></script>
-  <![endif]-->
-  
-        <script src="_static/jquery.js?v=5d32c60e"></script>
-        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="_static/documentation_options.js?v=01f34227"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
-        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
-    <script src="_static/js/theme.js"></script>
-    <link rel="index" title="Index" href="#" />
-    <link rel="search" title="Search" href="search.html" /> 
-</head>
-
-<body class="wy-body-for-nav"> 
-  <div class="wy-grid-for-nav">
-    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
-      <div class="wy-side-scroll">
-        <div class="wy-side-nav-search" >
-
-          
-          
-          <a href="index.html" class="icon icon-home">
-            mzdata2mat
-          </a>
-<div role="search">
-  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
-    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
-    <input type="hidden" name="check_keywords" value="yes" />
-    <input type="hidden" name="area" value="default" />
-  </form>
-</div>
-        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
-<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
-<li class="toctree-l1"><a class="reference internal" href="matStructure.html">Matlab saving structure</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
-</ul>
-
-        </div>
-      </div>
-    </nav>
-
-    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
-          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
-          <a href="index.html">mzdata2mat</a>
-      </nav>
-
-      <div class="wy-nav-content">
-        <div class="rst-content">
-          <div role="navigation" aria-label="Page navigation">
-  <ul class="wy-breadcrumbs">
-      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
-      <li class="breadcrumb-item active">Index</li>
-      <li class="wy-breadcrumbs-aside">
-      </li>
-  </ul>
-  <hr/>
-</div>
-          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
-           <div itemprop="articleBody">
-             
-
-<h1 id="index">Index</h1>
-
-<div class="genindex-jumpbox">
- 
-</div>
-
-
-           </div>
-          </div>
-          <footer>
-
-  <hr/>
-
-  <div role="contentinfo">
-    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
-  </div>
-
-  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
-    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
-    provided by <a href="https://readthedocs.org">Read the Docs</a>.
-   
-
-</footer>
-        </div>
-      </div>
-    </section>
-  </div>
-  <script>
-      jQuery(function () {
-          SphinxRtdTheme.Navigation.enable(true);
-      });
-  </script> 
-
-</body>
+<!DOCTYPE html>
+<html class="writer-html5" lang="en" data-content_root="./">
+<head>
+  <meta charset="utf-8" />
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>Index &mdash; mzdata2mat 0.2.0 documentation</title>
+      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
+      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
+
+  
+  <!--[if lt IE 9]>
+    <script src="_static/js/html5shiv.min.js"></script>
+  <![endif]-->
+  
+        <script src="_static/jquery.js?v=5d32c60e"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
+        <script src="_static/documentation_options.js?v=938c9ccc"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
+        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
+    <script src="_static/js/theme.js"></script>
+    <link rel="index" title="Index" href="#" />
+    <link rel="search" title="Search" href="search.html" /> 
+</head>
+
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
+
+          
+          
+          <a href="index.html" class="icon icon-home">
+            mzdata2mat
+          </a>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
+<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Advanced</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="advancedLoadSaveLogic.html">Advanced load and save logic</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
+<li class="toctree-l1"><a class="reference internal" href="matStruct.html">matStruct</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">CLI</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
+</ul>
+
+        </div>
+      </div>
+    </nav>
+
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">mzdata2mat</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Index</li>
+      <li class="wy-breadcrumbs-aside">
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+
+<h1 id="index">Index</h1>
+
+<div class="genindex-jumpbox">
+ 
+</div>
+
+
+           </div>
+          </div>
+          <footer>
+
+  <hr/>
+
+  <div role="contentinfo">
+    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
+
+</footer>
+        </div>
+      </div>
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
+
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,23 @@
 _m_z_d_a_t_a_2_m_a_t
 [q                   ]
 Infos
     * _C_h_a_n_g_e_l_o_g
 Quickstart
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _E_x_a_m_p_l_e_ _C_o_d_e
+Advanced
+    * _A_d_v_a_n_c_e_d_ _l_o_a_d_ _a_n_d_ _s_a_v_e_ _l_o_g_i_c
 API Reference
     * _m_z_D_a_t_a_M_a_n_a_g_e_r
-    * _M_a_t_l_a_b_ _s_a_v_i_n_g_ _s_t_r_u_c_t_u_r_e
+    * _m_a_t_S_t_r_u_c_t
     * _m_z_D_a_t_a
-    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
     * _m_z_D_a_t_a_X_M_L_S_t_r_u_c_t
+CLI
+    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
 _m_z_d_a_t_a_2_m_a_t
     * Index
 ===============================================================================
 ************ IInnddeexx ************
 ===============================================================================
 © Copyright 2024, CORDELLA Maxime.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/index.html` & `mzdata2mat-0.2.0/docs/build/html/index.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,179 +1,191 @@
-<!DOCTYPE html>
-<html class="writer-html5" lang="en" data-content_root="./">
-<head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome &mdash; mzdata2mat 0.1.0 documentation</title>
-      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
-      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
-
-  
-  <!--[if lt IE 9]>
-    <script src="_static/js/html5shiv.min.js"></script>
-  <![endif]-->
-  
-        <script src="_static/jquery.js?v=5d32c60e"></script>
-        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="_static/documentation_options.js?v=01f34227"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
-        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
-    <script src="_static/js/theme.js"></script>
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="Changelog" href="Changelog.html" /> 
-</head>
-
-<body class="wy-body-for-nav"> 
-  <div class="wy-grid-for-nav">
-    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
-      <div class="wy-side-scroll">
-        <div class="wy-side-nav-search" >
-
-          
-          
-          <a href="#" class="icon icon-home">
-            mzdata2mat
-          </a>
-<div role="search">
-  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
-    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
-    <input type="hidden" name="check_keywords" value="yes" />
-    <input type="hidden" name="area" value="default" />
-  </form>
-</div>
-        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
-<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
-<li class="toctree-l1"><a class="reference internal" href="matStructure.html">Matlab saving structure</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
-</ul>
-
-        </div>
-      </div>
-    </nav>
-
-    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
-          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
-          <a href="#">mzdata2mat</a>
-      </nav>
-
-      <div class="wy-nav-content">
-        <div class="rst-content">
-          <div role="navigation" aria-label="Page navigation">
-  <ul class="wy-breadcrumbs">
-      <li><a href="#" class="icon icon-home" aria-label="Home"></a></li>
-      <li class="breadcrumb-item active">Welcome</li>
-      <li class="wy-breadcrumbs-aside">
-            <a href="_sources/index.rst.txt" rel="nofollow"> View page source</a>
-      </li>
-  </ul>
-  <hr/>
-</div>
-          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
-           <div itemprop="articleBody">
-             
-  <section id="welcome">
-<h1>Welcome<a class="headerlink" href="#welcome" title="Link to this heading"></a></h1>
-<p>Welcome ! <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> is a Python package from <a class="reference external" href="https://lartic.fsaa.ulaval.ca/">LARTIC research team</a>, which converts mzData.xml files (version 1.05, Agilent Technologies) into mat files readable using matlab.</p>
-<p>Author : Maxime R.A. Cordella</p>
-<p>Team leader : Pr. Christophe B.Y. Cordella</p>
-<p>Copyright(c)2024_LARTIC</p>
-<p><a class="reference external" href="https://mzdata2mat.readthedocs.io/en/latest/?badge=latest"><img alt="Documentation Status" src="https://readthedocs.org/projects/mzdata2mat/badge/?version=latest" /></a> <a class="reference external" href="https://pypi.org/project/mzdata2mat/"><img alt="PyPI" src="https://img.shields.io/pypi/v/mzdata2mat" /></a> <a class="reference external" href="https://pepy.tech/project/mzdata2mat"><img alt="downloads" src="https://static.pepy.tech/badge/mzdata2mat/month" /></a></p>
-<section id="current-version-0-1-0">
-<h2>Current version <code class="docutils literal notranslate"><span class="pre">0.1.0</span></code><a class="headerlink" href="#current-version-0-1-0" title="Link to this heading"></a></h2>
-<p>The current version of mzdata2mat is the following : <code class="docutils literal notranslate"><span class="pre">0.1.0</span></code></p>
-<p>You can see the complete changelog <a class="reference external" href="Changelog.html">here</a></p>
-</section>
-<section id="compatible-hardware">
-<h2>Compatible hardware<a class="headerlink" href="#compatible-hardware" title="Link to this heading"></a></h2>
-<p>At this time, the following OSes have been tested :</p>
-<section id="macos">
-<h3>macOS<a class="headerlink" href="#macos" title="Link to this heading"></a></h3>
-<p>At this time, <code class="docutils literal notranslate"><span class="pre">macOS</span> <span class="pre">Sonoma</span> <span class="pre">14.0</span></code> is officially supported, other macOS
-versions could be supported as long as they follow the requirements
-listed below.</p>
-</section>
-<section id="windows">
-<h3>Windows<a class="headerlink" href="#windows" title="Link to this heading"></a></h3>
-<p>At this time, <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> have been tested and is supported on
-<code class="docutils literal notranslate"><span class="pre">Windows</span> <span class="pre">11</span></code>, no testing has been done on Windows 10 or 7 but if you
-want to extend the compatibility, we are open to tester’s feedback on
-thoses machines.</p>
-</section>
-</section>
-<section id="requirements">
-<h2>Requirements<a class="headerlink" href="#requirements" title="Link to this heading"></a></h2>
-<section id="other-than-python">
-<h3>Other than Python<a class="headerlink" href="#other-than-python" title="Link to this heading"></a></h3>
-<p>This package <strong>requires node.js installed</strong>. you can download and
-install it at <a class="reference external" href="https://nodejs.org/en">nodejs.org</a>. It is available
-for both macOS and Windows for free.</p>
-</section>
-<section id="python-version">
-<h3>Python version<a class="headerlink" href="#python-version" title="Link to this heading"></a></h3>
-<p>This package is compatible to any python version equal or newer than
-<code class="docutils literal notranslate"><span class="pre">3.9</span></code>.</p>
-</section>
-<section id="python-packages">
-<h3>Python packages<a class="headerlink" href="#python-packages" title="Link to this heading"></a></h3>
-<p>When mzdata2mat will be installed on your system, the following packages
-will also be installed (if they are not) into your Python enviuronment :</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>pydantic&gt;=2.6.4
-mat4py&gt;=0.6.0
-javascript&gt;=1!1.1.3
-</pre></div>
-</div>
-<div class="toctree-wrapper compound">
-</div>
-<div class="toctree-wrapper compound">
-</div>
-<div class="toctree-wrapper compound">
-</div>
-</section>
-</section>
-</section>
-
-
-           </div>
-          </div>
-          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="Changelog.html" class="btn btn-neutral float-right" title="Changelog" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
-    </div>
-
-  <hr/>
-
-  <div role="contentinfo">
-    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
-  </div>
-
-  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
-    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
-    provided by <a href="https://readthedocs.org">Read the Docs</a>.
-   
-
-</footer>
-        </div>
-      </div>
-    </section>
-  </div>
-  <script>
-      jQuery(function () {
-          SphinxRtdTheme.Navigation.enable(true);
-      });
-  </script> 
-
-</body>
+<!DOCTYPE html>
+<html class="writer-html5" lang="en" data-content_root="./">
+<head>
+  <meta charset="utf-8" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>Welcome &mdash; mzdata2mat 0.2.0 documentation</title>
+      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
+      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
+
+  
+  <!--[if lt IE 9]>
+    <script src="_static/js/html5shiv.min.js"></script>
+  <![endif]-->
+  
+        <script src="_static/jquery.js?v=5d32c60e"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
+        <script src="_static/documentation_options.js?v=938c9ccc"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
+        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
+    <script src="_static/js/theme.js"></script>
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="Changelog" href="Changelog.html" /> 
+</head>
+
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
+
+          
+          
+          <a href="#" class="icon icon-home">
+            mzdata2mat
+          </a>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
+<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Advanced</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="advancedLoadSaveLogic.html">Advanced load and save logic</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
+<li class="toctree-l1"><a class="reference internal" href="matStruct.html">matStruct</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">CLI</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
+</ul>
+
+        </div>
+      </div>
+    </nav>
+
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="#">mzdata2mat</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="#" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Welcome</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/index.rst.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+  <section id="welcome">
+<h1>Welcome<a class="headerlink" href="#welcome" title="Link to this heading"></a></h1>
+<p>Welcome ! <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> is a Python package from <a class="reference external" href="https://lartic.fsaa.ulaval.ca/">LARTIC research team</a>, which converts mzData.xml files (version 1.05, Agilent Technologies) into mat files readable using matlab.</p>
+<p>Author : Maxime R.A. Cordella</p>
+<p>Team leader : Pr. Christophe B.Y. Cordella</p>
+<p>Copyright(c) 2024_LARTIC</p>
+<p><a class="reference external" href="https://mzdata2mat.readthedocs.io/en/latest/?badge=latest"><img alt="Documentation Status" src="https://readthedocs.org/projects/mzdata2mat/badge/?version=latest" /></a> <a class="reference external" href="https://pypi.org/project/mzdata2mat/"><img alt="PyPI" src="https://img.shields.io/pypi/v/mzdata2mat" /></a> <a class="reference external" href="https://pepy.tech/project/mzdata2mat"><img alt="downloads" src="https://static.pepy.tech/badge/mzdata2mat/month" /></a></p>
+<section id="current-version-0-2-0">
+<h2>Current version <code class="docutils literal notranslate"><span class="pre">0.2.0</span></code><a class="headerlink" href="#current-version-0-2-0" title="Link to this heading"></a></h2>
+<p>The current version of mzdata2mat is the following : <code class="docutils literal notranslate"><span class="pre">0.2.0</span></code></p>
+<p>You can see the complete changelog <a class="reference external" href="Changelog.html">here</a></p>
+</section>
+<section id="compatible-hardware">
+<h2>Compatible hardware<a class="headerlink" href="#compatible-hardware" title="Link to this heading"></a></h2>
+<p>At this time, the following OSes have been tested :</p>
+<section id="macos">
+<h3>macOS<a class="headerlink" href="#macos" title="Link to this heading"></a></h3>
+<p>At this time, <code class="docutils literal notranslate"><span class="pre">macOS</span> <span class="pre">Sonoma</span> <span class="pre">14.0</span></code> is officially supported, other macOS
+versions could be supported as long as they follow the requirements
+listed below.</p>
+</section>
+<section id="windows">
+<h3>Windows<a class="headerlink" href="#windows" title="Link to this heading"></a></h3>
+<p>At this time, <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> have been tested and is supported on
+<code class="docutils literal notranslate"><span class="pre">Windows</span> <span class="pre">11</span></code>, no testing has been done on Windows 10 or 7 but if you
+want to extend the compatibility, we are open to tester’s feedback on
+thoses machines.</p>
+</section>
+</section>
+<section id="requirements">
+<h2>Requirements<a class="headerlink" href="#requirements" title="Link to this heading"></a></h2>
+<section id="other-than-python">
+<h3>Other than Python<a class="headerlink" href="#other-than-python" title="Link to this heading"></a></h3>
+<p>This package <strong>requires node.js installed</strong>. you can download and
+install it at <a class="reference external" href="https://nodejs.org/en">nodejs.org</a>. It is available
+for both macOS and Windows for free.</p>
+</section>
+<section id="python-version">
+<h3>Python version<a class="headerlink" href="#python-version" title="Link to this heading"></a></h3>
+<p>This package is compatible to any python version equal or newer than
+<code class="docutils literal notranslate"><span class="pre">3.9</span></code>.</p>
+</section>
+<section id="python-packages">
+<h3>Python packages<a class="headerlink" href="#python-packages" title="Link to this heading"></a></h3>
+<p>When mzdata2mat will be installed on your system, the following packages
+will also be installed (if they are not) into your Python enviuronment :</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>pydantic&gt;=2.6.4
+mat4py&gt;=0.6.0
+javascript&gt;=1!1.1.3
+colorama&gt;=0.4.6
+</pre></div>
+</div>
+<div class="toctree-wrapper compound">
+</div>
+<div class="toctree-wrapper compound">
+</div>
+<div class="toctree-wrapper compound">
+</div>
+<div class="toctree-wrapper compound">
+</div>
+<div class="toctree-wrapper compound">
+</div>
+</section>
+</section>
+</section>
+
+
+           </div>
+          </div>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="Changelog.html" class="btn btn-neutral float-right" title="Changelog" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+    </div>
+
+  <hr/>
+
+  <div role="contentinfo">
+    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
+
+</footer>
+        </div>
+      </div>
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
+
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,34 +1,37 @@
 _m_z_d_a_t_a_2_m_a_t
 [q                   ]
 Infos
     * _C_h_a_n_g_e_l_o_g
 Quickstart
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _E_x_a_m_p_l_e_ _C_o_d_e
+Advanced
+    * _A_d_v_a_n_c_e_d_ _l_o_a_d_ _a_n_d_ _s_a_v_e_ _l_o_g_i_c
 API Reference
     * _m_z_D_a_t_a_M_a_n_a_g_e_r
-    * _M_a_t_l_a_b_ _s_a_v_i_n_g_ _s_t_r_u_c_t_u_r_e
+    * _m_a_t_S_t_r_u_c_t
     * _m_z_D_a_t_a
-    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
     * _m_z_D_a_t_a_X_M_L_S_t_r_u_c_t
+CLI
+    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
 _m_z_d_a_t_a_2_m_a_t
     * Welcome
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ WWeellccoommee_? ************
 Welcome ! mzdata2mat is a Python package from _L_A_R_T_I_C_ _r_e_s_e_a_r_c_h_ _t_e_a_m, which
 converts mzData.xml files (version 1.05, Agilent Technologies) into mat files
 readable using matlab.
 Author : Maxime R.A. Cordella
 Team leader : Pr. Christophe B.Y. Cordella
-Copyright(c)2024_LARTIC
+Copyright(c) 2024_LARTIC
 _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_P_y_P_I_]_[_d_o_w_n_l_o_a_d_s_]
-********** CCuurrrreenntt vveerrssiioonn 00..11..00_? **********
-The current version of mzdata2mat is the following : 0.1.0
+********** CCuurrrreenntt vveerrssiioonn 00..22..00_? **********
+The current version of mzdata2mat is the following : 0.2.0
 You can see the complete changelog _h_e_r_e
 ********** CCoommppaattiibbllee hhaarrddwwaarree_? **********
 At this time, the following OSes have been tested :
 ******** mmaaccOOSS_? ********
 At this time, macOS Sonoma 14.0 is officially supported, other macOS versions
 could be supported as long as they follow the requirements listed below.
 ******** WWiinnddoowwss_? ********
@@ -43,11 +46,12 @@
 This package is compatible to any python version equal or newer than 3.9.
 ******** PPyytthhoonn ppaacckkaaggeess_? ********
 When mzdata2mat will be installed on your system, the following packages will
 also be installed (if they are not) into your Python enviuronment :
 pydantic>=2.6.4
 mat4py>=0.6.0
 javascript>=1!1.1.3
+colorama>=0.4.6
 _N_e_x_t
 ===============================================================================
 © Copyright 2024, CORDELLA Maxime.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/installation.html` & `mzdata2mat-0.2.0/docs/build/html/installation.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,173 +1,180 @@
-<!DOCTYPE html>
-<html class="writer-html5" lang="en" data-content_root="./">
-<head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; mzdata2mat 0.1.0 documentation</title>
-      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
-      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
-
-  
-  <!--[if lt IE 9]>
-    <script src="_static/js/html5shiv.min.js"></script>
-  <![endif]-->
-  
-        <script src="_static/jquery.js?v=5d32c60e"></script>
-        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="_static/documentation_options.js?v=01f34227"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
-        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
-    <script src="_static/js/theme.js"></script>
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="Example Code" href="code-example.html" />
-    <link rel="prev" title="Changelog" href="Changelog.html" /> 
-</head>
-
-<body class="wy-body-for-nav"> 
-  <div class="wy-grid-for-nav">
-    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
-      <div class="wy-side-scroll">
-        <div class="wy-side-nav-search" >
-
-          
-          
-          <a href="index.html" class="icon icon-home">
-            mzdata2mat
-          </a>
-<div role="search">
-  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
-    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
-    <input type="hidden" name="check_keywords" value="yes" />
-    <input type="hidden" name="area" value="default" />
-  </form>
-</div>
-        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
-<ul class="current">
-<li class="toctree-l1 current"><a class="current reference internal" href="#">Installation</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#command">Command</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#verify-the-installation">Verify the installation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#troubbleshooting">Troubbleshooting</a></li>
-</ul>
-</li>
-<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
-<li class="toctree-l1"><a class="reference internal" href="matStructure.html">Matlab saving structure</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
-</ul>
-
-        </div>
-      </div>
-    </nav>
-
-    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
-          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
-          <a href="index.html">mzdata2mat</a>
-      </nav>
-
-      <div class="wy-nav-content">
-        <div class="rst-content">
-          <div role="navigation" aria-label="Page navigation">
-  <ul class="wy-breadcrumbs">
-      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
-      <li class="breadcrumb-item active">Installation</li>
-      <li class="wy-breadcrumbs-aside">
-            <a href="_sources/installation.md.txt" rel="nofollow"> View page source</a>
-      </li>
-  </ul>
-  <hr/>
-</div>
-          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
-           <div itemprop="articleBody">
-             
-  <section id="installation">
-<h1>Installation<a class="headerlink" href="#installation" title="Link to this heading"></a></h1>
-<section id="command">
-<h2>Command<a class="headerlink" href="#command" title="Link to this heading"></a></h2>
-<p>To install <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> into your Python environment, run the following command inside your terminal :</p>
-<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>pip<span class="w"> </span>install<span class="w"> </span>mzdata2mat
-</pre></div>
-</div>
-<p>If you have multiple instances of Python installed, run this command with the chosen Python interpreter to install <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> in the corresponding Python installation :</p>
-<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>&lt;pathToPythonApp&gt;<span class="w"> </span>-m<span class="w"> </span>pip<span class="w"> </span>install<span class="w"> </span>mzdata2mat
-</pre></div>
-</div>
-<p>When the command terminates, you have successfully installed mzdata2mat !</p>
-</section>
-<section id="verify-the-installation">
-<h2>Verify the installation<a class="headerlink" href="#verify-the-installation" title="Link to this heading"></a></h2>
-<p>To verfiy if the installation was successful, run in your terminal this command :</p>
-<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>mzdata2mat-verify
-</pre></div>
-</div>
-<p>When you will first run this command, node.js will download and install the <code class="docutils literal notranslate"><span class="pre">mzdata</span></code> package from <code class="docutils literal notranslate"><span class="pre">npm</span></code>. This will only happen the first time you run the command. The terminal will show you these lines during the process :</p>
-<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span><span class="w"> </span>Installing<span class="w"> </span><span class="s1">&#39;mzdata&#39;</span><span class="w"> </span>version<span class="w"> </span><span class="s1">&#39;latest&#39;</span>...<span class="w"> </span>This<span class="w"> </span>will<span class="w"> </span>only<span class="w"> </span>happen<span class="w"> </span>once.<span class="w"> </span>
-
-added<span class="w"> </span><span class="m">7</span><span class="w"> </span>packages,<span class="w"> </span>and<span class="w"> </span>audited<span class="w"> </span><span class="m">8</span><span class="w"> </span>packages<span class="w"> </span><span class="k">in</span><span class="w"> </span>2s
-
-<span class="m">1</span><span class="w"> </span>package<span class="w"> </span>is<span class="w"> </span>looking<span class="w"> </span><span class="k">for</span><span class="w"> </span>funding
-<span class="w">  </span>run<span class="w"> </span><span class="sb">`</span>npm<span class="w"> </span>fund<span class="sb">`</span><span class="w"> </span><span class="k">for</span><span class="w"> </span>details
-
-found<span class="w"> </span><span class="m">0</span><span class="w"> </span>vulnerabilities
-
-<span class="w"> </span>OK.<span class="w"> </span>
-<span class="o">[</span>JSE<span class="o">]</span><span class="w"> </span>
-
-<span class="o">[</span>JSE<span class="o">]</span><span class="w"> </span>
-</pre></div>
-</div>
-<p>When it’s done, the <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> package will attempt to convert an example <code class="docutils literal notranslate"><span class="pre">.mzdata.xml</span></code> file into a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file. If everything goes right, you will get this message :</p>
-<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>mzdata2mat<span class="w"> </span>-<span class="w"> </span>Ready<span class="w"> </span>to<span class="w"> </span>use<span class="w"> </span>!
-</pre></div>
-</div>
-<p>The example file (.mzdata.xml) will be copied in the current working directory and the converted file (.mat) will be added as soon as the conversion finishes.</p>
-</section>
-<section id="troubbleshooting">
-<h2>Troubbleshooting<a class="headerlink" href="#troubbleshooting" title="Link to this heading"></a></h2>
-<p>If an error occurs, this probably means that you do not have <strong>node.js</strong> installed on your machine or you didn’t add it to your PATH.</p>
-</section>
-</section>
-
-
-           </div>
-          </div>
-          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="Changelog.html" class="btn btn-neutral float-left" title="Changelog" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="code-example.html" class="btn btn-neutral float-right" title="Example Code" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
-    </div>
-
-  <hr/>
-
-  <div role="contentinfo">
-    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
-  </div>
-
-  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
-    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
-    provided by <a href="https://readthedocs.org">Read the Docs</a>.
-   
-
-</footer>
-        </div>
-      </div>
-    </section>
-  </div>
-  <script>
-      jQuery(function () {
-          SphinxRtdTheme.Navigation.enable(true);
-      });
-  </script> 
-
-</body>
+<!DOCTYPE html>
+<html class="writer-html5" lang="en" data-content_root="./">
+<head>
+  <meta charset="utf-8" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>Installation &mdash; mzdata2mat 0.2.0 documentation</title>
+      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
+      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
+
+  
+  <!--[if lt IE 9]>
+    <script src="_static/js/html5shiv.min.js"></script>
+  <![endif]-->
+  
+        <script src="_static/jquery.js?v=5d32c60e"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
+        <script src="_static/documentation_options.js?v=938c9ccc"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
+        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
+    <script src="_static/js/theme.js"></script>
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="Example Code" href="code-example.html" />
+    <link rel="prev" title="Changelog" href="Changelog.html" /> 
+</head>
+
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
+
+          
+          
+          <a href="index.html" class="icon icon-home">
+            mzdata2mat
+          </a>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
+<ul class="current">
+<li class="toctree-l1 current"><a class="current reference internal" href="#">Installation</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="#command">Command</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#verify-the-installation">Verify the installation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#troubbleshooting">Troubbleshooting</a></li>
+</ul>
+</li>
+<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Advanced</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="advancedLoadSaveLogic.html">Advanced load and save logic</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
+<li class="toctree-l1"><a class="reference internal" href="matStruct.html">matStruct</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">CLI</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
+</ul>
+
+        </div>
+      </div>
+    </nav>
+
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">mzdata2mat</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Installation</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/installation.md.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+  <section id="installation">
+<h1>Installation<a class="headerlink" href="#installation" title="Link to this heading"></a></h1>
+<section id="command">
+<h2>Command<a class="headerlink" href="#command" title="Link to this heading"></a></h2>
+<p>To install <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> into your Python environment, run the following command inside your terminal :</p>
+<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>pip<span class="w"> </span>install<span class="w"> </span>mzdata2mat
+</pre></div>
+</div>
+<p>If you have multiple instances of Python installed, run this command with the chosen Python interpreter to install <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> in the corresponding Python installation :</p>
+<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>&lt;pathToPythonApp&gt;<span class="w"> </span>-m<span class="w"> </span>pip<span class="w"> </span>install<span class="w"> </span>mzdata2mat
+</pre></div>
+</div>
+<p>When the command terminates, you have successfully installed mzdata2mat !</p>
+</section>
+<section id="verify-the-installation">
+<h2>Verify the installation<a class="headerlink" href="#verify-the-installation" title="Link to this heading"></a></h2>
+<p>To verfiy if the installation was successful, run in your terminal this command :</p>
+<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>mzdata2mat-verify
+</pre></div>
+</div>
+<p>When you will first run this command, node.js will download and install the <code class="docutils literal notranslate"><span class="pre">mzdata</span></code> package from <code class="docutils literal notranslate"><span class="pre">npm</span></code>. This will only happen the first time you run the command. The terminal will show you these lines during the process :</p>
+<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span><span class="w"> </span>Installing<span class="w"> </span><span class="s1">&#39;mzdata&#39;</span><span class="w"> </span>version<span class="w"> </span><span class="s1">&#39;latest&#39;</span>...<span class="w"> </span>This<span class="w"> </span>will<span class="w"> </span>only<span class="w"> </span>happen<span class="w"> </span>once.<span class="w"> </span>
+
+added<span class="w"> </span><span class="m">7</span><span class="w"> </span>packages,<span class="w"> </span>and<span class="w"> </span>audited<span class="w"> </span><span class="m">8</span><span class="w"> </span>packages<span class="w"> </span><span class="k">in</span><span class="w"> </span>2s
+
+<span class="m">1</span><span class="w"> </span>package<span class="w"> </span>is<span class="w"> </span>looking<span class="w"> </span><span class="k">for</span><span class="w"> </span>funding
+<span class="w">  </span>run<span class="w"> </span><span class="sb">`</span>npm<span class="w"> </span>fund<span class="sb">`</span><span class="w"> </span><span class="k">for</span><span class="w"> </span>details
+
+found<span class="w"> </span><span class="m">0</span><span class="w"> </span>vulnerabilities
+
+<span class="w"> </span>OK.<span class="w"> </span>
+<span class="o">[</span>JSE<span class="o">]</span><span class="w"> </span>
+
+<span class="o">[</span>JSE<span class="o">]</span><span class="w"> </span>
+</pre></div>
+</div>
+<p>When it’s done, the <code class="docutils literal notranslate"><span class="pre">mzdata2mat</span></code> package will attempt to convert an example <code class="docutils literal notranslate"><span class="pre">.mzdata.xml</span></code> file into a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file. If everything goes right, you will get this message :</p>
+<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>mzdata2mat<span class="w"> </span>-<span class="w"> </span>Ready<span class="w"> </span>to<span class="w"> </span>use<span class="w"> </span>!
+</pre></div>
+</div>
+<p>The example file (.mzdata.xml) will be copied in the current working directory and the converted file (.mat) will be added as soon as the conversion finishes.</p>
+</section>
+<section id="troubbleshooting">
+<h2>Troubbleshooting<a class="headerlink" href="#troubbleshooting" title="Link to this heading"></a></h2>
+<p>If an error occurs, this probably means that you do not have <strong>node.js</strong> installed on your machine or you didn’t add it to your PATH.</p>
+</section>
+</section>
+
+
+           </div>
+          </div>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="Changelog.html" class="btn btn-neutral float-left" title="Changelog" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="code-example.html" class="btn btn-neutral float-right" title="Example Code" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+    </div>
+
+  <hr/>
+
+  <div role="contentinfo">
+    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
+
+</footer>
+        </div>
+      </div>
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
+
+</body>
 </html>
```

#### html2text {}

```diff
@@ -4,20 +4,23 @@
     * _C_h_a_n_g_e_l_o_g
 Quickstart
     * _I_n_s_t_a_l_l_a_t_i_o_n
           o _C_o_m_m_a_n_d
           o _V_e_r_i_f_y_ _t_h_e_ _i_n_s_t_a_l_l_a_t_i_o_n
           o _T_r_o_u_b_b_l_e_s_h_o_o_t_i_n_g
     * _E_x_a_m_p_l_e_ _C_o_d_e
+Advanced
+    * _A_d_v_a_n_c_e_d_ _l_o_a_d_ _a_n_d_ _s_a_v_e_ _l_o_g_i_c
 API Reference
     * _m_z_D_a_t_a_M_a_n_a_g_e_r
-    * _M_a_t_l_a_b_ _s_a_v_i_n_g_ _s_t_r_u_c_t_u_r_e
+    * _m_a_t_S_t_r_u_c_t
     * _m_z_D_a_t_a
-    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
     * _m_z_D_a_t_a_X_M_L_S_t_r_u_c_t
+CLI
+    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
 _m_z_d_a_t_a_2_m_a_t
     * Installation
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ IInnssttaallllaattiioonn_? ************
 ********** CCoommmmaanndd_? **********
 To install mzdata2mat into your Python environment, run the following command
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/mzDataManager.html` & `mzdata2mat-0.2.0/docs/build/html/mzDataManager.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,308 +1,315 @@
-<!DOCTYPE html>
-<html class="writer-html5" lang="en" data-content_root="./">
-<head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>mzDataManager &mdash; mzdata2mat 0.1.0 documentation</title>
-      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
-      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
-
-  
-  <!--[if lt IE 9]>
-    <script src="_static/js/html5shiv.min.js"></script>
-  <![endif]-->
-  
-        <script src="_static/jquery.js?v=5d32c60e"></script>
-        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="_static/documentation_options.js?v=01f34227"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
-        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
-    <script src="_static/js/theme.js"></script>
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="Matlab saving structure" href="matStructure.html" />
-    <link rel="prev" title="Example Code" href="code-example.html" /> 
-</head>
-
-<body class="wy-body-for-nav"> 
-  <div class="wy-grid-for-nav">
-    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
-      <div class="wy-side-scroll">
-        <div class="wy-side-nav-search" >
-
-          
-          
-          <a href="index.html" class="icon icon-home">
-            mzdata2mat
-          </a>
-<div role="search">
-  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
-    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
-    <input type="hidden" name="check_keywords" value="yes" />
-    <input type="hidden" name="area" value="default" />
-  </form>
-</div>
-        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
-<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
-<ul class="current">
-<li class="toctree-l1 current"><a class="current reference internal" href="#">mzDataManager</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#presentation">Presentation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#definition">Definition</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#how-to-use">How to use</a><ul>
-<li class="toctree-l3"><a class="reference internal" href="#with-path">With path</a></li>
-<li class="toctree-l3"><a class="reference internal" href="#without-path">Without path</a></li>
-</ul>
-</li>
-<li class="toctree-l2"><a class="reference internal" href="#functions">Functions</a><ul>
-<li class="toctree-l3"><a class="reference internal" href="#mzdataxmlread">mzDataXMLread</a><ul>
-<li class="toctree-l4"><a class="reference internal" href="#id1">Presentation</a></li>
-<li class="toctree-l4"><a class="reference internal" href="#id2">Definition</a></li>
-<li class="toctree-l4"><a class="reference internal" href="#id3">How to use</a></li>
-</ul>
-</li>
-<li class="toctree-l3"><a class="reference internal" href="#savematfile">saveMatfile</a><ul>
-<li class="toctree-l4"><a class="reference internal" href="#id4">Presentation</a></li>
-<li class="toctree-l4"><a class="reference internal" href="#id5">Definition</a></li>
-<li class="toctree-l4"><a class="reference internal" href="#id6">How to use</a></li>
-</ul>
-</li>
-<li class="toctree-l3"><a class="reference internal" href="#convertfile">convertFile</a><ul>
-<li class="toctree-l4"><a class="reference internal" href="#id7">Presentation</a></li>
-<li class="toctree-l4"><a class="reference internal" href="#id8">Definition</a></li>
-<li class="toctree-l4"><a class="reference internal" href="#id9">How to use</a></li>
-</ul>
-</li>
-</ul>
-</li>
-</ul>
-</li>
-<li class="toctree-l1"><a class="reference internal" href="matStructure.html">Matlab saving structure</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
-</ul>
-
-        </div>
-      </div>
-    </nav>
-
-    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
-          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
-          <a href="index.html">mzdata2mat</a>
-      </nav>
-
-      <div class="wy-nav-content">
-        <div class="rst-content">
-          <div role="navigation" aria-label="Page navigation">
-  <ul class="wy-breadcrumbs">
-      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
-      <li class="breadcrumb-item active">mzDataManager</li>
-      <li class="wy-breadcrumbs-aside">
-            <a href="_sources/mzDataManager.md.txt" rel="nofollow"> View page source</a>
-      </li>
-  </ul>
-  <hr/>
-</div>
-          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
-           <div itemprop="articleBody">
-             
-  <section id="mzdatamanager">
-<h1>mzDataManager<a class="headerlink" href="#mzdatamanager" title="Link to this heading"></a></h1>
-<section id="presentation">
-<h2>Presentation<a class="headerlink" href="#presentation" title="Link to this heading"></a></h2>
-<p>Main class used for converting mzData files into matlab files.</p>
-</section>
-<section id="definition">
-<h2>Definition<a class="headerlink" href="#definition" title="Link to this heading"></a></h2>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">class</span> <span class="nc">mzDataManager</span><span class="p">(</span><span class="n">BaseModel</span><span class="p">):</span>
-    <span class="n">mzDataPath</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-    <span class="n">exportPath</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-    <span class="n">useDirectory</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</pre></div>
-</div>
-</section>
-<section id="how-to-use">
-<h2>How to use<a class="headerlink" href="#how-to-use" title="Link to this heading"></a></h2>
-<section id="with-path">
-<h3>With path<a class="headerlink" href="#with-path" title="Link to this heading"></a></h3>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="n">manager</span> <span class="o">=</span> <span class="n">mzDataManager</span><span class="p">(</span>
-    <span class="n">mzDataPath</span> <span class="o">=</span> <span class="s2">&quot;Some/Path&quot;</span><span class="p">,</span>
-    <span class="n">exportPath</span> <span class="o">=</span> <span class="s2">&quot;Some/Export/Path&quot;</span><span class="p">,</span>
-<span class="p">)</span>
-</pre></div>
-</div>
-<p>The path you specify in those arguments will be stored in the class, so when you use the integrated functions, you only need to specify the relative path to the file.</p>
-</section>
-<section id="without-path">
-<h3>Without path<a class="headerlink" href="#without-path" title="Link to this heading"></a></h3>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="n">manager</span> <span class="o">=</span> <span class="n">mzDataManager</span><span class="p">(</span><span class="n">useDirectory</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-</pre></div>
-</div>
-<p>Setting up the class this way will require to specify each time you call a function to give the full path and the export directory.</p>
-</section>
-</section>
-<section id="functions">
-<h2>Functions<a class="headerlink" href="#functions" title="Link to this heading"></a></h2>
-<section id="mzdataxmlread">
-<h3>mzDataXMLread<a class="headerlink" href="#mzdataxmlread" title="Link to this heading"></a></h3>
-<section id="id1">
-<h4>Presentation<a class="headerlink" href="#id1" title="Link to this heading"></a></h4>
-<p>This function reads a <code class="docutils literal notranslate"><span class="pre">.mzData.xml</span></code> file and returns a <code class="docutils literal notranslate"><span class="pre">mzData</span></code> structure which can be modified before saving it’s data to a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file (See <a class="reference internal" href="mzData.html"><span class="std std-doc">mzData</span></a> class for further details).</p>
-</section>
-<section id="id2">
-<h4>Definition<a class="headerlink" href="#id2" title="Link to this heading"></a></h4>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">def</span> <span class="nf">mzDataXMLread</span><span class="p">(</span><span class="bp">self</span><span class="nd">@mzDataManager</span><span class="p">,</span> <span class="n">fileName</span> <span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">customDirectory</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span>
-</pre></div>
-</div>
-</section>
-<section id="id3">
-<h4>How to use<a class="headerlink" href="#id3" title="Link to this heading"></a></h4>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="c1"># Considering that mzDataManager class has been intialized before and stored as manager variable</span>
-
-<span class="n">content</span> <span class="o">=</span> <span class="n">manager</span><span class="o">.</span><span class="n">mzDataXMLread</span><span class="p">(</span>
-    <span class="n">fileName</span><span class="o">=</span><span class="n">Path2File</span>
-<span class="p">)</span>
-</pre></div>
-</div>
-<p><u>Parameters</u></p>
-<ul class="simple">
-<li><p>If directories were provided in the init process :</p>
-<ul>
-<li><p><code class="docutils literal notranslate"><span class="pre">fileName</span></code> : Relative path of the <code class="docutils literal notranslate"><span class="pre">mzData.xml</span></code> file to read</p></li>
-<li><p><code class="docutils literal notranslate"><span class="pre">customDirectory</span></code> : Set this parameter to <code class="docutils literal notranslate"><span class="pre">True</span></code> if you provide a full path which is different than the one specified in the init process.</p></li>
-</ul>
-</li>
-<li><p>Otherwise :</p>
-<ul>
-<li><p><code class="docutils literal notranslate"><span class="pre">fileName</span></code> : Full path to the <code class="docutils literal notranslate"><span class="pre">mzData.xml</span></code> file to read</p></li>
-<li><p><code class="docutils literal notranslate"><span class="pre">customDirectory</span></code> : Does nothing</p></li>
-</ul>
-</li>
-</ul>
-<p><u>Outputs</u></p>
-<ul class="simple">
-<li><p>Outputs a <code class="docutils literal notranslate"><span class="pre">mzData</span></code> class containing the content of the file parsed.</p></li>
-</ul>
-</section>
-</section>
-<section id="savematfile">
-<h3>saveMatfile<a class="headerlink" href="#savematfile" title="Link to this heading"></a></h3>
-<section id="id4">
-<h4>Presentation<a class="headerlink" href="#id4" title="Link to this heading"></a></h4>
-<p>Saves a <code class="docutils literal notranslate"><span class="pre">mzData</span></code> class into a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file with all metadata included.</p>
-</section>
-<section id="id5">
-<h4>Definition<a class="headerlink" href="#id5" title="Link to this heading"></a></h4>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">def</span> <span class="nf">saveMatfile</span><span class="p">(</span><span class="bp">self</span><span class="nd">@mzDataManager</span><span class="p">,</span> <span class="n">mzData</span> <span class="p">:</span> <span class="n">mzData</span><span class="p">,</span> <span class="n">remove</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">dir2Save</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">force</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span>
-</pre></div>
-</div>
-</section>
-<section id="id6">
-<h4>How to use<a class="headerlink" href="#id6" title="Link to this heading"></a></h4>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="c1"># Considering that mzDataManager class has been intialized before and stored as manager variable</span>
-
-<span class="c1"># Considering also the variable content which is the result of the function mzDataXMLread presented above</span>
-
-<span class="n">manager</span><span class="o">.</span><span class="n">saveMatFile</span><span class="p">(</span>
-    <span class="n">mzData</span><span class="o">=</span><span class="n">content</span>
-<span class="p">)</span>
-</pre></div>
-</div>
-<p><u>Parameters</u></p>
-<ul class="simple">
-<li><p><code class="docutils literal notranslate"><span class="pre">mzData</span></code> : The <code class="docutils literal notranslate"><span class="pre">mzData</span></code> structure to save as a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file. (See <a class="reference internal" href="matStructure.html"><span class="std std-doc">here</span></a> for the <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file structure)</p></li>
-<li><p><code class="docutils literal notranslate"><span class="pre">remove</span></code> : Should the original file (so the original <code class="docutils literal notranslate"><span class="pre">.mzData.xml</span></code> file) be removed when save is complete ?</p></li>
-<li><p><code class="docutils literal notranslate"><span class="pre">force</span></code> : If a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file already exists with the same name in the export folder, should it be replaced ? If this parameter is set to <code class="docutils literal notranslate"><span class="pre">False</span></code>, save will be aborted if a file is found.</p></li>
-<li><p>If directories were not provided during init process:</p>
-<ul>
-<li><p><code class="docutils literal notranslate"><span class="pre">dir2save</span></code> : Full directory specifying where to save the converted file. If this parameter is set while a directory was specified in the init process, this value is prioritized.</p></li>
-</ul>
-</li>
-</ul>
-<p><u>Outputs</u><br>
-If function ran correctly, no output, otherwise raises the error.</p>
-</section>
-</section>
-<section id="convertfile">
-<h3>convertFile<a class="headerlink" href="#convertfile" title="Link to this heading"></a></h3>
-<section id="id7">
-<h4>Presentation<a class="headerlink" href="#id7" title="Link to this heading"></a></h4>
-<p>All in one function. Reads <code class="docutils literal notranslate"><span class="pre">mzData.xml</span></code> file and automatically saves it into the export folder. No transition to the <code class="docutils literal notranslate"><span class="pre">mzData</span></code> class.</p>
-</section>
-<section id="id8">
-<h4>Definition<a class="headerlink" href="#id8" title="Link to this heading"></a></h4>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">def</span> <span class="nf">convertFile</span><span class="p">(</span><span class="bp">self</span><span class="nd">@mzDataManager</span><span class="p">,</span> <span class="n">fileName</span> <span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">customDirectory</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">dir2Save</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">force</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">remove</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span>
-</pre></div>
-</div>
-</section>
-<section id="id9">
-<h4>How to use<a class="headerlink" href="#id9" title="Link to this heading"></a></h4>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="c1"># Considering that mzDataManager class has been intialized before and stored as manager variable</span>
-
-<span class="n">manager</span><span class="o">.</span><span class="n">convertFile</span><span class="p">(</span>
-    <span class="n">fileName</span><span class="o">=</span><span class="n">FileName</span>
-<span class="p">)</span>
-</pre></div>
-</div>
-<p><u>Parameters</u></p>
-<ul class="simple">
-<li><p><code class="docutils literal notranslate"><span class="pre">fileName</span></code> :<br></p>
-<ul>
-<li><p>Should be the full path to the file and it’s extension (.mzdata.xml) to convert if no value was given to <code class="docutils literal notranslate"><span class="pre">mzDataPath</span></code> when initializing the class.</p></li>
-<li><p>Otherwise, the file’s relative path with it’s extension (.mzdata.xml)</p></li>
-</ul>
-</li>
-<li><p><code class="docutils literal notranslate"><span class="pre">customDirectory</span></code> : Set this parameter to <code class="docutils literal notranslate"><span class="pre">True</span></code> if the <code class="docutils literal notranslate"><span class="pre">fileName</span></code> is in a different path than the one given in configuration.</p></li>
-<li><p><code class="docutils literal notranslate"><span class="pre">dir2Save</span></code>   : Save directory to save the .mat file. If path was given in configuration, it is not needed. This parameter will be prioritised over the path given in configuration (if any).</p></li>
-<li><p><code class="docutils literal notranslate"><span class="pre">force</span></code>      : If a file has the same name in the converted folder, should it be replaced ? (File will not be saved if sibling found in convert folder and this parameter set to <code class="docutils literal notranslate"><span class="pre">False</span></code>.)</p></li>
-<li><p><code class="docutils literal notranslate"><span class="pre">remove</span></code>     : Should the original file be removed when it is saved as <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file ?</p></li>
-</ul>
-<p><u>Outputs</u><br>
-No outputs</p>
-</section>
-</section>
-</section>
-</section>
-
-
-           </div>
-          </div>
-          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="code-example.html" class="btn btn-neutral float-left" title="Example Code" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="matStructure.html" class="btn btn-neutral float-right" title="Matlab saving structure" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
-    </div>
-
-  <hr/>
-
-  <div role="contentinfo">
-    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
-  </div>
-
-  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
-    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
-    provided by <a href="https://readthedocs.org">Read the Docs</a>.
-   
-
-</footer>
-        </div>
-      </div>
-    </section>
-  </div>
-  <script>
-      jQuery(function () {
-          SphinxRtdTheme.Navigation.enable(true);
-      });
-  </script> 
-
-</body>
+<!DOCTYPE html>
+<html class="writer-html5" lang="en" data-content_root="./">
+<head>
+  <meta charset="utf-8" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>mzDataManager &mdash; mzdata2mat 0.2.0 documentation</title>
+      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
+      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
+
+  
+  <!--[if lt IE 9]>
+    <script src="_static/js/html5shiv.min.js"></script>
+  <![endif]-->
+  
+        <script src="_static/jquery.js?v=5d32c60e"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
+        <script src="_static/documentation_options.js?v=938c9ccc"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
+        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
+    <script src="_static/js/theme.js"></script>
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="matStruct" href="matStruct.html" />
+    <link rel="prev" title="Advanced load and save logic" href="advancedLoadSaveLogic.html" /> 
+</head>
+
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
+
+          
+          
+          <a href="index.html" class="icon icon-home">
+            mzdata2mat
+          </a>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
+<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Advanced</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="advancedLoadSaveLogic.html">Advanced load and save logic</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
+<ul class="current">
+<li class="toctree-l1 current"><a class="current reference internal" href="#">mzDataManager</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="#presentation">Presentation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#definition">Definition</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#how-to-use">How to use</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#with-path">With path</a></li>
+<li class="toctree-l3"><a class="reference internal" href="#without-path">Without path</a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="#functions">Functions</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#mzdataxmlread">mzDataXMLread</a><ul>
+<li class="toctree-l4"><a class="reference internal" href="#id1">Presentation</a></li>
+<li class="toctree-l4"><a class="reference internal" href="#id2">Definition</a></li>
+<li class="toctree-l4"><a class="reference internal" href="#id3">How to use</a></li>
+</ul>
+</li>
+<li class="toctree-l3"><a class="reference internal" href="#savematfile">saveMatfile</a><ul>
+<li class="toctree-l4"><a class="reference internal" href="#id5">Presentation</a></li>
+<li class="toctree-l4"><a class="reference internal" href="#id6">Definition</a></li>
+<li class="toctree-l4"><a class="reference internal" href="#id7">How to use</a></li>
+</ul>
+</li>
+<li class="toctree-l3"><a class="reference internal" href="#convertfile">convertFile</a><ul>
+<li class="toctree-l4"><a class="reference internal" href="#id8">Presentation</a></li>
+<li class="toctree-l4"><a class="reference internal" href="#id9">Definition</a></li>
+<li class="toctree-l4"><a class="reference internal" href="#id10">How to use</a></li>
+</ul>
+</li>
+</ul>
+</li>
+</ul>
+</li>
+<li class="toctree-l1"><a class="reference internal" href="matStruct.html">matStruct</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzDataXMLStruct.html">mzDataXMLStruct</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">CLI</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
+</ul>
+
+        </div>
+      </div>
+    </nav>
+
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">mzdata2mat</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">mzDataManager</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/mzDataManager.md.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+  <section id="mzdatamanager">
+<h1>mzDataManager<a class="headerlink" href="#mzdatamanager" title="Link to this heading"></a></h1>
+<section id="presentation">
+<h2>Presentation<a class="headerlink" href="#presentation" title="Link to this heading"></a></h2>
+<p>Main class used for converting mzData files into matlab files.</p>
+</section>
+<section id="definition">
+<h2>Definition<a class="headerlink" href="#definition" title="Link to this heading"></a></h2>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">class</span> <span class="nc">mzDataManager</span><span class="p">(</span><span class="n">BaseModel</span><span class="p">):</span>
+    <span class="n">mzDataPath</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
+    <span class="n">exportPath</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
+    <span class="n">useDirectory</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</pre></div>
+</div>
+</section>
+<section id="how-to-use">
+<h2>How to use<a class="headerlink" href="#how-to-use" title="Link to this heading"></a></h2>
+<section id="with-path">
+<h3>With path<a class="headerlink" href="#with-path" title="Link to this heading"></a></h3>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="n">manager</span> <span class="o">=</span> <span class="n">mzDataManager</span><span class="p">(</span>
+    <span class="n">mzDataPath</span> <span class="o">=</span> <span class="s2">&quot;Some/Path&quot;</span><span class="p">,</span>
+    <span class="n">exportPath</span> <span class="o">=</span> <span class="s2">&quot;Some/Export/Path&quot;</span><span class="p">,</span>
+<span class="p">)</span>
+</pre></div>
+</div>
+<p>The path you specify in those arguments will be stored in the class, so when you use the integrated functions, you only need to specify the relative path to the file.</p>
+</section>
+<section id="without-path">
+<h3>Without path<a class="headerlink" href="#without-path" title="Link to this heading"></a></h3>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="n">manager</span> <span class="o">=</span> <span class="n">mzDataManager</span><span class="p">(</span><span class="n">useDirectory</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+</pre></div>
+</div>
+<p>Setting up the class this way will require to specify each time you call a function to give the full path and the export directory.</p>
+</section>
+</section>
+<section id="functions">
+<h2>Functions<a class="headerlink" href="#functions" title="Link to this heading"></a></h2>
+<section id="mzdataxmlread">
+<h3>mzDataXMLread<a class="headerlink" href="#mzdataxmlread" title="Link to this heading"></a></h3>
+<section id="id1">
+<h4>Presentation<a class="headerlink" href="#id1" title="Link to this heading"></a></h4>
+<p>This function reads a <code class="docutils literal notranslate"><span class="pre">.mzData.xml</span></code> file and returns a <code class="docutils literal notranslate"><span class="pre">mzData</span></code> structure which can be modified before saving it’s data to a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file (See <a class="reference internal" href="mzData.html"><span class="std std-doc">mzData</span></a> class for further details).</p>
+</section>
+<section id="id2">
+<h4>Definition<a class="headerlink" href="#id2" title="Link to this heading"></a></h4>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">def</span> <span class="nf">mzDataXMLread</span><span class="p">(</span><span class="bp">self</span><span class="nd">@mzDataManager</span><span class="p">,</span> <span class="n">fileName</span> <span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">customDirectory</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span>
+</pre></div>
+</div>
+</section>
+<section id="id3">
+<h4>How to use<a class="headerlink" href="#id3" title="Link to this heading"></a></h4>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="c1"># Considering that mzDataManager class has been intialized before and stored as manager variable</span>
+
+<span class="n">content</span> <span class="o">=</span> <span class="n">manager</span><span class="o">.</span><span class="n">mzDataXMLread</span><span class="p">(</span>
+    <span class="n">fileName</span><span class="o">=</span><span class="n">Path2File</span>
+<span class="p">)</span>
+</pre></div>
+</div>
+<p><u>Parameters</u></p>
+<ul class="simple">
+<li><p>If directories were provided in the init process :</p>
+<ul>
+<li><p><code class="docutils literal notranslate"><span class="pre">fileName</span></code> : Relative path of the <code class="docutils literal notranslate"><span class="pre">mzData.xml</span></code> file to read</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">customDirectory</span></code> : Set this parameter to <code class="docutils literal notranslate"><span class="pre">True</span></code> if you provide a full path which is different than the one specified in the init process.</p></li>
+</ul>
+</li>
+<li><p>Otherwise :</p>
+<ul>
+<li><p><code class="docutils literal notranslate"><span class="pre">fileName</span></code> : Full path to the <code class="docutils literal notranslate"><span class="pre">mzData.xml</span></code> file to read</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">customDirectory</span></code> : Does nothing</p></li>
+</ul>
+</li>
+</ul>
+<p><u>Outputs</u></p>
+<ul class="simple">
+<li><p>Outputs a <code class="docutils literal notranslate"><span class="pre">mzData</span></code> class containing the content of the file parsed.</p></li>
+</ul>
+</section>
+</section>
+<section id="savematfile">
+<span id="id4"></span><h3>saveMatfile<a class="headerlink" href="#savematfile" title="Link to this heading"></a></h3>
+<section id="id5">
+<h4>Presentation<a class="headerlink" href="#id5" title="Link to this heading"></a></h4>
+<p>Saves a <code class="docutils literal notranslate"><span class="pre">mzData</span></code> class into a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file with all metadata included.</p>
+</section>
+<section id="id6">
+<h4>Definition<a class="headerlink" href="#id6" title="Link to this heading"></a></h4>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">def</span> <span class="nf">saveMatfile</span><span class="p">(</span><span class="bp">self</span><span class="nd">@mzDataManager</span><span class="p">,</span> <span class="n">mzData</span> <span class="p">:</span> <span class="n">mzData</span><span class="p">,</span> <span class="n">remove</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">dir2Save</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">force</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span>
+</pre></div>
+</div>
+</section>
+<section id="id7">
+<h4>How to use<a class="headerlink" href="#id7" title="Link to this heading"></a></h4>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="c1"># Considering that mzDataManager class has been intialized before and stored as manager variable</span>
+
+<span class="c1"># Considering also the variable content which is the result of the function mzDataXMLread presented above</span>
+
+<span class="n">manager</span><span class="o">.</span><span class="n">saveMatFile</span><span class="p">(</span>
+    <span class="n">mzData</span><span class="o">=</span><span class="n">content</span>
+<span class="p">)</span>
+</pre></div>
+</div>
+<p><u>Parameters</u></p>
+<ul class="simple">
+<li><p><code class="docutils literal notranslate"><span class="pre">mzData</span></code> : The <code class="docutils literal notranslate"><span class="pre">mzData</span></code> structure to save as a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file. (See <a class="reference internal" href="matStruct.html"><span class="std std-doc">here</span></a> for the <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file structure)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">remove</span></code> : Should the original file (so the original <code class="docutils literal notranslate"><span class="pre">.mzData.xml</span></code> file) be removed when save is complete ?</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">force</span></code> : If a <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file already exists with the same name in the export folder, should it be replaced ? If this parameter is set to <code class="docutils literal notranslate"><span class="pre">False</span></code>, save will be aborted if a file is found.</p></li>
+<li><p>If directories were not provided during init process:</p>
+<ul>
+<li><p><code class="docutils literal notranslate"><span class="pre">dir2save</span></code> : Full directory specifying where to save the converted file. If this parameter is set while a directory was specified in the init process, this value is prioritized.</p></li>
+</ul>
+</li>
+</ul>
+<p><u>Outputs</u><br>
+If function ran correctly, no output, otherwise raises the error.</p>
+</section>
+</section>
+<section id="convertfile">
+<h3>convertFile<a class="headerlink" href="#convertfile" title="Link to this heading"></a></h3>
+<section id="id8">
+<h4>Presentation<a class="headerlink" href="#id8" title="Link to this heading"></a></h4>
+<p>All in one function. Reads <code class="docutils literal notranslate"><span class="pre">mzData.xml</span></code> file and automatically saves it into the export folder. No transition to the <code class="docutils literal notranslate"><span class="pre">mzData</span></code> class.</p>
+</section>
+<section id="id9">
+<h4>Definition<a class="headerlink" href="#id9" title="Link to this heading"></a></h4>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">def</span> <span class="nf">convertFile</span><span class="p">(</span><span class="bp">self</span><span class="nd">@mzDataManager</span><span class="p">,</span> <span class="n">fileName</span> <span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">customDirectory</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">dir2Save</span> <span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">force</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">remove</span> <span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span>
+</pre></div>
+</div>
+</section>
+<section id="id10">
+<h4>How to use<a class="headerlink" href="#id10" title="Link to this heading"></a></h4>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="c1"># Considering that mzDataManager class has been intialized before and stored as manager variable</span>
+
+<span class="n">manager</span><span class="o">.</span><span class="n">convertFile</span><span class="p">(</span>
+    <span class="n">fileName</span><span class="o">=</span><span class="n">FileName</span>
+<span class="p">)</span>
+</pre></div>
+</div>
+<p><u>Parameters</u></p>
+<ul class="simple">
+<li><p><code class="docutils literal notranslate"><span class="pre">fileName</span></code> :<br></p>
+<ul>
+<li><p>Should be the full path to the file and it’s extension (.mzdata.xml) to convert if no value was given to <code class="docutils literal notranslate"><span class="pre">mzDataPath</span></code> when initializing the class.</p></li>
+<li><p>Otherwise, the file’s relative path with it’s extension (.mzdata.xml)</p></li>
+</ul>
+</li>
+<li><p><code class="docutils literal notranslate"><span class="pre">customDirectory</span></code> : Set this parameter to <code class="docutils literal notranslate"><span class="pre">True</span></code> if the <code class="docutils literal notranslate"><span class="pre">fileName</span></code> is in a different path than the one given in configuration.</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">dir2Save</span></code>   : Save directory to save the .mat file. If path was given in configuration, it is not needed. This parameter will be prioritised over the path given in configuration (if any).</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">force</span></code>      : If a file has the same name in the converted folder, should it be replaced ? (File will not be saved if sibling found in convert folder and this parameter set to <code class="docutils literal notranslate"><span class="pre">False</span></code>.)</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">remove</span></code>     : Should the original file be removed when it is saved as <code class="docutils literal notranslate"><span class="pre">.mat</span></code> file ?</p></li>
+</ul>
+<p><u>Outputs</u><br>
+No outputs</p>
+</section>
+</section>
+</section>
+</section>
+
+
+           </div>
+          </div>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="advancedLoadSaveLogic.html" class="btn btn-neutral float-left" title="Advanced load and save logic" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="matStruct.html" class="btn btn-neutral float-right" title="matStruct" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+    </div>
+
+  <hr/>
+
+  <div role="contentinfo">
+    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
+
+</footer>
+        </div>
+      </div>
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
+
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 _m_z_d_a_t_a_2_m_a_t
 [q                   ]
 Infos
     * _C_h_a_n_g_e_l_o_g
 Quickstart
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _E_x_a_m_p_l_e_ _C_o_d_e
+Advanced
+    * _A_d_v_a_n_c_e_d_ _l_o_a_d_ _a_n_d_ _s_a_v_e_ _l_o_g_i_c
 API Reference
     * _m_z_D_a_t_a_M_a_n_a_g_e_r
           o _P_r_e_s_e_n_t_a_t_i_o_n
           o _D_e_f_i_n_i_t_i_o_n
           o _H_o_w_ _t_o_ _u_s_e
                 # _W_i_t_h_ _p_a_t_h
                 # _W_i_t_h_o_u_t_ _p_a_t_h
@@ -21,18 +23,19 @@
                       # _P_r_e_s_e_n_t_a_t_i_o_n
                       # _D_e_f_i_n_i_t_i_o_n
                       # _H_o_w_ _t_o_ _u_s_e
                 # _c_o_n_v_e_r_t_F_i_l_e
                       # _P_r_e_s_e_n_t_a_t_i_o_n
                       # _D_e_f_i_n_i_t_i_o_n
                       # _H_o_w_ _t_o_ _u_s_e
-    * _M_a_t_l_a_b_ _s_a_v_i_n_g_ _s_t_r_u_c_t_u_r_e
+    * _m_a_t_S_t_r_u_c_t
     * _m_z_D_a_t_a
-    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
     * _m_z_D_a_t_a_X_M_L_S_t_r_u_c_t
+CLI
+    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
 _m_z_d_a_t_a_2_m_a_t
     * mzDataManager
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ mmzzDDaattaaMMaannaaggeerr_? ************
 ********** PPrreesseennttaattiioonn_? **********
 Main class used for converting mzData files into matlab files.
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/mzDataXMLStruct.html` & `mzdata2mat-0.2.0/docs/build/html/mzDataXMLStruct.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,161 +1,170 @@
-<!DOCTYPE html>
-<html class="writer-html5" lang="en" data-content_root="./">
-<head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>mzDataXMLStruct &mdash; mzdata2mat 0.1.0 documentation</title>
-      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
-      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
-
-  
-  <!--[if lt IE 9]>
-    <script src="_static/js/html5shiv.min.js"></script>
-  <![endif]-->
-  
-        <script src="_static/jquery.js?v=5d32c60e"></script>
-        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="_static/documentation_options.js?v=01f34227"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
-        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
-    <script src="_static/js/theme.js"></script>
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="prev" title="mzdata2mat-verify" href="mzdata2mat-verify.html" /> 
-</head>
-
-<body class="wy-body-for-nav"> 
-  <div class="wy-grid-for-nav">
-    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
-      <div class="wy-side-scroll">
-        <div class="wy-side-nav-search" >
-
-          
-          
-          <a href="index.html" class="icon icon-home">
-            mzdata2mat
-          </a>
-<div role="search">
-  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
-    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
-    <input type="hidden" name="check_keywords" value="yes" />
-    <input type="hidden" name="area" value="default" />
-  </form>
-</div>
-        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
-<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
-</ul>
-<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
-<ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
-<li class="toctree-l1"><a class="reference internal" href="matStructure.html">Matlab saving structure</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
-<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
-<li class="toctree-l1 current"><a class="current reference internal" href="#">mzDataXMLStruct</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#presentation">Presentation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#definition">Definition</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#how-to-use">How to use</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#functions">Functions</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#notes">Notes</a></li>
-</ul>
-</li>
-</ul>
-
-        </div>
-      </div>
-    </nav>
-
-    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
-          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
-          <a href="index.html">mzdata2mat</a>
-      </nav>
-
-      <div class="wy-nav-content">
-        <div class="rst-content">
-          <div role="navigation" aria-label="Page navigation">
-  <ul class="wy-breadcrumbs">
-      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
-      <li class="breadcrumb-item active">mzDataXMLStruct</li>
-      <li class="wy-breadcrumbs-aside">
-            <a href="_sources/mzDataXMLStruct.md.txt" rel="nofollow"> View page source</a>
-      </li>
-  </ul>
-  <hr/>
-</div>
-          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
-           <div itemprop="articleBody">
-             
-  <section id="mzdataxmlstruct">
-<h1>mzDataXMLStruct<a class="headerlink" href="#mzdataxmlstruct" title="Link to this heading"></a></h1>
-<section id="presentation">
-<h2>Presentation<a class="headerlink" href="#presentation" title="Link to this heading"></a></h2>
-<p>Internal class, do not use it to store data. Consider using <a class="reference internal" href="mzData.html"><span class="std std-doc">mzData</span></a> class instead.</p>
-</section>
-<section id="definition">
-<h2>Definition<a class="headerlink" href="#definition" title="Link to this heading"></a></h2>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">class</span> <span class="nc">mzDataXMLStruct</span><span class="p">(</span><span class="n">BaseModel</span><span class="p">):</span>
-    <span class="n">metadata</span> <span class="p">:</span> <span class="nb">dict</span>
-    <span class="n">times</span> <span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span>
-    <span class="n">series</span> <span class="p">:</span> <span class="n">Any</span>
-</pre></div>
-</div>
-</section>
-<section id="how-to-use">
-<h2>How to use<a class="headerlink" href="#how-to-use" title="Link to this heading"></a></h2>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="n">value</span> <span class="o">=</span> <span class="n">mzDataXMLStruct</span><span class="p">(</span>
-    <span class="n">metadata</span> <span class="o">=</span> <span class="n">someDict</span><span class="p">,</span>
-    <span class="n">times</span> <span class="o">=</span> <span class="n">listOfTimes</span><span class="p">,</span>
-    <span class="n">series</span> <span class="o">=</span> <span class="n">series</span>
-<span class="p">)</span>
-</pre></div>
-</div>
-</section>
-<section id="functions">
-<h2>Functions<a class="headerlink" href="#functions" title="Link to this heading"></a></h2>
-<p>None</p>
-</section>
-<section id="notes">
-<h2>Notes<a class="headerlink" href="#notes" title="Link to this heading"></a></h2>
-<p>This is an <strong>internal</strong> class, it shouldn’t be used to store mz values. This class is automatically populated when parsing a <code class="docutils literal notranslate"><span class="pre">.mzData.xml</span></code> file and is private.</p>
-<p>Consider using <a class="reference internal" href="mzData.html"><span class="std std-doc">mzData</span></a> class to store your mz and intensities values.</p>
-</section>
-</section>
-
-
-           </div>
-          </div>
-          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="mzdata2mat-verify.html" class="btn btn-neutral float-left" title="mzdata2mat-verify" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-    </div>
-
-  <hr/>
-
-  <div role="contentinfo">
-    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
-  </div>
-
-  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
-    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
-    provided by <a href="https://readthedocs.org">Read the Docs</a>.
-   
-
-</footer>
-        </div>
-      </div>
-    </section>
-  </div>
-  <script>
-      jQuery(function () {
-          SphinxRtdTheme.Navigation.enable(true);
-      });
-  </script> 
-
-</body>
+<!DOCTYPE html>
+<html class="writer-html5" lang="en" data-content_root="./">
+<head>
+  <meta charset="utf-8" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>mzDataXMLStruct &mdash; mzdata2mat 0.2.0 documentation</title>
+      <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
+      <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
+
+  
+  <!--[if lt IE 9]>
+    <script src="_static/js/html5shiv.min.js"></script>
+  <![endif]-->
+  
+        <script src="_static/jquery.js?v=5d32c60e"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
+        <script src="_static/documentation_options.js?v=938c9ccc"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
+        <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
+    <script src="_static/js/theme.js"></script>
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="mzdata2mat-verify" href="mzdata2mat-verify.html" />
+    <link rel="prev" title="mzData" href="mzData.html" /> 
+</head>
+
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
+
+          
+          
+          <a href="index.html" class="icon icon-home">
+            mzdata2mat
+          </a>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Infos</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="Changelog.html">Changelog</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Quickstart</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
+<li class="toctree-l1"><a class="reference internal" href="code-example.html">Example Code</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">Advanced</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="advancedLoadSaveLogic.html">Advanced load and save logic</a></li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">API Reference</span></p>
+<ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="mzDataManager.html">mzDataManager</a></li>
+<li class="toctree-l1"><a class="reference internal" href="matStruct.html">matStruct</a></li>
+<li class="toctree-l1"><a class="reference internal" href="mzData.html">mzData</a></li>
+<li class="toctree-l1 current"><a class="current reference internal" href="#">mzDataXMLStruct</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="#presentation">Presentation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#definition">Definition</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#how-to-use">How to use</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#functions">Functions</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#notes">Notes</a></li>
+</ul>
+</li>
+</ul>
+<p class="caption" role="heading"><span class="caption-text">CLI</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="mzdata2mat-verify.html">mzdata2mat-verify</a></li>
+</ul>
+
+        </div>
+      </div>
+    </nav>
+
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">mzdata2mat</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">mzDataXMLStruct</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/mzDataXMLStruct.md.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+  <section id="mzdataxmlstruct">
+<h1>mzDataXMLStruct<a class="headerlink" href="#mzdataxmlstruct" title="Link to this heading"></a></h1>
+<section id="presentation">
+<h2>Presentation<a class="headerlink" href="#presentation" title="Link to this heading"></a></h2>
+<p>Internal class, do not use it to store data. Consider using <a class="reference internal" href="mzData.html"><span class="std std-doc">mzData</span></a> class instead.</p>
+</section>
+<section id="definition">
+<h2>Definition<a class="headerlink" href="#definition" title="Link to this heading"></a></h2>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="k">class</span> <span class="nc">mzDataXMLStruct</span><span class="p">(</span><span class="n">BaseModel</span><span class="p">):</span>
+    <span class="n">metadata</span> <span class="p">:</span> <span class="nb">dict</span>
+    <span class="n">times</span> <span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span>
+    <span class="n">series</span> <span class="p">:</span> <span class="n">Any</span>
+</pre></div>
+</div>
+</section>
+<section id="how-to-use">
+<h2>How to use<a class="headerlink" href="#how-to-use" title="Link to this heading"></a></h2>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="n">value</span> <span class="o">=</span> <span class="n">mzDataXMLStruct</span><span class="p">(</span>
+    <span class="n">metadata</span> <span class="o">=</span> <span class="n">someDict</span><span class="p">,</span>
+    <span class="n">times</span> <span class="o">=</span> <span class="n">listOfTimes</span><span class="p">,</span>
+    <span class="n">series</span> <span class="o">=</span> <span class="n">series</span>
+<span class="p">)</span>
+</pre></div>
+</div>
+</section>
+<section id="functions">
+<h2>Functions<a class="headerlink" href="#functions" title="Link to this heading"></a></h2>
+<p>None</p>
+</section>
+<section id="notes">
+<h2>Notes<a class="headerlink" href="#notes" title="Link to this heading"></a></h2>
+<p>This is an <strong>internal</strong> class, it shouldn’t be used to store mz values. This class is automatically populated when parsing a <code class="docutils literal notranslate"><span class="pre">.mzData.xml</span></code> file and is private.</p>
+<p>Consider using <a class="reference internal" href="mzData.html"><span class="std std-doc">mzData</span></a> class to store your mz and intensities values.</p>
+</section>
+</section>
+
+
+           </div>
+          </div>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="mzData.html" class="btn btn-neutral float-left" title="mzData" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="mzdata2mat-verify.html" class="btn btn-neutral float-right" title="mzdata2mat-verify" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+    </div>
+
+  <hr/>
+
+  <div role="contentinfo">
+    <p>&#169; Copyright 2024, CORDELLA Maxime.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
+
+</footer>
+        </div>
+      </div>
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
+
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,25 +1,28 @@
 _m_z_d_a_t_a_2_m_a_t
 [q                   ]
 Infos
     * _C_h_a_n_g_e_l_o_g
 Quickstart
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _E_x_a_m_p_l_e_ _C_o_d_e
+Advanced
+    * _A_d_v_a_n_c_e_d_ _l_o_a_d_ _a_n_d_ _s_a_v_e_ _l_o_g_i_c
 API Reference
     * _m_z_D_a_t_a_M_a_n_a_g_e_r
-    * _M_a_t_l_a_b_ _s_a_v_i_n_g_ _s_t_r_u_c_t_u_r_e
+    * _m_a_t_S_t_r_u_c_t
     * _m_z_D_a_t_a
-    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
     * _m_z_D_a_t_a_X_M_L_S_t_r_u_c_t
           o _P_r_e_s_e_n_t_a_t_i_o_n
           o _D_e_f_i_n_i_t_i_o_n
           o _H_o_w_ _t_o_ _u_s_e
           o _F_u_n_c_t_i_o_n_s
           o _N_o_t_e_s
+CLI
+    * _m_z_d_a_t_a_2_m_a_t_-_v_e_r_i_f_y
 _m_z_d_a_t_a_2_m_a_t
     * mzDataXMLStruct
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ mmzzDDaattaaXXMMLLSSttrruucctt_? ************
 ********** PPrreesseennttaattiioonn_? **********
 Internal class, do not use it to store data. Consider using _m_z_D_a_t_a class
@@ -37,11 +40,11 @@
 )
 ********** FFuunnccttiioonnss_? **********
 None
 ********** NNootteess_? **********
 This is an iinntteerrnnaall class, it shouldn’t be used to store mz values. This class
 is automatically populated when parsing a .mzData.xml file and is private.
 Consider using _m_z_D_a_t_a class to store your mz and intensities values.
-_P_r_e_v_i_o_u_s
+_P_r_e_v_i_o_u_s _N_e_x_t
 ===============================================================================
 © Copyright 2024, CORDELLA Maxime.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/_sources/code-example.md.txt` & `mzdata2mat-0.2.0/docs/build/html/_sources/code-example.md.txt`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_sources/installation.md.txt` & `mzdata2mat-0.2.0/docs/build/html/_sources/installation.md.txt`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_sources/mzDataManager.md.txt` & `mzdata2mat-0.2.0/docs/build/html/_sources/mzDataManager.md.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 - Otherwise :
     - `fileName` : Full path to the `mzData.xml` file to read
     - `customDirectory` : Does nothing
 
 <u>Outputs</u>
 - Outputs a `mzData` class containing the content of the file parsed.
 
+(savematfile)=
 ### saveMatfile
 #### Presentation
 Saves a `mzData` class into a `.mat` file with all metadata included.
 
 #### Definition
 ```python
 def saveMatfile(self@mzDataManager, mzData : mzData, remove : bool = False, dir2Save : str = None, force : bool = False)
@@ -74,15 +75,15 @@
 # Considering also the variable content which is the result of the function mzDataXMLread presented above
 
 manager.saveMatFile(
     mzData=content
 )
 ```
 <u>Parameters</u>
-- `mzData` : The `mzData` structure to save as a `.mat` file. (See [here](matStructure.md) for the `.mat` file structure)
+- `mzData` : The `mzData` structure to save as a `.mat` file. (See [here](matStruct.md) for the `.mat` file structure)
 - `remove` : Should the original file (so the original `.mzData.xml` file) be removed when save is complete ?
 - `force` : If a `.mat` file already exists with the same name in the export folder, should it be replaced ? If this parameter is set to `False`, save will be aborted if a file is found.
 - If directories were not provided during init process:
     - `dir2save` : Full directory specifying where to save the converted file. If this parameter is set while a directory was specified in the init process, this value is prioritized.
 
 <u>Outputs</u><br>
 If function ran correctly, no output, otherwise raises the error.
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/_sources/mzDataXMLStruct.md.txt` & `mzdata2mat-0.2.0/docs/build/html/_sources/mzDataXMLStruct.md.txt`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_sources/mzdata2mat-verify.md.txt` & `mzdata2mat-0.2.0/docs/build/html/_sources/mzdata2mat-verify.md.txt`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `mzdata2mat-0.2.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/doctools.js` & `mzdata2mat-0.2.0/docs/build/html/_static/doctools.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * doctools.js
  * ~~~~~~~~~~~
  *
  * Base JavaScript utilities for all Sphinx HTML documentation.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 const BLACKLISTED_KEY_CONTROL_ELEMENTS = new Set([
     "TEXTAREA",
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/jquery.js` & `mzdata2mat-0.2.0/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/language_data.js` & `mzdata2mat-0.2.0/docs/build/html/_static/language_data.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,195 +1,195 @@
-/*
- * language_data.js
- * ~~~~~~~~~~~~~~~~
- *
- * This script contains the language-specific data used by searchtools.js,
- * namely the list of stopwords, stemmer, scorer and splitter.
- *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
- * :license: BSD, see LICENSE for details.
- *
- */
-
-var stopwords = ["a", "and", "are", "as", "at", "be", "but", "by", "for", "if", "in", "into", "is", "it", "near", "no", "not", "of", "on", "or", "such", "that", "the", "their", "then", "there", "these", "they", "this", "to", "was", "will", "with"];
-
-
-/* Non-minified version is copied as a separate JS file, is available */
-
-/**
- * Porter Stemmer
- */
-var Stemmer = function() {
-
-    var step2list = {
-        ational: 'ate',
-        tional: 'tion',
-        enci: 'ence',
-        anci: 'ance',
-        izer: 'ize',
-        bli: 'ble',
-        alli: 'al',
-        entli: 'ent',
-        eli: 'e',
-        ousli: 'ous',
-        ization: 'ize',
-        ation: 'ate',
-        ator: 'ate',
-        alism: 'al',
-        iveness: 'ive',
-        fulness: 'ful',
-        ousness: 'ous',
-        aliti: 'al',
-        iviti: 'ive',
-        biliti: 'ble',
-        logi: 'log'
-    };
-
-    var step3list = {
-        icate: 'ic',
-        ative: '',
-        alize: 'al',
-        iciti: 'ic',
-        ical: 'ic',
-        ful: '',
-        ness: ''
-    };
-
-    var c = "[^aeiou]"; // consonant
-    var v = "[aeiouy]"; // vowel
-    var C = c + "[^aeiouy]*"; // consonant sequence
-    var V = v + "[aeiou]*"; // vowel sequence
-
-    var mgr0 = "^(" + C + ")?" + V + C; // [C]VC... is m>0
-    var meq1 = "^(" + C + ")?" + V + C + "(" + V + ")?$"; // [C]VC[V] is m=1
-    var mgr1 = "^(" + C + ")?" + V + C + V + C; // [C]VCVC... is m>1
-    var s_v = "^(" + C + ")?" + v; // vowel in stem
-
-    this.stemWord = function(w) {
-        var stem;
-        var suffix;
-        var firstch;
-        var origword = w;
-
-        if (w.length < 3)
-            return w;
-
-        var re;
-        var re2;
-        var re3;
-        var re4;
-
-        firstch = w.substr(0, 1);
-        if (firstch == "y")
-            w = firstch.toUpperCase() + w.substr(1);
-
-        // Step 1a
-        re = /^(.+?)(ss|i)es$/;
-        re2 = /^(.+?)([^s])s$/;
-
-        if (re.test(w))
-            w = w.replace(re, "$1$2");
-        else if (re2.test(w))
-            w = w.replace(re2, "$1$2");
-
-        // Step 1b
-        re = /^(.+?)eed$/;
-        re2 = /^(.+?)(ed|ing)$/;
-        if (re.test(w)) {
-            var fp = re.exec(w);
-            re = new RegExp(mgr0);
-            if (re.test(fp[1])) {
-                re = /.$/;
-                w = w.replace(re, "");
-            }
-        } else if (re2.test(w)) {
-            var fp = re2.exec(w);
-            stem = fp[1];
-            re2 = new RegExp(s_v);
-            if (re2.test(stem)) {
-                w = stem;
-                re2 = /(at|bl|iz)$/;
-                re3 = new RegExp("([^aeiouylsz])\\1$");
-                re4 = new RegExp("^" + C + v + "[^aeiouwxy]$");
-                if (re2.test(w))
-                    w = w + "e";
-                else if (re3.test(w)) {
-                    re = /.$/;
-                    w = w.replace(re, "");
-                } else if (re4.test(w))
-                    w = w + "e";
-            }
-        }
-
-        // Step 1c
-        re = /^(.+?)y$/;
-        if (re.test(w)) {
-            var fp = re.exec(w);
-            stem = fp[1];
-            re = new RegExp(s_v);
-            if (re.test(stem))
-                w = stem + "i";
-        }
-
-        // Step 2
-        re = /^(.+?)(ational|tional|enci|anci|izer|bli|alli|entli|eli|ousli|ization|ation|ator|alism|iveness|fulness|ousness|aliti|iviti|biliti|logi)$/;
-        if (re.test(w)) {
-            var fp = re.exec(w);
-            stem = fp[1];
-            suffix = fp[2];
-            re = new RegExp(mgr0);
-            if (re.test(stem))
-                w = stem + step2list[suffix];
-        }
-
-        // Step 3
-        re = /^(.+?)(icate|ative|alize|iciti|ical|ful|ness)$/;
-        if (re.test(w)) {
-            var fp = re.exec(w);
-            stem = fp[1];
-            suffix = fp[2];
-            re = new RegExp(mgr0);
-            if (re.test(stem))
-                w = stem + step3list[suffix];
-        }
-
-        // Step 4
-        re = /^(.+?)(al|ance|ence|er|ic|able|ible|ant|ement|ment|ent|ou|ism|ate|iti|ous|ive|ize)$/;
-        re2 = /^(.+?)(s|t)(ion)$/;
-        if (re.test(w)) {
-            var fp = re.exec(w);
-            stem = fp[1];
-            re = new RegExp(mgr1);
-            if (re.test(stem))
-                w = stem;
-        } else if (re2.test(w)) {
-            var fp = re2.exec(w);
-            stem = fp[1] + fp[2];
-            re2 = new RegExp(mgr1);
-            if (re2.test(stem))
-                w = stem;
-        }
-
-        // Step 5
-        re = /^(.+?)e$/;
-        if (re.test(w)) {
-            var fp = re.exec(w);
-            stem = fp[1];
-            re = new RegExp(mgr1);
-            re2 = new RegExp(meq1);
-            re3 = new RegExp("^" + C + v + "[^aeiouwxy]$");
-            if (re.test(stem) || (re2.test(stem) && !(re3.test(stem))))
-                w = stem;
-        }
-        re = /ll$/;
-        re2 = new RegExp(mgr1);
-        if (re.test(w) && re2.test(w)) {
-            re = /.$/;
-            w = w.replace(re, "");
-        }
-
-        // and turn initial Y back to y
-        if (firstch == "y")
-            w = firstch.toLowerCase() + w.substr(1);
-        return w;
-    }
+/*
+ * language_data.js
+ * ~~~~~~~~~~~~~~~~
+ *
+ * This script contains the language-specific data used by searchtools.js,
+ * namely the list of stopwords, stemmer, scorer and splitter.
+ *
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
+ * :license: BSD, see LICENSE for details.
+ *
+ */
+
+var stopwords = ["a", "and", "are", "as", "at", "be", "but", "by", "for", "if", "in", "into", "is", "it", "near", "no", "not", "of", "on", "or", "such", "that", "the", "their", "then", "there", "these", "they", "this", "to", "was", "will", "with"];
+
+
+/* Non-minified version is copied as a separate JS file, if available */
+
+/**
+ * Porter Stemmer
+ */
+var Stemmer = function() {
+
+    var step2list = {
+        ational: 'ate',
+        tional: 'tion',
+        enci: 'ence',
+        anci: 'ance',
+        izer: 'ize',
+        bli: 'ble',
+        alli: 'al',
+        entli: 'ent',
+        eli: 'e',
+        ousli: 'ous',
+        ization: 'ize',
+        ation: 'ate',
+        ator: 'ate',
+        alism: 'al',
+        iveness: 'ive',
+        fulness: 'ful',
+        ousness: 'ous',
+        aliti: 'al',
+        iviti: 'ive',
+        biliti: 'ble',
+        logi: 'log'
+    };
+
+    var step3list = {
+        icate: 'ic',
+        ative: '',
+        alize: 'al',
+        iciti: 'ic',
+        ical: 'ic',
+        ful: '',
+        ness: ''
+    };
+
+    var c = "[^aeiou]"; // consonant
+    var v = "[aeiouy]"; // vowel
+    var C = c + "[^aeiouy]*"; // consonant sequence
+    var V = v + "[aeiou]*"; // vowel sequence
+
+    var mgr0 = "^(" + C + ")?" + V + C; // [C]VC... is m>0
+    var meq1 = "^(" + C + ")?" + V + C + "(" + V + ")?$"; // [C]VC[V] is m=1
+    var mgr1 = "^(" + C + ")?" + V + C + V + C; // [C]VCVC... is m>1
+    var s_v = "^(" + C + ")?" + v; // vowel in stem
+
+    this.stemWord = function(w) {
+        var stem;
+        var suffix;
+        var firstch;
+        var origword = w;
+
+        if (w.length < 3)
+            return w;
+
+        var re;
+        var re2;
+        var re3;
+        var re4;
+
+        firstch = w.substr(0, 1);
+        if (firstch == "y")
+            w = firstch.toUpperCase() + w.substr(1);
+
+        // Step 1a
+        re = /^(.+?)(ss|i)es$/;
+        re2 = /^(.+?)([^s])s$/;
+
+        if (re.test(w))
+            w = w.replace(re, "$1$2");
+        else if (re2.test(w))
+            w = w.replace(re2, "$1$2");
+
+        // Step 1b
+        re = /^(.+?)eed$/;
+        re2 = /^(.+?)(ed|ing)$/;
+        if (re.test(w)) {
+            var fp = re.exec(w);
+            re = new RegExp(mgr0);
+            if (re.test(fp[1])) {
+                re = /.$/;
+                w = w.replace(re, "");
+            }
+        } else if (re2.test(w)) {
+            var fp = re2.exec(w);
+            stem = fp[1];
+            re2 = new RegExp(s_v);
+            if (re2.test(stem)) {
+                w = stem;
+                re2 = /(at|bl|iz)$/;
+                re3 = new RegExp("([^aeiouylsz])\\1$");
+                re4 = new RegExp("^" + C + v + "[^aeiouwxy]$");
+                if (re2.test(w))
+                    w = w + "e";
+                else if (re3.test(w)) {
+                    re = /.$/;
+                    w = w.replace(re, "");
+                } else if (re4.test(w))
+                    w = w + "e";
+            }
+        }
+
+        // Step 1c
+        re = /^(.+?)y$/;
+        if (re.test(w)) {
+            var fp = re.exec(w);
+            stem = fp[1];
+            re = new RegExp(s_v);
+            if (re.test(stem))
+                w = stem + "i";
+        }
+
+        // Step 2
+        re = /^(.+?)(ational|tional|enci|anci|izer|bli|alli|entli|eli|ousli|ization|ation|ator|alism|iveness|fulness|ousness|aliti|iviti|biliti|logi)$/;
+        if (re.test(w)) {
+            var fp = re.exec(w);
+            stem = fp[1];
+            suffix = fp[2];
+            re = new RegExp(mgr0);
+            if (re.test(stem))
+                w = stem + step2list[suffix];
+        }
+
+        // Step 3
+        re = /^(.+?)(icate|ative|alize|iciti|ical|ful|ness)$/;
+        if (re.test(w)) {
+            var fp = re.exec(w);
+            stem = fp[1];
+            suffix = fp[2];
+            re = new RegExp(mgr0);
+            if (re.test(stem))
+                w = stem + step3list[suffix];
+        }
+
+        // Step 4
+        re = /^(.+?)(al|ance|ence|er|ic|able|ible|ant|ement|ment|ent|ou|ism|ate|iti|ous|ive|ize)$/;
+        re2 = /^(.+?)(s|t)(ion)$/;
+        if (re.test(w)) {
+            var fp = re.exec(w);
+            stem = fp[1];
+            re = new RegExp(mgr1);
+            if (re.test(stem))
+                w = stem;
+        } else if (re2.test(w)) {
+            var fp = re2.exec(w);
+            stem = fp[1] + fp[2];
+            re2 = new RegExp(mgr1);
+            if (re2.test(stem))
+                w = stem;
+        }
+
+        // Step 5
+        re = /^(.+?)e$/;
+        if (re.test(w)) {
+            var fp = re.exec(w);
+            stem = fp[1];
+            re = new RegExp(mgr1);
+            re2 = new RegExp(meq1);
+            re3 = new RegExp("^" + C + v + "[^aeiouwxy]$");
+            if (re.test(stem) || (re2.test(stem) && !(re3.test(stem))))
+                w = stem;
+        }
+        re = /ll$/;
+        re2 = new RegExp(mgr1);
+        if (re.test(w) && re2.test(w)) {
+            re = /.$/;
+            w = w.replace(re, "");
+        }
+
+        // and turn initial Y back to y
+        if (firstch == "y")
+            w = firstch.toLowerCase() + w.substr(1);
+        return w;
+    }
 }
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/pygments.css` & `mzdata2mat-0.2.0/docs/build/html/_static/pygments.css`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-pre { line-height: 125%; }
-td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
-span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
-td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
-span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
-.highlight .hll { background-color: #ffffcc }
-.highlight { background: #f8f8f8; }
-.highlight .c { color: #3D7B7B; font-style: italic } /* Comment */
-.highlight .err { border: 1px solid #FF0000 } /* Error */
-.highlight .k { color: #008000; font-weight: bold } /* Keyword */
-.highlight .o { color: #666666 } /* Operator */
-.highlight .ch { color: #3D7B7B; font-style: italic } /* Comment.Hashbang */
-.highlight .cm { color: #3D7B7B; font-style: italic } /* Comment.Multiline */
-.highlight .cp { color: #9C6500 } /* Comment.Preproc */
-.highlight .cpf { color: #3D7B7B; font-style: italic } /* Comment.PreprocFile */
-.highlight .c1 { color: #3D7B7B; font-style: italic } /* Comment.Single */
-.highlight .cs { color: #3D7B7B; font-style: italic } /* Comment.Special */
-.highlight .gd { color: #A00000 } /* Generic.Deleted */
-.highlight .ge { font-style: italic } /* Generic.Emph */
-.highlight .ges { font-weight: bold; font-style: italic } /* Generic.EmphStrong */
-.highlight .gr { color: #E40000 } /* Generic.Error */
-.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
-.highlight .gi { color: #008400 } /* Generic.Inserted */
-.highlight .go { color: #717171 } /* Generic.Output */
-.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
-.highlight .gs { font-weight: bold } /* Generic.Strong */
-.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
-.highlight .gt { color: #0044DD } /* Generic.Traceback */
-.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
-.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
-.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
-.highlight .kp { color: #008000 } /* Keyword.Pseudo */
-.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
-.highlight .kt { color: #B00040 } /* Keyword.Type */
-.highlight .m { color: #666666 } /* Literal.Number */
-.highlight .s { color: #BA2121 } /* Literal.String */
-.highlight .na { color: #687822 } /* Name.Attribute */
-.highlight .nb { color: #008000 } /* Name.Builtin */
-.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
-.highlight .no { color: #880000 } /* Name.Constant */
-.highlight .nd { color: #AA22FF } /* Name.Decorator */
-.highlight .ni { color: #717171; font-weight: bold } /* Name.Entity */
-.highlight .ne { color: #CB3F38; font-weight: bold } /* Name.Exception */
-.highlight .nf { color: #0000FF } /* Name.Function */
-.highlight .nl { color: #767600 } /* Name.Label */
-.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
-.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
-.highlight .nv { color: #19177C } /* Name.Variable */
-.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
-.highlight .w { color: #bbbbbb } /* Text.Whitespace */
-.highlight .mb { color: #666666 } /* Literal.Number.Bin */
-.highlight .mf { color: #666666 } /* Literal.Number.Float */
-.highlight .mh { color: #666666 } /* Literal.Number.Hex */
-.highlight .mi { color: #666666 } /* Literal.Number.Integer */
-.highlight .mo { color: #666666 } /* Literal.Number.Oct */
-.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
-.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
-.highlight .sc { color: #BA2121 } /* Literal.String.Char */
-.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
-.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
-.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
-.highlight .se { color: #AA5D1F; font-weight: bold } /* Literal.String.Escape */
-.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
-.highlight .si { color: #A45A77; font-weight: bold } /* Literal.String.Interpol */
-.highlight .sx { color: #008000 } /* Literal.String.Other */
-.highlight .sr { color: #A45A77 } /* Literal.String.Regex */
-.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
-.highlight .ss { color: #19177C } /* Literal.String.Symbol */
-.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
-.highlight .fm { color: #0000FF } /* Name.Function.Magic */
-.highlight .vc { color: #19177C } /* Name.Variable.Class */
-.highlight .vg { color: #19177C } /* Name.Variable.Global */
-.highlight .vi { color: #19177C } /* Name.Variable.Instance */
-.highlight .vm { color: #19177C } /* Name.Variable.Magic */
+pre { line-height: 125%; }
+td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
+span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
+td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
+span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
+.highlight .hll { background-color: #ffffcc }
+.highlight { background: #f8f8f8; }
+.highlight .c { color: #3D7B7B; font-style: italic } /* Comment */
+.highlight .err { border: 1px solid #FF0000 } /* Error */
+.highlight .k { color: #008000; font-weight: bold } /* Keyword */
+.highlight .o { color: #666666 } /* Operator */
+.highlight .ch { color: #3D7B7B; font-style: italic } /* Comment.Hashbang */
+.highlight .cm { color: #3D7B7B; font-style: italic } /* Comment.Multiline */
+.highlight .cp { color: #9C6500 } /* Comment.Preproc */
+.highlight .cpf { color: #3D7B7B; font-style: italic } /* Comment.PreprocFile */
+.highlight .c1 { color: #3D7B7B; font-style: italic } /* Comment.Single */
+.highlight .cs { color: #3D7B7B; font-style: italic } /* Comment.Special */
+.highlight .gd { color: #A00000 } /* Generic.Deleted */
+.highlight .ge { font-style: italic } /* Generic.Emph */
+.highlight .ges { font-weight: bold; font-style: italic } /* Generic.EmphStrong */
+.highlight .gr { color: #E40000 } /* Generic.Error */
+.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
+.highlight .gi { color: #008400 } /* Generic.Inserted */
+.highlight .go { color: #717171 } /* Generic.Output */
+.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
+.highlight .gs { font-weight: bold } /* Generic.Strong */
+.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
+.highlight .gt { color: #0044DD } /* Generic.Traceback */
+.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
+.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
+.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
+.highlight .kp { color: #008000 } /* Keyword.Pseudo */
+.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
+.highlight .kt { color: #B00040 } /* Keyword.Type */
+.highlight .m { color: #666666 } /* Literal.Number */
+.highlight .s { color: #BA2121 } /* Literal.String */
+.highlight .na { color: #687822 } /* Name.Attribute */
+.highlight .nb { color: #008000 } /* Name.Builtin */
+.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
+.highlight .no { color: #880000 } /* Name.Constant */
+.highlight .nd { color: #AA22FF } /* Name.Decorator */
+.highlight .ni { color: #717171; font-weight: bold } /* Name.Entity */
+.highlight .ne { color: #CB3F38; font-weight: bold } /* Name.Exception */
+.highlight .nf { color: #0000FF } /* Name.Function */
+.highlight .nl { color: #767600 } /* Name.Label */
+.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
+.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
+.highlight .nv { color: #19177C } /* Name.Variable */
+.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
+.highlight .w { color: #bbbbbb } /* Text.Whitespace */
+.highlight .mb { color: #666666 } /* Literal.Number.Bin */
+.highlight .mf { color: #666666 } /* Literal.Number.Float */
+.highlight .mh { color: #666666 } /* Literal.Number.Hex */
+.highlight .mi { color: #666666 } /* Literal.Number.Integer */
+.highlight .mo { color: #666666 } /* Literal.Number.Oct */
+.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
+.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
+.highlight .sc { color: #BA2121 } /* Literal.String.Char */
+.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
+.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
+.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
+.highlight .se { color: #AA5D1F; font-weight: bold } /* Literal.String.Escape */
+.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
+.highlight .si { color: #A45A77; font-weight: bold } /* Literal.String.Interpol */
+.highlight .sx { color: #008000 } /* Literal.String.Other */
+.highlight .sr { color: #A45A77 } /* Literal.String.Regex */
+.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
+.highlight .ss { color: #19177C } /* Literal.String.Symbol */
+.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
+.highlight .fm { color: #0000FF } /* Name.Function.Magic */
+.highlight .vc { color: #19177C } /* Name.Variable.Class */
+.highlight .vg { color: #19177C } /* Name.Variable.Global */
+.highlight .vi { color: #19177C } /* Name.Variable.Instance */
+.highlight .vm { color: #19177C } /* Name.Variable.Magic */
 .highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/searchtools.js` & `mzdata2mat-0.2.0/docs/build/html/_static/searchtools.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 /**
  * Simple result scoring code.
@@ -94,15 +94,15 @@
             highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
     } else if (showSearchSummary)
         fetch(requestUrl)
         .then((responseData) => responseData.text())
         .then((data) => {
             if (data)
                 listItem.appendChild(
-                    Search.makeSearchSummary(data, searchTerms)
+                    Search.makeSearchSummary(data, searchTerms, anchor)
                 );
             // highlight search terms in the summary
             if (SPHINX_HIGHLIGHT_ENABLED) // set in sphinx_highlight.js
                 highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
         });
     Search.output.appendChild(listItem);
 };
@@ -111,16 +111,16 @@
     Search.title.innerText = _("Search Results");
     if (!resultCount)
         Search.status.innerText = Documentation.gettext(
             "Your search did not match any documents. Please make sure that all words are spelled correctly and that you've selected enough categories."
         );
     else
         Search.status.innerText = _(
-            `Search finished, found ${resultCount} page(s) matching the search query.`
-        );
+            "Search finished, found ${resultCount} page(s) matching the search query."
+        ).replace('${resultCount}', resultCount);
 };
 const _displayNextItem = (
     results,
     resultCount,
     searchTerms,
     highlightTerms,
 ) => {
@@ -132,14 +132,30 @@
             () => _displayNextItem(results, resultCount, searchTerms, highlightTerms),
             5
         );
     }
     // search finished, update title and status message
     else _finishSearch(resultCount);
 };
+// Helper function used by query() to order search results.
+// Each input is an array of [docname, title, anchor, descr, score, filename].
+// Order the results by score (in opposite order of appearance, since the
+// `_displayNextItem` function uses pop() to retrieve items) and then alphabetically.
+const _orderResultsByScoreThenName = (a, b) => {
+    const leftScore = a[4];
+    const rightScore = b[4];
+    if (leftScore === rightScore) {
+        // same score: sort alphabetically
+        const leftTitle = a[1].toLowerCase();
+        const rightTitle = b[1].toLowerCase();
+        if (leftTitle === rightTitle) return 0;
+        return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
+    }
+    return leftScore > rightScore ? 1 : -1;
+};
 
 /**
  * Default splitQuery function. Can be overridden in ``sphinx.search`` with a
  * custom function per language.
  *
  * The regular expression works by splitting the string on consecutive characters
  * that are not Unicode letters, numbers, underscores, or emoji characters.
@@ -155,23 +171,36 @@
  * Search Module
  */
 const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
-    htmlToText: (htmlString) => {
+    htmlToText: (htmlString, anchor) => {
         const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
-        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
-            el.remove()
-        });
+        for (const removalQuery of [".headerlinks", "script", "style"]) {
+            htmlElement.querySelectorAll(removalQuery).forEach((el) => {
+                el.remove()
+            });
+        }
+        if (anchor) {
+            const anchorContent = htmlElement.querySelector(`[role="main"] ${anchor}`);
+            if (anchorContent) return anchorContent.textContent;
+
+            console.warn(
+                `Anchored content block not found. Sphinx search tries to obtain it via DOM query '[role=main] ${anchor}'. Check your theme or template.`
+            );
+        }
+
+        // if anchor not specified or not found, fall back to main content
         const docContent = htmlElement.querySelector('[role="main"]');
-        if (docContent !== undefined) return docContent.textContent;
+        if (docContent) return docContent.textContent;
+
         console.warn(
-            "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
+            "Content block not found. Sphinx search tries to obtain it via DOM query '[role=main]'. Check your theme or template."
         );
         return "";
     },
 
     init: () => {
         const query = new URLSearchParams(window.location.search).get("q");
         document
@@ -236,24 +265,15 @@
         Search.startPulse();
 
         // index already loaded, the browser was quick!
         if (Search.hasIndex()) Search.query(query);
         else Search.deferQuery(query);
     },
 
-    /**
-     * execute search (requires search index to be loaded)
-     */
-    query: (query) => {
-        const filenames = Search._index.filenames;
-        const docNames = Search._index.docnames;
-        const titles = Search._index.titles;
-        const allTitles = Search._index.alltitles;
-        const indexEntries = Search._index.indexentries;
-
+    _parseQuery: (query) => {
         // stem the search terms and add them to the correct list
         const stemmer = new Stemmer();
         const searchTerms = new Set();
         const excludedTerms = new Set();
         const highlightTerms = new Set();
         const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
         splitQuery(query.trim()).forEach((queryTerm) => {
@@ -281,92 +301,114 @@
             localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
         }
 
         // console.debug("SEARCH: searching for:");
         // console.info("required: ", [...searchTerms]);
         // console.info("excluded: ", [...excludedTerms]);
 
-        // array of [docname, title, anchor, descr, score, filename]
-        let results = [];
+        return [query, searchTerms, excludedTerms, highlightTerms, objectTerms];
+    },
+
+    /**
+     * execute search (requires search index to be loaded)
+     */
+    _performSearch: (query, searchTerms, excludedTerms, highlightTerms, objectTerms) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
+        // Collect multiple result groups to be sorted separately and then ordered.
+        // Each is an array of [docname, title, anchor, descr, score, filename].
+        const normalResults = [];
+        const nonMainIndexResults = [];
+
         _removeChildren(document.getElementById("search-progress"));
 
-        const queryLower = query.toLowerCase();
+        const queryLower = query.toLowerCase().trim();
         for (const [title, foundTitles] of Object.entries(allTitles)) {
-            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+            if (title.toLowerCase().trim().includes(queryLower) && (queryLower.length >= title.length / 2)) {
                 for (const [file, id] of foundTitles) {
                     let score = Math.round(100 * queryLower.length / title.length)
-                    results.push([
+                    normalResults.push([
                         docNames[file],
                         titles[file] !== title ? `${titles[file]} > ${title}` : title,
                         id !== null ? "#" + id : "",
                         null,
                         score,
                         filenames[file],
                     ]);
                 }
             }
         }
 
         // search for explicit entries in index directives
         for (const [entry, foundEntries] of Object.entries(indexEntries)) {
             if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
-                for (const [file, id] of foundEntries) {
-                    let score = Math.round(100 * queryLower.length / entry.length)
-                    results.push([
+                for (const [file, id, isMain] of foundEntries) {
+                    const score = Math.round(100 * queryLower.length / entry.length);
+                    const result = [
                         docNames[file],
                         titles[file],
                         id ? "#" + id : "",
                         null,
                         score,
                         filenames[file],
-                    ]);
+                    ];
+                    if (isMain) {
+                        normalResults.push(result);
+                    } else {
+                        nonMainIndexResults.push(result);
+                    }
                 }
             }
         }
 
         // lookup as object
         objectTerms.forEach((term) =>
-            results.push(...Search.performObjectSearch(term, objectTerms))
+            normalResults.push(...Search.performObjectSearch(term, objectTerms))
         );
 
         // lookup as search terms in fulltext
-        results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
+        normalResults.push(...Search.performTermsSearch(searchTerms, excludedTerms));
 
         // let the scorer override scores with a custom scoring function
-        if (Scorer.score) results.forEach((item) => (item[4] = Scorer.score(item)));
+        if (Scorer.score) {
+            normalResults.forEach((item) => (item[4] = Scorer.score(item)));
+            nonMainIndexResults.forEach((item) => (item[4] = Scorer.score(item)));
+        }
 
-        // now sort the results by score (in opposite order of appearance, since the
-        // display function below uses pop() to retrieve items) and then
-        // alphabetically
-        results.sort((a, b) => {
-            const leftScore = a[4];
-            const rightScore = b[4];
-            if (leftScore === rightScore) {
-                // same score: sort alphabetically
-                const leftTitle = a[1].toLowerCase();
-                const rightTitle = b[1].toLowerCase();
-                if (leftTitle === rightTitle) return 0;
-                return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
-            }
-            return leftScore > rightScore ? 1 : -1;
-        });
+        // Sort each group of results by score and then alphabetically by name.
+        normalResults.sort(_orderResultsByScoreThenName);
+        nonMainIndexResults.sort(_orderResultsByScoreThenName);
+
+        // Combine the result groups in (reverse) order.
+        // Non-main index entries are typically arbitrary cross-references,
+        // so display them after other results.
+        let results = [...nonMainIndexResults, ...normalResults];
 
         // remove duplicate search results
         // note the reversing of results, so that in the case of duplicates, the highest-scoring entry is kept
         let seen = new Set();
         results = results.reverse().reduce((acc, result) => {
             let resultStr = result.slice(0, 4).concat([result[5]]).map(v => String(v)).join(',');
             if (!seen.has(resultStr)) {
                 acc.push(result);
                 seen.add(resultStr);
             }
             return acc;
         }, []);
 
-        results = results.reverse();
+        return results.reverse();
+    },
+
+    query: (query) => {
+        const [searchQuery, searchTerms, excludedTerms, highlightTerms, objectTerms] = Search._parseQuery(query);
+        const results = Search._performSearch(searchQuery, searchTerms, excludedTerms, highlightTerms, objectTerms);
 
         // for debugging
         //Search.lastresults = results.slice();  // a copy
         // console.info("search results:", Search.lastresults);
 
         // print the results
         _displayNextItem(results, results.length, searchTerms, highlightTerms);
@@ -466,28 +508,32 @@
             }, {
                 files: titleTerms[word],
                 score: Scorer.title
             }, ];
             // add support for partial matches
             if (word.length > 2) {
                 const escapedWord = _escapeRegExp(word);
-                Object.keys(terms).forEach((term) => {
-                    if (term.match(escapedWord) && !terms[word])
-                        arr.push({
-                            files: terms[term],
-                            score: Scorer.partialTerm
-                        });
-                });
-                Object.keys(titleTerms).forEach((term) => {
-                    if (term.match(escapedWord) && !titleTerms[word])
-                        arr.push({
-                            files: titleTerms[word],
-                            score: Scorer.partialTitle
-                        });
-                });
+                if (!terms.hasOwnProperty(word)) {
+                    Object.keys(terms).forEach((term) => {
+                        if (term.match(escapedWord))
+                            arr.push({
+                                files: terms[term],
+                                score: Scorer.partialTerm
+                            });
+                    });
+                }
+                if (!titleTerms.hasOwnProperty(word)) {
+                    Object.keys(titleTerms).forEach((term) => {
+                        if (term.match(escapedWord))
+                            arr.push({
+                                files: titleTerms[term],
+                                score: Scorer.partialTitle
+                            });
+                    });
+                }
             }
 
             // no match but word was a required one
             if (arr.every((record) => record.files === undefined)) return;
 
             // found search word in contents
             arr.forEach((record) => {
@@ -502,17 +548,16 @@
                     if (!scoreMap.has(file)) scoreMap.set(file, {});
                     scoreMap.get(file)[word] = record.score;
                 });
             });
 
             // create the mapping
             files.forEach((file) => {
-                if (fileMap.has(file) && fileMap.get(file).indexOf(word) === -1)
-                    fileMap.get(file).push(word);
-                else fileMap.set(file, [word]);
+                if (!fileMap.has(file)) fileMap.set(file, [word]);
+                else if (fileMap.get(file).indexOf(word) === -1) fileMap.get(file).push(word);
             });
         });
 
         // now check if the files don't contain excluded terms
         const results = [];
         for (const [file, wordList] of fileMap) {
             // check if all requirements are matched
@@ -555,16 +600,16 @@
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
      * of stemmed words.
      */
-    makeSearchSummary: (htmlText, keywords) => {
-        const text = Search.htmlToText(htmlText);
+    makeSearchSummary: (htmlText, keywords, anchor) => {
+        const text = Search.htmlToText(htmlText, anchor);
         if (text === "") return null;
 
         const textLower = text.toLowerCase();
         const actualStartPosition = [...keywords]
             .map((k) => textLower.indexOf(k.toLowerCase()))
             .filter((i) => i > -1)
             .slice(-1)[0];
```

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/sphinx_highlight.js` & `mzdata2mat-0.2.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/badge_only.css` & `mzdata2mat-0.2.0/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/theme.css` & `mzdata2mat-0.2.0/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-bold.woff` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-bold.woff2` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-normal.woff` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/css/fonts/lato-normal.woff2` & `mzdata2mat-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/js/badge_only.js` & `mzdata2mat-0.2.0/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `mzdata2mat-0.2.0/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/js/html5shiv.min.js` & `mzdata2mat-0.2.0/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/build/html/_static/js/theme.js` & `mzdata2mat-0.2.0/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/source/code-example.md` & `mzdata2mat-0.2.0/docs/source/code-example.md`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/source/conf.py` & `mzdata2mat-0.2.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'mzdata2mat'
 copyright = '2024, CORDELLA Maxime'
 author = 'CORDELLA Maxime'
-release = '0.1.0'
+release = '0.2.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['myst_parser']
 
 templates_path = ['_templates']
```

### Comparing `mzdata2mat-0.1.1/docs/source/installation.md` & `mzdata2mat-0.2.0/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/source/mzDataManager.md` & `mzdata2mat-0.2.0/docs/source/mzDataManager.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 - Otherwise :
     - `fileName` : Full path to the `mzData.xml` file to read
     - `customDirectory` : Does nothing
 
 <u>Outputs</u>
 - Outputs a `mzData` class containing the content of the file parsed.
 
+(savematfile)=
 ### saveMatfile
 #### Presentation
 Saves a `mzData` class into a `.mat` file with all metadata included.
 
 #### Definition
 ```python
 def saveMatfile(self@mzDataManager, mzData : mzData, remove : bool = False, dir2Save : str = None, force : bool = False)
@@ -74,15 +75,15 @@
 # Considering also the variable content which is the result of the function mzDataXMLread presented above
 
 manager.saveMatFile(
     mzData=content
 )
 ```
 <u>Parameters</u>
-- `mzData` : The `mzData` structure to save as a `.mat` file. (See [here](matStructure.md) for the `.mat` file structure)
+- `mzData` : The `mzData` structure to save as a `.mat` file. (See [here](matStruct.md) for the `.mat` file structure)
 - `remove` : Should the original file (so the original `.mzData.xml` file) be removed when save is complete ?
 - `force` : If a `.mat` file already exists with the same name in the export folder, should it be replaced ? If this parameter is set to `False`, save will be aborted if a file is found.
 - If directories were not provided during init process:
     - `dir2save` : Full directory specifying where to save the converted file. If this parameter is set while a directory was specified in the init process, this value is prioritized.
 
 <u>Outputs</u><br>
 If function ran correctly, no output, otherwise raises the error.
```

### Comparing `mzdata2mat-0.1.1/docs/source/mzDataXMLStruct.md` & `mzdata2mat-0.2.0/docs/source/mzDataXMLStruct.md`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/docs/source/mzdata2mat-verify.md` & `mzdata2mat-0.2.0/docs/source/mzdata2mat-verify.md`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/src/mzdata2mat/mzdata2mat.py` & `mzdata2mat-0.2.0/src/mzdata2mat/mzdata2mat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,49 @@
 from pydantic import BaseModel
-from mat4py import savemat
+from mat4py import savemat, loadmat
+from mat4py.loadmat import ParseError
 from javascript import require
 from javascript.errors import JavaScriptError
 from .errors import mzDataError
 import os
 import shutil
-from typing import Any
-
-class mzDataXMLStruct(BaseModel):
-    metadata : dict
-    times : list[float]
-    series : Any
-
-class mzData(BaseModel):
-    fileName : str = ""
-    filePath : str = ""
-    metadata : dict = {}
-    mz : list[list[float]] = [[]]
-    intensities : list[list[float]] = [[]]
-    time : list[float] = []
-
-    def __init__(self):
-        super().__init__()
-
-    def toDict(self):
-        copyright : dict = {
-        'Author' : '(c)LARTIC_2024_Maxime_CORDELLA',
-        'URL' : 'https://lartic.fsaa.ulaval.ca/chimiometrie/routines-de-conversion'
-        }
-        tempDict = self.model_dump()
-        tempDict['copyright'] = copyright
-        tempDict['documentation'] = "https://mzdata2mat.readthedocs.io/"
-        return {self.fileName.lower().split(".mzdata")[0] : tempDict}
+from .classes import matStruct, mzData, mzDataXMLStruct
+from colorama import Fore
 
 class mzDataManager(BaseModel):
+    """Main class for converting .mzData.xml files into .mat files for realeases of Matlab r2019b and newer.
+        -> `useDirectory` : Set this parameter to `False` to not use directories and specify them when using the functions.
+        -> `mzDataPath` : Path to the folder containing the .mzdata.xml files \n
+        -> `exportPath` : Path to save the converted .mat files \n
+    """
     mzDataPath : str = None
     exportPath : str = None
-    mzDataPackage : str = None
+    __mzDataPackage__ : str = None
+    matStructure : matStruct = matStruct()
 
-    def __init__(self, useDirectory : bool = True, mzDataPath : str = None, exportPath : str = None):
+    def __init__(self, useDirectory : bool = True, mzDataPath : str = None, exportPath : str = None, matStructure : matStruct = None):
         """Main class for converting .mzData.xml files into .mat files for realeases of Matlab r2019b and newer.
-        -> `mzDataPath` : Path to the folder containing the .mzdata.xml files \n
-        -> `exportPath` : Path to save the converted .mat files \n
-        -> `useDirectory` : Set this parameter to `False` to not use directories and specify them when using the functions.
-        
+            -> `useDirectory` : Set this parameter to `False` to not use directories and specify them when using the functions.
+            -> `mzDataPath` : Path to the folder containing the .mzdata.xml files \n
+            -> `exportPath` : Path to save the converted .mat files \n
         """
+        super().__init__()
         if useDirectory:
             if os.path.isdir(mzDataPath) and os.path.exists(mzDataPath):
                 self.mzDataPath = mzDataPath
             else:
                 raise mzDataError("The directory entered for .mzdata.xml files is not valid", 3)
             if os.path.isdir(exportPath) and os.path.exists(exportPath):
                 self.exportPath = exportPath
             else:
-                raise mzDataError("The directory entered for converted .mat files is not valid")
-        super().__init__()
+                raise mzDataError("The directory entered for converted .mat files is not valid", 3)
+        if matStructure != None:
+            self.matStructure = matStructure
         try:
-            self.mzDataPackage = require('mzdata')
+            self.__mzDataPackage__ = require('mzdata')
         except Exception as e:
             # This error will often be related with node.js not being installed on the target machine.
             raise e
 
     def mzDataXMLread(self, fileName : str, customDirectory : bool = False):
         """
         Reads mzML files and returns the given object.\n
@@ -68,20 +51,20 @@
             -> Should be the full path to the file and it's extension (.mzdata.xml) to convert if no value was given to `mzDataPath` when initializing the class.\n
             -> Otherwise, the file's relative path with it's extension (.mzdata.xml)\n
         -> `customDirectory` : Set this parameter to `True` if the `fileName` is in a different path than the one given in configuration.
         """
         try:
             if self.mzDataPath == None or customDirectory:
                     if os.path.exists(fileName):
-                        result = self.mzDataPackage.parseMZ(open(fileName).read())
+                        result = self.__mzDataPackage__.parseMZ(open(fileName).read())
                     else:
                         raise mzDataError("The path given for the mzData file is not valid.", 10)
             else:
                 if os.path.exists(os.path.join(self.mzDataPath, fileName)):
-                    result = self.mzDataPackage.parseMZ(open(os.path.join(self.mzDataPath, fileName)).read())
+                    result = self.__mzDataPackage__.parseMZ(open(os.path.join(self.mzDataPath, fileName)).read())
                 else:
                     raise mzDataError("The path given for the mzData file is not valid.", 10)
         except JavaScriptError as e:
             raise e
         metadata = {
             'software' : str(result.metadata["software"]),
             'analyser' : str(result.metadata["analyser"]),
@@ -100,49 +83,52 @@
                 intensityDataSet.append(i[1][str(z)])
             totalMasseDataSet.append(massesDataSet)
             totalIntensityDataSet.append(intensityDataSet)
         returnStruct.mz = totalMasseDataSet
         returnStruct.intensities = totalIntensityDataSet
         returnStruct.time = dataStruct.times
         if customDirectory or self.mzDataPath == None:
-            file = fileName
+            file = fileName.rsplit("/", 1)[0]
         else:
             file = self.mzDataPath
         returnStruct.filePath = file
         try:
-            returnStruct.fileName = file.rsplit("/", 1)[1]
+            returnStruct.fileName = fileName.rsplit("/", 1)[1]
         except IndexError:
-            returnStruct.fileName = file.rsplit("\\", 1)[1]
+            if fileName.find("\\") != -1:
+                returnStruct.fileName = fileName.rsplit("\\", 1)[1]
+            else:
+                returnStruct.fileName = fileName
         returnStruct.metadata = dataStruct.metadata
         return returnStruct
     
-    def saveMatfile(self, mzData : mzData, remove : bool = False, dir2Save : str = None, force : bool = False):
+    def saveMatfile(self, mzData : mzData, remove : bool = False, dir2Save : str = None, force : bool = False, fileName : str = None, partialSave : bool = False):
         """
         Saves a `mzData` structure to a .mat file.\n
         -> `mzData`     : The structure got from `mzMLread` function.\n
         -> `remove`     : Should the original file be removed when it is saved as .mat file ?\n
         -> `dir2Save`   : Save directory to save the .mat file. If path was given in configuration, it is not needed. This parameter will be prioritised over the path given in configuration (if any).\n
         -> `force`      : If a file has the same name in the converted folder, should it be replaced ? (File will not be saved if sibling found in convert folder and this parameter set to `False`.)
         """
         if self.exportPath == None or dir2Save != None:
             if os.path.exists(dir2Save):
-                saveDir = os.path.join(dir2Save, f"{mzData.fileName.lower().split('.mzdata')[0]}.mat")
+                saveDir = os.path.join(dir2Save, f"{mzData.fileName.lower().split('.mzdata')[0] if fileName == None else fileName.split('.mat')[0]}.mat")
             else:
                 raise mzDataError("No save directory specified", 4)
         else:
-            saveDir = os.path.join(self.exportPath, f"{mzData.fileName.split('.mzdata')[0]}.mat")
+            saveDir = os.path.join(self.exportPath, f"{mzData.fileName.lower().split('.mzdata')[0] if fileName == None else fileName.split('.mat')[0]}.mat")
         
         if os.path.exists(saveDir):
             if force:
                 os.remove(saveDir)
-                savemat(saveDir, mzData.toDict())
+                savemat(saveDir, mzData.toDict(self.matStructure, partialSave=partialSave))
             else:
-                print(f"File {mzData.fileName} skipped because same file exists in export folder and parameter `force` is not set to `True`")
+                print(Fore.BLUE+ f"Info : File {mzData.fileName} skipped because same file exists in export folder and parameter `force` is not set to `True`" + Fore.RESET)
         else:
-            savemat(saveDir, mzData.toDict())
+            savemat(saveDir, mzData.toDict(self.matStructure, partialSave=partialSave))
         if remove:
             os.remove(os.path.join(mzData.filePath, mzData.fileName))
         return
     
     def convertFile(self, fileName : str, customDirectory : bool = False, dir2Save : str = None, force : bool = False, remove : bool = False):
         """
         Reads mzData.xml file and saves it directly into the folder specified.\n
@@ -154,24 +140,67 @@
         -> `force`      : If a file has the same name in the converted folder, should it be replaced ? (File will not be saved if sibling found in convert folder and this parameter set to `False`.)
         -> `remove`     : Should the original file be removed when it is saved as .mat file ?\n
 
         """
         fileContent = self.mzDataXMLread(fileName=fileName, customDirectory=customDirectory)
         self.saveMatfile(mzData=fileContent, remove=remove, dir2Save=dir2Save, force=force)
         return
+    
+    def loadMatfile(self, fileName : str, fromOneStruct : bool = True) -> mzData:
+        """
+        Creates a `mzData` structure from a matlab file.\n
+        -> `fileName` : Full path of the matlab file to load the data from.
+        -> `fromOneStruct` : Is the data contained in one variable ? Set this paramteter to `True` if that's the case.
+        """
+        PATH = ""
+        if os.path.isfile(fileName):
+            PATH = fileName
+        
+        elif self.mzDataPath != None:
+            PATH = os.path.join(self.mzDataPath, fileName)
+        
+        else:
+            raise mzDataError("No such file or directory.", 3)
+
+        try:
+            tempClass = mzData()
+            data = loadmat(PATH)
+            dump = self.matStructure.model_dump()
+            if fromOneStruct:
+                name : str = list(data.keys())[0]
+                content = data[name]
+            else:
+                content = data
+            for key in list(dump.keys()):
+                try:
+                    tempClass.__setattr__(key, content[dump[key]])
+                except KeyError:
+                    if key != "oneStruct":
+                        print(Fore.YELLOW + f"Warning : {Fore.BLUE} {dump[key]} {Fore.YELLOW} corresponding to {Fore.BLUE + key} {Fore.YELLOW} field has not been found in mat file : Using default value in created structure."+Fore.RESET)
+            try:
+                list(content.keys()).index('extra')
+                if content['extra'] == '':
+                    tempClass.__extra__ = {}
+                else:
+                    tempClass.__extra__ = content['extra']
+            except ValueError:
+                tempClass.__extra__ = {}
+            return tempClass
+        except ParseError:
+            raise mzDataError("Error while reading, some data have incompatible type.", 11)
 
 def verify():
-    print("Starting verifying process...")
+    print(Fore.BLUE + "Starting verifying process..." + Fore.RESET)
     try:
         path = os.getcwd()
         testFile = os.path.join(__file__.lower().rsplit("mzdata", 1)[0], "tiny1.mzData.xml")
-        print("Creating class... ")
+        print(Fore.BLUE + "Creating class... " + Fore.RESET)
         testClass = mzDataManager(useDirectory=False)
-        print("Copying file in current directory...")
+        print(Fore.BLUE + "Copying file in current directory..." + Fore.RESET)
         shutil.copyfile(testFile, os.path.join(path, "tiny1.mzData.xml"))
-        print("Reading file...")
+        print(Fore.BLUE + "Reading file..." + Fore.RESET)
         value = testClass.mzDataXMLread(os.path.join(path, "tiny1.mzData.xml"))
-        print("Saving file...")
-        testClass.saveMatfile(value, dir2Save=path)
-        print("mzdata2mat - Ready to use !")
+        print(Fore.BLUE + "Saving file..." + Fore.RESET)
+        testClass.saveMatfile(value, dir2Save=path, force=True)
+        print(Fore.BLUE + "mzdata2mat - Ready to use !" + Fore.RESET)
     except Exception as e:
         raise e
```

### Comparing `mzdata2mat-0.1.1/src/mzdata2mat/tiny1.mzData.xml` & `mzdata2mat-0.2.0/src/mzdata2mat/tiny1.mzData.xml`

 * *Files identical despite different names*

### Comparing `mzdata2mat-0.1.1/LICENSE.txt` & `mzdata2mat-0.2.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2024 Maxime CORDELLA - LARTIC
+Copyright (c) 2024 Maxime CORDELLA - LARTIC - Université Laval, Québec
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mzdata2mat-0.1.1/README.md` & `mzdata2mat-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 Copyright(c)2024_LARTIC
 
 [![Documentation Status](https://readthedocs.org/projects/mzdata2mat/badge/?version=latest)](https://mzdata2mat.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/mzdata2mat)](https://pypi.org/project/mzdata2mat/)
 [![downloads](https://static.pepy.tech/badge/mzdata2mat/month)](https://pepy.tech/project/mzdata2mat)
 
 ## Documentation
-The complete documentation is available [here](https://mzdata2mat.readthedocs.io/). All classes are explained and methods.
+The complete documentation is available [here](https://mzdata2mat.readthedocs.io/). All classes and methods are explained.
 
 ## Changelog
-The current version of mzdata2mat is the following : `0.1.0`
+The current version of mzdata2mat is the following : `0.2.0`
 
-You can see the complete changelog [here](Changelog.md)
+You can see the complete changelog [here](https://github.com/MaximeLeMagicien/mzdata2mat/blob/main/Changelog.md)
 
 ## Compatible hardware
 At this time, the following OSes have been tested :
 
 ### macOS
 At this time, `macOS Sonoma 14.0` is officially supported, other macOS versions could be supported as long as they follow the requirements listed below.
 
@@ -26,22 +26,23 @@
 At this time, `mzdata2mat` have been tested and is supported on `Windows 11`, no testing has been done on Windows 10 or 7 but if you want to extend the compatibility, we are open to tester's feedback on thoses machines.
 
 ## Requirements
 ### Other than Python
 This package __requires node.js installed__. you can download and install it at [nodejs.org](https://nodejs.org/en). It is available for both macOS and Windows for free.
 
 ### Python version
-This package has been developped with Python `3.12.1` however, other python versions are actively being tested to add other versions as soon as possible.
+This package is compatible to any python version equal or newer than `3.9`.
 
 ### Python packages
 When mzdata2mat will be installed on your system, the following packages will also be installed (if they are not) into your Python enviuronment : 
 ```
     pydantic>=2.6.4
     mat4py>=0.6.0
     javascript>=1!1.1.3
+    colorama>=0.4.6
 ```
 # Installation
 From your terminal run the following command to install mzdata2mat into your environment :
 ```shell
 $ pip install mzdata2mat
 ```
 If you have multiple instances of Python installed, run this command with the chosen Python interpreter to install mzdata2mat in the corresponding Python installation :
```

### Comparing `mzdata2mat-0.1.1/PKG-INFO` & `mzdata2mat-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.3
 Name: mzdata2mat
-Version: 0.1.1
-Summary: Package used to convert mzData.xml files into matlab files.
+Version: 0.2.0
+Summary: Package used to convert mzData.xml files version 1.05 into matlab files.
 Project-URL: Documentation, https://mzdata2mat.readthedocs.io/
 Project-URL: Repository, https://github.com/MaximeLeMagicien/mzdata2mat.git
 Project-URL: Issues, https://github.com/MaximeLeMagicien/mzdata2mat/issues
-Project-URL: Changelog, https://github.com/MaximeLeMagicien/mzdata2mat/blob/main/Changelog.md
-Author-email: CORDELLA Maxime <maxime.cordella911@gmail.com>
+Project-URL: Changelog, https://github.com/MaximeLeMagicien/mzdata2mat/blob/main/docs/source/Changelog.md
+Author-email: LARTIC <christophe.cordella@fsaa.ulaval.ca>
+Maintainer-email: CORDELLA Maxime <maxime.cordella911@gmail.com>, CORDELLA Christophe <christophe.cordella@fsaa.ulaval.ca>
 License: MIT License
 License-File: LICENSE.txt
 Keywords: .mat,.mzData.xml,.xml,convert,matlab,mzData
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
+Requires-Dist: colorama>=0.4.6
 Requires-Dist: javascript>=1!1.1.3
 Requires-Dist: mat4py>=0.6.0
 Requires-Dist: pydantic>=2.6.4
 Description-Content-Type: text/markdown
 
 # mzdata2mat
 Welcome ! `mzdata2mat` is a Python package from [LARTIC research team](https://lartic.fsaa.ulaval.ca/), which converts mzData.xml files (version 1.05, Agilent Technologies) into mat files readable using matlab. <br><br>
@@ -29,20 +35,20 @@
 Copyright(c)2024_LARTIC
 
 [![Documentation Status](https://readthedocs.org/projects/mzdata2mat/badge/?version=latest)](https://mzdata2mat.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/mzdata2mat)](https://pypi.org/project/mzdata2mat/)
 [![downloads](https://static.pepy.tech/badge/mzdata2mat/month)](https://pepy.tech/project/mzdata2mat)
 
 ## Documentation
-The complete documentation is available [here](https://mzdata2mat.readthedocs.io/). All classes are explained and methods.
+The complete documentation is available [here](https://mzdata2mat.readthedocs.io/). All classes and methods are explained.
 
 ## Changelog
-The current version of mzdata2mat is the following : `0.1.0`
+The current version of mzdata2mat is the following : `0.2.0`
 
-You can see the complete changelog [here](Changelog.md)
+You can see the complete changelog [here](https://github.com/MaximeLeMagicien/mzdata2mat/blob/main/Changelog.md)
 
 ## Compatible hardware
 At this time, the following OSes have been tested :
 
 ### macOS
 At this time, `macOS Sonoma 14.0` is officially supported, other macOS versions could be supported as long as they follow the requirements listed below.
 
@@ -50,22 +56,23 @@
 At this time, `mzdata2mat` have been tested and is supported on `Windows 11`, no testing has been done on Windows 10 or 7 but if you want to extend the compatibility, we are open to tester's feedback on thoses machines.
 
 ## Requirements
 ### Other than Python
 This package __requires node.js installed__. you can download and install it at [nodejs.org](https://nodejs.org/en). It is available for both macOS and Windows for free.
 
 ### Python version
-This package has been developped with Python `3.12.1` however, other python versions are actively being tested to add other versions as soon as possible.
+This package is compatible to any python version equal or newer than `3.9`.
 
 ### Python packages
 When mzdata2mat will be installed on your system, the following packages will also be installed (if they are not) into your Python enviuronment : 
 ```
     pydantic>=2.6.4
     mat4py>=0.6.0
     javascript>=1!1.1.3
+    colorama>=0.4.6
 ```
 # Installation
 From your terminal run the following command to install mzdata2mat into your environment :
 ```shell
 $ pip install mzdata2mat
 ```
 If you have multiple instances of Python installed, run this command with the chosen Python interpreter to install mzdata2mat in the corresponding Python installation :
```

