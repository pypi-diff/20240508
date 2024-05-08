# Comparing `tmp/coldp-2024.0.2.tar.gz` & `tmp/coldp-2024.5.2.tar.gz`

## Comparing `coldp-2024.0.2.tar` & `coldp-2024.5.2.tar`

### file list

```diff
@@ -1,1909 +1,53 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 coldp-2024.0.2/.gitattributes
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 coldp-2024.0.2/src/coldp/__init__.py
--rw-r--r--   0        0        0    71863 2020-02-02 00:00:00.000000 coldp-2024.0.2/src/coldp/coldp.py
--rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 coldp-2024.0.2/src/coldp/coldp_distribution.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/Distribution.tsv
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/Media.tsv
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/NameRelation.tsv
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/NameUsage.tsv
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/Reference.tsv
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/SpeciesEstimate.tsv
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/SpeciesInteraction.tsv
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/TaxonConceptRelation.tsv
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/TypeMaterial.tsv
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/VernacularName.tsv
--rw-r--r--   0        0        0   697219 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/logo.png
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/metadata.yaml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.0.2/test/input/Tonzidae/reference.json
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/pyvenv.cfg
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports/__init__.py
--rw-r--r--   0        0        0   106960 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports/tarfile/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports/tarfile/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports/tarfile/compat/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports/tarfile/compat/py38.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports.tarfile-1.1.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports.tarfile-1.1.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports.tarfile-1.1.1.dist-info/METADATA
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports.tarfile-1.1.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/backports.tarfile-1.1.1.dist-info/WHEEL
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/__init__.py
--rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/__main__.py
--rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/_builder.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/_ctx.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/_exceptions.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/_types.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/_util.py
--rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/py.typed
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/_compat/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/_compat/importlib.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/_compat/tarfile.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build/_compat/tomllib.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build-1.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build-1.2.1.dist-info/LICENSE
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build-1.2.1.dist-info/METADATA
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build-1.2.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build-1.2.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/build-1.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi/__main__.py
--rw-r--r--   0        0        0   292541 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi/cacert.pem
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi-2024.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi-2024.2.2.dist-info/LICENSE
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi-2024.2.2.dist-info/METADATA
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi-2024.2.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/certifi-2024.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/__init__.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/__main__.py
--rw-r--r--   0        0        0    21723 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/api.py
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/cd.py
--rw-r--r--   0        0        0    42476 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/constant.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/legacy.py
--rw-r--r--   0        0        0    20239 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/md.py
--rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/py.typed
--rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/version.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer/cli/__main__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
--rw-r--r--   0        0        0    34233 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/METADATA
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/RECORD
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/WHEEL
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/INSTALLER
--rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/METADATA
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/RECORD
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/WHEEL
--rw-r--r--   0        0        0    10293 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/__init__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/__main__.py
--rw-r--r--   0        0        0    33045 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/core.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/docutils.conf
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/examples.py
--rw-r--r--   0        0        0    44396 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/frontend.py
--rw-r--r--   0        0        0    22583 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/io.py
--rw-r--r--   0        0        0    80628 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/nodes.py
--rw-r--r--   0        0        0    56956 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/statemachine.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/af.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/ar.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/ca.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/cs.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/da.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/de.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/en.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/eo.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/es.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/fa.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/fi.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/fr.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/gl.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/he.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/it.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/ja.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/ka.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/ko.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/lt.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/lv.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/nl.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/pl.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/pt_br.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/ru.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/sk.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/sv.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/uk.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/zh_cn.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/languages/zh_tw.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/__init__.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/null.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
--rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/__init__.py
--rw-r--r--   0        0        0    16119 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/roles.py
--rw-r--r--   0        0        0   133123 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/states.py
--rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/tableparser.py
--rw-r--r--   0        0        0    14812 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/body.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/html.py
--rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/images.py
--rw-r--r--   0        0        0    26700 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/references.py
--rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/af.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/da.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/de.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/en.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/es.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/he.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/it.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ka.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/readers/__init__.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/readers/doctree.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/readers/pep.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/readers/standalone.py
--rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/transforms/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/transforms/components.py
--rw-r--r--   0        0        0    20809 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/transforms/frontmatter.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/transforms/misc.py
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/transforms/parts.py
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/transforms/peps.py
--rw-r--r--   0        0        0    36821 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/transforms/references.py
--rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/transforms/universal.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/transforms/writer_aux.py
--rw-r--r--   0        0        0    30381 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/__init__.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/code_analyzer.py
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/error_reporting.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/punctuation_chars.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/roman.py
--rw-r--r--   0        0        0    39136 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/smartquotes.py
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/urischemes.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/math/__init__.py
--rw-r--r--   0        0        0    46961 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/math/latex2mathml.py
--rw-r--r--   0        0        0   107808 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/math/math2html.py
--rw-r--r--   0        0        0    56217 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/math/mathalphabet2unichar.py
--rw-r--r--   0        0        0    14564 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/math/mathml_elements.py
--rw-r--r--   0        0        0     9436 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
--rw-r--r--   0        0        0    37497 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/math/tex2unichar.py
--rw-r--r--   0        0        0    18393 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/utils/math/unichar2tex.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/__init__.py
--rw-r--r--   0        0        0    75401 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/_html_base.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/docutils_xml.py
--rw-r--r--   0        0        0    38128 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/manpage.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/null.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/pseudoxml.py
--rw-r--r--   0        0        0    38125 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/html4css1/__init__.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/html4css1/html4css1.css
--rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/italic-field-names.css
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/math.css
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/plain.css
--rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css
--rw-r--r--   0        0        0   138165 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/latex2e/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/latex2e/default.tex
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/latex2e/docutils.sty
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/latex2e/titlepage.tex
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/latex2e/titlingpage.tex
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/latex2e/xelatex.tex
--rw-r--r--   0        0        0   132081 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/styles.odt
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/pep_html/__init__.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/pep_html/pep.css
--rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/__base__
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/opera.css
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.css
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/__base__
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/__base__
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
--rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils/writers/xetex/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils-0.21.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils-0.21.2.dist-info/METADATA
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils-0.21.2.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/docutils-0.21.2.dist-info/WHEEL
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna/__init__.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna/compat.py
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna/core.py
--rw-r--r--   0        0        0    78320 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna/py.typed
--rw-r--r--   0        0        0   206503 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna/uts46data.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna-3.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna-3.7.dist-info/LICENSE.md
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna-3.7.dist-info/METADATA
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna-3.7.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/idna-3.7.dist-info/WHEEL
--rw-r--r--   0        0        0    34302 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/_text.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/diagnose.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/compat/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata/compat/py39.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/METADATA
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco/context.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco/classes/__init__.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco/classes/ancestry.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco/classes/meta.py
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco/classes/properties.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco/classes/py.typed
--rw-r--r--   0        0        0    16642 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco/functools/__init__.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco/functools/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco/functools/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/METADATA
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/METADATA
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.functools-4.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.functools-4.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.functools-4.0.1.dist-info/METADATA
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.functools-4.0.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/jaraco.functools-4.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/__main__.py
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backend.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backend_complete.bash
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backend_complete.zsh
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/cli.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/completion.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/core.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/credentials.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/devpi_client.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/errors.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/http.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/py.typed
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/SecretService.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/Windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/__init__.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/chainer.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/fail.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/kwallet.py
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/libsecret.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/null.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/macOS/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/backends/macOS/api.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/compat/__init__.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/compat/properties.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/compat/py312.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/compat/py38.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/testing/__init__.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/testing/backend.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/testing/util.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/util/__init__.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring/util/platform_.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring-25.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring-25.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring-25.2.0.dist-info/METADATA
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring-25.2.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/keyring-25.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/_compat.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/_punycode.py
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/main.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/parser_block.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/parser_core.py
--rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/parser_inline.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/port.yaml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/py.typed
--rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/renderer.py
--rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/ruler.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/token.py
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/tree.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/cli/__init__.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/cli/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/common/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/common/entities.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/common/html_blocks.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/common/html_re.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/common/normalize_url.py
--rw-r--r--   0        0        0    10728 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/common/utils.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/helpers/__init__.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/presets/__init__.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/presets/commonmark.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/presets/default.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/presets/zero.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/__init__.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/blockquote.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/code.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/fence.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/heading.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/hr.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/html_block.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/lheading.py
--rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/list.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/paragraph.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/reference.py
--rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/state_block.py
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_block/table.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_core/__init__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_core/block.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_core/inline.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_core/linkify.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_core/normalize.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_core/replacements.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_core/state_core.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_core/text_join.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/__init__.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/autolink.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/backticks.py
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/entity.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/escape.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/fragments_join.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/image.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/link.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/linkify.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/newline.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it/rules_inline/text.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/METADATA
--rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl/__init__.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl/_decode.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl/_encode.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl/_format.py
--rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl/_parse.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl/_url.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/WHEEL
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools/__init__.pyi
--rw-r--r--   0        0        0   143045 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools/more.py
--rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools/more.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools/py.typed
--rw-r--r--   0        0        0    27548 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools/recipes.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools/recipes.pyi
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools-10.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools-10.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0    34886 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools-10.2.0.dist-info/METADATA
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools-10.2.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/more_itertools-10.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/nh3/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/nh3/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/nh3/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/nh3-0.2.17.dist-info/INSTALLER
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/nh3-0.2.17.dist-info/METADATA
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/nh3-0.2.17.dist-info/RECORD
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/nh3-0.2.17.dist-info/WHEEL
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/_elffile.py
--rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/_manylinux.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/_musllinux.py
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/markers.py
--rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/py.typed
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/requirements.py
--rw-r--r--   0        0        0    39784 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/specifiers.py
--rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/tags.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/utils.py
--rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging-24.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging-24.0.dist-info/METADATA
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging-24.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/packaging-24.0.dist-info/WHEEL
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/py.typed
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10234 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    20942 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8020 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    29381 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    31726 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16503 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37596 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    17552 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    18083 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    12190 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0        0        0    27407 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35600 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24045 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24129 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    27878 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    21617 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11728 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0    80114 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   286370 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    13919 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30068 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13280 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34557 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/_compat.py
--rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/build.py
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/check.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/meta.py
--rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0        0        0    12831 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    32005 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    70232 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53376 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35287 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     5944 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    95885 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11471 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    36576 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59746 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24224 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    26240 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    34697 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39515 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    44666 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    26060 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    18364 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39093 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30109 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17182 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22001 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/METADATA
--rw-r--r--   0        0        0    76141 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/WHEEL
--rw-r--r--   0        0        0   108568 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   132569 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    18410 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/__init__.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/__init__.pyi
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/bdist.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/bdist.pyi
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/commandline.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/commandline.pyi
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/develop.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/develop.pyi
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/distribution.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/distribution.pyi
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/index.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/index.pyi
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/installed.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/installed.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/py.typed
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/sdist.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/sdist.pyi
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/utils.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/utils.pyi
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/wheel.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/wheel.pyi
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/__init__.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/test_bdist.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/test_commandline.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/test_develop.py
--rw-r--r--   0        0        0    19713 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/test_distribution.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/test_index.py
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/test_installed.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/test_sdist.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/test_utils.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo/tests/test_wheel.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo-1.10.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo-1.10.0.dist-info/METADATA
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo-1.10.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pkginfo-1.10.0.dist-info/WHEEL
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/__init__.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/__main__.py
--rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/filter.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatter.py
--rw-r--r--   0        0        0    35044 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/modeline.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/scanner.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/sphinxext.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/style.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/util.py
--rw-r--r--   0        0        0    40338 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35640 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/html.py
--rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/img.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/other.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_ada_builtins.py
--rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_asy_builtins.py
--rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_cl_builtins.py
--rw-r--r--   0        0        0   105182 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
--rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_csound_builtins.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_css_builtins.py
--rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_julia_builtins.py
--rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py
--rw-r--r--   0        0        0   108094 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_lua_builtins.py
--rw-r--r--   0        0        0    68026 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_mql_builtins.py
--rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py
--rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py
--rw-r--r--   0        0        0   107930 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_php_builtins.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py
--rw-r--r--   0        0        0    52413 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py
--rw-r--r--   0        0        0    26781 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
--rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_stan_builtins.py
--rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_stata_builtins.py
--rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_usd_builtins.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
--rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/_vim_builtins.py
--rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/actionscript.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ada.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/agile.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/algebra.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ambient.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/amdgpu.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ampl.py
--rw-r--r--   0        0        0    30766 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/apdlexer.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/apl.py
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/archetype.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/arrow.py
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/arturo.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/asc.py
--rw-r--r--   0        0        0    41243 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/asm.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/asn1.py
--rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/automation.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/bare.py
--rw-r--r--   0        0        0    27923 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/basic.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/bdd.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/berry.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/bibtex.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/blueprint.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/boa.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/bqn.py
--rw-r--r--   0        0        0    28112 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/business.py
--rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/c_cpp.py
--rw-r--r--   0        0        0    29206 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/c_like.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/capnproto.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/carbon.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/cddl.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/chapel.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/clean.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/comal.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/compiled.py
--rw-r--r--   0        0        0    50077 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/configs.py
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/console.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/cplint.py
--rw-r--r--   0        0        0    15757 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/crystal.py
--rw-r--r--   0        0        0    16994 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/csound.py
--rw-r--r--   0        0        0    25322 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/css.py
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/d.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/dalvik.py
--rw-r--r--   0        0        0    27032 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/data.py
--rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/dax.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/devicetree.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/diff.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/dns.py
--rw-r--r--   0        0        0    37623 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/dotnet.py
--rw-r--r--   0        0        0    36786 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/dsls.py
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/dylan.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ecl.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/eiffel.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/elm.py
--rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/elpi.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/email.py
--rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/erlang.py
--rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/esoteric.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ezhil.py
--rw-r--r--   0        0        0    19531 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/factor.py
--rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/fantom.py
--rw-r--r--   0        0        0     9646 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/felix.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/fift.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/floscript.py
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/forth.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/fortran.py
--rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/foxpro.py
--rw-r--r--   0        0        0    26914 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/freefem.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/func.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/functional.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/futhark.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/gcodelexer.py
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/gdscript.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/go.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/grammar_notation.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/graph.py
--rw-r--r--   0        0        0    39026 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/graphics.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/graphql.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/graphviz.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/gsql.py
--rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/haskell.py
--rw-r--r--   0        0        0    30976 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/haxe.py
--rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/hdl.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/hexdump.py
--rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/html.py
--rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/idl.py
--rw-r--r--   0        0        0    31658 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/igor.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/inferno.py
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/installers.py
--rw-r--r--   0        0        0    57119 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/int_fiction.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/iolang.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/j.py
--rw-r--r--   0        0        0    62859 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/javascript.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/jmespath.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/jslt.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/jsonnet.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/jsx.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/julia.py
--rw-r--r--   0        0        0    72929 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/jvm.py
--rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/kuin.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/kusto.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ldap.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/lean.py
--rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/lilypond.py
--rw-r--r--   0        0        0   144398 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/lisp.py
--rw-r--r--   0        0        0    32171 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/macaulay2.py
--rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/make.py
--rw-r--r--   0        0        0    60257 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/markup.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/math.py
--rw-r--r--   0        0        0   132852 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/matlab.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/maxima.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/meson.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/mime.py
--rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/minecraft.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/mips.py
--rw-r--r--   0        0        0    35315 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ml.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/modeling.py
--rw-r--r--   0        0        0    53073 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/modula2.py
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/monte.py
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/mosel.py
--rw-r--r--   0        0        0    63962 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ncl.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/nimrod.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/nit.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/nix.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/oberon.py
--rw-r--r--   0        0        0    22961 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/objective.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ooc.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/openscad.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/other.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/parasail.py
--rw-r--r--   0        0        0    25904 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/parsers.py
--rw-r--r--   0        0        0    30880 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/pascal.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/pawn.py
--rw-r--r--   0        0        0    39170 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/perl.py
--rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/phix.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/php.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/pointless.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/pony.py
--rw-r--r--   0        0        0    12677 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/praat.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/procfile.py
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/prolog.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/promql.py
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/prql.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ptx.py
--rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/python.py
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/q.py
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/qlik.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/qvt.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/r.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/rdf.py
--rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/rebol.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/resource.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ride.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/rita.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/rnc.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/roboconf.py
--rw-r--r--   0        0        0    18449 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/robotframework.py
--rw-r--r--   0        0        0    22672 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ruby.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/rust.py
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/sas.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/savi.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/scdoc.py
--rw-r--r--   0        0        0    70014 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/scripting.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/sgf.py
--rw-r--r--   0        0        0    36466 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/shell.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/sieve.py
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/slash.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/smalltalk.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/smithy.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/smv.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/snobol.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/solidity.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/sophia.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/special.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/spice.py
--rw-r--r--   0        0        0    42107 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/sql.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/srcinfo.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/stata.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/supercollider.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/tal.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/tcl.py
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/teal.py
--rw-r--r--   0        0        0    72610 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/templates.py
--rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/teraterm.py
--rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/testing.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/text.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/textedit.py
--rw-r--r--   0        0        0    15310 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/textfmts.py
--rw-r--r--   0        0        0    16659 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/theorem.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/thingsdb.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/tlb.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/tls.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/tnt.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/trafficscript.py
--rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/typoscript.py
--rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/ul4.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/unicon.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/urbi.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/usd.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/varnish.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/verification.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/verifpal.py
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/vip.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/vyper.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/web.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/webassembly.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/webidl.py
--rw-r--r--   0        0        0    40549 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/webmisc.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/wgsl.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/whiley.py
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/wowtoc.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/wren.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/x10.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/xorg.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/yang.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/yara.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/lexers/zig.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/__init__.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/_mapping.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/abap.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/algol.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/algol_nu.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/arduino.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/autumn.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/borland.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/bw.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/colorful.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/default.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/dracula.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/emacs.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/friendly.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/friendly_grayscale.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/fruity.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/gh_dark.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/gruvbox.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/igor.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/inkpot.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/lightbulb.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/lilypond.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/lovelace.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/manni.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/material.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/monokai.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/murphy.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/native.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/nord.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/onedark.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/paraiso_dark.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/paraiso_light.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/pastie.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/perldoc.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/rainbow_dash.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/rrt.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/sas.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/solarized.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/staroffice.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/stata_dark.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/stata_light.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/tango.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/trac.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/vim.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/vs.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/xcode.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments/styles/zenburn.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments-2.17.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments-2.17.2.dist-info/METADATA
--rw-r--r--   0        0        0    45069 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments-2.17.2.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments-2.17.2.dist-info/WHEEL
--rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pyproject_hooks/py.typed
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pyproject_hooks-1.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pyproject_hooks-1.1.0.dist-info/METADATA
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pyproject_hooks-1.1.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pyproject_hooks-1.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/METADATA
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer/__init__.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer/__main__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer/clean.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer/markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer/py.typed
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer/rst.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer/txt.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer-43.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer-43.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer-43.0.dist-info/METADATA
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer-43.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/readme_renderer-43.0.dist-info/WHEEL
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/_internal_utils.py
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/auth.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/certs.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/cookies.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/exceptions.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/hooks.py
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/models.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/structures.py
--rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests-2.31.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests-2.31.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests-2.31.0.dist-info/METADATA
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests-2.31.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests-2.31.0.dist-info/WHEEL
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/__init__.py
--rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/_compat.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/exceptions.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/sessions.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/__init__.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/source.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py
--rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/x509.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/auth/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/auth/guess.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/auth/handler.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/cookies/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py
--rw-r--r--   0        0        0    20769 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/pool.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/thread.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/utils/__init__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/utils/dump.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/utils/formdata.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0    14638 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/__init__.py
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/_mixin.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/abnf_regexp.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/api.py
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/builder.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/compat.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/exceptions.py
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/iri.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/misc.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/normalizers.py
--rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/parseresult.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/uri.py
--rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986/validators.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/__init__.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/__main__.py
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_export_format.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_inspect.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_pick.py
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_timer.py
--rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_win32_console.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_windows.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_windows_renderer.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/_wrap.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/abc.py
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/ansi.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/bar.py
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/box.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/cells.py
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/columns.py
--rw-r--r--   0        0        0    99101 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/constrain.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/containers.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/control.py
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/default_styles.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/diagnose.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/filesize.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/highlighter.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/json.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/jupyter.py
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/layout.py
--rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/live.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/live_render.py
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/logging.py
--rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/markdown.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/measure.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/pager.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/palette.py
--rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/panel.py
--rw-r--r--   0        0        0    35812 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/pretty.py
--rw-r--r--   0        0        0    59703 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/progress.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/progress_bar.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/prompt.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/region.py
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/repr.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/rule.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/scope.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/screen.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/spinner.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/style.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/styled.py
--rw-r--r--   0        0        0    35367 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/syntax.py
--rw-r--r--   0        0        0    39644 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/terminal_theme.py
--rw-r--r--   0        0        0    47300 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/themes.py
--rw-r--r--   0        0        0    29529 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/traceback.py
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich/tree.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich-13.7.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich-13.7.1.dist-info/LICENSE
--rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich-13.7.1.dist-info/METADATA
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich-13.7.1.dist-info/RECORD
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/rich-13.7.1.dist-info/WHEEL
--rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_entry_points.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_importlib.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_itertools.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_path.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_reqs.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    19539 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0   137216 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/cli-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    20799 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/discovery.py
--rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0   137728 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/gui-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/logging.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    47724 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    40020 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/py34compat.py
--rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14789 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    47369 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    17973 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    50186 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    13713 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    30235 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23602 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    18858 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    22051 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    31558 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    16568 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    30221 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0        0        0    30130 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    16623 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/build.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    14115 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    85662 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    31188 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0        0        0    26795 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/__init__.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0        0        0    16319 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/expand.py
--rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0        0        0    25198 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0        0        0   269900 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools-65.5.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools-65.5.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools-65.5.0.dist-info/METADATA
--rw-r--r--   0        0        0    37694 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools-65.5.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools-65.5.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/setuptools-65.5.0.dist-info/WHEEL
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/__main__.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/auth.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/cli.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/exceptions.py
--rw-r--r--   0        0        0    11018 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/py.typed
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/repository.py
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/settings.py
--rw-r--r--   0        0        0    10979 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/utils.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/wheel.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/wininst.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/commands/__init__.py
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/commands/check.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/commands/register.py
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine/commands/upload.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine-5.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine-5.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine-5.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine-5.0.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine-5.0.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/twine-5.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/__init__.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/_base_connection.py
--rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/_collections.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/_request_methods.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/_version.py
--rw-r--r--   0        0        0    34704 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/connection.py
--rw-r--r--   0        0        0    43556 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/exceptions.py
--rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/fields.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/filepost.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/http2.py
--rw-r--r--   0        0        0    22935 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/py.typed
--rw-r--r--   0        0        0    43874 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0    19161 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/contrib/socks.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/contrib/emscripten/__init__.py
--rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/contrib/emscripten/connection.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/contrib/emscripten/fetch.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/contrib/emscripten/request.py
--rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/contrib/emscripten/response.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/connection.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/request.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/response.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/retry.py
--rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/timeout.py
--rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3/util/wait.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3-2.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3-2.2.1.dist-info/METADATA
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3-2.2.1.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/urllib3-2.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/__init__.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/pywintypes.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/version.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/win32api.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/win32cred.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/_winerrors.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/compat.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/__init__.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_common.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_time.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_util.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_time.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/pywin32/__init__.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
--rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/pywin32/win32api.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/tests/__init__.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/tests/test_backends.py
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/tests/test_win32api.py
--rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/zipp/__init__.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/zipp/glob.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/zipp/compat/__init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/zipp/compat/py310.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/zipp-3.18.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/zipp-3.18.1.dist-info/LICENSE
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/zipp-3.18.1.dist-info/METADATA
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/zipp-3.18.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Lib/site-packages/zipp-3.18.1.dist-info/WHEEL
--rw-r--r--   0        0        0    24167 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/activate
--rwxr-xr-x   0        0        0     1000 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/activate.bat
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   108404 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/docutils.exe
--rwxr-xr-x   0        0        0   108398 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/keyring.exe
--rwxr-xr-x   0        0        0   108408 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/markdown-it.exe
--rwxr-xr-x   0        0        0   108421 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/normalizer.exe
--rwxr-xr-x   0        0        0   108409 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108409 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/pip3.11.exe
--rwxr-xr-x   0        0        0   108409 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   108406 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/pkginfo.exe
--rwxr-xr-x   0        0        0   108403 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/pygmentize.exe
--rwxr-xr-x   0        0        0   108413 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/pyproject-build.exe
--rwxr-xr-x   0        0        0   268160 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/python.exe
--rwxr-xr-x   0        0        0   256376 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/pythonw.exe
--rwxr-xr-x   0        0        0   108408 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2html.exe
--rwxr-xr-x   0        0        0   108410 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2html4.exe
--rwxr-xr-x   0        0        0   108410 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2html5.exe
--rwxr-xr-x   0        0        0   108410 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2latex.exe
--rwxr-xr-x   0        0        0   108406 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2man.exe
--rwxr-xr-x   0        0        0   108406 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2odt.exe
--rwxr-xr-x   0        0        0   108418 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2pseudoxml.exe
--rwxr-xr-x   0        0        0   108404 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2s5.exe
--rwxr-xr-x   0        0        0   108410 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2xetex.exe
--rwxr-xr-x   0        0        0   108406 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/rst2xml.exe
--rwxr-xr-x   0        0        0   108401 2020-02-02 00:00:00.000000 coldp-2024.0.2/venv/Scripts/twine.exe
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coldp-2024.0.2/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coldp-2024.0.2/LICENSE
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 coldp-2024.0.2/README.md
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 coldp-2024.0.2/pyproject.toml
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 coldp-2024.0.2/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 coldp-2024.5.2/.gitattributes
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 coldp-2024.5.2/VERSION
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 coldp-2024.5.2/makefile
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coldp-2024.5.2/version.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/make.bat
+-rw-r--r--   0        0        0    97590 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/coldp.html
+-rw-r--r--   0        0        0    25588 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/index.html
+-rw-r--r--   0        0        0    13217 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/name-bundle.html
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/search.html
+-rw-r--r--   0        0        0    21036 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/source/coldp.rst
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/source/conf.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/source/index.rst
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/source/name-bundle.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/__init__.py
+-rw-r--r--   0        0        0   100701 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/coldp.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/coldp_coldp.svg
+-rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/coldp_distribution.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/testit.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/Distribution.tsv
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/Media.tsv
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/NameRelation.tsv
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/NameUsage.tsv
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/Reference.tsv
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/SpeciesEstimate.tsv
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/SpeciesInteraction.tsv
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/TaxonConceptRelation.tsv
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/TypeMaterial.tsv
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/VernacularName.tsv
+-rw-r--r--   0        0        0   697219 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/logo.png
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/metadata.yaml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/reference.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 coldp-2024.5.2/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coldp-2024.5.2/LICENSE
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 coldp-2024.5.2/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 coldp-2024.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 coldp-2024.5.2/PKG-INFO
```

