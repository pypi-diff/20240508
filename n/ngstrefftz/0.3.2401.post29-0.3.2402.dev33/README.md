# Comparing `tmp/ngstrefftz-0.3.2401.post29.tar.gz` & `tmp/ngstrefftz-0.3.2402.dev33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngstrefftz-0.3.2401.post29.tar", last modified: Sat Apr 13 05:47:53 2024, max compression
+gzip compressed data, was "ngstrefftz-0.3.2402.dev33.tar", last modified: Wed May  8 20:05:06 2024, max compression
```

## Comparing `ngstrefftz-0.3.2401.post29.tar` & `ngstrefftz-0.3.2402.dev33.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.280027 ngstrefftz-0.3.2401.post29/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.252027 ngstrefftz-0.3.2401.post29/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.260028 ngstrefftz-0.3.2401.post29/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/build_linux_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/ngsolve_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.260028 ngstrefftz-0.3.2401.post29/.github/workflows/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/pyodide/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/pyodide/build_in_docker.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/pyodide/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.github/workflows/pyodide/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-13 05:47:53.280027 ngstrefftz-0.3.2401.post29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.260028 ngstrefftz-0.3.2401.post29/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.260028 ngstrefftz-0.3.2401.post29/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/_static/breadcrumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.260028 ngstrefftz-0.3.2401.post29/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/_static/css/mytheme.css
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/contrib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/docu.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.264027 ngstrefftz-0.3.2401.post29/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-adv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-helm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-poi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-stokes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-wave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/helmholtz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/laplace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/qtwave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/tunfitted.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/twave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/notebooks/twavetents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.264027 ngstrefftz-0.3.2401.post29/docs/paper/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/paper/codemeta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.252027 ngstrefftz-0.3.2401.post29/external_dependencies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.264027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.252027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.264027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.256027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.264027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/advection/
--rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/advection/advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.264027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/burgers/
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/burgers/burgers1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/burgers/burgers2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.264027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/euler/
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/euler/euler2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.264027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/maxwell/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.268027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.268027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/tents/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/tents/draw3dtent.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/tents/draw3dvertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.268027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/wave/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/wave/horn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/wave/wave2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/wave/wave3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.268027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/BurgersMTP.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/INDEX.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/StartPitching.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.268027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/figs/
--rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/figs/CausalityCond.png
--rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/figs/dag.png
--rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/figs/map.png
--rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/figs/subtents.png
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.268027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.268027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/conslaw/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/conslaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.268027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/utils/_drawtents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/utils/_drawtents2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.272027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/advection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/burgers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/concurrentqueue.h
--rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/conservationlaw.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/euler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/maxwell.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/paralleldepend.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/python_conslaw.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/python_tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/symbolic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tentsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tentsolver_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/vis3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/vis3d.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/wave.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.272027 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_burgers_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_causal_tents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_conslaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_tent_height_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-13 05:47:16.000000 ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_tentlayers.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:47:53.280027 ngstrefftz-0.3.2401.post29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.276027 ngstrefftz-0.3.2401.post29/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/airy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/condensedg.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/condensedg.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/diffopmapped.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26486 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/embtrefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/embtrefftz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/mesh1dtents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/mesh1dtents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/monomialfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/monomialfespace.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.280027 ngstrefftz-0.3.2401.post29/src/ngstrefftz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-13 05:47:53.000000 ngstrefftz-0.3.2401.post29/src/ngstrefftz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-13 05:47:53.000000 ngstrefftz-0.3.2401.post29/src/ngstrefftz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:47:53.000000 ngstrefftz-0.3.2401.post29/src/ngstrefftz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 05:47:53.000000 ngstrefftz-0.3.2401.post29/src/ngstrefftz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 05:47:53.000000 ngstrefftz-0.3.2401.post29/src/ngstrefftz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/ngsttd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/planewavefe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/planewavefe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/python_trefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/scalarmappedfe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/scalarmappedfe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/specialcoefficientfunction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/specialcoefficientfunction.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/specialintegrator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/specialintegrator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    56525 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/trefftzfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/trefftzfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    45126 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/twavetents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/src/twavetents.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:47:53.280027 ngstrefftz-0.3.2401.post29/test/
--rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/test/dg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/test/embt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/test/tents.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-13 05:47:15.000000 ngstrefftz-0.3.2401.post29/test/trefftz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.780124 ngstrefftz-0.3.2402.dev33/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build_linux_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/ngsolve_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/build_in_docker.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/_static/breadcrumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/_static/css/mytheme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/docu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-adv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-helm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-poi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-stokes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-wave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/helmholtz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/laplace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/qtwave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/tunfitted.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/twave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/twavetents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/docs/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/paper/codemeta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.784124 ngstrefftz-0.3.2402.dev33/external_dependencies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.784124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.784124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/burgers1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/burgers2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/euler2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/maxwell/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/draw3dtent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/draw3dvertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/horn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/BurgersMTP.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/INDEX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/StartPitching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/
+-rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/CausalityCond.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/dag.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/subtents.png
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/conslaw/
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/conslaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/_drawtents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/_drawtents2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.804124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/advection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/burgers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/concurrentqueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/conservationlaw.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/maxwell.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/paralleldepend.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/python_conslaw.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/python_tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/symbolic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tentsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tentsolver_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/vis3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/vis3d.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/wave.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.804124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_burgers_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_causal_tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_conslaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_tent_height_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_tentlayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.808124 ngstrefftz-0.3.2402.dev33/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/airy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/condensedg.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/condensedg.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/diffopmapped.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/embtrefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/embtrefftz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/mesh1dtents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/mesh1dtents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/monomialfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/monomialfespace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/ngsttd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/planewavefe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/planewavefe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/python_trefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/scalarmappedfe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/scalarmappedfe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/specialcoefficientfunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/specialcoefficientfunction.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/specialintegrator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/specialintegrator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    56525 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/trefftzfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/trefftzfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45126 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/twavetents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/twavetents.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/test/dg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/test/embt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/test/tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/test/trefftz.py
```

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/build.yml` & `ngstrefftz-0.3.2402.dev33/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
           name: python-package-distributions-linux
           path: NGSTrefftz/wheelhouse
 
   pypi-mac:
     name: Build wheels for macOS
     strategy:
       matrix:
-        py: ['3.8', '3.9', '3.10', '3.11']
+        py: ['3.8', '3.9', '3.10', '3.11', '3.12']
     runs-on: macos-11
     env:
       MACOSX_DEPLOYMENT_TARGET: '10.15'
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
@@ -66,15 +66,15 @@
           name: python-package-distributions-mac-${{ matrix.py }}
           path: NGSTrefftz/wheelhouse
 
   pypi-win:
     name: Build wheels for Windows
     strategy:
       matrix:
-        py: ['3.8', '3.9', '3.10', '3.11']
+        py: ['3.8', '3.9', '3.10', '3.11', '3.12']
     runs-on: windows-2019
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           submodules: recursive
           fetch-depth: 0
@@ -103,15 +103,15 @@
           path: 'NGSTrefftz'
       - name: install pkgs
         run: |
              sudo apt-get update && DEBIAN_FRONTEND="noninteractive" sudo apt-get -y install vim python3 python3-pip python3-distutils python3-tk libpython3-dev libxmu-dev tk-dev tcl-dev cmake git g++ libglu1-mesa-dev libblas-dev liblapack-dev
       - name: Update pip and Install setuptools
         run: |
           python3 -m pip install --upgrade pip
-          python3 -m pip install -U pytest-check numpy wheel scikit-build mkl==2023.* mkl-devel==2023.* setuptools
+          python3 -m pip install -U pytest-check numpy wheel scikit-build mkl==2023.* mkl-devel==2023.* setuptools setuptools_scm
           python3 -m pip install ngsolve --pre
       - name: Package ngstrefftz sources for PyPI
         run: cd NGSTrefftz && python3 setup.py sdist -d wheelhouse
       #- name: pip install ngstrefftz
         #run: pip install dist/*
       - name: Store the sdist
         uses: actions/upload-artifact@v4
@@ -172,15 +172,16 @@
           context: .
           file: "Dockerfile"
           push: ${{ github.event_name == 'release' && github.event.action == 'created' }}
           tags: ${{ steps.meta.outputs.tags }}
           #labels: ${{ steps.meta.outputs.labels }}
 
   pyodide:
-    needs: [publish-pypi]
+    #needs: [publish-pypi]
+    if: false
     runs-on: ubuntu-latest
     steps:
       - name: clear cache
         run: rm -rf /opt/hostedtoolcache
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # otherwise, you will failed to push refs to dest repo
@@ -206,15 +207,15 @@
         with:
           name: ngst-pyodide
           path: ./ngst-pyodide
 
 
 
   docs:
-    needs: [pyodide]
+    needs: [publish-pypi]
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # otherwise, you will failed to push refs to dest repo
           submodules: 'True'
           path: 'NGSTrefftz'
@@ -224,29 +225,22 @@
         #run: python3 -m pip list
       - name: pip install requirements
         run: pip install --user -r $GITHUB_WORKSPACE/NGSTrefftz/docs/requirements.txt
       - name: set path
         run: |
              echo "NETGENDIR=/usr/bin/" >> $GITHUB_ENV
              echo "LD_LIBRARY_PATH=${{ env.LD_LIBRARY_PATH }}:/home/runner/.local/lib:/usr/local/lib/" >> $GITHUB_ENV
-      - name: webgui
-        run: |
-             pip install jupyter_contrib_nbextensions 
-             jupyter contrib nbextension install --user
-             jupyter nbextension install --user --py widgetsnbextension
-             jupyter nbextension enable --user --py widgetsnbextension
-             jupyter nbextension install --user --py webgui_jupyter_widgets
-             jupyter nbextension enable --user --py webgui_jupyter_widgets            
       - name: Build and Commit
         uses: sphinx-notes/pages@v2
         with:
           repository_path: 'NGSTrefftz'
           publish: false
           #requirements_path: ./docs/requirements.txt
       - name: Download pyodide stuff
+        if: false
         uses: actions/download-artifact@v4
         with:
           name: ngst-pyodide
           path: NGSTrefftz/ngst-pyodide
       - run: tree -d .
       - name: Upload
         uses: actions/upload-pages-artifact@v3
```

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/build_linux_test.sh` & `ngstrefftz-0.3.2402.dev33/.github/workflows/build_linux_test.sh`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 cd workspace
 yum -y update && yum -y install git ninja-build fontconfig-devel tk-devel tcl-devel libXmu-devel mesa-libGLU-devel ccache python-devel lapack blas 
 
 export pyversion=310
 export PYDIR="/opt/python/cp${pyversion}-cp${pyversion}/bin"
 export PATH=$PATH:$PYDIR
 
+$PYDIR/pip install numpy mkl==2023.* mkl-devel==2023.* 
 $PYDIR/pip install -r ./NGSTrefftz/.github/workflows/ngsolve_version.txt
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/opt/_internal/cpython-3.10.9/lib/
 
+echo "SHOW MKL"
+$PYDIR/pip show mkl
+
 cmake -DCMAKE_CXX_COMPILER=ngscxx -DNETGENDIR=$PYDIR/.. -DCMAKE_PREFIX_PATH=$PYDIR/..  -DPYTHON_EXECUTABLE=$PYDIR/python3 -DPYTHON_LIBRARY=$PYDIR/../lib -DPYTHON_INCLUDE_DIR=$PYDIR/../include -B ./NGSTrefftz/make -S ./NGSTrefftz/src/
 make -C ./NGSTrefftz/make
 env CTEST_OUTPUT_ON_FAILURE=1 make -C ./NGSTrefftz/make test
 make -C ./NGSTrefftz/make install
```

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip.ps1`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #Get-ChildItem venv_ngs
 #Get-ChildItem venv_ngs\lib
 #Get-ChildItem venv_ngs\include
 #Get-ChildItem venv_ngs\scripts
 #Write-Host $env:LIB
 
 
-pip3 install scikit-build wheel numpy twine mkl-devel==2022.* mkl==2022.*
+pip3 install scikit-build wheel numpy twine mkl-devel==2022.* mkl==2022.* setuptools setuptools_scm
 pip3 install -r ngsolve_version.txt
 
 
 #$env:PYDIR = "$env:Python3_ROOT_DIR"
 #$env:PATH += ";$env:pythonLibrary;$env:Python3_ROOT_DIR"
 $env:NGSolve_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\ngsolve\cmake"
 $env:Netgen_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\netgen\cmake"
```

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip.sh`

 * *Files 7% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 rm -rf wheelhouse
 mkdir wheelhouse
 
 git config --global --add safe.directory '*'
 
 export ORIGINAL_PATH="$PATH"
 
-for pyversion in 38 39 310 311
+for pyversion in 38 39 310 311 312
 do
     export PYDIR="/opt/python/cp${pyversion}-cp${pyversion}/bin"
     export PATH="$ORIGINAL_PATH:$PYDIR"
     #echo $PYDIR
     #$PYDIR/pip install -U pytest-check numpy wheel scikit-build mkl==2021.* mkl-devel==2021.*
     #$PYDIR/pip install netgen-mesher
     #NETGENDIR=/opt/_internal/cpython-3.9.13/bin
 
     #rm -rf /home/app/ngstrefftz/make
     rm -rf _skbuild
-    $PYDIR/pip install pytest-check numpy wheel scikit-build mkl==2023.* mkl-devel==2023.* setuptools
+    $PYDIR/pip install pytest-check numpy wheel scikit-build mkl==2023.* mkl-devel==2023.* setuptools setuptools_scm
     $PYDIR/pip install -r ./.github/workflows/ngsolve_version.txt
 
     $PYDIR/pip wheel -vvv .
-    cat src/ngstrefftz.egg-info/SOURCES.txt
+    #cat src/ngstrefftz.egg-info/SOURCES.txt
     #auditwheel repair ngstrefftz*.whl
     rename linux_ manylinux_2_17_x86_64.manylinux2014_ ngstrefftz*.whl
     mv ngstrefftz*.whl wheelhouse/
     rm -rf *.whl
-    $PYDIR/pip uninstall -y ngsolve netgen-mesher setuptools pytest-check numpy wheel scikit-build mkl mkl-devel 
+    $PYDIR/pip uninstall -y ngsolve netgen-mesher setuptools setuptools_scm pytest-check numpy wheel scikit-build mkl mkl-devel 
 
 
     # avx2 build:
     #rm -rf _skbuild
     #$PYDIR/pip install ngsolve-avx2 --pre
     #NETGEN_ARCH=avx2 $PYDIR/pip wheel -vvv .
     #auditwheel repair ngstrefftz*.whl
```

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip_mac.sh`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 export PATH=/Applications/CMake.app/Contents/bin:$PATH
 export NETGEN_Dir=$PYDIR/../lib/python$1/site-packages/netgen/cmake
 export NGSolve_Dir=$PYDIR/../lib/python$1/site-packages/ngsolve/cmake
 export CMAKE_PREFIX_PATH=$CMAKE_PREFIX_PATH:$NGSolve_Dir:$NETGEN_Dir
 #export PYDIR=/Library/Frameworks/Python.framework/Versions/$1/bin
 #$PYDIR/python3 -m venv ../venv_ngs
 #source ../venv_ngs/bin/activate
-$PYDIR/pip3 install scikit-build wheel
+$PYDIR/pip3 install scikit-build wheel setuptools setuptools_scm
 #$PYDIR/pip3 install -U pytest-check numpy wheel scikit-build mkl==2022.* mkl-devel==2022.* setuptools
 
 export CMAKE_OSX_ARCHITECTURES='arm64;x86_64'
 #export CMAKE_OSX_ARCHITECTURES='x86_64'
 $PYDIR/pip3 install -r ./.github/workflows/ngsolve_version.txt
 
 #$PYDIR/pip3 wheel .
```

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2402.dev33/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/pyodide/Dockerfile` & `ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/pyodide/build_in_docker.sh` & `ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/build_in_docker.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/pyodide/merge.py` & `ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/merge.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/.github/workflows/pyodide/requirements.txt` & `ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/CONTRIBUTING.md` & `ngstrefftz-0.3.2402.dev33/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/Dockerfile` & `ngstrefftz-0.3.2402.dev33/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/LICENSE` & `ngstrefftz-0.3.2402.dev33/LICENSE`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/PKG-INFO` & `ngstrefftz-0.3.2402.dev33/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2401.post29
+Version: 0.3.2402.dev33
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
 Requires-Dist: ngsolve>=6.2.2401.post24.dev0
-Requires-Dist: ngstents>=0.0.1.post31
+Requires-Dist: ngstents>=0.0.2.dev39
 Requires-Dist: mkl
 
 NGSTrefftz provides a framework to implement Trefftz finite element spaces for NGSolve, with several Trefftz spaces already implemented. Additionally, Trefftz-DG on tent-pitched meshes for the acoustic wave equation is implemented using meshes provided by ngstents. Furthermore, the package includes an implementation of the embedded Trefftz method.
```

