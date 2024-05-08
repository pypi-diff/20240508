# Comparing `tmp/sparkx-1.2.0.tar.gz` & `tmp/sparkx-1.2.1.tar.gz`

## Comparing `sparkx-1.2.0.tar` & `sparkx-1.2.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 sparkx-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sparkx-1.2.0/CONTRIBUTORS.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sparkx-1.2.0/INSTALL.md
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 sparkx-1.2.0/requirements.txt
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sparkx-1.2.0/setup.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 sparkx-1.2.0/.github/workflows/GitHub_tests.yml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 sparkx-1.2.0/.github/workflows/PyPI_release.yml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 sparkx-1.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/make.bat
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/conf.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/credits.md
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/index.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/install.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/license.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/_static/.placeholder
--rw-r--r--   0        0        0   264764 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/_static/SPARKX_logo.png
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/index.rst
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/CentralityClasses/index.rst
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/EventCharacteristics/index.rst
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/Histogram/index.rst
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/JetAnalysis/index.rst
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/Jetscape/index.rst
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/Lattice3D/index.rst
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/Oscar/index.rst
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/Particle/index.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/flow/index.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/flow/EventPlaneFlow/index.rst
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/flow/GenerateFlow/index.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/flow/LeeYangZeroFlow/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/flow/PCAFlow/index.rst
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/flow/QCumulantFlow/index.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/flow/ReactionPlaneFlow/index.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/classes/flow/ScalarProductFlow/index.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/utilities/index.rst
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sparkx-1.2.0/docs/source/utilities/functions/index.rst
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/CentralityClasses.py
--rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/EventCharacteristics.py
--rw-r--r--   0        0        0    25336 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/Filter.py
--rwxr-xr-x   0        0        0    27406 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/Histogram.py
--rwxr-xr-x   0        0        0    18146 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/JetAnalysis.py
--rw-r--r--   0        0        0    33353 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/Jetscape.py
--rw-r--r--   0        0        0    45649 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/Lattice3D.py
--rw-r--r--   0        0        0    42230 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/Oscar.py
--rwxr-xr-x   0        0        0    31312 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/Particle.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/Utilities.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/__init__.py
--rw-r--r--   0        0        0    17070 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/flow/EventPlaneFlow.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/flow/FlowInterface.py
--rw-r--r--   0        0        0    41222 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/flow/GenerateFlow.py
--rw-r--r--   0        0        0    22510 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/flow/LeeYangZeroFlow.py
--rw-r--r--   0        0        0    19755 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/flow/PCAFlow.py
--rw-r--r--   0        0        0    30610 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/flow/QCumulantFlow.py
--rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/flow/ReactionPlaneFlow.py
--rw-r--r--   0        0        0    14778 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/flow/ScalarProductFlow.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 sparkx-1.2.0/src/sparkx/flow/__init__.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_CentralityClasses.py
--rw-r--r--   0        0        0    20866 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_EventCharacteristics.py
--rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_Filter.py
--rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_Flow.py
--rw-r--r--   0        0        0    10394 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_Histogram.py
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_JetAnalysis.py
--rw-r--r--   0        0        0    14792 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_Jetscape.py
--rw-r--r--   0        0        0    19482 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_Lattice3D.py
--rw-r--r--   0        0        0    26323 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_Oscar.py
--rw-r--r--   0        0        0    17936 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_Particle.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_Utilities.py
--rw-r--r--   0        0        0    15782 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_files/particle_lists.oscar
--rw-r--r--   0        0        0    20755 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_files/particle_lists_extended.oscar
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_files/particle_lists_extended_old.oscar
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_files/test_jet_finding.csv
--rwxr-xr-x   0        0        0     9551 2020-02-02 00:00:00.000000 sparkx-1.2.0/tests/test_files/test_jetscape.dat
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparkx-1.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sparkx-1.2.0/LICENSE
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 sparkx-1.2.0/README.md
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sparkx-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 sparkx-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 sparkx-1.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 sparkx-1.2.1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sparkx-1.2.1/INSTALL.md
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 sparkx-1.2.1/requirements.txt
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 sparkx-1.2.1/setup.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 sparkx-1.2.1/.github/workflows/GitHub_tests.yml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 sparkx-1.2.1/.github/workflows/PyPI_release.yml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 sparkx-1.2.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/credits.md
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/install.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/license.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/_static/.placeholder
+-rw-r--r--   0        0        0   264764 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/_static/SPARKX_logo.png
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/index.rst
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/CentralityClasses/index.rst
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/EventCharacteristics/index.rst
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/Histogram/index.rst
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/JetAnalysis/index.rst
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/Jetscape/index.rst
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/Lattice3D/index.rst
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/Oscar/index.rst
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/Particle/index.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/flow/index.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/flow/EventPlaneFlow/index.rst
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/flow/GenerateFlow/index.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/flow/LeeYangZeroFlow/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/flow/PCAFlow/index.rst
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/flow/QCumulantFlow/index.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/flow/ReactionPlaneFlow/index.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/classes/flow/ScalarProductFlow/index.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/utilities/index.rst
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sparkx-1.2.1/docs/source/utilities/functions/index.rst
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/CentralityClasses.py
+-rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/EventCharacteristics.py
+-rw-r--r--   0        0        0    25336 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/Filter.py
+-rwxr-xr-x   0        0        0    27406 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/Histogram.py
+-rwxr-xr-x   0        0        0    18146 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/JetAnalysis.py
+-rw-r--r--   0        0        0    33353 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/Jetscape.py
+-rw-r--r--   0        0        0    45649 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/Lattice3D.py
+-rw-r--r--   0        0        0    42230 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/Oscar.py
+-rwxr-xr-x   0        0        0    32115 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/Particle.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/Utilities.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/__init__.py
+-rw-r--r--   0        0        0    17070 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/flow/EventPlaneFlow.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/flow/FlowInterface.py
+-rw-r--r--   0        0        0    41222 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/flow/GenerateFlow.py
+-rw-r--r--   0        0        0    22510 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/flow/LeeYangZeroFlow.py
+-rw-r--r--   0        0        0    19755 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/flow/PCAFlow.py
+-rw-r--r--   0        0        0    30610 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/flow/QCumulantFlow.py
+-rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/flow/ReactionPlaneFlow.py
+-rw-r--r--   0        0        0    14778 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/flow/ScalarProductFlow.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 sparkx-1.2.1/src/sparkx/flow/__init__.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_CentralityClasses.py
+-rw-r--r--   0        0        0    20866 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_EventCharacteristics.py
+-rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_Filter.py
+-rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_Flow.py
+-rw-r--r--   0        0        0    10394 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_Histogram.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_JetAnalysis.py
+-rw-r--r--   0        0        0    15042 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_Jetscape.py
+-rw-r--r--   0        0        0    19482 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_Lattice3D.py
+-rw-r--r--   0        0        0    26323 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_Oscar.py
+-rw-r--r--   0        0        0    18495 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_Particle.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_Utilities.py
+-rw-r--r--   0        0        0    15782 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_files/particle_lists.oscar
+-rw-r--r--   0        0        0    20755 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_files/particle_lists_extended.oscar
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_files/particle_lists_extended_old.oscar
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_files/test_jet_finding.csv
+-rwxr-xr-x   0        0        0     9551 2020-02-02 00:00:00.000000 sparkx-1.2.1/tests/test_files/test_jetscape.dat
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparkx-1.2.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sparkx-1.2.1/LICENSE
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 sparkx-1.2.1/README.md
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 sparkx-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    42524 2020-02-02 00:00:00.000000 sparkx-1.2.1/PKG-INFO
```

### Comparing `sparkx-1.2.0/CHANGELOG.md` & `sparkx-1.2.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,22 @@
 * `Added` for new features;
 * `Changed` for changes in existing functionality;
 * `Fixed` for any bug fixes;
 * `Removed` for now removed features.
 
 A `Deprecated` section could be added if needed for soon-to-be removed features.
 
