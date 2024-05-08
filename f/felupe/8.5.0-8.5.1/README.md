# Comparing `tmp/felupe-8.5.0.tar.gz` & `tmp/felupe-8.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-8.5.0.tar", last modified: Sat Apr 27 14:14:00 2024, max compression
+gzip compressed data, was "felupe-8.5.1.tar", last modified: Wed May  8 14:42:00 2024, max compression
```

## Comparing `felupe-8.5.0.tar` & `felupe-8.5.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.133736 felupe-8.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-04-27 14:13:54.000000 felupe-8.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55533 2024-04-27 14:14:00.133736 felupe-8.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-27 14:13:54.000000 felupe-8.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-27 14:13:54.000000 felupe-8.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 14:14:00.133736 felupe-8.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.105736 felupe-8.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.109736 felupe-8.5.0/src/felupe/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.109736 felupe-8.5.0/src/felupe/assembly/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/_axi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/_integral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.113736 felupe-8.5.0/src/felupe/assembly/expression/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_bilinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.113736 felupe-8.5.0/src/felupe/constitution/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24929 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_mixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    18171 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_hyperelasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_hyperelasticity_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_user_materials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_user_materials_hyperelastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_user_materials_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.117736 felupe-8.5.0/src/felupe/dof/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/dof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/dof/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    21950 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/dof/_loadcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/dof/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.117736 felupe-8.5.0/src/felupe/element/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_hexahedron.py
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_quad.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.117736 felupe-8.5.0/src/felupe/field/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_axi.py
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_planestrain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.121736 felupe-8.5.0/src/felupe/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    45045 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.121736 felupe-8.5.0/src/felupe/mechanics/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_pointload.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_solidbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_solidbody_gravity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_solidbody_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_solidbody_pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.125736 felupe-8.5.0/src/felupe/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_discrete_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_dual.py
--rw-r--r--   0 runner    (1001) docker     (127)    15599 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_line_rectangle_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)    48571 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    32125 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.125736 felupe-8.5.0/src/felupe/quadrature/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_gausslegendre.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.125736 felupe-8.5.0/src/felupe/region/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/region/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/region/_region.py
--rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/region/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.125736 felupe-8.5.0/src/felupe/solve/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/solve/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.129736 felupe-8.5.0/src/felupe/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_newton.py
--rw-r--r--   0 runner    (1001) docker     (127)    20261 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_post.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_save.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.133736 felupe-8.5.0/src/felupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55533 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.133736 felupe-8.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_bilinearform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_constitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_constitution_newton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_dof.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_planestrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.928463 felupe-8.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-05-08 14:41:57.000000 felupe-8.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55747 2024-05-08 14:42:00.928463 felupe-8.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-05-08 14:41:57.000000 felupe-8.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-08 14:41:57.000000 felupe-8.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:42:00.928463 felupe-8.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.904463 felupe-8.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.908463 felupe-8.5.1/src/felupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.908463 felupe-8.5.1/src/felupe/assembly/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/_integral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.908463 felupe-8.5.1/src/felupe/assembly/expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/expression/_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/expression/_bilinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/expression/_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/expression/_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/expression/_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/assembly/expression/_mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.912463 felupe-8.5.1/src/felupe/constitution/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24929 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_models_hyperelasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_models_hyperelasticity_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_models_linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_models_linear_elasticity_large_strain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_models_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_user_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_user_materials_hyperelastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_user_materials_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19098 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/constitution/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.912463 felupe-8.5.1/src/felupe/dof/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/dof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/dof/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22016 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/dof/_loadcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/dof/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.912463 felupe-8.5.1/src/felupe/element/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/element/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/element/_hexahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/element/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/element/_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/element/_quad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/element/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/element/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.916463 felupe-8.5.1/src/felupe/field/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/field/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/field/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/field/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/field/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/field/_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/field/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/field/_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/field/_planestrain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.916463 felupe-8.5.1/src/felupe/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/math/_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/math/_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/math/_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/math/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45045 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/math/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.916463 felupe-8.5.1/src/felupe/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_pointload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_solidbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_solidbody_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_solidbody_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_solidbody_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mechanics/_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.920463 felupe-8.5.1/src/felupe/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_discrete_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15599 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_line_rectangle_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48571 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32125 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/mesh/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.920463 felupe-8.5.1/src/felupe/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/quadrature/_gausslegendre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/quadrature/_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/quadrature/_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/quadrature/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/quadrature/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.920463 felupe-8.5.1/src/felupe/region/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/region/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/region/_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/region/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.920463 felupe-8.5.1/src/felupe/solve/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/solve/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.924463 felupe-8.5.1/src/felupe/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/tools/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/tools/_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20261 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/tools/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/tools/_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/tools/_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/tools/_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-08 14:41:57.000000 felupe-8.5.1/src/felupe/tools/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.928463 felupe-8.5.1/src/felupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55747 2024-05-08 14:42:00.000000 felupe-8.5.1/src/felupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-08 14:42:00.000000 felupe-8.5.1/src/felupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:42:00.000000 felupe-8.5.1/src/felupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-08 14:42:00.000000 felupe-8.5.1/src/felupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 14:42:00.000000 felupe-8.5.1/src/felupe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:42:00.928463 felupe-8.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_bilinearform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_constitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_constitution_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_dof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_planestrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-05-08 14:41:57.000000 felupe-8.5.1/tests/test_tools.py
```

### Comparing `felupe-8.5.0/LICENSE` & `felupe-8.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/PKG-INFO` & `felupe-8.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 8.5.0
+Version: 8.5.1
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -738,25 +738,26 @@
 </p>
 
 [![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 FElupe is a Python 3.8+ 🐍 finite element analysis package 📦 focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics 🔧 of solid bodies 🚂. Its name is a combination of FE (finite element) and the german word *Lupe* 🔍 (magnifying glass) as a synonym for getting an insight 📖 how a finite element analysis code 🧮 looks like under the hood 🕳️.
 
 <p align="center">
-  <a href="https://felupe.readthedocs.io/en/latest/examples/ex01_beam.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex01_beam_thumb.png" height="160px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/ex02_plate-with-hole.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex02_plate-with-hole_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex03_plasticity.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex03_plasticity_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex04_balloon.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex04_balloon_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex05_rubber-metal-bushing.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex05_rubber-metal-bushing_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex06_rubber-metal-spring.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex06_rubber-metal-spring_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex07_engine-mount.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex07_engine-mount_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex08_shear.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex08_shear_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex09_numeric-continuation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex09_numeric-continuation_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex10_poisson-equation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex10_poisson-equation_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex11_notch-stress.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex11_notch-stress_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex12_foot-bone.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex12_foot-bone_thumb.png" height="160px"/></a>
+  <a href="https://felupe.readthedocs.io/en/latest/examples/ex01_beam.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex01_beam_thumb.png" height="120px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/ex02_plate-with-hole.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex02_plate-with-hole_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex03_plasticity.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex03_plasticity_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex04_balloon.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex04_balloon_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex05_rubber-metal-bushing.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex05_rubber-metal-bushing_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex06_rubber-metal-spring.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex06_rubber-metal-spring_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex07_engine-mount.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex07_engine-mount_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex08_shear.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex08_shear_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex09_numeric-continuation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex09_numeric-continuation_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex10_poisson-equation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex10_poisson-equation_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex11_notch-stress.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex11_notch-stress_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex12_foot-bone.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex12_foot-bone_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex13_morph-rubber-wheel.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex13_morph-rubber-wheel_thumb.png" height="120px"/></a>
 </p>
 
 # Installation
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
 pip install felupe[all]
```

### Comparing `felupe-8.5.0/README.md` & `felupe-8.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 </p>
 
 [![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 FElupe is a Python 3.8+ 🐍 finite element analysis package 📦 focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics 🔧 of solid bodies 🚂. Its name is a combination of FE (finite element) and the german word *Lupe* 🔍 (magnifying glass) as a synonym for getting an insight 📖 how a finite element analysis code 🧮 looks like under the hood 🕳️.
 
 <p align="center">
-  <a href="https://felupe.readthedocs.io/en/latest/examples/ex01_beam.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex01_beam_thumb.png" height="160px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/ex02_plate-with-hole.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex02_plate-with-hole_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex03_plasticity.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex03_plasticity_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex04_balloon.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex04_balloon_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex05_rubber-metal-bushing.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex05_rubber-metal-bushing_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex06_rubber-metal-spring.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex06_rubber-metal-spring_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex07_engine-mount.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex07_engine-mount_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex08_shear.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex08_shear_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex09_numeric-continuation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex09_numeric-continuation_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex10_poisson-equation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex10_poisson-equation_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex11_notch-stress.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex11_notch-stress_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex12_foot-bone.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex12_foot-bone_thumb.png" height="160px"/></a>
+  <a href="https://felupe.readthedocs.io/en/latest/examples/ex01_beam.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex01_beam_thumb.png" height="120px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/ex02_plate-with-hole.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex02_plate-with-hole_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex03_plasticity.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex03_plasticity_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex04_balloon.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex04_balloon_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex05_rubber-metal-bushing.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex05_rubber-metal-bushing_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex06_rubber-metal-spring.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex06_rubber-metal-spring_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex07_engine-mount.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex07_engine-mount_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex08_shear.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex08_shear_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex09_numeric-continuation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex09_numeric-continuation_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex10_poisson-equation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex10_poisson-equation_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex11_notch-stress.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex11_notch-stress_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex12_foot-bone.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex12_foot-bone_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex13_morph-rubber-wheel.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex13_morph-rubber-wheel_thumb.png" height="120px"/></a>
 </p>
 
 # Installation
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
 pip install felupe[all]
```

#### html2text {}

```diff
@@ -30,15 +30,16 @@
       _s_p_r_i_n_g___t_h_u_m_b_._p_n_g_]_[_h_t_t_p_s_:_/_/_f_e_l_u_p_e_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_e_n_/_l_a_t_e_s_t_/___i_m_a_g_e_s_/
 _s_p_h_x___g_l_r___e_x_0_7___e_n_g_i_n_e_-_m_o_u_n_t___t_h_u_m_b_._p_n_g_]_[_h_t_t_p_s_:_/_/_f_e_l_u_p_e_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_e_n_/_l_a_t_e_s_t_/
 ___i_m_a_g_e_s_/_s_p_h_x___g_l_r___e_x_0_8___s_h_e_a_r___t_h_u_m_b_._p_n_g_]_[_h_t_t_p_s_:_/_/_f_e_l_u_p_e_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_e_n_/_l_a_t_e_s_t_/
         ___i_m_a_g_e_s_/_s_p_h_x___g_l_r___e_x_0_9___n_u_m_e_r_i_c_-_c_o_n_t_i_n_u_a_t_i_o_n___t_h_u_m_b_._p_n_g_]_[_h_t_t_p_s_:_/_/
         _f_e_l_u_p_e_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_e_n_/_l_a_t_e_s_t_/___i_m_a_g_e_s_/_s_p_h_x___g_l_r___e_x_1_0___p_o_i_s_s_o_n_-
      _e_q_u_a_t_i_o_n___t_h_u_m_b_._p_n_g_]_[_h_t_t_p_s_:_/_/_f_e_l_u_p_e_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_e_n_/_l_a_t_e_s_t_/___i_m_a_g_e_s_/
 _s_p_h_x___g_l_r___e_x_1_1___n_o_t_c_h_-_s_t_r_e_s_s___t_h_u_m_b_._p_n_g_]_[_h_t_t_p_s_:_/_/_f_e_l_u_p_e_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_e_n_/_l_a_t_e_s_t_/
-                  ___i_m_a_g_e_s_/_s_p_h_x___g_l_r___e_x_1_2___f_o_o_t_-_b_o_n_e___t_h_u_m_b_._p_n_g_]
+ ___i_m_a_g_e_s_/_s_p_h_x___g_l_r___e_x_1_2___f_o_o_t_-_b_o_n_e___t_h_u_m_b_._p_n_g_]_[_h_t_t_p_s_:_/_/_f_e_l_u_p_e_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_e_n_/
+          _l_a_t_e_s_t_/___i_m_a_g_e_s_/_s_p_h_x___g_l_r___e_x_1_3___m_o_r_p_h_-_r_u_b_b_e_r_-_w_h_e_e_l___t_h_u_m_b_._p_n_g_]
 # Installation Install Python, fire up ð¥ a terminal and run ð ```shell
 pip install felupe[all] ``` where `[all]` is a combination of `
 [io,parallel,plot,progress,view]` and installs all optional dependencies.
 FElupe has minimal requirements, all available at PyPI supporting all
 platforms. * [`numpy`](https://github.com/numpy/numpy) for array operations *
 [`scipy`](https://github.com/scipy/scipy) for sparse matrices * [`tensortrax`]
 (https://github.com/adtzlr/tensortrax) for automatic differentiation In order
```

### Comparing `felupe-8.5.0/pyproject.toml` & `felupe-8.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/__init__.py` & `felupe-8.5.1/src/felupe/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/assembly/_axi.py` & `felupe-8.5.1/src/felupe/assembly/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/assembly/_cartesian.py` & `felupe-8.5.1/src/felupe/assembly/_cartesian.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/assembly/_integral.py` & `felupe-8.5.1/src/felupe/assembly/_integral.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/assembly/expression/_basis.py` & `felupe-8.5.1/src/felupe/assembly/expression/_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/assembly/expression/_bilinear.py` & `felupe-8.5.1/src/felupe/assembly/expression/_bilinear.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/assembly/expression/_decorator.py` & `felupe-8.5.1/src/felupe/assembly/expression/_decorator.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/assembly/expression/_expression.py` & `felupe-8.5.1/src/felupe/assembly/expression/_expression.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/assembly/expression/_linear.py` & `felupe-8.5.1/src/felupe/assembly/expression/_linear.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/assembly/expression/_mixed.py` & `felupe-8.5.1/src/felupe/assembly/expression/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/__init__.py` & `felupe-8.5.1/src/felupe/constitution/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/_base.py` & `felupe-8.5.1/src/felupe/constitution/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/_kinematics.py` & `felupe-8.5.1/src/felupe/constitution/_kinematics.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/_mixed.py` & `felupe-8.5.1/src/felupe/constitution/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/_models_hyperelasticity.py` & `felupe-8.5.1/src/felupe/constitution/_models_hyperelasticity.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,16 +537,15 @@
 
         if lmbda is None:
             Pb = np.multiply(iFT, -mu, out=iFT)
         else:
             lmbda_lnJ = np.multiply(lmbda, lnJ, out=lnJ)
             Pb = np.multiply(iFT, -mu + lmbda_lnJ, out=iFT)
 
-        if lmbda is not None:
-            np.add(P, Pb, out=P)
+        np.add(P, Pb, out=P)
 
         return [P, statevars]
 
     def hessian(self, x, mu=None, lmbda=None, out=None):
         """Hessian of the strain energy density function per unit undeformed volume of
         the Neo-Hookean material formulation.
```

### Comparing `felupe-8.5.0/src/felupe/constitution/_models_hyperelasticity_ad.py` & `felupe-8.5.1/src/felupe/constitution/_models_hyperelasticity_ad.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,22 +54,27 @@
     mu : float
         Second Lamé constant (shear modulus).
     lmbda : float
         First Lamé constant (shear modulus).
 
     Notes
     -----
+    The strain energy function is given in Eq. :eq:`psi-svk`
+
     ..  math::
+        :label: psi-svk
 
         \psi = \mu I_2 + \lambda \frac{I_1^2}{2}
 
-    With the first and second invariant of the Green-Lagrange strain tensor
-    :math:`\boldsymbol{E} = \frac{1}{2} (\boldsymbol{C} - \boldsymbol{1})`.
+    with the first and second invariant of the Green-Lagrange strain tensor
+    :math:`\boldsymbol{E} = \frac{1}{2} (\boldsymbol{C} - \boldsymbol{1})`, see Eq.
+    :eq:`invariants-svk`.
 
     ..  math::
+        :label: invariants-svk
 
         I_1 &= \text{tr}\left( \boldsymbol{E} \right)
 
         I_2 &= \boldsymbol{E} : \boldsymbol{E}
 
     Examples
     --------
@@ -112,15 +117,18 @@
     C : tensortrax.Tensor
         Right Cauchy-Green deformation tensor.
     mu : float
         Shear modulus.
 
     Notes
     -----
+    The strain energy function is given in Eq. :eq:`psi-nh`.
+
     ..  math::
+        :label: psi-nh
 
         \psi = \frac{\mu}{2} \left(\text{tr}\left(\hat{\boldsymbol{C}}\right) - 3\right)
 
     Examples
     --------
 
     ..  pyvista-plot::
@@ -158,34 +166,39 @@
     C10 : float
         First material parameter associated to the first invariant.
     C01 : float
         Second material parameter associated to the second invariant.
 
     Notes
     -----
+    The strain energy function is given in Eq. :eq:`psi-mr`
+
     ..  math::
+        :label: psi-mr
 
         \psi = C_{10} \left(\hat{I}_1 - 3 \right) + C_{01} \left(\hat{I}_2 - 3 \right)
 
-    With the first and second main invariant of the distortional part of the right
-    Cauchy-Green deformation tensor.
+    with the first and second main invariant of the distortional part of the right
+    Cauchy-Green deformation tensor, see Eq. :eq:`invariants-mr`.
 
     ..  math::
+        :label: invariants-mr
 
         \hat{I}_1 &= J^{-2/3} \text{tr}\left( \boldsymbol{C} \right)
 
         \hat{I}_2 &= J^{-4/3} \frac{1}{2} \left(
             \text{tr}\left(\boldsymbol{C}\right)^2 -
             \text{tr}\left(\boldsymbol{C}^2\right)
         \right)
 
     The doubled sum of both material parameters is equal to the shear modulus
-    :math:`\mu`.
+    :math:`\mu` as denoted in Eq. :eq:`shear-modulus-mr`.
 
     ..  math::
+        :label: shear-modulus-mr
 
         \mu = 2 \left( C_{10} + C_{01} \right)
 
     Examples
     --------
 
     ..  pyvista-plot::
@@ -228,30 +241,35 @@
     C20 : float
         Material parameter associated to the quadratic term of the first invariant.
     C30 : float
         Material parameter associated to the cubic term of the first invariant.
 
     Notes
     -----
+    The strain energy function is given in Eq. :eq:`psi-yeoh`
+
     ..  math::
+        :label: psi-yeoh
 
         \psi = C_{10} \left(\hat{I}_1 - 3 \right) + C_{20} \left(\hat{I}_1 - 3 \right)^2
              + C_{30} \left(\hat{I}_1 - 3 \right)^3
 
-    With the first main invariant of the distortional part of the right
-    Cauchy-Green deformation tensor.
+    with the first main invariant of the distortional part of the right
+    Cauchy-Green deformation tensor, see Eq. :eq:`invariants-yeoh`.
 
     ..  math::
+        :label: invariants-yeoh
 
         \hat{I}_1 = J^{-2/3} \text{tr}\left( \boldsymbol{C} \right)
 
     The :math:`C_{10}` material parameter is equal to half the initial shear modulus
-    :math:`\mu`.
+    :math:`\mu` as denoted in Eq. :eq:`shear-modulus-yeoh`.
 
     ..  math::
+        label: shear-modulus-yeoh
 
         \mu = 2 C_{10}
 
     Examples
     --------
 
     ..  pyvista-plot::
@@ -298,38 +316,44 @@
     C20 : float
         Material parameter associated to the quadratic term of the first invariant.
     C30 : float
         Material parameter associated to the cubic term of the first invariant.
 
     Notes
     -----
+    The strain energy function is given in Eq. :eq:`psi-tod`
+
     ..  math::
+        :label: psi-tod
 
         \psi &= C_{10} \left(\hat{I}_1 - 3 \right) + C_{01} \left(\hat{I}_2 - 3 \right)
              + C_{11} \left(\hat{I}_1 - 3 \right) \left(\hat{I}_2 - 3 \right)
 
             &+ C_{20} \left(\hat{I}_1 - 3 \right)^2
              + C_{30} \left(\hat{I}_1 - 3 \right)^3
 
-    With the first and second main invariant of the distortional part of the right
-    Cauchy-Green deformation tensor.
+    with the first and second main invariant of the distortional part of the right
+    Cauchy-Green deformation tensor, see Eq. :eq:`invariants-tod`.
 
     ..  math::
+        :label: invariants-tod
 
         \hat{I}_1 &= J^{-2/3} \text{tr}\left( \boldsymbol{C} \right)
 
         \hat{I}_2 &= J^{-4/3} \frac{1}{2} \left(
             \text{tr}\left(\boldsymbol{C}\right)^2 -
             \text{tr}\left(\boldsymbol{C}^2\right)
         \right)
 
     The doubled sum of the material parameters :math:`C_{10}` and :math:`C_{01}` is
-    equal to the initial shear modulus :math:`\mu`.
+    equal to the initial shear modulus :math:`\mu` as denoted in Eq.
+    :eq:`shear-modulus-tod`.
 
     ..  math::
+        :label: shear-modulus-tod
 
         \mu = 2 \left( C_{10} + C_{01} \right)
 
     Examples
     --------
 
     ..  pyvista-plot::
@@ -378,24 +402,28 @@
     mu : list of float
         List of moduli.
     alpha : list of float
         List of stretch exponents.
 
     Notes
     -----
+    The strain energy function is given in Eq. :eq:`psi-ogden`
+
     ..  math::
+        :label: psi-ogden
 
         \psi = \sum_i \frac{2 \mu_i}{\alpha^2_i} \left(
             \lambda_1^{\alpha_i} + \lambda_2^{\alpha_i} + \lambda_3^{\alpha_i} - 3
         \right)
 
     The sum of the moduli :math:`\mu_i` is equal to the initial shear modulus
-    :math:`\mu`.
+    :math:`\mu`, see Eq. :eq:`shear-modulus-ogden`.
 
     ..  math::
+        :label: shear-modulus-ogden
 
         \mu = \sum_i \mu_i
 
     Examples
     --------
 
     ..  pyvista-plot::
@@ -428,50 +456,57 @@
     `Arruda-Boyce <https://en.wikipedia.org/wiki/Arruda-Boyce_model>`_ material
     formulation.
 
     Parameters
     ----------
     C : tensortrax.Tensor
         Right Cauchy-Green deformation tensor.
-    C1 : list of float
+    C1 : float
         Initial shear modulus.
-    limit : list of float
-        Limiting stretch at which the polymer chain network becomes locked 
-        :math:`\lambda_m`.
+    limit : float
+        Limiting stretch :math:`\lambda_m` at which the polymer chain network becomes
+        locked.
 
     Notes
     -----
+    The strain energy function is given in Eq. :eq:`psi-ab`
+    
     ..  math::
+        :label: psi-ab
 
         \psi = C_1 \sum_{i=1}^5 \alpha_i \beta^{i-1} \left( \hat{I}_1^i - 3^i \right)
 
-    With the first main invariant of the distortional part of the right
-    Cauchy-Green deformation tensor
+    with the first main invariant of the distortional part of the right
+    Cauchy-Green deformation tensor as given in Eq. :eq:`invariants-ab`
     
     ..  math::
+        :label: invariants-ab
     
         \hat{I}_1 = J^{-2/3} \text{tr}\left( \boldsymbol{C} \right)
     
-    and :math_`\alpha_i` and :math`\beta`.
+    and :math:`\alpha_i` and :math:`\beta` as denoted in Eq. :eq:`ab-param`.
     
     ..  math::
+        :label: ab-param
         
         \boldsymbol{\alpha} &= \begin{bmatrix} 
             \frac{1}{2} \\ 
             \frac{1}{20} \\
             \frac{11}{1050} \\
             \frac{19}{7000} \\
             \frac{519}{673750}
         \end{bmatrix}
         
         \beta &= \frac{1}{\lambda_m^2}
     
-    The initial shear modulus is a function of both material parameters.
+    The initial shear modulus is a function of both material parameters, see Eq.
+    :eq:`shear-modulus-ab`.
     
     ..  math::
+        :label: shear-modulus-ab
         
         \mu = C_1 \left( 
             1 + \frac{3}{5 \lambda_m^2} + \frac{99}{175 \lambda_m^4} 
               + \frac{513}{875 \lambda_m^6} + \frac{42039}{67375 \lambda_m^8} 
         \right)
 
     Examples
@@ -526,40 +561,49 @@
         Constraint contribution to the initial shear modulus.
     beta : float
         Global rearrangements of cross-links upon deformation (release of topological
         constraints).
 
     Notes
     -----
+    The strain energy function is given in Eq. :eq:`psi-et`
+
     ..  math::
+        :label: psi-et
 
         \psi = \frac{G_c}{2} \left[ \frac{\left( 1 - \delta^2 \right)
             \left( \hat{I}_1 - 3 \right)}{1 - \delta^2 \left( \hat{I}_1 - 3 \right)} +
             \ln \left( 1 - \delta^2 \left( \hat{I}_1 - 3 \right) \right) \right] +
             \frac{2 G_e}{\beta^2} \left( \hat{\lambda}_1^{-\beta} +
             \hat{\lambda}_2^{-\beta} + \hat{\lambda}_3^{-\beta} - 3 \right)
 
-    With the first main invariant of the distortional part of the right
-    Cauchy-Green deformation tensor
+    with the first main invariant of the distortional part of the right
+    Cauchy-Green deformation tensor as given in Eq. :eq:`invariants-et`
 
     ..  math::
+        :label: invariants-et
 
         \hat{I}_1 = J^{-2/3} \text{tr}\left( \boldsymbol{C} \right)
 
     and the principal stretches, obtained from the distortional part of the right
-    Cauchy-Green deformation tensor
+    Cauchy-Green deformation tensor, see Eq. :eq:`stretches-et`.
 
     ..  math::
+        :label: stretches-et
 
-        \hat{\lambda}_\alpha = J^{-1/3} \lambda_\alpha
+        \lambda^2_\alpha &= \text{eigvals}\left \boldsymbol{C} \right)
+
+        \hat{\lambda}_\alpha &= J^{-1/3} \lambda_\alpha
 
     The initial shear modulus results from the sum of the cross-link and the constraint
-    contributions to the total initial shear modulus.
+    contributions to the total initial shear modulus as denoted in Eq.
+    :eq:`shear-modulus-et`.
 
     ..  math::
+        :label: shear-modulus-et
 
         \mu = G_e + G_c
 
     Examples
     --------
 
     ..  pyvista-plot::
@@ -600,15 +644,29 @@
     We = 2 * Ge / beta**2 * sum1(wC ** (-beta / 2) - 1)
     return Wc + We
 
 
 def van_der_waals(C, mu, limit, a, beta):
     r"""Strain energy function of the
     `Van der Waals <https://doi.org/10.1016/0032-3861(81)90200-7>`_ [1]_ material
-    formulation.
+    formulation.,
+
+    Parameters
+    ----------
+    C : tensortrax.Tensor
+        Right Cauchy-Green deformation tensor.
+    mu : float
+        Initial shear modulus.
+    limit : float
+        Limiting stretch :math:`\lambda_m` at which the polymer chain network becomes
+        locked.
+    a : float
+        Attractive interactions between the quasi-particles.
+    beta : float
+        Mixed-Invariant factor: 0 for pure I1- and 1 for pure I2-contribution.
 
     Examples
     --------
     ..  pyvista-plot::
         :context:
 
         >>> import felupe as fem
@@ -641,20 +699,65 @@
     Im.x[np.isclose(Im.x, 3)] += 1e-8
     eta = sqrt((Im - 3) / (limit**2 - 3))
     return mu * (
         -(limit**2 - 3) * (log(1 - eta) + eta) - 2 / 3 * a * ((Im - 3) / 2) ** (3 / 2)
     )
 
 
-@isochoric_volumetric_split
 def finite_strain_viscoelastic(C, Cin, mu, eta, dtime):
     r"""Multiplicative
     `finite strain viscoelastic <https://doi.org/10.1016/j.cma.2013.07.004>`_ [1]_
     material formulation.
 
+    Notes
+    -----
+    The material formulation is built upon the multiplicative decomposition of the
+    deformation gradient tensor into an elastic and an inelastic part, see Eq.
+    :eq:`multiplicative-split`.
+
+    ..  math::
+        :label: multiplicative-split
+
+        \boldsymbol{F} &= \boldsymbol{F}_e \boldsymbol{F}_i
+
+        \boldsymbol{C}_e &= \boldsymbol{F}_e^T \boldsymbol{F}_e
+
+        \boldsymbol{C}_i &= \boldsymbol{F}_i^T \boldsymbol{F}_i
+
+        \text{tr}\left( \boldsymbol{C}_e \right) &= \text{tr}\left(
+            \boldsymbol{C} \boldsymbol{C}_i^{-1}
+        \right)
+
+    The components of the inelastic right Cauchy-Green deformation tensor are used as
+    state variables with the evolution equation and its explicit update formula as given
+    in Eq. :eq:`evolution` [1]_. Here, the inelastic right Cauchy-Green deformation
+    tensor is enforced to be an unimodular tensor.
+
+    ..  math::
+        :label: evolution
+
+        \dot{\boldsymbol{C}}_i &= \frac{\mu}{\eta} \text{dev}\left(
+            \hat{\boldsymbol{C}} \boldsymbol{C}_i^{-1}
+        \right) \boldsymbol{C}_i
+
+        \boldsymbol{X} &= \boldsymbol{C}_{i,n}
+            + \frac{\Delta t \mu}{\eta} \hat{\boldsymbol{C}}
+
+        \boldsymbol{C}_i &= \det(\boldsymbol{X})^{-1/3}\ \boldsymbol{X}
+
+    The distortional part of the strain energy density per unit undeformed volume is
+    assumed to be of a Neo-Hookean form, see Eq. :eq:`nh-w`.
+
+    ..  math::
+        :label: nh-w
+
+        \hat{\psi} = \frac{\mu}{2} \left( \text{tr}\left(
+            \hat{\boldsymbol{C}} \boldsymbol{C}_i^{-1}
+        \right) - 3 \right)
+
     Examples
     --------
     ..  pyvista-plot::
         :context:
 
         >>> import felupe as fem
         >>>
@@ -684,21 +787,22 @@
     ..  [1] A. V. Shutov, R. Landgraf, and J. Ihlemann, "An explicit solution for
         implicit time stepping in multiplicative finite strain viscoelasticity",
         Computer Methods in Applied Mechanics and Engineering, vol. 265. Elsevier BV,
         pp. 213–225, Oct. 2013. doi:
         `10.1016/j.cma.2013.07.004 <https://doi.org/10.1016/j.cma.2013.07.004>`_.
 
     """
+    J3 = det(C) ** (-1 / 3)
 
     # update of state variables by evolution equation
-    Ci = from_triu_1d(Cin, like=C) + mu / eta * dtime * C
+    Ci = from_triu_1d(Cin, like=C) + (mu / eta * dtime) * (J3 * C)
     Ci = det(Ci) ** (-1 / 3) * Ci
 
     # first invariant of elastic part of right Cauchy-Green deformation tensor
-    I1 = trace(C @ inv(Ci))
+    I1 = J3 * trace(C @ inv(Ci))
 
     # strain energy function and state variable
     return mu / 2 * (I1 - 3), triu_1d(Ci)
 
 
 # default material parameters
 saint_venant_kirchhoff.kwargs = dict(mu=0.0, lmbda=0.0)
```

### Comparing `felupe-8.5.0/src/felupe/constitution/_models_linear_elasticity.py` & `felupe-8.5.1/src/felupe/constitution/_models_linear_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py` & `felupe-8.5.1/src/felupe/constitution/_models_linear_elasticity_large_strain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/_models_pseudo_elasticity.py` & `felupe-8.5.1/src/felupe/constitution/_models_pseudo_elasticity.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,19 +38,23 @@
     m : float
         The initial Mullins softening modulus.
     beta : float
         Maximum deformation-dependent part of the Mullins softening modulus.
 
     Notes
     -----
+    ..  note::
+        This implementation uses the hyperbolic tangent instead of the Gauss error
+        function.
 
     ..  math::
 
-        \eta(\psi, \psi_{max}) &= 1 - \frac{1}{r} erf\left( \frac{\psi_{max} - \psi}
-        {m + \beta~\psi_{max}} \right)
+        \eta(\psi, \psi_\text{max}) &= 1 - \frac{1}{r} \tanh \left(
+            \frac{\psi_\text{max} - \psi}{m + \beta~\psi_\text{max}}
+        \right)
 
         \boldsymbol{P} &= \eta \frac{\partial \psi}{\partial \boldsymbol{F}}
 
         \mathbb{A} &= \frac{\partial^2 \psi}{\partial \boldsymbol{F} \partial
         \boldsymbol{F}} + \frac{\partial \eta}{\partial \psi} \frac{\partial \psi}
         {\partial \boldsymbol{F}} \otimes \frac{\partial \psi}{\partial \boldsymbol{F}}
```

### Comparing `felupe-8.5.0/src/felupe/constitution/_user_materials.py` & `felupe-8.5.1/src/felupe/constitution/_user_materials.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/_user_materials_hyperelastic.py` & `felupe-8.5.1/src/felupe/constitution/_user_materials_hyperelastic.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/_user_materials_models.py` & `felupe-8.5.1/src/felupe/constitution/_user_materials_models.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/constitution/_view.py` & `felupe-8.5.1/src/felupe/constitution/_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,20 +197,21 @@
         λ2 = λ3 = 1 / np.sqrt(λ1)
         eye = np.eye(3).reshape(3, 3, 1, 1)
 
         def fun(λ3):
             λ2 = λ3
             F = eye * np.array([λ1, λ2, λ3]).reshape(1, 3, 1, -1)
             if self.statevars_included:
-                if self.statevars is None:
-                    self.statevars = np.zeros((*self.umat.x[-1].shape, 1, 1))
+                statevars = self.statevars
+                if statevars is None:
+                    statevars = np.zeros((*self.umat.x[-1].shape, 1, 1))
                 P = np.zeros_like(F)
                 for increment, defgrad in enumerate(F.T):
                     P[..., [increment]], statevars = self.umat.gradient(
-                        [F[..., [increment]], self.statevars]
+                        [F[..., [increment]], statevars]
                     )
             else:
                 P, statevars = self.umat.gradient([F, None])
             return P[2, 2].ravel()
 
         from scipy.optimize import root
 
@@ -258,20 +259,21 @@
         λ2 = np.ones_like(λ1)
         λ3 = 1 / λ1
         eye = np.eye(3).reshape(3, 3, 1, 1)
 
         def fun(λ3):
             F = eye * np.array([λ1, λ2, λ3]).reshape(1, 3, 1, -1)
             if self.statevars_included:
-                if self.statevars is None:
-                    self.statevars = np.zeros((*self.umat.x[-1].shape, 1, 1))
+                statevars = self.statevars
+                if statevars is None:
+                    statevars = np.zeros((*self.umat.x[-1].shape, 1, 1))
                 P = np.zeros_like(F)
                 for increment, defgrad in enumerate(F.T):
                     P[..., [increment]], statevars = self.umat.gradient(
-                        [F[..., [increment]], self.statevars]
+                        [F[..., [increment]], statevars]
                     )
             else:
                 P, statevars = self.umat.gradient([F, None])
             return P[2, 2].ravel()
 
         from scipy.optimize import root
 
@@ -318,20 +320,21 @@
         λ1 = λ2 = stretches
         λ3 = 1 / λ1**2
         eye = np.eye(3).reshape(3, 3, 1, 1)
 
         def fun(λ3):
             F = eye * np.array([λ1, λ2, λ3]).reshape(1, 3, 1, -1)
             if self.statevars_included:
-                if self.statevars is None:
-                    self.statevars = np.zeros((*self.umat.x[-1].shape, 1, 1))
+                statevars = self.statevars
+                if statevars is None:
+                    statevars = np.zeros((*self.umat.x[-1].shape, 1, 1))
                 P = np.zeros_like(F)
                 for increment, defgrad in enumerate(F.T):
                     P[..., [increment]], statevars = self.umat.gradient(
-                        [F[..., [increment]], self.statevars]
+                        [F[..., [increment]], statevars]
                     )
             else:
                 P, self.statevars = self.umat.gradient([F, None])
             return P[2, 2].ravel()
 
         from scipy.optimize import root
```

### Comparing `felupe-8.5.0/src/felupe/dof/_boundary.py` & `felupe-8.5.1/src/felupe/dof/_boundary.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,148 +65,148 @@
         freedom are prescribed.
     value : ndarray or float
         Value of the selected (prescribed) degrees of freedom.
 
     Examples
     --------
     A boundary condition prescribes values for chosen degrees of freedom of a given
-    field (**not** a field container). This is demonstrated for a plane-strain
-    vector field on a quad-mesh of a circle.
+    field (**not** a field container). This is demonstrated for a vector field on a
+    hex-mesh of a cylinder.
 
     ..  pyvista-plot::
         :context:
 
         >>> import felupe as fem
         >>>
-        >>> mesh = fem.Circle(radius=1, n=6)
-        >>> x, y = mesh.points.T
-        >>> region = fem.RegionQuad(mesh)
-        >>> displacement = fem.FieldPlaneStrain(region, dim=2)
+        >>> mesh = fem.Circle(radius=1, n=6).expand(n=6)
+        >>> x, y, z = mesh.points.T
+        >>> region = fem.RegionHexahedron(mesh)
+        >>> displacement = fem.Field(region, dim=3)
         >>> field = fem.FieldContainer([displacement])
 
     A boundary on the displacement field which prescribes all components of the field
-    on the outermost left point of the circle is created. The easiest way is to pass the
-    desired value to ``fx``. The same result is obtained if a callable function is
+    on the outermost right point of the circle is created. The easiest way is to pass
+    the desired value to ``fx``. The same result is obtained if a callable function is
     passed to ``fx``.
 
     ..  pyvista-plot::
         :context:
 
-        >>> import numpy as np
+        >>> import pyvista as pv
         >>>
-        >>> left = fem.Boundary(displacement, fx=x.min())
-        >>> left = fem.Boundary(displacement, fx=lambda x: np.isclose(x, x.min()))
+        >>> right = fem.Boundary(displacement, fx=x.max())
+        >>> right = fem.Boundary(displacement, fx=lambda x: np.isclose(x, x.max()))
         >>>
-        >>> plotter = mesh.plot()
+        >>> plotter = pv.Plotter()
         >>> actor = plotter.add_points(
-        ...     np.pad(mesh.points[left.points], ((0, 0), (0, 1))),
+        ...     mesh.points[right.points],
         ...     point_size=20,
         ...     color="red",
         ... )
-        >>> plotter.show()
+        >>> mesh.plot(plotter=plotter, opacity=0.7).show()
 
     If ``fx`` and ``fy`` are given, the masks are combined by *logical-or*.
 
     ..  pyvista-plot::
         :context:
 
         >>> axes = fem.Boundary(displacement, fx=0, fy=0, mode="or")
         >>>
-        >>> plotter = mesh.plot()
+        >>> plotter = pv.Plotter()
         >>> actor = plotter.add_points(
-        ...     np.pad(mesh.points[axes.points], ((0, 0), (0, 1))),
+        ...     mesh.points[axes.points],
         ...     point_size=20,
         ...     color="red",
         ... )
-        >>> plotter.show()
+        >>> mesh.plot(plotter=plotter, opacity=0.7).show()
 
     This may be changed to *logical-and* if desired.
 
     ..  pyvista-plot::
         :context:
 
         >>> center = fem.Boundary(displacement, fx=0, fy=0, mode="and")
         >>>
-        >>> plotter = mesh.plot()
+        >>> plotter = pv.Plotter()
         >>> actor = plotter.add_points(
-        ...     np.pad(mesh.points[center.points], ((0, 0), (0, 1))),
+        ...     mesh.points[center.points],
         ...     point_size=20,
         ...     color="red",
         ... )
-        >>> plotter.show()
+        >>> mesh.plot(plotter=plotter, opacity=0.7).show()
 
     For the most-general case, a user-defined boolean mask for the selection of the
     mesh-points is provided. While the two upper methods are useful to select
     points separated per point-coordinates, providing a mask is more flexible as
     it may involve all three coordinates (or any other quantities of interest).
 
     ..  pyvista-plot::
         :context:
 
-        >>> mask = np.logical_and(np.isclose(x**2 + y**2, 1), x <= 0)
+        >>> mask = np.logical_and(np.isclose(x**2 + y**2, 1), x >= 0)
         >>> surface = fem.Boundary(displacement, mask=mask)
         >>>
-        >>> plotter = mesh.plot()
+        >>> plotter = pv.Plotter()
         >>> actor = plotter.add_points(
-        ...     np.pad(mesh.points[surface.points], ((0, 0), (0, 1))),
+        ...     mesh.points[surface.points],
         ...     point_size=20,
         ...     color="red",
         ... )
-        >>> plotter.show()
+        >>> mesh.plot(plotter=plotter, opacity=0.7).show()
 
     The application of a new mask allows to change the selected points of an existing
     boundary condition.
 
     ..  pyvista-plot::
         :context:
 
-        >>> new_mask = np.logical_and(mask, y >= 0)
+        >>> new_mask = np.logical_and(mask, y <= 0)
         >>> surface.apply_mask(new_mask)
         >>>
-        >>> plotter = mesh.plot()
+        >>> plotter = pv.Plotter()
         >>> actor = plotter.add_points(
-        ...     np.pad(mesh.points[surface.points], ((0, 0), (0, 1))),
+        ...     mesh.points[surface.points],
         ...     point_size=20,
         ...     color="red",
         ... )
-        >>> plotter.show()
+        >>> mesh.plot(plotter=plotter, opacity=0.7).show()
 
     A boundary condition may be skipped on given axes, i.e. if only the x-components
     of a field should be prescribed on the selected points, then the y-axis must
     be skipped.
 
     ..  pyvista-plot::
         :context:
 
         >>> axes_x = fem.Boundary(displacement, fx=0, fy=0, skip=(False, True))
         >>>
-        >>> plotter = mesh.plot()
+        >>> plotter = pv.Plotter()
         >>> actor = plotter.add_points(
-        ...     np.pad(mesh.points[axes_x.points], ((0, 0), (0, 1))),
+        ...     mesh.points[axes_x.points],
         ...     point_size=20,
         ...     color="red",
         ... )
-        >>> plotter.show()
+        >>> mesh.plot(plotter=plotter, opacity=0.7).show()
 
     Values for the prescribed degress of freedom are either applied during creation
     or by the update-method.
 
     ..  pyvista-plot::
         :context:
 
         >>> left = fem.Boundary(displacement, fx=x.min(), value=-0.2)
         >>> left.update(-0.3)
         >>>
-        >>> plotter = mesh.plot()
+        >>> plotter = pv.Plotter()
         >>> actor = plotter.add_points(
-        ...     np.pad(mesh.points[left.points], ((0, 0), (0, 1))),
+        ...     mesh.points[left.points],
         ...     point_size=20,
         ...     color="red",
         ... )
-        >>> plotter.show()
+        >>> mesh.plot(plotter=plotter, opacity=0.7).show()
 
     Sometimes it is useful to create a boundary with all axes skipped. This
     boundary has no prescribed degrees of freedom and hence, is without effect.
     However, it may still be used in a characteristic job for the boundary to be
     tracked.
 
     See Also
```

### Comparing `felupe-8.5.0/src/felupe/dof/_loadcase.py` & `felupe-8.5.1/src/felupe/dof/_loadcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,29 +66,30 @@
     given x-coordinate. The degrees of freedom are prescribed except for the symmetry
     x-axis.
 
     ..  pyvista-plot::
 
         >>> import numpy as np
         >>> import felupe as fem
+        >>> import pyvista as pv
         >>>
         >>> mesh = fem.Circle(radius=1, n=6, sections=[0, 270])
         >>> x, y = mesh.points.T
         >>> region = fem.RegionQuad(mesh)
         >>> displacement = fem.FieldPlaneStrain(region, dim=2)
         >>>
         >>> boundaries = fem.dof.symmetry(displacement, axes=(True, False), x=0.0)
         >>>
-        >>> plotter = mesh.plot()
+        >>> plotter = pv.Plotter()
         >>> actor = plotter.add_points(
         ...     np.pad(mesh.points[boundaries["symx"].points], ((0, 0), (0, 1))),
         ...     point_size=20,
         ...     color="red",
         ... )
-        >>> plotter.show()
+        >>> mesh.plot(plotter=plotter, opacity=0.7).show()
 
     See Also
     --------
     felupe.Boundary : A collection of prescribed degrees of freedom.
     """
 
     # convert axes to array and slice by mesh dimension
```

### Comparing `felupe-8.5.0/src/felupe/dof/_tools.py` & `felupe-8.5.1/src/felupe/dof/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/element/__init__.py` & `felupe-8.5.1/src/felupe/element/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/element/_base.py` & `felupe-8.5.1/src/felupe/element/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/element/_hexahedron.py` & `felupe-8.5.1/src/felupe/element/_hexahedron.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/element/_lagrange.py` & `felupe-8.5.1/src/felupe/element/_lagrange.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/element/_line.py` & `felupe-8.5.1/src/felupe/element/_line.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/element/_quad.py` & `felupe-8.5.1/src/felupe/element/_quad.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/element/_tetra.py` & `felupe-8.5.1/src/felupe/element/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/element/_triangle.py` & `felupe-8.5.1/src/felupe/element/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/field/_axi.py` & `felupe-8.5.1/src/felupe/field/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/field/_base.py` & `felupe-8.5.1/src/felupe/field/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/field/_container.py` & `felupe-8.5.1/src/felupe/field/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/field/_dual.py` & `felupe-8.5.1/src/felupe/field/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/field/_evaluate.py` & `felupe-8.5.1/src/felupe/field/_evaluate.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/field/_fields.py` & `felupe-8.5.1/src/felupe/field/_fields.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/field/_indices.py` & `felupe-8.5.1/src/felupe/field/_indices.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/field/_planestrain.py` & `felupe-8.5.1/src/felupe/field/_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/math/__init__.py` & `felupe-8.5.1/src/felupe/math/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/math/_field.py` & `felupe-8.5.1/src/felupe/math/_field.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/math/_math.py` & `felupe-8.5.1/src/felupe/math/_math.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/math/_solve.py` & `felupe-8.5.1/src/felupe/math/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/math/_spatial.py` & `felupe-8.5.1/src/felupe/math/_spatial.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/math/_tensor.py` & `felupe-8.5.1/src/felupe/math/_tensor.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/__init__.py` & `felupe-8.5.1/src/felupe/mechanics/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_curve.py` & `felupe-8.5.1/src/felupe/mechanics/_curve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_helpers.py` & `felupe-8.5.1/src/felupe/mechanics/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_item.py` & `felupe-8.5.1/src/felupe/mechanics/_item.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_job.py` & `felupe-8.5.1/src/felupe/mechanics/_job.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_multipoint.py` & `felupe-8.5.1/src/felupe/mechanics/_multipoint.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_pointload.py` & `felupe-8.5.1/src/felupe/mechanics/_pointload.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_solidbody.py` & `felupe-8.5.1/src/felupe/mechanics/_solidbody.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_solidbody_gravity.py` & `felupe-8.5.1/src/felupe/mechanics/_solidbody_gravity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_solidbody_incompressible.py` & `felupe-8.5.1/src/felupe/mechanics/_solidbody_incompressible.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_solidbody_pressure.py` & `felupe-8.5.1/src/felupe/mechanics/_solidbody_pressure.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mechanics/_step.py` & `felupe-8.5.1/src/felupe/mechanics/_step.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/__init__.py` & `felupe-8.5.1/src/felupe/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_container.py` & `felupe-8.5.1/src/felupe/mesh/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_convert.py` & `felupe-8.5.1/src/felupe/mesh/_convert.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_discrete_geometry.py` & `felupe-8.5.1/src/felupe/mesh/_discrete_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_dual.py` & `felupe-8.5.1/src/felupe/mesh/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_geometry.py` & `felupe-8.5.1/src/felupe/mesh/_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_helpers.py` & `felupe-8.5.1/src/felupe/mesh/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_line_rectangle_cube.py` & `felupe-8.5.1/src/felupe/mesh/_line_rectangle_cube.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_mesh.py` & `felupe-8.5.1/src/felupe/mesh/_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_read.py` & `felupe-8.5.1/src/felupe/mesh/_read.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/mesh/_tools.py` & `felupe-8.5.1/src/felupe/mesh/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/quadrature/_gausslegendre.py` & `felupe-8.5.1/src/felupe/quadrature/_gausslegendre.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/quadrature/_scheme.py` & `felupe-8.5.1/src/felupe/quadrature/_scheme.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/quadrature/_sphere.py` & `felupe-8.5.1/src/felupe/quadrature/_sphere.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/quadrature/_tetra.py` & `felupe-8.5.1/src/felupe/quadrature/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/quadrature/_triangle.py` & `felupe-8.5.1/src/felupe/quadrature/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/region/__init__.py` & `felupe-8.5.1/src/felupe/region/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/region/_boundary.py` & `felupe-8.5.1/src/felupe/region/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/region/_region.py` & `felupe-8.5.1/src/felupe/region/_region.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/region/_templates.py` & `felupe-8.5.1/src/felupe/region/_templates.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/solve/_solve.py` & `felupe-8.5.1/src/felupe/solve/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/tools/__init__.py` & `felupe-8.5.1/src/felupe/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/tools/_misc.py` & `felupe-8.5.1/src/felupe/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/tools/_newton.py` & `felupe-8.5.1/src/felupe/tools/_newton.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/tools/_plot.py` & `felupe-8.5.1/src/felupe/tools/_plot.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/tools/_post.py` & `felupe-8.5.1/src/felupe/tools/_post.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/tools/_project.py` & `felupe-8.5.1/src/felupe/tools/_project.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/tools/_save.py` & `felupe-8.5.1/src/felupe/tools/_save.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe/tools/_solve.py` & `felupe-8.5.1/src/felupe/tools/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/src/felupe.egg-info/PKG-INFO` & `felupe-8.5.1/src/felupe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 8.5.0
+Version: 8.5.1
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -738,25 +738,26 @@
 </p>
 
 [![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 FElupe is a Python 3.8+ 🐍 finite element analysis package 📦 focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics 🔧 of solid bodies 🚂. Its name is a combination of FE (finite element) and the german word *Lupe* 🔍 (magnifying glass) as a synonym for getting an insight 📖 how a finite element analysis code 🧮 looks like under the hood 🕳️.
 
 <p align="center">
-  <a href="https://felupe.readthedocs.io/en/latest/examples/ex01_beam.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex01_beam_thumb.png" height="160px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/ex02_plate-with-hole.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex02_plate-with-hole_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex03_plasticity.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex03_plasticity_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex04_balloon.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex04_balloon_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex05_rubber-metal-bushing.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex05_rubber-metal-bushing_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex06_rubber-metal-spring.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex06_rubber-metal-spring_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex07_engine-mount.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex07_engine-mount_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex08_shear.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex08_shear_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex09_numeric-continuation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex09_numeric-continuation_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex10_poisson-equation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex10_poisson-equation_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex11_notch-stress.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex11_notch-stress_thumb.png" height="160px"/></a> <a 
-  href="https://felupe.readthedocs.io/en/latest/examples/ex12_foot-bone.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex12_foot-bone_thumb.png" height="160px"/></a>
+  <a href="https://felupe.readthedocs.io/en/latest/examples/ex01_beam.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex01_beam_thumb.png" height="120px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/ex02_plate-with-hole.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex02_plate-with-hole_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex03_plasticity.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex03_plasticity_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex04_balloon.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex04_balloon_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex05_rubber-metal-bushing.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex05_rubber-metal-bushing_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex06_rubber-metal-spring.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex06_rubber-metal-spring_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex07_engine-mount.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex07_engine-mount_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex08_shear.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex08_shear_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex09_numeric-continuation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex09_numeric-continuation_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex10_poisson-equation.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex10_poisson-equation_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex11_notch-stress.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex11_notch-stress_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex12_foot-bone.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex12_foot-bone_thumb.png" height="120px"/></a> <a 
+  href="https://felupe.readthedocs.io/en/latest/examples/ex13_morph-rubber-wheel.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex13_morph-rubber-wheel_thumb.png" height="120px"/></a>
 </p>
 
 # Installation
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
 pip install felupe[all]
```

### Comparing `felupe-8.5.0/src/felupe.egg-info/SOURCES.txt` & `felupe-8.5.1/src/felupe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_basis.py` & `felupe-8.5.1/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_bilinearform.py` & `felupe-8.5.1/tests/test_bilinearform.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_composite.py` & `felupe-8.5.1/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_constitution.py` & `felupe-8.5.1/tests/test_constitution.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_constitution_newton.py` & `felupe-8.5.1/tests/test_constitution_newton.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_dof.py` & `felupe-8.5.1/tests/test_dof.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_element.py` & `felupe-8.5.1/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_field.py` & `felupe-8.5.1/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_form.py` & `felupe-8.5.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_job.py` & `felupe-8.5.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_math.py` & `felupe-8.5.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_mechanics.py` & `felupe-8.5.1/tests/test_mechanics.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_mesh.py` & `felupe-8.5.1/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_mpc.py` & `felupe-8.5.1/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_planestrain.py` & `felupe-8.5.1/tests/test_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_plot.py` & `felupe-8.5.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_quadrature.py` & `felupe-8.5.1/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_readme.py` & `felupe-8.5.1/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_region.py` & `felupe-8.5.1/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_solve.py` & `felupe-8.5.1/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.5.0/tests/test_tools.py` & `felupe-8.5.1/tests/test_tools.py`

 * *Files identical despite different names*