### Comparing `ngstrefftz-0.3.2401.post29/README.md` & `ngstrefftz-0.3.2402.dev33/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/conf.py` & `ngstrefftz-0.3.2402.dev33/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,14 @@
 from os.path import dirname, isdir, join
 import os
 import re
 import subprocess
-def get_version():
-    """
-    Gets the current version number.
-    If in a git repository, it is the current git tag.
-    Otherwise it is the one contained in the PKG-INFO file.
-    """
-    version_re = re.compile('^Version: (.+)$', re.M)
-    d = dirname(__file__)+'/..'
-
-    if isdir(join(d, '.git')):
-        # Get the version using "git describe".
-        cmd = 'git describe --always --tags --match v[0-9]*'.split()
-        try:
-            version = subprocess.check_output(cmd).decode().strip()
-        except subprocess.CalledProcessError:
-            print('Unable to get version number from git tags')
-            exit(1)
-
-        # PEP 386 compatibility
-        if '-' in version:
-            version = '.post'.join(version.split('-')[:2])
-
-        # Don't declare a version "dirty" merely because a time stamp has
-        # changed. If it is dirty, append a ".dev1" suffix to indicate a
-        # development revision after the release.
-        with open(os.devnull, 'w') as fd_devnull:
-            subprocess.call(['git', 'status'],
-                            stdout=fd_devnull, stderr=fd_devnull)
-
-        cmd = 'git diff-index --name-only HEAD'.split()
-        try:
-            dirty = subprocess.check_output(cmd).decode().strip()
-        except subprocess.CalledProcessError:
-            print('Unable to get git index status')
-            exit(1)
-
-        # if dirty != '':
-            # version += '.dev1'
-
-        # strip the v for pypi
-        version = version[1:]
-
-    else:
-        # Extract the version from the PKG-INFO file.
-        with open(join(d, 'PKG-INFO')) as f:
-            version = version_re.search(f.read()).group(1)
 