### Comparing `coldp-2024.0.2/src/coldp/coldp.py` & `coldp-2024.5.2/src/coldp/coldp.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 # -*- coding: utf-8 -*-
 # ----------------------------------------------------------------------------
 # Created By  : Donald Hobern, dhobern@gmail.com
 # Created Date: 2022-11-27
 # version ='2024.0.2'
 # ---------------------------------------------------------------------------
 """ 
-COLDP.py
-
 COLDP is a Python class for creating or loading, manipulating and serialising 
-Catalogue of Life Data Package (COLDP) files.
+Catalogue of Life Data Package (COLDP) files, the preferred format within 
+Catalogue of Life for organising taxonomic checklist datasets. 
 
-COLDP is the preferred format within Catalogue of Life for organising taxonomic 
-checklist datasets. See: https://github.com/CatalogueOfLife/coldp 
+See: https://github.com/CatalogueOfLife/coldp 
 """
 # ---------------------------------------------------------------------------
 # Imports
 # ---------------------------------------------------------------------------
 import pandas as pd
 import numpy as np
 import logging
@@ -255,95 +253,114 @@
 # ---------------------------------------------------------------------------
 name_from_nameusage = {
     "status": "nameStatus",
     "genus": "genericName",
     "referenceID": "nameReferenceID",
     "remarks": "nameRemarks",
 }
