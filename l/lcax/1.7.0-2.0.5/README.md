# Comparing `tmp/lcax-1.7.0.tar.gz` & `tmp/lcax-2.0.5.tar.gz`

## Comparing `lcax-1.7.0.tar` & `lcax-2.0.5.tar`

### file list

```diff
@@ -1,79 +1,71 @@
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 lcax-1.7.0/Cargo.toml
--rw-r--r--   0     1001      127       11 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/CODEOWNERS
--rw-r--r--   0     1001      127       64 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/FUNDING.yml
--rw-r--r--   0     1001      127      845 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/build_csharp.yaml
--rw-r--r--   0     1001      127      843 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/build_javascript.yaml
--rw-r--r--   0     1001      127     1171 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/build_python.yaml
--rw-r--r--   0     1001      127      659 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/build_rust.yaml
--rw-r--r--   0     1001      127     1849 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/cicd.yaml
--rw-r--r--   0     1001      127     2550 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/create_release.yaml
--rw-r--r--   0     1001      127     1175 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/publish_csharp.yaml
--rw-r--r--   0     1001      127      881 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/publish_javascript.yaml
--rw-r--r--   0     1001      127     1089 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/publish_python.yaml
--rw-r--r--   0     1001      127     2083 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/release_docs.yaml
--rw-r--r--   0     1001      127     3433 2024-04-08 10:17:44.000000 lcax-1.7.0/.gitignore
--rw-r--r--   0     1001      127      886 2024-04-08 10:17:44.000000 lcax-1.7.0/.releaserc.yaml
--rw-r--r--   0     1001      127     4329 2024-04-08 10:17:44.000000 lcax-1.7.0/CHANGELOG.md
--rw-r--r--   0     1001      127      560 2024-04-08 10:17:44.000000 lcax-1.7.0/COPYRIGHT
--rw-r--r--   0     1001      127    21165 2024-04-08 10:17:44.000000 lcax-1.7.0/Cargo.lock
--rw-r--r--   0     1001      127    10173 2024-04-08 10:17:44.000000 lcax-1.7.0/LICENSE
--rw-r--r--   0     1001      127     1555 2024-04-08 10:17:44.000000 lcax-1.7.0/README.md
--rw-r--r--   0     1001      127       79 2024-04-08 10:17:44.000000 lcax-1.7.0/codegen.template.json
--rw-r--r--   0     1001      127     2238 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/CHANGELOG.md
--rw-r--r--   0     1001      127    45567 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/assets/benchmark.png
--rw-r--r--   0     1001      127    23752 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/assets/epdx.png
--rw-r--r--   0     1001      127   253397 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/assets/lcax_structure.png
--rw-r--r--   0     1001      127    13935 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/code/data/lcabyg_project.json
--rw-r--r--   0     1001      127      259 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/code/javascript/usage.js
--rw-r--r--   0     1001      127      527 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/code/python/usage.py
--rw-r--r--   0     1001      127     1341 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/data_structure.md
--rw-r--r--   0     1001      127    16059 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/examples/basic_project.json
--rw-r--r--   0     1001      127      127 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/examples.md
--rw-r--r--   0     1001      127     2104 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/index.md
--rw-r--r--   0     1001      127      122 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/overrides/partials/integrations/analytics/custom.html
--rw-r--r--   0     1001      127      418 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/overrides/stylesheets/extra.css
--rw-r--r--   0     1001      127        0 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/schemas/.gitkeep
--rw-r--r--   0     1001      127      692 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/schemas.md
--rw-r--r--   0     1001      127      157 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/usage.md
--rw-r--r--   0     1001      127     1118 2024-04-08 10:17:44.000000 lcax-1.7.0/mkdocs.yml
--rw-r--r--   0     1001      127     6280 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/csharp/lcax/lcax.cs
--rw-r--r--   0     1001      127      705 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/csharp/lcax/lcax.csproj
--rw-r--r--   0     1001      127    10173 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/LICENSE
--rw-r--r--   0     1001      127     1485 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/README.md
--rw-r--r--   0     1001      127    50825 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/package-lock.json
--rw-r--r--   0     1001      127      753 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/package.json
--rw-r--r--   0     1001      127     3983 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax.d.ts
--rw-r--r--   0     1001      127      139 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax.js
--rw-r--r--   0     1001      127     4563 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax_bg.js
--rw-r--r--   0     1001      127   345131 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax_bg.wasm
--rw-r--r--   0     1001      127      451 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax_bg.wasm.d.ts
--rw-r--r--   0     1001      127      516 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/tests/convertLCAbyg.spec.tsx
--rw-r--r--   0     1001      127    13935 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/tests/datafixtures/lcabyg_project.json
--rw-r--r--   0     1001      127      222 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/vitest.config.js
--rw-r--r--   0     1001      127     1131 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/src/lcax/__init__.py
--rw-r--r--   0     1001      127      149 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/src/lcax/lcax.pyi
--rw-r--r--   0     1001      127    17703 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/src/lcax/lcax.schema.json
--rw-r--r--   0     1001      127    15367 2024-04-08 10:17:45.000000 lcax-1.7.0/packages/python/src/lcax/pydantic.py
--rw-r--r--   0     1001      127    13935 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/tests/datafixtures/lcabyg_project.json
--rw-r--r--   0     1001      127      671 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/tests/test_lcabyg.py
--rw-r--r--   0     1001      127      545 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/tests/test_lcax.py
--rw-r--r--   0     1001      127     2431 2024-04-08 10:17:44.000000 lcax-1.7.0/src/country.rs
--rw-r--r--   0     1001      127      687 2024-04-08 10:17:44.000000 lcax-1.7.0/src/javascript.rs
--rw-r--r--   0     1001      127     4042 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/categories.rs
--rw-r--r--   0     1001      127     2045 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/edges.rs
--rw-r--r--   0     1001      127       66 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/mod.rs
--rw-r--r--   0     1001      127     4004 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/nodes.rs
--rw-r--r--   0     1001      127    12863 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/parse.rs
--rw-r--r--   0     1001      127     1788 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/results.rs
--rw-r--r--   0     1001      127      465 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lib.rs
--rw-r--r--   0     1001      127    11588 2024-04-08 10:17:44.000000 lcax-1.7.0/src/project.rs
--rw-r--r--   0     1001      127      804 2024-04-08 10:17:44.000000 lcax-1.7.0/src/python.rs
--rw-r--r--   0     1001      127      200 2024-04-08 10:17:44.000000 lcax-1.7.0/src/schemars.rs
--rw-r--r--   0     1001      127      686 2024-04-08 10:17:44.000000 lcax-1.7.0/src/utils.rs
--rw-r--r--   0     1001      127    25028 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/datafixtures/lcabyg_example_project.json
--rw-r--r--   0     1001      127  2051524 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/datafixtures/lcabyg_example_results.json
--rw-r--r--   0     1001      127    13935 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/datafixtures/lcabyg_project.json
--rw-r--r--   0     1001      127     1047 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/test_lcax.rs
--rw-r--r--   0     1001      127     2383 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/test_parse_lcabyg.rs
--rw-r--r--   0     1001      127     1311 2024-04-08 10:17:44.000000 lcax-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 lcax-1.7.0/PKG-INFO
+-rw-r--r--   0     1001      127      845 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/Cargo.toml
+-rw-r--r--   0     1001      127     5582 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/ilcd/ilcd.rs
+-rw-r--r--   0     1001      127       29 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/ilcd/mod.rs
+-rw-r--r--   0     1001      127    16269 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/ilcd/parse.rs
+-rw-r--r--   0     1001      127     4042 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/categories.rs
+-rw-r--r--   0     1001      127     2045 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/edges.rs
+-rw-r--r--   0     1001      127       70 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/mod.rs
+-rw-r--r--   0     1001      127     8325 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/nodes.rs
+-rw-r--r--   0     1001      127    13218 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/parse.rs
+-rw-r--r--   0     1001      127     1788 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/results.rs
+-rw-r--r--   0     1001      127       45 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lib.rs
+-rw-r--r--   0     1001      127       30 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/slice/mod.rs
+-rw-r--r--   0     1001      127    13472 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/slice/model.rs
+-rw-r--r--   0     1001      127     5871 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/slice/parse.rs
+-rw-r--r--   0     1001      127      261 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/convert_tests.rs
+-rw-r--r--   0     1001      127    64785 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json
+-rw-r--r--   0     1001      127    68643 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json
+-rw-r--r--   0     1001      127    81962 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json
+-rw-r--r--   0     1001      127    70431 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json
+-rw-r--r--   0     1001      127    70200 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json
+-rw-r--r--   0     1001      127    84820 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json
+-rw-r--r--   0     1001      127    50733 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json
+-rw-r--r--   0     1001      127    80754 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json
+-rw-r--r--   0     1001      127   102497 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json
+-rw-r--r--   0     1001      127   111759 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json
+-rw-r--r--   0     1001      127    87077 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json
+-rw-r--r--   0     1001      127   100644 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json
+-rw-r--r--   0     1001      127    52735 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json
+-rwxr-xr-x   0     1001      127    69619 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
+-rwxr-xr-x   0     1001      127    47820 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json
+-rw-r--r--   0     1001      127     4625 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/test_parse_ilcd.rs
+-rw-r--r--   0     1001      127     2779 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json
+-rw-r--r--   0     1001      127    25028 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json
+-rw-r--r--   0     1001      127  2051524 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json
+-rw-r--r--   0     1001      127    13935 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json
+-rw-r--r--   0     1001      127     1961 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/test_parse_lcabyg.rs
+-rw-r--r--   0     1001      127     2158 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs
+-rw-r--r--   0     1001      127      133 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/slice/datafixtures/results_slice_WLCR.parquet
+-rw-r--r--   0     1001      127      905 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/slice/test_parse_slice.rs
+-rw-r--r--   0     1001      127     1524 2024-05-08 11:58:51.000000 lcax-2.0.5/README.md
+-rw-r--r--   0     1001      127     1135 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/Cargo.toml
+-rw-r--r--   0     1001      127      959 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/assembly.rs
+-rw-r--r--   0     1001      127     4080 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/epd.rs
+-rw-r--r--   0     1001      127      124 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/lib.rs
+-rw-r--r--   0     1001      127     5764 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/life_cycle_base.rs
+-rw-r--r--   0     1001      127     1959 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/product.rs
+-rw-r--r--   0     1001      127     7201 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/project.rs
+-rw-r--r--   0     1001      127     1295 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/shared.rs
+-rw-r--r--   0     1001      127     1296 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/techflow.rs
+-rw-r--r--   0     1001      127      147 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/tests/test_epd.rs
+-rw-r--r--   0     1001      127      168 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/tests/test_project.rs
+-rw-r--r--   0     1001      127      180 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/tests/test_techflow.rs
+-rw-r--r--   0     1001      127      589 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/Cargo.toml
+-rw-r--r--   0     1001      127    20171 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/src/country.rs
+-rw-r--r--   0     1001      127     1391 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/src/dates.rs
+-rw-r--r--   0     1001      127       47 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/src/lib.rs
+-rw-r--r--   0     1001      127      686 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/src/utils.rs
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 lcax-2.0.5/modules/lcax/Cargo.toml
+-rw-r--r--   0     1001      127     1521 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/javascript.rs
+-rw-r--r--   0     1001      127      113 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/lib.rs
+-rw-r--r--   0     1001      127     1551 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/python.rs
+-rw-r--r--   0     1001      127      859 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/rust.rs
+-rw-r--r--   0     1001      127      246 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/schemars.rs
+-rw-r--r--   0     1001      127    35772 2024-05-08 11:58:52.000000 lcax-2.0.5/Cargo.lock
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 lcax-2.0.5/Cargo.toml
+-rw-r--r--   0     1001      127     1441 2024-05-08 11:58:52.000000 lcax-2.0.5/pyproject.toml
+-rw-r--r--   0     1001      127     2825 2024-05-08 11:58:51.000000 lcax-2.0.5/packages/python/src/lcax/__init__.py
+-rw-r--r--   0     1001      127      407 2024-05-08 11:58:52.000000 lcax-2.0.5/packages/python/src/lcax/lcax.pyi
+-rw-r--r--   0     1001      127    14761 2024-05-08 11:58:53.000000 lcax-2.0.5/packages/python/src/lcax/pydantic.py
+-rw-r--r--   0     1001      127    10173 2024-05-08 11:58:51.000000 lcax-2.0.5/LICENSE
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 lcax-2.0.5/PKG-INFO
```