-    return version
+from setuptools_scm import get_version
+_cmake_args = []
 
 
 # Configuration file for the Sphinx documentation builder.
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
@@ -72,15 +27,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'NGSTrefftz'
 copyright = '2022, Paul Stocker'
 author = 'Paul Stocker'
 
 # The full version, including alpha/beta/rc tags
-release = get_version()
+release = get_version(root='..', relative_to=__file__).split('+')[0]
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 # extensions = [ "myst_nb" ]
```

### Comparing `ngstrefftz-0.3.2401.post29/docs/docu.rst` & `ngstrefftz-0.3.2402.dev33/docs/docu.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/index.rst` & `ngstrefftz-0.3.2402.dev33/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/intro.rst` & `ngstrefftz-0.3.2402.dev33/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-adv.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-adv.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-helm.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-helm.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-poi.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-poi.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-stokes.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-stokes.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz-wave.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-wave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/embTrefftz.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/helmholtz.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/helmholtz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/index.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/laplace.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/laplace.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/qtwave.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/qtwave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/tunfitted.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/tunfitted.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/twave.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/twave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/notebooks/twavetents.ipynb` & `ngstrefftz-0.3.2402.dev33/docs/notebooks/twavetents.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/paper/codemeta.json` & `ngstrefftz-0.3.2402.dev33/docs/paper/codemeta.json`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/paper/paper.bib` & `ngstrefftz-0.3.2402.dev33/docs/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/paper/paper.md` & `ngstrefftz-0.3.2402.dev33/docs/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/docs/requirements.txt` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -103,9 +103,8 @@
 webencodings==0.5.1
 webgui-jupyter-widgets==0.2.14
 websocket-client==1.4.1
 widgetsnbextension==4.0.3
 scipy>=1.11.1 
 
 ngsolve==6.2.2304