+""" Dictionary mapping names of columns in COLDP Name records to the corresponding column names in COLDP NameUsage records """
 
 taxon_from_nameusage = {"nameID": "ID", "provisional": "status"}
+""" Dictionary mapping names of columns in COLDP Taxon records to the corresponding column names in COLDP NameUsage records """
 
 synonym_from_nameusage = {"taxonID": "parentID", "nameID": "ID"}
+""" Dictionary mapping names of columns in COLDP Synonym records to the corresponding column names in COLDP NameUsage records """
 
 # ----------------------------------------------------------------------------
 # Dictionary for mappings between id columns in tables
 #
 # The keys to the outer dictionary are table names (for use with
 # table_by_name()) which contain an "ID" column. Each key is associated with
 # an inner dictionary that maps the name of another (or sometimes the same
 # table) to a list of columns that contain ID values from the first table.
 # ----------------------------------------------------------------------------
 id_mappings = {
     "name": {
         "name": ["basionymID"],
         "taxon": ["nameID"],
-        "name_relation": ["nameID", "relatedNameID"],
+        "namerelation": ["nameID", "relatedNameID"],
         "synonym": ["nameID"],
     },
     "taxon": {
         "taxon": ["parentID"],
         "distribution": ["taxonID"],
-        "species_interaction": ["taxonID", "relatedTaxonID"],
+        "speciesinteraction": ["taxonID", "relatedTaxonID"],
         "synonym": ["taxonID"],
     },
     "reference": {
         "name": ["sourceID", "referenceID"],
         "taxon": ["sourceID", "referenceID", "nameReferenceID"],
         "synonym": ["sourceID", "referenceID"],
-        "type_material": ["referenceID"],
+        "typematerial": ["referenceID"],
         "distribution": ["referenceID"],
-        "species_interaction": ["referenceID"],
-        "name_relation": ["referenceID"],
+        "speciesinteraction": ["referenceID"],
+        "namerelation": ["referenceID"],
     },
     "synonym": {},
 }
+"""
+Dictionary mapping table names (name, taxon, reference or synonym) to a
+dictionary that maps another table name to the properties in the second table
+that reference ID values from the first table.
+
+For example, :py:data:`~coldp.COLDP.id_mappings` maps the key "name" to a 
+dictionary that includes the key "namerelation" with a list containing 
+"nameID" and "relatedNameID" as its value.
+
+This is a map of the foreign-key relationships that need to be validated 
+and preserved between the COLDP data tables.
+"""
 
 # ---------------------------------------------------------------------------
 # Recognised file extensions and their associated separator characters
 # ---------------------------------------------------------------------------
 csv_extensions = {"csv": ",", "tsv": "\t", "txt": "\t"}
+"""
+Dictionary mapping supported CSV/TSV file extensions to the expected delimiter.
+
+Supported extensions are .csv for comma-separated data files and .tsv or .txt for tab-delimited data files.
+"""
 
 # ---------------------------------------------------------------------------
 # Regular expression patterns for uninomial and species-rank epithets and a
 # superset expression including both
 # ---------------------------------------------------------------------------
 uninomial_pattern = re.compile("^[A-Z][a-z]+$")
 epithet_pattern = re.compile("^[a-z]-?[a-z]+$")
 name_pattern = re.compile("^[A-Za-z]-?[a-z]+$")
 
 
 class NameBundle:
     """
-    CLASS: NameBundle
-
     Wrapper class to manage set of associated names, normally an accepted name
     and one or more synonyms. The bundle handles the logic of associated name
     variations.
 
-    Usage:
-      The minimal usage is to create a new bundle with an accepted name. One
-      or more synonyms can also be supplied using the add_synonym() method.
-      The bundle is then submitted to the COLDP add_names method for
-      processing.
+    :param coldp: :py:class:`~coldp.COLDP` object to handle logging of any issues and normalise name records
+    :param accepted: Dictionary mapping COLDP name elements to values for the accepted name - a name record and a taxon record will be added to the COLDP package for the accepted name
+    :param incertae_sedis: Flag to indicate if the resulting taxon record should be marked "incertae sedis"
+    :param sic: Flag to indicate if the accepted name should be processed without reporting issues for invalid format
+
+    The minimal usage is to create a new bundle with an accepted name. One
+    or more synonyms can also be supplied using the :py:func:`~coldp.NameBundle.add_synonym` method.
+    The bundle is then submitted to the :py:func:`coldp.COLDP.add_names` method for
+    processing.
+
+    NameBundle objects should not be created directly. Use the :py:punc`coldp.COLDP.start_name_bundle` method instead.
+
+    accepted should contain a dictionary with keys that match property names from the `COLDP Name class <https://github.com/CatalogueOfLife/coldp?tab=readme-ov-file#name>`_
     """
 
     def __init__(
-        self, coldp, accepted: dict, incertae_sedis: bool = False, sic: bool = False
+        self,
+        coldp,
+        accepted: dict[str:str],
+        incertae_sedis: bool = False,
+        sic: bool = False,
     ) -> None:
-        """
-        __init__ - Initialise NameBundle
-
-        coldp: COLDP object to handle logging of any issues and normalise
-            name records
-        accepted: Dictionary mapping COLDP name elements to values for the
-            accepted name - a name record and a taxon record will be added to
-            the COLDP package for the accepted name
-        incertae_sedis: Flag to indicate if the resulting taxon record should
-            be marked "incertae sedis"
-        """
 
         self.coldp = coldp
         if "rank" not in accepted:
             self.coldp.issue(
                 "Accepted name missing rank, assume species: " + str(accepted)
             )
             accepted["rank"] = "species"
@@ -352,25 +369,23 @@
         self.incertae_sedis = incertae_sedis
         self.accepted_taxon_id = None
         self.synonyms = []
         self.species = None
         self.species_synonym = None
         self.accepted_species_id = None
 
-    def add_synonym(self, synonym: dict, sic: bool = False) -> None:
+    def add_synonym(self, synonym: dict[str:str], sic: bool = False) -> None:
         """
-        add_synonym - Register an additional name as a synonym for the accepted
-            name
+        Register an additional name as a synonym for the accepted name
+
+        synonym should contain a dictionary with keys that match property names from the `COLDP Name class <https://github.com/CatalogueOfLife/coldp?tab=readme-ov-file#name>`_
+
+        :param synonym: Dictionary mapping COLDP name elements to values for the synonymous name - a name record and a synonym record will be added to the COLDP package for the synonym
+        :param sic: Flag to indicate that the name does not follow expected formatting rules for a code-compliant name and that no issues should be logged for this
 
-        synonym: Dictionary mapping COLDP name elements to values for the
-            synonymous name - a name record and a synonym record will be
-            added to the COLDP package for the synonym
-        sic: Flag to indicate that the name does not follow expected
-            formatting rules for a code-compliant name and that no issues
-            should be logged for this
         """
 
         normalised = self.normalise_name(synonym, sic)
         present = normalised["scientificName"] == self.accepted["scientificName"]
         if not present:
             for s in self.synonyms:
                 if normalised["scientificName"] == s["scientificName"]:
@@ -380,25 +395,21 @@
                         or normalised["authorship"] == s["authorship"]
                     ):
                         present = True
                         break
         if not present:
             self.synonyms.append(self.normalise_name(synonym, sic))
 
-    def normalise_name(self, name: dict, sic: bool = False) -> dict:
+    def normalise_name(self, name: dict[str:str], sic: bool = False) -> dict:
         """
-        normalise_name - Ensure that a name record dictionary contains all
-            necessary/appropriate elements
+        Ensure that a name record dictionary contains all necessary/appropriate elements
 
-        name: Dictionary containing name to be normalised
-        sic: Flag to indicate that the name does not follow expected
-            formatting rules for a code-compliant name and that no issues
-            should be logged for this
-
-        Returns name dictionary updated with extra values
+        :param name: Dictionary containing name to be normalised
+        :param sic: Flag to indicate that the name does not follow expected formatting rules for a code-compliant name and that no issues should be logged for this
+        :return: Name dictionary updated with extra values
         """
 
         # Ensure main elements are present in dictionary
         for k in [
             "uninomial",
             "genus",
             "infragenericEpithet",
@@ -455,23 +466,23 @@
                 )
             else:
                 name["scientificName"] = name["uninomial"]
 
         # Return normalised version of name
         return name
 
-    def derive_name(self, name: dict, values: dict, sic: bool = False) -> dict:
-        """
-        derive_name - Use supplied values to create new name dictionary with
-            missing elements copied from an existing name dictionary
-
-        name: Dictionary containing name on which new name is to be based
-        values: Dictionary of values to override values in name
-
-        Returns name dictionary with supplied values supplemented from name
+    def derive_name(
+        self, name: dict[str:str], values: dict[str:str], sic: bool = False
+    ) -> dict:
+        """
+        Use supplied values to create new name dictionary with missing elements copied from an existing name dictionary
+
+        :param name: Dictionary containing name on which new name is to be based
+        :param values: Dictionary of values to override values in name
+        :return: Name dictionary with supplied values supplemented from name
         """
 
         if (
             "authorship" not in values
             and "authorship" in name
             and not name["authorship"].startswith("(")
         ):
@@ -493,84 +504,96 @@
             if k in name and k not in values:
                 values[k] = name[k]
         return self.normalise_name(values, sic)
 
 
 class COLDP:
     """
-    CLASS: COLDP
-
     Class to manage a set of Pandas dataframes for CSV tables in Catalogue
     of Life Data Package.
 