### Comparing `lcax-1.7.0/Cargo.lock` & `lcax-2.0.5/Cargo.lock`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
+name = "ahash"
+version = "0.8.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
+dependencies = [
+ "cfg-if 1.0.0",
+ "const-random",
+ "getrandom",
+ "once_cell",
+ "version_check",
+ "zerocopy",
+]
+
+[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
@@ -26,20 +46,38 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+
+[[package]]
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
+name = "byteorder"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
+
+[[package]]
+name = "bytes"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
+
+[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
@@ -51,23 +89,22 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.33"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f13690e35a5e4ace198e7beea2895d29f3a9cc55015fcebe6336bd2010af9eb"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
- "serde",
  "wasm-bindgen",
  "windows-targets 0.52.0",
 ]
 
 [[package]]
 name = "console_error_panic_hook"
 version = "0.1.7"
@@ -75,40 +112,109 @@
 checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
 dependencies = [
  "cfg-if 1.0.0",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "const-random"
+version = "0.1.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87e00182fe74b066627d63b85fd550ac2998d4b0bd86bfed477a0ae4c7c71359"
+dependencies = [
+ "const-random-macro",
+]
+
+[[package]]
+name = "const-random-macro"
+version = "0.1.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f9d839f2a20b0aee515dc581a6172f2321f96cab76c1a38a4c584a194955390e"
+dependencies = [
+ "getrandom",
+ "once_cell",
+ "tiny-keccak",
+]
+
+[[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
-name = "dyn-clone"
-version = "1.0.11"
+name = "crc32fast"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
+checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+dependencies = [
+ "cfg-if 1.0.0",
+]
 
 [[package]]
-name = "epdx"
-version = "1.2.0"
+name = "crunchy"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c226ab1f4c08095c8a29a808fca08eaa845bf8138a5d74d43621eaf76379e46"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
+name = "csv"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac574ff4d437a7b5ad237ef331c17ccca63c46479e5b5453eb8e10bb99a759fe"
 dependencies = [
- "chrono",
- "pkg-version",
- "schemars",
+ "csv-core",
+ "itoa",
+ "ryu",
  "serde",
- "serde_json",
- "wee_alloc",
 ]
 
 [[package]]
+name = "csv-core"
+version = "0.1.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
+name = "dirs-next"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b98cf8ebf19c3d1b223e151f99a4f9f0690dca41414773390fc824184ac833e1"
+dependencies = [
+ "cfg-if 1.0.0",
+ "dirs-sys-next",
+]
+
+[[package]]
+name = "dirs-sys-next"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4ebda144c4fe02d1f7ea1a7d9641b6fc6b580adcfa024ae48797ecdeb6825b4d"
+dependencies = [
+ "libc",
+ "redox_users",
+ "winapi",
+]
+
+[[package]]
+name = "dyn-clone"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
+
+[[package]]
+name = "encode_unicode"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34aa73646ffb006b8f5147f3dc182bd4bcb190227ce861fc4a4844bf8e3cb2c0"
+
+[[package]]
 name = "field_access"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8964d92be54024fcd6a5ad8c204e85499249acc126a86ea5cabe7686c01af595"
 dependencies = [
  "field_access_derive",
  "paste",
@@ -118,15 +224,38 @@
 name = "field_access_derive"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e474d58478b562f802cf6097e46965bbadbbf4b134d3299aa7c45b91d5e40756"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
+]
+
+[[package]]
+name = "flate2"
+version = "1.0.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
+dependencies = [
+ "crc32fast",
+ "miniz_oxide",
+]
+
+[[package]]
+name = "getrandom"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+dependencies = [
+ "cfg-if 1.0.0",
+ "js-sys",
+ "libc",
+ "wasi",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "gloo-utils"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "037fcb07216cb3a30f7292bd0176b050b7b9a052ba830ef7d5d65f6dc64ba58e"
@@ -135,20 +264,43 @@
  "serde",
  "serde_json",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
+name = "half"
+version = "2.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
+dependencies = [
+ "cfg-if 1.0.0",
+ "crunchy",
+ "num-traits",
+]
+
+[[package]]
+name = "hashbrown"
+version = "0.14.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
+
+[[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
+
+[[package]]
 name = "iana-time-zone"
 version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
@@ -170,14 +322,31 @@
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
+name = "integer-encoding"
+version = "3.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
+
+[[package]]
+name = "is-terminal"
+version = "0.4.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
+dependencies = [
+ "hermit-abi",
+ "libc",
+ "windows-sys",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
 
 [[package]]
 name = "js-sys"
@@ -185,37 +354,106 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "lazy_static"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
+
+[[package]]
 name = "lcax"
-version = "1.7.0"
+version = "2.0.5"
 dependencies = [
  "console_error_panic_hook",
- "epdx",
+ "getrandom",
+ "lcax_convert",
+ "lcax_core",
+ "lcax_models",
+ "pyo3",
+ "schemars",
+ "serde",
+ "serde-wasm-bindgen",
+ "serde_json",
+ "tsify",
+ "wasm-bindgen",
+ "wee_alloc",
+]
+
+[[package]]
+name = "lcax_convert"
+version = "2.0.5"
+dependencies = [
+ "bytes",
+ "chrono",
  "field_access",
+ "lcax_core",
+ "lcax_models",
+ "parquet",
+ "schemars",
+ "serde",
+ "serde_json",
+ "uuid",
+]
+
+[[package]]
+name = "lcax_core"
+version = "2.0.5"
+dependencies = [
+ "chrono",
  "pkg-version",
+ "rust_iso3166",
+ "schemars",
+ "serde",
+ "serde_json",
+]
+
+[[package]]
+name = "lcax_models"
+version = "2.0.5"
+dependencies = [
+ "chrono",
+ "console_error_panic_hook",
+ "lcax_core",
  "pyo3",
  "schemars",
  "serde",
  "serde_json",
  "tsify",
+ "uuid",
  "wasm-bindgen",
  "wee_alloc",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
+name = "libm"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
+
+[[package]]
+name = "libredox"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
+dependencies = [
+ "bitflags 2.5.0",
+ "libc",
+]
+
+[[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -224,14 +462,20 @@
 [[package]]
 name = "log"
 version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
+name = "memchr"
+version = "2.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
+
+[[package]]
 name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
@@ -239,29 +483,112 @@
 [[package]]
 name = "memory_units"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8452105ba047068f40ff7093dd1d9da90898e63dd61736462e9cdda6a90ad3c3"
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
+name = "num"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
+dependencies = [
+ "num-complex",
+ "num-integer",
+ "num-iter",
+ "num-rational",
+ "num-traits",
+]
+
+[[package]]
+name = "num-bigint"
+version = "0.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "num-complex"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "num-integer"
+version = "0.1.46"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "num-iter"
+version = "0.1.44"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "num-rational"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
+ "libm",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
+name = "ordered-float"
+version = "2.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68f19d67e5a2795c94e73e0bb1cc1a7edeb2e28efd39e2e1c9b7a40c1108b11c"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -277,20 +604,83 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.1",
 ]
 
 [[package]]
+name = "parquet"
+version = "51.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "096795d4f47f65fd3ee1ec5a98b77ab26d602f2cc785b0e4be5443add17ecc32"
+dependencies = [
+ "ahash",
+ "bytes",
+ "chrono",
+ "flate2",
+ "half",
+ "hashbrown",
+ "num",
+ "num-bigint",
+ "paste",
+ "seq-macro",
+ "snap",
+ "thrift",
+ "twox-hash",
+]
+
+[[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
+name = "phf"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
+dependencies = [
+ "phf_macros",
+ "phf_shared",
+]
+
+[[package]]
+name = "phf_generator"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "48e4cc64c2ad9ebe670cb8fd69dd50ae301650392e81c05f9bfcb2d5bdbc24b0"
+dependencies = [
+ "phf_shared",
+ "rand",
+]
+
+[[package]]
+name = "phf_macros"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3444646e286606587e49f3bcf1679b8cef1dc2c5ecc29ddacaffc305180d464b"
+dependencies = [
+ "phf_generator",
+ "phf_shared",
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "phf_shared"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
+dependencies = [
+ "siphasher",
+]
+
+[[package]]
 name = "pkg-version"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e848f61ee4b2010345e65757e427a077213af1cee5d3e6a02e4a151dabca377"
 dependencies = [
  "pkg-version-impl",
  "proc-macro-hack",
@@ -308,14 +698,28 @@
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
+name = "prettytable-rs"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eea25e07510aa6ab6547308ebe3c036016d162b8da920dbb079e3ba8acf3d95a"
+dependencies = [
+ "csv",
+ "encode_unicode",
+ "is-terminal",
+ "lazy_static",
+ "term",
+ "unicode-width",
+]
+
+[[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
@@ -324,17 +728,17 @@
 checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if 1.0.0",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -342,181 +746,255 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+
+[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_users"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
+dependencies = [
+ "getrandom",
+ "libredox",
+ "thiserror",
+]
+
+[[package]]
+name = "rust_iso3166"
+version = "0.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e676677b94480848a8d88c74553bad50aed2ee77d8c0985aa50d8c4e26f3054b"
+dependencies = [
+ "js-sys",
+ "phf",
+ "prettytable-rs",
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "rustversion"
+version = "1.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
+
+[[package]]
 name = "ryu"
-version = "1.0.14"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "schemars"
-version = "0.8.16"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45a28f4c49489add4ce10783f7911893516f15afe45d015608d41faca6bc4d29"
+checksum = "fc6e7ed6919cb46507fb01ff1654309219f62b4d603822501b0b80d42f6f21ef"
 dependencies = [
  "chrono",
  "dyn-clone",
  "schemars_derive",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "schemars_derive"
-version = "0.8.16"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c767fd6fa65d9ccf9cf026122c1b555f2ef9a4f0cea69da4d7dbc3e258d30967"
+checksum = "185f2b7aa7e02d418e453790dde16890256bbd2bcd04b7dc5348811052b53f49"
 dependencies = [
  "proc-macro2",
  "quote",
- "serde_derive_internals 0.26.0",
- "syn 1.0.109",
+ "serde_derive_internals 0.29.0",
+ "syn",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
+name = "seq-macro"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
+
+[[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
+name = "serde-wasm-bindgen"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8302e169f0eddcc139c70f139d19d6467353af16f9fce27e8c30158036a1e16b"
+dependencies = [
+ "js-sys",
+ "serde",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "serde_derive_internals"
-version = "0.26.0"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
+checksum = "e578a843d40b4189a4d66bba51d7684f57da5bd7c304c64e14bd63efbef49509"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "serde_derive_internals"
-version = "0.28.0"
+version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e578a843d40b4189a4d66bba51d7684f57da5bd7c304c64e14bd63efbef49509"
+checksum = "330f01ce65a3a5fe59a60c82f3c9a024b573b8a6e875bd233fe5f934e71d54e3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.113"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69801b70b1c3dac963ecb03a364ba0ceda9cf60c71cfe475e99864759c8b8a79"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "sha1_smol"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae1a47186c03a32177042e55dbc5fd5aee900b8e0069a8d70fba96a9375cd012"
+
+[[package]]
+name = "siphasher"
+version = "0.3.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38b58827f4464d87d377d175e90bf58eb00fd8716ff0a62f80356b5e61555d0d"
+
+[[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
-name = "syn"
-version = "1.0.109"
+name = "snap"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
+checksum = "1b6b67fb9a61334225b5b790716f609cd58395f895b3fe8b328786812a40bc3b"
+
+[[package]]
+name = "static_assertions"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "syn"
 version = "2.0.48"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
 dependencies = [
@@ -528,14 +1006,65 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
+name = "term"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c59df8ac95d96ff9bede18eb7300b0fda5e5d8d90960e76f8e14ae765eedbf1f"
+dependencies = [
+ "dirs-next",
+ "rustversion",
+ "winapi",
+]
+
+[[package]]
+name = "thiserror"
+version = "1.0.59"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+dependencies = [
+ "thiserror-impl",
+]
+
+[[package]]
+name = "thiserror-impl"
+version = "1.0.59"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "thrift"
+version = "0.17.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
+dependencies = [
+ "byteorder",
+ "integer-encoding",
+ "ordered-float",
+]
+
+[[package]]
+name = "tiny-keccak"
+version = "2.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
+dependencies = [
+ "crunchy",
+]
+
+[[package]]
 name = "tsify"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d6b26cf145f2f3b9ff84e182c448eaf05468e247f148cf3d2a7d67d78ff023a0"
 dependencies = [
  "gloo-utils",
  "serde",
@@ -549,82 +1078,120 @@
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a94b0f0954b3e59bfc2c246b4c8574390d94a4ad4ad246aaf2fb07d7dfd3b47"
 dependencies = [
  "proc-macro2",
  "quote",
  "serde_derive_internals 0.28.0",
- "syn 2.0.48",
+ "syn",
+]
+
+[[package]]
+name = "twox-hash"
+version = "1.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
+dependencies = [
+ "cfg-if 1.0.0",
+ "static_assertions",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
+name = "unicode-width"
+version = "0.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
+
+[[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
+name = "uuid"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
+dependencies = [
+ "getrandom",
+ "sha1_smol",
+]
+
+[[package]]
+name = "version_check"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+
+[[package]]
+name = "wasi"
+version = "0.11.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
+
+[[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if 1.0.0",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "web-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
@@ -672,14 +1239,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets 0.48.1",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.0",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm 0.48.0",
  "windows_aarch64_msvc 0.48.0",
@@ -784,7 +1360,27 @@
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+
+[[package]]
+name = "zerocopy"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+dependencies = [
+ "zerocopy-derive",
+]
+
+[[package]]
+name = "zerocopy-derive"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
```

### Comparing `lcax-1.7.0/LICENSE` & `lcax-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lcax-1.7.0/README.md` & `lcax-2.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
 ```bash
 maturin develop --extras tests,codegen --target x86_64-unknown-linux-gnu
 source .venv/bin/activate .
 
 datamodel-codegen \
 --input lcax.schema.json \
---input-file-type jsonschema \
 --output packages/python/src/lcax/pydantic.py
           
 cd packages/python
 pytest tests/
 ```
 
 ## Build Documentation
```

### Comparing `lcax-1.7.0/docs/code/data/lcabyg_project.json` & `lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json`

 * *Files identical despite different names*

### Comparing `lcax-1.7.0/packages/python/src/lcax/__init__.py` & `lcax-2.0.5/packages/python/src/lcax/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
+from pathlib import Path
 from typing import Type, TypeVar
 
 from .lcax import *
 from .pydantic import *
 
 __doc__ = lcax.__doc__
 if hasattr(lcax, "__all__"):
     __all__ = lcax.__all__
 
-T = TypeVar("T", str, dict, LCAxProject)
+Project_Type = TypeVar("Project_Type", str, dict, Project)
 
 
-def convert_lcabyg(data: str | dict, result_data: str | dict | None = None, *, as_type: Type[T] = dict) -> T:
+def convert_lcabyg(data: str | dict, result_data: str | dict | None = None, *, as_type: Type[Project_Type] = dict) -> Project_Type:
     """
     Converts json formatted LCAbyg data into a LCAx project
 
     The LCAx project can either be returned as a string, a dict or a Pydantic class.
     """
 
     if isinstance(data, dict):
@@ -29,15 +30,71 @@
     except Exception as err:
         raise ParsingException(err)
 
     if as_type == str:
         return _project
     elif as_type == dict:
         return json.loads(_project)
-    elif as_type == LCAxProject:
-        return LCAxProject(**json.loads(_project))
+    elif as_type == Project:
+        return Project(**json.loads(_project))
     else:
         raise NotImplementedError("Currently only 'dict', 'str' and 'lcax.LCAxProject' is implemented as_type.")
 
 
+EPD_Type = TypeVar("EPD_Type", str, dict, EPD)
+
+
+def convert_ilcd(data: str | dict, *, as_type: Type[EPD_Type] = dict) -> EPD_Type:
+    """
+    Converts a json formatted ILCD+EPD data into EPDx
+
+    The EPDx data can either be returned as a string, a dict or a Pydantic class.
+    """
+
+    if isinstance(data, dict):
+        data = json.dumps(data)
+
+    try:
+        _epd = lcax._convert_ilcd(data)
+    except Exception as err:
+        raise ParsingException(err)
+
+    if as_type == str:
+        return _epd
+    elif as_type == dict:
+        return json.loads(_epd)
+    elif as_type == EPD:
+        return EPD(**json.loads(_epd))
+    else:
+        raise NotImplementedError("Currently only 'dict', 'str' and 'lcax.EPD' is implemented as_type.")
+
+
+def convert_slice(path: str | Path, *, as_type: Type[Project_Type] = dict) -> list[Project_Type]:
+    """
+    Converts a SLiCE .parquet file into a list of LCAx projects
+
+    The LCAx project can either be returned as a list of strings, dicts or Pydantic classes.
+    """
+
+    if isinstance(path, str):
+        path = Path(path)
+
+    if not path.is_file():
+        raise FileNotFoundError(f"File not found: {path}")
+
+    try:
+        projects = lcax._convert_slice(str(path))
+    except Exception as err:
+        raise ParsingException(err)
+
+    if as_type == str:
+        return projects
+    elif as_type == dict:
+        return [json.loads(project) for project in projects]
+    elif as_type == EPD:
+        return [Project(**json.loads(project)) for project in projects]
+    else:
+        raise NotImplementedError("Currently only 'dict', 'str' and 'lcax.EPD' is implemented as_type.")
+
+
 class ParsingException(Exception):
     ...
```

### Comparing `lcax-1.7.0/src/lcabyg/categories.rs` & `lcax-2.0.5/modules/convert/src/lcabyg/categories.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.7.0/src/lcabyg/edges.rs` & `lcax-2.0.5/modules/convert/src/lcabyg/edges.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.7.0/src/lcabyg/parse.rs` & `lcax-2.0.5/modules/convert/src/lcabyg/parse.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-use crate::country::Country;
-use epdx::epd::{Unit, EPD};
-use field_access::FieldAccess;
-use serde::{Deserialize, Deserializer, Serialize};
-use serde_json::Error;
-use std::collections::HashMap;
-
 use crate::lcabyg::edges::EdgeType;
-use crate::lcabyg::nodes::Node;
+use crate::lcabyg::nodes::{epd_from_lcabyg_stages, Node};
 use crate::lcabyg::results::Model::InstanceModel;
 use crate::lcabyg::results::{LCAbygResults, YearResult};
 use crate::lcabyg::{categories, edges, nodes};
-use crate::project::*;
-use crate::utils::get_version;
+use field_access::FieldAccess;
+use lcax_core::country::Country;
+use lcax_core::utils::get_version;
+use lcax_models::assembly::{Assembly, Classification};
+use lcax_models::life_cycle_base::{ImpactCategoryKey, LifeCycleStage};
+use lcax_models::product::{ImpactDataSource, Product as LCAxProduct};
+use lcax_models::project::{
+    AreaType, BuildingInfo, BuildingType, BuildingTypology, GeneralEnergyClass, Location,
+    Project as LCAxProject, ProjectInfo, RoofType, SoftwareInfo,
+};
+use lcax_models::shared::Unit;
+use serde::{Deserialize, Serialize};
+use serde_json::Error;
+use std::collections::HashMap;
 
 type Edge = (EdgeType, String, String);
 
 #[derive(Deserialize, Serialize)]
-enum NodesAndEdges {
+pub enum NodesAndEdges {
     Node(Node),
     Edge(Edge),
 }
 
 /// Parse an LCAByg project exported as json files.
 ///
 /// # Arguments
@@ -105,15 +110,15 @@
 ) {
     lcax_project.results = collect_lcabyg_object_results(
         building_id,
         results,
         &lcax_project.impact_categories,
         &lcax_project.life_cycle_stages,
     );
-    for (assembly_id, mut assembly) in &mut lcax_project.assemblies {
+    for (assembly_id, assembly) in &mut lcax_project.assemblies {
         assembly.results = collect_lcabyg_object_results(
             &get_result_id(assembly_id, results),
             results,
             &lcax_project.impact_categories,
             &lcax_project.life_cycle_stages,
         )
     }
@@ -279,17 +284,15 @@
                 );
                 if found == (false, true) {
                     break;
                 } else {
                     found = (true, false);
                 }
             }
-            (EdgeType::CategoryToElement(category_edge), category_id, element_id)
-                if element_id == &node_id =>
-            {
+            (EdgeType::CategoryToElement(_), category_id, element_id) if element_id == &node_id => {
                 assembly.classification = Some(get_lcabyg_classification(category_id));
                 if found == (true, false) {
                     break;
                 } else {
                     found = (false, true);
                 }
             }
@@ -344,42 +347,42 @@
     }
 }
 
 fn add_construction_to_product_data(
     product_id: &String,
     edge: &edges::ConstructionToProductEdge,
     nodes: &Vec<Node>,
-) -> Product {
-    let mut product = Product {
+) -> LCAxProduct {
+    let mut product = LCAxProduct {
         id: product_id.clone(),
         name: "".to_string(),
         description: "".to_string(),
         reference_service_life: edge.lifespan,
         impact_data: Default::default(),
         quantity: edge.amount,
         unit: Unit::from(&edge.unit),
         transport: None,
         results: None,
         meta_data: None,
     };
 
-    let mut stages: Vec<epdx::lcabyg::Stage> = vec![];
+    let mut stages: Vec<nodes::Stage> = vec![];
 
     for node in nodes {
         match node {
             Node::Product(product_node) => {
                 product.name = product_node.name.english.clone().unwrap();
                 product.description = product_node.comment.english.clone().unwrap();
             }
             Node::Stage(stage_node) => stages.append(&mut vec![stage_node.clone()]),
             _ => continue,
         }
     }
 
-    let epd_data = EPD::from(&stages);
+    let epd_data = epd_from_lcabyg_stages(&stages);
 
     product.impact_data = ImpactDataSource::EPD(epd_data);
     product
 }
 
 fn get_lcabyg_classification(category_id: &str) -> Vec<Classification> {
     vec![Classification {
```

### Comparing `lcax-1.7.0/src/lcabyg/results.rs` & `lcax-2.0.5/modules/convert/src/lcabyg/results.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.7.0/src/utils.rs` & `lcax-2.0.5/modules/core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.7.0/tests/datafixtures/lcabyg_example_project.json` & `lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json`

 * *Files identical despite different names*

### Comparing `lcax-1.7.0/tests/datafixtures/lcabyg_example_results.json` & `lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json`

 * *Files identical despite different names*

### Comparing `lcax-1.7.0/pyproject.toml` & `lcax-2.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 license = { file = "LICENSE" }
 authors = [
     { name = "Christian Kongsgaard", email = "christian@kongsgaard.eu" },
 ]
 
 dependencies = [
     "cffi",
-    "pydantic >=1.8.2,<2.0.0",
+    "pydantic >2.0.0",
 ]
 
 [project.optional-dependencies]
 doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
     "mdx-include >=1.4.1,<2.0.0",
 ]
@@ -28,27 +28,31 @@
 
 [project.urls]
 homepage = "https://lcax.kongsgaard.eu"
 documentation = "https://lcax.kongsgaard.eu"
 repository = "https://github.com/ocni-dtu/lcax"
 
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [tool.maturin]
 # "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
 features = ["pybindings"]
 python-source = "packages/python/src"
+manifest-path = "modules/lcax/Cargo.toml"
 
 [tool.pytest.ini_options]
 pythonpath = "packages/python/src"
 testpaths = ["packages/python/tests/"]
 
 [tool.datamodel-codegen]
 field-constraints = true
 snake-case-field = true
 strip-default-none = false
 target-python-version = "3.10"
 collapse-root-models = true
 disable-timestamp = true
-extra-template-data = "codegen.template.json"
+capitalise-enum-members = true
+input-file-type = "jsonschema"
+output-model-type = "pydantic_v2.BaseModel"
+allow_population_by_field_name = true
```

### Comparing `lcax-1.7.0/PKG-INFO` & `lcax-2.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: lcax
-Version: 1.7.0
+Version: 2.0.5
 Requires-Dist: cffi
-Requires-Dist: pydantic >=1.8.2, <2.0.0
+Requires-Dist: pydantic >2.0.0
 Requires-Dist: mkdocs-material >=8.1.4, <9.0.0 ; extra == 'doc'
 Requires-Dist: mdx-include >=1.4.1, <2.0.0 ; extra == 'doc'
 Requires-Dist: datamodel-code-generator ; extra == 'codegen'
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: pytest-datafixtures ; extra == 'tests'
 Provides-Extra: doc
 Provides-Extra: codegen
@@ -68,15 +68,14 @@
 
 ```bash
 maturin develop --extras tests,codegen --target x86_64-unknown-linux-gnu
 source .venv/bin/activate .
 
 datamodel-codegen \
 --input lcax.schema.json \
---input-file-type jsonschema \
 --output packages/python/src/lcax/pydantic.py
           
 cd packages/python
 pytest tests/
 ```
 
 ## Build Documentation
```