-xfem==2.1.2303.post8.dev0
-ngstrefftz==0.2.6
+ngstents==0.0.1.post2
```

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/build.yml` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip.ps1`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/README.md` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/advection/advection2d.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/advection/advection2d_periodic.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/advection2d_periodic.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/burgers/burgers1d.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/burgers1d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/burgers/burgers2d.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/burgers2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/euler/euler2d.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/euler2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/maxwell/maxwell3d.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/maxwell/maxwell3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/tents/draw3dtent.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/draw3dtent.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/tents/draw3dvertex.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/draw3dvertex.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/wave/horn.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/horn.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/wave/wave2d.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/demo/wave/wave3d.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/BurgersMTP.ipynb` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/BurgersMTP.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/INDEX.ipynb` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/INDEX.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/StartPitching.ipynb` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/StartPitching.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/conf.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/figs/CausalityCond.png` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/CausalityCond.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/figs/dag.png` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/dag.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/figs/map.png` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/map.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/figs/subtents.png` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/subtents.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/docs/index.rst` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/conslaw/__init__.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/conslaw/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/utils/_drawtents.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/_drawtents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/py/utils/_drawtents2d.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/_drawtents2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/setup.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/setup.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/CMakeLists.txt` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/advection.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/advection.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/burgers.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/burgers.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/concurrentqueue.h` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/concurrentqueue.h`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/conservationlaw.hpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/conservationlaw.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/euler.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/euler.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/maxwell.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/maxwell.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/paralleldepend.hpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/paralleldepend.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/python_conslaw.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/python_conslaw.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/python_tents.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/python_tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/symbolic.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/symbolic.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tents.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tents.hpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tentsolver.hpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tentsolver.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/tentsolver_impl.hpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tentsolver_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/vis3d.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/vis3d.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/vis3d.hpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/vis3d.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/src/wave.cpp` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/wave.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_burgers_2D.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_burgers_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_causal_tents.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_causal_tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_conslaw.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_conslaw.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_tent_height_2D.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_tent_height_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/external_dependencies/ngstents/tests/test_tentlayers.py` & `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_tentlayers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/__init__.py` & `ngstrefftz-0.3.2402.dev33/src/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ngsolve.fem import ET,IntegrationRule
 from ngsolve.comp import L2,BilinearForm,LinearForm,SymbolicBFI,SymbolicLFI,FESpace
 from ngsolve.fem import CoordCF