-    Usage:
-    Initialise the COLDP object with folder, COLDP package name and other
-    options. If the package exists in the folder, the COLDP package is
-    initialised as a set of dataframes based on its data. Otherwise empty
-    dataframes are created.
-
-    Data is added using the add_references, add_names, add_typematerial,
-    add_distribution and modify_taxon methods. The start_name_bundle is
-    used to produce a NameBundle object for preparing an accepted name
-    and associated synonyms to pass to add_names.
+    :param name: The name for the COLDP package. If a folder of this name exists inside the folder specied by the folder parameter, this COLDP instance will be initialised with the contents of any COLDP-compliant CSV or TSV files in the named folder.
+    :param folder: Name of folder that may contain the named COLDP source folder from which source files should be read (name specified via the name parameter) and that is the default folder in which a COLDP folder will be written when the COLDP instance is saved. This is not the folder in which the CSV files are written. It is the folder which will contain the subfolder holding CSV files.
+    :param code: ICZN or ICBN to indicate the nomenclatural code for name formatting. ICZN is the default.
+    :param default_taxon_record: Any values in the dictionary are automatically used as default values in taxon records added to the COLDP instance. In other words, the dictionary becomes the base into which other taxon record properties are then inserted.
+    :param insert_species_for_trinomials: If true, insert species (taxon and name) if trinomials are provided without the associated species. This can be convenient when mapping source data that only lists infraspecific taxa for species with subspecies, varieties or forms.
+    :param create_subspecies_for_infrasubspecifics: If true, automatically add a trinomial at subspecific rank as a synonym whenever an infrasubspecific name is added. This may be useful if the resulting dataset is intended to provide easy mapping of strings to taxon concepts, since versions of the trinomial lacking the rank marker will often be found in source data.
+    :param create_synonyms_without_subgenus: If true, automatically add a binomial or trinomial without an included subgenus name as a synonym whenever a name including a subgenus is added. This may be useful if the resulting dataset is intended to provide easy mapping of strings to taxon concepts, since versions of lacking the subgeneric component will often be found in source data.
+    :param basionyms_from_synonyms: If true, basionym associations are automatically created from synonyms within a loaded COLDP dataset. If an accepted name includes parentheses around the authorship, and if a name with the same epithet and authorship but no parentheses is included in the synonyms, the ID value for the synonym will be used for the basionymID element in the accepted name. This is normally a housekeeping step when first loading a new COLDP dataset. This option is only used when the dataset is first loaded. Addition of basionym relationships is automatic for names added as part of the same NameBundle.
+    :param classification_from_parents: If true, insert names for higher ranks into relevant elements in each taxon record based on the parent and higher ancestry for the taxon.
+    :param allow_repeated_binomials: If true, omit checks rejecting the addition of the same binomial more than once to the COLDP name dataframe.
+    :param create_taxa_for_not_established: If true, generate taxon records even if the associated name is flagged as not established (i.e. not satisfying the relevant nomenclatural code)
+    :param issues_to_stdout: If true, print any issue messages (see :py:func:`~coldp.COLDP.issue`) to stdout as well as inserting then in the issue dataframe.
+    :param context: Value to be used in labeling issue records (see :py:func:`~coldp.COLDP.issue`). This value is more normally set using :py:func:`~coldp.COLDP.set_context`.
+
+    A COLDP object is initalised with a source/destination folder, COLDP package
+    name and other options.
+
+    If a subfolder exists with the supplied name in the supplied folder, it
+    will be initialised with data from any CSV/TSV files it contains with any
+    of the following base names: name, taxon, synonym, reference,
+    distribution, speciesinteraction, namerelation, typematerial or nameusage,
+    and with a file extension recognised via :py:data:`~coldp.COLDP.csv_extensions`.
+    File names are case insensitive.
+
+    Files with the base name nameusage are loaded only if the name, taxon or
+    synonym file is absent, in which case the contents of the nameusage file
+    are mapped internally to the more normalised COLDP format with separate
+    name + taxon + synonym tables.
+
+    If no folder exists with the supplied name, an empty instance is created.
+    Pandas dataframes are created as required for the COLDP data types as
+    data are inserted into the instance.
+
+    The :py:func:`~coldp.COLDP.start_name_bundle` method produces a :py:class:`~coldp.COLDP.NameBundle` object for preparing an
+    accepted name and associated synonyms to pass to the :py:func:`~coldp.COLDP.add_names` method
+    which creates name, taxon and synonym records as a set of cross-referenced
+    objects.
+
+    Other data is added using the :py:func:`~coldp.COLDP.add_references, :py:func:`~coldp.COLDP.add_names`, :py:func:`~coldp.COLDP.add_name_relation`,
+    :py:func:`~coldp.COLDP.add_typematerial`, :py:func:`~coldp.COLDP.add_distribution`, :py:func:`~coldp.COLDP.add_species_interaction` and
+    :py:func:`~coldp.COLDP.modify_taxon` methods.
 
-    The save method writes the data back to the same or another folder.
+    The :py:func:`~coldp.COLDP.save` method writes the data back to the same or another folder.
     """
 
-    def __init__(self, folder: str, name: str, **kwargs: dict):
-        """
-        __init__ - Initialise COLDP instance
-
-        folder: Name of folder that may contain the named COLDP source
-            folder from which source files should be read (name specified via
-            the name parameter) and that is the default folder in which a
-            COLDP folder will be written when the COLDP instance is saved. This
-            is not the folder in which the CSV files are written. It is the
-            folder which will contain the subfolder holding CSV files.
-        name: The name for the COLDP package. If a folder of this name exists
-            inside the folder specied by the folder parameter, this COLDP
-            instance will be initialised with the contents of any
-            COLDP-compliant CSV or TSV files in the named folder.
-        kwargs: Set of options for controlling the behaviour of the COLDP
-            package - see set_options().
-
-        If a folder exists with the supplied name in the supplied folder, it
-        will be initialised with data from any CSV/TSV files it contains with any
-        of the following base names: name, taxon, synonym, reference,
-        distribution, speciesinteraction, namerelation, typematerial or nameusage,
-        and with any of the following extensions: .csv, .tsv, .txt. File names
-        are case insensitive.
-
-        Files with the base name nameusage are loaded only if the name, taxon or
-        synonym file is absent, in which case the contents of the nameusage file
-        are mapped internally to the more normalised name + taxon + synonym
-        format.
-
-        If no folder exists with the supplied name, an empty instance is created.
-        Pandas dataframes are created as required for the COLDP data types as
-        data are inserted into the instance.
-        """
+    def __init__(
+        self,
+        name: str,
+        folder: str = ".",
+        code: str = "ICZN",
+        default_taxon_record: dict[str:str] = None,
+        insert_species_for_trinomials: bool = False,
+        create_subspecies_for_infrasubspecifics: bool = False,
+        create_synonyms_without_subgenus: bool = False,
+        basionyms_from_synonyms: bool = False,
+        classification_from_parents: bool = False,
+        allow_repeated_binomials: bool = False,
+        create_taxa_for_not_established: bool = False,
+        issues_to_stdout: bool = False,
+        context: str = None,
+    ) -> None:
 
         self.default_taxon = {
             "provisional": "false",
             "extinct": "false",
             "temporalRangeEnd": "Holocene",
         }
+        self.default_taxon_record = default_taxon_record
         self.code = "ICZN"
-        self.species_from_trinomials = False
-        self.subspecies_from_trinomials = False
-        self.subgenus_free_synonyms = False
-        self.basionyms_from_synonyms = False
-        self.classification_from_parents = False
-        self.allow_repeated_binomials = False
-        self.create_taxa_for_not_established = False
-        self.issues_to_stdout = False
+        self.species_from_trinomials = insert_species_for_trinomials
+        self.subspecies_from_trinomials = create_subspecies_for_infrasubspecifics
+        self.subgenus_free_synonyms = create_synonyms_without_subgenus
+        self.basionyms_from_synonyms = basionyms_from_synonyms
+        self.classification_from_parents = classification_from_parents
+        self.allow_repeated_binomials = allow_repeated_binomials
+        self.create_taxa_for_not_established = create_taxa_for_not_established
+        self.issues_to_stdout = issues_to_stdout
+        self.context = context
 
-        if kwargs:
-            self.set_options(kwargs)
         self.folder = folder
         self.name = name
         if folder is not None:
             source_folder = os.path.join(folder, name)
         else:
             source_folder = None
         self.name_usages = None
@@ -595,136 +618,103 @@
             source_folder, "typematerial", type_material_headings
         )
         if self.classification_from_parents:
             self.fix_classification()
         if self.basionyms_from_synonyms:
             self.fix_basionyms(self.names, self.synonyms)
         self.issues = None
-        self.context = None
 
-    def set(self, **kwargs):
+    def set_options(self, **options: bool):
         """
-        set - Set options controlling COLDP instance
+        Set options controlling COLDP instance from keyword arguments
 
-        kwargs: Set of options for controlling the behaviour of the COLDP
-            package - see set_options().
+        :param options: Set of boolean options for controlling the behaviour of the COLDP package - see :py:class:`~coldp.COLDP` for boolean options that can be set.
 
-        Convenience method for setting options via keyword arguments after the
-        COLDP instance has been created.
-        """
-
-        self.set_options(kwargs)
-
-    def set_options(self, options):
-        """
-        set_options - Set options controlling COLDP instance
-
-        options: Dictionary containing options to control the behaviour of the
-            COLDP instance. Any combination of the following may be specified.
-            Option values may be dictionaries, booleans or string values. All
-            boolean options default to False.
-
-            Dictionary options
-                default_taxon_record
-                    If supplied, any values in the dictionary are automatically
-                    used as default values in taxon records added to the COLDP
-                    instance. In other words, the dictionary becomes the base
-                    into which other taxon record properties are then inserted.
-
-            Boolean options
-                insert_species_for_trinomials
-                    If true, insert species (taxon and name) if trinomials
-                    are provided without the associated species. This can be
-                    convenient when mapping source data that only lists
-                    infraspecific taxa for species with subspecies, varieties
-                    or forms.
-                create_subspecies_for_infrasubspecifics
-                    If true, automatically add a trinomial at subspecific
-                    rank as a synonym whenever an infrasubspecific name is
-                    added. This may be useful if the resulting dataset is
-                    intended to provide easy mapping of strings to taxon
-                    concepts, since versions of the trinomial lacking the
-                    rank marker will often be found in source data.
-                create_synonyms_without_subgenus
-                    If true, automatically add a binomial or trinomial without
-                    an included subgenus name as a synonym whenever a name
-                    including a subgenus is added. This may be useful if the
-                    resulting dataset is intended to provide easy mapping of
-                    strings to taxon concepts, since versions of lacking the
-                    subgeneric component will often be found in source data.
-                basionyms_from_synonyms
-                    If true, basionym associations are automatically created
-                    from synonyms within a NameBundle. In other words, if the
-                    accepted name in a NameBundle includes parentheses around
-                    the authorship, and if a name with the same epithet and
-                    authorship but no parentheses is included in the synonyms,
-                    the ID value for the synonym will be used for the
-                    basionymID element in the accepted name. The same
-                    processing is also carried out on any synonyms that can be
-                    interpreted as subsequent combinations of other names in
-                    the bundle. This is particularly useful if the COLDP
-                    instance is left to allocate all ID values instead of
-                    providing IDs in each supplied record.
-                classification_from_parents
-                    If true, insert names for higher ranks into relevant
-                    elements in each taxon record based on the parent and
-                    higher ancestry for the taxon.
-                allow_repeated_binomials
-                    If true, omit checks rejecting the addition of the same
-                    binomial more than once to the COLDP name dataframe.
-                create_taxa_for_not_established
-                    If true, generate taxon records even if the associated
-                    name is flagged as not established (i.e. not satisfying
-                    the relevant nomenclatural code)
-                issues_to_stdout
-                    If true, print any issue messages (see issue()) to stdout
-                    as well as inserting then in the issue dataframe.
-
-            String options
-                code
-                    ICZN or ICBN to indicate the nomenclatural code for name
-                    formatting. ICZN is the default.
-                context
-                    Value to be used in labeling issue records (see issue()).
-                    This value is more normally set using set_context().
+        Convenience method for setting options via keyword arguments after the COLDP instance has been created.
         """
-
         for key, value in options.items():
             if key == "insert_species_for_trinomials":
                 self.species_from_trinomials = value
             elif key == "create_subspecies_for_infrasubspecifics":
                 self.subspecies_from_trinomials = value
             elif key == "create_synonyms_without_subgenus":
                 self.subgenus_free_synonyms = value
             elif key == "default_taxon_record":
                 self.default_taxon = value
-            elif key == "context":
-                self.context = value
             elif key == "issues_to_stdout":
                 self.issues_to_stdout = value
             elif key == "basionyms_from_synonyms":
                 self.basionyms_from_synonyms = value
             elif key == "classification_from_parents":
                 self.classification_from_parents = value
             elif key == "allow_repeated_binomials":
                 self.allow_repeated_binomials = value
             elif key == "create_taxa_for_not_established":
                 self.create_taxa_for_not_established = value
-            elif key == "code" and value in ["ICZN", "ICBN"]:
-                self.code = value
 
-    def set_context(self, context):
+    def set_default_taxon_record(self, default_taxon_record: dict[str:str]) -> None:
+        """
+        Set default values for properties in taxon records created by this COLDP instance
+
+        :param default_taxon_record: Any values in the dictionary are automatically used as default values in taxon records added to the COLDP instance. In other words, the dictionary becomes the base into which other taxon record properties are then inserted.
+
+        Convenience method for setting default taxon record after the COLDP instance has been created.
+        """
+        self.default_taxon_record = default_taxon_record
+
+    def set_context(self, context: str) -> None:
+        """
+        Set a string label for annotating issues in the COLDP issue table
+
+        :param context: String to label any issues associated with data changes from the current point forward
+
+        The COLDP class automatically logs errors and issues to an issues
+        dataframe. This dataframe is included among the CSV output files when
+        a COLDP instance is saved.
+
+        Each row in the issue table indicates a possible problem with data added
+        to the instance. The context variable provides an external mechanism for
+        the user to label these issues as they occur. For example, if the user
+        is processing a spreadsheet of species names, they can call set_context
+        with a string identifying the row from the source spreadsheet. This
+        value will be included in the context column in the issue.csv output.
+        """
         self.context = context
 
-    def initialise_dataframe(self, foldername, name, default_headings):
+    def initialise_dataframe(
+        self, foldername: str, name: str, default_headings: list[str]
+    ) -> pd.DataFrame:
+        """
+        Load or create a dataframe for one of the COLDP record types
+
+        :param foldername: Path string for COLDP folder potentially containing serialised dataframe
+        :param name: Base name for COLDP class (name, taxon, etc.) for which the dataframe is requested
+        :param default_headings: Column headings to use if returning a new empty dataframe
+        :return: Dataframe for requested COLDP data class
+
+        Checks for a file in the COLDP folder with a supported extension (.csv, .tsv, .txt)
+        and a name matching one of the COLDP record types (name, taxon, synonym,
+        reference, distribution, typematerial or speciesinteraction). If this
+        exists, it is loaded as a Pandas dataframe.
+
+        If it is not found but the name is one of name, taxon or synonym and a
+        file with the name nameusage does exist, the relevant columns will be
+        loaded from the nameusage file.
+
+        If no matching file is found, returns an empty dataframe.
+        """
+
         df = None
         nameusage_filename = None
         if foldername is not None and os.path.isdir(foldername):
             if os.path.isdir(os.path.join(foldername, "data")):
                 foldername = os.path.join(foldername, "data")
+
+            # Look for and load file with expected name, and remember if a
+            # nameusage file is present.
             for filename in os.listdir(foldername):
                 parts = filename.lower().split(".")
                 if parts[0] == "nameusage":
                     nameusage_filename = filename
                 if (
                     len(parts) == 2
                     and parts[0] == name
@@ -732,58 +722,81 @@
                 ):
                     df = pd.read_csv(
                         os.path.join(foldername, filename),
                         dtype=str,
                         keep_default_na=False,
                         sep=csv_extensions[parts[1]],
                     )
+
+                    # Remove namespace component from column names if present
                     columns = df.columns.tolist()
                     for i in range(len(columns)):
                         if ":" in columns[i]:
                             columns[i] = columns[i].split(":")[1]
                     df.columns = columns
                     break
+
+        # As a backup, use nameusage where appropriate
         if (
             df is None
             and nameusage_filename is not None
             and name in ["name", "taxon", "synonym"]
         ):
             if self.name_usages is None:
                 self.name_usages = self.initialise_dataframe(
                     foldername, "nameusage", nameusage_headings
                 )
             if self.name_usages is not None:
                 synonym_statuses = ["synonym", "ambiguous synonym", "misapplied"]
+                # For name, get records from all rows
                 if name == "name":
                     df = self.extract_table(
                         self.name_usages, name_headings, name_from_nameusage
                     )
+                # For synonym, get records from all synonym rows
                 elif name == "synonym":
                     df = self.extract_table(
                         self.name_usages[
                             self.name_usages.status.isin(synonym_statuses)
                         ],
                         synonym_headings,
                         synonym_from_nameusage,
                     )
+                # For taxon, get records from all non-synonym rows
                 else:
                     df = self.extract_table(
                         self.name_usages[
                             ~self.name_usages.status.isin(synonym_statuses)
                         ],
                         taxon_headings,
                         taxon_from_nameusage,
                     )
 
+        # Empty dataframe by default
         if df is None and default_headings is not None:
             df = pd.DataFrame(columns=default_headings)
 
         return df
 
-    def extract_table(self, df, headings, mappings):
+    def extract_table(
+        self, df: pd.DataFrame, headings: list[str], mappings: dict[str:str]
+    ) -> pd.DataFrame:
+        """
+        Extract a set of columns from a dataframe using a dictionary that maps
+        source columns names to target column names
+
+        :param df: Dataframe from which columns are to be extracted/mapped
+        :param headings: List of column headings for destination dataframe
+        :param mappings: Dictionary mapping destination column names to source column names
+        :return: New Dataframe based on supplied mappings
+
+        This method is used to extract and rename a subset of columns from a
+        COLDP NameUsage table.
+        """
+
         table = None
 
         headings_out = []
         headings_in = []
 
         for h in headings:
             m = mappings[h] if h in mappings else h
@@ -793,17 +806,37 @@
 
         if len(headings_in) > 0:
             table = df.loc[:, headings_in]
             table.columns = headings_out
 
         return table
 
-    def fix_basionyms(self, names, synonyms):
+    def fix_basionyms(self, names: pd.DataFrame, synonyms: pd.DataFrame) -> None:
+        """
+        Update dataframe of name records so that subsequent combination names refer to the original basionym record where present
+
+        :param names: Dataframe containing COLDP name records to be updated
+        :param synonyms: Dataframe containing COLDP synonym records corresponding to the name records in names
+
+        For any name record in :paramref:`~coldp.COLDP.fix_basionyms.names`
+        if the name is a subsequent zoological combination (with
+        parentheses around authorship), find any other record in
+        :paramref:`~coldp.COLDP.fix_basionyms.names`
+        that matches the authorship, year and epithet but lacks parentheses and
+        update the basionymID property of the name to refer to this second
+        record's ID. :paramref:`~coldp.COLDP.fix_basionyms.synonyms` is used to
+        assist with selection of the correct match in cases where more than one
+        possible record is found.
+
+        The parameters are the two relevant DataFrames from the same COLDP instance.
+        """
+
         for index, row in names.iterrows():
             if row["authorship"].startswith("("):
+                # Find matches for the final epithet and authorship without parentheses
                 authorship = self.get_original_authorship(row["authorship"])
                 if row["infraspecificEpithet"]:
                     epithet = row["infraspecificEpithet"]
                 else:
                     epithet = row["specificEpithet"]
                 match = names[
                     (names["authorship"] == authorship)
@@ -811,66 +844,113 @@
                         (names["infraspecificEpithet"] == epithet)
                         | (
                             (names["infraspecificEpithet"] == "")
                             & (names["specificEpithet"] == epithet)
                         )
                     )
                 ]
+
+                # If there are multiple potential matches, find one associated
+                # (via synonym records) with the same taxon
                 if len(match) > 1:
                     synonym_match = pd.merge(
                         synonyms[synonyms["taxonID"] == row["ID"]][
                             ["nameID", "taxonID"]
                         ],
                         names,
                         left_on="nameID",
                         right_on="ID",
                         how="left",
                     )[["ID"]]
                     match = pd.merge(match, synonym_match, on="ID", how="inner")
+
+                # Report failures or set basionymID
                 if len(match) == 0:
                     print(
                         f"Cannot find basionym for {row['ID']}: "
                         + f"{row['scientificName']} {row['authorship']}"
                     )
                 elif len(match) == 1:
                     names.loc[names["ID"] == row["ID"], "basionymID"] = match.iloc[0][
                         "ID"
                     ]
             else:
+                # Original combinations are their own basionyms
                 names.loc[names["ID"] == row["ID"], "basionymID"] = row["ID"]
+
+        # Tidy up nominate subspecies
         for index, row in names[
             (names["infraspecificEpithet"] != "")
             & (names["specificEpithet"] == names["infraspecificEpithet"])
         ].iterrows():
             species = names[
                 (names["genus"] == row["genus"])
                 & (names["authorship"] == row["authorship"])
                 & (names["rank"] == "species")
             ]
             if len(species) == 1:
                 names.loc[names["ID"] == row["ID"], "basionymID"] = species.iloc[0][
                     "basionymID"
                 ]
 
-    def fix_classification(self):
+    def fix_classification(self) -> None:
+        """
+        Tidy and fill in higher classification for taxon records based on hierarchy
+
+        Recursively fixes classification elements for whole taxa dataframe
+        """
+
         ranks = self.names.loc[:, ["ID", "rank", "scientificName"]]
         ranks.columns = ["nameID", "rank", "scientificName"]
-        self.fix_classification_recursive(self.taxa, ranks, None)
+        self.fix_classification_recursive(self.taxa, ranks)
 
-    def fix_classification_recursive(self, taxa, ranks, parent):
+    def fix_classification_recursive(
+        self, taxa: pd.DataFrame, ranks: pd.DataFrame, parent: dict[str:str] = None
+    ) -> None:
+        """
+        Recursively complete classification elements (higher taxon IDs) in
+        taxon records descended from a given parent or for all taxon records
+        in the COLDP instance at the highest included rank
+
+        :param taxa: Dataframe containing COLDP taxon records
+        :param ranks: DataFrame containing at least nameID, rank and scientificName for all names in COLDP instance (can be the complete table of COLDP names)
+        :param parent: Taxon record for which children should be updated, or None if all top-level taxa should be updated
+
+        If :paramref:`~coldp.COLDP.fix_classification_recursive.taxa` is None, select all top-level taxa from the dataframe (i.e. all without a parentID) and process these recursively.
+
+        If a parent is supplied, copy classification properties (kingdom, phylum,
+        subphylum, class, subclass, order, suborder, superfamily, family, subfamily,
+        tribe, subtribe, genus, subgenus, section, species) from the parent
+        record, set any rank-specific column matching the rank of the parent
+        to the name of the parent taxon, and then copy these rank values into
+        all taxon records that are immediate descendents of the parent.
+        This will ensure that the higher classification for all children matches
+        this parent. Then call this method recursively for all children.
+        """
+
+        # If no parent provided, get list of taxa at the highest included rank,
+        # expanded to include values from the name record, including rank and
+        # scientificName - these will be passed for the first recursion
         if parent is None:
             for p in range(len(rank_headings)):
                 parents = pd.merge(
                     taxa,
                     ranks[ranks["rank"] == rank_headings[p]],
                     on="nameID",
                     how="right",
                 )
                 if parents is not None and len(parents) > 0:
                     break
+
+        # Otherwise, get the classification columns from the parent and set
+        # any column with a name matching the parent's rank to contain the
+        # parent's name. This will enable it to propagate down on recursion.
+        # Then get the parent's children as the parents for the next recursion
+        # and set all their higher taxon columns to match the parent. Use these
+        # as parents for the next recursion.
         else:
             classification = parent[rank_headings]
             if parent["rank"] in rank_headings:
                 classification[rank_headings.index(parent["rank"])] = parent[
                     "scientificName"
                 ]
 
@@ -879,50 +959,104 @@
             )
             parents = pd.merge(
                 taxa.loc[taxa["parentID"] == parent["ID"]],
                 ranks,
                 on="nameID",
                 how="left",
             )
+
+        # Recurse for all identified parents at the next level
         for i in range(len(parents)):
             self.fix_classification_recursive(taxa, ranks, parents.iloc[i])
 
-    def sort_taxa(self):
+    def sort_taxa(self) -> None:
+        """
+        Sort taxa dataframe so that all taxon records are sequenced
+        hierarchically and alphabetically.
+
+        Following this method, the taxon table is sorted so that any taxa
+        without parents are sorted alphabetically by scientific nameand each is
+        followed immediately by its children and their descendents also sorted
+        alphabetically. The result is a tree with siblings ordered
+        alphabetically.
+
+        Existing ID values for all records are unchanged.
+
+        This is a convenience method to simplify review of the data in a
+        spreadsheet or editor tool. It also simplifies import of the data into
+        a database since there are no forward references to parent taxa.
+        """
+
+        # Get list of all IDs, parentIDs and ranks sorted by scientificName
         df = pd.merge(
             self.taxa,
             self.names,
             left_on="nameID",
             right_on="ID",
             how="left",
             suffixes=["", "_name"],
         )[["ID", "parentID", "rank", "scientificName"]].sort_values(["scientificName"])
 
+        # Get recursively generated list of alternating taxon IDs and the
+        # preferred sequence positions (as strings) for each top-level taxon
+        # and its descendents. At each level, siblings will be sorted
+        # alphabetically and will be followed by their children.
         ids = []
         for index, row in df[
             (df["parentID"] == "") | (df["parentID"].isnull())
         ].iterrows():
             ids = self.sort_taxa_recursive(df, ids, row["ID"])
-        ids = ids + df[~df["ID"].isin(np.array(ids))]["ID"].tolist()
 
+        # Convert alternating list into dictionary
         sort_index = dict(zip(ids, range(len(ids))))
+
+        # Join the preferred sequence positions as a new column, sort on
+        # that column and then drop the sequence values.
         self.taxa["sequence"] = self.taxa["ID"].map(sort_index)
         self.taxa = self.taxa.sort_values(["sequence"])
         self.taxa.drop("sequence", axis=1, inplace=True)
         self.taxa = self.taxa.reset_index(drop=True)
 
-    def sort_taxa_recursive(self, df, ids, id):
-        ids.append(str(len(ids) + 1))
+    def sort_taxa_recursive(
+        self, df: pd.DataFrame, ids: list[str], id: str
+    ) -> list[str]:
+        """
+        Internal method for recursive sorting of taxon records by parent and
+        name
+
+        :param df: Taxa dataframe to be sorted
+        :param ids: Alternative list of IDs and preferred positions (as strings)
+        :param id: Taxon ID for current taxon
+        :return: :paramref:`~coldp.COLDP.sort_taxa_recursive.ids` with additional values for current taxon and its descendents
+
+        Appends next taxon ID to the list along with a value guaranteed to be
+        higher than the one added on the previous execution of this method.
+        Recursively add IDs for children.
+        """
+
         ids.append(id)
+        ids.append(str(len(ids) + 1))
         for index, row in df[df["parentID"] == id].iterrows():
             ids = self.sort_taxa_recursive(df, ids, row["ID"])
         return ids
 
-    def sort_names(self):
+    def sort_names(self) -> None:
+        """
+        Sort name records to match order of records in taxa dataframe and with
+        accepted names and synonyms sorted alphabetically
+
+        Records are sorted first in the current order of the taxon table and
+        then alphabetically within the set of names for each taxon.
+
+        Existing ID values for all records are unchanged.
+
+        This method is most useful following a call to :py:func:`~coldp.COLDP.sort_taxa`.
+        """
         taxon_subset = self.taxa[["ID", "nameID"]]
-        taxon_subset["idx"] = self.taxa.index
+        taxon_subset.loc[:, ["idx"]] = self.taxa.index
         sort_table = pd.merge(
             self.names[["ID"]],
             taxon_subset,
             left_on="ID",
             right_on="nameID",
             how="left",
             suffixes=["", "_taxon"],
@@ -931,74 +1065,105 @@
             sort_table,
             self.synonyms[["taxonID", "nameID"]],
             left_on="ID",
             right_on="nameID",
             how="left",
             suffixes=["", "_synonym"],
         )
-        sort_table.loc[sort_table["idx"].isnull(), ["idx"]] = pd.merge(
-            sort_table.loc[sort_table["idx"].isnull()],
+        sort_table = pd.merge(
+            sort_table,
             taxon_subset,
             left_on="taxonID",
             right_on="ID",
             how="left",
-        )["idx_y"]
-        self.names[["idx"]] = sort_table[["idx"]]
-        self.names = self.names.sort_values(["idx", "scientificName"])
-        self.names.drop(["idx"], axis=1, inplace=True)
+            suffixes=["", "_y"],
+        )
+        sort_table.loc[sort_table["idx"].isnull(), ["idx"]] = sort_table["idx_y"]
+        sort_table["junior"] = True
+        sort_table.loc[sort_table["ID"] == sort_table["nameID"], ["junior"]] = False
+        self.names[["idx", "junior"]] = sort_table[["idx", "junior"]]
+        self.names = self.names.sort_values(["idx", "junior", "scientificName"])
+        self.names.drop(["idx", "junior"], axis=1, inplace=True)
         self.names = self.names.reset_index(drop=True)
 
-    def table_by_name(self, name):
+    def table_by_name(self, name: str) -> pd.DataFrame:
+        """
+        Return dataframe for named COLDP data class
+
+        :param name: Name of data frame to return (one of: name, taxon, synonym, reference, type_material, distribution, species_interaction, name_relation)
+        :return: Requested dataframe or None if no such table exists
+
+        Returns dataframe if one exists for supplied name.
+        """
         tables = {
             "name": self.names,
             "taxon": self.taxa,
             "synonym": self.synonyms,
             "reference": self.references,
-            "type_material": self.type_materials,
+            "typematerial": self.type_materials,
             "distribution": self.distributions,
-            "species_interaction": self.species_interactions,
-            "name_relation": self.name_relations,
+            "speciesinteraction": self.species_interactions,
+            "namerelation": self.name_relations,
         }
         return tables[name] if name in tables.keys() else None
 
-    def reset_ids(self, name=None, prefix=None):
+    def reset_ids(self, name: str = None, prefix: str = None) -> None:
+        """
+        Reset all IDs for one or more COLDP data tables to consecutive values in the order of the table records
+
+        :param name: Table to be modified. One of name, taxon, reference or synonym. If name is None, all four are processed
+        :param prefix: Optional prefix string to be prepended before consecutive integer record ids
+
+        Resets all ids for one or all of the four supported classes to consecutive
+        id values, with an optional string prefix which defaults to ``"s_"`` in the
+        case of synonym records and is otherwise empty.
+
+        Also modifies corresponding foreign ID references in other tables so they
+        continue to resolve correctly using the :py:data:`~coldp.COLDP.id_mappings`
+        dictionary.
+
+        If no table name is specified, all four are processed.
+        """
         for table_name in ["name", "taxon", "reference", "synonym"]:
             if name is None or table_name == name:
                 table = self.table_by_name(table_name)
                 if prefix is None:
                     prefix = ""
                 if prefix == "" and table_name == "synonym":
                     prefix = "s_"
                 table["newID"] = prefix + (table.index + 1).astype(str)
                 by_ids = table.set_index("ID")
+
+                # The id_mappings dictionary identifies references to the
+                # current table in other tables. These will be corrected here.
                 joins = id_mappings[table_name]
                 for key in joins.keys():
                     other_table = self.table_by_name(key)
                     for value in joins[key]:
                         if value in other_table.columns:
                             other_table[value] = other_table[value].map(by_ids["newID"])
+
                 table["ID"] = table["newID"]
                 table.drop("newID", axis=1, inplace=True)
 
-    def add_references(self, reference_list):
+    def add_references(
+        self, reference_list: list[dict[str:str]]
+    ) -> list[dict[str:str]]:
         """
         Ensure one or more references are included in references dataframe
 
-        Parameters:
-        reference_list - list of dictionaries - each dictionary contains
-            values keyed by terms from reference_headings
+        :param reference_list: List of dictionaries - each dictionary contains values keyed by terms from reference_headings
+        :return: Updated :paramref:`~coldp.COLDP.add_references.reference_list` with IDs for references in this COLDP instance
 
-        Behaviour:
         Find existing ID values for each supplied reference, based on identity
-        of: author, title, issued, containerTitle, volume, issue and page. Add
+        of: author, title, issued, containerTitle, volume, issue, page and citation. Add
         ID to the appropriate reference dictionary in references. If none
-        found, set ID to next index and add to references
+        found, set ID to next unused index and add to references.
 
-        Returns:
-        Updated copy of reference_list
+        The list is returned updated with current ID values so these can be used for referenceID values in other classes.
         """
 
         for i in range(len(reference_list)):
             has_content = False
             for k in reference_list[i].keys():
                 if reference_list[i][k]:
                     has_content = True
@@ -1017,23 +1182,44 @@
                         ignore_index=True,
                     )
                     logging.debug("Added reference " + str(r))
             else:
                 reference_list[i]["ID"] = ""
         return reference_list
 
-    def get_reference(self, id):
+    def get_reference(self, id: str) -> dict[str:str]:
+        """
+        Get reference record as dictionary from ID string
+
+        :param id: ID string for requested COLDP reference record
+        :return: Dictionary of COLDP reference properties for requested ID
+
+        Returns None if no matching reference. If multiple records exist with
+        the given id, a warning is logged and the first match is returned.
+        """
         match = self.references[self.references["ID"] == id]
         if len(match) == 0:
             return None
         if len(match) > 1:
             logging.warn(f"Multiple matches for reference ID: {id}")
         return match.to_dict("records")[0]
 
-    def find_reference(self, reference):
+    def find_reference(self, reference: dict[str:str]) -> pd.DataFrame:
+        """
+        Locate existing COLDP reference record exactly matching all major
+        fields in :py:paramref:`~coldp.COLDP.find_reference.reference`
+
+        :param reference: Dictionary of COLDP reference properties representing a record to be found
+        :return: DataFrame with one COLDP reference record if found, else None
+
+        Only returns a record that exactly matches the values supplied in
+        :py:paramref:`~coldp.COLDP.find_reference.reference` for all of
+        author, title, issued, containerTitle, volume, issue, page and citation.
+        """
+
         for k in [
             "ID",
             "author",
             "title",
             "issued",
             "containerTitle",
             "volume",
@@ -1058,29 +1244,59 @@
         if len(match) == 0:
             return None
         return match.iloc[0]
 
     def start_name_bundle(self, accepted, incertae_sedis=False, sic=False):
         return NameBundle(self, accepted, incertae_sedis, sic)
 
-    def add_names(self, bundle, parent):
+    def add_names(self, bundle: NameBundle, parent: str = None) -> None:
         """
         Ensure one or more names are included in names dataframe and update
         taxa and synonyms dataframes as necessary
 
-        Parameters:
-        name_dict - list of dictionaries - each dictionary contains
-            values keyed by terms from name_headings
+        :param bundle: :py:class:`~coldp.NameBundle` object with set of associated taxon names
+        :param parent: ID for taxon record for which the accepted taxon in this bundle is to be added as a child
 
-        Behaviour:
-        Add names, taxon and synonyms to package and update bundle records
-        with id values
+        The supplied :py:class:`~coldp.NameBundle` object includes an accepted
+        name record (as a dictionary of COLDP name properties) and a list, which
+        may be empty, of synonym name records in the same format. :py:func:`~coldp.COLDP.add_names`
+        ensures that name records exist for all these names in the names dataframe,
+        that a taxon record exists for the accepted taxon name, and that synonym
+        records exist for this taxon record for all supplied synonyms.
+
+        Depending on the options supplied for the :py:class:`~coldp.COLDP` object,
+        additional synonyms may be created to represent subspecies-rank versions
+        of infrasubspecific trinomials and subgenus-free versions of combinations
+        including a subgenus name.
+
+        If a matching name already exists in the COLDP instance, no new name will
+        normally be added. Instead, the name record in the bundle will be updated
+        with the ID (and basionymID where applicable) from the existing name. This
+        allows for additional synonyms to be added to an existing taxon. The
+        behaviour can be over-ridden with the :paramref:`~coldp.COLDP.allow_repeated_binomials`
+        option, in which case any number of matching names can be added.
+
+        If the :paramref:`~coldp.COLDP.insert_species_for_trinomials` option is
+        set, a new species will be created if required before adding the
+        trinomial as its child. In this case the bundle will contain the id
+        for the species taxon as a species_taxon_id property.
+
+        Name records in the bundle are all updated with existing or new IDs and
+        basionymIDs, which are inferred automatically for zoological names by
+        associating combinations with and without parentheses around the
+        authorship.
+
+        Upon completion, the bundle also contains an accepted_taxon_id property
+        which includes the string ID for the taxon.
+
+        If :paramref:`~coldp.COLDP.add_names.parent` is None, the new taxon record
+        is created without a parent, i.e. becomes a root node in the classification.
         """
 
-        # Tag any names that are already known with the appropriate id
+        # Handle any options and get species if exists already.
         self.prepare_bundle(bundle)
 
         # Ensure all names have IDs
         bundle.accepted = self.identify_name(bundle.accepted)
         if bundle.species:
             bundle.species = self.identify_name(bundle.species)
         if bundle.species_synonym:
@@ -1133,53 +1349,108 @@
 
         if (
             "status" not in bundle.accepted
             or bundle.accepted["status"] == "established"
             or self.create_taxa_for_not_established
         ):
             if bundle.species:
-                taxon = self.add_taxon(bundle.species, parent)
+                taxon = self.insert_taxon(bundle.species, parent)
                 parent = taxon["ID"]
                 bundle.species_taxon_id = parent
                 if bundle.species_synonym:
-                    self.add_synonym(parent, bundle.species_synonym["ID"])
+                    self.insert_synonym(parent, bundle.species_synonym["ID"])
 
-            taxon = self.add_taxon(bundle.accepted, parent, bundle.incertae_sedis)
+            taxon = self.insert_taxon(bundle.accepted, parent, bundle.incertae_sedis)
             bundle.accepted_taxon_id = taxon["ID"]
             for i in range(len(bundle.synonyms)):
-                self.add_synonym(bundle.accepted_taxon_id, bundle.synonyms[i]["ID"])
+                self.insert_synonym(bundle.accepted_taxon_id, bundle.synonyms[i]["ID"])
 
         return
 
-    def add_name_relation(self, name_relation):
+    def add_name_relation(self, name_relation: dict[str:str]) -> dict[str:str]:
+        """
+        Add COLDP NameRelation record to COLDP instance
+
+        :param name_relation: COLDP NameRelation record represented as dictionary of properties
+        :return: NameRelation record returned unchanged
+
+        The nameID and relatedNameID values must match the ID values for existing
+        name records.
+
+        This method returns the record unchanged (for consistency with other
+        add records which may alter the provided record).
+        """
+
         if self.name_relations is None:
             logging.info("Adding name_relation table")
             self.name_relations = pd.DataFrame(columns=name_relation_headings)
 
         if (
             "nameID" not in name_relation
             or name_relation["nameID"] not in self.names["ID"].values
         ):
-            self.issue("Type material must be associated with a valid name ID")
+            self.issue("Name relation must be associated with a valid name ID")
             return None
 
         if (
             "relatedNameID" not in name_relation
             or name_relation["relatedNameID"] not in self.names["ID"].values
         ):
-            self.issue("Type material must be associated with a valid related name ID")
+            self.issue("Name relation must be associated with a valid related name ID")
             return None
 
         self.name_relations = pd.concat(
             (self.name_relations, pd.DataFrame.from_records([name_relation])),
             ignore_index=True,
         )
         return name_relation
 
-    def add_type_material(self, type_material):
+    def add_synonym(self, synonym: dict[str:str]) -> dict[str:str]:
+        """
+        Add COLDP Synonym record to COLDP instance
+
+        :param synonym: COLDP Synonym record represented as dictionary of properties
+        :return: Synonym record returned unchanged
+
+        The taxonID value must match the ID value for an existing taxon record
+        and the nameID value must match the ID value for an existing name record.
+
+        This method returns the record unchanged (for consistency with other
+        add records which may alter the provided record).
+        """
+        if self.synonyms is None:
+            logging.info("Adding synonym table")
+            self.synonyms = pd.DataFrame(columns=synonym_headings)
+
+        if "taxonID" not in synonym or synonym["taxonID"] not in self.taxa["ID"].values:
+            self.issue("Synonym must be associated with a valid taxon ID")
+            return None
+
+        if "nameID" not in synonym or synonym["nameID"] not in self.names["ID"].values:
+            self.issue("Synonym must be associated with a valid name ID")
+            return None
+
+        self.synonyms = pd.concat(
+            (self.synonyms, pd.DataFrame.from_records([synonym])),
+            ignore_index=True,
+        )
+        return synonym
+
+    def add_type_material(self, type_material: dict[str:str]) -> dict[str:str]:
+        """
+        Add COLDP TypeMaterial record to COLDP instance
+
+        :param type_material: COLDP TypeMaterial record represented as dictionary of properties
+        :return: TypeMaterial record returned unchanged
+
+        The nameID value must match the ID value for an existing name record.
+
+        This method returns the record unchanged (for consistency with other
+        add records which may alter the provided record).
+        """
         if self.type_materials is None:
             logging.info("Adding type_material table")
             self.type_materials = pd.DataFrame(columns=type_material_headings)
 
         if (
             "nameID" not in type_material
             or type_material["nameID"] not in self.names["ID"].values
@@ -1189,15 +1460,26 @@
 
         self.type_materials = pd.concat(
             (self.type_materials, pd.DataFrame.from_records([type_material])),
             ignore_index=True,
         )
         return type_material
 
-    def add_distribution(self, distribution):
+    def add_distribution(self, distribution: dict[str:str]) -> dict[str:str]:
+        """
+        Add COLDP Distribution record to COLDP instance
+
+        :param distribution: COLDP Distribution record represented as dictionary of properties
+        :return: Distribution record returned unchanged
+
+        The taxonID value must match the ID value for an existing taxon record.
+
+        This method returns the record unchanged (for consistency with other
+        add records which may alter the provided record).
+        """
         if self.distributions is None:
             logging.info("Adding distribution table")
             self.distributions = pd.DataFrame(columns=distribution_headings)
 
         if (
             "taxonID" not in distribution
             or distribution["taxonID"] not in self.taxa["ID"].values
@@ -1209,15 +1491,26 @@
 
         self.distributions = pd.concat(
             (self.distributions, pd.DataFrame.from_records([distribution])),
             ignore_index=True,
         )
         return distribution
 
-    def add_species_interaction(self, interaction):
+    def add_species_interaction(self, interaction: dict[str:str]) -> dict[str:str]:
+        """
+        Add COLDP SpeciesInteraction record to COLDP instance
+
+        :param interaction: COLDP SpeciesInteraction record represented as dictionary of properties
+        :return: SpeciesInteraction record returned unchanged
+
+        The taxonID value must match the ID value for an existing taxon record.
+
+        This method returns the record unchanged (for consistency with other
+        add records which may alter the provided record).
+        """
         if self.species_interactions is None:
             logging.info("Adding species interaction table")
             self.species_interactions = pd.DataFrame(
                 columns=species_interaction_headings
             )
 
         if (
@@ -1231,15 +1524,23 @@
             (self.species_interactions, pd.DataFrame.from_records([interaction])),
             ignore_index=True,
         )
         return interaction
 
     def prepare_bundle(self, bundle):
         """
-        Add extra names
+        Add extra names to :py:class:`~coldp.NameBundle` if required based on current options
+
+        :param bundle: NameBundle to be processed
+
+        If :paramref:`~coldp.COLDP.insert_species_for_trinomials` is True, ensure that the implied binomial exists for any new trinomials.
+
+        If :paramref:`~coldp.COLDP.create_subspecies_for_infrasubspecifics` is True, add a subspecies-rank synonym to the bundle for each infrasubspecific name.
+
+        If :paramref:`~coldp.COLDP.create_synonyms_without_subgenus` is True, add a subgenus-free synonym to the bundle for each name containing a subgenus.
         """
 
         # Identify the species that should exist to allow the accepted name to be grafted. E.g. Aus bus cus --> Aus bus
         if self.species_from_trinomials:
             if bundle.accepted["infraspecificEpithet"]:
                 bundle.species = bundle.derive_name(
                     bundle.accepted,
@@ -1295,28 +1596,76 @@
                     )
 
             if bundle.species and bundle.species["infragenericEpithet"]:
                 bundle.species_synonym = bundle.derive_name(
                     bundle.species, {"infragenericEpithet": ""}
                 )
 
-    def add_synonym(self, taxon_id, name_id):
+    def insert_synonym(self, taxon_id: str, name_id: str) -> None:
+        """
+        Add basic COLDP Synonym record to COLDP instance
+
+        :param taxon_id: String ID for taxon for which synonym is being registered
+        :param name_id: String ID for name which is being registered as a synonym
+
+        Ensures that a synonym record exists in the COLDP instance for the given taxon and name.
+        """
         match = self.synonyms[
             (self.synonyms["taxonID"] == taxon_id)
             & (self.synonyms["nameID"] == name_id)
         ]
         if len(match) > 0:
             return match.iloc[0]
         synonym_row = {"taxonID": taxon_id, "nameID": name_id, "status": "synonym"}
         self.synonyms = pd.concat(
             (self.synonyms, pd.DataFrame.from_records([synonym_row])), ignore_index=True
         )
         return
 
-    def add_taxon(self, name, parent, incertae_sedis=False):
+    def validate_record(self, record_type: str, record: dict[str:str]) -> bool:
+        """
+        Verify whether all ID values used as forign keys in :paramref:`~coldp.COLDP.validate_record.record` correspond with existing records in the relevant tables
+
+        :param record_type: Name for the data class to which this record should below
+        :param record: Dictionary of COLDP properties for the record
+
+        Uses the :py:data:`~coldp.id_mappings` dictionary to identify which properties
+        should be foreign keys. If these are present in the current record, check
+        that the supplied value is indeed an ID from the relevant table.
+        """
+
+        valid = True
+
+        for table in id_mappings:
+            print(f"Table: {table}")
+            if record_type in id_mappings[table]:
+                print(f"Record type {record_type}")
+                df = self.table_by_name(table)
+                for property in id_mappings[table][record_type]:
+                    print(f"Checking property: {property} ")
+                    if property in record:
+                        print(f"Value: {record[property]}")
+                        if df is not None:
+                            print(df["ID"].values)
+                    if (
+                        property in record
+                        and record[property]
+                        and (df is None or record[property] not in df["ID"].values)
+                    ):
+                        print(f"BAD")
+                        self.issue(
+                            f"Record {record_type} {record} includes unrecognised {property}: {record[property]}"
+                        )
+                        valid = False
+
+        return valid
+
+    def insert_taxon(self, name, parent, incertae_sedis=False):
+
+        print(f"Name: {name}\nParent: {parent}")
         match = self.taxa[self.taxa["nameID"] == name["ID"]]
         if len(match) > 0:
             if len(match) > 1:
                 self.issue("More than one taxon matches name " + name["ID"])
             match = match.iloc[0]
             if match["uninomial"] != name["uninomial"]:
                 self.issue(
@@ -1336,15 +1685,20 @@
                     "Species mismatch ("
                     + match["species"]
                     + " vs "
                     + name["scientificName"]
                     + ") for taxon id "
                     + match["ID"]
                 )
-            if match["parentID"] and parent and match["parentID"] != parent:
+            if (
+                "parentID" in match
+                and match["parentID"]
+                and parent
+                and match["parentID"] != parent
+            ):
                 match = self.taxa[self.taxa["ID"] == match["parentID"]].iloc[0]
                 parentA = self.names[self.names["ID"] == match["nameID"]].iloc[0]
                 match = self.taxa[self.taxa["ID"] == parent].iloc[0]
                 parentB = self.names[self.names["ID"] == match["nameID"]].iloc[0]
                 self.issue(
                     "Parent mismatch for "
                     + name["rank"]
@@ -1412,40 +1766,76 @@
                     taxon_row["remarks"] = "Incertae sedis"
             self.taxa = pd.concat(
                 (self.taxa, pd.DataFrame.from_records([taxon_row])), ignore_index=True
             )
 
             return taxon_row
 
-    def modify_taxon(self, taxon_id, properties):
+    def modify_taxon(self, taxon_id: str, properties: dict[str:str]) -> None:
+        """
+        Add or modify properties on a COLDP Taxon record
+
+        :param taxon_id: String ID for a Taxon record
+        :param properties: Dictionary of COLDP Taxon properties to be set for the identified record
+
+        If a taxon record exists with the given ID, set all properties in the dictionary.
+        """
+        if taxon_id not in self.taxa["ID"].values:
+            logging.error(f"Taxon ID {taxon_id} not recognised")
+            return
+
         self.taxa.loc[self.taxa["ID"] == taxon_id, list(properties.keys())] = list(
             properties.values()
         )
 
-    def modify_name(self, name_id, properties):
+    def modify_name(self, name_id: str, properties: dict[str:str]) -> None:
+        """
+        Add or modify properties on a COLDP Name record
+
+        :param taxon_id: String ID for a Name record
+        :param properties: Dictionary of COLDP Name properties to be set for the identified record
+
+        If a name record exists with the given ID, set all properties in the dictionary.
+        """
+        if name_id not in self.names["ID"].values:
+            logging.error(f"Name ID {name_id} not recognised")
+            return
+
         self.names.loc[self.names["ID"] == name_id, list(properties.keys())] = list(
             properties.values()
         )
 
-    def identify_name(self, name):
+    def identify_name(self, name: dict[str:str]) -> dict[str:str]:
+        """
+        Ensure COLDP Name record is present and return a copy containing the current ID and basionymID
+
+        :param name: Dictionary containing COLDP Name properties
+        :return: Currently stored version of the name record in question
+        """
         match = None
+
         if name["rank"] != "species" or not self.allow_repeated_binomials:
             match = self.find_name_record(name)
         if match is not None:
-            name["ID"] = match["ID"]
-            name["basionymID"] = match["basionymID"]
+            return match
         else:
             if "ID" not in name or not name["ID"]:
                 name["ID"] = str(len(self.names) + 1)
             self.names = pd.concat(
                 (self.names, pd.DataFrame.from_records([name])), ignore_index=True
             )
         return name
 
-    def same_basionym(self, a, b):
+    def same_basionym(self, a: dict[str:str], b: dict[str:str]) -> bool:
+        """
+        Validates whether two name records share the same basionym (i.e. are different combinations for the same original name)
+        :param a: Dictionary with parameters representing a COLDP Name record
+        :param b: Dictionary with parameters representing a COLDP Name record
+        :return: True if the parenthensis-free authorship and lowest-ranked epithets match, False otherwise.
+        """
         authorship_a = self.get_original_authorship(a["authorship"])
         authorship_b = self.get_original_authorship(b["authorship"])
         epithet_a = (
             a["infraspecificEpithet"]
             if a["infraspecificEpithet"]
             else a["specificEpithet"]
         )
@@ -1454,41 +1844,69 @@
             if b["infraspecificEpithet"]
             else b["specificEpithet"]
         )
         return authorship_a == authorship_b and self.remove_gender(
             epithet_a
         ) == self.remove_gender(epithet_b)
 
-    def remove_gender(self, epithet):
+    def remove_gender(self, epithet: str) -> str:
+        """
+        Return epithet stripped on all likely gender-specific endings
+
+        :param epithet: String zoological epithet
+        :return: Epithet stripped of any possible Greek or Latin gender endings
+
+        Removes "a", "us", "um", "is", "e", "os" or "on" as an ending.
+        """
         for suffix in ["a", "us", "um", "is", "e", "os", "on"]:
             if epithet.endswith(suffix):
                 return epithet[0 : len(epithet) - len(suffix)]
         return epithet
 
-    def get_original_authorship(self, authorship):
+    def get_original_authorship(self, authorship: str) -> str:
+        """
+        Return authorship string without enclosing parentheses
+
+        :param authorship: Authorship string
+        :return: Authorship stripped of enclosing parentheses
+
+        Relevant only for zoological names
+        """
         if authorship.startswith("(") and ")" in authorship:
             return authorship[1 : authorship.index(")")]
         return authorship
 
     def epithet_and_authorship_match(self, name, epithet, authorship):
         epithet = self.remove_gender(epithet)
         return name["authorship"] == authorship and (
             self.remove_gender(name["infraspecificEpithet"]) == epithet
             or (
                 self.remove_gender(name["specificEpithet"]) == epithet
                 and not name["infraspecificEpithet"]
             )
         )
 
-    def set_basionymid(self, name, basionymid):
-        self.names.loc[self.names["ID"] == name["ID"], ["basionymID"]] = basionymid
-        name["basionymID"] = basionymid
+    def set_basionymid(self, name: dict[str:str], basionymid: str) -> dict[str:str]:
+        """
+        Set basionymID on Name record in names DataFrame
+
+        :param name: Name record as dictionary of COLDP properties
+        :param basionymid: String ID of associated basionyn record
+
+        """
+        if basionymid not in self.names["ID"].values:
+            logging.error(f"Basionym ID {basionymid} not recognised")
+        else:
+            self.names.loc[self.names["ID"] == name["ID"], ["basionymID"]] = basionymid
+            name["basionymID"] = basionymid
         return name
 
-    def fix_basionymid(self, name, synonyms):
+    def fix_basionymid(
+        self, name: dict[str:str], synonyms: list[dict[str:str]]
+    ) -> dict[str:str]:
         original_authorship = self.get_original_authorship(name["authorship"])
         if name["authorship"] != original_authorship:
             epithet = (
                 name["infraspecificEpithet"]
                 if name["infraspecificEpithet"]
                 else name["specificEpithet"]
             )
@@ -1498,18 +1916,31 @@
                 ):
                     name = self.set_basionymid(name, synonyms[i]["basionymID"])
                     break
         else:
             name = self.set_basionymid(name, name["ID"])
         return name
 
-    def find_name_record(self, name):
-        return self.find_name(name["scientificName"], name["authorship"], name["rank"])
+    def find_name_record(self, name: dict[str:str]) -> dict[str:str]:
+        """
+        Return record from names DataFrame matching key fields in supplied record
+
+        :param name: Dictionary containing Name properties
+        :return: Dictionary containing matching record if found
+
+        Locates any existing record in the names DataFrame that matches the
+        supplied scientificName, authorship and rank and returns it as a
+        COLDP Name properties dictionary, or None if no match is found.
+        """
+        record = self.find_name(
+            name["scientificName"], name["authorship"], name["rank"]
+        )
+        return None if record is None else record.to_dict()
 
-    def get_name(self, id):
+    def get_name(self, id: str):
         match = self.names[self.names["ID"] == id]
         if len(match) == 0:
             return None
         if len(match) > 1:
             logging.warn(f"Multiple matches for name ID: {id}")
         return match.to_dict("records")[0]
 
@@ -1621,37 +2052,75 @@
         match = self.taxa[self.taxa["parentID"] == taxonID]
         if match.empty:
             return None
         if to_dict:
             return match.to_dict("records")
         return match
 
-    def get_text_tree(self, taxonID, indent=""):
+    def get_text_tree(
+        self,
+        taxonID: str,
+        indent: str = "  ",
+        initial_prefix: str = "",
+        synonym_prefix=" = ",
+    ) -> str:
+        """
+        Generate formatted text tree for specified taxon and its descendents
+
+        :param taxonID: String ID for taxon to be formatted
+        :param indent: Indent string to be added one or more times before each nested row, defaults to two spaces
+        :param initial_prefix: Optional prefix string for all rows (preceeds indentation), defaults to empty string
+        :param synonym_prefix: Prefix to appear before synonymised names, defaults to an equal sign with spaces on either side
+        :return: Multiline string representation of taxonomic hierarchy
+
+        The tree view shows the name, authorship and rank for the selected taxon.
+        Synonyms follow, one to a row at the same indent level but preceded by a
+        space and an asterisk. Then each child follows, indented two more spaces per level,
+        with its own synonyms and children following.
+        """
         taxon = self.get_taxon(taxonID)
         if taxon is None:
             return ""
         name = self.get_name(taxon["nameID"])
         if name is None:
             logging.error(f"No name for taxon {taxonID}")
-        tree = f"{indent}{name['scientificName']} {name['authorship']} [{name['rank']}]"
+        tree = f"{initial_prefix}{name['scientificName']} {name['authorship']} [{name['rank']}]"
         synonyms = self.get_synonyms(taxonID)
         if synonyms is not None:
             for synonym in synonyms["nameID"]:
                 junior = self.get_name(synonym)
                 if junior is None:
                     logging.error(f"Could not find name {synonym} for synonym")
                 else:
-                    tree += f"\n {indent}* {junior['scientificName']} {junior['authorship']} [{junior['rank']}]"
+                    tree += f"\n{initial_prefix} = {junior['scientificName']} {junior['authorship']} [{junior['rank']}]"
         children = self.get_children(taxonID)
         if children is not None:
             for child in children["ID"]:
-                tree += "\n" + self.get_text_tree(child, indent + "  ")
+                tree += "\n" + self.get_text_tree(
+                    child, indent, initial_prefix + indent
+                )
         return tree
 
-    def construct_species_rank_name(self, g, sg, s, ss, marker):
+    def construct_species_rank_name(
+        self, g: str, sg: str, s: str, ss: str, marker: str
+    ) -> str:
+        """
+        Consistently construct a species or infraspecific name from the included epithets and optional rank marker
+
+        :param g: Genus name
+        :param sg: Subgenus name
+        :param s: Specific epithet
+        :param ss: Infraspecific epithet
+        :param marker: Rank marker (e.g. "var.") or rank name ("variety")
+        :return: Complete scientific name string (no italics or authorship)
+
+        Convenience method for composing a scientific name with option subgenus,
+        infraspecific epithet and rank marker. A variety of markers are handled
+        and mapped to one of "var.", "subvar.", "f." and "ab.".
+        """
         if not g:
             self.issue(
                 "Missing genus for species rank name " + str([g, sg, s, ss, marker])
             )
             g = "?"
         if not s:
             self.issue(
@@ -1699,15 +2168,32 @@
         if sg:
             if not sg.startswith("("):
                 sg = "(" + sg + ")"
             sn.insert(1, sg)
 
         return " ".join(sn), rank
 
-    def construct_authorship(self, a, y, is_basionym):
+    def construct_authorship(self, a: str, y: str, is_basionym: bool) -> str:
+        """
+        Consistently construct a scientific name authorship from the included author names and year with parentheses where required
+
+        :param a: Author string
+        :param y: Publication year as string
+        :param is_basionym: Boolean to indicate whether this is the original combination (basionym) or a subsequent combination that requires parentheses
+        :return: Tuple including 1) formatted authorship string and 2) publication year as a separate string
+
+        Convenience method for composing an authorship string. Includes parentheses if :paramref:`~coldp.COLDP.construct_authorship.is_basionym` is True.
+
+        If the :paramref:`~coldp.COLDP.construct_authorship.year` includes more
+        than one part (e.g. "1832 [1831-1838]"), the first part ("1832") is used
+        for the year in the authorship string and the second part ("[1831-1838]")
+        is returned as the publication year. Otherwise, the same string is used
+        in both cases.
+        """
+
         if not a:
             self.issue("No author supplied")
             a = ""
         if not y:
             self.issue("No year supplied")
             y = ""
 
@@ -1728,21 +2214,44 @@
             combined = ""
 
         if not is_basionym and combined:
             combined = "(" + combined + ")"
 
         return combined, y, year_publication
 
-    def is_species_group(self, name):
+    def is_species_group(self, name: dict[str:str]) -> bool:
+        """
+        Check whether name is in the species group (species or lower rank)
+
+        :param name: Dictionary representing a COLDP Name record
+        :return: True if the name is in the species group, False otherwise
+
+        Simply checks if the name includes a specificEpithet value. Any name
+        passed to this method should include atomic name components and not
+        just a scientificName.
+        """
         if name["specificEpithet"]:
             return True
         return False
 
-    def is_infrasubspecific(self, name):
-        return "rank" in name and name["rank"] in ["variety", "form", "aberration"]
+    def is_infrasubspecific(self, name: dict[str:str]) -> bool:
+        """
+        Check whether name is in for a rank below the subspecies
+
+        :param name: Dictionary representing a COLDP Name record
+        :return: True if the name is infraspecific
+
+        Simply checks if the supplied rank is one of those below the subspecies.
+        """
+        return "rank" in name and name["rank"] in [
+            "variety",
+            "subvariety",
+            "form",
+            "aberration",
+        ]
 
     def save(self, destination=None, name=None):
         """
         Write dataframes as COLDP CSV files
 
         Behaviour:
         Ensure that <folder>/<name>/ exists and write all dataframes as CSV.
@@ -1777,49 +2286,51 @@
                 value.dropna(how="all", axis=1, inplace=True)
                 value.replace(np.nan, "", inplace=True)
                 file_name = os.path.join(coldp_folder, item + ".csv")
                 value.to_csv(file_name, index=False)
         logging.info("COLDP saved to " + coldp_folder)
         return
 
-    def issue(self, message, **record):
+    def issue(self, message):
         if self.issues is None:
             self.issues = pd.DataFrame(columns=issues_headings)
 
         context = self.context if self.context else ""
-        record = {"issue": message, "context": context}
+        issue_record = {"issue": message, "context": context}
 
         if self.issues_to_stdout:
             logging.error(context + ": " + message)
 
         self.issues = pd.concat(
-            (self.issues, pd.DataFrame.from_records([record])), ignore_index=True
+            (self.issues, pd.DataFrame.from_records([issue_record])), ignore_index=True
         )
 
 
 if __name__ == "__main__":
     logging.basicConfig(filename="COLDP.log", level=logging.DEBUG)
 
+    test_folder = "../../test"
+
     default_taxon = {
         "kingdom": "Animalia",
         "phylum": "Arthropoda",
         "class": "Insecta",
         "order": "Lepidoptera",
-        "scrutinizer": "Geometridae Working Group",
+        "scrutinizer": "A Taxonomist",
         "provisional": "false",
         "extinct": "false",
         "lifezone": "terrestrial",
         "temporalRangeEnd": "Holocene",
     }
 
-    for f in os.listdir("./test/output/"):
-        shutil.rmtree(os.path.join("./test/output/", f))
+    for f in os.listdir(os.path.join(test_folder, "output")):
+        shutil.rmtree(os.path.join(test_folder, "output", f))
 
     coldp = COLDP(
-        "./test/output/",
+        os.path.join(test_folder, "output"),
         "fake",
         default_taxon_record=default_taxon,
         insert_species_for_trinomials=True,
         create_subspecies_for_infrasubspecifics=True,
         create_synonyms_without_subgenus=True,
         issues_to_stdout=True,
     )
@@ -1905,25 +2416,16 @@
     coldp.add_names(nb, None)
 
     coldp.modify_taxon(nb.accepted_taxon_id, {"extinct": "true", "lifezone": "marine"})
 
     coldp.save()
 
     coldp = COLDP(
+        os.path.join(test_folder, "input"),
         "./test/input",
         "Tonzidae",
         basionyms_from_synonyms=True,
         classification_from_parents=True,
         issues_to_stdout=True,
     )
 
-    coldp.save("./test/output")
-
-    coldp = COLDP(
-        "../../Dropbox/NetBeans Projects/Tineidae",
-        "NHM_Tineidae_2011-11-21",
-        basionyms_from_synonyms=True,
-        classification_from_parents=True,
-        issues_to_stdout=True,
-    )
-
-    coldp.save("./test/output")
+    coldp.save(os.path.join(test_folder, "output"))
```

