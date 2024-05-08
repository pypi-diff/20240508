# Comparing `tmp/mobspy-2.4.0.tar.gz` & `tmp/mobspy-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobspy-2.4.0.tar", last modified: Sat May  4 20:37:25 2024, max compression
+gzip compressed data, was "mobspy-2.4.1.tar", last modified: Tue May  7 17:51:37 2024, max compression
```

## Comparing `mobspy-2.4.0.tar` & `mobspy-2.4.1.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.728331 mobspy-2.4.0/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:24.785379 mobspy-2.4.0/.github/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:24.958803 mobspy-2.4.0/.github/workflows/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-06-15 12:59:57.000000 mobspy-2.4.0/.github/workflows/python-app.yml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      415 2024-04-09 17:41:00.000000 mobspy-2.4.0/.gitignore
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1034 2024-02-26 16:22:21.000000 mobspy-2.4.0/.readthedocs.yaml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-06-15 12:59:57.000000 mobspy-2.4.0/LICENSE
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-04 20:37:25.727055 mobspy-2.4.0/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6331 2024-03-08 01:34:03.000000 mobspy-2.4.0/README.md
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:24.993806 mobspy-2.4.0/docs/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      634 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Makefile
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.036800 mobspy-2.4.0/docs/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.039528 mobspy-2.4.0/docs/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_autosummary/mobspy.rst
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:24.805672 mobspy-2.4.0/docs/_build/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.103494 mobspy-2.4.0/docs/_build/doctrees/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.150735 mobspy-2.4.0/docs/_build/doctrees/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    95114 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23601 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30820 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/03_Characteristics.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7466 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    24161 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/05_For_Loops.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21599 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    50076 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18699 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/08_Units.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41471 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/09_Result_Data.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    28500 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15272 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17080 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/12_Born_Species.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    39545 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/13_Events.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15325 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.152782 mobspy-2.4.0/docs/_build/doctrees/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2971 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/_autosummary/mobspy.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4285 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/api.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)  1736636 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2754 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/for_local_use.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4048 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/index.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    26568 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/mobspy.data_handler.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67412 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/mobspy.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   490595 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/mobspy.modules.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16088 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/mobspy.parameter_scripts.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8486 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/mobspy.parameters.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8077 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/mobspy.plot_params.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    86993 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/mobspy.plot_scripts.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    33712 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/mobspy.sbml_simulator.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9059 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/mobspy.simulation_logging.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2767 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/modules.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.185328 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.218000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2407 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/setup.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2439 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/doctrees/test_script.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.271534 mobspy-2.4.0/docs/_build/html/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      230 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/.buildinfo
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.326280 mobspy-2.4.0/docs/_build/html/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41132 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/01_Basic_Intro.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16265 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/02_Reaction_Inheritance.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17425 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/03_Characteristics.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10225 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/04_Characteristic_restriction.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15743 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/05_For_Loops.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14878 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/06_Order_Matters.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23518 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/07_Initial_Condition.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15642 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/08_Units.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23686 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/09_Result_Data.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23178 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/10_Reaction_Rates.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14337 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/11_Looping_Through_Species.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14032 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/12_Born_Species.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    28370 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/13_Events.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18015 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/14_Concatenating_Simulations.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.327803 mobspy-2.4.0/docs/_build/html/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7201 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_autosummary/mobspy.html
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.352791 mobspy-2.4.0/docs/_build/html/_images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_13_Events_11_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_13_Events_1_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_13_Events_4_3.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_13_Events_8_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.378603 mobspy-2.4.0/docs/_build/html/_sources/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.405097 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.406950 mobspy-2.4.0/docs/_build/html/_sources/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/_autosummary/mobspy.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/api.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/for_local_use.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/mobspy.data_handler.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/mobspy.modules.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/mobspy.parameters.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/mobspy.plot_params.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/mobspy.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/mobspy.simulation_logging.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/setup.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_sources/test_script.rst.txt
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.433930 mobspy-2.4.0/docs/_build/html/_static/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4289 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15094 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.436219 mobspy-2.4.0/docs/_build/html/_static/css/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3229 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.510618 mobspy-2.4.0/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    87624 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67312 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    86288 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    66444 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   165742 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   444379 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   165548 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    98024 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    77160 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   323344 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   193308 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   309728 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   184912 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   328412 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   195704 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   309192 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   182708 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   135314 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4472 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/file.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    89501 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.516062 mobspy-2.4.0/docs/_build/html/_static/js/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      934 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4370 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2734 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5023 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4758 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4467 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6861 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/nbsphinx-code-cells.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      584 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/nbsphinx-gallery.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2871 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4902 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18732 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5123 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7627 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/api.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6551 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/for_local_use.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67727 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/genindex.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10018 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/index.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14863 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/mobspy.data_handler.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    91437 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/mobspy.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   178543 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/mobspy.modules.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11761 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/mobspy.parameter_scripts.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8867 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/mobspy.parameters.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8736 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/mobspy.plot_params.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    36208 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/mobspy.plot_scripts.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16526 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/mobspy.sbml_simulator.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9250 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/mobspy.simulation_logging.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23199 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/modules.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8450 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/objects.inv
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17062 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/py-modindex.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6595 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/search.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    96699 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/searchindex.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6464 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/setup.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6500 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/_build/html/test_script.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/api.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1220 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/conf.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/for_local_use.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/index.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      800 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/make.bat
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/mobspy.data_handler.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/mobspy.modules.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/mobspy.parameter_scripts.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/mobspy.parameters.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/mobspy.plot_params.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/mobspy.plot_scripts.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/mobspy.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/mobspy.sbml_simulator.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/mobspy.simulation_logging.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/modules.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/setup.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.0/docs/test_script.rst
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:24.813505 mobspy-2.4.0/example_models/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.538528 mobspy-2.4.0/example_models/Tutorial Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   101374 2024-02-28 22:33:14.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6432 2023-11-22 11:36:42.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7971 2023-11-22 11:38:40.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-04-10 17:13:33.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5458 2023-11-22 12:06:45.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2023-04-10 19:38:34.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9479 2023-11-22 12:08:40.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2023-04-19 15:35:09.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7347 2023-11-22 22:08:58.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    26061 2023-11-22 12:57:35.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4029 2023-11-22 12:58:00.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4498 2023-11-22 13:00:12.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    49256 2023-11-22 13:00:32.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2023-04-21 15:54:19.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.541673 mobspy-2.4.0/example_models/Tutorial Notebooks/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12324 2023-04-19 14:32:18.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/images/Matching_Meta.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   141303 2023-04-09 17:03:35.000000 mobspy-2.4.0/example_models/Tutorial Notebooks/images/vectorial_space.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.557679 mobspy-2.4.0/example_models/application_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      572 2024-01-28 20:43:25.000000 mobspy-2.4.0/example_models/application_models/AB_2CD.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1448 2024-01-28 20:44:42.000000 mobspy-2.4.0/example_models/application_models/AND_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2357 2024-01-28 20:43:25.000000 mobspy-2.4.0/example_models/application_models/CRISPR_Oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1421 2024-01-28 20:47:50.000000 mobspy-2.4.0/example_models/application_models/For_The_Trees.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1291 2024-01-28 20:48:26.000000 mobspy-2.4.0/example_models/application_models/NOR_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1237 2024-01-28 20:47:24.000000 mobspy-2.4.0/example_models/application_models/donor_receptor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1371 2024-01-28 20:48:41.000000 mobspy-2.4.0/example_models/application_models/oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      994 2023-07-07 11:50:03.000000 mobspy-2.4.0/example_models/application_models/positive_phage_feedback_loop.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2917 2024-01-28 20:49:35.000000 mobspy-2.4.0/example_models/application_models/random_walk.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      637 2023-07-05 11:46:34.000000 mobspy-2.4.0/example_models/application_models/simple_infection.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      564 2024-01-28 20:50:18.000000 mobspy-2.4.0/example_models/application_models/simple_repressor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      828 2023-07-05 12:49:47.000000 mobspy-2.4.0/example_models/application_models/simple_rule_based_and_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       63 2024-05-04 20:13:28.000000 mobspy-2.4.0/for_local_use.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.558440 mobspy-2.4.0/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-06-15 12:59:57.000000 mobspy-2.4.0/images/img.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.562796 mobspy-2.4.0/mobspy/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2024-05-04 20:34:54.000000 mobspy-2.4.0/mobspy/_version.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.572392 mobspy-2.4.0/mobspy/data_handler/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/data_handler/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5329 2024-02-28 23:26:14.000000 mobspy-2.4.0/mobspy/data_handler/process_result_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8085 2024-05-02 12:49:07.000000 mobspy-2.4.0/mobspy/data_handler/time_series_object.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.599290 mobspy-2.4.0/mobspy/modules/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/modules/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6945 2024-05-04 20:11:38.000000 mobspy-2.4.0/mobspy/modules/assignments_implementation.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5146 2024-02-25 21:08:54.000000 mobspy-2.4.0/mobspy/modules/class_of_meta_specie_named_any.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1827 2024-02-25 21:10:55.000000 mobspy-2.4.0/mobspy/modules/context_related_scripts.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5110 2023-06-25 17:16:47.000000 mobspy-2.4.0/mobspy/modules/event_functions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12554 2024-02-29 01:47:29.000000 mobspy-2.4.0/mobspy/modules/function_rate_code.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13014 2024-02-26 15:53:24.000000 mobspy-2.4.0/mobspy/modules/logic_operator_objects.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    72570 2024-05-04 14:39:37.000000 mobspy-2.4.0/mobspy/modules/meta_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5240 2023-12-21 15:41:16.000000 mobspy-2.4.0/mobspy/modules/meta_class_utils.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    37827 2024-05-04 14:22:09.000000 mobspy-2.4.0/mobspy/modules/mobspy_expressions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5042 2024-02-26 16:20:28.000000 mobspy-2.4.0/mobspy/modules/mobspy_parameters.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15158 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/modules/order_operators.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17445 2024-02-29 01:46:20.000000 mobspy-2.4.0/mobspy/modules/reaction_construction_nb.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18457 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/modules/reaction_construction_nb_parallel.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4363 2024-02-25 00:46:32.000000 mobspy-2.4.0/mobspy/modules/set_counts_module.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-08-03 14:16:13.000000 mobspy-2.4.0/mobspy/modules/species_string_generator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7765 2024-04-11 13:50:51.000000 mobspy-2.4.0/mobspy/modules/unit_handler.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2024-02-26 16:20:28.000000 mobspy-2.4.0/mobspy/modules/user_functions.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.601779 mobspy-2.4.0/mobspy/parameter_estimation_data_loader/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-02-28 22:21:33.000000 mobspy-2.4.0/mobspy/parameter_estimation_data_loader/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      912 2024-01-31 10:55:41.000000 mobspy-2.4.0/mobspy/parameter_estimation_data_loader/data_loader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7714 2024-04-09 18:34:07.000000 mobspy-2.4.0/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.605215 mobspy-2.4.0/mobspy/parameter_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/parameter_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8401 2024-05-02 12:53:02.000000 mobspy-2.4.0/mobspy/parameter_scripts/parameter_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1957 2024-02-01 12:50:35.000000 mobspy-2.4.0/mobspy/parameter_scripts/parametric_sweeps.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.609373 mobspy-2.4.0/mobspy/parameters/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/parameters/README.md
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/parameters/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1188 2024-01-30 18:15:37.000000 mobspy-2.4.0/mobspy/parameters/default_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1285 2024-01-30 17:59:16.000000 mobspy-2.4.0/mobspy/parameters/example_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.611381 mobspy-2.4.0/mobspy/patch_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-04-09 18:34:07.000000 mobspy-2.4.0/mobspy/patch_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    71177 2024-04-11 13:10:09.000000 mobspy-2.4.0/mobspy/patch_scripts/basico_task_parametrization.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.615193 mobspy-2.4.0/mobspy/plot_params/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/plot_params/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/plot_params/default_plot_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1608 2024-04-11 13:39:08.000000 mobspy-2.4.0/mobspy/plot_params/example_plot_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.623035 mobspy-2.4.0/mobspy/plot_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-03-28 14:29:54.000000 mobspy-2.4.0/mobspy/plot_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9213 2024-05-02 12:53:46.000000 mobspy-2.4.0/mobspy/plot_scripts/default_plots.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17541 2024-04-11 13:55:55.000000 mobspy-2.4.0/mobspy/plot_scripts/hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2482 2024-03-28 14:29:54.000000 mobspy-2.4.0/mobspy/plot_scripts/process_plot_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3885 2024-03-28 14:34:48.000000 mobspy-2.4.0/mobspy/plot_scripts/statistics_calculations.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.628693 mobspy-2.4.0/mobspy/sbml_simulator/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8702 2024-03-20 17:46:34.000000 mobspy-2.4.0/mobspy/sbml_simulator/SBMLWriter.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/sbml_simulator/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.635010 mobspy-2.4.0/mobspy/sbml_simulator/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5705 2024-04-09 18:33:16.000000 mobspy-2.4.0/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      146 2024-04-09 18:33:16.000000 mobspy-2.4.0/mobspy/sbml_simulator/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1040 2024-04-09 18:33:16.000000 mobspy-2.4.0/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8808 2024-04-09 18:33:16.000000 mobspy-2.4.0/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-03-20 17:44:19.000000 mobspy-2.4.0/mobspy/sbml_simulator/builder.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11972 2024-03-20 17:43:06.000000 mobspy-2.4.0/mobspy/sbml_simulator/run.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    39732 2024-05-04 20:33:31.000000 mobspy-2.4.0/mobspy/simulation.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.637429 mobspy-2.4.0/mobspy/simulation_logging/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.0/mobspy/simulation_logging/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      986 2024-05-04 14:29:46.000000 mobspy-2.4.0/mobspy/simulation_logging/log_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.568839 mobspy-2.4.0/mobspy.egg-info/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-04 20:37:23.000000 mobspy-2.4.0/mobspy.egg-info/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16564 2024-05-04 20:37:24.000000 mobspy-2.4.0/mobspy.egg-info/SOURCES.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2024-05-04 20:37:23.000000 mobspy-2.4.0/mobspy.egg-info/dependency_links.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2024-05-04 20:37:23.000000 mobspy-2.4.0/mobspy.egg-info/requires.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2024-05-04 20:37:23.000000 mobspy-2.4.0/mobspy.egg-info/top_level.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-06-15 12:59:57.000000 mobspy-2.4.0/requirements.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2024-05-04 20:37:25.728924 mobspy-2.4.0/setup.cfg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-06-15 12:59:57.000000 mobspy-2.4.0/setup.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.643657 mobspy-2.4.0/test_plot_images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10767 2024-05-04 20:32:18.000000 mobspy-2.4.0/test_plot_images/constant_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    46412 2024-05-04 20:32:18.000000 mobspy-2.4.0/test_plot_images/deterministic_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    53451 2024-05-04 20:32:18.000000 mobspy-2.4.0/test_plot_images/stochastic_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41762 2024-05-04 20:13:28.000000 mobspy-2.4.0/test_script.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-04 20:37:25.724984 mobspy-2.4.0/test_tools/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_1.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      241 2023-06-26 11:54:08.000000 mobspy-2.4.0/test_tools/model_10.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_11.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_12.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_13.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_14.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_15.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_16.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_17.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_18.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_19.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_2.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_20.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_21.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      471 2023-07-03 11:25:39.000000 mobspy-2.4.0/test_tools/model_22.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_23.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_24.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_25.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      518 2023-07-03 11:30:10.000000 mobspy-2.4.0/test_tools/model_26.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_27.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_28.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_29.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_3.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_30.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    55662 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_31.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      129 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_32.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      831 2023-07-03 15:00:26.000000 mobspy-2.4.0/test_tools/model_33.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2023-07-03 23:04:22.000000 mobspy-2.4.0/test_tools/model_34.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       61 2023-07-30 20:48:11.000000 mobspy-2.4.0/test_tools/model_35.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      175 2023-08-01 18:04:20.000000 mobspy-2.4.0/test_tools/model_36.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      391 2023-08-03 14:43:06.000000 mobspy-2.4.0/test_tools/model_37.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1427 2023-08-19 22:03:11.000000 mobspy-2.4.0/test_tools/model_38.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2853 2023-08-19 22:23:06.000000 mobspy-2.4.0/test_tools/model_39.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_4.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-11-15 12:57:45.000000 mobspy-2.4.0/test_tools/model_40.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1412 2023-11-15 12:57:45.000000 mobspy-2.4.0/test_tools/model_41.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      178 2023-11-15 12:57:45.000000 mobspy-2.4.0/test_tools/model_42.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      419 2023-11-17 12:18:00.000000 mobspy-2.4.0/test_tools/model_43.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      197 2024-01-31 16:54:44.000000 mobspy-2.4.0/test_tools/model_44.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8874 2024-02-22 02:44:14.000000 mobspy-2.4.0/test_tools/model_45.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      317 2024-02-24 00:21:58.000000 mobspy-2.4.0/test_tools/model_46.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      243 2024-02-24 13:50:27.000000 mobspy-2.4.0/test_tools/model_47.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      119 2024-05-02 10:01:49.000000 mobspy-2.4.0/test_tools/model_48.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_5.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      389 2023-07-03 10:56:19.000000 mobspy-2.4.0/test_tools/model_6.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1362 2023-07-03 11:02:54.000000 mobspy-2.4.0/test_tools/model_7.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      433 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_8.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-06-15 12:59:57.000000 mobspy-2.4.0/test_tools/model_9.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-06-15 12:59:57.000000 mobspy-2.4.0/useful_parameters.json
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.349417 mobspy-2.4.1/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.879269 mobspy-2.4.1/.github/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.893188 mobspy-2.4.1/.github/workflows/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-06-15 12:59:57.000000 mobspy-2.4.1/.github/workflows/python-app.yml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      415 2024-04-09 17:41:00.000000 mobspy-2.4.1/.gitignore
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1034 2024-02-26 16:22:21.000000 mobspy-2.4.1/.readthedocs.yaml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-06-15 12:59:57.000000 mobspy-2.4.1/LICENSE
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-07 17:51:37.348696 mobspy-2.4.1/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6331 2024-03-08 01:34:03.000000 mobspy-2.4.1/README.md
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.904383 mobspy-2.4.1/docs/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      634 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Makefile
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.918753 mobspy-2.4.1/docs/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.919406 mobspy-2.4.1/docs/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_autosummary/mobspy.rst
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.881056 mobspy-2.4.1/docs/_build/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.945105 mobspy-2.4.1/docs/_build/doctrees/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.958344 mobspy-2.4.1/docs/_build/doctrees/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    95114 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23601 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30820 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/03_Characteristics.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7466 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    24161 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/05_For_Loops.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21599 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    50076 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18699 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/08_Units.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    41471 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/09_Result_Data.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    28500 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15272 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17080 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/12_Born_Species.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    39545 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/13_Events.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15325 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.960093 mobspy-2.4.1/docs/_build/doctrees/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2971 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/_autosummary/mobspy.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4285 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/api.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)  1736636 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2754 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/for_local_use.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4048 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26568 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/mobspy.data_handler.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67412 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/mobspy.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   490595 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/mobspy.modules.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16088 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/mobspy.parameter_scripts.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8486 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/mobspy.parameters.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8077 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/mobspy.plot_params.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    86993 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/mobspy.plot_scripts.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    33712 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/mobspy.sbml_simulator.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9059 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/mobspy.simulation_logging.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2767 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/modules.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.986411 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.000770 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2407 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/setup.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2439 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/doctrees/test_script.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.032481 mobspy-2.4.1/docs/_build/html/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      230 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/.buildinfo
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.066168 mobspy-2.4.1/docs/_build/html/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    41132 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/01_Basic_Intro.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16265 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/02_Reaction_Inheritance.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17425 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/03_Characteristics.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10225 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/04_Characteristic_restriction.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15743 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/05_For_Loops.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14878 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/06_Order_Matters.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23518 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/07_Initial_Condition.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15642 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/08_Units.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23686 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/09_Result_Data.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23178 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/10_Reaction_Rates.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14337 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/11_Looping_Through_Species.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14032 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/12_Born_Species.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    28370 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/13_Events.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18015 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/14_Concatenating_Simulations.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.067031 mobspy-2.4.1/docs/_build/html/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7201 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_autosummary/mobspy.html
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.085374 mobspy-2.4.1/docs/_build/html/_images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_13_Events_11_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_13_Events_1_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_13_Events_4_3.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_13_Events_8_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.102395 mobspy-2.4.1/docs/_build/html/_sources/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.123196 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.124997 mobspy-2.4.1/docs/_build/html/_sources/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/_autosummary/mobspy.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/api.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/for_local_use.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/mobspy.data_handler.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/mobspy.modules.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/mobspy.parameters.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/mobspy.plot_params.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/mobspy.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/mobspy.simulation_logging.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/setup.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_sources/test_script.rst.txt
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.143844 mobspy-2.4.1/docs/_build/html/_static/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4289 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15094 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.145627 mobspy-2.4.1/docs/_build/html/_static/css/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3229 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.193567 mobspy-2.4.1/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    87624 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67312 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    86288 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    66444 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   165742 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   444379 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   165548 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    98024 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    77160 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   323344 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   193308 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   309728 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   184912 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   328412 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   195704 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   309192 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   182708 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   135314 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4472 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    89501 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.198408 mobspy-2.4.1/docs/_build/html/_static/js/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      934 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4370 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2734 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5023 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4758 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4467 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6861 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/nbsphinx-code-cells.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      584 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/nbsphinx-gallery.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2871 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4902 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18732 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5123 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7627 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/api.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6551 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/for_local_use.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67727 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/genindex.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10018 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/index.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14863 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/mobspy.data_handler.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    91437 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/mobspy.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   178543 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/mobspy.modules.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11761 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/mobspy.parameter_scripts.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8867 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/mobspy.parameters.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8736 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/mobspy.plot_params.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    36208 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/mobspy.plot_scripts.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16526 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/mobspy.sbml_simulator.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9250 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/mobspy.simulation_logging.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23199 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/modules.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8450 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/objects.inv
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17062 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/py-modindex.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6595 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/search.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    96699 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/searchindex.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6464 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/setup.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6500 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/_build/html/test_script.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/api.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1220 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/conf.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/for_local_use.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/index.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      800 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/make.bat
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/mobspy.data_handler.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/mobspy.modules.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/mobspy.parameter_scripts.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/mobspy.parameters.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/mobspy.plot_params.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/mobspy.plot_scripts.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/mobspy.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/mobspy.sbml_simulator.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/mobspy.simulation_logging.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/modules.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/setup.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.1/docs/test_script.rst
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:36.883563 mobspy-2.4.1/example_models/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.215663 mobspy-2.4.1/example_models/Tutorial Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   132826 2024-05-05 13:25:04.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6793 2024-05-05 18:27:41.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8153 2024-05-05 20:46:30.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3725 2024-05-06 09:21:49.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5464 2024-05-06 12:26:05.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8168 2024-05-06 13:31:40.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9479 2023-11-22 12:08:40.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2023-04-19 15:35:09.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7347 2023-11-22 22:08:58.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26061 2023-11-22 12:57:35.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4029 2023-11-22 12:58:00.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4498 2023-11-22 13:00:12.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    49256 2023-11-22 13:00:32.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2023-04-21 15:54:19.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.218034 mobspy-2.4.1/example_models/Tutorial Notebooks/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12324 2023-04-19 14:32:18.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/images/Matching_Meta.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   141303 2023-04-09 17:03:35.000000 mobspy-2.4.1/example_models/Tutorial Notebooks/images/vectorial_space.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.231038 mobspy-2.4.1/example_models/application_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      572 2024-01-28 20:43:25.000000 mobspy-2.4.1/example_models/application_models/AB_2CD.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1448 2024-01-28 20:44:42.000000 mobspy-2.4.1/example_models/application_models/AND_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2357 2024-01-28 20:43:25.000000 mobspy-2.4.1/example_models/application_models/CRISPR_Oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1447 2024-05-07 17:47:59.000000 mobspy-2.4.1/example_models/application_models/For_The_Trees.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1291 2024-01-28 20:48:26.000000 mobspy-2.4.1/example_models/application_models/NOR_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1237 2024-01-28 20:47:24.000000 mobspy-2.4.1/example_models/application_models/donor_receptor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1371 2024-01-28 20:48:41.000000 mobspy-2.4.1/example_models/application_models/oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      994 2023-07-07 11:50:03.000000 mobspy-2.4.1/example_models/application_models/positive_phage_feedback_loop.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2917 2024-01-28 20:49:35.000000 mobspy-2.4.1/example_models/application_models/random_walk.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      637 2023-07-05 11:46:34.000000 mobspy-2.4.1/example_models/application_models/simple_infection.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      564 2024-01-28 20:50:18.000000 mobspy-2.4.1/example_models/application_models/simple_repressor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      828 2023-07-05 12:49:47.000000 mobspy-2.4.1/example_models/application_models/simple_rule_based_and_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      307 2024-05-07 12:20:54.000000 mobspy-2.4.1/for_local_use.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.232211 mobspy-2.4.1/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-06-15 12:59:57.000000 mobspy-2.4.1/images/img.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.235684 mobspy-2.4.1/mobspy/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2024-05-07 17:49:48.000000 mobspy-2.4.1/mobspy/_version.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.241678 mobspy-2.4.1/mobspy/data_handler/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/data_handler/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5759 2024-05-07 13:05:25.000000 mobspy-2.4.1/mobspy/data_handler/process_result_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8085 2024-05-02 12:49:07.000000 mobspy-2.4.1/mobspy/data_handler/time_series_object.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.262838 mobspy-2.4.1/mobspy/modules/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/modules/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6945 2024-05-04 20:11:38.000000 mobspy-2.4.1/mobspy/modules/assignments_implementation.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5146 2024-02-25 21:08:54.000000 mobspy-2.4.1/mobspy/modules/class_of_meta_specie_named_any.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1827 2024-02-25 21:10:55.000000 mobspy-2.4.1/mobspy/modules/context_related_scripts.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5110 2023-06-25 17:16:47.000000 mobspy-2.4.1/mobspy/modules/event_functions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12554 2024-02-29 01:47:29.000000 mobspy-2.4.1/mobspy/modules/function_rate_code.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13014 2024-02-26 15:53:24.000000 mobspy-2.4.1/mobspy/modules/logic_operator_objects.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    72570 2024-05-04 14:39:37.000000 mobspy-2.4.1/mobspy/modules/meta_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5240 2023-12-21 15:41:16.000000 mobspy-2.4.1/mobspy/modules/meta_class_utils.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    37827 2024-05-04 14:22:09.000000 mobspy-2.4.1/mobspy/modules/mobspy_expressions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5042 2024-02-26 16:20:28.000000 mobspy-2.4.1/mobspy/modules/mobspy_parameters.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15158 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/modules/order_operators.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17445 2024-02-29 01:46:20.000000 mobspy-2.4.1/mobspy/modules/reaction_construction_nb.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18457 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/modules/reaction_construction_nb_parallel.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4363 2024-02-25 00:46:32.000000 mobspy-2.4.1/mobspy/modules/set_counts_module.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-08-03 14:16:13.000000 mobspy-2.4.1/mobspy/modules/species_string_generator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7765 2024-04-11 13:50:51.000000 mobspy-2.4.1/mobspy/modules/unit_handler.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2024-02-26 16:20:28.000000 mobspy-2.4.1/mobspy/modules/user_functions.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.264891 mobspy-2.4.1/mobspy/parameter_estimation_data_loader/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-02-28 22:21:33.000000 mobspy-2.4.1/mobspy/parameter_estimation_data_loader/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      912 2024-01-31 10:55:41.000000 mobspy-2.4.1/mobspy/parameter_estimation_data_loader/data_loader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7714 2024-04-09 18:34:07.000000 mobspy-2.4.1/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.267638 mobspy-2.4.1/mobspy/parameter_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/parameter_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8401 2024-05-02 12:53:02.000000 mobspy-2.4.1/mobspy/parameter_scripts/parameter_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1957 2024-02-01 12:50:35.000000 mobspy-2.4.1/mobspy/parameter_scripts/parametric_sweeps.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.270811 mobspy-2.4.1/mobspy/parameters/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/parameters/README.md
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/parameters/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1188 2024-01-30 18:15:37.000000 mobspy-2.4.1/mobspy/parameters/default_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1285 2024-01-30 17:59:16.000000 mobspy-2.4.1/mobspy/parameters/example_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.271974 mobspy-2.4.1/mobspy/patch_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-04-09 18:34:07.000000 mobspy-2.4.1/mobspy/patch_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    71233 2024-05-05 13:14:45.000000 mobspy-2.4.1/mobspy/patch_scripts/basico_task_parametrization.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.275431 mobspy-2.4.1/mobspy/plot_params/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/plot_params/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2024-05-06 14:50:24.000000 mobspy-2.4.1/mobspy/plot_params/default_plot_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1682 2024-05-06 14:53:26.000000 mobspy-2.4.1/mobspy/plot_params/example_plot_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.279997 mobspy-2.4.1/mobspy/plot_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-03-28 14:29:54.000000 mobspy-2.4.1/mobspy/plot_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10975 2024-05-07 17:42:50.000000 mobspy-2.4.1/mobspy/plot_scripts/default_plots.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17947 2024-05-07 13:15:06.000000 mobspy-2.4.1/mobspy/plot_scripts/hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2483 2024-05-07 13:17:04.000000 mobspy-2.4.1/mobspy/plot_scripts/process_plot_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3885 2024-03-28 14:34:48.000000 mobspy-2.4.1/mobspy/plot_scripts/statistics_calculations.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.283141 mobspy-2.4.1/mobspy/sbml_simulator/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8702 2024-03-20 17:46:34.000000 mobspy-2.4.1/mobspy/sbml_simulator/SBMLWriter.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/sbml_simulator/__init__.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.287190 mobspy-2.4.1/mobspy/sbml_simulator/__pycache__/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5705 2024-04-09 18:33:16.000000 mobspy-2.4.1/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      146 2024-04-09 18:33:16.000000 mobspy-2.4.1/mobspy/sbml_simulator/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1040 2024-04-09 18:33:16.000000 mobspy-2.4.1/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8808 2024-04-09 18:33:16.000000 mobspy-2.4.1/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-03-20 17:44:19.000000 mobspy-2.4.1/mobspy/sbml_simulator/builder.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11972 2024-03-20 17:43:06.000000 mobspy-2.4.1/mobspy/sbml_simulator/run.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    40003 2024-05-07 12:03:53.000000 mobspy-2.4.1/mobspy/simulation.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.288494 mobspy-2.4.1/mobspy/simulation_logging/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.1/mobspy/simulation_logging/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      986 2024-05-04 14:29:46.000000 mobspy-2.4.1/mobspy/simulation_logging/log_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.239857 mobspy-2.4.1/mobspy.egg-info/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-07 17:51:36.000000 mobspy-2.4.1/mobspy.egg-info/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16564 2024-05-07 17:51:36.000000 mobspy-2.4.1/mobspy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2024-05-07 17:51:36.000000 mobspy-2.4.1/mobspy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2024-05-07 17:51:36.000000 mobspy-2.4.1/mobspy.egg-info/requires.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2024-05-07 17:51:36.000000 mobspy-2.4.1/mobspy.egg-info/top_level.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-06-15 12:59:57.000000 mobspy-2.4.1/requirements.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2024-05-07 17:51:37.349903 mobspy-2.4.1/setup.cfg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-06-15 12:59:57.000000 mobspy-2.4.1/setup.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.292107 mobspy-2.4.1/test_plot_images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10767 2024-05-07 17:43:41.000000 mobspy-2.4.1/test_plot_images/constant_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    46264 2024-05-07 17:43:41.000000 mobspy-2.4.1/test_plot_images/deterministic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    55545 2024-05-07 17:43:41.000000 mobspy-2.4.1/test_plot_images/stochastic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    41762 2024-05-04 20:13:28.000000 mobspy-2.4.1/test_script.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-07 17:51:37.346791 mobspy-2.4.1/test_tools/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_1.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      241 2023-06-26 11:54:08.000000 mobspy-2.4.1/test_tools/model_10.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_11.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_12.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_13.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_14.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_15.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_16.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_17.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_18.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_19.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_2.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_20.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_21.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      471 2023-07-03 11:25:39.000000 mobspy-2.4.1/test_tools/model_22.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_23.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_24.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_25.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      518 2023-07-03 11:30:10.000000 mobspy-2.4.1/test_tools/model_26.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_27.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_28.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_29.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_3.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_30.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    55662 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_31.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      129 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_32.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      831 2023-07-03 15:00:26.000000 mobspy-2.4.1/test_tools/model_33.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2023-07-03 23:04:22.000000 mobspy-2.4.1/test_tools/model_34.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       61 2023-07-30 20:48:11.000000 mobspy-2.4.1/test_tools/model_35.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      175 2023-08-01 18:04:20.000000 mobspy-2.4.1/test_tools/model_36.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      391 2023-08-03 14:43:06.000000 mobspy-2.4.1/test_tools/model_37.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1427 2023-08-19 22:03:11.000000 mobspy-2.4.1/test_tools/model_38.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2853 2023-08-19 22:23:06.000000 mobspy-2.4.1/test_tools/model_39.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_4.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-11-15 12:57:45.000000 mobspy-2.4.1/test_tools/model_40.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1412 2023-11-15 12:57:45.000000 mobspy-2.4.1/test_tools/model_41.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      178 2023-11-15 12:57:45.000000 mobspy-2.4.1/test_tools/model_42.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      419 2023-11-17 12:18:00.000000 mobspy-2.4.1/test_tools/model_43.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      197 2024-01-31 16:54:44.000000 mobspy-2.4.1/test_tools/model_44.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8874 2024-02-22 02:44:14.000000 mobspy-2.4.1/test_tools/model_45.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      317 2024-02-24 00:21:58.000000 mobspy-2.4.1/test_tools/model_46.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      243 2024-02-24 13:50:27.000000 mobspy-2.4.1/test_tools/model_47.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      119 2024-05-02 10:01:49.000000 mobspy-2.4.1/test_tools/model_48.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_5.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      389 2023-07-03 10:56:19.000000 mobspy-2.4.1/test_tools/model_6.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1362 2023-07-03 11:02:54.000000 mobspy-2.4.1/test_tools/model_7.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      433 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_8.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-06-15 12:59:57.000000 mobspy-2.4.1/test_tools/model_9.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-06-15 12:59:57.000000 mobspy-2.4.1/useful_parameters.json
```

### Comparing `mobspy-2.4.0/.github/workflows/python-app.yml` & `mobspy-2.4.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/.readthedocs.yaml` & `mobspy-2.4.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/LICENSE` & `mobspy-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/PKG-INFO` & `mobspy-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.4.0
+Version: 2.4.1
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.4.0/README.md` & `mobspy-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Makefile` & `mobspy-2.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.1/docs/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.1/docs/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.1/docs/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.1/docs/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.1/docs/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.1/docs/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.1/docs/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/08_Units.ipynb` & `mobspy-2.4.1/docs/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.1/docs/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.1/docs/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.1/docs/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.1/docs/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/13_Events.ipynb` & `mobspy-2.4.1/docs/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.1/docs/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/03_Characteristics.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/03_Characteristics.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/05_For_Loops.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/05_For_Loops.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/08_Units.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/08_Units.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/09_Result_Data.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/09_Result_Data.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/12_Born_Species.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/12_Born_Species.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/13_Events.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/13_Events.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree` & `mobspy-2.4.1/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/_autosummary/mobspy.doctree` & `mobspy-2.4.1/docs/_build/doctrees/_autosummary/mobspy.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/api.doctree` & `mobspy-2.4.1/docs/_build/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/environment.pickle` & `mobspy-2.4.1/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/for_local_use.doctree` & `mobspy-2.4.1/docs/_build/doctrees/for_local_use.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/index.doctree` & `mobspy-2.4.1/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/mobspy.data_handler.doctree` & `mobspy-2.4.1/docs/_build/doctrees/mobspy.data_handler.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/mobspy.doctree` & `mobspy-2.4.1/docs/_build/doctrees/mobspy.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/mobspy.modules.doctree` & `mobspy-2.4.1/docs/_build/doctrees/mobspy.modules.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/mobspy.parameter_scripts.doctree` & `mobspy-2.4.1/docs/_build/doctrees/mobspy.parameter_scripts.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/mobspy.parameters.doctree` & `mobspy-2.4.1/docs/_build/doctrees/mobspy.parameters.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/mobspy.plot_params.doctree` & `mobspy-2.4.1/docs/_build/doctrees/mobspy.plot_params.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/mobspy.plot_scripts.doctree` & `mobspy-2.4.1/docs/_build/doctrees/mobspy.plot_scripts.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/mobspy.sbml_simulator.doctree` & `mobspy-2.4.1/docs/_build/doctrees/mobspy.sbml_simulator.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/mobspy.simulation_logging.doctree` & `mobspy-2.4.1/docs/_build/doctrees/mobspy.simulation_logging.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/modules.doctree` & `mobspy-2.4.1/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png` & `mobspy-2.4.1/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/setup.doctree` & `mobspy-2.4.1/docs/_build/doctrees/setup.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/doctrees/test_script.doctree` & `mobspy-2.4.1/docs/_build/doctrees/test_script.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/01_Basic_Intro.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/01_Basic_Intro.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/02_Reaction_Inheritance.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/02_Reaction_Inheritance.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/03_Characteristics.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/03_Characteristics.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/04_Characteristic_restriction.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/04_Characteristic_restriction.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/05_For_Loops.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/05_For_Loops.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/06_Order_Matters.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/06_Order_Matters.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/07_Initial_Condition.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/07_Initial_Condition.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/08_Units.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/08_Units.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/08_Units.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/09_Result_Data.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/09_Result_Data.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/10_Reaction_Rates.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/10_Reaction_Rates.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/11_Looping_Through_Species.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/11_Looping_Through_Species.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/12_Born_Species.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/12_Born_Species.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/13_Events.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/13_Events.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/13_Events.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/14_Concatenating_Simulations.html` & `mobspy-2.4.1/docs/_build/html/Notebooks/14_Concatenating_Simulations.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.1/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_autosummary/mobspy.html` & `mobspy-2.4.1/docs/_build/html/_autosummary/mobspy.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_13_Events_11_2.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_13_Events_11_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_13_Events_1_2.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_13_Events_1_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_13_Events_4_3.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_13_Events_4_3.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_13_Events_8_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_13_Events_8_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png` & `mobspy-2.4.1/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt` & `mobspy-2.4.1/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/index.rst.txt` & `mobspy-2.4.1/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/mobspy.data_handler.rst.txt` & `mobspy-2.4.1/docs/_build/html/_sources/mobspy.data_handler.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/mobspy.modules.rst.txt` & `mobspy-2.4.1/docs/_build/html/_sources/mobspy.modules.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt` & `mobspy-2.4.1/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/mobspy.parameters.rst.txt` & `mobspy-2.4.1/docs/_build/html/_sources/mobspy.parameters.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/mobspy.plot_params.rst.txt` & `mobspy-2.4.1/docs/_build/html/_sources/mobspy.plot_params.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt` & `mobspy-2.4.1/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/mobspy.rst.txt` & `mobspy-2.4.1/docs/_build/html/_sources/mobspy.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt` & `mobspy-2.4.1/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `mobspy-2.4.1/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/basic.css` & `mobspy-2.4.1/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/badge_only.css` & `mobspy-2.4.1/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-bold.woff` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-normal.woff` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `mobspy-2.4.1/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/css/theme.css` & `mobspy-2.4.1/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/doctools.js` & `mobspy-2.4.1/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/jquery.js` & `mobspy-2.4.1/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/js/badge_only.js` & `mobspy-2.4.1/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `mobspy-2.4.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/js/html5shiv.min.js` & `mobspy-2.4.1/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/js/theme.js` & `mobspy-2.4.1/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/language_data.js` & `mobspy-2.4.1/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg` & `mobspy-2.4.1/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/nbsphinx-code-cells.css` & `mobspy-2.4.1/docs/_build/html/_static/nbsphinx-code-cells.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/nbsphinx-gallery.css` & `mobspy-2.4.1/docs/_build/html/_static/nbsphinx-gallery.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/nbsphinx-no-thumbnail.svg` & `mobspy-2.4.1/docs/_build/html/_static/nbsphinx-no-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/pygments.css` & `mobspy-2.4.1/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/searchtools.js` & `mobspy-2.4.1/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/_static/sphinx_highlight.js` & `mobspy-2.4.1/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/api.html` & `mobspy-2.4.1/docs/_build/html/api.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/for_local_use.html` & `mobspy-2.4.1/docs/_build/html/for_local_use.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/genindex.html` & `mobspy-2.4.1/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/index.html` & `mobspy-2.4.1/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/mobspy.data_handler.html` & `mobspy-2.4.1/docs/_build/html/mobspy.data_handler.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/mobspy.html` & `mobspy-2.4.1/docs/_build/html/mobspy.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/mobspy.modules.html` & `mobspy-2.4.1/docs/_build/html/mobspy.modules.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/mobspy.parameter_scripts.html` & `mobspy-2.4.1/docs/_build/html/mobspy.parameter_scripts.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/mobspy.parameters.html` & `mobspy-2.4.1/docs/_build/html/mobspy.parameters.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/mobspy.plot_params.html` & `mobspy-2.4.1/docs/_build/html/mobspy.plot_params.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/mobspy.plot_scripts.html` & `mobspy-2.4.1/docs/_build/html/mobspy.plot_scripts.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/mobspy.sbml_simulator.html` & `mobspy-2.4.1/docs/_build/html/mobspy.sbml_simulator.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/mobspy.simulation_logging.html` & `mobspy-2.4.1/docs/_build/html/mobspy.simulation_logging.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/modules.html` & `mobspy-2.4.1/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/objects.inv` & `mobspy-2.4.1/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/py-modindex.html` & `mobspy-2.4.1/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/search.html` & `mobspy-2.4.1/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/searchindex.js` & `mobspy-2.4.1/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/setup.html` & `mobspy-2.4.1/docs/_build/html/setup.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/_build/html/test_script.html` & `mobspy-2.4.1/docs/_build/html/test_script.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/conf.py` & `mobspy-2.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/index.rst` & `mobspy-2.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/make.bat` & `mobspy-2.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/mobspy.data_handler.rst` & `mobspy-2.4.1/docs/mobspy.data_handler.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/mobspy.modules.rst` & `mobspy-2.4.1/docs/mobspy.modules.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/mobspy.parameter_scripts.rst` & `mobspy-2.4.1/docs/mobspy.parameter_scripts.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/mobspy.parameters.rst` & `mobspy-2.4.1/docs/mobspy.parameters.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/mobspy.plot_params.rst` & `mobspy-2.4.1/docs/mobspy.plot_params.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/mobspy.plot_scripts.rst` & `mobspy-2.4.1/docs/mobspy.plot_scripts.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/mobspy.rst` & `mobspy-2.4.1/docs/mobspy.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/docs/mobspy.sbml_simulator.rst` & `mobspy-2.4.1/docs/mobspy.sbml_simulator.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954427083333333%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'In MobsPy, meta-species can be used to create new "*

 * *            'meta-species, and the new meta-species receive all reactions defined for the ones '*

 * *            "used to make them. \\n'), (3, 'This concept is called reaction inheritance. \\n'), "*

 * *            "(5, 'We present an example of inheritance starting by defining several "*

 * *            "BaseSpecies:')], delete: [4, 2]}}, 1: {'source': {insert: [(2, 'Duplicator, Mortal, "*

 * *            "Eater, Food = BaseSpecie […]*

```diff
@@ -3,50 +3,51 @@
         {
             "cell_type": "markdown",
             "id": "8718382c-245b-472d-9346-560baf8ea4c9",
             "metadata": {},
             "source": [
                 "# Reaction Inheritance\n",
                 "\n",
-                "MobsPy allows Meta-Species to inherit reactions from other Meta-Species\n",
+                "In MobsPy, meta-species can be used to create new meta-species, and the new meta-species receive all reactions defined for the ones used to make them. \n",
+                "This concept is called reaction inheritance. \n",
                 "\n",
-                "We start by defining the BaseSpecies we will use:"
+                "We present an example of inheritance starting by defining several BaseSpecies:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "115322c4-e3a8-4a0b-9d38-8d0d26c4c79b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from mobspy import *\n",
                 "\n",
-                "Duplicator, Mortal, Eater, Food = BaseSpecies(4)"
+                "Duplicator, Mortal, Eater, Food = BaseSpecies()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bd283d31-7e59-4f4c-84e4-bb379fcbcb6a",
             "metadata": {},
             "source": [
-                "Next, we define the reactions for each of the BaseSpecies.\n",
-                "Zero is a meta-species that represents no species."
+                "Next, we define reactions for the BaseSpecies.\n",
+                "Furthermore, Zero, a meta-species that appears in these reactions, is a meta-species made available by the MobsPy to represent nothing."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "f9687e7a-abc5-4fde-a61c-aa8b6a2e8181",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7f885d9a8070>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7fda25321c70>"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -57,16 +58,18 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "857582f8-7b9c-4ae2-b7e8-ef4c83f3af0a",
             "metadata": {},
             "source": [
-                "In MobsPy, the multiplication of meta-species allows for the inheritance of reactions from the factor species.\n",
-                "For example, we would like to define a Bacteria species that is also a Duplicator, an Eater, and a Mortal. This is done via:"
+                "There are two ways of creating new meta-species with other meta-species.\u00a0\n",
+                "The first one is to multiple meta-species.\n",
+                "The product of this multiplication is a new meta-species that inherits from all the factors in this multiplication.\u00a0\n",
+                "Below, we show an example where we define Bacteria, a species that is also a Duplicator, an Eater, and a Mortal:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "43d91f12-5c95-4789-b10d-ef88c0d02f74",
             "metadata": {},
@@ -86,15 +89,15 @@
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "2fc1888a-bbd9-431f-95fd-34b62f4865dd",
             "metadata": {},
             "outputs": [],
             "source": [
-                "Ecoli, Strepto = New(Bacteria, 2)"
+                "Ecoli, Strepto = New(Bacteria)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d4ac10e7-ccbf-4d3c-b02a-1966af2fed5d",
             "metadata": {},
             "source": [
@@ -104,15 +107,15 @@
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "30df3ac6-f019-43f0-87ae-c50beab9b0da",
             "metadata": {},
             "outputs": [],
             "source": [
-                "Glucose, Amino = New(Food, 2)"
+                "Glucose, Amino = New(Food)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4d291352-6fee-4d98-9c39-b469df6d3042",
             "metadata": {},
             "source": [
@@ -127,18 +130,18 @@
             "execution_count": 6,
             "id": "5f0c9765-b7d0-4e26-98ed-8660fcd74f26",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(<mobspy.modules.meta_class.Species at 0x7f885d8d6bb0>,\n",
-                            " <mobspy.modules.meta_class.Species at 0x7f88569a3100>,\n",
-                            " <mobspy.modules.meta_class.Species at 0x7f885697dd00>,\n",
-                            " <mobspy.modules.meta_class.Species at 0x7f885d8d6e50>)"
+                            "(<mobspy.modules.meta_class.Species at 0x7fda1f179d90>,\n",
+                            " <mobspy.modules.meta_class.Species at 0x7fda1f19f670>,\n",
+                            " <mobspy.modules.meta_class.Species at 0x7fda25321940>,\n",
+                            " <mobspy.modules.meta_class.Species at 0x7fda25321910>)"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/03_Characteristics.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735460069444445%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'Characteristics are the units combined to generate "*

 * *            "meta-species states. \\n'), (3, 'They allow for the construction of reactions through "*

 * *            "queries in both the products and the reactants. \\n'), (5, 'Characteristics can be "*

 * *            "added using the dot operator to a meta-species.\\n'), (6, 'They can be added "*

 * *            'implicitly inside a reaction and explicitly outside of one. When added implicitly, '*

 * *            'the characteri […]*

```diff
@@ -3,110 +3,100 @@
         {
             "cell_type": "markdown",
             "id": "dbac9fd1-6de0-4b42-bc80-9e0c98d7515a",
             "metadata": {},
             "source": [
                 "# Characteristics\n",
                 "\n",
-                "MobsPy can also add characteristics to species and construct reactions based on these characteristics by a querying mechanism. In this example, we describe the characteristic mechanism in detail \n",
+                "Characteristics are the units combined to generate meta-species states. \n",
+                "They allow for the construction of reactions through queries in both the products and the reactants. \n",
                 "\n",
-                "First we define 2 BaseSpecies:"
+                "Characteristics can be added using the dot operator to a meta-species.\n",
+                "They can be added implicitly inside a reaction and explicitly outside of one. When added implicitly, the characteristics will automatically partake in the reaction. An example follows: "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "5ed4381b-a079-44be-8183-21ca30e0adb5",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from mobspy import *\n",
-                "\n",
-                "Age, Color = BaseSpecies(2)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "08d2ba60-b2e3-406f-91ef-5c212c0e0cd9",
-            "metadata": {},
-            "source": [
-                "Characteristics can be added using the dot operator to a meta-species in the first time it is called. They can be added implicitly inside a reaction and explicitly outside a reaction. When added explicitly, the characteristics will automatically partake in the reaction. An example follows:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 2,
             "id": "8a97e372-3f01-40f2-b3fc-c2309ba74efa",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fc7b5180f10>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7f9367aa3580>"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "from mobspy import *\n",
+                "\n",
+                "Age, Color = BaseSpecies()\n",
+                "\n",
                 "Color.blue, Color.red, Color.yellow\n",
                 "Age.young >> Age.old [1]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bbf5bfc3-cd90-492c-a5a2-a0f47d22f689",
             "metadata": {},
             "source": [
-                "We next multiply Age and Color to create a Dummy meta-species. The new meta-species inherit the characteristics of Color and Age. It inherits them as a two-dimensional vector space with orthogonal characteristic sets.\n",
-                "The Dummy meta-species represents all the possible combinations of characteristics from the meta-species it inherits from, separated by a dot. As an example, Dummy can be in the following states:\n",
-                "\n",
-                "Dummy.blue.young, \\\n",
-                "Dummy.blue.old, \\\n",
-                "Dummy.red.young, \\\n",
-                "Dummy.red.old, \\\n",
-                "Dummy.yellow.young, \\\n",
-                "Dummy.yellow.old"
+                "We now multiply Age and Color to create a Dummy meta-species that inherits from both of them. \n",
+                "In MobsPy, inheritance is not only for reactions but also for characteristics. \n",
+                "Thus, the Dummy meta-species will inherit all of the characteristics from the meta-species used to create it. \n",
+                "Further, the states of the meta-species are constructed using all possible orthogonal combinations of characteristics coming from different inheritors."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "id": "cf2fc33f-e028-4090-9f35-c3a8f6a6fc33",
             "metadata": {},
             "outputs": [],
             "source": [
                 "Dummy = Age*Color"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "71980e63-98e4-4190-a615-a243ec772079",
             "metadata": {},
             "source": [
+                "The Dummy meta-species can be in the following states:\n",
+                "\n",
+                "Dummy.blue.young, \\\n",
+                "Dummy.blue.old, \\\n",
+                "Dummy.red.young, \\\n",
+                "Dummy.red.old, \\\n",
+                "Dummy.yellow.young, \\\n",
+                "Dummy.yellow.old\n",
+                "\n",
                 "One can query the meta-species that Dummy represents using characteristics.\n",
                 "If the query is present on a reactant, it filters through the states that do not possess the requested characteristic.\n",
                 "As an example, the meta-reaction:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "id": "21118e41-f9f2-478b-bd73-9cf6ce5d4646",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fc7b51a6130>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7f9367a42220>"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "Dummy.old >> Zero [1]"
             ]
@@ -124,44 +114,48 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "366c3b80-97d9-44d3-8c07-0e7e1f4fb7a5",
             "metadata": {},
             "source": [
-                "One can also perform a query in the products. When performed in the products, the query specifies in which space one wishes the transformation to occur. For instance, the meta-reaction: "
+                "One can also perform a query in the products. When performed in the products, the query specifies in which characteristics space one wishes the transformation to occur. \n",
+                "Characteristic spaces are spaces shared by characteristics coming from the same inheritor, with the spaces being defined by the characteristics that were initially added to that species. \n",
+                "The Dummy meta species also has an empty characteristic space, as it obtained all its characteristics from inheritance.\n",
+                "\n",
+                "As an example, the meta-reaction: "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "id": "96ceda1e-c397-4e01-a815-bc7a262d2619",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fc7b51a6400>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7f9367aae070>"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "Dummy >> Dummy.blue [1]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f294a057-6ab7-4b44-8b0f-7901c3f4deae",
             "metadata": {},
             "source": [
-                "Defines the following reactions:\n",
+                "Uses the characteristic space of meta-species Color to define the following reactions:\n",
                 "\n",
                 "Dummy.red.young -> Dummy.blue.young \\\n",
                 "Dummy.red.old -> Dummy.blue.old \\\n",
                 "Dummy.blue.young -> Dummy.blue.young \\\n",
                 "Dummy.blue.old -> Dummy.blue.old \\\n",
                 "Dummy.yellow.young -> Dummy.blue.young \\\n",
                 "Dummy.yellow.old -> Dummy.blue.old\n",
@@ -171,15 +165,15 @@
                 "It is also possible to query over multiple characteristics at the same time, and the order is irrelevant.\n",
                 "\n",
                 "We finish by compiling the model to visualize all the reactions in detail:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "id": "4e3d95b8-ec1a-4969-87a0-93b39a421160",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
```

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/05_For_Loops.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957142857142858%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'Here, we discuss the proper way of using MobsPy to "*

 * *            "perform queries inside for loops.\\n'), (4, 'We start by giving an example of what "*

 * *            "not to do. Below, we wish to define a model that cycles through different colors:')], "*

 * *            "delete: [4, 2]}}, 2: {'source': {insert: [(0, 'Since Python resolves Color.c1 by "*

 * *            'adding the characteristic c1 to Color, this loop adds the same reaction three times '*

 * *            'to the Co […]*

```diff
@@ -3,17 +3,17 @@
         {
             "cell_type": "markdown",
             "id": "b9393853-5359-4ab2-991c-4e8b07e842de",
             "metadata": {},
             "source": [
                 "# For Loops\n",
                 "\n",
-                "Here we discuss the proper way of using MobsPy to perform queries inside for loops.\n",
+                "Here, we discuss the proper way of using MobsPy to perform queries inside for loops.\n",
                 "\n",
-                "We start by giving an example of what not to do. Here we wish to define a model that cycles through different colors."
+                "We start by giving an example of what not to do. Below, we wish to define a model that cycles through different colors:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "09b7f076-20c3-4dd2-83fa-a6abeeb25ebb",
             "metadata": {},
@@ -94,17 +94,17 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "76c9e058-6801-489f-8788-ad8d8f57efe4",
             "metadata": {},
             "source": [
-                "Since Python resolves Color.c1 by adding the characteristic c1 to Color, this loop adds the same reaction three times to the Color meta-species. Furthermore, the characteristics added are wrong. We wish to add the actual colors, not c1 and c2, which have been used for looping over the colors list. \n",
+                "Since Python resolves Color.c1 by adding the characteristic c1 to Color, this loop adds the same reaction three times to the Color meta-species. Furthermore, the characteristics added are the wrong ones. We wish to add the actual colors, not c1 and c2, which were used for looping over the colors list. \n",
                 "\n",
-                "To perform a query over the value of a stored variable and not it's name, one can use the .c() method. The corrected version of the model follows:"
+                "To perform a query over the value of a stored variable and not its name, one can use the .c() method. The corrected version of the model follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "f189db7a-b3fd-4175-b9c1-6ad69e393698",
             "metadata": {},
```

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/08_Units.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/13_Events.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.1/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/images/Matching_Meta.png` & `mobspy-2.4.1/example_models/Tutorial Notebooks/images/Matching_Meta.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/Tutorial Notebooks/images/vectorial_space.png` & `mobspy-2.4.1/example_models/Tutorial Notebooks/images/vectorial_space.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/AB_2CD.py` & `mobspy-2.4.1/example_models/application_models/AB_2CD.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/AND_gate.py` & `mobspy-2.4.1/example_models/application_models/AND_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/CRISPR_Oscillator.py` & `mobspy-2.4.1/example_models/application_models/CRISPR_Oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/For_The_Trees.py` & `mobspy-2.4.1/example_models/application_models/For_The_Trees.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,9 +32,10 @@
     MySim = Simulation(Tree)
     MySim.simulation_method = 'stochastic'
     MySim.save_data = False
     MySim.plot_data = False
     MySim.duration = 100*u.years
     MySim.unit_x = 'year'
     MySim.volume = 1*u.meter**2
+    MySim.repetitions = 3
     MySim.run()
     MySim.plot_stochastic(Tree.dense, Tree.sparse, Tree.brown)
```

### Comparing `mobspy-2.4.0/example_models/application_models/NOR_gate.py` & `mobspy-2.4.1/example_models/application_models/NOR_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/donor_receptor.py` & `mobspy-2.4.1/example_models/application_models/donor_receptor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/oscillator.py` & `mobspy-2.4.1/example_models/application_models/oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/positive_phage_feedback_loop.py` & `mobspy-2.4.1/example_models/application_models/positive_phage_feedback_loop.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/random_walk.py` & `mobspy-2.4.1/example_models/application_models/random_walk.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/simple_infection.py` & `mobspy-2.4.1/example_models/application_models/simple_infection.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/simple_repressor.py` & `mobspy-2.4.1/example_models/application_models/simple_repressor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/example_models/application_models/simple_rule_based_and_gate.py` & `mobspy-2.4.1/example_models/application_models/simple_rule_based_and_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/images/img.png` & `mobspy-2.4.1/images/img.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/data_handler/process_result_data.py` & `mobspy-2.4.1/mobspy/data_handler/process_result_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,32 +82,39 @@
     def multiply_data_by_factor(data, factor):
         for key in data:
             if key == 'Time':
                 continue
 
             converted_data[key] = [count * factor for count in data[key]]
 
-    def convert_data(data, from_unit, to_unit):
-        for key in data:
-            if key == 'Time':
-                continue
+    # Old function - remove if not need in future. Removed because it is to slow to do this with pint
+    #def convert_data(data, from_unit, to_unit):
+    #    for key in data:
+    #        if key == 'Time':
+    #            continue
 
-            converted_data[key] = [(count * from_unit).to(to_unit).magnitude for count in data[key]]
+    #        converted_data[key] = [(count * from_unit).to(to_unit).magnitude for count in data[key]]
 
     if output_concentration:
         converted_data = convert_to_concentration(data, converted_data, volume_list, time_list)
 
-    # Fix here:
+    # Fix here - forgot concentration conversion
     if unit_y is not None:
         if 'mol' in str(unit_y):
             multiply_data_by_factor(converted_data, N_A ** -1)
             if output_concentration:
-                convert_data(converted_data, ur.molar, unit_y)
+                factor = (1*ur.molar).to(unit_y).magnitude
+                multiply_data_by_factor(converted_data, factor)
             else:
-                convert_data(converted_data, ur.moles, unit_y)
+                factor = (1*ur.moles).to(unit_y).magnitude
+                multiply_data_by_factor(converted_data, factor)
+        else:
+            if output_concentration:
+                factor = (1/ur.l).to(unit_y).magnitude
+                multiply_data_by_factor(converted_data, factor)
 
     return converted_data
 
 
 def convert_to_concentration(data, converted_data, volume_list, time_list):
     """
         Converts output data from counts to concentration according to simulation volume
```

### Comparing `mobspy-2.4.0/mobspy/data_handler/time_series_object.py` & `mobspy-2.4.1/mobspy/data_handler/time_series_object.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/assignments_implementation.py` & `mobspy-2.4.1/mobspy/modules/assignments_implementation.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/class_of_meta_specie_named_any.py` & `mobspy-2.4.1/mobspy/modules/class_of_meta_specie_named_any.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/context_related_scripts.py` & `mobspy-2.4.1/mobspy/modules/context_related_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/event_functions.py` & `mobspy-2.4.1/mobspy/modules/event_functions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/function_rate_code.py` & `mobspy-2.4.1/mobspy/modules/function_rate_code.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/logic_operator_objects.py` & `mobspy-2.4.1/mobspy/modules/logic_operator_objects.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/meta_class.py` & `mobspy-2.4.1/mobspy/modules/meta_class.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/meta_class_utils.py` & `mobspy-2.4.1/mobspy/modules/meta_class_utils.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/mobspy_expressions.py` & `mobspy-2.4.1/mobspy/modules/mobspy_expressions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/mobspy_parameters.py` & `mobspy-2.4.1/mobspy/modules/mobspy_parameters.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/order_operators.py` & `mobspy-2.4.1/mobspy/modules/order_operators.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/reaction_construction_nb.py` & `mobspy-2.4.1/mobspy/modules/reaction_construction_nb.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/reaction_construction_nb_parallel.py` & `mobspy-2.4.1/mobspy/modules/reaction_construction_nb_parallel.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/set_counts_module.py` & `mobspy-2.4.1/mobspy/modules/set_counts_module.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/species_string_generator.py` & `mobspy-2.4.1/mobspy/modules/species_string_generator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/modules/unit_handler.py` & `mobspy-2.4.1/mobspy/modules/unit_handler.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/parameter_estimation_data_loader/data_loader.py` & `mobspy-2.4.1/mobspy/parameter_estimation_data_loader/data_loader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py` & `mobspy-2.4.1/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/parameter_scripts/parameter_reader.py` & `mobspy-2.4.1/mobspy/parameter_scripts/parameter_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/parameter_scripts/parametric_sweeps.py` & `mobspy-2.4.1/mobspy/parameter_scripts/parametric_sweeps.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/parameters/README.md` & `mobspy-2.4.1/mobspy/parameters/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/parameters/default_reader.py` & `mobspy-2.4.1/mobspy/parameters/default_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/parameters/example_reader.py` & `mobspy-2.4.1/mobspy/parameters/example_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/patch_scripts/basico_task_parametrization.py` & `mobspy-2.4.1/mobspy/patch_scripts/basico_task_parametrization.py`

 * *Files 0% similar despite different names*

```diff
@@ -2018,7 +2018,12 @@
                 None
         if cn is not None:
             obj_map.setObjectCN(i, str(cn))
         if role == COPASI.CExperiment.dependent and 'weight' in mapping:
             obj_map.setScale(i, float(mapping['weight']))
 
     exp_set.addExperiment(experiment)
+
+
+if __name__ == '__main__':
+
+    get_default_handler()
```

### Comparing `mobspy-2.4.0/mobspy/plot_params/example_plot_reader.py` & `mobspy-2.4.1/mobspy/plot_params/example_plot_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,12 +46,14 @@
         "vertical_lines": [1, 2],
 
         # These parameters are not supported by plot_raw
         # Their only function is to alter the plot labels so please use that parameter
         # They are only listed here to avoid printing out errors during parameter checks
         "unit_x": '',
         "unit_y": '',
+        "ignore_unit_label_x": True,
+        "ignore_unit_label_y": True,
         "output_concentration": False,
         'simulation_method': 'stochastic'
     }
     return example_parameters
```

### Comparing `mobspy-2.4.0/mobspy/plot_scripts/default_plots.py` & `mobspy-2.4.1/mobspy/plot_scripts/default_plots.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,31 +27,36 @@
 
 def set_plot_units(new_plot_params):
     """
         Sets the plot labels to the unit names by adding to the xlabel and ylabel
 
         :param new_plot_params: (dict) plot parameters after some changes
     """
-    new_plot_params['xlabel'] = 'Time'
-    if new_plot_params['unit_x'] is not None:
-        if not isinstance(new_plot_params['unit_x'], Quantity):
-            new_plot_params['xlabel'] += f' ({new_plot_params["unit_x"]})'
-        else:
-            new_plot_params['xlabel'] += f' ({new_plot_params["unit_x"].units})'
+    if 'xlabel' not in new_plot_params:
+        new_plot_params['xlabel'] = 'Time'
 
-    if new_plot_params['output_concentration']:
-        new_plot_params['ylabel'] = 'Conc.'
-    else:
-        new_plot_params['ylabel'] = 'Counts'
-
-    if new_plot_params['unit_y'] is not None:
-        if not isinstance(new_plot_params['unit_y'], Quantity):
-            new_plot_params['ylabel'] += f' ({new_plot_params["unit_y"]})'
+        if new_plot_params['unit_x'] is not None and not ("ignore_unit_label_x" in new_plot_params and
+                                                          new_plot_params["ignore_unit_label_x"]):
+            if not isinstance(new_plot_params['unit_x'], Quantity):
+                new_plot_params['xlabel'] += f' ({new_plot_params["unit_x"]})'
+            else:
+                new_plot_params['xlabel'] += f' ({new_plot_params["unit_x"].units})'
+
+    if 'ylabel' not in new_plot_params:
+        if new_plot_params['output_concentration']:
+            new_plot_params['ylabel'] = 'Conc.'
         else:
-            new_plot_params['ylabel'] += f' ({new_plot_params["unit_y"].units})'
+            new_plot_params['ylabel'] = 'Counts'
+
+        if new_plot_params['unit_y'] is not None and not ("ignore_unit_label_x" in new_plot_params and
+                                                          new_plot_params["ignore_unit_label_y"]):
+            if not isinstance(new_plot_params['unit_y'], Quantity):
+                new_plot_params['ylabel'] += f' ({new_plot_params["unit_y"]})'
+            else:
+                new_plot_params['ylabel'] += f' ({new_plot_params["unit_y"].units})'
 
 
 def stochastic_plot(species, data, plot_params):
     """
         Design default stochastic plot using MobsPy plotting hierarchy. It them passes the parameters for plotting
         in the hierarchical plot module
 
@@ -90,28 +95,56 @@
             key_average = spe + '$' + 'average'
             key_dev = spe + '$' + 'deviation'
 
             data_to_plot[0][key_average] = processed_runs[0]
             data_to_plot[0][key_dev] = [processed_runs[1], processed_runs[2]]
 
             # We define the standard plot for the average and deviation
-            color = color_cycler(1)
-            plots_for_spe_i.append({'species_to_plot': [spe],
-                                    spe: {'color': color, 'label': spe}})
-
-            plots_for_spe_i_sta.append({'species_to_plot': [key_average], 'time_series': [0],
-                                        key_average: {'color': color, 'linestyle': '-', 'label': 'mean'}})
-            plots_for_spe_i_sta.append({'species_to_plot': [key_dev], 'fill_between': True, 'time_series': [0],
-                                        key_dev: {'color': (0.8, 0.8, 0.8), 'linestyle': ':', 'label': 'std. dev'}})
+            plots_for_spe_i.append({'species_to_plot': [spe]})
+
+            plots_for_spe_i_sta.append({'species_to_plot': [key_average], 'time_series': [0]})
+            plots_for_spe_i_sta.append({'species_to_plot': [key_dev], 'fill_between': True, 'time_series': [0]})
+
         except ValueError:
             simlog.error(f'{spe} species not found in data')
         new_plot_params['figures'].append({'ylabel': spe + ' ' + new_plot_params['ylabel'], 'plots': plots_for_spe_i})
         new_plot_params['figures'].append(
             {'ylabel': spe + ' ' + new_plot_params['ylabel'], 'plots': plots_for_spe_i_sta})
 
+    # Setting species parameters
+    for spe in species:
+        key_average = spe + '$' + 'average'
+        key_dev = spe + '$' + 'deviation'
+
+        color = color_cycler(1)
+
+        new_plot_params[key_dev] = {'color': (0.8, 0.8, 0.8), 'linestyle': ':', 'label': 'std. dev'}
+        if spe not in new_plot_params:
+            new_plot_params[spe] = {'color': color, 'label': spe}
+            new_plot_params[key_average] = {'color': color, 'linestyle': '-', 'label': 'mean'}
+        else:
+            new_plot_params[key_average] = {}
+
+            for par in new_plot_params[spe]:
+                new_plot_params[key_average][par] = new_plot_params[spe][par]
+                new_plot_params[key_dev][par] = new_plot_params[spe][par]
+
+            if 'label' not in new_plot_params[spe]:
+                new_plot_params[spe]['label'] = spe
+
+            if 'color' not in new_plot_params[spe]:
+                new_plot_params[spe]['color'] = color
+                new_plot_params[key_average]['color'] = color
+                new_plot_params[key_average]['linestyle'] = '-'
+                new_plot_params[key_average]['label'] = 'mean'
+            else:
+                new_plot_params[key_average]['color'] = new_plot_params[spe]['color']
+                new_plot_params[key_average]['linestyle'] = '-'
+                new_plot_params[key_average]['label'] = 'mean'
+
     return hp.plot_data(data_to_plot, new_plot_params)
 
 
 def deterministic_plot(species, data, plot_params):
     """
         Design default deterministic plot using MobsPy plotting hierarchy. It them passes the parameters for plotting
         in the hierarchical plot module
@@ -133,15 +166,22 @@
     set_plot_units(new_plot_params)
 
     #  Plot Config
     new_plot_params['frameon'] = False
     new_plot_params['species_to_plot'] = species
     color_cycler = hp.Color_cycle()
     for spe in species:
-        new_plot_params[spe] = {'label': spe, 'color': color_cycler(1)}
+        if spe not in new_plot_params:
+            new_plot_params[spe] = {'label': spe, 'color': color_cycler(1)}
+        else:
+            if 'label' not in new_plot_params[spe]:
+                new_plot_params[spe]['label'] = spe
+            if 'color' not in new_plot_params[spe]:
+                new_plot_params[spe]['color'] = color_cycler(1)
+
     return hp.plot_data(data, new_plot_params)
 
 
 def parametric_plot(species, data, plot_params):
 
     max_labels = 15
     current_labels = 0
```

### Comparing `mobspy-2.4.0/mobspy/plot_scripts/hierarchical_plot.py` & `mobspy-2.4.1/mobspy/plot_scripts/hierarchical_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -263,14 +263,21 @@
 
             if find_parameter(species_characteristics, key='label') is not None:
                 label = find_parameter(species_characteristics, key='label')
                 legend_flag = True
             else:
                 label = None
 
+            if find_parameter(species_characteristics, key='ylabel') is not None:
+                y_label = find_parameter(species_characteristics, key='ylabel')
+                if find_parameter(plot_params, 'ylabel_fontsize', figure_index) is not None:
+                    axs.set_ylabel(y_label, fontsize=plot_params['ylabel_fontsize'])
+                else:
+                    axs.set_ylabel(y_label)
+
             for ts in time_series:
                 ts_time = data['Time'][ts]
                 if '$' not in spe:
                     ts_data = data[spe][ts]
                 else:
                     ts_data = data[ts][spe]
 
@@ -395,15 +402,14 @@
 def plot_data(data, plot_params, return_fig_object=False):
     """
         This function plots the simulation results according to the specifications
 
         :param data: (dict) Data in MobsPy format
         :param plot_params: (dict) Plot parameters received
     """
-
     # Get the figure number from the list of figures
     # Add it to parameters
     try:
         figure_number = len(find_parameter(plot_params, 'figures'))
     except TypeError:
         # No figures plot only the default
         figure_number = 1
```

### Comparing `mobspy-2.4.0/mobspy/plot_scripts/process_plot_data.py` & `mobspy-2.4.1/mobspy/plot_scripts/process_plot_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
             spe_name = key.split('.')[0]
             if spe_name not in species:
                 simlog.warning(f'Parameter {key} not supported')
             validated_keys.add(key)
 
 
 def time_filter_operation(low, high, time_data, data):
+
     new_time_data = []
     new_data = []
 
     for t, d in zip(time_data, data):
         if t < low:
             continue
         elif low < t < high:
```

### Comparing `mobspy-2.4.0/mobspy/plot_scripts/statistics_calculations.py` & `mobspy-2.4.1/mobspy/plot_scripts/statistics_calculations.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/sbml_simulator/SBMLWriter.py` & `mobspy-2.4.1/mobspy/sbml_simulator/SBMLWriter.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc` & `mobspy-2.4.1/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc` & `mobspy-2.4.1/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc` & `mobspy-2.4.1/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/sbml_simulator/builder.py` & `mobspy-2.4.1/mobspy/sbml_simulator/builder.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/sbml_simulator/run.py` & `mobspy-2.4.1/mobspy/sbml_simulator/run.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy/simulation.py` & `mobspy-2.4.1/mobspy/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,14 +563,18 @@
             parameters_to_config = pr.read_json(config)
         elif type(config) == dict:
             parameters_to_config = config
         else:
             simlog.error("Parameters must be python dictionary or json file", stack_index=3)
         return parameters_to_config
 
+    def add_plot_params(self, **kwargs):
+        for key in kwargs:
+            self.plot_parameters[key] = deepcopy(kwargs[key])
+
     # Plotting encapsulation
     def extract_plot_essentials(self, *species):
         """
             Extract essential information for plotting
 
             :param species: (meta-species objects) meta-species objects to plot
             :return: species_strings (str) = species strings to be plotted, self.results = data resulting from the
@@ -844,14 +848,18 @@
 
     def plot(self, *species):
         self.base_sim.plot(*species)
 
     def plot_raw(self, parameters_or_file):
         self.base_sim.plot_raw(parameters_or_file)
 
+    def add_plot_params(self, **kwargs):
+        for key in kwargs:
+            self.base_sim.plot_parameters[key] = deepcopy(kwargs[key])
+
     def generate_sbml(self):
 
         self._check_all_sims_compilation()
         self._compile_multi_simulation()
 
         for sim in self.list_of_simulations:
```

### Comparing `mobspy-2.4.0/mobspy/simulation_logging/log_scripts.py` & `mobspy-2.4.1/mobspy/simulation_logging/log_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/mobspy.egg-info/PKG-INFO` & `mobspy-2.4.1/mobspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.4.0
+Version: 2.4.1
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.4.0/mobspy.egg-info/SOURCES.txt` & `mobspy-2.4.1/mobspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/setup.py` & `mobspy-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_plot_images/constant_tree.png` & `mobspy-2.4.1/test_plot_images/constant_tree.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_script.py` & `mobspy-2.4.1/test_script.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_15.txt` & `mobspy-2.4.1/test_tools/model_15.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_19.txt` & `mobspy-2.4.1/test_tools/model_19.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_21.txt` & `mobspy-2.4.1/test_tools/model_21.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_24.txt` & `mobspy-2.4.1/test_tools/model_24.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_26.txt` & `mobspy-2.4.1/test_tools/model_26.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_3.txt` & `mobspy-2.4.1/test_tools/model_3.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_31.txt` & `mobspy-2.4.1/test_tools/model_31.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_33.txt` & `mobspy-2.4.1/test_tools/model_33.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_38.txt` & `mobspy-2.4.1/test_tools/model_38.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_39.txt` & `mobspy-2.4.1/test_tools/model_39.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_4.txt` & `mobspy-2.4.1/test_tools/model_4.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_40.txt` & `mobspy-2.4.1/test_tools/model_40.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_41.txt` & `mobspy-2.4.1/test_tools/model_41.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_45.txt` & `mobspy-2.4.1/test_tools/model_45.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_5.txt` & `mobspy-2.4.1/test_tools/model_5.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_7.txt` & `mobspy-2.4.1/test_tools/model_7.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.0/test_tools/model_9.txt` & `mobspy-2.4.1/test_tools/model_9.txt`

 * *Files identical despite different names*