-from ngstents._pytents import TentSlab, Tent
+from ngstents import TentSlab, Tent
 from ._trefftz import *
 
 def GetWave(self,U):
     order=self.GetOrder()
     D = self.GetSpaceDim()
     initmesh = self.GetInitmesh()
     if D==3: eltyp = ET.TET
```

### Comparing `ngstrefftz-0.3.2401.post29/src/airy.cpp` & `ngstrefftz-0.3.2402.dev33/src/airy.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/condensedg.cpp` & `ngstrefftz-0.3.2402.dev33/src/condensedg.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #include "condensedg.hpp"
 
 namespace ngcomp
 {
-  template <typename TSCAL>
-  void
-  GetSubMatrix (shared_ptr<SparseMatrixTM<TSCAL>> mat, FlatArray<int> drow,
-                FlatArray<int> dcol, FlatMatrix<> out)
+  void GetSubMatrix (shared_ptr<BaseMatrix> mat, FlatArray<int> drow,
+                     FlatArray<int> dcol, FlatMatrix<> out)
   {
     // auto colnr = mat->GetColIndices();
     // for (int i = 0; i < drow.Size (); i++)
     // for (size_t si = mat->First[drow[i]], j = 0; si < mat->First[drow[i] +
     // 1]; si++) if (dcol.Contains (colnr[si])) out (i, j++) = data[si];
+    auto smat = dynamic_pointer_cast<SparseMatrix<double>> (mat);
     for (int i = 0; i < drow.Size (); i++)
       for (int j = 0; j < dcol.Size (); j++)
-        out (i, j) = (*mat) (drow[i], dcol[j]);
+        out (i, j) = smat->operator() (drow[i], dcol[j]);
   }
 
   // template <typename T>
   // inline void AInvBt (ngbla::FlatMatrix<T> a, ngbla::FlatMatrix<T> b)
   //{
   // LapackAInvBt (a, b, 'N');
   //}
@@ -57,19 +56,19 @@
     return els;
   }
 
   shared_ptr<BaseMatrix>
   CondenseDG (shared_ptr<BaseMatrix> mat, shared_ptr<BaseVector> vec,
               shared_ptr<FESpace> fes)
   {
-    auto smat = dynamic_pointer_cast<SparseMatrixTM<double>> (mat);
+    auto smat = dynamic_pointer_cast<SparseMatrix<double>> (mat);
     auto svec = vec; // dynamic_pointer_cast<VVector<double>> (vec);
     if (!smat || !svec)
       throw Exception ("CondenseDG: matrix must be of type "
-                       "SparseMatrixTM and vector must be of type VVector");
+                       "SparseMatrix and vector must be of type VVector");
 
     static Timer sc ("CondenseDG");
     RegionTimer reg (sc);
     LocalHeap lh (1000 * 1000 * 1000);
 
     auto ma = fes->GetMeshAccess ();
     size_t ne = ma->GetNE (VOL);