### Comparing `coldp-2024.0.2/src/coldp/coldp_distribution.py` & `coldp-2024.5.2/src/coldp/coldp_distribution.py`

 * *Files identical despite different names*

### Comparing `coldp-2024.0.2/test/input/Tonzidae/NameUsage.tsv` & `coldp-2024.5.2/test/input/Tonzidae/NameUsage.tsv`

 * *Files identical despite different names*

### Comparing `coldp-2024.0.2/test/input/Tonzidae/Reference.tsv` & `coldp-2024.5.2/test/input/Tonzidae/Reference.tsv`

 * *Files identical despite different names*

### Comparing `coldp-2024.0.2/test/input/Tonzidae/logo.png` & `coldp-2024.5.2/test/input/Tonzidae/logo.png`

 * *Files identical despite different names*

### Comparing `coldp-2024.0.2/test/input/Tonzidae/metadata.yaml` & `coldp-2024.5.2/test/input/Tonzidae/metadata.yaml`

 * *Files identical despite different names*

### Comparing `coldp-2024.0.2/venv/Lib/site-packages/backports.tarfile-1.1.1.dist-info/LICENSE` & `coldp-2024.5.2/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+MIT License
+
+Copyright (c) [2024] [Donald Hobern]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `coldp-2024.0.2/README.md` & `coldp-2024.5.2/README.md`

 * *Files identical despite different names*