+## v1.2.1-Newton
+Date: 2024-05-08
+
+### Fixed
+* Jetscape: Fix for Jetscape charged particle filtering
+
+[Link to diff from previous version](https://github.com/smash-transport/sparkx/compare/v1.2.0...v1.2.1)
+
 ## v1.2.0-Newton
 Date: 2024-04-21
 
 ### Added
 
 * QCumulantFlow: Differential flow for two and four particle cumulants
 * Tests: Tests for Histogram, Utilities, CentralityClasses, Oscar, Jetscape, JetAnalysis, Flow, Lattice3D, Filter, EventCharacteristics
```

### Comparing `sparkx-1.2.0/setup.py` & `sparkx-1.2.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import find_packages, setup
 
 setup(
     name='sparkx',
-    packages=find_packages(),
+    packages=find_packages(where='src/sparkx'),
     package_dir={'': 'sparkx'},
     install_requires=[
         "particle==0.23.0",
         "numpy>=1.23.5",
         "scipy>=1.10.1",
         "abc-property==1.0",
         "fastjet==3.4.1.3",
         "matplotlib>=3.7.1",
     ],
-    version='1.2.0',
+    version='1.2.1',
     description='Software Package for Analyzing Relativistic Kinematics in Collision eXperiments',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Niklas Götz, Hendrik Roch, Nils Sass',
-    author_email="goetz@fias.uni-frankfurt.de, roch@fias.uni-frankfurt.de, nsass@fias.uni-frankfurt.de",
+    author_email="goetz@itp.uni-frankfurt.de, hroch@wayne.edu, nsass@itp.uni-frankfurt.de",
     url="https://smash-transport.github.io/sparkx/",
     download_url="https://github.com/smash-transport/sparkx",
     license='MIT',
     include_package_data = True
 )
```

### Comparing `sparkx-1.2.0/.github/workflows/GitHub_tests.yml` & `sparkx-1.2.1/.github/workflows/GitHub_tests.yml`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/.github/workflows/PyPI_release.yml` & `sparkx-1.2.1/.github/workflows/PyPI_release.yml`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/.github/workflows/docs.yml` & `sparkx-1.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/Makefile` & `sparkx-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/make.bat` & `sparkx-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/source/conf.py` & `sparkx-1.2.1/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'sparkx'
 copyright = '2024, SPARKX Collaboration'
 author = 'Hendrik Roch, Nils Sass, Niklas Götz'
-release = '1.2.0'
+release = '1.2.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autosummary',
     'sphinx.ext.autodoc',
```

### Comparing `sparkx-1.2.0/docs/source/index.rst` & `sparkx-1.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/source/_static/SPARKX_logo.png` & `sparkx-1.2.1/docs/source/_static/SPARKX_logo.png`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/source/_static/favicon.ico` & `sparkx-1.2.1/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/source/classes/Histogram/index.rst` & `sparkx-1.2.1/docs/source/classes/Histogram/index.rst`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/source/classes/Jetscape/index.rst` & `sparkx-1.2.1/docs/source/classes/Jetscape/index.rst`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/source/classes/Lattice3D/index.rst` & `sparkx-1.2.1/docs/source/classes/Lattice3D/index.rst`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/source/classes/Oscar/index.rst` & `sparkx-1.2.1/docs/source/classes/Oscar/index.rst`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/source/classes/Particle/index.rst` & `sparkx-1.2.1/docs/source/classes/Particle/index.rst`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/docs/source/classes/flow/GenerateFlow/index.rst` & `sparkx-1.2.1/docs/source/classes/flow/GenerateFlow/index.rst`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/CentralityClasses.py` & `sparkx-1.2.1/src/sparkx/CentralityClasses.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/EventCharacteristics.py` & `sparkx-1.2.1/src/sparkx/EventCharacteristics.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/Filter.py` & `sparkx-1.2.1/src/sparkx/Filter.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/Histogram.py` & `sparkx-1.2.1/src/sparkx/Histogram.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/JetAnalysis.py` & `sparkx-1.2.1/src/sparkx/JetAnalysis.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/Jetscape.py` & `sparkx-1.2.1/src/sparkx/Jetscape.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/Lattice3D.py` & `sparkx-1.2.1/src/sparkx/Lattice3D.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/Oscar.py` & `sparkx-1.2.1/src/sparkx/Oscar.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/Particle.py` & `sparkx-1.2.1/src/sparkx/Particle.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,22 +210,22 @@
     of this array is float, therefore casting is required when int or bool values are 
     required.
     """
     __slots__ = ['data_'] 
     def __init__(self,input_format=None,particle_array=None):
         self.data_ = np.array(25*[np.nan],dtype=float)
         self.pdg_valid = False
-        
+
         if ((input_format is not None) and (particle_array is None)) or ((input_format is None) and (particle_array is not None)):
             raise ValueError("'input_format' or 'particle_array' not given")
 
         if (input_format is not None) and (particle_array is not None):
             self.__initialize_from_array(input_format,particle_array)
-            
-        
+
+
     def __initialize_from_array(self,input_format,particle_array):
         """
         Initialize instance attributes based on the provided input format and array.
 
         Parameters
         ----------
         input_format : str
@@ -364,24 +364,28 @@
                     if attribute in ["t_", "x_", "y_", "z_", "mass_", "E_", "px_", "py_", "pz_", "form_time_", "xsecfac_", "t_last_coll_", "weight_"]:
                         self.data_[index[0]] = float(particle_array[index[1]])
                     elif attribute in ["pdg_", "ID_", "ncoll_", "proc_id_origin_", "proc_type_origin_", "pdg_mother1_", "pdg_mother2_", "status_"]:
                         self.data_[index[0]] = int(particle_array[index[1]])
                     else:
                         self.data_[index[0]] = int(particle_array[index[1]])
 
+                # It is important for JETSCAPE particles to compute pdg_valid
+                # here because the compute_charge_from_pdg function depends on it. 
+                self.pdg_valid = PDGID(self.pdg).is_valid
+
                 if input_format == "JETSCAPE":
                     self.mass = self.compute_mass_from_energy_momentum()
                     self.charge = self.compute_charge_from_pdg()
+                    if self.pdg_valid == False and np.isnan(self.charge):
+                        warnings.warn('The PDG code ' + str(int(self.pdg)) + ' is not known by PDGID, charge could not be computed. Consider setting it by hand.')
             else:
                 raise ValueError("The input file is corrupted! " +\
                                  "A line with wrong number of columns "+str(len(particle_array))+" was found.")
         else:
             raise ValueError(f"Unsupported input format '{input_format}'")
-        
-        self.pdg_valid = PDGID(self.pdg).is_valid
 
         if(not self.pdg_valid):
              warnings.warn('The PDG code ' + str(int(self.pdg)) + ' is not valid. '+
                            'All properties extracted from the PDG are set to default values.')
 
     @property
     def t(self):
@@ -430,14 +434,15 @@
         """Get or set the z-position of the particle.
 
         Returns
         -------
         z : float
         """
         return self.data_[3]
+
     @z.setter
     def z(self,value):
         self.data_[3] = value
 
     @property
     def mass(self):
         """Get or set the mass of the particle.
@@ -757,15 +762,15 @@
         -------
         pdg_valid : bool
         """
         return bool(self.data_[10])
 
     @pdg_valid.setter
     def pdg_valid(self,value):
-        self.data_[10] = value
+        self.data_[10] = 1 if value else 0
 
     def print_particle(self):
         """Print the whole particle information as csv string.
 
         This function prints a header line with the different quantities.
         All particle quantities are then printed in the next line separated by
         a comma.
@@ -1110,15 +1115,15 @@
         if not self.pdg_valid:
             return np.nan
         if PDGID(self.pdg).has_charm or PDGID(self.pdg).has_bottom\
               or PDGID(self.pdg).has_top:
             return True
         else:
             return False
-     
+
     def spin(self):
         """
         Get the total spin :math:`J` of the particle.
 
         Returns
         -------
         float
@@ -1127,15 +1132,15 @@
         Notes
         -----
         If the PDG ID is not known by `PDGID`, then `np.nan` is returned.
         """
         if not self.pdg_valid:
             return np.nan
         return PDGID(self.pdg).J
-           
+
     def spin_degeneracy(self):
         """
         Get the number of all possible spin projections (:math:`2J + 1`).
 
         Returns
         -------
         int
@@ -1144,8 +1149,24 @@
         Notes
         -----
         If the PDG ID is not known by `PDGID`, then `np.nan` is returned.
         """
         if not self.pdg_valid:
             return np.nan
         return PDGID(self.pdg).j_spin
-    
+
+format1 = "JETSCAPE"
+array1 = np.array([1,211,27,4.36557,3.56147,0.562961,2.45727])
+
+p1 = Particle(input_format=format1,particle_array=array1)
+assert p1.ID == 1
+assert p1.pdg == 211
+assert p1.status == 27
+assert p1.E == 4.36557
+assert p1.px == 3.56147
+assert p1.py == 0.562961
+assert p1.pz == 2.45727
+assert np.isclose(p1.mass, 0.137956238, rtol=1e-6)
+assert p1.pdg_valid == True
+assert p1.charge == 1
+
+print(p1.compute_charge_from_pdg())
```

### Comparing `sparkx-1.2.0/src/sparkx/Utilities.py` & `sparkx-1.2.1/src/sparkx/Utilities.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/__init__.py` & `sparkx-1.2.1/src/sparkx/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/flow/EventPlaneFlow.py` & `sparkx-1.2.1/src/sparkx/flow/EventPlaneFlow.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/flow/FlowInterface.py` & `sparkx-1.2.1/src/sparkx/flow/FlowInterface.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/flow/GenerateFlow.py` & `sparkx-1.2.1/src/sparkx/flow/GenerateFlow.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/flow/LeeYangZeroFlow.py` & `sparkx-1.2.1/src/sparkx/flow/LeeYangZeroFlow.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/flow/PCAFlow.py` & `sparkx-1.2.1/src/sparkx/flow/PCAFlow.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/flow/QCumulantFlow.py` & `sparkx-1.2.1/src/sparkx/flow/QCumulantFlow.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/flow/ReactionPlaneFlow.py` & `sparkx-1.2.1/src/sparkx/flow/ReactionPlaneFlow.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/flow/ScalarProductFlow.py` & `sparkx-1.2.1/src/sparkx/flow/ScalarProductFlow.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/src/sparkx/flow/__init__.py` & `sparkx-1.2.1/src/sparkx/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_CentralityClasses.py` & `sparkx-1.2.1/tests/test_CentralityClasses.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_EventCharacteristics.py` & `sparkx-1.2.1/tests/test_EventCharacteristics.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_Filter.py` & `sparkx-1.2.1/tests/test_Filter.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_Flow.py` & `sparkx-1.2.1/tests/test_Flow.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_Histogram.py` & `sparkx-1.2.1/tests/test_Histogram.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_JetAnalysis.py` & `sparkx-1.2.1/tests/test_JetAnalysis.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_Jetscape.py` & `sparkx-1.2.1/tests/test_Jetscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,8 +374,12 @@
     jetscape.print_particle_lists_to_file(output_path)
     assert filecmp.cmp(jetscape_file_path, output_path)
     os.remove(output_path)
 
 def test_Jetscape_get_sigmaGen(jetscape_file_path):
     jetscape = Jetscape(jetscape_file_path)
     assert jetscape.get_sigmaGen() == (0.000314633,6.06164e-07)
-    
+    
+def test_Jetscape_charge_filter_one_event(jetscape_file_path):
+    jetscape = Jetscape(jetscape_file_path, events=0).charged_particles()
+    assert jetscape.num_events() == 1
+    assert (jetscape.num_output_per_event() == np.array([[1, 14]])).all()
```

### Comparing `sparkx-1.2.0/tests/test_Lattice3D.py` & `sparkx-1.2.1/tests/test_Lattice3D.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_Oscar.py` & `sparkx-1.2.1/tests/test_Oscar.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_Particle.py` & `sparkx-1.2.1/tests/test_Particle.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,24 +173,28 @@
     p = Particle()
     p.status = 27
     assert p.status == 27
     assert isinstance(p.status, int)
 
 def test_initialize_from_array_valid_formats():
     format1 = "JETSCAPE"
-    array1 = np.array([1,211,27,3.0,0.5,1.0,1.5])
+    array1 = np.array([1,211,27,4.36557,3.56147,0.562961,2.45727])
 
     p1 = Particle(input_format=format1,particle_array=array1)
     assert p1.ID == 1
     assert p1.pdg == 211
     assert p1.status == 27
-    assert p1.E == 3.0
-    assert p1.px == 0.5
-    assert p1.py == 1.0
-    assert p1.pz == 1.5
+    assert p1.E == 4.36557
+    assert p1.px == 3.56147
+    assert p1.py == 0.562961
+    assert p1.pz == 2.45727
+    assert np.isclose(p1.mass, 0.137956238, rtol=1e-6)
+    assert p1.pdg_valid == True
+    assert p1.charge == 1
+
 
     format2 = "Oscar2013"
     array2 = np.array([0.0,1.0,2.0,3.0,0.138,4.0,5.0,6.0,7.0,211,100,1])
 
     p2 = Particle(input_format=format2,particle_array=array2)
     assert p2.t == 0.0
     assert p2.x == 1.0
@@ -280,14 +284,23 @@
     assert p5.proc_id_origin == 101
     assert p5.proc_type_origin == 2
     assert p5.t_last_coll == 2.5
     assert p5.pdg_mother1 == 321
     assert p5.pdg_mother2 == 2212
     assert p5.weight == 0.75
 
+def test_initialize_from_array_Jetscape_invalid_pdg_warning():
+    format1 = "JETSCAPE"
+    array1 = np.array([1,99999999,27,4.36557,3.56147,0.562961,2.45727])
+
+    # check that a warning is issued
+    with pytest.warns(UserWarning, match=r"The PDG code 99999999 is not known by PDGID, charge could not be computed. Consider setting it by hand."):
+        Particle(input_format=format1,particle_array=array1)
+
+
 def test_initialize_from_array_invalid_format():
     with pytest.raises(ValueError, match=r"Unsupported input format 'InvalidFormat'"):
         Particle(input_format="InvalidFormat", particle_array=np.array([1, 2, 3]))
 
 def test_initialize_from_array_corrupted_data():
     format1 = "Oscar2013"
     # Provide an array with incorrect length to trigger ValueError
```

### Comparing `sparkx-1.2.0/tests/test_Utilities.py` & `sparkx-1.2.1/tests/test_Utilities.py`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_files/particle_lists.oscar` & `sparkx-1.2.1/tests/test_files/particle_lists.oscar`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_files/particle_lists_extended.oscar` & `sparkx-1.2.1/tests/test_files/particle_lists_extended.oscar`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_files/particle_lists_extended_old.oscar` & `sparkx-1.2.1/tests/test_files/particle_lists_extended_old.oscar`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/tests/test_files/test_jetscape.dat` & `sparkx-1.2.1/tests/test_files/test_jetscape.dat`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/LICENSE` & `sparkx-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/README.md` & `sparkx-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sparkx-1.2.0/pyproject.toml` & `sparkx-1.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sparkx"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
-    { name="Niklas Götz", email="goetz@fias.uni-frankfurt.de"},
-    { name="Hendrik Roch", email="roch@fias.uni-frankfurt.de" },
-    { name="Nils Sass", email="nsass@fias.uni-frankfurt.de" }
+    { name="Niklas Götz", email="goetz@itp.uni-frankfurt.de"},
+    { name="Hendrik Roch", email="hroch@wayne.edu" },
+    { name="Nils Sass", email="nsass@itp.uni-frankfurt.de" }
 ]
 description = "Software Package for Analyzing Relativistic Kinematics in Collision eXperiments"
 readme = "README.md"
+license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
```