@@ -115,17 +114,17 @@
                         creator.Add (ei.Nr (), d);
                   }
               }
           }
       }
     table = creator.MoveTable ();
 
-    SparseMatrix<double> PP (vndof, vndof, table, table,
-                             false); // TODO: support symmetric
-    PP.SetZero ();
+    auto PP = make_shared<SparseMatrix<double>> (
+        vndof, vndof, table, table, false); // TODO: support symmetric
+    PP->SetZero ();
     // finished output matrix
 
     ma->IterateElements (VOL, lh, [&] (auto ei, LocalHeap &mlh) {
       Array<DofId> dofs1;
       fes->GetDofNrs (ei, dofs1);
       Array<int> idofs1 (dofs1.Size (), mlh), odofs1 (dofs1.Size (), mlh);
       idofs1.SetSize0 ();
@@ -138,15 +137,15 @@
           if (ct & ctype)
             idofs1.AppendHaveMem (i);
           else if (ct != UNUSED_DOF)
             odofs1.AppendHaveMem (i);
         }
 
       FlatMatrix<> DD (idofs1.Size (), idofs1.Size (), mlh);
-      GetSubMatrix<double> (smat, idofs1, idofs1, DD);
+      GetSubMatrix (smat, idofs1, idofs1, DD);
 
       FlatVector<> dd (idofs1.Size (), mlh);
       svec->GetIndirect (idofs1, dd);
 
       Array<int> els = GetElNeighbours (ma, ei);
       els.Append (ei.Nr ());
 
@@ -165,19 +164,19 @@
               if (ct & ctype)
                 idofs2.AppendHaveMem (i);
               else if (ct != UNUSED_DOF)
                 odofs2.AppendHaveMem (i);
             }
 
           FlatMatrix<> AA (odofs1.Size (), odofs2.Size (), mlh);
-          GetSubMatrix<double> (smat, odofs1, odofs2, AA);
-          PP.AddElementMatrix (odofs1, odofs2, AA, true);
+          GetSubMatrix (smat, odofs1, odofs2, AA);
+          PP->AddElementMatrix (odofs1, odofs2, AA, true);
 
           FlatMatrix<> BB (odofs2.Size (), idofs1.Size (), mlh);
-          GetSubMatrix<double> (smat, odofs2, idofs1, BB);
+          GetSubMatrix (smat, odofs2, idofs1, BB);
           AInvBt (DD, BB); // b <--- b d^-1 TODO: compute only once Dinv
 
           FlatVector<> vv (odofs2.Size (), mlh);
           vv = -1.0 * BB * dd;
           svec->AddIndirect (odofs2, vv, true);
 
           // Array<int> *odofs[2] = { &odofs1, &odofs2 };
@@ -197,30 +196,30 @@
                   if (ct & ctype)
                     idofs3.AppendHaveMem (i);
                   else if (ct != UNUSED_DOF)
                     odofs3.AppendHaveMem (i);
                 }
 
               FlatMatrix<> CC (idofs1.Size (), odofs3.Size (), mlh);