### Comparing `coldp-2024.0.2/pyproject.toml` & `coldp-2024.5.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "coldp"
-version = "2024.0.2"
+version = "2024.5.2"
 authors = [
   { name="Donald Hobern", email="dhobern@gmail.com" },
 ]
 description = "Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format"
 keywords = ["Catalogue of Life", "COLDP", "taxonomic checklist"]
 readme = "README.md"
 requires-python = ">=3.8"
@@ -24,9 +24,14 @@
 ]
 license = {file = "LICENSE"}
 
 [project.urls]
 Homepage = "https://github.com/dhobern/py-coldp"
 Issues = "https://github.com/dhobern/py-coldp/issues"
 
+[project.optional-dependencies]
+doc = [
+    "sphinx", "sphinx-paramlinks"
+]
+
 [tool.hatch.build.targets.wheel]
 packages = ["src/coldp"]
```

### Comparing `coldp-2024.0.2/PKG-INFO` & `coldp-2024.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coldp
-Version: 2024.0.2
+Version: 2024.5.2
 Summary: Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format
 Project-URL: Homepage, https://github.com/dhobern/py-coldp
 Project-URL: Issues, https://github.com/dhobern/py-coldp/issues
 Author-email: Donald Hobern <dhobern@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Donald Hobern]
@@ -31,14 +31,17 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: numpy
 Requires-Dist: pandas
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == 'doc'
+Requires-Dist: sphinx-paramlinks; extra == 'doc'
 Description-Content-Type: text/markdown
 
 # py-coldp
  Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format
 
 # Overview
 py-coldp is a Python package to facilitate creation, manipulation, editing and serialisation of taxonomic checklists in the [Catalogue of Life Data Package](https://github.com/CatalogueOfLife/coldp ) format.
```