-              GetSubMatrix<double> (smat, idofs1, odofs3, CC);
+              GetSubMatrix (smat, idofs1, odofs3, CC);
 
               FlatMatrix<> BDC (odofs2.Size (), odofs3.Size (), mlh);
               BDC = 0.0;
               // GetSubMatrix<double> (smat, odofs2, odofs3, AA);
               SubAB (BB, CC, BDC); // AA <--- -b c = -b d^-1 c why no SubABt?
-              PP.AddElementMatrix (odofs2, odofs3, BDC, true);
+              PP->AddElementMatrix (odofs2, odofs3, BDC, true);
               // smat->AddElementMatrix (odofs2, odofs3, BDC, true);
             }
         }
     });
 
     //*smat.get() = move(PP);
     // SparseMatrixTM<double> SPP (move(PP));
     // swap (SPP, PP);
-    return make_shared<SparseMatrix<double>> (PP);
+    return PP;
   }
 }
 
 ////////////////////////// python interface ///////////////////////////
 
 #ifdef NGS_PYTHON
```

### Comparing `ngstrefftz-0.3.2401.post29/src/condensedg.hpp` & `ngstrefftz-0.3.2402.dev33/src/condensedg.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 #include <fem.hpp>
 // #include <integratorcf.hpp>
 // #include <variant>
 #include <bla.hpp>
 
 namespace ngcomp
 {
-  template <typename TSCAL>
-  void
-  GetSubMatrix (shared_ptr<SparseMatrixTM<TSCAL>> mat, FlatArray<int> drow,
-                FlatArray<int> dcol, FlatMatrix<> out);
+  void GetSubMatrix (shared_ptr<BaseMatrix> mat, FlatArray<int> drow,
+                     FlatArray<int> dcol, FlatMatrix<> out);
 
   shared_ptr<BaseMatrix>
   CondenseDG (shared_ptr<BaseMatrix> mat, shared_ptr<BaseVector> vec,
               shared_ptr<FESpace> fes);
 }
 
 #ifdef NGS_PYTHON
```

### Comparing `ngstrefftz-0.3.2401.post29/src/diffopmapped.hpp` & `ngstrefftz-0.3.2402.dev33/src/diffopmapped.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/embtrefftz.cpp` & `ngstrefftz-0.3.2402.dev33/src/embtrefftz.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,15 @@
       for (auto icf : lf->icfs)
         {
           auto &dx = icf->dx;
           lfis[dx.vb] += icf->MakeLinearFormIntegrator ();
         }
 
     vector<shared_ptr<Matrix<SCAL>>> ETmats (ne);
-    VVector<SCAL> lfvec (ndof);
-    lfvec = 0.0;
+    auto lfvec = make_shared<VVector<SCAL>> (ndof);
 
     size_t active_elements = 0;
     size_t test_local_ndof = test_fes->GetNDof () / ne;
     Vector<SCAL> sing_val_avg;
     Vector<double> sing_val_max;
     Vector<double> sing_val_min;
 
@@ -264,15 +263,15 @@
             = make_shared<Matrix<SCAL>> (U.Cols (0, dofs.Size () - nz));
       else
         ETmats[ei.Nr ()] = make_shared<Matrix<SCAL>> (
             Trans (Vt.Rows (dofs.Size () - nz, dofs.Size ())));
 
       if (stats)
         {
-          const lock_guard<mutex> lock(stats_mutex);
+          const lock_guard<mutex> lock (stats_mutex);
           if (sing_val_avg.Size () == 0)
             {
               sing_val_avg.SetSize (elmat.Height ());
               sing_val_max.SetSize (elmat.Height ());
               sing_val_min.SetSize (elmat.Height ());
               sing_val_avg = 0;
               sing_val_max = 0;
@@ -315,27 +314,27 @@
           for (int i = 0; i < nnz; i++)
             SigI (i, i) = 1.0 / elmat (i, i);
           Matrix<SCAL> elinverse = V * SigI * Ut;
 
           // lfvec.FV () (dofs) = elinverse * elvec;
           FlatVector<SCAL> elsol (dofs.Size (), mlh);
           elsol = elinverse * elvec;
-          lfvec.SetIndirect (dofs, elsol);
+          lfvec->SetIndirect (dofs, elsol);
         }
     });
 
     if (stats)
       {
         sing_val_avg /= active_elements;
         (*stats)["singavg"] = Vector<SCAL> (sing_val_avg);
         (*stats)["singmax"] = Vector<double> (sing_val_max);
         (*stats)["singmin"] = Vector<double> (sing_val_min);
       }
 
-    return std::make_tuple (ETmats, make_shared<VVector<SCAL>> (lfvec));
+    return std::make_tuple (ETmats, lfvec);
   }
 
   template std::tuple<vector<shared_ptr<Matrix<double>>>,
                       shared_ptr<BaseVector>>
   EmbTrefftz<double> (shared_ptr<SumOfIntegrals> bf, shared_ptr<FESpace> fes,
                       shared_ptr<SumOfIntegrals> lf, double eps,
                       shared_ptr<FESpace> test_fes, int tndof, bool getrange,
@@ -399,16 +398,16 @@
               creator.Add (ne + hcnt, d);
               creator2.Add (ne + hcnt++, prevdofs++);
             }
       }
     table = creator.MoveTable ();
     table2 = creator2.MoveTable ();
 
-    SparseMatrix<SCAL> PP (fes->GetNDof (), prevdofs, table, table2, false);
-    auto P = make_shared<SparseMatrix<SCAL>> (PP);
+    auto P = make_shared<SparseMatrix<SCAL>> (fes->GetNDof (), prevdofs, table,
+                                              table2, false);
     P->SetZero ();
     for (auto ei : ma->Elements (VOL))
       if (ETmats[ei.Nr ()])
         P->AddElementMatrix (table[ei.Nr ()], table2[ei.Nr ()],
                              *(ETmats[ei.Nr ()]));
 
     SCAL one = 1;
@@ -522,22 +521,22 @@
     static Timer timer ("EmbTrefftz: VTransform");
     RegionTimer reg (timer);
 
     size_t nz = (ETmats[ei.Nr ()])->Width ();
 
     if (type == TRANSFORM_RHS)
       {
-        Vector<double> new_vec (vec.Size ());
+        Vector<double> new_vec (nz);
         new_vec = Trans (*(ETmats[ei.Nr ()])) * vec;
         vec = new_vec;
       }
     else if (type == TRANSFORM_SOL)
       {
         Vector<double> new_vec (vec.Size ());
-        new_vec = (*(ETmats[ei.Nr ()])) * vec;
+        new_vec = (*(ETmats[ei.Nr ()])) * vec.Range (0, nz);
         vec = new_vec;
       }
   }
 
   template class EmbTrefftzFESpace<L2HighOrderFESpace,
                                    shared_ptr<L2HighOrderFESpace>>;
   static RegisterFESpace<
```

### Comparing `ngstrefftz-0.3.2401.post29/src/embtrefftz.hpp` & `ngstrefftz-0.3.2402.dev33/src/embtrefftz.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/mesh1dtents.cpp` & `ngstrefftz-0.3.2402.dev33/src/mesh1dtents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/monomialfespace.cpp` & `ngstrefftz-0.3.2402.dev33/src/monomialfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/monomialfespace.hpp` & `ngstrefftz-0.3.2402.dev33/src/monomialfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/ngstrefftz.egg-info/PKG-INFO` & `ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2401.post29
+Version: 0.3.2402.dev33
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
 Requires-Dist: ngsolve>=6.2.2401.post24.dev0
-Requires-Dist: ngstents>=0.0.1.post31
+Requires-Dist: ngstents>=0.0.2.dev39
 Requires-Dist: mkl
 
 NGSTrefftz provides a framework to implement Trefftz finite element spaces for NGSolve, with several Trefftz spaces already implemented. Additionally, Trefftz-DG on tent-pitched meshes for the acoustic wave equation is implemented using meshes provided by ngstents. Furthermore, the package includes an implementation of the embedded Trefftz method.
```

### Comparing `ngstrefftz-0.3.2401.post29/src/ngstrefftz.egg-info/SOURCES.txt` & `ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/planewavefe.cpp` & `ngstrefftz-0.3.2402.dev33/src/planewavefe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/planewavefe.hpp` & `ngstrefftz-0.3.2402.dev33/src/planewavefe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/python_trefftz.cpp` & `ngstrefftz-0.3.2402.dev33/src/python_trefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/scalarmappedfe.cpp` & `ngstrefftz-0.3.2402.dev33/src/scalarmappedfe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/scalarmappedfe.hpp` & `ngstrefftz-0.3.2402.dev33/src/scalarmappedfe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/specialcoefficientfunction.cpp` & `ngstrefftz-0.3.2402.dev33/src/specialcoefficientfunction.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/specialcoefficientfunction.hpp` & `ngstrefftz-0.3.2402.dev33/src/specialcoefficientfunction.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/specialintegrator.cpp` & `ngstrefftz-0.3.2402.dev33/src/specialintegrator.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/specialintegrator.hpp` & `ngstrefftz-0.3.2402.dev33/src/specialintegrator.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/trefftzfespace.cpp` & `ngstrefftz-0.3.2402.dev33/src/trefftzfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/trefftzfespace.hpp` & `ngstrefftz-0.3.2402.dev33/src/trefftzfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/twavetents.cpp` & `ngstrefftz-0.3.2402.dev33/src/twavetents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/src/twavetents.hpp` & `ngstrefftz-0.3.2402.dev33/src/twavetents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/test/dg.py` & `ngstrefftz-0.3.2402.dev33/test/dg.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/test/embt.py` & `ngstrefftz-0.3.2402.dev33/test/embt.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/test/tents.py` & `ngstrefftz-0.3.2402.dev33/test/tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post29/test/trefftz.py` & `ngstrefftz-0.3.2402.dev33/test/trefftz.py`

 * *Files identical despite different names*

