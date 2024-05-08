# Comparing `tmp/pelicun-3.3.2.tar.gz` & `tmp/pelicun-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelicun-3.3.2.tar", last modified: Tue Apr 30 01:37:31 2024, max compression
+gzip compressed data, was "pelicun-3.3.3.tar", last modified: Wed May  8 06:21:23 2024, max compression
```

## Comparing `pelicun-3.3.2.tar` & `pelicun-3.3.3.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.106868 pelicun-3.3.2/
--rw-r--r--   0 adamzs     (504) staff       (20)     1661 2022-12-05 20:30:08.000000 pelicun-3.3.2/LICENSE
--rw-r--r--   0 adamzs     (504) staff       (20)      486 2024-04-04 20:31:52.000000 pelicun-3.3.2/MANIFEST.in
--rw-r--r--   0 adamzs     (504) staff       (20)    21964 2024-04-30 01:37:31.106529 pelicun-3.3.2/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)    20703 2024-04-04 20:38:24.000000 pelicun-3.3.2/README.md
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.053395 pelicun-3.3.2/pelicun/
--rw-r--r--   0 adamzs     (504) staff       (20)     2012 2024-04-30 01:07:33.000000 pelicun-3.3.2/pelicun/__init__.py
--rw-r--r--   0 adamzs     (504) staff       (20)     7284 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/assessment.py
--rw-r--r--   0 adamzs     (504) staff       (20)     3684 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/auto.py
--rw-r--r--   0 adamzs     (504) staff       (20)    38835 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/base.py
--rw-r--r--   0 adamzs     (504) staff       (20)   104242 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/db.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.047481 pelicun-3.3.2/pelicun/examples/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.055884 pelicun-3.3.2/pelicun/examples/001/
--rw-r--r--   0 adamzs     (504) staff       (20)     5011 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/001/CMP_QNT.csv
--rw-r--r--   0 adamzs     (504) staff       (20)    11827 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/001/demands_s4.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     2149 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/001/input.json
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.057178 pelicun-3.3.2/pelicun/examples/002/
--rw-r--r--   0 adamzs     (504) staff       (20)      211 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/002/CMP_QNT.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      902 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/002/input.json
--rw-r--r--   0 adamzs     (504) staff       (20)     4139 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/002/response.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.059019 pelicun-3.3.2/pelicun/examples/0_tmp/
--rw-r--r--   0 adamzs     (504) staff       (20)      652 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/CMP_marginals.csv
--rw-r--r--   0 adamzs     (504) staff       (20)       52 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/DMG_process_P58.json
--rw-r--r--   0 adamzs     (504) staff       (20)      347 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/LOSS_map.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     2782 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/config.json
--rw-r--r--   0 adamzs     (504) staff       (20)     3892 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/demands.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      890 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/fragility_Additional.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      158 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/repair_Additional.csv
--rw-r--r--   0 adamzs     (504) staff       (20)    16427 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/file_io.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.061578 pelicun-3.3.2/pelicun/model/
--rw-r--r--   0 adamzs     (504) staff       (20)     2010 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/__init__.py
--rw-r--r--   0 adamzs     (504) staff       (20)    15084 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/asset_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)    60323 2024-04-30 01:02:56.000000 pelicun-3.3.2/pelicun/model/damage_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)    33061 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/demand_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)    40848 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/loss_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)     8855 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/pelicun_model.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.048043 pelicun-3.3.2/pelicun/resources/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.084927 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/
--rw-r--r--   0 adamzs     (504) staff       (20)    80663 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv
--rw-r--r--   0 adamzs     (504) staff       (20)  1167069 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json
--rw-r--r--   0 adamzs     (504) staff       (20)    36386 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   881431 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json
--rw-r--r--   0 adamzs     (504) staff       (20)     9616 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   183256 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json
--rw-r--r--   0 adamzs     (504) staff       (20)     4297 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv
--rw-r--r--   0 adamzs     (504) staff       (20)    52505 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json
--rw-r--r--   0 adamzs     (504) staff       (20)     2203 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     3921 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv
--rw-r--r--   0 adamzs     (504) staff       (20)    18199 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json
--rw-r--r--   0 adamzs     (504) staff       (20)  3714342 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   521287 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv
--rw-r--r--   0 adamzs     (504) staff       (20)  1132502 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json
--rw-r--r--   0 adamzs     (504) staff       (20)     8934 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   262248 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json
--rw-r--r--   0 adamzs     (504) staff       (20)     5912 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   204054 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json
--rw-r--r--   0 adamzs     (504) staff       (20)      302 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     3873 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json
--rw-r--r--   0 adamzs     (504) staff       (20)  2118028 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.089131 pelicun-3.3.2/pelicun/resources/auto/
--rw-r--r--   0 adamzs     (504) staff       (20)    31025 2024-04-30 01:01:03.000000 pelicun-3.3.2/pelicun/resources/auto/Hazus_Earthquake_IM.py
--rw-r--r--   0 adamzs     (504) staff       (20)     9220 2024-04-30 01:01:14.000000 pelicun-3.3.2/pelicun/resources/auto/Hazus_Earthquake_Story.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.091216 pelicun-3.3.2/pelicun/settings/
--rw-r--r--   0 adamzs     (504) staff       (20)      661 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/settings/default_config.json
--rw-r--r--   0 adamzs     (504) staff       (20)     1610 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/settings/default_units.json
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.094348 pelicun-3.3.2/pelicun/tests/
--rw-r--r--   0 adamzs     (504) staff       (20)     3113 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/code_repetition_checker.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.049053 pelicun-3.3.2/pelicun/tests/data/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.048627 pelicun-3.3.2/pelicun/tests/data/assessment/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.094674 pelicun-3.3.2/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/
--rw-r--r--   0 adamzs     (504) staff       (20)       55 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/custom_units.json
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.048801 pelicun-3.3.2/pelicun/tests/data/base/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.098077 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/
--rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/additional_units_a.json
--rw-r--r--   0 adamzs     (504) staff       (20)     1547 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/duplicate.json
--rw-r--r--   0 adamzs     (504) staff       (20)     1531 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/duplicate2.json
--rw-r--r--   0 adamzs     (504) staff       (20)       43 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/invalid.json
--rw-r--r--   0 adamzs     (504) staff       (20)       26 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/not_dict.json
--rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/not_float.json
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.048968 pelicun-3.3.2/pelicun/tests/data/file_io/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.099417 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/
--rw-r--r--   0 adamzs     (504) staff       (20)     1537 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/no_units.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      372 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/orient_1.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      445 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/orient_1_units.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     1641 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/units.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.049966 pelicun-3.3.2/pelicun/tests/data/model/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.100894 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/
--rwxr-xr-x   0 adamzs     (504) staff       (20)      108 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      317 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals_2.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      125 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals_block_weights.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      116 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_dir.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      111 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_loc.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.101129 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/
--rw-r--r--   0 adamzs     (504) staff       (20)      229 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/demand_sample.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.101616 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/
--rw-r--r--   0 adamzs     (504) staff       (20)      208 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/demand_sample.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.102032 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/
--rw-r--r--   0 adamzs     (504) staff       (20)      237 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/damage_model.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.102746 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/
--rwxr-xr-x   0 adamzs     (504) staff       (20)       75 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      109 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals_2.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      249 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/fragility_DB_test.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.102975 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_estimate_RID/
--rw-r--r--   0 adamzs     (504) staff       (20)       51 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_estimate_RID/demand_sample_A.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.103185 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/
--rw-r--r--   0 adamzs     (504) staff       (20)      138 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/sample.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.104055 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/
--rw-r--r--   0 adamzs     (504) staff       (20)      162 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_A.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_B.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_C.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_D.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     5729 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/reset_tests.py
--rw-r--r--   0 adamzs     (504) staff       (20)     5155 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_assessment.py
--rw-r--r--   0 adamzs     (504) staff       (20)     4416 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_auto.py
--rw-r--r--   0 adamzs     (504) staff       (20)    26202 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_base.py
--rw-r--r--   0 adamzs     (504) staff       (20)     7915 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_file_io.py
--rw-r--r--   0 adamzs     (504) staff       (20)    76806 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)    46929 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_uq.py
--rw-r--r--   0 adamzs     (504) staff       (20)     3298 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/util.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.105387 pelicun-3.3.2/pelicun/tools/
--rw-r--r--   0 adamzs     (504) staff       (20)    70920 2024-04-30 01:07:19.000000 pelicun-3.3.2/pelicun/tools/DL_calculation.py
--rw-r--r--   0 adamzs     (504) staff       (20)     2411 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tools/HDF_to_CSV.py
--rw-r--r--   0 adamzs     (504) staff       (20)     3256 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tools/export_DB.py
--rw-r--r--   0 adamzs     (504) staff       (20)    76038 2024-04-30 01:15:29.000000 pelicun-3.3.2/pelicun/uq.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.105849 pelicun-3.3.2/pelicun.egg-info/
--rw-r--r--   0 adamzs     (504) staff       (20)    21964 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)     4829 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/SOURCES.txt
--rw-r--r--   0 adamzs     (504) staff       (20)        1 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/dependency_links.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       62 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/entry_points.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       74 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/requires.txt
--rw-r--r--   0 adamzs     (504) staff       (20)        8 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/top_level.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-30 01:37:31.106938 pelicun-3.3.2/setup.cfg
--rw-r--r--   0 adamzs     (504) staff       (20)     2162 2024-04-30 01:27:58.000000 pelicun-3.3.2/setup.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.891991 pelicun-3.3.3/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1661 2022-12-05 20:30:08.000000 pelicun-3.3.3/LICENSE
+-rw-r--r--   0 adamzs     (504) staff       (20)      486 2024-04-04 20:31:52.000000 pelicun-3.3.3/MANIFEST.in
+-rw-r--r--   0 adamzs     (504) staff       (20)    22472 2024-05-08 06:21:23.891525 pelicun-3.3.3/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)    20617 2024-05-07 20:53:01.000000 pelicun-3.3.3/README.md
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.837390 pelicun-3.3.3/pelicun/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1992 2024-05-08 06:21:05.000000 pelicun-3.3.3/pelicun/__init__.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     7858 2024-05-07 20:56:35.000000 pelicun-3.3.3/pelicun/assessment.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     4492 2024-05-07 20:56:56.000000 pelicun-3.3.3/pelicun/auto.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    47268 2024-05-07 20:57:12.000000 pelicun-3.3.3/pelicun/base.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    95101 2024-05-07 20:57:43.000000 pelicun-3.3.3/pelicun/db.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.830595 pelicun-3.3.3/pelicun/examples/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.839798 pelicun-3.3.3/pelicun/examples/001/
+-rw-r--r--   0 adamzs     (504) staff       (20)     5011 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/001/CMP_QNT.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    11827 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/001/demands_s4.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     2149 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/001/input.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.840791 pelicun-3.3.3/pelicun/examples/002/
+-rw-r--r--   0 adamzs     (504) staff       (20)      211 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/002/CMP_QNT.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      902 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/002/input.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     4139 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/002/response.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.843582 pelicun-3.3.3/pelicun/examples/0_tmp/
+-rw-r--r--   0 adamzs     (504) staff       (20)      652 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/0_tmp/CMP_marginals.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)       52 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/0_tmp/DMG_process_P58.json
+-rw-r--r--   0 adamzs     (504) staff       (20)      347 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/0_tmp/LOSS_map.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     2782 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/0_tmp/config.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     3892 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/0_tmp/demands.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      890 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/0_tmp/fragility_Additional.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      158 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/examples/0_tmp/repair_Additional.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    17145 2024-05-07 20:58:14.000000 pelicun-3.3.3/pelicun/file_io.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.846612 pelicun-3.3.3/pelicun/model/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2010 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/model/__init__.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    24282 2024-05-07 20:59:42.000000 pelicun-3.3.3/pelicun/model/asset_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    65903 2024-05-07 20:59:42.000000 pelicun-3.3.3/pelicun/model/damage_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    38762 2024-05-07 20:59:42.000000 pelicun-3.3.3/pelicun/model/demand_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    44003 2024-05-07 20:59:42.000000 pelicun-3.3.3/pelicun/model/loss_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     8756 2024-05-07 20:59:42.000000 pelicun-3.3.3/pelicun/model/pelicun_model.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.830942 pelicun-3.3.3/pelicun/resources/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.870925 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/
+-rw-r--r--   0 adamzs     (504) staff       (20)    80663 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)  1167069 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json
+-rw-r--r--   0 adamzs     (504) staff       (20)    36386 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   881431 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     9616 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   183256 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     4297 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    52505 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     2203 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     3921 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    18199 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json
+-rw-r--r--   0 adamzs     (504) staff       (20)  3714342 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    12543 2024-05-07 20:53:01.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg_template.json
+-rw-r--r--   0 adamzs     (504) staff       (20)   521287 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)  1132502 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     8934 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   262248 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     5912 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   204054 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json
+-rw-r--r--   0 adamzs     (504) staff       (20)      302 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     3873 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json
+-rw-r--r--   0 adamzs     (504) staff       (20)  2118028 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.875139 pelicun-3.3.3/pelicun/resources/auto/
+-rw-r--r--   0 adamzs     (504) staff       (20)    30851 2024-05-07 20:59:22.000000 pelicun-3.3.3/pelicun/resources/auto/Hazus_Earthquake_IM.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     9228 2024-05-07 20:59:22.000000 pelicun-3.3.3/pelicun/resources/auto/Hazus_Earthquake_Story.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.877502 pelicun-3.3.3/pelicun/settings/
+-rw-r--r--   0 adamzs     (504) staff       (20)      741 2024-05-07 20:53:01.000000 pelicun-3.3.3/pelicun/settings/default_config.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     1610 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/settings/default_units.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.881290 pelicun-3.3.3/pelicun/tests/
+-rw-r--r--   0 adamzs     (504) staff       (20)     3113 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/code_repetition_checker.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.831750 pelicun-3.3.3/pelicun/tests/data/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.831355 pelicun-3.3.3/pelicun/tests/data/assessment/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.881651 pelicun-3.3.3/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/
+-rw-r--r--   0 adamzs     (504) staff       (20)       55 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/custom_units.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.831508 pelicun-3.3.3/pelicun/tests/data/base/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.883497 pelicun-3.3.3/pelicun/tests/data/base/test_parse_units/
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/base/test_parse_units/additional_units_a.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     1547 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/base/test_parse_units/duplicate.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     1531 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/base/test_parse_units/duplicate2.json
+-rw-r--r--   0 adamzs     (504) staff       (20)       43 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/base/test_parse_units/invalid.json
+-rw-r--r--   0 adamzs     (504) staff       (20)       26 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/base/test_parse_units/not_dict.json
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/base/test_parse_units/not_float.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.831663 pelicun-3.3.3/pelicun/tests/data/file_io/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.884543 pelicun-3.3.3/pelicun/tests/data/file_io/test_load_data/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1537 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/file_io/test_load_data/no_units.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      372 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/file_io/test_load_data/orient_1.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      445 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/file_io/test_load_data/orient_1_units.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     1641 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/file_io/test_load_data/units.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.832417 pelicun-3.3.3/pelicun/tests/data/model/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.885637 pelicun-3.3.3/pelicun/tests/data/model/test_AssetModel/
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      108 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      317 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals_2.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      125 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals_block_weights.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      116 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_dir.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      111 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_loc.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.885843 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/
+-rw-r--r--   0 adamzs     (504) staff       (20)      229 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/demand_sample.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.886031 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/
+-rw-r--r--   0 adamzs     (504) staff       (20)      208 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/demand_sample.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.886238 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/
+-rw-r--r--   0 adamzs     (504) staff       (20)      237 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/damage_model.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.887047 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/
+-rwxr-xr-x   0 adamzs     (504) staff       (20)       75 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      109 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals_2.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      249 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/fragility_DB_test.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.887297 pelicun-3.3.3/pelicun/tests/data/model/test_DemandModel_estimate_RID/
+-rw-r--r--   0 adamzs     (504) staff       (20)       51 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DemandModel_estimate_RID/demand_sample_A.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.887604 pelicun-3.3.3/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/
+-rw-r--r--   0 adamzs     (504) staff       (20)      138 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/sample.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.888609 pelicun-3.3.3/pelicun/tests/data/model/test_DemandModel_load_sample/
+-rw-r--r--   0 adamzs     (504) staff       (20)      162 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_A.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_B.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_C.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_D.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     5717 2024-05-07 20:58:49.000000 pelicun-3.3.3/pelicun/tests/reset_tests.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     5155 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/test_assessment.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     4396 2024-05-07 20:58:49.000000 pelicun-3.3.3/pelicun/tests/test_auto.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    26333 2024-05-07 20:58:49.000000 pelicun-3.3.3/pelicun/tests/test_base.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     7901 2024-05-07 20:58:49.000000 pelicun-3.3.3/pelicun/tests/test_file_io.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    76382 2024-05-07 20:58:50.000000 pelicun-3.3.3/pelicun/tests/test_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    46851 2024-05-07 20:58:50.000000 pelicun-3.3.3/pelicun/tests/test_uq.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     3298 2024-04-04 20:31:52.000000 pelicun-3.3.3/pelicun/tests/util.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.890019 pelicun-3.3.3/pelicun/tools/
+-rw-r--r--   0 adamzs     (504) staff       (20)    72006 2024-05-08 01:34:25.000000 pelicun-3.3.3/pelicun/tools/DL_calculation.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     2409 2024-05-07 21:02:02.000000 pelicun-3.3.3/pelicun/tools/HDF_to_CSV.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     3216 2024-05-07 21:02:02.000000 pelicun-3.3.3/pelicun/tools/export_DB.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    75928 2024-05-07 20:58:28.000000 pelicun-3.3.3/pelicun/uq.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-05-08 06:21:23.890492 pelicun-3.3.3/pelicun.egg-info/
+-rw-r--r--   0 adamzs     (504) staff       (20)    22472 2024-05-08 06:21:23.000000 pelicun-3.3.3/pelicun.egg-info/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)     4909 2024-05-08 06:21:23.000000 pelicun-3.3.3/pelicun.egg-info/SOURCES.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)        1 2024-05-08 06:21:23.000000 pelicun-3.3.3/pelicun.egg-info/dependency_links.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       62 2024-05-08 06:21:23.000000 pelicun-3.3.3/pelicun.egg-info/entry_points.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)      196 2024-05-08 06:21:23.000000 pelicun-3.3.3/pelicun.egg-info/requires.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)        8 2024-05-08 06:21:23.000000 pelicun-3.3.3/pelicun.egg-info/top_level.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-05-08 06:21:23.892091 pelicun-3.3.3/setup.cfg
+-rw-r--r--   0 adamzs     (504) staff       (20)     2487 2024-05-07 20:53:01.000000 pelicun-3.3.3/setup.py
```

### Comparing `pelicun-3.3.2/LICENSE` & `pelicun-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/PKG-INFO` & `pelicun-3.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: pelicun
-Version: 3.3.2
-Summary: Probabilistic Estimation of Losses, Injuries, and Community resilience Under Natural hazard events
-Home-page: http://nheri-simcenter.github.io/pelicun/
-Author: Adam Zsarnóczay
-Author-email: adamzs@stanford.edu
-License: BSD License
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Environment :: Console
-Classifier: Framework :: Jupyter
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy<2.0,>=1.22.0
-Requires-Dist: scipy<2.0,>=1.7.0
-Requires-Dist: pandas<3.0,>=1.4.0
-Provides-Extra: testing
-Requires-Dist: pytest; extra == "testing"
-
 <p align="center">
 	<img src="https://raw.githubusercontent.com/NHERI-SimCenter/pelicun/gh-pages/doc_src/common/figures/pelicun-Logo-white.png"
 		alt="pelicun" align="middle" height="200"/>
 </p>
 
 <p align="center">
 	<a href="https://doi.org/10.5281/zenodo.2558558", alt="DOI">
@@ -102,18 +69,15 @@
 git clone https://github.com/<user>/pelicun
 cd pelicun
 # Switch to the appropriate branch, if needed.
 # git checkout <branch>
 
 # Install pelicun:
 # Note: don't forget to activate the corresponding environment.
-python -m pip install -e .
-
-# Install additional development setup dependencies
-python -m pip install -r requirements_dev.txt
+python -m pip install -e .[development]
 
 ```
 
 Contributions are managed with pull requests.
 It is required that contributed code is [PEP 8](https://peps.python.org/pep-0008/) compliant, does not introduce linter warnings and includes sufficient unit tests so as to avoid reducing the current coverage level.
 
 The following lines implement the aforementioned checks.
```

#### html2text {}

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1 Name: pelicun Version: 3.3.2 Summary: Probabilistic
-Estimation of Losses, Injuries, and Community resilience Under Natural hazard
-events Home-page: http://nheri-simcenter.github.io/pelicun/ Author: Adam
-ZsarnÃ³czay Author-email: adamzs@stanford.edu License: BSD License Platform:
-any Classifier: Programming Language :: Python Classifier: Development Status
-:: 5 - Production/Stable Classifier: Natural Language :: English Classifier:
-Environment :: Console Classifier: Framework :: Jupyter Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
-:: English Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: numpy<2.0,>=1.22.0 Requires-Dist:
-scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Provides-Extra: testing
-Requires-Dist: pytest; extra == "testing"
                                    [pelicun]
       alt="DOI">[https://zenodo.org/badge/DOI/10.5281/zenodo.2558558.svg]
  PPrroobbaabbiilliissttiicc EEssttiimmaattiioonn ooff LLoosssseess,, IInnjjuurriieess,, aanndd CCoommmmuunniittyy rreessiilliieennccee UUnnddeerr
                              NNaattuurraall hhaazzaarrdd eevveennttss
 ![Tests](https://github.com/NHERI-SimCenter/pelicun/actions/workflows/
 tests.yml/badge.svg) [![codecov](https://codecov.io/github/NHERI-SimCenter/
 pelicun/branch/master/graph/badge.svg?token=W79M5FGOCG)](https://codecov.io/
@@ -73,30 +56,29 @@
 pelicun==2.6.0 ``` Note that 2.6.0 is the last minor version before the v3.0
 release. Other earlier versions can be found [here](https://pypi.org/project/
 pelicun/#history). ### For contributors Developers are expected to fork and
 clone this repository, and install their copy in development mode. Using a
 virtual environment is highly recommended. ```shell # Clone the repository: git
 clone https://github.com//pelicun cd pelicun # Switch to the appropriate
 branch, if needed. # git checkout # Install pelicun: # Note: don't forget to
-activate the corresponding environment. python -m pip install -e . # Install
-additional development setup dependencies python -m pip install -
-r requirements_dev.txt ``` Contributions are managed with pull requests. It is
-required that contributed code is [PEP 8](https://peps.python.org/pep-0008/
-) compliant, does not introduce linter warnings and includes sufficient unit
-tests so as to avoid reducing the current coverage level. The following lines
-implement the aforementioned checks. `flake8`, `pylint` and `pytest` can all be
-configured for use within an IDE. ```shell cd /pelicun export
-PYTHONPATH=$PYTHONPATH:$(pwd) # Linting with flake8: flake8 pelicun # Linting
-with pylint: pylint pelicun # Running the tests: python -m pytest pelicun/tests
---cov=pelicun --cov-report html # Open `htmlcov/index.html`in a browser to see
-coverage results. ``` Feel free to [open an issue](https://github.com/NHERI-
-SimCenter/pelicun/issues/new/choose) if you encounter problems setting up the
-provided development environment. ## Changelog ### Changes in v3.3 - Changes
-affecting backwards compatibility - **Remove "bldg" from repair consequence
-output filenames**: The increasing scope of Pelicun now covers simulations for
+activate the corresponding environment. python -m pip install -e .[development]
+``` Contributions are managed with pull requests. It is required that
+contributed code is [PEP 8](https://peps.python.org/pep-0008/) compliant, does
+not introduce linter warnings and includes sufficient unit tests so as to avoid
+reducing the current coverage level. The following lines implement the
+aforementioned checks. `flake8`, `pylint` and `pytest` can all be configured
+for use within an IDE. ```shell cd /pelicun export PYTHONPATH=$PYTHONPATH:$
+(pwd) # Linting with flake8: flake8 pelicun # Linting with pylint: pylint
+pelicun # Running the tests: python -m pytest pelicun/tests --cov=pelicun --
+cov-report html # Open `htmlcov/index.html`in a browser to see coverage
+results. ``` Feel free to [open an issue](https://github.com/NHERI-SimCenter/
+pelicun/issues/new/choose) if you encounter problems setting up the provided
+development environment. ## Changelog ### Changes in v3.3 - Changes affecting
+backwards compatibility - **Remove "bldg" from repair consequence output
+filenames**: The increasing scope of Pelicun now covers simulations for
 transportation and water networks. Hence, labeling repair consequence outputs
 as if they were limited to buildings no longer seems appropriate. The `bldg`
 label was dropped from the following files:
 `DV_bldg_repair_sample`,`DV_bldg_repair_stats`,`DV_bldg_repair_grp`,
 `DV_bldg_repair_grp_stats`, `DV_bldg_repair_agg`, `DV_bldg_repair_agg_stats`. -
 Deprecation warnings - **Remove `Bldg` from repair settings label in DL
 configuration file**: Following the changes above, we dropped `Bldg` from
```

### Comparing `pelicun-3.3.2/README.md` & `pelicun-3.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,52 @@
+Metadata-Version: 2.1
+Name: pelicun
+Version: 3.3.3
+Summary: Probabilistic Estimation of Losses, Injuries, and Community resilience Under Natural hazard events
+Home-page: http://nheri-simcenter.github.io/pelicun/
+Author: Adam Zsarnóczay
+Author-email: adamzs@stanford.edu
+License: BSD License
+Platform: any
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Environment :: Console
+Classifier: Framework :: Jupyter
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy<2.0,>=1.22.0
+Requires-Dist: scipy<2.0,>=1.7.0
+Requires-Dist: pandas<3.0,>=1.4.0
+Provides-Extra: development
+Requires-Dist: flake8; extra == "development"
+Requires-Dist: pylint; extra == "development"
+Requires-Dist: black; extra == "development"
+Requires-Dist: pytest; extra == "development"
+Requires-Dist: pytest-cov; extra == "development"
+Requires-Dist: glob2; extra == "development"
+Requires-Dist: jupyter; extra == "development"
+Requires-Dist: jupytext; extra == "development"
+Requires-Dist: sphinx; extra == "development"
+Requires-Dist: sphinx-autoapi; extra == "development"
+Requires-Dist: nbsphinx; extra == "development"
+Requires-Dist: flake8-rst; extra == "development"
+Requires-Dist: flake8-rst-docstrings; extra == "development"
+
 <p align="center">
 	<img src="https://raw.githubusercontent.com/NHERI-SimCenter/pelicun/gh-pages/doc_src/common/figures/pelicun-Logo-white.png"
 		alt="pelicun" align="middle" height="200"/>
 </p>
 
 <p align="center">
 	<a href="https://doi.org/10.5281/zenodo.2558558", alt="DOI">
@@ -69,18 +114,15 @@
 git clone https://github.com/<user>/pelicun
 cd pelicun
 # Switch to the appropriate branch, if needed.
 # git checkout <branch>
 
 # Install pelicun:
 # Note: don't forget to activate the corresponding environment.
-python -m pip install -e .
-
-# Install additional development setup dependencies
-python -m pip install -r requirements_dev.txt
+python -m pip install -e .[development]
 
 ```
 
 Contributions are managed with pull requests.
 It is required that contributed code is [PEP 8](https://peps.python.org/pep-0008/) compliant, does not introduce linter warnings and includes sufficient unit tests so as to avoid reducing the current coverage level.
 
 The following lines implement the aforementioned checks.
```

#### html2text {}

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1 Name: pelicun Version: 3.3.3 Summary: Probabilistic
+Estimation of Losses, Injuries, and Community resilience Under Natural hazard
+events Home-page: http://nheri-simcenter.github.io/pelicun/ Author: Adam
+ZsarnÃ³czay Author-email: adamzs@stanford.edu License: BSD License Platform:
+any Classifier: Programming Language :: Python Classifier: Development Status
+:: 5 - Production/Stable Classifier: Natural Language :: English Classifier:
+Environment :: Console Classifier: Framework :: Jupyter Classifier: Intended
+Audience :: Education Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
+:: English Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: numpy<2.0,>=1.22.0 Requires-Dist:
+scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Provides-Extra: development
+Requires-Dist: flake8; extra == "development" Requires-Dist: pylint; extra ==
+"development" Requires-Dist: black; extra == "development" Requires-Dist:
+pytest; extra == "development" Requires-Dist: pytest-cov; extra ==
+"development" Requires-Dist: glob2; extra == "development" Requires-Dist:
+jupyter; extra == "development" Requires-Dist: jupytext; extra == "development"
+Requires-Dist: sphinx; extra == "development" Requires-Dist: sphinx-autoapi;
+extra == "development" Requires-Dist: nbsphinx; extra == "development"
+Requires-Dist: flake8-rst; extra == "development" Requires-Dist: flake8-rst-
+docstrings; extra == "development"
                                    [pelicun]
       alt="DOI">[https://zenodo.org/badge/DOI/10.5281/zenodo.2558558.svg]
  PPrroobbaabbiilliissttiicc EEssttiimmaattiioonn ooff LLoosssseess,, IInnjjuurriieess,, aanndd CCoommmmuunniittyy rreessiilliieennccee UUnnddeerr
                              NNaattuurraall hhaazzaarrdd eevveennttss
 ![Tests](https://github.com/NHERI-SimCenter/pelicun/actions/workflows/
 tests.yml/badge.svg) [![codecov](https://codecov.io/github/NHERI-SimCenter/
 pelicun/branch/master/graph/badge.svg?token=W79M5FGOCG)](https://codecov.io/
@@ -56,30 +81,29 @@
 pelicun==2.6.0 ``` Note that 2.6.0 is the last minor version before the v3.0
 release. Other earlier versions can be found [here](https://pypi.org/project/
 pelicun/#history). ### For contributors Developers are expected to fork and
 clone this repository, and install their copy in development mode. Using a
 virtual environment is highly recommended. ```shell # Clone the repository: git
 clone https://github.com//pelicun cd pelicun # Switch to the appropriate
 branch, if needed. # git checkout # Install pelicun: # Note: don't forget to
-activate the corresponding environment. python -m pip install -e . # Install
-additional development setup dependencies python -m pip install -
-r requirements_dev.txt ``` Contributions are managed with pull requests. It is
-required that contributed code is [PEP 8](https://peps.python.org/pep-0008/
-) compliant, does not introduce linter warnings and includes sufficient unit
-tests so as to avoid reducing the current coverage level. The following lines
-implement the aforementioned checks. `flake8`, `pylint` and `pytest` can all be
-configured for use within an IDE. ```shell cd /pelicun export
-PYTHONPATH=$PYTHONPATH:$(pwd) # Linting with flake8: flake8 pelicun # Linting
-with pylint: pylint pelicun # Running the tests: python -m pytest pelicun/tests
---cov=pelicun --cov-report html # Open `htmlcov/index.html`in a browser to see
-coverage results. ``` Feel free to [open an issue](https://github.com/NHERI-
-SimCenter/pelicun/issues/new/choose) if you encounter problems setting up the
-provided development environment. ## Changelog ### Changes in v3.3 - Changes
-affecting backwards compatibility - **Remove "bldg" from repair consequence
-output filenames**: The increasing scope of Pelicun now covers simulations for
+activate the corresponding environment. python -m pip install -e .[development]
+``` Contributions are managed with pull requests. It is required that
+contributed code is [PEP 8](https://peps.python.org/pep-0008/) compliant, does
+not introduce linter warnings and includes sufficient unit tests so as to avoid
+reducing the current coverage level. The following lines implement the
+aforementioned checks. `flake8`, `pylint` and `pytest` can all be configured
+for use within an IDE. ```shell cd /pelicun export PYTHONPATH=$PYTHONPATH:$
+(pwd) # Linting with flake8: flake8 pelicun # Linting with pylint: pylint
+pelicun # Running the tests: python -m pytest pelicun/tests --cov=pelicun --
+cov-report html # Open `htmlcov/index.html`in a browser to see coverage
+results. ``` Feel free to [open an issue](https://github.com/NHERI-SimCenter/
+pelicun/issues/new/choose) if you encounter problems setting up the provided
+development environment. ## Changelog ### Changes in v3.3 - Changes affecting
+backwards compatibility - **Remove "bldg" from repair consequence output
+filenames**: The increasing scope of Pelicun now covers simulations for
 transportation and water networks. Hence, labeling repair consequence outputs
 as if they were limited to buildings no longer seems appropriate. The `bldg`
 label was dropped from the following files:
 `DV_bldg_repair_sample`,`DV_bldg_repair_stats`,`DV_bldg_repair_grp`,
 `DV_bldg_repair_grp_stats`, `DV_bldg_repair_agg`, `DV_bldg_repair_agg_stats`. -
 Deprecation warnings - **Remove `Bldg` from repair settings label in DL
 configuration file**: Following the changes above, we dropped `Bldg` from
```

### Comparing `pelicun-3.3.2/pelicun/__init__.py` & `pelicun-3.3.3/pelicun/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
 Contributors:
 Adam Zsarnóczay
 """
 
 name = "pelicun"
 
-__version__ = '3.3.2'
+__version__ = '3.3.3'
 
-__copyright__ = ("Copyright (c) 2018 Leland Stanford "
-                 "Junior University and The Regents "
-                 "of the University of California")
+__copyright__ = (
+    "Copyright (c) 2018 Leland Stanford "
+    "Junior University and The Regents "
+    "of the University of California"
+)
 
 __license__ = "BSD 3-Clause License"
```

### Comparing `pelicun-3.3.2/pelicun/assessment.py` & `pelicun-3.3.3/pelicun/assessment.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,21 +86,23 @@
             User-specified configuration dictionary.
         """
 
         self.stories = None
 
         self.options = base.Options(config_options, self)
 
-        self.unit_conversion_factors = base.parse_units(
-            self.options.units_file)
+        self.unit_conversion_factors = base.parse_units(self.options.units_file)
 
         self.log = self.options.log
 
-        self.log.msg(f'pelicun {pelicun_version} | \n',
-                     prepend_timestamp=False, prepend_blank_space=False)
+        self.log.msg(
+            f'pelicun {pelicun_version} | \n',
+            prepend_timestamp=False,
+            prepend_blank_space=False,
+        )
 
         self.log.print_system_info()
 
         self.log.div()
         self.log.msg('Assessment Started')
 
     @property
@@ -157,23 +159,32 @@
             return self._repair
 
         self._repair = model.RepairModel(self)
         return self.repair
 
     def get_default_data(self, data_name):
         """
-        Load a default data file and pass it to the user.
+        Loads a default data file by name and returns it. This method
+        is specifically designed to access predefined CSV files from a
+        structured directory path related to the SimCenter fragility
+        library.
 
         Parameters
         ----------
-        data_name: string
-            Name of the csv file to be loaded
+        data_name : str
+            The name of the CSV file to be loaded, without the '.csv'
+            extension. This name is used to construct the full path to
+            the file.
 
+        Returns
+        -------
+        pd.DataFrame
+            The DataFrame containing the data loaded from the
+            specified CSV file.
         """
-
         data_path = f'{base.pelicun_path}/resources/SimCenterDBDL/{data_name}.csv'
 
         return file_io.load_data(
             data_path, None, orientation=1, reindex=False, log=self.log
         )
 
     def get_default_metadata(self, data_name):
@@ -181,14 +192,19 @@
         Load a default metadata file and pass it to the user.
 
         Parameters
         ----------
         data_name: string
             Name of the json file to be loaded
 
+        Returns
+        -------
+        dict
+            Default metadata
+
         """
 
         data_path = f'{base.pelicun_path}/resources/SimCenterDBDL/{data_name}.json'
 
         with open(data_path, 'r', encoding='utf-8') as f:
             data = json.load(f)
 
@@ -204,15 +220,15 @@
         unit: str
             Either a unit name, or a quantity and a unit name
             separated by a space.
             For example: 'ft' or '100 ft'.
 
         Returns
         -------
-        scale_factor: float
+        float
             Scale factor that convert values from unit to base unit
 
         Raises
         ------
         KeyError
             When an invalid unit is specified
         """
@@ -228,39 +244,44 @@
             unit_count = 1
             unit_name = unit_lst[0]
 
         try:
             scale_factor = unit_count * self.unit_conversion_factors[unit_name]
 
         except KeyError as exc:
-            raise KeyError(f"Specified unit not recognized: "
-                           f"{unit_count} {unit_name}") from exc
+            raise KeyError(
+                f"Specified unit not recognized: {unit_count} {unit_name}"
+            ) from exc
 
         return scale_factor
 
     def scale_factor(self, unit):
         """
         Returns the scale factor of a given unit. If the unit is
         unknown it raises an error. If the unit is None it returns
         1.00.
 
         Parameters
         ----------
         unit: str
             A unit name.
 
+        Returns
+        -------
+        float
+            Scale factor
+
         Raises
         ------
         ValueError
             If the unit is unknown.
 
         """
 
         if unit is not None:
-
             if unit in self.unit_conversion_factors:
                 scale_factor = self.unit_conversion_factors[unit]
 
             else:
                 raise ValueError(f"Unknown unit: {unit}")
         else:
             scale_factor = 1.0
```

### Comparing `pelicun-3.3.2/pelicun/auto.py` & `pelicun-3.3.3/pelicun/auto.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,34 +48,56 @@
 
 """
 
 import sys
 import importlib
 from pathlib import Path
 
-from . import base
+from pelicun import base
 
 
 def auto_populate(
     config, auto_script_path, **kwargs  # pylint: disable=unused-argument
 ):
     """
-    Automatically populates the DL configuration for a Pelicun
-    calculation.
+    Automatically populates the Damage and Loss (DL) configuration for
+    a Pelicun calculation using predefined rules.
+
+    This function modifies the provided configuration dictionary based
+    on an external Python script that defines auto-population
+    rules. It supports using built-in scripts or custom scripts
+    specified by the user.
 
     Parameters
     ----------
-    config: dict
-        Configuration dictionary with a GeneralInformation key that
-        holds another dictionary with attributes of the asset of
-        interest.
-    auto_script_path: string
-        Path pointing to a python script with the auto-population
-        rules.  Built-in scripts can be referenced using the
-        PelicunDefault/XY format where XY is the name of the script.
+    config : dict
+        A configuration dictionary with a 'GeneralInformation' key
+        that holds another dictionary with attributes of the asset of
+        interest. This dictionary is modified in-place with
+        auto-populated values.
+    auto_script_path : str
+        The path pointing to a Python script with the auto-population
+        rules. Built-in scripts can be referenced using the
+        'PelicunDefault/XY' format where 'XY' is the name of the
+        script.
+
+    Returns
+    -------
+    tuple
+        A tuple containing two items:
+        1. Updated configuration dictionary including new 'DL' key
+        with damage and loss information.
+        2. A dictionary of component quantities (CMP) derived from the
+        auto-population process.
+
+    Raises
+    ------
+    ValueError
+        If the configuration dictionary does not contain necessary
+        asset information under 'GeneralInformation'.
     """
 
     # try to get the AIM attributes
     AIM = config.get('GeneralInformation', None)
     if AIM is None:
         raise ValueError(
             "No Asset Information provided for the auto-population routine."
```

### Comparing `pelicun-3.3.2/pelicun/base.py` & `pelicun-3.3.3/pelicun/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 pd.options.display.expand_frame_repr = True
 pd.options.display.width = 300
 
 idx = pd.IndexSlice
 
 
 class Options:
-
     """
     Options objects store analysis options and the logging
     configuration.
 
     Attributes
     ----------
     sampling_method: str
@@ -179,19 +178,18 @@
         self.defaults = None
         self.sampling_method = None
         self.list_all_ds = None
 
         self._seed = None
 
         self._rng = np.random.default_rng()
-        merged_config_options = merge_default_config(
-            user_config_options)
+        merged_config_options = merge_default_config(user_config_options)
 
         self._seed = merged_config_options['Seed']
-        self.sampling_method = merged_config_options['SamplingMethod']
+        self.sampling_method = merged_config_options['Sampling']['SamplingMethod']
         self.list_all_ds = merged_config_options['ListAllDamageStates']
 
         self.units_file = merged_config_options['UnitsFile']
 
         self.demand_offset = merged_config_options['DemandOffset']
         self.nondir_multi_dict = merged_config_options['NonDirectionalMultipliers']
         self.rho_cost_time = merged_config_options['RepairCostAndTimeCorrelation']
@@ -199,27 +197,33 @@
 
         # instantiate a Logger object with the finalized configuration
         self.log = Logger(
             merged_config_options['Verbose'],
             merged_config_options['ShowWarnings'],
             merged_config_options['LogShowMS'],
             merged_config_options['LogFile'],
-            merged_config_options['PrintLog'])
+            merged_config_options['PrintLog'],
+        )
 
     def nondir_multi(self, EDP_type):
         """
         Returns the multiplicative factor used in nondirectional
         component demand generation. Read the description of the
         nondir_multi_dict attribute of the Options class.
 
         Parameters
         ----------
         EDP_type: str
             EDP type (e.g. "PFA", "PFV", ..., "ALL")
 
+        Returns
+        -------
+        float
+            Nondirectional component multiplicative factor.
+
         Raises
         ------
         ValueError
             If the specified EDP type is not present in the
             dictionary.  If this is the case, a value for that type
             needs to be specified in the user's configuration
             dictionary, under ['Options']['NonDirectionalMultipliers']
@@ -233,20 +237,26 @@
             return self.nondir_multi_dict['ALL']
 
         raise ValueError(
             f"Peak orthogonal EDP multiplier for non-directional demand "
             f"calculation of {EDP_type} not specified.\n"
             f"Please add {EDP_type} in the configuration dictionary "
             f"under ['Options']['NonDirectionalMultipliers']"
-            " = {{'edp_type': value, ...}}")
+            " = {{'edp_type': value, ...}}"
+        )
 
     @property
     def seed(self):
         """
-        seed property
+        Seed property
+
+        Returns
+        -------
+        float
+            Seed value
         """
         return self._seed
 
     @seed.setter
     def seed(self, value):
         """
         seed property setter
@@ -254,34 +264,43 @@
         self._seed = value
         self._rng = np.random.default_rng(self._seed)
 
     @property
     def rng(self):
         """
         rng property
+
+        Returns
+        -------
+        Generator
+            Random generator
         """
         return self._rng
 
     @property
     def units_file(self):
         """
         units file property
+
+        Returns
+        -------
+        str
+            Units file
         """
         return self._units_file
 
     @units_file.setter
     def units_file(self, value):
         """
         units file property setter
         """
         self._units_file = value
 
 
 class Logger:
-
     """
     Logger objects are used to generate log files documenting
     execution events and related messages.
 
     Attributes
     ----------
     verbose: bool
@@ -310,14 +329,15 @@
     print_log: bool
         If True, the log is also printed to standard output. The
         value is specified in the user's configuration dictionary,
         otherwise left as provided in the default configuration file
         (see settings/default_config.json in the pelicun source code).
 
     """
+
     # TODO: finalize docstring
 
     def __init__(self, verbose, show_warnings, log_show_ms, log_file, print_log):
         """
         Initializes a Logger object.
 
         Parameters
@@ -332,28 +352,38 @@
         self.print_log = print_log
         self.reset_log_strings()
 
     @property
     def verbose(self):
         """
         verbose property
+
+        Returns
+        -------
+        bool
+            Verbose property value
         """
         return self._verbose
 
     @verbose.setter
     def verbose(self, value):
         """
         verbose property setter
         """
         self._verbose = bool(value)
 
     @property
     def show_warnings(self):
         """
         show_warnings property
+
+        Returns
+        -------
+        bool
+            show_warnings value
         """
         return self._show_warnings
 
     @show_warnings.setter
     def show_warnings(self, value):
         """
         show_warnings property setter
@@ -362,14 +392,18 @@
         # control warnings according to the desired setting
         control_warnings(show=self._show_warnings)
 
     @property
     def log_show_ms(self):
         """
         log_show_ms property
+
+        Returns
+        bool
+            log_show_ms value
         """
         return self._log_show_ms
 
     @log_show_ms.setter
     def log_show_ms(self, value):
         """
         log_show_ms property setter
@@ -378,21 +412,31 @@
 
         self.reset_log_strings()
 
     @property
     def log_pref(self):
         """
         log_pref property
+
+        Returns
+        -------
+        str
+            log_pref value
         """
         return self._log_pref
 
     @property
     def log_div(self):
         """
         log_div property
+
+        Returns
+        -------
+        str
+            log_div value
         """
         return self._log_div
 
     @property
     def log_time_format(self):
         """
         log_time_format property
@@ -412,29 +456,29 @@
         log_file property setter
         """
 
         if value is None:
             self._log_file = None
 
         else:
-
             try:
-
                 filepath = Path(value).resolve()
 
                 self._log_file = str(filepath)
 
                 with open(filepath, 'w', encoding='utf-8') as f:
                     f.write('')
 
             except BaseException as err:
-                print(f"WARNING: The filepath provided for the log file does "
-                      f"not point to a valid location: {value}. \nPelicun "
-                      f"cannot print the log to a file.\n"
-                      f"The error was: '{err}'")
+                print(
+                    f"WARNING: The filepath provided for the log file does "
+                    f"not point to a valid location: {value}. \nPelicun "
+                    f"cannot print the log to a file.\n"
+                    f"The error was: '{err}'"
+                )
                 raise
 
     @property
     def print_log(self):
         """
         print_log property
         """
@@ -480,18 +524,18 @@
 
         """
 
         # pylint: disable = consider-using-f-string
         msg_lines = msg.split('\n')
 
         for msg_i, msg_line in enumerate(msg_lines):
-
-            if (prepend_timestamp and (msg_i == 0)):
+            if prepend_timestamp and (msg_i == 0):
                 formatted_msg = '{} {}'.format(
-                    datetime.now().strftime(self.log_time_format), msg_line)
+                    datetime.now().strftime(self.log_time_format), msg_line
+                )
             elif prepend_timestamp:
                 formatted_msg = self.log_pref + msg_line
             elif prepend_blank_space:
                 formatted_msg = self.log_pref + msg_line
             else:
                 formatted_msg = msg_line
 
@@ -515,31 +559,31 @@
 
     def print_system_info(self):
         """
         Writes system information in the log.
         """
 
         self.msg(
-            'System Information:',
-            prepend_timestamp=False, prepend_blank_space=False)
+            'System Information:', prepend_timestamp=False, prepend_blank_space=False
+        )
         self.msg(
             f'local time zone: {datetime.utcnow().astimezone().tzinfo}\n'
             f'start time: {datetime.now().strftime("%Y-%m-%dT%H:%M:%S")}\n'
             f'python: {sys.version}\n'
             f'numpy: {np.__version__}\n'
             f'pandas: {pd.__version__}\n',
-            prepend_timestamp=False)
+            prepend_timestamp=False,
+        )
 
 
 # get the absolute path of the pelicun directory
 pelicun_path = Path(os.path.dirname(os.path.abspath(__file__)))
 
 
 def control_warnings(show):
-
     """
     Convenience function to turn warnings on/off
 
     Parameters
     ----------
     show: bool
         If True, warnings are set to the default level. If False,
@@ -548,41 +592,41 @@
     """
     if show:
         action = 'default'
     else:
         action = 'ignore'
 
     if not sys.warnoptions:
-        warnings.filterwarnings(
-            category=FutureWarning, action=action)
+        warnings.filterwarnings(category=FutureWarning, action=action)
 
-        warnings.filterwarnings(
-            category=DeprecationWarning, action=action)
+        warnings.filterwarnings(category=DeprecationWarning, action=action)
 
-        warnings.filterwarnings(
-            category=pd.errors.PerformanceWarning, action=action)
+        warnings.filterwarnings(category=pd.errors.PerformanceWarning, action=action)
 
 
 def load_default_options():
     """
     Load the default_config.json file to set options to default values
+
+    Returns
+    -------
+    dict
+        Default options
     """
 
-    with open(pelicun_path / "settings/default_config.json",
-              'r', encoding='utf-8') as f:
+    with open(
+        pelicun_path / "settings/default_config.json", 'r', encoding='utf-8'
+    ) as f:
         default_config = json.load(f)
 
     default_options = default_config['Options']
     return default_options
 
 
-def update_vals(
-        update, primary,
-        update_path, primary_path
-):
+def update_vals(update, primary, update_path, primary_path):
     """
     Updates the values of the `update` nested dictionary with
     those provided in the `primary` nested dictionary. If a key
     already exists in update, and does not map to another
     dictionary, the value is left unchanged.
 
     Parameters
@@ -631,16 +675,19 @@
                     f'{update_path}["{key}"] = {update[key]}, but '
                     f'the default value is '
                     f'{primary_path}["{key}"] = {primary[key]}. '
                     f'Please revise {update_path}["{key}"].'
                 )
             # With both being dictionaries, we recurse.
             update_vals(
-                update[key], primary[key],
-                f'{update_path}["{key}"]', f'{primary_path}["{key}"]')
+                update[key],
+                primary[key],
+                f'{update_path}["{key}"]',
+                f'{primary_path}["{key}"]',
+            )
         # if `primary[key]` is NOT a dictionary:
         else:
             # if `key` does not exist in `update`, we add it, with
             # its corresponding value.
             if key not in update:
                 update[key] = primary[key]
             else:
@@ -662,37 +709,35 @@
 def merge_default_config(user_config):
     """
     Merge the user-specified config with the configuration defined in
     the default_config.json file. If the user-specified config does
     not include some option available in the default options, then the
     default option is used in the merged config.
 
-    Parameters.
+    Parameters
     ----------
     user_config: dict
         User-specified configuration dictionary
 
     Returns
     -------
-    user_config: dict
+    dict
         Merged configuration dictionary
     """
 
     config = user_config  # start from the user's config
     default_config = load_default_options()
 
     if config is None:
         config = {}
 
     # We fill out the user's config with the values available in the
     # default config that were not set.
     # We use a recursive function to handle nesting.
-    update_vals(
-        config, default_config,
-        'user_settings', 'default_settings')
+    update_vals(config, default_config, 'user_settings', 'default_settings')
 
     return config
 
 
 def convert_to_SimpleIndex(data, axis=0, inplace=False):
     """
     Converts the index of a DataFrame to a simple, one-level index
@@ -710,50 +755,45 @@
         edited.
     inplace: bool, optional, default:False
         If yes, the operation is performed directly on the input
         DataFrame and not on a copy of it.
 
     Returns
     -------
-    data: DataFrame
+    DataFrame
         The modified DataFrame
 
     Raises
     ------
     ValueError
         When an invalid axis parameter is specified
     """
 
     if axis in {0, 1}:
-
         if inplace:
             data_mod = data
         else:
             data_mod = data.copy()
 
         if axis == 0:
-
             # only perform this if there are multiple levels
             if data.index.nlevels > 1:
-
                 simple_name = '-'.join(
                     [n if n is not None else "" for n in data.index.names]
                 )
                 simple_index = [
                     '-'.join([str(id_i) for id_i in id]) for id in data.index
                 ]
 
                 data_mod.index = simple_index
                 data_mod.index.name = simple_name
 
         elif axis == 1:
-
             # only perform this if there are multiple levels
             if data.columns.nlevels > 1:
-
                 simple_name = '-'.join(
                     [n if n is not None else "" for n in data.columns.names]
                 )
                 simple_index = [
                     '-'.join([str(id_i) for id_i in id]) for id in data.columns
                 ]
 
@@ -783,28 +823,27 @@
         edited.
     inplace: bool, optional, default:False
         If yes, the operation is performed directly on the input
         DataFrame and not on a copy of it.
 
     Returns
     -------
-    data: DataFrame
+    DataFrame
         The modified DataFrame.
 
     Raises
     ------
     ValueError
         If an invalid axis is specified.
     """
 
     # check if the requested axis is already a MultiIndex
     if ((axis == 0) and (isinstance(data.index, pd.MultiIndex))) or (
         (axis == 1) and (isinstance(data.columns, pd.MultiIndex))
     ):
-
         # if yes, return the data unchanged
         return data
 
     if axis == 0:
         index_labels = [str(label).split('-') for label in data.index]
 
     elif axis == 1:
@@ -812,25 +851,23 @@
 
     else:
         raise ValueError(f"Invalid axis parameter: {axis}")
 
     max_lbl_len = np.max([len(labels) for labels in index_labels])
 
     for l_i, labels in enumerate(index_labels):
-
         if len(labels) != max_lbl_len:
             labels += [
                 '',
             ] * (max_lbl_len - len(labels))
             index_labels[l_i] = labels
 
     index_labels = np.array(index_labels)
 
     if index_labels.shape[1] > 1:
-
         if inplace:
             data_mod = data
         else:
             data_mod = data.copy()
 
         if axis == 0:
             data_mod.index = pd.MultiIndex.from_arrays(index_labels.T)
@@ -870,27 +907,54 @@
     # See:
     # https://pandas.pydata.org/docs/reference/api/pandas.to_numeric.html
     return dataframe.apply(lambda x: pd.to_numeric(x, errors='ignore'), axis=0)
 
 
 def show_matrix(data, use_describe=False):
     """
-    Print a matrix in a nice way using a DataFrame
+    Print a matrix in a nice way using a DataFrame.
+    Parameters
+    ----------
+    data : array-like
+        The matrix data to display. Can be any array-like structure that pandas can convert to a DataFrame.
+    use_describe : bool, default: False
+        If True, provides a descriptive statistical summary of the matrix including specified percentiles.
+        If False, simply prints the matrix as is.
     """
     if use_describe:
-        pp.pprint(
-            pd.DataFrame(data).describe(percentiles=[0.01, 0.1, 0.5, 0.9, 0.99])
-        )
+        pp.pprint(pd.DataFrame(data).describe(percentiles=[0.01, 0.1, 0.5, 0.9, 0.99]))
     else:
         pp.pprint(pd.DataFrame(data))
 
 
 def _warning(message, category, filename, lineno, file=None, line=None):
     """
-    Monkeypatch warnings to get prettier messages
+    Custom warning function to format and print warnings more
+    attractively. This function modifies how warning messages are
+    displayed, emphasizing the file path and line number from where
+    the warning originated.
+
+    Parameters
+    ----------
+    message : str
+        The warning message to be displayed.
+    category : Warning
+        The category of the warning (unused, but required for
+        compatibility with standard warning signature).
+    filename : str
+        The path of the file from which the warning is issued. The
+        function simplifies the path for display.
+    lineno : int
+        The line number in the file at which the warning is issued.
+    file : file-like object, optional
+        The target file object to write the warning to (unused, but
+        required for compatibility with standard warning signature).
+    line : str, optional
+        Line of code causing the warning (unused, but required for
+        compatibility with standard warning signature).
     """
     # pylint:disable = unused-argument
     if '\\' in filename:
         file_path = filename.split('\\')
     elif '/' in filename:
         file_path = filename.split('/')
     else:
@@ -903,18 +967,42 @@
 
     print(f'WARNING in {python_file} at line {lineno}\n{message}\n')
 
 
 warnings.showwarning = _warning
 
 
-def describe(df, percentiles=(0.001, 0.023, 0.10, 0.159, 0.5, 0.841, 0.90,
-                              0.977, 0.999)):
+def describe(
+    df, percentiles=(0.001, 0.023, 0.10, 0.159, 0.5, 0.841, 0.90, 0.977, 0.999)
+):
     """
-    Provide descriptive statistics.
+    Provides extended descriptive statistics for given data, including
+    percentiles and log standard deviation for applicable columns.
+
+    This function accepts both pandas Series and DataFrame objects
+    directly, or any array-like structure which can be converted to
+    them. It calculates common descriptive statistics and optionally
+    adds log standard deviation for columns where all values are
+    positive.
+
+    Parameters
+    ----------
+    df : pd.Series, pd.DataFrame, or array-like
+        The data to describe. If array-like, it is converted to a
+        DataFrame or Series before analysis.
+    percentiles : tuple of float, optional
+        Specific percentiles to include in the output. Default
+        includes an extensive range tailored to provide a detailed
+        summary.
+
+    Returns
+    -------
+    pd.DataFrame
+        A DataFrame containing the descriptive statistics of the input
+        data, transposed so that each descriptive statistic is a row.
     """
     if not isinstance(df, (pd.Series, pd.DataFrame)):
         vals = df
         cols = np.arange(vals.shape[1]) if vals.ndim > 1 else 0
 
         if vals.ndim == 1:
             df = pd.Series(vals, name=cols)
@@ -936,15 +1024,40 @@
             desc.loc['log_std', col] = np.std(np.log(df[col]), ddof=1)
 
     return desc
 
 
 def str2bool(v):
     """
-    Converts various bool-like forms of string to actual booleans
+    Converts a string representation of truth to boolean True or
+    False.
+
+    This function is designed to convert string inputs that represent
+    boolean values into actual Python boolean types. It handles
+    typical representations of truthiness and falsiness, and is case
+    insensitive.
+
+    Parameters
+    ----------
+    v : str or bool
+        The value to convert into a boolean. This can be a boolean
+        itself (in which case it is simply returned) or a string that
+        is expected to represent a boolean value.
+
+    Returns
+    -------
+    bool
+        The boolean value corresponding to the input.
+
+    Raises
+    ------
+    argparse.ArgumentTypeError
+        If `v` is a string that does not correspond to a boolean
+        value, an error is raised indicating that a boolean value was
+        expected.
     """
     # courtesy of Maxim @ stackoverflow
 
     if isinstance(v, bool):
         return v
     if v.lower() in {'yes', 'true', 'True', 't', 'y', '1'}:
         return True
@@ -961,15 +1074,15 @@
     Parameters
     ----------
     string: str
         A string
 
     Returns
     -------
-    res: float, optional
+    float or None
         A float, if the given string can be converted to a
         float. Otherwise, it returns None
     """
     try:
         res = float(string)
         return res
     except ValueError:
@@ -984,118 +1097,187 @@
     Parameters
     ----------
     string: str
         A string
 
     Returns
     -------
-    res: int, optional
+    int or None
         An int, if the given string can be converted to an
         int. Otherwise, it returns None
     """
     try:
         res = int(string)
         return res
     except ValueError:
         return None
 
 
 def process_loc(string, stories):
     """
-    Parses the location parameter.
+    Parses the 'location' parameter from input to determine the
+    specific locations to be processed. This function interprets
+    various string formats to output a list of integers representing
+    locations.
+
+    Parameters
+    ----------
+    string : str
+        A string that describes the location or range of locations of
+        the asset.  It can be a single number, a range (e.g., '3-7'),
+        'all', 'top', 'roof', or 'last'.
+    stories : int
+        The total number of locations in the asset, used to interpret
+        relative terms like 'top' or 'roof', or to generate a range
+        for 'all'.
+
+    Returns
+    -------
+    list of int or None
+        A list of integers representing each floor specified by the
+        string. Returns None if the string does not conform to
+        expected formats.
+
+    Raises
+    ------
+    ValueError
+        Raises an exception if the string contains a range that is not
+        interpretable (e.g., non-integer values or logical
+        inconsistencies in the range).
     """
     try:
         res = int(string)
-        return [res, ]
-    except ValueError:
+        return [
+            res,
+        ]
+    except ValueError as exc:
         if "-" in string:
             s_low, s_high = string.split('-')
             s_low = process_loc(s_low, stories)
             s_high = process_loc(s_high, stories)
             return list(range(s_low[0], s_high[0] + 1))
         if string == "all":
             return list(range(1, stories + 1))
-        if string == "top":
-            return [stories, ]
-        if string == "roof":
-            return [stories, ]
-        return None
+        if string in {"top", "roof", "last"}:
+            return [
+                stories,
+            ]
+        raise ValueError(f'Invalid string: {string}') from exc
 
 
 def dedupe_index(dataframe, dtype=str):
     """
-    Adds an extra level to the index of a dataframe so that all
-    resulting index elements are unique. Assumes that the original
-    index is a MultiIndex with specified names.
+    Modifies the index of a DataFrame to ensure all index elements are
+    unique by adding an extra level.  Assumes that the DataFrame's
+    original index is a MultiIndex with specified names. A unique
+    identifier ('uid') is added as an additional index level based on
+    the cumulative count of occurrences of the original index
+    combinations.
 
-    """
+    Parameters
+    ----------
+    dataframe : pd.DataFrame
+        The DataFrame whose index is to be modified. It must have a
+        MultiIndex.
+    dtype : type, optional
+        The data type for the new index level 'uid'. Defaults to str.
+
+    Notes
+    -----
+    This function changes the DataFrame in place, hence it does not
+    return the DataFrame but modifies the original one provided.
 
+    """
     inames = dataframe.index.names
     dataframe.reset_index(inplace=True)
-    dataframe['uid'] = (
-        dataframe.groupby([*inames]).cumcount()).astype(dtype)
+    dataframe['uid'] = (dataframe.groupby([*inames]).cumcount()).astype(dtype)
     dataframe.set_index([*inames] + ['uid'], inplace=True)
     dataframe.sort_index(inplace=True)
 
 
 # Input specs
 
 EDP_to_demand_type = {
     # Drifts
-    'Story Drift Ratio':               'PID',
-    'Peak Interstory Drift Ratio':     'PID',
-    'Roof Drift Ratio':                'PRD',
-    'Peak Roof Drift Ratio':           'PRD',
-    'Damageable Wall Drift':           'DWD',
-    'Racking Drift Ratio':             'RDR',
-    'Mega Drift Ratio':                'PMD',
-    'Residual Drift Ratio':            'RID',
+    'Story Drift Ratio': 'PID',
+    'Peak Interstory Drift Ratio': 'PID',
+    'Roof Drift Ratio': 'PRD',
+    'Peak Roof Drift Ratio': 'PRD',
+    'Damageable Wall Drift': 'DWD',
+    'Racking Drift Ratio': 'RDR',
+    'Mega Drift Ratio': 'PMD',
+    'Residual Drift Ratio': 'RID',
     'Residual Interstory Drift Ratio': 'RID',
-    'Peak Effective Drift Ratio':      'EDR',
-
+    'Peak Effective Drift Ratio': 'EDR',
     # Floor response
-    'Peak Floor Acceleration':        'PFA',
-    'Peak Floor Velocity':            'PFV',
-    'Peak Floor Displacement':        'PFD',
-
+    'Peak Floor Acceleration': 'PFA',
+    'Peak Floor Velocity': 'PFV',
+    'Peak Floor Displacement': 'PFD',
     # Component response
-    'Peak Link Rotation Angle':       'LR',
-    'Peak Link Beam Chord Rotation':  'LBR',
-
+    'Peak Link Rotation Angle': 'LR',
+    'Peak Link Beam Chord Rotation': 'LBR',
     # Wind Intensity
-    'Peak Gust Wind Speed':           'PWS',
-
+    'Peak Gust Wind Speed': 'PWS',
     # Inundation Intensity
-    'Peak Inundation Height':         'PIH',
-
+    'Peak Inundation Height': 'PIH',
     # Shaking Intensity
-    'Peak Ground Acceleration':       'PGA',
-    'Peak Ground Velocity':           'PGV',
-    'Spectral Acceleration':          'SA',
-    'Spectral Velocity':              'SV',
-    'Spectral Displacement':          'SD',
-    'Peak Spectral Acceleration':     'SA',
-    'Peak Spectral Velocity':         'SV',
-    'Peak Spectral Displacement':     'SD',
-    'Permanent Ground Deformation':   'PGD',
-
+    'Peak Ground Acceleration': 'PGA',
+    'Peak Ground Velocity': 'PGV',
+    'Spectral Acceleration': 'SA',
+    'Spectral Velocity': 'SV',
+    'Spectral Displacement': 'SD',
+    'Peak Spectral Acceleration': 'SA',
+    'Peak Spectral Velocity': 'SV',
+    'Peak Spectral Displacement': 'SD',
+    'Permanent Ground Deformation': 'PGD',
     # Placeholder for advanced calculations
-    'One':                            'ONE'
+    'One': 'ONE',
 }
 
 
 def dict_raise_on_duplicates(ordered_pairs):
     """
-    Reject duplicate keys.
+    Constructs a dictionary from a list of key-value pairs, raising an
+    exception if duplicate keys are found.
 
-    https://stackoverflow.com/questions/14902299/
-    json-loads-allows-duplicate-keys-
-    in-a-dictionary-overwriting-the-first-value
+    This function ensures that no two pairs have the same key. It is
+    particularly useful when parsing JSON-like data where unique keys
+    are expected but not enforced by standard parsing methods.
 
+    Parameters
+    ----------
+    ordered_pairs : list of tuples
+        A list of tuples, each containing a key and a value. Keys are
+        expected to be unique across the list.
+
+    Returns
+    -------
+    dict
+        A dictionary constructed from the ordered_pairs without any
+        duplicates.
+
+    Raises
+    ------
+    ValueError
+        If a duplicate key is found in the input list, a ValueError is
+        raised with a message indicating the duplicate key.
+
+    Examples
+    --------
+    >>> dict_raise_on_duplicates(
+    ...     [("key1", "value1"), ("key2", "value2"), ("key1", "value3")]
+    ... )
+    ValueError: duplicate key: key1
+
+    Notes
+    -----
+    This implementation is useful for contexts in which data integrity
+    is crucial and key uniqueness must be ensured.
     """
+
     d = {}
     for k, v in ordered_pairs:
         if k in d:
             raise ValueError(f"duplicate key: {k}")
         d[k] = v
     return d
 
@@ -1106,27 +1288,88 @@
 
     Parameters
     ----------
     custom_file: str, optional
         If a custom file is provided, only the units specified in the
         custom file are used.
 
+    Returns
+    -------
+    dict
+        A dictionary where keys are unit names and values are
+        their corresponding conversion factors. If
+        `preserve_categories` is True, the dictionary may maintain
+        its original nested structure based on the JSON file. If
+        `preserve_categories` is False, the dictionary is flattened
+        to have globally unique unit names.
+
     Raises
     ------
     KeyError
         If a key is defined twice.
     ValueError
         If a unit conversion factor is not a float.
     FileNotFoundError
         If a file does not exist.
     Exception
         If a file does not have the JSON format.
     """
 
     def get_contents(file_path, preserve_categories=False):
+        """
+        Parses a unit conversion factors JSON file and returns a
+        dictionary mapping unit names to conversion factors.
+
+        This function allows the use of a custom JSON file for
+        defining unit conversion factors or defaults to a predefined
+        file. It ensures that each unit name is unique and that all
+        conversion factors are float values. Additionally, it supports
+        the option to preserve the original data types of category
+        values from the JSON.
+
+        Parameters
+        ----------
+        file_path : str
+            The file path to a JSON file containing unit conversion
+            factors. If not provided, a default file is used.
+        preserve_categories : bool, optional
+            If True, maintains the original data types of category
+            values from the JSON file. If False, converts all values
+            to floats and flattens the dictionary structure, ensuring
+            that each unit name is globally unique across categories.
+
+        Returns
+        -------
+        dict
+            A dictionary where keys are unit names and values are
+            their corresponding conversion factors. If
+            `preserve_categories` is True, the dictionary may maintain
+            its original nested structure based on the JSON file.
+
+        Raises
+        ------
+        FileNotFoundError
+            If the specified file does not exist.
+        ValueError
+            If a unit name is duplicated, a conversion factor is not a
+            float, or other JSON structure issues are present.
+        json.decoder.JSONDecodeError
+            If the file is not a valid JSON file.
+        TypeError
+            If any value that needs to be converted to float cannot be
+            converted.
+
+        Examples
+        --------
+        >>> parse_units('custom_units.json')
+        { 'm': 1.0, 'cm': 0.01, 'mm': 0.001 }
+
+        >>> parse_units('custom_units.json', preserve_categories=True)
+        { 'Length': {'m': 1.0, 'cm': 0.01, 'mm': 0.001} }
+        """
         try:
             with open(file_path, 'r', encoding='utf-8') as f:
                 dictionary = json.load(f, object_pairs_hook=dict_raise_on_duplicates)
         except FileNotFoundError as exc:
             raise FileNotFoundError(f'{file_path} was not found.') from exc
         except json.decoder.JSONDecodeError as exc:
             raise ValueError(f'{file_path} is not a valid JSON file.') from exc
@@ -1164,19 +1407,19 @@
 
     return get_contents(
         pelicun_path / "settings/default_units.json", preserve_categories
     )
 
 
 def convert_units(
-    values: (float | list[float] | np.ndarray),
+    values: float | list[float] | np.ndarray,
     unit: str,
     to_unit: str,
-    category: (str | None) = None
-) -> (float | list[float] | np.ndarray):
+    category: str | None = None,
+) -> float | list[float] | np.ndarray:
     """
     Converts numeric values between different units.
 
     Supports conversion within a specified category of units and
     automatically infers the category if not explicitly provided. It
     maintains the type of the input in the output.
 
@@ -1191,24 +1434,24 @@
     category (Optional[str]):
       The category of the units (e.g., 'length', 'pressure'). If not
       provided, the category will be inferred based on the provided
       units.
 
     Returns
     -------
-    (float | list[float] | np.ndarray):
+    float or list[float] or np.ndarray
       The converted value(s) in the target unit, in the same data type
       as the input values.
 
     Raises
     ------
-    TypeError:
+    TypeError
       If the input `values` are not of type float, list, or
       np.ndarray.
-    ValueError:
+    ValueError
       If the `unit`, `to_unit`, or `category` is unknown or if `unit`
       and `to_unit` are not in the same category.
 
     """
 
     if isinstance(values, (float, list)):
         vals = np.atleast_1d(values)
@@ -1223,19 +1466,17 @@
     # if a category is given use it, otherwise try to determine it
     if category:
         if category not in all_units:
             raise ValueError(f'Unknown category: `{category}`')
         units = all_units[category]
         for unt in unit, to_unit:
             if unt not in units:
-                raise ValueError(
-                    f'Unknown unit: `{unt}`'
-                )
+                raise ValueError(f'Unknown unit: `{unt}`')
     else:
-        unit_category: (str | None) = None
+        unit_category: str | None = None
         for key in all_units:
             units = all_units[key]
             if unit in units:
                 unit_category = key
                 break
         if not unit_category:
             raise ValueError(f'Unknown unit `{unit}`')
```

### Comparing `pelicun-3.3.2/pelicun/db.py` & `pelicun-3.3.3/pelicun/db.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,44 +42,53 @@
 
 .. rubric:: Contents
 
 .. autosummary::
 
     create_FEMA_P58_fragility_db
     create_FEMA_P58_repair_db
-    create_FEMA_P58_bldg_injury_db
     create_FEMA_P58_bldg_redtag_db
 
     create_Hazus_EQ_fragility_db
     create_Hazus_EQ_repair_db
-    create_Hazus_EQ_bldg_injury_db
 
 """
 
+from __future__ import annotations
 import re
 import json
 from pathlib import Path
 from copy import deepcopy
 import numpy as np
 from scipy.stats import norm
 import pandas as pd
 
-from . import base
-from .uq import fit_distribution_to_percentiles
+from pelicun import base
+from pelicun.uq import fit_distribution_to_percentiles
 
 idx = base.idx
 
 
 # pylint: disable=too-many-statements
 # pylint: disable=too-many-locals
 
 
 def parse_DS_Hierarchy(DSH):
     """
     Parses the FEMA P58 DS hierarchy into a set of arrays.
+
+    Parameters
+    ----------
+    DSH: str
+       Damage state hierarchy
+
+    Returns
+    -------
+    list
+      Damage state setup
     """
     if DSH[:3] == 'Seq':
         DSH = DSH[4:-1]
 
     DS_setup = []
 
     while len(DSH) > 0:
@@ -316,17 +325,15 @@
             comments = cmp_meta['Component_Description']
         else:
             comments = ''
 
         # the additional fields are added to the description if they exist
 
         if cmp_meta['Construction_Quality'] != 'Not Specified':
-            comments += (
-                f'\nConstruction Quality: {cmp_meta["Construction_Quality"]}'
-            )
+            comments += f'\nConstruction Quality: {cmp_meta["Construction_Quality"]}'
 
         if cmp_meta['Seismic_Installation_Conditions'] not in [
             'Not Specified',
             'Not applicable',
             'Unknown',
             'Any',
         ]:
@@ -402,17 +409,15 @@
                         repair_action = cmp_meta[f"DS_{ds_id}_Repair_Description"]
                         if pd.isna(repair_action):
                             repair_action = "<missing data>"
 
                         ls_meta.update(
                             {
                                 f"DS{ds_id}": {
-                                    "Description": cmp_meta[
-                                        f"DS_{ds_id}_Description"
-                                    ],
+                                    "Description": cmp_meta[f"DS_{ds_id}_Description"],
                                     "RepairAction": repair_action,
                                 }
                             }
                         )
 
                 else:
                     # in simultaneous cases, convert simultaneous weights into
@@ -424,17 +429,19 @@
 
                     for ds_id in range(1, ds_count + 1):
                         ds_map = format(ds_id, f'0{sim_ds_count}b')
 
                         sim_weights.append(
                             np.product(
                                 [
-                                    weights[ds_i]
-                                    if ds_map[-ds_i - 1] == '1'
-                                    else 1.0 - weights[ds_i]
+                                    (
+                                        weights[ds_i]
+                                        if ds_map[-ds_i - 1] == '1'
+                                        else 1.0 - weights[ds_i]
+                                    )
                                     for ds_i in range(sim_ds_count)
                                 ]
                             )
                         )
 
                         # save ds metadata - we need to be clever here
                         # the original metadata is saved for the pure cases
@@ -892,47 +899,55 @@
             ds_count = 2 ** (sim_ds_count) - 1
 
             for DS_i in range(1, ds_count + 1):
                 ds_map = format(DS_i, f'0{sim_ds_count}b')
 
                 cost_vals = np.sum(
                     [
-                        cost_est[f'DS{ds_i + 1}']
-                        if ds_map[-ds_i - 1] == '1'
-                        else np.zeros(5)
+                        (
+                            cost_est[f'DS{ds_i + 1}']
+                            if ds_map[-ds_i - 1] == '1'
+                            else np.zeros(5)
+                        )
                         for ds_i in range(sim_ds_count)
                     ],
                     axis=0,
                 )
 
                 time_vals = np.sum(
                     [
-                        time_est[f'DS{ds_i + 1}']
-                        if ds_map[-ds_i - 1] == '1'
-                        else np.zeros(6)
+                        (
+                            time_est[f'DS{ds_i + 1}']
+                            if ds_map[-ds_i - 1] == '1'
+                            else np.zeros(6)
+                        )
                         for ds_i in range(sim_ds_count)
                     ],
                     axis=0,
                 )
 
                 carbon_vals = np.sum(
                     [
-                        carbon_est[f'DS{ds_i + 1}']
-                        if ds_map[-ds_i - 1] == '1'
-                        else np.zeros(3)
+                        (
+                            carbon_est[f'DS{ds_i + 1}']
+                            if ds_map[-ds_i - 1] == '1'
+                            else np.zeros(3)
+                        )
                         for ds_i in range(sim_ds_count)
                     ],
                     axis=0,
                 )
 
                 energy_vals = np.sum(
                     [
-                        energy_est[f'DS{ds_i + 1}']
-                        if ds_map[-ds_i - 1] == '1'
-                        else np.zeros(3)
+                        (
+                            energy_est[f'DS{ds_i + 1}']
+                            if ds_map[-ds_i - 1] == '1'
+                            else np.zeros(3)
+                        )
                         for ds_i in range(sim_ds_count)
                     ],
                     axis=0,
                 )
 
                 # fit a distribution
                 family_hat, theta_hat = fit_distribution_to_percentiles(
@@ -1003,29 +1018,25 @@
                     (cmp.Index, 'Time'), f'DS{DS_i}-Theta_1'
                 ] = f"{time_theta[1]:g}"
 
                 df_db.loc[(cmp.Index, 'Time'), f'DS{DS_i}-LongLeadTime'] = int(
                     time_vals[5] > 0
                 )
 
-                df_db.loc[
-                    (cmp.Index, 'Carbon'), f'DS{DS_i}-Family'
-                ] = family_hat_carbon
+                df_db.loc[(cmp.Index, 'Carbon'), f'DS{DS_i}-Family'] = family_hat_carbon
 
                 df_db.loc[
                     (cmp.Index, 'Carbon'), f'DS{DS_i}-Theta_0'
                 ] = f"{carbon_theta[0]:g}"
 
                 df_db.loc[
                     (cmp.Index, 'Carbon'), f'DS{DS_i}-Theta_1'
                 ] = f"{carbon_theta[1]:g}"
 
-                df_db.loc[
-                    (cmp.Index, 'Energy'), f'DS{DS_i}-Family'
-                ] = family_hat_energy
+                df_db.loc[(cmp.Index, 'Energy'), f'DS{DS_i}-Family'] = family_hat_energy
 
                 df_db.loc[
                     (cmp.Index, 'Energy'), f'DS{DS_i}-Theta_0'
                 ] = f"{energy_theta[0]:g}"
 
                 df_db.loc[
                     (cmp.Index, 'Energy'), f'DS{DS_i}-Theta_1'
@@ -1052,42 +1063,39 @@
                     ds_combo = [
                         f'DS{_.start() + 1}' for _ in re.finditer('1', ds_map[::-1])
                     ]
 
                     meta_data['DamageStates'].update(
                         {
                             f"DS{DS_i}": {
-                                "Description": 'Combination of '
-                                + ' & '.join(ds_combo),
+                                "Description": 'Combination of ' + ' & '.join(ds_combo),
                                 "RepairAction": 'Combination of pure DS repair '
                                 'actions.',
                             }
                         }
                     )
 
         # for every other component...
         else:
             # now look at each Damage State
             for DS_i in range(1, 6):
                 # cost
                 if not pd.isna(getattr(cmp, f'Best_Fit_DS{DS_i}')):
-                    df_db.loc[
-                        (cmp.Index, 'Cost'), f'DS{DS_i}-Family'
-                    ] = convert_family[getattr(cmp, f'Best_Fit_DS{DS_i}')]
+                    df_db.loc[(cmp.Index, 'Cost'), f'DS{DS_i}-Family'] = convert_family[
+                        getattr(cmp, f'Best_Fit_DS{DS_i}')
+                    ]
 
                     if not pd.isna(getattr(cmp, f'Lower_Qty_Mean_DS{DS_i}')):
                         theta_0_low = getattr(cmp, f'Lower_Qty_Mean_DS{DS_i}')
                         theta_0_up = getattr(cmp, f'Upper_Qty_Mean_DS{DS_i}')
                         qnt_low = getattr(cmp, f'Lower_Qty_Cutoff_DS{DS_i}')
                         qnt_up = getattr(cmp, f'Upper_Qty_Cutoff_DS{DS_i}')
 
                         if theta_0_low == 0.0 and theta_0_up == 0.0:
-                            df_db.loc[
-                                (cmp.Index, 'Cost'), f'DS{DS_i}-Family'
-                            ] = np.nan
+                            df_db.loc[(cmp.Index, 'Cost'), f'DS{DS_i}-Family'] = np.nan
 
                         else:
                             df_db.loc[(cmp.Index, 'Cost'), f'DS{DS_i}-Theta_0'] = (
                                 f"{theta_0_low:g},{theta_0_up:g}|"
                                 f"{qnt_low:g},{qnt_up:g}"
                             )
 
@@ -1109,42 +1117,40 @@
                                 "RepairAction": repair_action,
                             }
                         }
                     )
 
                 # time
                 if not pd.isna(getattr(cmp, f'Best_Fit_DS{DS_i}_1')):
-                    df_db.loc[
-                        (cmp.Index, 'Time'), f'DS{DS_i}-Family'
-                    ] = convert_family[getattr(cmp, f'Best_Fit_DS{DS_i}_1')]
+                    df_db.loc[(cmp.Index, 'Time'), f'DS{DS_i}-Family'] = convert_family[
+                        getattr(cmp, f'Best_Fit_DS{DS_i}_1')
+                    ]
 
                     if not pd.isna(getattr(cmp, f'Lower_Qty_Mean_DS{DS_i}_1')):
                         theta_0_low = getattr(cmp, f'Lower_Qty_Mean_DS{DS_i}_1')
                         theta_0_up = getattr(cmp, f'Upper_Qty_Mean_DS{DS_i}_1')
                         qnt_low = getattr(cmp, f'Lower_Qty_Cutoff_DS{DS_i}_1')
                         qnt_up = getattr(cmp, f'Upper_Qty_Cutoff_DS{DS_i}_1')
 
                         if theta_0_low == 0.0 and theta_0_up == 0.0:
-                            df_db.loc[
-                                (cmp.Index, 'Time'), f'DS{DS_i}-Family'
-                            ] = np.nan
+                            df_db.loc[(cmp.Index, 'Time'), f'DS{DS_i}-Family'] = np.nan
 
                         else:
                             df_db.loc[(cmp.Index, 'Time'), f'DS{DS_i}-Theta_0'] = (
                                 f"{theta_0_low:g},{theta_0_up:g}|"
                                 f"{qnt_low:g},{qnt_up:g}"
                             )
 
                             df_db.loc[
                                 (cmp.Index, 'Time'), f'DS{DS_i}-Theta_1'
                             ] = f"{getattr(cmp, f'CV__Dispersion_DS{DS_i}_2'):g}"
 
-                        df_db.loc[
-                            (cmp.Index, 'Time'), f'DS{DS_i}-LongLeadTime'
-                        ] = int(getattr(cmp, f'DS_{DS_i}_Long_Lead_Time') == 'YES')
+                        df_db.loc[(cmp.Index, 'Time'), f'DS{DS_i}-LongLeadTime'] = int(
+                            getattr(cmp, f'DS_{DS_i}_Long_Lead_Time') == 'YES'
+                        )
 
                     else:
                         incomplete_time = True
 
                 # Carbon
                 if not pd.isna(getattr(cmp, f'DS{DS_i}_Best_Fit')):
                     df_db.loc[
@@ -1216,717 +1222,15 @@
     # save the consequence data
     df_db.to_csv(target_data_file)
 
     # save the metadata
     with open(target_meta_file, 'w+', encoding='utf-8') as f:
         json.dump(meta_dict, f, indent=2)
 
-    print(
-        "Successfully parsed and saved the repair consequence data from FEMA P58"
-    )
-
-
-def create_FEMA_P58_bldg_injury_db(
-    source_file,
-    target_data_file='bldg_injury_DB_FEMA_P58_2nd.csv',
-    target_meta_file='bldg_injury_DB_FEMA_P58_2nd.json',
-):
-    """
-    Create an injury consequence parameter database based on the FEMA P58 data
-
-    The method was developed to process v3.1.2 of the FragilityDatabase xls
-    that is provided with FEMA P58 2nd edition.
-
-    Parameters
-    ----------
-    source_file: string
-        Path to the fragility database file.
-    target_data_file: string
-        Path where the consequence data file should be saved. A csv file is
-        expected.
-    target_meta_file: string
-        Path where the consequence metadata should be saved. A json file is
-        expected.
-
-    """
-
-    # parse the source file
-    df = pd.read_excel(
-        source_file,
-        sheet_name='Summary',
-        header=2,
-        index_col=1,
-        true_values=["YES", "Yes", "yes"],
-        false_values=["NO", "No", "no"],
-    )
-
-    # remove empty rows and columns
-    df.dropna(axis=0, how='all', inplace=True)
-    df.dropna(axis=1, how='all', inplace=True)
-
-    # filter the columns we need for the injury database
-    cols_to_db = [
-        "Fragility Unit of Measure",
-        'DS Hierarchy',
-    ]
-    for DS_i in range(1, 6):
-        cols_to_db += [
-            f'DS {DS_i}, Potential non-collapse casualty?',
-            f'DS {DS_i} - Casualty Affected Area',
-            f'DS {DS_i} Serious Injury Rate - Median',
-            f'DS {DS_i} Serious Injury Rate - Dispersion',
-            f'DS {DS_i} Loss of Life Rate - Median',
-            f'DS {DS_i} Loss of Life Rate - Dispersion',
-        ]
-
-    # filter the columns that we need for the metadata
-    cols_to_meta = [
-        "Component Name",
-        "Component Description",
-        "Construction Quality:",
-        "Seismic Installation Conditions:",
-        "Comments / Notes",
-        "Author",
-        "Fragility Unit of Measure",
-        "Round to Integer Unit?",
-        "DS 1, Description",
-        "DS 2, Description",
-        "DS 3, Description",
-        "DS 4, Description",
-        "DS 5, Description",
-    ]
-
-    # remove special characters to make it easier to work with column names
-    str_map = {
-        ord(' '): "_",
-        ord('.'): "_",
-        ord('-'): "_",
-        ord(':'): None,
-        ord('('): None,
-        ord(')'): None,
-        ord('?'): None,
-        ord('/'): None,
-        ord(','): None,
-    }
-
-    df_db_source = df.loc[:, cols_to_db]
-    df_db_source.columns = [s.translate(str_map) for s in cols_to_db]
-    df_db_source.sort_index(inplace=True)
-
-    df_meta = df.loc[:, cols_to_meta]
-    df_meta.columns = [s.translate(str_map) for s in cols_to_meta]
-
-    df_db_source.replace('BY USER', np.nan, inplace=True)
-    df_db_source.replace('By User', np.nan, inplace=True)
-
-    # initialize the output loss table
-    # define the columns
-    out_cols = [
-        "Index",
-        "Incomplete",
-        "Quantity-Unit",
-        "DV-Unit",
-    ]
-    for DS_i in range(1, 16):
-        out_cols += [
-            f"DS{DS_i}-Family",
-            f"DS{DS_i}-Theta_0",
-            f"DS{DS_i}-Theta_1",
-            f"DS{DS_i}-AffectedArea",
-        ]
-
-    # create the MultiIndex
-    comps = df_db_source.index.values
-    DVs = ['S1', 'S2']
-    df_MI = pd.MultiIndex.from_product([comps, DVs], names=['ID', 'Severity'])
-
-    df_db = pd.DataFrame(columns=out_cols, index=df_MI, dtype=float)
-
-    # initialize the dictionary that stores the loss metadata
-    meta_dict = {}
-
-    # for each component...
-    # (this approach is not efficient, but easy to follow which was considered
-    # more important than efficiency.)
-    for cmp in df_db_source.itertuples():
-        ID = cmp.Index.split('.')
-        cmpID = f'{ID[0][0]}.{ID[0][1:3]}.{ID[0][3:5]}.{ID[1]}'
-
-        # store the new index
-        df_db.loc[cmp.Index, 'Index'] = cmpID
-
-        # assume the component information is complete
-        incomplete_S1 = False
-        incomplete_S2 = False
-
-        # store units
-
-        df_db.loc[cmp.Index, 'Quantity-Unit'] = ' '.join(
-            cmp.Fragility_Unit_of_Measure.split(' ')[::-1]
-        ).strip()
-        df_db.loc[(cmp.Index, 'S1'), 'DV-Unit'] = "persons"
-        df_db.loc[(cmp.Index, 'S2'), 'DV-Unit'] = "persons"
-
-        # get the raw metadata for the component
-        cmp_meta = df_meta.loc[cmp.Index, :]
-
-        # store the global (i.e., not DS-specific) metadata
-
-        # start with a comp. description
-        if not pd.isna(cmp_meta['Component_Description']):
-            comments = cmp_meta['Component_Description']
-        else:
-            comments = ''
-
-        # the additional fields are added to the description if they exist
-        if cmp_meta['Construction_Quality'] != 'Not Specified':
-            comments += (
-                f'\nConstruction Quality: ' f'{cmp_meta["Construction_Quality"]}'
-            )
-
-        if cmp_meta['Seismic_Installation_Conditions'] not in [
-            'Not Specified',
-            'Not applicable',
-            'Unknown',
-            'Any',
-        ]:
-            comments += (
-                f'\nSeismic Installation Conditions: '
-                f'{cmp_meta["Seismic_Installation_Conditions"]}'
-            )
-
-        if cmp_meta['Comments__Notes'] != 'None':
-            comments += f'\nNotes: {cmp_meta["Comments__Notes"]}'
-
-        if cmp_meta['Author'] not in ['Not Given', 'By User']:
-            comments += f'\nAuthor: {cmp_meta["Author"]}'
-
-        # get the suggested block size and replace the misleading values with ea
-        block_size = cmp_meta['Fragility_Unit_of_Measure'].split(' ')[::-1]
-
-        meta_data = {
-            "Description": cmp_meta['Component_Name'],
-            "Comments": comments,
-            "SuggestedComponentBlockSize": ' '.join(block_size),
-            "RoundUpToIntegerQuantity": cmp_meta['Round_to_Integer_Unit'],
-            "ControllingDemand": "Damage Quantity",
-            "DamageStates": {},
-        }
-
-        # Handle components with simultaneous damage states separately
-        if 'Simul' in cmp.DS_Hierarchy:
-            # Note that we are assuming that all damage states are triggered by
-            # a single limit state in these components.
-            # This assumption holds for the second edition of FEMA P58, but it
-            # might need to be revisited in future editions.
-
-            inj_data = {}
-            ds_tot = 0
-
-            # get the p10, p50, and p90 estimates for all damage states
-            for DS_i in range(1, 6):
-                casualty_model = getattr(
-                    cmp, f'DS_{DS_i}_Potential_non_collapse_casualty'
-                )
-
-                if casualty_model is True:
-                    inj_data.update(
-                        {
-                            f'DS{DS_i}': np.array(
-                                [
-                                    getattr(
-                                        cmp, f'DS_{DS_i}___Casualty_Affected_Area'
-                                    ),
-                                    getattr(
-                                        cmp,
-                                        f'DS_{DS_i}_Serious_Injury_Rate'
-                                        f'___Median',
-                                    ),
-                                    getattr(
-                                        cmp,
-                                        f'DS_{DS_i}_Serious_Injury_Rate'
-                                        f'___Dispersion',
-                                    ),
-                                    getattr(
-                                        cmp,
-                                        f'DS_{DS_i}_Loss_of_Life_Rate' f'___Median',
-                                    ),
-                                    getattr(
-                                        cmp,
-                                        f'DS_{DS_i}_Loss_of_Life_Rate'
-                                        f'___Dispersion',
-                                    ),
-                                ]
-                            )
-                        }
-                    )
-                    ds_tot += 1
-
-                elif casualty_model is False:
-                    ds_tot += 1
-
-            # only continue if there is injury data
-            if len(inj_data) == 0:
-                continue
-
-            # now prepare the equivalent mutex damage states
-            sim_ds_count = ds_tot
-            ds_count = 2 ** (sim_ds_count) - 1
-
-            # Here we take advantage of knowing that for every component with
-            # simultaneous damage states, only one of the DSs has injury
-            # consequences.
-            # This assumption holds for the second edition of FEMA P58, but it
-            # might need to be revisited in future editions.
-
-            ds_trig = list(inj_data.keys())[0]
-            inj_data = inj_data[ds_trig]
-            ds_trig = int(ds_trig[2:])
-
-            for DS_i in range(1, ds_count + 1):
-                ds_map = format(DS_i, f'0{sim_ds_count}b')
-
-                if ds_map[-ds_trig] == '1':
-                    # store the consequence data
-                    for severity in ('S1', 'S2'):
-                        A_affected = inj_data[0]
-
-                        if severity == 'S1':
-                            theta_0 = inj_data[1]
-                            theta_1 = inj_data[2]
-                        elif severity == 'S2':
-                            theta_0 = inj_data[3]
-                            theta_1 = inj_data[4]
-
-                        if theta_0 != 0.0:
-                            df_db.loc[
-                                (cmp.Index, severity), f'DS{DS_i}-Family'
-                            ] = 'lognormal'
-
-                            df_db.loc[
-                                (cmp.Index, severity), f'DS{DS_i}-Theta_0'
-                            ] = theta_0
-
-                            df_db.loc[
-                                (cmp.Index, severity), f'DS{DS_i}-Theta_1'
-                            ] = theta_1
-
-                            df_db.loc[
-                                (cmp.Index, severity), f'DS{DS_i}-AffectedArea'
-                            ] = A_affected
-
-                # store the metadata
-                if ds_map.count('1') == 1:
-                    ds_pure_id = ds_map[::-1].find('1') + 1
-
-                    meta_data['DamageStates'].update(
-                        {
-                            f"DS{DS_i}": {
-                                "Description": f"Pure DS{ds_pure_id}. "
-                                + cmp_meta[f"DS_{ds_pure_id}_Description"]
-                            }
-                        }
-                    )
-
-                else:
-                    ds_combo = [
-                        f'DS{_.start() + 1}' for _ in re.finditer('1', ds_map[::-1])
-                    ]
-
-                    meta_data['DamageStates'].update(
-                        {
-                            f"DS{DS_i}": {
-                                "Description": 'Combination of '
-                                + ' & '.join(ds_combo)
-                            }
-                        }
-                    )
-
-        # for every other component...
-        else:
-            # now look at each Damage State
-            for DS_i in range(1, 6):
-                casualty_flag = getattr(
-                    cmp, f'DS_{DS_i}_Potential_non_collapse_casualty'
-                )
-
-                if casualty_flag is True:
-                    A_affected = getattr(cmp, f'DS_{DS_i}___Casualty_Affected_Area')
-
-                    for severity in ('S1', 'S2'):
-                        if severity == 'S1':
-                            theta_0 = getattr(
-                                cmp, f'DS_{DS_i}_Serious_Injury_' f'Rate___Median'
-                            )
-                            theta_1 = getattr(
-                                cmp,
-                                f'DS_{DS_i}_Serious_Injury_' f'Rate___Dispersion',
-                            )
-                        elif severity == 'S2':
-                            theta_0 = getattr(
-                                cmp, f'DS_{DS_i}_Loss_of_Life_' f'Rate___Median'
-                            )
-                            theta_1 = getattr(
-                                cmp, f'DS_{DS_i}_Loss_of_Life_' f'Rate___Dispersion'
-                            )
-
-                        if theta_0 != 0.0:
-                            df_db.loc[
-                                (cmp.Index, severity), f'DS{DS_i}-Family'
-                            ] = 'lognormal'
-
-                            df_db.loc[
-                                (cmp.Index, severity), f'DS{DS_i}-Theta_0'
-                            ] = theta_0
-
-                            df_db.loc[
-                                (cmp.Index, severity), f'DS{DS_i}-Theta_1'
-                            ] = theta_1
-
-                            df_db.loc[
-                                (cmp.Index, severity), f'DS{DS_i}-AffectedArea'
-                            ] = A_affected
-
-                            if (
-                                pd.isna(theta_0)
-                                or pd.isna(theta_1)
-                                or pd.isna(A_affected)
-                            ):
-                                if severity == 'S1':
-                                    incomplete_S1 = True
-                                else:
-                                    incomplete_S2 = True
-
-                if ~np.isnan(casualty_flag):
-                    meta_data['DamageStates'].update(
-                        {
-                            f"DS{DS_i}": {
-                                "Description": cmp_meta[f"DS_{DS_i}_Description"]
-                            }
-                        }
-                    )
-
-        df_db.loc[(cmp.Index, 'S1'), 'Incomplete'] = int(incomplete_S1)
-        df_db.loc[(cmp.Index, 'S2'), 'Incomplete'] = int(incomplete_S2)
-
-        # store the metadata for this component
-        meta_dict.update({cmpID: meta_data})
-
-    # assign the Index column as the new ID
-    df_db.index = pd.MultiIndex.from_arrays(
-        [df_db['Index'].values, df_db.index.get_level_values(1)]
-    )
-
-    df_db.drop('Index', axis=1, inplace=True)
-
-    # review the database and drop rows with no information
-    cmp_to_drop = []
-    for cmp in df_db.index:
-        empty = True
-
-        for DS_i in range(1, 16):
-            if not pd.isna(df_db.loc[cmp, f'DS{DS_i}-Family']):
-                empty = False
-                break
-
-        if empty:
-            cmp_to_drop.append(cmp)
-
-    df_db.drop(cmp_to_drop, axis=0, inplace=True)
-    cmp_kept = df_db.index.get_level_values(0).unique()
-
-    cmp_to_drop = []
-    for cmp in meta_dict:
-        if cmp not in cmp_kept:
-            cmp_to_drop.append(cmp)
-
-    for cmp in cmp_to_drop:
-        del meta_dict[cmp]
-
-    # convert to optimal datatypes to reduce file size
-    df_db = df_db.convert_dtypes()
-
-    df_db = base.convert_to_SimpleIndex(df_db, 0)
-
-    # rename the index
-    df_db.index.name = "ID"
-
-    # save the consequence data
-    df_db.to_csv(target_data_file)
-
-    # save the metadata
-    with open(target_meta_file, 'w+', encoding='utf-8') as f:
-        json.dump(meta_dict, f, indent=2)
-
-    print(
-        "Successfully parsed and saved the injury consequence data from FEMA P58"
-    )
-
-
-def create_FEMA_P58_bldg_redtag_db(
-    source_file,
-    target_data_file='bldg_redtag_DB_FEMA_P58_2nd.csv',
-    target_meta_file='bldg_redtag_DB_FEMA_P58_2nd.json',
-):
-    """
-    Create an red tag consequence parameter database based on the FEMA P58 data
-
-    The method was developed to process v3.1.2 of the FragilityDatabase xls
-    that is provided with FEMA P58 2nd edition.
-
-    Parameters
-    ----------
-    source_file: string
-        Path to the fragility database file.
-    target_data_file: string
-        Path where the consequence data file should be saved. A csv file is
-        expected.
-    target_meta_file: string
-        Path where the consequence metadata should be saved. A json file is
-        expected.
-
-    """
-
-    # parse the source file
-    df = pd.read_excel(
-        source_file,
-        sheet_name='Summary',
-        header=2,
-        index_col=1,
-        true_values=["YES", "Yes", "yes"],
-        false_values=["NO", "No", "no"],
-    )
-
-    # take another pass with booleans because the first does not always work
-    for true_str in ("YES", "Yes", "yes"):
-        df.replace(true_str, True, inplace=True)
-
-    for false_str in ("NO", "No", "no"):
-        df.replace(false_str, False, inplace=True)
-
-    # remove empty rows and columns
-    df.dropna(axis=0, how='all', inplace=True)
-    df.dropna(axis=1, how='all', inplace=True)
-
-    # filter the columns we need for the injury database
-    cols_to_db = [
-        'DS Hierarchy',
-    ]
-    for DS_i in range(1, 6):
-        cols_to_db += [
-            f'DS {DS_i}, Unsafe Placard Trigger Flag',
-            f'DS {DS_i}, Unsafe Placard Damage Median',
-            f'DS {DS_i}, Unsafe Placard Damage Dispersion',
-        ]
-
-    # filter the columns that we need for the metadata
-    cols_to_meta = [
-        "Component Name",
-        "Component Description",
-        "Construction Quality:",
-        "Seismic Installation Conditions:",
-        "Comments / Notes",
-        "Author",
-        "Fragility Unit of Measure",
-        "Round to Integer Unit?",
-        "DS 1, Description",
-        "DS 2, Description",
-        "DS 3, Description",
-        "DS 4, Description",
-        "DS 5, Description",
-    ]
-
-    # remove special characters to make it easier to work with column names
-    str_map = {
-        ord(' '): "_",
-        ord('.'): "_",
-        ord('-'): "_",
-        ord(':'): None,
-        ord('('): None,
-        ord(')'): None,
-        ord('?'): None,
-        ord('/'): None,
-        ord(','): None,
-    }
-
-    df_db_source = df.loc[:, cols_to_db]
-    df_db_source.columns = [s.translate(str_map) for s in cols_to_db]
-    df_db_source.sort_index(inplace=True)
-
-    df_meta = df.loc[:, cols_to_meta]
-    df_meta.columns = [s.translate(str_map) for s in cols_to_meta]
-
-    df_db_source.replace('BY USER', np.nan, inplace=True)
-    df_db_source.replace('By User', np.nan, inplace=True)
-
-    # initialize the output loss table
-    # define the columns
-    out_cols = [
-        "Index",
-        "Incomplete",
-    ]
-    for DS_i in range(1, 6):
-        out_cols += [f"DS{DS_i}-Family", f"DS{DS_i}-Theta_0", f"DS{DS_i}-Theta_1"]
-
-    # create the database index
-    comps = df_db_source.index.values
-
-    df_db = pd.DataFrame(columns=out_cols, index=comps, dtype=float)
-
-    # initialize the dictionary that stores the loss metadata
-    meta_dict = {}
-
-    # for each component...
-    # (this approach is not efficient, but easy to follow which was considered
-    # more important than efficiency.)
-    for cmp in df_db_source.itertuples():
-        ID = cmp.Index.split('.')
-        cmpID = f'{ID[0][0]}.{ID[0][1:3]}.{ID[0][3:5]}.{ID[1]}'
-
-        # store the new index
-        df_db.loc[cmp.Index, 'Index'] = cmpID
-
-        # assume the component information is complete
-        incomplete = False
-
-        # get the raw metadata for the component
-        cmp_meta = df_meta.loc[cmp.Index, :]
-
-        # store the global (i.e., not DS-specific) metadata
-
-        # start with a comp. description
-        if not pd.isna(cmp_meta['Component_Description']):
-            comments = cmp_meta['Component_Description']
-        else:
-            comments = ''
-
-        # the additional fields are added to the description if they exist
-        if cmp_meta['Construction_Quality'] != 'Not Specified':
-            comments += (
-                f'\nConstruction Quality: ' f'{cmp_meta["Construction_Quality"]}'
-            )
-
-        if cmp_meta['Seismic_Installation_Conditions'] not in [
-            'Not Specified',
-            'Not applicable',
-            'Unknown',
-            'Any',
-        ]:
-            comments += (
-                f'\nSeismic Installation Conditions: '
-                f'{cmp_meta["Seismic_Installation_Conditions"]}'
-            )
-
-        if cmp_meta['Comments__Notes'] != 'None':
-            comments += f'\nNotes: {cmp_meta["Comments__Notes"]}'
-
-        if cmp_meta['Author'] not in ['Not Given', 'By User']:
-            comments += f'\nAuthor: {cmp_meta["Author"]}'
-
-        # get the suggested block size and replace the misleading values with ea
-        block_size = cmp_meta['Fragility_Unit_of_Measure'].split(' ')[::-1]
-
-        meta_data = {
-            "Description": cmp_meta['Component_Name'],
-            "Comments": comments,
-            "SuggestedComponentBlockSize": ' '.join(block_size),
-            "RoundUpToIntegerQuantity": cmp_meta['Round_to_Integer_Unit'],
-            "ControllingDemand": "Damage Quantity",
-            "DamageStates": {},
-        }
-
-        # Handle components with simultaneous damage states separately
-        if 'Simul' in cmp.DS_Hierarchy:
-            pass
-            # Note that we are assuming that components with simultaneous
-            # damage states do not have damage that would trigger a red tag.
-            # This assumption holds for the second edition of FEMA P58, but it
-            # might need to be revisited in future editions.
-
-        # for every other component...
-        else:
-            # now look at each Damage State
-            for DS_i in range(1, 6):
-                redtag_flag = getattr(cmp, f'DS_{DS_i}_Unsafe_Placard_Trigger_Flag')
-
-                if redtag_flag is True:
-                    theta_0 = getattr(
-                        cmp, f'DS_{DS_i}_Unsafe_Placard_Damage_' f'Median'
-                    )
-                    theta_1 = getattr(
-                        cmp, f'DS_{DS_i}_Unsafe_Placard_Damage_' f'Dispersion'
-                    )
-
-                    if theta_0 != 0.0:
-                        df_db.loc[cmp.Index, f'DS{DS_i}-Family'] = 'lognormal'
-
-                        df_db.loc[cmp.Index, f'DS{DS_i}-Theta_0'] = theta_0
-
-                        df_db.loc[cmp.Index, f'DS{DS_i}-Theta_1'] = theta_1
-
-                        if pd.isna(theta_0) or pd.isna(theta_1):
-                            incomplete = True
-
-                if ~np.isnan(redtag_flag):
-                    meta_data['DamageStates'].update(
-                        {
-                            f"DS{DS_i}": {
-                                "Description": cmp_meta[f"DS_{DS_i}_Description"]
-                            }
-                        }
-                    )
-
-        df_db.loc[cmp.Index, 'Incomplete'] = int(incomplete)
-
-        # store the metadata for this component
-        meta_dict.update({cmpID: meta_data})
-
-    # assign the Index column as the new ID
-    df_db.set_index('Index', inplace=True)
-
-    # review the database and drop rows with no information
-    cmp_to_drop = []
-    for cmp in df_db.index:
-        empty = True
-
-        for DS_i in range(1, 6):
-            if not pd.isna(df_db.loc[cmp, f'DS{DS_i}-Family']):
-                empty = False
-                break
-
-        if empty:
-            cmp_to_drop.append(cmp)
-
-    df_db.drop(cmp_to_drop, axis=0, inplace=True)
-    cmp_kept = df_db.index.get_level_values(0).unique()
-
-    cmp_to_drop = []
-    for cmp in meta_dict:
-        if cmp not in cmp_kept:
-            cmp_to_drop.append(cmp)
-
-    for cmp in cmp_to_drop:
-        del meta_dict[cmp]
-
-    # convert to optimal datatypes to reduce file size
-    df_db = df_db.convert_dtypes()
-
-    # rename the index
-    df_db.index.name = "ID"
-
-    # save the consequence data
-    df_db.to_csv(target_data_file)
-
-    # save the metadata
-    with open(target_meta_file, 'w+', encoding='utf-8') as f:
-        json.dump(meta_dict, f, indent=2)
-
-    print(
-        "Successfully parsed and saved the red tag consequence data from FEMA P58"
-    )
+    print("Successfully parsed and saved the repair consequence data from FEMA P58")
 
 
 def create_Hazus_EQ_fragility_db(
     source_file,
     meta_file='',
     target_data_file='damage_DB_Hazus_EQ_bldg.csv',
     target_meta_file='damage_DB_Hazus_EQ_bldg.json',
@@ -1971,21 +1275,17 @@
     if Path(meta_file).is_file():
         with open(meta_file, 'r', encoding='utf-8') as f:
             frag_meta = json.load(f)
     else:
         frag_meta = {}
 
     # prepare lists of labels for various building features
-    design_levels = list(
-        raw_data['Structural_Fragility_Groups']['EDP_limits'].keys()
-    )
+    design_levels = list(raw_data['Structural_Fragility_Groups']['EDP_limits'].keys())
 
-    building_types = list(
-        raw_data['Structural_Fragility_Groups']['P_collapse'].keys()
-    )
+    building_types = list(raw_data['Structural_Fragility_Groups']['P_collapse'].keys())
 
     convert_design_level = {
         'High_code': 'HC',
         'Moderate_code': 'MC',
         'Low_code': 'LC',
         'Pre_code': 'PC',
     }
@@ -2079,17 +1379,15 @@
 
                 # add metadata
                 if hc is not None:
                     cmp_meta = {
                         "Description": (
                             frag_meta['Meta']['Collections']['STR']['Description']
                             + ", "
-                            + frag_meta['Meta']['StructuralSystems'][st][
-                                'Description'
-                            ]
+                            + frag_meta['Meta']['StructuralSystems'][st]['Description']
                             + ", "
                             + frag_meta['Meta']['HeightClasses'][hc]['Description']
                             + ", "
                             + frag_meta['Meta']['DesignLevels'][
                                 convert_design_level[dl]
                             ]['Description']
                         ),
@@ -2109,17 +1407,15 @@
                         "LimitStates": {},
                     }
                 else:
                     cmp_meta = {
                         "Description": (
                             frag_meta['Meta']['Collections']['STR']['Description']
                             + ", "
-                            + frag_meta['Meta']['StructuralSystems'][st][
-                                'Description'
-                            ]
+                            + frag_meta['Meta']['StructuralSystems'][st]['Description']
                             + ", "
                             + frag_meta['Meta']['DesignLevels'][
                                 convert_design_level[dl]
                             ]['Description']
                         ),
                         "Comments": (
                             frag_meta['Meta']['Collections']['STR']['Comment']
@@ -2135,20 +1431,20 @@
                         "LimitStates": {},
                     }
 
                 # store the Limit State parameters
                 ds_meta = frag_meta['Meta']['StructuralSystems'][st]['DamageStates']
                 for LS_i in range(1, 5):
                     df_db.loc[counter, f'LS{LS_i}-Family'] = 'lognormal'
-                    df_db.loc[counter, f'LS{LS_i}-Theta_0'] = S_data['EDP_limits'][
+                    df_db.loc[counter, f'LS{LS_i}-Theta_0'] = S_data['EDP_limits'][dl][
+                        bt
+                    ][LS_i - 1]
+                    df_db.loc[counter, f'LS{LS_i}-Theta_1'] = S_data['Fragility_beta'][
                         dl
-                    ][bt][LS_i - 1]
-                    df_db.loc[counter, f'LS{LS_i}-Theta_1'] = S_data[
-                        'Fragility_beta'
-                    ][dl]
+                    ]
 
                     if LS_i == 4:
                         p_coll = S_data['P_collapse'][bt]
                         df_db.loc[
                             counter, f'LS{LS_i}-DamageStateWeights'
                         ] = f'{1.0 - p_coll} | {p_coll}'
 
@@ -2161,17 +1457,15 @@
                             }
                         )
 
                     else:
                         cmp_meta["LimitStates"].update(
                             {
                                 f"LS{LS_i}": {
-                                    f"DS{LS_i}": {
-                                        "Description": ds_meta[f"DS{LS_i}"]
-                                    }
+                                    f"DS{LS_i}": {"Description": ds_meta[f"DS{LS_i}"]}
                                 }
                             }
                         )
 
                 # store metadata
                 meta_dict.update({cmp_id: cmp_meta})
 
@@ -2239,17 +1533,15 @@
                 + frag_meta['Meta']['DesignLevels'][convert_design_level[dl]][
                     'Description'
                 ]
             ),
             "Comments": (
                 frag_meta['Meta']['Collections']['NSA']['Comment']
                 + "\n"
-                + frag_meta['Meta']['DesignLevels'][convert_design_level[dl]][
-                    'Comment'
-                ]
+                + frag_meta['Meta']['DesignLevels'][convert_design_level[dl]]['Comment']
             ),
             "SuggestedComponentBlockSize": "1 EA",
             "RoundUpToIntegerQuantity": "True",
             "LimitStates": {},
         }
 
         # store the Limit State parameters
@@ -2303,28 +1595,24 @@
                             "Description": (
                                 frag_meta['Meta']['Collections']['LF']['Description']
                                 + ", "
                                 + frag_meta['Meta']['StructuralSystems'][st][
                                     'Description'
                                 ]
                                 + ", "
-                                + frag_meta['Meta']['HeightClasses'][hc][
-                                    'Description'
-                                ]
+                                + frag_meta['Meta']['HeightClasses'][hc]['Description']
                                 + ", "
                                 + frag_meta['Meta']['DesignLevels'][
                                     convert_design_level[dl]
                                 ]['Description']
                             ),
                             "Comments": (
                                 frag_meta['Meta']['Collections']['LF']['Comment']
                                 + "\n"
-                                + frag_meta['Meta']['StructuralSystems'][st][
-                                    'Comment'
-                                ]
+                                + frag_meta['Meta']['StructuralSystems'][st]['Comment']
                                 + "\n"
                                 + frag_meta['Meta']['HeightClasses'][hc]['Comment']
                                 + "\n"
                                 + frag_meta['Meta']['DesignLevels'][
                                     convert_design_level[dl]
                                 ]['Comment']
                             ),
@@ -2344,36 +1632,32 @@
                                 + frag_meta['Meta']['DesignLevels'][
                                     convert_design_level[dl]
                                 ]['Description']
                             ),
                             "Comments": (
                                 frag_meta['Meta']['Collections']['LF']['Comment']
                                 + "\n"
-                                + frag_meta['Meta']['StructuralSystems'][st][
-                                    'Comment'
-                                ]
+                                + frag_meta['Meta']['StructuralSystems'][st]['Comment']
                                 + "\n"
                                 + frag_meta['Meta']['DesignLevels'][
                                     convert_design_level[dl]
                                 ]['Comment']
                             ),
                             "SuggestedComponentBlockSize": "1 EA",
                             "RoundUpToIntegerQuantity": "True",
                             "LimitStates": {},
                         }
 
                     # store the Limit State parameters
-                    ds_meta = frag_meta['Meta']['StructuralSystems'][st][
-                        'DamageStates'
-                    ]
+                    ds_meta = frag_meta['Meta']['StructuralSystems'][st]['DamageStates']
                     for LS_i in range(1, 5):
                         df_db.loc[counter, f'LS{LS_i}-Family'] = 'lognormal'
-                        df_db.loc[counter, f'LS{LS_i}-Theta_0'] = LF_data[
-                            'EDP_limits'
-                        ][dl][bt][LS_i - 1]
+                        df_db.loc[counter, f'LS{LS_i}-Theta_0'] = LF_data['EDP_limits'][
+                            dl
+                        ][bt][LS_i - 1]
                         df_db.loc[counter, f'LS{LS_i}-Theta_1'] = LF_data[
                             'Fragility_beta'
                         ][dl]
 
                         if LS_i == 4:
                             p_coll = LF_data['P_collapse'][bt]
                             df_db.loc[
@@ -2548,17 +1832,15 @@
         out_cols += [
             f"DS{DS_i}-Theta_0",
         ]
 
     # create the MultiIndex
     cmp_types = ['STR', 'NSD', 'NSA', 'LF']
     comps = [
-        f'{cmp_type}.{occ_type}'
-        for cmp_type in cmp_types
-        for occ_type in occupancies
+        f'{cmp_type}.{occ_type}' for cmp_type in cmp_types for occ_type in occupancies
     ]
     DVs = ['Cost', 'Time']
     df_MI = pd.MultiIndex.from_product([comps, DVs], names=['ID', 'DV'])
 
     df_db = pd.DataFrame(columns=out_cols, index=df_MI, dtype=float)
 
     # initialize the dictionary that stores the loss metadata
@@ -2650,17 +1932,17 @@
         # store the consequence values for each Damage State
         ds_meta = frag_meta['Meta']['Collections']['NSD']['DamageStates']
         for DS_i in range(1, 5):
             cmp_meta["DamageStates"].update(
                 {f"DS{DS_i}": {"Description": ds_meta[f"DS{DS_i}"]}}
             )
 
-            df_db.loc[(cmp_id, 'Cost'), f'DS{DS_i}-Theta_0'] = NSD_data[
-                'Repair_cost'
-            ][occ_type][DS_i - 1]
+            df_db.loc[(cmp_id, 'Cost'), f'DS{DS_i}-Theta_0'] = NSD_data['Repair_cost'][
+                occ_type
+            ][DS_i - 1]
 
         # store metadata
         meta_dict.update({cmp_id: cmp_meta})
 
     # Third, the non-structural acceleration sensitive fragilities
     NSA_data = raw_data['NonStructural_Acceleration_Sensitive_Fragility_Groups']
 
@@ -2687,17 +1969,17 @@
         # store the consequence values for each Damage State
         ds_meta = frag_meta['Meta']['Collections']['NSA']['DamageStates']
         for DS_i in range(1, 5):
             cmp_meta["DamageStates"].update(
                 {f"DS{DS_i}": {"Description": ds_meta[f"DS{DS_i}"]}}
             )
 
-            df_db.loc[(cmp_id, 'Cost'), f'DS{DS_i}-Theta_0'] = NSA_data[
-                'Repair_cost'
-            ][occ_type][DS_i - 1]
+            df_db.loc[(cmp_id, 'Cost'), f'DS{DS_i}-Theta_0'] = NSA_data['Repair_cost'][
+                occ_type
+            ][DS_i - 1]
 
         # store metadata
         meta_dict.update({cmp_id: cmp_meta})
 
     # Fourth, the lifeline facilities - only at the building-level resolution
     if resolution == 'building':
         LF_data = raw_data['Lifeline_Facilities']
@@ -2772,144 +2054,586 @@
     # save the consequence data
     df_db.to_csv(target_data_file)
 
     # save the metadata - later
     with open(target_meta_file, 'w+', encoding='utf-8') as f:
         json.dump(meta_dict, f, indent=2)
 
-    print(
-        "Successfully parsed and saved the repair consequence data from Hazus EQ"
-    )
+    print("Successfully parsed and saved the repair consequence data from Hazus EQ")
 
 
-def create_Hazus_EQ_bldg_injury_db(
-    source_file,
-    target_data_file='bldg_injury_DB_Hazus_EQ.csv',
-    target_meta_file='bldg_injury_DB_Hazus_EQ.json',
-):
+def create_Hazus_HU_fragility_db(
+    source_file: str = (
+        'pelicun/resources/SimCenterDBDL/' 'damage_DB_SimCenter_Hazus_HU_bldg.csv'
+    ),
+    meta_file: str = (
+        'pelicun/resources/SimCenterDBDL/'
+        'damage_DB_SimCenter_Hazus_HU_bldg_template.json'
+    ),
+    target_meta_file: str = 'damage_DB_SimCenter_Hazus_HU_bldg.json',
+) -> None:
     """
-    Create a database file based on the HAZUS EQ Technical Manual
+    Create a database metadata file for the HAZUS Hurricane fragilities.
 
-    This method was developed to process a json file with tabulated data from
-    v4.2.3 of the Hazus Earthquake Technical Manual. The json file is included
-    under data_sources in the SimCenter DB_DamageAndLoss repo on GitHub.
+    This method was developed to add a json file with metadata
+    accompanying `damage_DB_SimCenter_Hazus_HU_bldg.csv`. That file
+    contains fragility curves fitted to Hazus Hurricane data relaetd
+    to the Hazus Hurricane Technical Manual v4.2.
 
     Parameters
     ----------
     source_file: string
-        Path to the Hazus database file.
-    target_data_file: string
-        Path where the injury DB file should be saved. A csv file is
-        expected.
+        Path to the Hazus Hurricane fragility data.
+    meta_file: string
+        Path to a predefined fragility metadata file.
     target_meta_file: string
-        Path where the injury DB metadata should be saved. A json file is
+        Path where the fragility metadata should be saved. A json file is
         expected.
 
     """
 
-    # parse the source file
-    with open(source_file, 'r', encoding='utf-8') as f:
-        raw_data = json.load(f)
+    fragility_data = pd.read_csv(source_file)
 
-    # # parse the extra metadata file
-    # if Path(meta_file).is_file():
-    #     with open(meta_file, 'r') as f:
-    #         frag_meta = json.load(f)
-    # else:
-    #     frag_meta = {}
+    with open(meta_file, 'r', encoding='utf-8') as f:
+        meta_dict = json.load(f)
 
-    # prepare lists of labels for various building features
-    building_types = list(
-        raw_data['Structural_Fragility_Groups']['P_collapse'].keys()
-    )
+    # retrieve damage state descriptions and remove that part from
+    # `hazus_hu_metadata`
+    damage_state_classes = meta_dict.pop('DamageStateClasses')
+    damage_state_descriptions = meta_dict.pop('DamageStateDescriptions')
+
+    # Procedure Overview:
+    # (1) We define several dictionaries mapping chunks of the
+    # composite asset ID (the parts between periods) to human-readable
+    # (`-h` for short) representations.
+    # (2) We define -h asset type descriptions and map them to the
+    # first-most relevant ID chunks (`primary chunks`)
+    # (3) We map asset class codes with general asset classes
+    # (4) We define the required dictionaries from (1) that decode the
+    # ID chunks after the `primary chunks` for each general asset
+    # class
+    # (5) We decode:
+    # ID -> asset class -> general asset class -> dictionaries
+    # -> ID turns to -h text by combining the description of the asset class
+    # from the `primary chunks` and the decoded description of the
+    # following chunks using the dictionaries.
+
+    #
+    # (1) Dictionaries
+    #
+
+    roof_shape = {
+        'flt': 'Flat roof.',
+        'gab': 'Gable roof.',
+        'hip': 'Hip roof.',
+    }
 
-    # initialize the output loss table
-    # define the columns
-    out_cols = [
-        "Incomplete",
-        "Quantity-Unit",
-        "DV-Unit",
-    ]
-    for DS_i in range(1, 6):
-        out_cols += [
-            f"DS{DS_i}-Theta_0",
-        ]
+    secondary_water_resistance = {
+        '1': 'Secondary water resistance.',
+        '0': 'No secondary water resistance.',
+        'null': 'No information on secondary water resistance.',
+    }
 
-    # create the MultiIndex
-    cmp_types = ['STR', 'LF']
-    comps = [f'{cmp_type}.{bt}' for cmp_type in cmp_types for bt in building_types]
-    DVs = ['S1', 'S2', 'S3', 'S4']
-    df_MI = pd.MultiIndex.from_product([comps, DVs], names=['ID', 'DV'])
+    roof_deck_attachment = {
+        '6d': '6d roof deck nails.',
+        '6s': '6s roof deck nails.',
+        '8d': '8d roof deck nails.',
+        '8s': '8s roof deck nails.',
+        'st': 'Standard roof deck attachment.',
+        'su': 'Superior roof deck attachment.',
+        'null': 'Missing roof deck attachment information.',
+    }
 
-    df_db = pd.DataFrame(columns=out_cols, index=df_MI, dtype=float)
+    roof_wall_connection = {
+        'tnail': 'Roof-to-wall toe nails.',
+        'strap': 'Roof-to-wall straps.',
+        'null': 'Missing roof-to-wall connection information.',
+    }
 
-    # First, prepare the structural damage consequences
-    S_data = raw_data['Structural_Fragility_Groups']
+    garage_presence = {
+        'no': 'No garage.',
+        'wkd': 'Weak garage door.',
+        'std': 'Standard garage door.',
+        'sup': 'Strong garage door.',
+        'null': 'No information on garage.',
+    }
 
-    for bt in building_types:
-        # create the component id
-        cmp_id = f'STR.{bt}'
+    shutters = {'1': 'Has Shutters.', '0': 'No shutters.'}
 
-        # store the consequence values for each Damage State
-        for DS_i in range(1, 6):
-            # DS5 is stored under 'collapse'
-            if DS_i == 5:
-                ds_i = 'Collapse'
-            else:
-                ds_i = f'DS{DS_i}'
+    roof_cover = {
+        'bur': 'Built-up roof cover.',
+        'spm': 'Single-ply membrane roof cover.',
+        'smtl': 'Sheet metal roof cover.',
+        'cshl': 'Shingle roof cover.',
+        'null': 'No information on roof cover.',
+    }
 
-            for S_i in range(1, 5):
-                s_label = f'S{S_i}'
-                df_db.loc[(cmp_id, s_label), f'DS{DS_i}-Theta_0'] = S_data[
-                    'Injury_rates'
-                ][ds_i][bt][S_i - 1]
+    roof_quality = {
+        'god': 'Good roof quality.',
+        'por': 'Poor roof quality.',
+        'null': 'No information on roof quality.',
+    }
 
-    # Second, the lifeline facilities
+    masonry_reinforcing = {
+        '1': 'Has masonry reinforcing.',
+        '0': 'No masonry reinforcing.',
+        'null': 'Unknown information on masonry reinfocing.',
+    }
 
-    for bt in building_types:
-        # create the component id
-        cmp_id = f'STR.{bt}'
+    roof_frame_type = {
+        'trs': 'Wood truss roof frame.',
+        'ows': 'OWSJ roof frame.',
+    }
 
-        # store the consequence values for each Damage State
-        for DS_i in range(1, 6):
-            # DS5 is stored under 'collapse'
-            if DS_i == 5:
-                ds_i = 'Collapse'
-            else:
-                ds_i = f'DS{DS_i}'
+    wind_debris_environment = {
+        'A': 'Residentiao/commercial wind debris environment.',
+        'B': 'Wind debris environment varies by direction.',
+        'C': 'Residential wind debris environment.',
+        'D': 'No wind debris environment.',
+    }
 
-            for S_i in range(1, 5):
-                s_label = f'S{S_i}'
-                df_db.loc[(cmp_id, s_label), f'DS{DS_i}-Theta_0'] = S_data[
-                    'Injury_rates'
-                ][ds_i][bt][S_i - 1]
+    roof_deck_age = {
+        'god': 'New or average roof age.',
+        'por': 'Old roof age.',
+        'null': 'Missing roof age information.',
+    }
 
-    # remove empty rows
-    df_db.dropna(how='all', inplace=True)
+    roof_metal_deck_attachment_quality = {
+        'std': 'Standard metal deck roof attachment.',
+        'sup': 'Superior metal deck roof attachment.',
+        'null': 'Missing roof attachment quality information.',
+    }
 
-    # All Hazus components have complete fragility info,
-    df_db.loc[:, 'Incomplete'] = 0
+    number_of_units = {
+        'sgl': 'Single unit.',
+        'mlt': 'Multi-unit.',
+        'null': 'Unknown number of units.',
+    }
 
-    # The damage quantity unit is the same for all consequence values
-    df_db.loc[:, 'Quantity-Unit'] = "1 EA"
+    joist_spacing = {
+        '4': '4 ft joist spacing.',
+        '6': '6 ft foot joist spacing.',
+        'null': 'Unknown joist spacing.',
+    }
 
-    # The output units are also identical among all components
-    df_db.loc[:, 'DV-Unit'] = "injury_rate"
+    window_area = {
+        'low': 'Low window area.',
+        'med': 'Medium window area.',
+        'hig': 'High window area.',
+    }
 
-    # convert to simple index
-    df_db = base.convert_to_SimpleIndex(df_db, 0)
+    tie_downs = {'1': 'Tie downs.', '0': 'No tie downs.'}
 
-    # rename the index
-    df_db.index.name = "ID"
+    terrain_surface_roughness = {
+        '3': 'Terrain surface roughness: 0.03 m.',
+        '15': 'Terrain surface roughness: 0.15 m.',
+        '35': 'Terrain surface roughness: 0.35 m.',
+        '70': 'Terrain surface roughness: 0.7 m.',
+        '100': 'Terrain surface roughness: 1 m.',
+    }
 
-    # convert to optimal datatypes to reduce file size
-    df_db = df_db.convert_dtypes()
+    #
+    # (2) Asset type descriptions
+    #
+
+    # maps class type code to -h description
+    class_types = {
+        # ------------------------
+        'W.SF.1': 'Wood, Single-family, One-story.',
+        'W.SF.2': 'Wood, Single-family, Two or More Stories.',
+        # ------------------------
+        'W.MUH.1': 'Wood, Multi-Unit Housing, One-story.',
+        'W.MUH.2': 'Wood, Multi-Unit Housing, Two Stories.',
+        'W.MUH.3': 'Wood, Multi-Unit Housing, Three or More Stories.',
+        # ------------------------
+        'M.SF.1': 'Masonry, Single-family, One-story.',
+        'M.SF.2': 'Masonry, Single-family, Two or More Stories.',
+        # ------------------------
+        'M.MUH.1': 'Masonry, Multi-Unit Housing, One-story.',
+        'M.MUH.2': 'Masonry, Multi-Unit Housing, Two Stories.',
+        'M.MUH.3': 'Masonry, Multi-Unit Housing, Three or More Stories.',
+        # ------------------------
+        'M.LRM.1': 'Masonry, Low-Rise Strip Mall, Up to 15 Feet.',
+        'M.LRM.2': 'Masonry, Low-Rise Strip Mall, More than 15 Feet.',
+        # ------------------------
+        'M.LRI': 'Masonry, Low-Rise Industrial/Warehouse/Factory Buildings.',
+        # ------------------------
+        'M.ERB.L': (
+            'Masonry, Engineered Residential Building, Low-Rise (1-2 Stories).'
+        ),
+        'M.ERB.M': (
+            'Masonry, Engineered Residential Building, Mid-Rise (3-5 Stories).'
+        ),
+        'M.ERB.H': (
+            'Masonry, Engineered Residential Building, High-Rise (6+ Stories).'
+        ),
+        # ------------------------
+        'M.ECB.L': ('Masonry, Engineered Commercial Building, Low-Rise (1-2 Stories).'),
+        'M.ECB.M': ('Masonry, Engineered Commercial Building, Mid-Rise (3-5 Stories).'),
+        'M.ECB.H': ('Masonry, Engineered Commercial Building, High-Rise (6+ Stories).'),
+        # ------------------------
+        'C.ERB.L': (
+            'Concrete, Engineered Residential Building, Low-Rise (1-2 Stories).'
+        ),
+        'C.ERB.M': (
+            'Concrete, Engineered Residential Building, Mid-Rise (3-5 Stories).'
+        ),
+        'C.ERB.H': (
+            'Concrete, Engineered Residential Building, High-Rise (6+ Stories).'
+        ),
+        # ------------------------
+        'C.ECB.L': (
+            'Concrete, Engineered Commercial Building, Low-Rise (1-2 Stories).'
+        ),
+        'C.ECB.M': (
+            'Concrete, Engineered Commercial Building, Mid-Rise (3-5 Stories).'
+        ),
+        'C.ECB.H': (
+            'Concrete, Engineered Commercial Building, High-Rise (6+ Stories).'
+        ),
+        # ------------------------
+        'S.PMB.S': 'Steel, Pre-Engineered Metal Building, Small.',
+        'S.PMB.M': 'Steel, Pre-Engineered Metal Building, Medium.',
+        'S.PMB.L': 'Steel, Pre-Engineered Metal Building, Large.',
+        # ------------------------
+        'S.ERB.L': 'Steel, Engineered Residential Building, Low-Rise (1-2 Stories).',
+        'S.ERB.M': 'Steel, Engineered Residential Building, Mid-Rise (3-5 Stories).',
+        'S.ERB.H': 'Steel, Engineered Residential Building, High-Rise (6+ Stories).',
+        # ------------------------
+        'S.ECB.L': 'Steel, Engineered Commercial Building, Low-Rise (1-2 Stories).',
+        'S.ECB.M': 'Steel, Engineered Commercial Building, Mid-Rise (3-5 Stories).',
+        'S.ECB.H': 'Steel, Engineered Commercial Building, High-Rise (6+ Stories).',
+        # ------------------------
+        'MH.PHUD': 'Manufactured Home, Pre-Housing and Urban Development (HUD).',
+        'MH.76HUD': 'Manufactured Home, 1976 HUD.',
+        'MH.94HUDI': 'Manufactured Home, 1994 HUD - Wind Zone I.',
+        'MH.94HUDII': 'Manufactured Home, 1994 HUD - Wind Zone II.',
+        'MH.94HUDIII': 'Manufactured Home, 1994 HUD - Wind Zone III.',
+        # ------------------------
+        'HUEF.H.S': 'Small Hospital, Hospital with fewer than 50 Beds.',
+        'HUEF.H.M': 'Medium Hospital, Hospital with beds between 50 & 150.',
+        'HUEF.H.L': 'Large Hospital, Hospital with more than 150 Beds.',
+        # ------------------------
+        'HUEF.S.S': 'Elementary School.',
+        'HUEF.S.M': 'High school, two-story.',
+        'HUEF.S.L': 'Large high school, three-story.',
+        # ------------------------
+        'HUEF.EO': 'Emergency Operation Centers.',
+        'HUEF.FS': 'Fire Station.',
+        'HUEF.PS': 'Police Station.',
+        # ------------------------
+    }
 
-    # save the consequence data
-    df_db.to_csv(target_data_file)
+    def find_class_type(entry: str) -> str | None:
+        """
+        Find the class type code from an entry string based on
+        predefined patterns.
+
+        Parameters
+        ----------
+        entry : str
+            A string representing the entry, consisting of delimited
+            segments that correspond to various attributes of an
+            asset.
+
+        Returns
+        -------
+        str or None
+            The class type code if a matching pattern is found;
+            otherwise, None if no pattern matches the input string.
+
+        """
+        entry_elements = entry.split('.')
+        for nper in range(1, len(entry_elements)):
+            first_parts = '.'.join(entry_elements[:nper])
+            if first_parts in class_types:
+                return first_parts
+        return None
+
+    #
+    # (3) General asset class
+    #
+
+    # maps class code type to general class code
+    general_classes = {
+        # ------------------------
+        'W.SF.1': 'WSF',
+        'W.SF.2': 'WSF',
+        # ------------------------
+        'W.MUH.1': 'WMUH',
+        'W.MUH.2': 'WMUH',
+        'W.MUH.3': 'WMUH',
+        # ------------------------
+        'M.SF.1': 'MSF',
+        'M.SF.2': 'MSF',
+        # ------------------------
+        'M.MUH.1': 'MMUH',
+        'M.MUH.2': 'MMUH',
+        'M.MUH.3': 'MMUH',
+        # ------------------------
+        'M.LRM.1': 'MLRM1',
+        'M.LRM.2': 'MLRM2',
+        # ------------------------
+        'M.LRI': 'MLRI',
+        # ------------------------
+        'M.ERB.L': 'MERB',
+        'M.ERB.M': 'MERB',
+        'M.ERB.H': 'MERB',
+        # ------------------------
+        'M.ECB.L': 'MECB',
+        'M.ECB.M': 'MECB',
+        'M.ECB.H': 'MECB',
+        # ------------------------
+        'C.ERB.L': 'CERB',
+        'C.ERB.M': 'CERB',
+        'C.ERB.H': 'CERB',
+        # ------------------------
+        'C.ECB.L': 'CECB',
+        'C.ECB.M': 'CECB',
+        'C.ECB.H': 'CECB',
+        # ------------------------
+        'S.PMB.S': 'SPMB',
+        'S.PMB.M': 'SPMB',
+        'S.PMB.L': 'SPMB',
+        # ------------------------
+        'S.ERB.L': 'SERB',
+        'S.ERB.M': 'SERB',
+        'S.ERB.H': 'SERB',
+        # ------------------------
+        'S.ECB.L': 'SECB',
+        'S.ECB.M': 'SECB',
+        'S.ECB.H': 'SECB',
+        # ------------------------
+        'MH.PHUD': 'MH',
+        'MH.76HUD': 'MH',
+        'MH.94HUDI': 'MH',
+        'MH.94HUDII': 'MH',
+        'MH.94HUDIII': 'MH',
+        # ------------------------
+        'HUEF.H.S': 'HUEFH',
+        'HUEF.H.M': 'HUEFH',
+        'HUEF.H.L': 'HUEFH',
+        # ------------------------
+        'HUEF.S.S': 'HUEFS',
+        'HUEF.S.M': 'HUEFS',
+        'HUEF.S.L': 'HUEFS',
+        # ------------------------
+        'HUEF.EO': 'HUEFEO',
+        'HUEF.FS': 'HUEFFS',
+        'HUEF.PS': 'HUEFPS',
+        # ------------------------
+    }
 
-    # save the metadata - later
-    # with open(target_meta_file, 'w+') as f:
-    #    json.dump(meta_dict, f, indent=2)
+    #
+    # (4) Relevant dictionaries
+    #
+
+    # maps general class code to list of dicts where the -h attribute
+    # descriptions will be pulled from
+    dictionaries_of_interest = {
+        'WSF': [
+            roof_shape,
+            secondary_water_resistance,
+            roof_deck_attachment,
+            roof_wall_connection,
+            garage_presence,
+            shutters,
+            terrain_surface_roughness,
+        ],
+        'WMUH': [
+            roof_shape,
+            roof_cover,
+            roof_quality,
+            secondary_water_resistance,
+            roof_deck_attachment,
+            roof_wall_connection,
+            shutters,
+            terrain_surface_roughness,
+        ],
+        'MSF': [
+            roof_shape,
+            roof_wall_connection,
+            roof_frame_type,
+            roof_deck_attachment,
+            shutters,
+            secondary_water_resistance,
+            garage_presence,
+            masonry_reinforcing,
+            roof_cover,
+            terrain_surface_roughness,
+        ],
+        'MMUH': [
+            roof_shape,
+            secondary_water_resistance,
+            roof_cover,
+            roof_quality,
+            roof_deck_attachment,
+            roof_wall_connection,
+            shutters,
+            masonry_reinforcing,
+            terrain_surface_roughness,
+        ],
+        'MLRM1': [
+            roof_cover,
+            shutters,
+            masonry_reinforcing,
+            wind_debris_environment,
+            roof_frame_type,
+            roof_deck_attachment,
+            roof_wall_connection,
+            roof_deck_age,
+            roof_metal_deck_attachment_quality,
+            terrain_surface_roughness,
+        ],
+        'MLRM2': [
+            roof_cover,
+            shutters,
+            masonry_reinforcing,
+            wind_debris_environment,
+            roof_frame_type,
+            roof_deck_attachment,
+            roof_wall_connection,
+            roof_deck_age,
+            roof_metal_deck_attachment_quality,
+            number_of_units,
+            joist_spacing,
+            terrain_surface_roughness,
+        ],
+        'MLRI': [
+            shutters,
+            masonry_reinforcing,
+            roof_deck_age,
+            roof_metal_deck_attachment_quality,
+            terrain_surface_roughness,
+        ],
+        'MERB': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            roof_metal_deck_attachment_quality,
+            window_area,
+            terrain_surface_roughness,
+        ],
+        'MECB': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            roof_metal_deck_attachment_quality,
+            window_area,
+            terrain_surface_roughness,
+        ],
+        'CERB': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            window_area,
+            terrain_surface_roughness,
+        ],
+        'CECB': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            window_area,
+            terrain_surface_roughness,
+        ],
+        'SPMB': [
+            shutters,
+            roof_deck_age,
+            roof_metal_deck_attachment_quality,
+            terrain_surface_roughness,
+        ],
+        'SERB': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            roof_metal_deck_attachment_quality,
+            window_area,
+            terrain_surface_roughness,
+        ],
+        'SECB': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            roof_metal_deck_attachment_quality,
+            window_area,
+            terrain_surface_roughness,
+        ],
+        'MH': [shutters, tie_downs, terrain_surface_roughness],
+        'HUEFH': [
+            roof_cover,
+            wind_debris_environment,
+            roof_metal_deck_attachment_quality,
+            shutters,
+            terrain_surface_roughness,
+        ],
+        'HUEFS': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            roof_deck_age,
+            roof_metal_deck_attachment_quality,
+            terrain_surface_roughness,
+        ],
+        'HUEFEO': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            roof_metal_deck_attachment_quality,
+            window_area,
+            terrain_surface_roughness,
+        ],
+        'HUEFFS': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            roof_deck_age,
+            roof_metal_deck_attachment_quality,
+            terrain_surface_roughness,
+        ],
+        'HUEFPS': [
+            roof_cover,
+            shutters,
+            wind_debris_environment,
+            roof_metal_deck_attachment_quality,
+            window_area,
+            terrain_surface_roughness,
+        ],
+    }
+
+    #
+    # (5) Decode IDs and extend metadata with the individual records
+    #
+
+    for fragility_id in fragility_data['ID'].to_list():
+        class_type = find_class_type(fragility_id)
+
+        class_type_human_readable = class_types[class_type]
+
+        general_class = general_classes[class_type]
+        dictionaries = dictionaries_of_interest[general_class]
+        remaining_chunks = fragility_id.replace(f'{class_type}.', '').split('.')
+        assert len(remaining_chunks) == len(dictionaries)
+        human_description = [class_type_human_readable]
+        for chunk, dictionary in zip(remaining_chunks, dictionaries):
+            human_description.append(dictionary[chunk])
+        human_description_str = ' '.join(human_description)
+
+        damage_state_class = damage_state_classes[class_type]
+        damage_state_description = damage_state_descriptions[damage_state_class]
+
+        limit_states = {}
+        for damage_state, description in damage_state_description.items():
+            limit_state = damage_state.replace('DS', 'LS')
+            limit_states[limit_state] = {damage_state: description}
+
+        record = {
+            'Description': human_description_str,
+            'SuggestedComponentBlockSize': '1 EA',
+            'RoundUpToIntegerQuantity': 'True',
+            'LimitStates': limit_states,
+        }
+
+        meta_dict[fragility_id] = record
 
-    print("Successfully parsed and saved the injury consequence data from Hazus "
-          "EQ")
+    # save the metadata
+    with open(target_meta_file, 'w+', encoding='utf-8') as f:
+        json.dump(meta_dict, f, indent=2)
```

### Comparing `pelicun-3.3.2/pelicun/examples/001/CMP_QNT.csv` & `pelicun-3.3.3/pelicun/examples/001/CMP_QNT.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/examples/001/demands_s4.csv` & `pelicun-3.3.3/pelicun/examples/001/demands_s4.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/examples/001/input.json` & `pelicun-3.3.3/pelicun/examples/001/input.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/examples/002/input.json` & `pelicun-3.3.3/pelicun/examples/002/input.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/examples/002/response.csv` & `pelicun-3.3.3/pelicun/examples/002/response.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/examples/0_tmp/CMP_marginals.csv` & `pelicun-3.3.3/pelicun/examples/0_tmp/CMP_marginals.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/examples/0_tmp/config.json` & `pelicun-3.3.3/pelicun/examples/0_tmp/config.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/examples/0_tmp/demands.csv` & `pelicun-3.3.3/pelicun/examples/0_tmp/demands.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/examples/0_tmp/fragility_Additional.csv` & `pelicun-3.3.3/pelicun/examples/0_tmp/fragility_Additional.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/file_io.py` & `pelicun-3.3.3/pelicun/file_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,117 +67,134 @@
     'DV_injuries_1': 'Injuries lvl. 2',
     'DV_injuries_2': 'Injuries lvl. 3',
     'DV_injuries_3': 'Injuries lvl. 4',
     'DV_red_tag': 'Red Tag ',
 }
 
 dependency_to_acronym = {
-    'btw. Fragility Groups':   'FG',
+    'btw. Fragility Groups': 'FG',
     'btw. Performance Groups': 'PG',
-    'btw. Floors':             'LOC',
-    'btw. Directions':         'DIR',
-    'btw. Component Groups':   'CSG',
-    'btw. Damage States':      'DS',
-    'Independent':             'IND',
-    'per ATC recommendation':  'ATC',
+    'btw. Floors': 'LOC',
+    'btw. Directions': 'DIR',
+    'btw. Component Groups': 'CSG',
+    'btw. Damage States': 'DS',
+    'Independent': 'IND',
+    'per ATC recommendation': 'ATC',
 }
 
 HAZUS_occ_converter = {
-    'RES':  'Residential',
-    'COM':  'Commercial',
-    'REL':  'Commercial',
-    'EDU':  'Educational',
-    'IND':  'Industrial',
-    'AGR':  'Industrial'
+    'RES': 'Residential',
+    'COM': 'Commercial',
+    'REL': 'Commercial',
+    'EDU': 'Educational',
+    'IND': 'Industrial',
+    'AGR': 'Industrial',
 }
 
 
-def save_to_csv(data, filepath, units=None, unit_conversion_factors=None,
-                orientation=0, use_simpleindex=True, log=None):
+def save_to_csv(
+    data,
+    filepath,
+    units=None,
+    unit_conversion_factors=None,
+    orientation=0,
+    use_simpleindex=True,
+    log=None,
+):
     """
-    Saves data to a CSV file following standard SimCenter schema.
+    Saves data to a CSV file following the standard SimCenter schema.
 
-    The produced CSV files have a single header line and an index column. The
-    second line may start with 'Units' in the index or the first column may be
-    'Units' to provide the units for the data in the file.
-
-    The following data types in pelicun can be saved with this function:
-
-    Demand Data: Each column in a table corresponds to a demand type; each
-    row corresponds to a simulation/sample. The header identifies each demand
-    type. The user guide section of the documentation provides more
-    information about the header format. Target need to be specified in the
-    second row of the DataFrame.
+    The produced CSV files have a single header line and an index
+    column. The second line may start with 'Units' in the index or the
+    first column may be 'Units' to provide the units for the data in
+    the file.
+
+    The following data types in pelicun can be saved with this
+    function:
+
+    Demand Data: Each column in a table corresponds to a demand type;
+    each row corresponds to a simulation/sample. The header identifies
+    each demand type. The user guide section of the documentation
+    provides more information about the header format. Target need to
+    be specified in the second row of the DataFrame.
 
     Parameters
     ----------
-    data: DataFrame
-        The data to save
-    filepath: string
-        The location of the destination file. If None, the data is not saved,
-        but returned in the end.
-    units: Series, optional
+    data : DataFrame
+        The data to save.
+    filepath : str
+        The location of the destination file. If None, the data is not
+        saved, but returned in the end.
+    units : Series, optional
         Provides a Series with variables and corresponding units.
-    unit_conversion_factors: dict
+    unit_conversion_factors : dict, optional
         Dictionary containing key-value pairs of unit names and their
-        corresponding factors. Conversion factors are defined as the number of
-        times a base unit fits in the alternative unit.
-    orientation: int, {0, 1}, default: 0
-        If 0, variables are organized along columns; otherwise they are along
-        the rows. This is important when converting values to follow the
-        prescribed units.
-    use_simpleindex: bool, default: True
-        If True, MultiIndex columns and indexes are converted to SimpleIndex
-        before saving
-    log: Logger
-        Logger object to be used. If no object is specified, no logging
-        is performed.
+        corresponding factors. Conversion factors are defined as the
+        number of times a base unit fits in the alternative unit.
+    orientation : int, {0, 1}, default 0
+        If 0, variables are organized along columns; otherwise, they
+        are along the rows. This is important when converting values
+        to follow the prescribed units.
+    use_simpleindex : bool, default True
+        If True, MultiIndex columns and indexes are converted to
+        SimpleIndex before saving.
+    log : Logger, optional
+        Logger object to be used. If no object is specified, no
+        logging is performed.
 
     Raises
     ------
     ValueError
-        If units is not None but unit_conversion_factors is None
+        If units is not None but unit_conversion_factors is None.
     ValueError
         If writing to a file fails.
     ValueError
         If the provided file name does not have the `.csv` suffix.
+
+    Returns
+    -------
+    DataFrame or None
+        If `filepath` is None, returns the DataFrame with potential
+        unit conversions and reformatting applied. Otherwise, returns
+        None after saving the data to a CSV file.
     """
 
     if filepath is None:
-        if log: log.msg('Preparing data ...', prepend_timestamp=False)
+        if log:
+            log.msg('Preparing data ...', prepend_timestamp=False)
 
-    elif log: log.msg(f'Saving data to {filepath}...', prepend_timestamp=False)
+    elif log:
+        log.msg(f'Saving data to {filepath}...', prepend_timestamp=False)
 
     if data is not None:
-
         # make sure we do not modify the original data
         data = data.copy()
 
         # convert units and add unit information, if needed
         if units is not None:
-
             if unit_conversion_factors is None:
                 raise ValueError(
                     'When units is not None, '
-                    'unit_conversion_factors must be provided')
+                    'unit_conversion_factors must be provided'
+                )
 
-            if log: log.msg('Converting units...', prepend_timestamp=False)
+            if log:
+                log.msg('Converting units...', prepend_timestamp=False)
 
             # if the orientation is 1, we might not need to scale all columns
             if orientation == 1:
                 cols_to_scale = [dt in [float, int] for dt in data.dtypes]
                 cols_to_scale = data.columns[cols_to_scale]
 
             labels_to_keep = []
 
             for unit_name in units.unique():
-
                 labels = units.loc[units == unit_name].index.values
 
-                unit_factor = 1. / unit_conversion_factors[unit_name]
+                unit_factor = 1.0 / unit_conversion_factors[unit_name]
 
                 active_labels = []
 
                 if orientation == 0:
                     for label in labels:
                         if label in data.columns:
                             active_labels.append(label)
@@ -200,49 +217,49 @@
             if orientation == 0:
                 data = pd.concat([units.T, data], axis=0)
                 data.sort_index(axis=1, inplace=True)
             else:
                 data = pd.concat([units, data], axis=1)
                 data.sort_index(inplace=True)
 
-            if log: log.msg('Unit conversion successful.', prepend_timestamp=False)
+            if log:
+                log.msg('Unit conversion successful.', prepend_timestamp=False)
 
         if use_simpleindex:
             # convert MultiIndex to regular index with '-' separators
             if isinstance(data.index, pd.MultiIndex):
                 data = base.convert_to_SimpleIndex(data)
 
             # same thing for the columns
             if isinstance(data.columns, pd.MultiIndex):
                 data = base.convert_to_SimpleIndex(data, axis=1)
 
         if filepath is not None:
-
             filepath = Path(filepath).resolve()
             if filepath.suffix == '.csv':
-
                 # save the contents of the DataFrame into a csv
                 data.to_csv(filepath)
 
-                if log: log.msg('Data successfully saved to file.',
-                                prepend_timestamp=False)
+                if log:
+                    log.msg('Data successfully saved to file.', prepend_timestamp=False)
 
             else:
                 raise ValueError(
                     f'ERROR: Unexpected file type received when trying '
-                    f'to save to csv: {filepath}')
+                    f'to save to csv: {filepath}'
+                )
 
             return None
 
         # at this line, filepath is None
         return data
 
     # at this line, data is None
-    if log: log.msg('WARNING: Data was empty, no file saved.',
-                    prepend_timestamp=False)
+    if log:
+        log.msg('WARNING: Data was empty, no file saved.', prepend_timestamp=False)
     return None
 
 
 def substitute_default_path(data_paths):
     """
     Substitutes the default directory path in a list of data paths
     with a specified path.
@@ -338,19 +355,27 @@
         in unit conversion.
     log: Logger
         Logger object to be used. If no object is specified, no logging
         is performed.
 
     Returns
     -------
-    data: DataFrame
-        Parsed data.
-    units: Series
-        Labels from the data and corresponding units specified in the
-        data. Units are only returned if return_units is set to True.
+    tuple
+        data: DataFrame
+            Parsed data.
+        units: Series
+            Labels from the data and corresponding units specified in the
+            data. Units are only returned if return_units is set to True.
+
+    Raises
+    ------
+    TypeError
+        If `data_source` is neither a string nor a DataFrame, a TypeError is raised.
+    ValueError
+        If `unit_conversion_factors` contains keys that do not correspond to any units in the data, a ValueError may be raised during processing.
     """
 
     if isinstance(data_source, pd.DataFrame):
         # store it at proceed (copying is needed to avoid changing the
         # original)
         data = data_source.copy()
     elif isinstance(data_source, str):
@@ -362,15 +387,14 @@
     # Define a dictionary to decide the axis based on the orientation
     axis = {0: 1, 1: 0}
     the_index = data.columns if orientation == 1 else data.index
 
     # if there is information about units, separate that information
     # and optionally apply conversions to all numeric values
     if 'Units' in the_index:
-
         units = data['Units'] if orientation == 1 else data.loc['Units']
         data.drop('Units', axis=orientation, inplace=True)
         data = base.convert_dtypes(data)
 
         if unit_conversion_factors is not None:
             numeric_elements = (
                 (data.select_dtypes(include=[np.number]).index)
@@ -378,27 +402,27 @@
                 else (data.select_dtypes(include=[np.number]).columns)
             )
 
             if log:
                 log.msg('Converting units...', prepend_timestamp=False)
 
             conversion_factors = units.map(
-                lambda unit: 1.00
-                if pd.isna(unit)
-                else unit_conversion_factors.get(unit, 1.00)
+                lambda unit: (
+                    1.00 if pd.isna(unit) else unit_conversion_factors.get(unit, 1.00)
+                )
             )
 
             if orientation == 1:
-                data.loc[:, numeric_elements] = data.loc[
-                    :, numeric_elements
-                ].multiply(conversion_factors, axis=axis[orientation])
+                data.loc[:, numeric_elements] = data.loc[:, numeric_elements].multiply(
+                    conversion_factors, axis=axis[orientation]
+                )
             else:
-                data.loc[numeric_elements, :] = data.loc[
-                    numeric_elements, :
-                ].multiply(conversion_factors, axis=axis[orientation])
+                data.loc[numeric_elements, :] = data.loc[numeric_elements, :].multiply(
+                    conversion_factors, axis=axis[orientation]
+                )
 
         if log:
             log.msg('Unit conversion successful.', prepend_timestamp=False)
 
     else:
         units = None
         data = base.convert_dtypes(data)
@@ -440,45 +464,54 @@
     Parameters
     ----------
     filepath: string
         The location of the source file
 
     Returns
     -------
-    data: DataFrame
-        Data loaded from the file.
-    log: Logger
-        Logger object to be used. If no object is specified, no logging
-        is performed.
+    tuple
+        data: DataFrame
+            Data loaded from the file.
+        log: Logger
+            Logger object to be used. If no object is specified, no logging
+            is performed.
 
     Raises
     ------
     FileNotFoundError
         If the filepath is invalid.
     ValueError
         If the file is not a CSV.
     """
 
-    if log: log.msg(f'Loading data from {filepath}...')
+    if log:
+        log.msg(f'Loading data from {filepath}...')
 
     # check if the filepath is valid
     filepath = Path(filepath).resolve()
 
     if not filepath.is_file():
         raise FileNotFoundError(
-            f"The filepath provided does not point to an existing "
-            f"file: {filepath}")
+            f"The filepath provided does not point to an existing " f"file: {filepath}"
+        )
 
     if filepath.suffix == '.csv':
-
         # load the contents of the csv into a DataFrame
 
-        data = pd.read_csv(filepath, header=0, index_col=0, low_memory=False,
-                           encoding_errors='replace')
+        data = pd.read_csv(
+            filepath,
+            header=0,
+            index_col=0,
+            low_memory=False,
+            encoding_errors='replace',
+        )
 
-        if log: log.msg('File successfully opened.', prepend_timestamp=False)
+        if log:
+            log.msg('File successfully opened.', prepend_timestamp=False)
 
     else:
-        raise ValueError(f'ERROR: Unexpected file type received when trying '
-                         f'to load from csv: {filepath}')
+        raise ValueError(
+            f'ERROR: Unexpected file type received when trying '
+            f'to load from csv: {filepath}'
+        )
 
     return data
```

### Comparing `pelicun-3.3.2/pelicun/model/__init__.py` & `pelicun-3.3.3/pelicun/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/model/damage_model.py` & `pelicun-3.3.3/pelicun/model/damage_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,40 +89,63 @@
         super().__init__(assessment)
 
         self.damage_params = None
         self.sample = None
 
     def save_sample(self, filepath=None, save_units=False):
         """
-        Save damage sample to a csv file
+        Saves the damage sample data to a CSV file or returns it
+        directly with an option to include units.
 
+        This function handles saving the sample data of damage
+        assessments to a specified file path or, if no path is
+        provided, returns the data as a DataFrame. The function can
+        optionally include a row for unit information when returning
+        data.
+
+        Parameters
+        ----------
+        filepath : str, optional
+            The path to the file where the damage sample should be
+            saved. If not provided, the sample is not saved to disk
+            but returned.
+        save_units : bool, default: False
+            Indicates whether to include a row with unit information
+            in the returned DataFrame. This parameter is ignored if a
+            file path is provided.
+
+        Returns
+        -------
+        None or tuple
+            If `filepath` is provided, the function returns None after
+            saving the data.
+            If no `filepath` is specified, returns:
+            - DataFrame containing the damage sample.
+            - Optionally, a Series containing the units for each
+              column if `save_units` is True.
         """
         self.log_div()
         self.log_msg('Saving damage sample...')
 
         cmp_units = self._asmnt.asset.cmp_units
-        qnt_units = pd.Series(
-            index=self.sample.columns, name='Units', dtype='object'
-        )
+        qnt_units = pd.Series(index=self.sample.columns, name='Units', dtype='object')
         for cmp in cmp_units.index:
             qnt_units.loc[cmp] = cmp_units.loc[cmp]
 
         res = file_io.save_to_csv(
             self.sample,
             filepath,
             units=qnt_units,
             unit_conversion_factors=self._asmnt.unit_conversion_factors,
             use_simpleindex=(filepath is not None),
             log=self._asmnt.log,
         )
 
         if filepath is not None:
-            self.log_msg(
-                'Damage sample successfully saved.', prepend_timestamp=False
-            )
+            self.log_msg('Damage sample successfully saved.', prepend_timestamp=False)
             return None
 
         # else:
         units = res.loc["Units"]
         res.drop("Units", inplace=True)
         res.index = res.index.astype('int64')
 
@@ -244,17 +267,22 @@
         operation: str
           Any of +, -, *, /
         other_value: float
           Value used to apply the operation
 
         Returns
         -------
-        result: float
+        float
           The result of the operation
 
+        Raises
+        ------
+        ValueError
+            If the operation is invalid.
+
         """
         if operation == '+':
             return initial_value + other_value
         if operation == '-':
             return initial_value - other_value
         if operation == '*':
             return initial_value * other_value
@@ -264,15 +292,15 @@
 
     def _create_dmg_RVs(self, PGB, scaling_specification=None):
         """
         Creates random variables required later for the damage calculation.
 
         The method initializes two random variable registries,
         capacity_RV_reg and lsds_RV_reg, and loops through each
-        performance group in the input performance group block (PGB)
+        performance group in the input performance group batch (PGB)
         dataframe. For each performance group, it retrieves the
         component sample and blocks and checks if the limit state is
         defined for the component. If the limit state is defined, the
         method gets the list of limit states and the parameters for
         each limit state. The method assigns correlation between limit
         state random variables, adds the limit state random variables
         to the capacity_RV_reg registry, and adds LSDS assignments to
@@ -289,22 +317,72 @@
             Example: {'CMP-1-1': '*1.2', 'CMP-1-2': '/1.4'}
             The keys are individual components that should be present
             in the `capacity_sample`.  The values should be strings
             containing an operation followed by the value formatted as
             a float.  The operation can be '+' for addition, '-' for
             subtraction, '*' for multiplication, and '/' for division.
 
+        Returns
+        -------
+        tuple
+            A tuple containing two RandomVariableRegistry instances:
+            one for the capacity random variables and one for the LSDS
+            assignments.
+
+        Raises
+        ------
+        ValueError
+            Raises an error if the scaling specification is invalid or
+            if the input DataFrame does not meet the expected format.
+            Also, raises errors if there are any issues with the types
+            or formats of the data in the input DataFrame.
         """
 
         def assign_lsds(ds_weights, ds_id, lsds_RV_reg, lsds_rv_tag):
             """
-            Prepare random variables to handle mutually exclusive damage states.
-
+            Assigns limit states to damage states using random
+            variables, updating the provided random variable registry.
+            This function either creates a deterministic random
+            variable for a single damage state or a multinomial random
+            variable for multiple damage states.
+
+            Parameters
+            ----------
+            ds_weights : str or None
+                A string representing the weights of different damage
+                states associated with a limit state, separated by
+                '|'.  If None, indicates that there is only one damage
+                state associated with the limit state.
+            ds_id : int
+                The starting index for damage state IDs. This ID helps
+                in mapping damage states to limit states.
+            lsds_RV_reg : RandomVariableRegistry
+                The registry where the newly created random variables
+                (for mapping limit states to damage states) will be
+                added.
+            lsds_rv_tag : str
+                A unique identifier for the random variable being
+                created, typically including identifiers for
+                component, location, direction, and limit state.
+
+            Returns
+            -------
+            int
+                The updated damage state ID, incremented based on the
+                number of damage states handled in this call.
+
+            Notes
+            -----
+            This function supports detailed control over the mapping
+            from limit states to damage states within a stochastic
+            framework, enhancing the flexibility and accuracy of
+            probabilistic damage assessments. It dynamically adjusts
+            to the number of damage states specified and applies a
+            mapping function to correctly assign state IDs.
             """
-
             # If the limit state has a single damage state assigned
             # to it, we don't need random sampling
             if pd.isnull(ds_weights):
                 ds_id += 1
 
                 lsds_RV_reg.add_RV(
                     uq.DeterministicRandomVariable(
@@ -317,14 +395,37 @@
             else:
                 # parse the DS weights
                 ds_weights = np.array(
                     ds_weights.replace(" ", "").split('|'), dtype=float
                 )
 
                 def map_ds(values, offset=int(ds_id + 1)):
+                    """
+                    Maps an array of damage state indices to their
+                    corresponding actual state IDs by applying an
+                    offset.
+
+                    Parameters
+                    ----------
+                    values : array-like
+                        An array of indices representing damage
+                        states. These indices are typically sequential
+                        integers starting from zero.
+                    offset : int
+                        The value to be added to each element in
+                        `values` to obtain the actual damage state
+                        IDs.
+
+                    Returns
+                    -------
+                    array
+                        An array where each original index from
+                        `values` has been incremented by `offset` to
+                        reflect its actual damage state ID.
+                    """
                     return values + offset
 
                 lsds_RV_reg.add_RV(
                     uq.MultinomialRandomVariable(
                         name=lsds_rv_tag,
                         theta=ds_weights,
                         f_map=map_ds,
@@ -374,17 +475,15 @@
                 )
                 scaling_specification = parsed_scaling_specification
 
         # get the component sample and blocks from the asset model
         for PG in PGB.index:
             # determine demand capacity adjustment operation, if required
             cmp_loc_dir = '-'.join(PG[0:3])
-            capacity_adjustment_operation = scaling_specification.get(
-                cmp_loc_dir, None
-            )
+            capacity_adjustment_operation = scaling_specification.get(cmp_loc_dir, None)
 
             cmp_id = PG[0]
             blocks = PGB.loc[PG, 'Blocks']
 
             # Calculate the block weights
             blocks = np.full(int(blocks), 1.0 / blocks)
 
@@ -588,17 +687,15 @@
         )
 
         if self._asmnt.log.verbose:
             self.log_msg("Raw samples are available", prepend_timestamp=True)
 
         # get the capacity and lsds samples
         capacity_sample = (
-            pd.DataFrame(capacity_RVs.RV_sample)
-            .sort_index(axis=0)
-            .sort_index(axis=1)
+            pd.DataFrame(capacity_RVs.RV_sample).sort_index(axis=0).sort_index(axis=1)
         )
         capacity_sample = base.convert_to_MultiIndex(capacity_sample, axis=1)['FRG']
         capacity_sample.columns.names = ['cmp', 'loc', 'dir', 'uid', 'block', 'ls']
 
         lsds_sample = (
             pd.DataFrame(lsds_RVs.RV_sample)
             .sort_index(axis=0)
@@ -644,15 +741,15 @@
         ----------
         `PGB`: pd.DataFrame
             A pandas DataFrame with the block information for
             each component
 
         Returns
         -------
-        EDP_req: dict
+        dict
             A dictionary of EDP requirements, where each key is the EDP
             string (e.g., "Peak Ground Acceleration-0-0"), and the
             corresponding value is a list of tuples (component_id,
             location, direction)
 
         """
 
@@ -792,17 +889,15 @@
             # if non-directional demand is requested...
             if EDP[2] == '0':
                 # assume that the demand at the given location is available
                 try:
                     # take the maximum of all available directions and scale it
                     # using the nondirectional multiplier specified in the
                     # self._asmnt.options (the default value is 1.2)
-                    demand = (
-                        demand_source.loc[:, (EDP[0], EDP[1])].max(axis=1).values
-                    )
+                    demand = demand_source.loc[:, (EDP[0], EDP[1])].max(axis=1).values
                     demand = demand * self._asmnt.options.nondir_multi(EDP[0])
 
                 except KeyError:
                     demand = None
 
             else:
                 demand = demand_source[(EDP[0], EDP[1], EDP[2])].values
@@ -835,15 +930,15 @@
             Provides a sample of the capacity.
         lsds_sample: DataFrame
             Provides the mapping between limit states and damage
             states.
 
         Returns
         -------
-        dmg_sample: DataFrame
+        DataFrame
             Assigns a Damage State to each component block in the
             asset model.
         """
 
         # Log a message indicating that damage states are being
         # evaluated
 
@@ -869,17 +964,15 @@
             PG_cols = pd.concat(
                 [dmg_eval.loc[:1, PG_i] for PG_i in PG_list], axis=1, keys=PG_list
             ).columns
             PG_cols.names = ['cmp', 'loc', 'dir', 'uid', 'block', 'ls']
             # Create a dataframe with demand values repeated for the
             # number of PGs and assign the columns as PG_cols
             demand_df.append(
-                pd.concat(
-                    [pd.Series(demand_vals)] * len(PG_cols), axis=1, keys=PG_cols
-                )
+                pd.concat([pd.Series(demand_vals)] * len(PG_cols), axis=1, keys=PG_cols)
             )
 
         # Concatenate all demand dataframes into a single dataframe
         demand_df = pd.concat(demand_df, axis=1)
         # Sort the columns of the demand dataframe
         demand_df.sort_index(axis=1, inplace=True)
 
@@ -890,15 +983,15 @@
         # Remove any columns with NaN values from the damage
         # exceedance dataframe
         dmg_eval.dropna(axis=1, inplace=True)
 
         # initialize the DataFrames that store the damage states and
         # quantities
         ds_sample = pd.DataFrame(
-            0,                  # fill value
+            0,  # fill value
             columns=capacity_sample.columns.droplevel('ls').unique(),
             index=capacity_sample.index,
             dtype='int32',
         )
 
         # get a list of limit state ids among all components in the damage model
         ls_list = dmg_eval.columns.get_level_values(5).unique()
@@ -931,43 +1024,41 @@
             # damage states.
             ds_sample.loc[:, dmg_e_ls.columns] = ds_sample.loc[
                 :, dmg_e_ls.columns
             ].mask(dmg_e_ls, lsds)
 
         return ds_sample
 
-    def _prepare_dmg_quantities(self, component_blocks, ds_sample, dropzero=True):
+    def _prepare_dmg_quantities(self, damage_state_sample, dropzero=True):
         """
         Combine component quantity and damage state information in one
         DataFrame.
 
         This method assumes that a component quantity sample is
         available in the asset model and a damage state sample is
         available in the damage model.
 
         Parameters
         ----------
-        component_blocks: DataFrame
-            A DataFrame that contains the number of blocks for each
-            component.
-        ds_sample: DataFrame
+        damage_state_sample: DataFrame
             A DataFrame that assigns a damage state to each component
             block in the asset model.
         dropzero: bool, optional, default: True
             If True, the quantity of non-damaged components is not
             saved.
 
         Returns
         -------
-        res_df: DataFrame
+        DataFrame
             A DataFrame that combines the component quantity and
             damage state information.
 
         """
 
+        # pylint: disable=missing-return-doc
         if self._asmnt.log.verbose:
             self.log_msg('Calculating damage quantities...', prepend_timestamp=True)
 
         # Retrieve the component quantity information and component
         # marginal parameters from the asset model
 
         # ('cmp', 'loc', 'dir', 'uid') -> component quantity series
@@ -979,51 +1070,50 @@
         ):
             # if this information is available, use it
 
             # ('cmp', 'loc', 'dir', 'uid) -> number of blocks
             num_blocks = component_marginal_parameters['Blocks'].to_dict()
 
             def get_num_blocks(key):
+                # pylint: disable=missing-return-type-doc
                 return float(num_blocks[key])
 
         else:
             # otherwise assume 1 block regardless of
             # ('cmp', 'loc', 'dir', 'uid) key
-            def get_num_blocks(key):
+            def get_num_blocks(_):
+                # pylint: disable=missing-return-type-doc
                 return 1.00
 
         # ('cmp', 'loc', 'dir', 'uid', 'block') -> damage state series
-        ds_sample_dict = ds_sample.to_dict('series')
+        damage_state_sample_dict = damage_state_sample.to_dict('series')
 
         dmg_qnt_series_collection = {}
-        for key, ds_series in ds_sample_dict.items():
+        for key, damage_state_series in damage_state_sample_dict.items():
             component, location, direction, uid, block = key
-            ds_set = set(ds_series.values)
-            for ds in ds_set:
+            damage_state_set = set(damage_state_series.values)
+            for ds in damage_state_set:
                 if ds == -1:
                     continue
                 if dropzero and ds == 0:
                     continue
-                else:
+                dmg_qnt_vals = np.where(
+                    damage_state_series.values == ds,
+                    component_quantities[component, location, direction, uid].values
+                    / get_num_blocks((component, location, direction, uid)),
+                    0.00,
+                )
+                if -1 in damage_state_set:
                     dmg_qnt_vals = np.where(
-                        ds_series.values == ds,
-                        component_quantities[
-                            component, location, direction, uid
-                        ].values
-                        / get_num_blocks((component, location, direction, uid)),
-                        0.00,
+                        damage_state_series.values != -1, dmg_qnt_vals, np.nan
                     )
-                    if -1 in ds_set:
-                        dmg_qnt_vals = np.where(
-                            ds_series.values != -1, dmg_qnt_vals, np.nan
-                        )
-                    dmg_qnt_series = pd.Series(dmg_qnt_vals)
-                    dmg_qnt_series_collection[
-                        (component, location, direction, uid, block, str(ds))
-                    ] = dmg_qnt_series
+                dmg_qnt_series = pd.Series(dmg_qnt_vals)
+                dmg_qnt_series_collection[
+                    (component, location, direction, uid, block, str(ds))
+                ] = dmg_qnt_series
 
         damage_quantities = pd.concat(
             dmg_qnt_series_collection.values(),
             axis=1,
             keys=dmg_qnt_series_collection.keys(),
         )
         damage_quantities.columns.names = ['cmp', 'loc', 'dir', 'uid', 'block', 'ds']
@@ -1069,14 +1159,19 @@
                 ['1_CMP.A-LOC', {'DS1': 'CMP.B_DS1'}]
         ds_sample : pandas DataFrame
             A DataFrame representing the damage state of the
             components. It is modified in place to represent the
             damage states of the components after the task has been
             performed.
 
+        Raises
+        ------
+        ValueError
+            Raises an error if the source or target event descriptions
+            do not follow expected formats.
         """
 
         if self._asmnt.log.verbose:
             self.log_msg(f'Applying task {task}...', prepend_timestamp=True)
 
         # parse task
         source_cmp = task[0].split('_')[1]  # source component
@@ -1100,15 +1195,14 @@
                 "skipped.",
                 prepend_timestamp=False,
             )
             return
 
         # execute the events pres prescribed in the damage task
         for source_event, target_infos in events.items():
-
             # events can only be triggered by damage state occurrence
             if not source_event.startswith('DS'):
                 raise ValueError(
                     f"Unable to parse source event in damage "
                     f"process: {source_event}"
                 )
             # get the ID of the damage state that triggers the event
@@ -1116,15 +1210,14 @@
 
             # turn the target_infos into a list if it is a single
             # argument, for consistency
             if not isinstance(target_infos, list):
                 target_infos = [target_infos]
 
             for target_info in target_infos:
-
                 # get the target component and event type
                 target_cmp, target_event = target_info.split('_')
 
                 if (target_cmp != 'ALL') and (
                     target_cmp not in ds_sample.columns.get_level_values('cmp')
                 ):
                     self.log_msg(
@@ -1134,15 +1227,14 @@
                         "skipped.",
                         prepend_timestamp=False,
                     )
                     continue
 
                 # trigger a damage state
                 if target_event.startswith('DS'):
-
                     # get the ID of the damage state to switch the target
                     # components to
                     ds_target = int(target_event[2:])
 
                 # clear damage state information
                 elif target_event == 'NA':
                     ds_target = -1
@@ -1231,15 +1323,16 @@
                         ds_sample.columns.get_level_values('loc') == loc,
                     )
                 )[0]
             ds_sample.iloc[row_selection, column_selection] = ds_target
 
     def _get_pg_batches(self, block_batch_size):
         """
-        Group performance groups into batches for efficient damage assessment.
+        Group performance groups into batches for efficient damage
+        assessment.
 
         The method takes as input the block_batch_size, which
         specifies the maximum number of blocks per batch. The method
         first checks if performance groups have been defined in the
         cmp_marginal_params dataframe, and if so, it uses the 'Blocks'
         column as the performance group information. If performance
         groups have not been defined in cmp_marginal_params, the
@@ -1255,14 +1348,31 @@
         group. The method then divides the performance groups into
         batches of size specified by block_batch_size and assigns a
         batch number to each group. Finally, the method groups the
         performance groups by batch number, component, location, and
         direction, and returns a dataframe that shows the number of
         blocks for each batch.
 
+        Returns
+        -------
+        DataFrame
+            A DataFrame indexed by batch number, component identifier,
+            location, direction, and unique ID, with a column
+            indicating the number of blocks assigned to each
+            batch. This dataframe facilitates the management and
+            execution of damage assessment tasks by grouping
+            components into manageable batches based on the specified
+            block batch size.
+
+        Raises
+        ------
+        Warning
+            Logs a warning if any performance groups do not have
+            corresponding damage model information and are therefore
+            excluded from the analysis.
         """
 
         # Get the marginal parameters for the components from the
         # asset model
         cmp_marginals = self._asmnt.asset.cmp_marginal_params
 
         # Initialize the batch dataframe
@@ -1398,17 +1508,15 @@
 
         """
         # get a shortcut for the damage model parameters
         DP = self.damage_params
 
         # Get the header for the results that we can use to identify
         # cmp-loc-dir-uid sets
-        dmg_header = (
-            dmg_sample.groupby(level=[0, 1, 2, 3], axis=1).first().iloc[:2, :]
-        )
+        dmg_header = dmg_sample.groupby(level=[0, 1, 2, 3], axis=1).first().iloc[:2, :]
 
         # get the number of possible limit states
         ls_list = [col for col in DP.columns.unique(level=0) if 'LS' in col]
 
         # initialize the result dataframe
         res = pd.DataFrame()
 
@@ -1426,17 +1534,15 @@
                 if not pd.isna(cmp_data[(ls, 'Theta_0')]):
                     # check if there is only one damage state
                     if pd.isna(cmp_data[(ls, 'DamageStateWeights')]):
                         ds_count += 1
 
                     else:
                         # or if there are more than one, how many
-                        ds_count += len(
-                            cmp_data[(ls, 'DamageStateWeights')].split('|')
-                        )
+                        ds_count += len(cmp_data[(ls, 'DamageStateWeights')].split('|'))
 
             # get the list of valid cmp-loc-dir-uid sets
             cmp_header = dmg_header.loc[
                 :,
                 [
                     cmp_id,
                 ],
@@ -1465,26 +1571,46 @@
 
         # replace zeros wherever the dmg_sample has results
         res.loc[:, dmg_sample.columns.to_list()] = dmg_sample
 
         return res
 
     def calculate(
-        self, dmg_process=None, block_batch_size=1000, scaling_specification=None
+        self,
+        sample_size=None,
+        dmg_process=None,
+        block_batch_size=1000,
+        scaling_specification=None,
+    ):
+        """
+        Wrapper around the new calculate method that requires sample size.
+        Exists for backwards compatibility
+        """
+        if not sample_size:
+            # todo: Deprecation warning
+            sample_size = self._asmnt.demand.sample.shape[0]
+        self.calculate_internal(
+            sample_size, dmg_process, block_batch_size, scaling_specification
+        )
+
+    def calculate_internal(
+        self,
+        sample_size,
+        dmg_process=None,
+        block_batch_size=1000,
+        scaling_specification=None,
     ):
         """
         Calculate the damage state of each component block in the asset.
 
         """
 
         self.log_div()
         self.log_msg('Calculating damages...')
 
-        sample_size = self._asmnt.demand.sample.shape[0]
-
         # Break up damage calculation and perform it by performance group.
         # Compared to the simultaneous calculation of all PGs, this approach
         # reduces demands on memory and increases the load on CPU. This leads
         # to a more balanced workload on most machines for typical problems.
         # It also allows for a straightforward extension with parallel
         # computing.
 
@@ -1508,32 +1634,31 @@
             "for damage assessment",
             prepend_timestamp=False,
         )
 
         # for PG_i in self._asmnt.asset.cmp_sample.columns:
         ds_samples = []
         for PGB_i in batches:
-
-            component_blocks = pg_batch.loc[PGB_i]
+            performance_group = pg_batch.loc[PGB_i]
 
             self.log_msg(
                 f"Calculating damage for PG batch {PGB_i} with "
-                f"{int(component_blocks['Blocks'].sum())} blocks"
+                f"{int(performance_group['Blocks'].sum())} blocks"
             )
 
             # Generate an array with component capacities for each block and
             # generate a second array that assigns a specific damage state to
             # each component limit state. The latter is primarily needed to
             # handle limit states with multiple, mutually exclusive DS options
             capacity_sample, lsds_sample = self._generate_dmg_sample(
-                sample_size, component_blocks, scaling_specification
+                sample_size, performance_group, scaling_specification
             )
 
             # Get the required demand types for the analysis
-            EDP_req = self._get_required_demand_type(component_blocks)
+            EDP_req = self._get_required_demand_type(performance_group)
 
             # Create the demand vector
             demand_dict = self._assemble_required_demand_data(EDP_req)
 
             # Evaluate the Damage State of each Component Block
             ds_sample = self._evaluate_damage_state(
                 demand_dict, EDP_req, capacity_sample, lsds_sample
@@ -1555,17 +1680,15 @@
             for task in dmg_process.items():
                 self._perform_dmg_task(task, ds_sample)
 
             self.log_msg(
                 "Damage processes successfully applied.", prepend_timestamp=False
             )
 
-        qnt_sample = self._prepare_dmg_quantities(
-            pg_batch.reset_index('Batch', drop=True), ds_sample, dropzero=False
-        )
+        qnt_sample = self._prepare_dmg_quantities(ds_sample, dropzero=False)
 
         # If requested, extend the quantity table with all possible DSs
         if self._asmnt.options.list_all_ds:
             qnt_sample = self._complete_ds_cols(qnt_sample)
 
         self.sample = qnt_sample
```

### Comparing `pelicun-3.3.2/pelicun/model/demand_model.py` & `pelicun-3.3.3/pelicun/model/demand_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,14 +105,29 @@
         self._RVs = None
         self.sample = None
 
     def save_sample(self, filepath=None, save_units=False):
         """
         Save demand sample to a csv file or return it in a DataFrame
 
+        Returns
+        -------
+        None or tuple
+            If `filepath` is specified, the function saves the demand
+            sample to a CSV file and returns None.
+            If `filepath` is not specified, it returns the DataFrame
+            containing the demand sample.
+            If `save_units` is True, it returns a tuple of the
+            DataFrame and a Series containing the units.
+
+        Raises
+        ------
+        IOError
+            Raises an IOError if there is an issue saving the file to
+            the specified `filepath`.
         """
 
         self.log_div()
         if filepath is not None:
             self.log_msg('Saving demand sample...')
 
         res = file_io.save_to_csv(
@@ -121,17 +136,15 @@
             units=self.units,
             unit_conversion_factors=self._asmnt.unit_conversion_factors,
             use_simpleindex=(filepath is not None),
             log=self._asmnt.log,
         )
 
         if filepath is not None:
-            self.log_msg(
-                'Demand sample successfully saved.', prepend_timestamp=False
-            )
+            self.log_msg('Demand sample successfully saved.', prepend_timestamp=False)
             return None
 
         # else:
         units = res.loc["Units"]
         res.drop("Units", inplace=True)
 
         if save_units:
@@ -152,14 +165,43 @@
         ----------
         filepath: string or DataFrame
             Location of the file with the demand sample.
 
         """
 
         def parse_header(raw_header):
+            """
+            Parses and cleans the header of a demand DataFrame from
+            raw multi-level index to a standardized format.
+
+            This function adjusts the raw header of a DataFrame,
+            removing optional event IDs and whitespace, and
+            standardizing the format to facilitate further
+            processing. It is designed to handle headers with either
+            three or four levels, where the first level (event_ID) is
+            optional and not used in further analysis.  Note: This
+            will soon change, and that first level will be enforced
+            instead of removed.
+
+            Parameters
+            ----------
+            raw_header : pd.MultiIndex
+                The original multi-level index (header) of the
+                DataFrame, which may contain an optional event_ID and
+                might have excess whitespace in the labels.
+
+            Returns
+            -------
+            pd.MultiIndex
+                A new MultiIndex for the DataFrame's columns that is
+                cleaned of any unwanted characters or levels. This
+                index has three levels: 'type', 'loc', and 'dir',
+                representing the type of demand, location, and
+                direction, respectively.
+            """
             old_MI = raw_header
 
             # The first number (event_ID) in the demand labels is optional and
             # currently not used. We remove it if it was in the raw data.
             if old_MI.nlevels == 4:
                 if self._asmnt.log.verbose:
                     self.log_msg(
@@ -236,26 +278,62 @@
 
         self.units = units
 
         self.log_msg('Demand units successfully parsed.', prepend_timestamp=False)
 
     def estimate_RID(self, demands, params, method='FEMA P58'):
         """
-        Estimate residual drift realizations based on other demands
+        Estimates residual inter-story drift (RID) realizations based
+        on peak inter-story drift (PID) and other demand parameters
+        using specified methods.
+
+        This method calculates RID based on the peak inter-story drift
+        provided in the demands DataFrame and parameters such as yield
+        drift specified in the params dictionary. The calculation
+        adheres to the FEMA P-58 methodology, which includes
+        conditions for different ranges of drift.
 
         Parameters
         ----------
-        demands: DataFrame
-            Sample of demands required for the method to estimate the RID values
-        params: dict
-            Parameters required for the method to estimate the RID values
-        method: {'FEMA P58'}, default: 'FEMA P58'
-            Method to use for the estimation - currently, only one is available.
-        """
+        demands : DataFrame
+            A DataFrame containing samples of demands, specifically
+            peak inter-story drift (PID) values for various
+            location-direction pairs required for the estimation
+            method.
+        params : dict
+            A dictionary containing parameters required for the
+            estimation method, such as 'yield_drift', which is the
+            drift at which yielding is expected to occur.
+        method : str, optional
+            The method used to estimate the RID values. Currently,
+            only 'FEMA P58' is implemented. Defaults to 'FEMA P58'.
+
+        Returns
+        -------
+        DataFrame
+            A DataFrame containing the estimated residual inter-story
+            drift (RID) realizations, indexed and structured similarly
+            to the input demands DataFrame.
 
+        Raises
+        ------
+        ValueError
+            Raises a ValueError if an unrecognized method is provided
+            or required parameters are missing in the `params`
+            dictionary.
+
+        Notes
+        -----
+        The FEMA P-58 estimation approach divides the drift into three
+        domains, with different transformation rules for
+        each. Additional stochastic variation is introduced to nonzero
+        RID values to model the inherent uncertainty. The method
+        ensures that the RID values do not exceed the corresponding
+        PID values.
+        """
         if method == 'FEMA P58':
             # method is described in FEMA P-58 Volume 1 Section 5.4 & Appendix C
 
             # the provided demands shall be PID values at various loc-dir pairs
             PID = demands
 
             # there's only one parameter needed: the yield drift
@@ -318,18 +396,18 @@
 
         if self.calibrated:
             self.log_msg(
                 'WARNING: DemandModel has been previously calibrated.',
                 prepend_timestamp=False,
             )
 
-            raise ValueError()
-
         def parse_settings(settings, demand_type):
             def parse_str_to_float(in_str, context_string):
+                # pylint: disable = missing-return-type-doc
+                # pylint: disable = missing-return-doc
                 try:
                     out_float = float(in_str)
 
                 except ValueError:
                     self.log_msg(
                         f"WARNING: Could not parse {in_str} provided as "
                         f"{context_string}. Using NaN instead.",
@@ -389,14 +467,16 @@
                 # scale the sig value if the target distribution family is normal
                 if settings['DistributionFamily'] == 'normal':
                     sig_increase *= scale_factor
 
                 cal_df.loc[idx[cols, :, :], 'SigIncrease'] = sig_increase
 
         def get_filter_mask(lower_lims, upper_lims):
+            # pylint: disable=missing-return-doc
+            # pylint: disable=missing-return-type-doc
             demands_of_interest = demand_sample.iloc[:, pd.notna(upper_lims)]
             limits_of_interest = upper_lims[pd.notna(upper_lims)]
             upper_mask = np.all(demands_of_interest < limits_of_interest, axis=1)
 
             demands_of_interest = demand_sample.iloc[:, pd.notna(lower_lims)]
             limits_of_interest = lower_lims[pd.notna(lower_lims)]
             lower_mask = np.all(demands_of_interest > limits_of_interest, axis=1)
@@ -521,17 +601,15 @@
         )
 
         demand_theta, demand_rho = uq.fit_distribution_to_sample(
             raw_samples=demand_sample.values.T,
             distribution=cal_df.loc[:, 'Family'].values,
             censored_count=censored_count,
             detection_limits=cal_df.loc[:, ['CensorLower', 'CensorUpper']].values,
-            truncation_limits=cal_df.loc[
-                :, ['TruncateLower', 'TruncateUpper']
-            ].values,
+            truncation_limits=cal_df.loc[:, ['TruncateLower', 'TruncateUpper']].values,
             multi_fit=False,
             logger_object=self._asmnt.log,
         )
         # fit the joint distribution
         self.log_msg(
             "\nCalibration successful, processing results...",
             prepend_timestamp=False,
@@ -557,27 +635,25 @@
         model_params = model_params[
             ['Family', 'Theta_0', 'Theta_1', 'TruncateLower', 'TruncateUpper']
         ]
 
         self.marginal_params = model_params
 
         self.log_msg(
-            "\nCalibrated demand model marginal distributions:\n"
-            + str(model_params),
+            "\nCalibrated demand model marginal distributions:\n" + str(model_params),
             prepend_timestamp=False,
         )
 
         # save the correlation matrix
         self.correlation = pd.DataFrame(
             demand_rho, columns=cal_df.index, index=cal_df.index
         )
 
         self.log_msg(
-            "\nCalibrated demand model correlation matrix:\n"
-            + str(self.correlation),
+            "\nCalibrated demand model correlation matrix:\n" + str(self.correlation),
             prepend_timestamp=False,
         )
 
         self.calibrated = True
 
     def save_model(self, file_prefix):
         """
@@ -812,14 +888,16 @@
         for new_columns in new_columns_list:
             flat_list.extend(new_columns)
         if len(set(flat_list)) != len(flat_list):
             raise ValueError('Duplicate entries in demand cloning configuration.')
 
         # turn the config entries to tuples
         def turn_to_tuples(demand_cloning):
+            # pylint: disable=missing-return-doc
+            # pylint: disable=missing-return-type-doc
             demand_cloning_tuples = {}
             for key, values in demand_cloning.items():
                 demand_cloning_tuples[tuple(key.split('-'))] = [
                     tuple(x.split('-')) for x in values
                 ]
             return demand_cloning_tuples
 
@@ -857,18 +935,68 @@
                 new_column_values = demand_cloning[column]
                 column_index.extend([i] * len(new_column_values))
                 column_values.extend(new_column_values)
         # copy the columns
         self.sample = self.sample.iloc[:, column_index]
         # update the column index
         self.sample.columns = pd.MultiIndex.from_tuples(column_values)
+        # update units
+        self.units = self.units.iloc[column_index]
+        self.units.index = self.sample.columns
 
     def generate_sample(self, config):
         """
-        Generates an RV sample with the specified configuration.
+        Generates a sample of random variables (RVs) based on the
+        specified configuration for demand modeling.
+
+        This method utilizes the current settings for marginal
+        distribution parameters to generate a sample of demand
+        variables. The configuration can specify details such as the
+        sample size, whether to preserve the order of raw data, and
+        whether to apply demand cloning. The generated sample is
+        stored internally and can be used for subsequent analysis.
+
+        Parameters
+        ----------
+        config : dict
+            A dictionary containing configuration options for the
+            sample generation. Key options include:
+            - 'SampleSize': The number of samples to generate.
+            - 'PreserveRawOrder': Boolean indicating whether to
+              preserve the order of the raw data. Defaults to False.
+            - 'DemandCloning': Specifies if and how demand cloning
+              should be applied. Can be a boolean or a detailed
+              configuration.
+
+        Raises
+        ------
+        ValueError
+            If model parameters are not loaded or specified before
+            attempting to generate a sample.
+
+        Notes
+        -----
+        The function is responsible for the creation of random
+        variables based on the distribution parameters specified in
+        `marginal_params`.  It ensures that the sample is properly
+        indexed and sorted according to type, location, and
+        direction. It also handles the configuration of demand cloning
+        if specified, which is a method to artificially augment the
+        variability in the sample based on existing realizations.
+
+        Examples
+        --------
+        >>> config = {
+                'SampleSize': 1000,
+                'PreserveRawOrder': True,
+                'DemandCloning': False
+            }
+        >>> model.generate_sample(config)
+        # This will generate 1000 realizations of demand variables
+        # with the specified configuration.
         """
 
         if self.marginal_params is None:
             raise ValueError(
                 'Model parameters have not been specified. Either'
                 'load parameters from a file or calibrate the '
                 'model using raw demand data.'
```

### Comparing `pelicun-3.3.2/pelicun/model/loss_model.py` & `pelicun-3.3.3/pelicun/model/loss_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     prep_bounded_multilinear_median_DV
 
     LossModel
     RepairModel
 
 """
 
+import warnings
 import numpy as np
 import pandas as pd
 from .pelicun_model import PelicunModel
 from .. import base
 from .. import uq
 from .. import file_io
 
@@ -74,30 +75,58 @@
     ----------
 
     """
 
     def __init__(self, assessment):
         super().__init__(assessment)
 
-        self._sample = None
+        self.sample = None
         self.loss_map = None
         self.loss_params = None
         self.loss_type = 'Generic'
 
-    @property
-    def sample(self):
-        """
-        sample property
-        """
-        return self._sample
-
     def save_sample(self, filepath=None, save_units=False):
         """
-        Save loss sample to a csv file
+        Saves the loss sample to a CSV file or returns it as a
+        DataFrame with optional units.
+
+        This method handles the storage of a sample of loss estimates,
+        which can either be saved directly to a file or returned as a
+        DataFrame for further manipulation. When saving to a file,
+        additional information such as unit conversion factors and
+        column units can be included. If the data is not being saved
+        to a file, the method can return the DataFrame with or without
+        units as specified.
 
+        Parameters
+        ----------
+        filepath : str, optional
+            The path to the file where the loss sample should be
+            saved. If not provided, the sample is not saved to disk
+            but returned.
+        save_units : bool, default: False
+            Indicates whether to include a row with unit information
+            in the returned DataFrame. This parameter is ignored if a
+            file path is provided.
+
+        Returns
+        -------
+        None or tuple
+            If `filepath` is provided, the function returns None after
+            saving the data.
+            If no `filepath` is specified, returns:
+            - DataFrame containing the loss sample.
+            - Optionally, a Series containing the units for each
+              column if `save_units` is True.
+
+        Raises
+        ------
+        IOError
+            Raises an IOError if there is an issue saving the file to
+            the specified `filepath`.
         """
         self.log_div()
         if filepath is not None:
             self.log_msg('Saving loss sample...')
 
         cmp_units = self.loss_params[('DV', 'Unit')]
         dv_units = pd.Series(index=self.sample.columns, name='Units', dtype='object')
@@ -135,15 +164,15 @@
         """
         Load damage sample data.
 
         """
         self.log_div()
         self.log_msg('Loading loss sample...')
 
-        self._sample = file_io.load_data(
+        self.sample = file_io.load_data(
             filepath, self._asmnt.unit_conversion_factors, log=self._asmnt.log
         )
 
         self.log_msg('Loss sample successfully loaded.', prepend_timestamp=False)
 
     def load_model(self, data_paths, mapping_path, decision_variables=None):
         """
@@ -299,33 +328,32 @@
 
         The method of sampling decision variables in Decision
         Variable-specific and needs to be implemented in every child
         of the LossModel independently.
         """
         raise NotImplementedError
 
-    def calculate(self):
+    def calculate(self, sample_size=None):
         """
         Calculate the consequences of each component block damage in
         the asset.
 
         """
+        if not sample_size:
+            sample_size = self._asmnt.demand.sample.shape[0]
+            warnings.warn(
+                'Using default sample size is deprecated and will '
+                'be removed in future versions. '
+                'Please provide the `sample_size` explicitly.',
+                DeprecationWarning,
+            )
 
         self.log_div()
         self.log_msg("Calculating losses...")
 
-        drivers = [d for d, _ in self.loss_map['Driver']]
-
-        if 'DMG' in drivers:
-            sample_size = self._asmnt.damage.sample.shape[0]
-        elif 'DEM' in drivers:
-            sample_size = self._asmnt.demand.sample.shape[0]
-        else:
-            raise ValueError('Invalid loss drivers. Check the specified loss map.')
-
         # First, get the damaged quantities in each damage state for
         # each component of interest.
         dmg_q = self._asmnt.damage.sample.copy()
 
         # Now sample random Decision Variables
         # Note that this method is DV-specific and needs to be
         # implemented in every child of the LossModel independently.
@@ -344,36 +372,39 @@
     """
 
     def __init__(self, assessment):
         super().__init__(assessment)
 
         self.loss_type = 'Repair'
 
-    # def load_model(self, data_paths, mapping_path):
-
-    #     super().load_model(data_paths, mapping_path)
-
-    # def calculate(self):
-
-    #     super().calculate()
-
     def _create_DV_RVs(self, case_list):
         """
-        Prepare the random variables used for repair cost and time simulation.
+        Prepare the random variables associated with decision
+        variables, such as repair cost and time.
 
         Parameters
         ----------
         case_list: MultiIndex
-            Index with cmp-loc-dir-ds descriptions that identify the RVs
-            we need for the simulation.
+            Index with cmp-loc-dir-ds descriptions that identify the
+            RVs we need for the simulation.
+
+        Returns
+        -------
+        RandomVariableRegistry or None
+            A RandomVariableRegistry containing all the generated
+            random variables necessary for the simulation. If no
+            random variables are generated (due to missing parameters
+            or conditions), returns None.
 
         Raises
         ------
         ValueError
-            When any Loss Driver is not recognized.
+            If an unrecognized loss driver type is encountered,
+            indicating a configuration or data input error.
+
         """
 
         RV_reg = uq.RandomVariableRegistry(self._asmnt.options.rng)
         LP = self.loss_params
 
         # make ds the second level in the MultiIndex
         case_DF = pd.DataFrame(
@@ -392,17 +423,15 @@
             # load the corresponding parameters
             driver_type, driver_cmp_id = self.loss_map.loc[loss_cmp_id, 'Driver']
             conseq_cmp_id = self.loss_map.loc[loss_cmp_id, 'Consequence']
 
             # currently, we only support DMG-based loss calculations
             # but this will be extended in the very near future
             if driver_type != 'DMG':
-                raise ValueError(
-                    f"Loss Driver type not recognized: " f"{driver_type}"
-                )
+                raise ValueError(f"Loss Driver type not recognized: " f"{driver_type}")
 
             # load the parameters
             # TODO: remove specific DV_type references and make the code below
             # generate parameters for any DV_types provided
             if (conseq_cmp_id, 'Cost') in LP.index:
                 cost_params = LP.loc[(conseq_cmp_id, 'Cost'), :]
             else:
@@ -431,16 +460,15 @@
                     continue
 
                 if cost_params is not None:
                     cost_params_DS = cost_params[f'DS{ds}']
 
                     cost_family = cost_params_DS.get('Family', np.nan)
                     cost_theta = [
-                        cost_params_DS.get(f"Theta_{t_i}", np.nan)
-                        for t_i in range(3)
+                        cost_params_DS.get(f"Theta_{t_i}", np.nan) for t_i in range(3)
                     ]
 
                     # If the first parameter is controlled by a function, we use
                     # 1.0 in its place and will scale the results in a later
                     # step
                     if '|' in str(cost_theta[0]):
                         # if isinstance(cost_theta[0], str):
@@ -450,16 +478,15 @@
                     cost_family = np.nan
 
                 if time_params is not None:
                     time_params_DS = time_params[f'DS{ds}']
 
                     time_family = time_params_DS.get('Family', np.nan)
                     time_theta = [
-                        time_params_DS.get(f"Theta_{t_i}", np.nan)
-                        for t_i in range(3)
+                        time_params_DS.get(f"Theta_{t_i}", np.nan) for t_i in range(3)
                     ]
 
                     # If the first parameter is controlled by a function, we use
                     # 1.0 in its place and will scale the results in a later
                     # step
                     if '|' in str(time_theta[0]):
                         # if isinstance(time_theta[0], str):
@@ -469,16 +496,15 @@
                     time_family = np.nan
 
                 if carbon_params is not None:
                     carbon_params_DS = carbon_params[f'DS{ds}']
 
                     carbon_family = carbon_params_DS.get('Family', np.nan)
                     carbon_theta = [
-                        carbon_params_DS.get(f"Theta_{t_i}", np.nan)
-                        for t_i in range(3)
+                        carbon_params_DS.get(f"Theta_{t_i}", np.nan) for t_i in range(3)
                     ]
 
                     # If the first parameter is controlled by a function, we use
                     # 1.0 in its place and will scale the results in a later
                     # step
                     if '|' in str(carbon_theta[0]):
                         # if isinstance(carbon_theta[0], str):
@@ -488,16 +514,15 @@
                     carbon_family = np.nan
 
                 if energy_params is not None:
                     energy_params_DS = energy_params[f'DS{ds}']
 
                     energy_family = energy_params_DS.get('Family', np.nan)
                     energy_theta = [
-                        energy_params_DS.get(f"Theta_{t_i}", np.nan)
-                        for t_i in range(3)
+                        energy_params_DS.get(f"Theta_{t_i}", np.nan) for t_i in range(3)
                     ]
 
                     # If the first parameter is controlled by a function, we use
                     # 1.0 in its place and will scale the results in a later
                     # step
                     if '|' in str(energy_theta[0]):
                         # if isinstance(energy_theta[0], str):
@@ -518,32 +543,28 @@
 
                 # Otherwise, load the loc-dir cases
                 loc_dir_uid = case_DF.loc[(driver_cmp_id, ds)].index.values
 
                 for loc, direction, uid in loc_dir_uid:
                     # assign cost RV
                     if pd.isna(cost_family) is False:
-                        cost_rv_tag = (
-                            f'Cost-{loss_cmp_id}-{ds}-{loc}-{direction}-{uid}'
-                        )
+                        cost_rv_tag = f'Cost-{loss_cmp_id}-{ds}-{loc}-{direction}-{uid}'
 
                         RV_reg.add_RV(
                             uq.rv_class_map(cost_family)(
                                 name=cost_rv_tag,
                                 theta=cost_theta,
                                 truncation_limits=[0.0, np.nan],
                             )
                         )
                         rv_count += 1
 
                     # assign time RV
                     if pd.isna(time_family) is False:
-                        time_rv_tag = (
-                            f'Time-{loss_cmp_id}-{ds}-{loc}-{direction}-{uid}'
-                        )
+                        time_rv_tag = f'Time-{loss_cmp_id}-{ds}-{loc}-{direction}-{uid}'
 
                         RV_reg.add_RV(
                             uq.rv_class_map(time_family)(
                                 name=time_rv_tag,
                                 theta=time_theta,
                                 truncation_limits=[0.0, np.nan],
                             )
@@ -589,34 +610,63 @@
                         and (self._asmnt.options.rho_cost_time != 0.0)
                     ):
                         rho = self._asmnt.options.rho_cost_time
 
                         RV_reg.add_RV_set(
                             uq.RandomVariableSet(
                                 f'DV-{loss_cmp_id}-{ds}-{loc}-{direction}-{uid}_set',
-                                list(
-                                    RV_reg.RVs([cost_rv_tag, time_rv_tag]).values()
-                                ),
+                                list(RV_reg.RVs([cost_rv_tag, time_rv_tag]).values()),
                                 np.array([[1.0, rho], [rho, 1.0]]),
                             )
                         )
 
-        self.log_msg(
-            f"\n{rv_count} random variables created.", prepend_timestamp=False
-        )
+        self.log_msg(f"\n{rv_count} random variables created.", prepend_timestamp=False)
 
         if rv_count > 0:
             return RV_reg
         # else:
         return None
 
     def _calc_median_consequence(self, eco_qnt):
         """
-        Calculate the median repair consequence for each loss component.
+        Calculates the median repair consequences for each loss
+        component based on their quantities and the associated loss
+        parameters.
+
+        This function evaluates the median consequences for different
+        types of decision variables (DV), such as repair costs or
+        repair time, based on the provided loss parameters. It
+        utilizes the eco_qnt DataFrame, which contains economic
+        quantity realizations for various damage states and
+        components, to compute the consequences.
+
+        Parameters
+        ----------
+        eco_qnt : DataFrame
+            A DataFrame containing economic quantity realizations for
+            various components and damage states, indexed or
+            structured to align with the loss parameters.
+
+        Returns
+        -------
+        dict
+            A dictionary where keys are the types of decision variables
+            (DV) like 'COST' or 'TIME', and values are DataFrames
+            containing the median consequences for each component and
+            damage state. These DataFrames are structured with
+            MultiIndex columns that may include 'cmp' (component),
+            'ds' (damage state), and potentially 'loc' (location),
+            depending on assessment options.
 
+        Raises
+        ------
+        ValueError
+            If any loss driver types or distribution types are not
+            recognized, or if the parameters are incomplete or
+            unsupported.
         """
 
         medians = {}
 
         DV_types = self.loss_params.index.unique(level=1)
 
         # for DV_type, DV_type_scase in zip(['COST', 'TIME'], ['Cost', 'Time']):
@@ -649,17 +699,15 @@
                         continue
 
                     ds_id = ds[2:]
 
                     if ds_id == '0':
                         continue
 
-                    loss_params_DS = self.loss_params.loc[
-                        (loss_cmp_name, DV_type), ds
-                    ]
+                    loss_params_DS = self.loss_params.loc[(loss_cmp_name, DV_type), ds]
 
                     # check if theta_0 is defined
                     theta_0 = loss_params_DS.get('Theta_0', np.nan)
 
                     if pd.isna(theta_0):
                         continue
 
@@ -742,118 +790,14 @@
                     result.columns.names = ['cmp', 'ds', 'loc']
 
                 # save the results to the returned dictionary
                 medians.update({DV_type: result})
 
         return medians
 
-    def aggregate_losses(self):
-        """
-        Aggregates repair consequences across components.
-
-        Repair costs are simply summed up for each realization while repair
-        times are aggregated to provide lower and upper limits of the total
-        repair time using the assumption of parallel and sequential repair of
-        floors, respectively. Repairs within each floor are assumed to occur
-        sequentially.
-        """
-
-        self.log_div()
-        self.log_msg("Aggregating repair consequences...")
-
-        DV = self.sample
-
-        if DV is None:
-            return
-
-        # group results by DV type and location
-        DVG = DV.groupby(level=[0, 4], axis=1).sum()
-
-        # create the summary DF
-        df_agg = pd.DataFrame(
-            index=DV.index,
-            columns=[
-                'repair_cost',
-                'repair_time-parallel',
-                'repair_time-sequential',
-                'repair_carbon',
-                'repair_energy',
-            ],
-        )
-
-        if 'Cost' in DVG.columns:
-            df_agg['repair_cost'] = DVG['Cost'].sum(axis=1)
-        else:
-            df_agg = df_agg.drop('repair_cost', axis=1)
-
-        if 'Time' in DVG.columns:
-            df_agg['repair_time-sequential'] = DVG['Time'].sum(axis=1)
-
-            df_agg['repair_time-parallel'] = DVG['Time'].max(axis=1)
-        else:
-            df_agg = df_agg.drop(
-                ['repair_time-parallel', 'repair_time-sequential'], axis=1
-            )
-
-        if 'Carbon' in DVG.columns:
-            df_agg['repair_carbon'] = DVG['Carbon'].sum(axis=1)
-        else:
-            df_agg = df_agg.drop('repair_carbon', axis=1)
-
-        if 'Energy' in DVG.columns:
-            df_agg['repair_energy'] = DVG['Energy'].sum(axis=1)
-        else:
-            df_agg = df_agg.drop('repair_energy', axis=1)
-
-        # convert units
-
-        cmp_units = (
-            self.loss_params[('DV', 'Unit')]
-            .groupby(
-                level=[
-                    1,
-                ]
-            )
-            .agg(lambda x: x.value_counts().index[0])
-        )
-
-        dv_units = pd.Series(index=df_agg.columns, name='Units', dtype='object')
-
-        if 'Cost' in DVG.columns:
-            dv_units['repair_cost'] = cmp_units['Cost']
-
-        if 'Time' in DVG.columns:
-            dv_units['repair_time-parallel'] = cmp_units['Time']
-            dv_units['repair_time-sequential'] = cmp_units['Time']
-
-        if 'Carbon' in DVG.columns:
-            dv_units['repair_carbon'] = cmp_units['Carbon']
-
-        if 'Energy' in DVG.columns:
-            dv_units['repair_energy'] = cmp_units['Energy']
-
-        df_agg = file_io.save_to_csv(
-            df_agg,
-            None,
-            units=dv_units,
-            unit_conversion_factors=self._asmnt.unit_conversion_factors,
-            use_simpleindex=False,
-            log=self._asmnt.log,
-        )
-
-        df_agg.drop("Units", inplace=True)
-
-        # convert header
-
-        df_agg = base.convert_to_MultiIndex(df_agg, axis=1)
-
-        self.log_msg("Repair consequences successfully aggregated.")
-
-        return df_agg.astype(float)
-
     def _generate_DV_sample(self, dmg_quantities, sample_size):
         """
         Generate a sample of repair costs and times.
 
         Parameters
         ----------
         dmg_quantities: DataFrame
@@ -871,15 +815,15 @@
         """
 
         # calculate the quantities for economies of scale
         self.log_msg("\nAggregating damage quantities...", prepend_timestamp=False)
 
         # If everything is undamaged there are no losses
         if set(dmg_quantities.columns.get_level_values('ds')) == {'0'}:
-            self._sample = None
+            self.sample = None
             self.log_msg(
                 "There is no damage---DV sample is set to None.",
                 prepend_timestamp=False,
             )
             return
 
         if self._asmnt.options.eco_scale["AcrossFloors"]:
@@ -972,17 +916,15 @@
             "deviation from the median consequences.",
             prepend_timestamp=False,
         )
 
         res_list = []
         key_list = []
 
-        dmg_quantities.columns = dmg_quantities.columns.reorder_levels(
-            [0, 4, 1, 2, 3]
-        )
+        dmg_quantities.columns = dmg_quantities.columns.reorder_levels([0, 4, 1, 2, 3])
         dmg_quantities.sort_index(axis=1, inplace=True)
 
         DV_types = self.loss_params.index.unique(level=1)
 
         if isinstance(std_sample, pd.DataFrame):
             std_DV_types = std_sample.columns.unique(level=0)
         else:
@@ -1015,21 +957,19 @@
 
                 ds_list = []
 
                 for ds in medians[DV_type].loc[:, cmp_i].columns.unique(level=0):
                     loc_list = []
 
                     for loc_id, loc in enumerate(
-                        dmg_quantities.loc[:, (dmg_cmp_i, ds)].columns.unique(
-                            level=0
-                        )
+                        dmg_quantities.loc[:, (dmg_cmp_i, ds)].columns.unique(level=0)
                     ):
-                        if (
-                            self._asmnt.options.eco_scale["AcrossFloors"] is True
-                        ) and (loc_id > 0):
+                        if (self._asmnt.options.eco_scale["AcrossFloors"] is True) and (
+                            loc_id > 0
+                        ):
                             break
 
                         if self._asmnt.options.eco_scale["AcrossFloors"] is True:
                             median_i = medians[DV_type].loc[:, (cmp_i, ds)]
                             dmg_i = dmg_quantities.loc[:, (dmg_cmp_i, ds)]
 
                             if cmp_i in prob_cmp_list:
@@ -1101,37 +1041,151 @@
             # get the list of non-zero locations
             locs = DV_sample.columns.get_level_values(4).unique().values
 
             locs = locs[locs != '0']
 
             DV_sample.loc[id_replacement, idx[:, :, :, :, locs]] = 0.0
 
-        self._sample = DV_sample
+        self.sample = DV_sample
 
         self.log_msg("Successfully obtained DV sample.", prepend_timestamp=False)
 
+    def aggregate_losses(self):
+        """
+        Aggregates repair consequences across components.
+
+        Returns
+        -------
+        DataFrame
+            A DataFrame containing aggregated repair
+            consequences. Columns include:
+            - 'repair_cost': Total repair costs across all components.
+            - 'repair_time-parallel': Minimum possible repair time
+              assuming repairs are conducted in parallel.
+            - 'repair_time-sequential': Maximum possible repair time
+              assuming sequential repairs.
+            - 'repair_carbon': Total carbon emissions associated with
+              repairs.
+            - 'repair_energy': Total energy usage associated with
+              repairs.
+            Each of these columns is summed or calculated based on the
+            repair data available.
+        """
+
+        self.log_div()
+        self.log_msg("Aggregating repair consequences...")
+
+        DV = self.sample
+
+        # group results by DV type and location
+        DVG = DV.groupby(level=[0, 4], axis=1).sum()
+
+        # create the summary DF
+        df_agg = pd.DataFrame(
+            index=DV.index,
+            columns=[
+                'repair_cost',
+                'repair_time-parallel',
+                'repair_time-sequential',
+                'repair_carbon',
+                'repair_energy',
+            ],
+        )
+
+        if 'Cost' in DVG.columns:
+            df_agg['repair_cost'] = DVG['Cost'].sum(axis=1)
+        else:
+            df_agg = df_agg.drop('repair_cost', axis=1)
+
+        if 'Time' in DVG.columns:
+            df_agg['repair_time-sequential'] = DVG['Time'].sum(axis=1)
+
+            df_agg['repair_time-parallel'] = DVG['Time'].max(axis=1)
+        else:
+            df_agg = df_agg.drop(
+                ['repair_time-parallel', 'repair_time-sequential'], axis=1
+            )
+
+        if 'Carbon' in DVG.columns:
+            df_agg['repair_carbon'] = DVG['Carbon'].sum(axis=1)
+        else:
+            df_agg = df_agg.drop('repair_carbon', axis=1)
+
+        if 'Energy' in DVG.columns:
+            df_agg['repair_energy'] = DVG['Energy'].sum(axis=1)
+        else:
+            df_agg = df_agg.drop('repair_energy', axis=1)
+
+        # convert units
+
+        cmp_units = (
+            self.loss_params[('DV', 'Unit')]
+            .groupby(
+                level=[
+                    1,
+                ]
+            )
+            .agg(lambda x: x.value_counts().index[0])
+        )
+
+        dv_units = pd.Series(index=df_agg.columns, name='Units', dtype='object')
+
+        if 'Cost' in DVG.columns:
+            dv_units['repair_cost'] = cmp_units['Cost']
+
+        if 'Time' in DVG.columns:
+            dv_units['repair_time-parallel'] = cmp_units['Time']
+            dv_units['repair_time-sequential'] = cmp_units['Time']
+
+        if 'Carbon' in DVG.columns:
+            dv_units['repair_carbon'] = cmp_units['Carbon']
+
+        if 'Energy' in DVG.columns:
+            dv_units['repair_energy'] = cmp_units['Energy']
+
+        df_agg = file_io.save_to_csv(
+            df_agg,
+            None,
+            units=dv_units,
+            unit_conversion_factors=self._asmnt.unit_conversion_factors,
+            use_simpleindex=False,
+            log=self._asmnt.log,
+        )
+
+        df_agg.drop("Units", inplace=True)
+
+        # convert header
+
+        df_agg = base.convert_to_MultiIndex(df_agg, axis=1)
+
+        self.log_msg("Repair consequences successfully aggregated.")
+
+        return df_agg.astype(float)
+
 
 def prep_constant_median_DV(median):
     """
     Returns a constant median Decision Variable (DV) function.
 
     Parameters
     ----------
     median: float
         The median DV for a consequence function with fixed median.
 
     Returns
     -------
-    f: callable
+    callable
         A function that returns the constant median DV for all component
         quantities.
     """
 
     def f(*args):
         # pylint: disable=unused-argument
+        # pylint: disable=missing-return-doc
+        # pylint: disable=missing-return-type-doc
         return median
 
     return f
 
 
 def prep_bounded_multilinear_median_DV(medians, quantities):
     """
@@ -1149,20 +1203,22 @@
     quantities: ndarray
         Series of values that define the component quantities corresponding to
         the series of medians and serving as the x coordinates of the
         multilinear DV function.
 
     Returns
     -------
-    f: callable
+    callable
         A function that returns the median DV given the quantity of damaged
         components.
     """
 
     def f(quantity):
+        # pylint: disable=missing-return-doc
+        # pylint: disable=missing-return-type-doc
         if quantity is None:
             raise ValueError(
                 'A bounded linear median Decision Variable function called '
                 'without specifying the quantity of damaged components'
             )
 
         q_array = np.asarray(quantity, dtype=np.float64)
```

### Comparing `pelicun-3.3.2/pelicun/model/pelicun_model.py` & `pelicun-3.3.3/pelicun/model/pelicun_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
     PelicunModel
 
 """
 
 import numpy as np
 import pandas as pd
-from .. import base
-from .. import uq
+from pelicun import base
+from pelicun import uq
 
 
 idx = base.idx
 
 
 class PelicunModel:
     """
@@ -96,15 +96,15 @@
             and the default value will ensure that the corresponding scaling is
             skipped. This Series provides the units of the reference entities
             for each component. Use '1 EA' if you want to skip such scaling for
             select components but provide arg units for others.
 
         Returns
         -------
-        marginal_params: DataFrame
+        DataFrame
             Same structure as the input DataFrame but with values scaled to
             represent internal Standard International units.
 
         """
         assert np.all(marginal_params.index == units.index)
         if arg_units is not None:
             assert np.all(marginal_params.index == arg_units.index)
@@ -185,17 +185,15 @@
                 # check if there is a need to scale due to argument units
                 if not (arg_units is None):
                     # get the argument unit for the given marginal
                     arg_unit = arg_units.get(row_id)
 
                     if arg_unit != '1 EA':
                         # get the scale factor
-                        arg_unit_factor = self._asmnt.calc_unit_scale_factor(
-                            arg_unit
-                        )
+                        arg_unit_factor = self._asmnt.calc_unit_scale_factor(arg_unit)
 
                         # scale arguments, if needed
                         for a_i, arg in enumerate(args):
                             if isinstance(arg, np.ndarray):
                                 args[a_i] = arg * arg_unit_factor
 
                 # convert the distribution parameters to SI
@@ -210,17 +208,15 @@
                             [
                                 ','.join([f'{val:g}' for val in vals])
                                 for vals in (theta[a_i], args[a_i])
                             ]
                         )
 
                 # and update the values in the DF
-                marginal_params.loc[
-                    row_id, ['Theta_0', 'Theta_1', 'Theta_2']
-                ] = theta
+                marginal_params.loc[row_id, ['Theta_0', 'Theta_1', 'Theta_2']] = theta
 
                 marginal_params.loc[
                     row_id, ['TruncateLower', 'TruncateUpper']
                 ] = tr_limits
 
         # remove the added columns
         marginal_params = marginal_params[original_cols]
```

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv` & `pelicun-3.3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/resources/auto/Hazus_Earthquake_IM.py` & `pelicun-3.3.3/pelicun/resources/auto/Hazus_Earthquake_IM.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,18 +405,16 @@
             "Losses": {
                 "Repair": {
                     "ConsequenceDatabase": "Hazus Earthquake - Buildings",
                     "MapApproach": "Automatic",
                 }
             },
             "Options": {
-                "NonDirectionalMultipliers": {
-                    "ALL": 1.0
-                },
-            }
+                "NonDirectionalMultipliers": {"ALL": 1.0},
+            },
         }
 
     elif assetType == "TransportationNetwork":
         inf_type = GI["assetSubtype"]
 
         if inf_type == "HwyBridge":
             # get the bridge class
@@ -443,18 +441,16 @@
                 "Losses": {
                     "Repair": {
                         "ConsequenceDatabase": "Hazus Earthquake - Transportation",
                         "MapApproach": "Automatic",
                     }
                 },
                 "Options": {
-                    "NonDirectionalMultipliers": {
-                        "ALL": 1.0
-                    },
-                }
+                    "NonDirectionalMultipliers": {"ALL": 1.0},
+                },
             }
 
         elif inf_type == "HwyTunnel":
             # get the tunnel class
             tt = convertTunnelToHAZUSclass(GI)
             GI_ap['TunnelHazusClass'] = tt
 
@@ -478,18 +474,16 @@
                 "Losses": {
                     "Repair": {
                         "ConsequenceDatabase": "Hazus Earthquake - Transportation",
                         "MapApproach": "Automatic",
                     }
                 },
                 "Options": {
-                    "NonDirectionalMultipliers": {
-                        "ALL": 1.0
-                    },
-                }
+                    "NonDirectionalMultipliers": {"ALL": 1.0},
+                },
             }
         elif inf_type == "Roadway":
             # get the road class
             rt = convertRoadToHAZUSclass(GI)
             GI_ap['RoadHazusClass'] = rt
 
             # fmt: off
@@ -511,24 +505,21 @@
                 "Losses": {
                     "Repair": {
                         "ConsequenceDatabase": "Hazus Earthquake - Transportation",
                         "MapApproach": "Automatic",
                     }
                 },
                 "Options": {
-                    "NonDirectionalMultipliers": {
-                        "ALL": 1.0
-                    },
-                }
+                    "NonDirectionalMultipliers": {"ALL": 1.0},
+                },
             }
         else:
             print("subtype not supported in HWY")
 
     elif assetType == "WaterDistributionNetwork":
-
         pipe_material_map = {
             "CI": "B",
             "AC": "B",
             "RCC": "B",
             "DI": "D",
             "PVC": "D",
             "DS": "B",
@@ -699,15 +690,14 @@
                     "DamageProcess": "User Defined",
                     "DamageProcessFilePath": "dmg_process.json",
                 },
                 "Demands": demand_config,
             }
 
         elif wdn_element_type == "Tank":
-
             tank_cmp_lines = {
                 ("OG", "C", 1): {'PST.G.C.A.GS': ['ea', 1, 1, 1, 'N/A']},
                 ("OG", "C", 0): {'PST.G.C.U.GS': ['ea', 1, 1, 1, 'N/A']},
                 ("OG", "S", 1): {'PST.G.S.A.GS': ['ea', 1, 1, 1, 'N/A']},
                 ("OG", "S", 0): {'PST.G.S.U.GS': ['ea', 1, 1, 1, 'N/A']},
                 # Anchored status and Wood is not defined for On Ground tanks
                 ("OG", "W", 0): {'PST.G.W.GS': ['ea', 1, 1, 1, 'N/A']},
```

### Comparing `pelicun-3.3.2/pelicun/resources/auto/Hazus_Earthquake_Story.py` & `pelicun-3.3.3/pelicun/resources/auto/Hazus_Earthquake_Story.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,21 +220,23 @@
             index=['Units', 'Location', 'Direction', 'Theta_0', 'Family'],
         ).T
 
         # if needed, add components to simulate damage from ground failure
         if ground_failure:
             foundation_type = 'S'
 
+            # fmt: off
             FG_GF_H = f'GF.H.{foundation_type}'                                        # noqa
             FG_GF_V = f'GF.V.{foundation_type}'                                        # noqa
             CMP_GF = pd.DataFrame(                                                     # noqa
                 {f'{FG_GF_H}':[  'ea',         1,          1,        1,   'N/A'],      # noqa
                  f'{FG_GF_V}':[  'ea',         1,          3,        1,   'N/A']},     # noqa
                 index = [     'Units','Location','Direction','Theta_0','Family']       # noqa
             ).T                                                                        # noqa
+            # fmt: on
 
             CMP = pd.concat([CMP, CMP_GF], axis=0)
 
         # get the occupancy class
         if GI['OccupancyClass'] in ap_Occupancy.keys():
             ot = ap_Occupancy[GI['OccupancyClass']]
         else:
@@ -261,18 +263,16 @@
                 "OccupancyType": f"{ot}",
                 "PlanArea": str(plan_area),
             },
             "Damage": {"DamageProcess": "Hazus Earthquake"},
             "Demands": {},
             "Losses": {"Repair": repair_config},
             "Options": {
-                "NonDirectionalMultipliers": {
-                    "ALL": 1.0
-                },
-            }
+                "NonDirectionalMultipliers": {"ALL": 1.0},
+            },
         }
 
     else:
         print(
             f"AssetType: {assetType} is not supported "
             f"in Hazus Earthquake Story-based DL method"
         )
```

### Comparing `pelicun-3.3.2/pelicun/settings/default_units.json` & `pelicun-3.3.3/pelicun/settings/default_units.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/tests/code_repetition_checker.py` & `pelicun-3.3.3/pelicun/tests/code_repetition_checker.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/duplicate.json` & `pelicun-3.3.3/pelicun/tests/data/base/test_parse_units/duplicate.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/duplicate2.json` & `pelicun-3.3.3/pelicun/tests/data/base/test_parse_units/duplicate2.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/no_units.csv` & `pelicun-3.3.3/pelicun/tests/data/file_io/test_load_data/no_units.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/units.csv` & `pelicun-3.3.3/pelicun/tests/data/file_io/test_load_data/units.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/tests/reset_tests.py` & `pelicun-3.3.3/pelicun/tests/reset_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,15 @@
       `pelicun` directory. Dangerous things may happen otherwise.
 
     """
 
     cwd = os.path.basename(os.getcwd())
     if cwd != 'pelicun':
         raise OSError(
-            'Wrong directory. '
-            'See the docstring of `reset_all_test_data`. Aborting'
+            'Wrong directory. ' 'See the docstring of `reset_all_test_data`. Aborting'
         )
 
     # where the test result data are stored
     testdir = os.path.join(*('tests', 'data'))
     if not os.path.exists(testdir):
         raise ValueError('pelicun/tests/data directory not found.')
```

### Comparing `pelicun-3.3.2/pelicun/tests/test_assessment.py` & `pelicun-3.3.3/pelicun/tests/test_assessment.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/tests/test_auto.py` & `pelicun-3.3.3/pelicun/tests/test_auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,22 +102,18 @@
 
 def test_pelicun_default_path_replacement(
     setup_auto_script_path, setup_expected_base_path
 ):
     modified_path = setup_auto_script_path.replace(
         'PelicunDefault/', setup_expected_base_path
     )
-    assert modified_path.startswith(
-        setup_expected_base_path
-    )
+    assert modified_path.startswith(setup_expected_base_path)
 
 
-def test_auto_population_script_execution(
-    setup_valid_config, setup_auto_script_path
-):
+def test_auto_population_script_execution(setup_valid_config, setup_auto_script_path):
     with patch('pelicun.base.pelicun_path', '/expected/path'), patch(
         'os.path.exists', return_value=True
     ), patch('importlib.__import__') as mock_import:
         mock_auto_populate_ext = MagicMock(
             return_value=({'AIM_ap': 'value'}, {'DL_ap': 'value'}, 'CMP')
         )
         mock_import.return_value.auto_populate = mock_auto_populate_ext
```

### Comparing `pelicun-3.3.2/pelicun/tests/test_base.py` & `pelicun-3.3.3/pelicun/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,19 @@
     user_config_options = {
         "Verbose": False,
         "Seed": None,
         "LogShowMS": False,
         "LogFile": 'test_log_file',
         "PrintLog": False,
         "DemandOffset": {"PFA": -1, "PFV": -1},
+        "Sampling": {
+            "SamplingMethod": "MonteCarlo",
+            "SampleSize": 1000,
+            "PreserveRawOrder": False,
+        },
         "SamplingMethod": "MonteCarlo",
         "NonDirectionalMultipliers": {"ALL": 1.2},
         "EconomiesOfScale": {"AcrossFloors": True, "AcrossDamageStates": True},
         "RepairCostAndTimeCorrelation": 0.7,
     }
 
     # Create an Options object using the user_config_options
@@ -405,31 +410,27 @@
     data_converted = base.convert_to_MultiIndex(data, axis=0, inplace=False)
     expected_index = pd.MultiIndex.from_arrays((('A', 'B', 'C'), ('1', '1', '1')))
     assert data_converted.index.equals(expected_index)
     # original data should not have changed
     assert data.index.equals(pd.Index(('A-1', 'B-1', 'C-1')))
 
     # Test a case where the index is already a MultiIndex
-    data_converted = base.convert_to_MultiIndex(
-        data_converted, axis=0, inplace=False
-    )
+    data_converted = base.convert_to_MultiIndex(data_converted, axis=0, inplace=False)
     assert data_converted.index.equals(expected_index)
 
     # Test a case where the columns need to be converted to a MultiIndex
     data = pd.DataFrame({'A-1': (1, 2, 3), 'B-1': (4, 5, 6)})
     data_converted = base.convert_to_MultiIndex(data, axis=1, inplace=False)
     expected_columns = pd.MultiIndex.from_arrays((('A', 'B'), ('1', '1')))
     assert data_converted.columns.equals(expected_columns)
     # original data should not have changed
     assert data.columns.equals(pd.Index(('A-1', 'B-1')))
 
     # Test a case where the columns are already a MultiIndex
-    data_converted = base.convert_to_MultiIndex(
-        data_converted, axis=1, inplace=False
-    )
+    data_converted = base.convert_to_MultiIndex(data_converted, axis=1, inplace=False)
     assert data_converted.columns.equals(expected_columns)
 
     # Test an invalid axis parameter
     with pytest.raises(ValueError):
         base.convert_to_MultiIndex(data_converted, axis=2, inplace=False)
 
     # inplace=True
@@ -500,17 +501,15 @@
         ),
         dtype='object',
     )
 
     # case 1:
     # passing a dataframe
 
-    df = pd.DataFrame(
-        ((1.00, 2.00, 3.00), (4.00, 5.00, 6.00)), columns=['A', 'B', 'C']
-    )
+    df = pd.DataFrame(((1.00, 2.00, 3.00), (4.00, 5.00, 6.00)), columns=['A', 'B', 'C'])
     desc = base.describe(df)
     assert np.all(desc.index == expected_idx)
     assert np.all(desc.columns == pd.Index(('A', 'B', 'C'), dtype='object'))
 
     # case 2:
     # passing a series
 
@@ -599,15 +598,16 @@
 
     # Test when string is 'roof'
     assert base.process_loc('roof', 10) == [
         10,
     ]
 
     # Test when string cannot be converted to an int or recognized
-    assert base.process_loc('abc', 10) is None
+    with pytest.raises(ValueError):
+        base.process_loc('abc', 10)
 
 
 def test_run_input_specs():
     assert os.path.basename(base.pelicun_path) == 'pelicun'
 
 
 def test_dict_raise_on_duplicates():
```

### Comparing `pelicun-3.3.2/pelicun/tests/test_file_io.py` & `pelicun-3.3.3/pelicun/tests/test_file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,17 +166,15 @@
 
     data = file_io.load_data(filepath, unit_conversion_factors)
     assert np.array_equal(data.index.values, np.array(range(6)))
     assert data.shape == (6, 19)
     assert isinstance(data.columns, pd.core.indexes.multi.MultiIndex)
     assert data.columns.nlevels == 4
 
-    _, units = file_io.load_data(
-        filepath, unit_conversion_factors, return_units=True
-    )
+    _, units = file_io.load_data(filepath, unit_conversion_factors, return_units=True)
 
     for item in unit_conversion_factors:
         assert item in units.unique()
 
     filepath = 'pelicun/tests/data/file_io/test_load_data/no_units.csv'
     data_nounits = file_io.load_data(filepath, {})
     assert isinstance(data_nounits, pd.DataFrame)
```

### Comparing `pelicun-3.3.2/pelicun/tests/test_model.py` & `pelicun-3.3.3/pelicun/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,21 +239,18 @@
 
     def test_estimate_RID(self, demand_model_with_sample):
         demands = demand_model_with_sample.sample['PID']
         params = {'yield_drift': 0.01}
         res = demand_model_with_sample.estimate_RID(demands, params)
         assert list(res.columns) == [('RID', '1', '1')]
         assert (
-            demand_model_with_sample.estimate_RID(demands, params, method='xyz')
-            is None
+            demand_model_with_sample.estimate_RID(demands, params, method='xyz') is None
         )
 
-    def test_calibrate_model(
-        self, calibrated_demand_model, demand_model_with_sample_C
-    ):
+    def test_calibrate_model(self, calibrated_demand_model, demand_model_with_sample_C):
         assert calibrated_demand_model.marginal_params['Family'].to_list() == [
             'normal',
             'normal',
             'lognormal',
             'empirical',
         ]
         assert (
@@ -291,17 +288,14 @@
             },
             "PID": {
                 "DistributionFamily": "lognormal",
                 "TruncateUpper": "0.04",
             },
         }
         demand_model_with_sample_C.calibrate_model(config)
-        # calibrating again should raise an error
-        with pytest.raises(ValueError):
-            demand_model_with_sample_C.calibrate_model(config)
 
     def test_save_load_model_with_empirical(
         self, calibrated_demand_model, assessment_instance
     ):
         # a model that has empirical marginal parameters
         temp_dir = tempfile.mkdtemp()
         calibrated_demand_model.save_model(f'{temp_dir}/temp')
@@ -371,17 +365,15 @@
     #         demand_model_with_sample_C.empirical_data,
     #         new_demand_model.empirical_data,
     #     )
 
     def test_generate_sample_exceptions(self, demand_model):
         # generating a sample from a non calibrated model should fail
         with pytest.raises(ValueError):
-            demand_model.generate_sample(
-                {"SampleSize": 3, 'PreserveRawOrder': False}
-            )
+            demand_model.generate_sample({"SampleSize": 3, 'PreserveRawOrder': False})
 
     def test_generate_sample(self, calibrated_demand_model):
         calibrated_demand_model.generate_sample(
             {"SampleSize": 3, 'PreserveRawOrder': False}
         )
 
         # get the generated demand sample
@@ -516,17 +508,15 @@
             columns=['Theta_0'],
             index=pd.MultiIndex.from_tuples(
                 (('A', '0', '1'),), names=('cmp', 'loc', 'dir')
             ),
         )
         units = pd.Series(['ea'], index=marginal_params.index)
         arg_units = None
-        res = pelicun_model.convert_marginal_params(
-            marginal_params, units, arg_units
-        )
+        res = pelicun_model.convert_marginal_params(marginal_params, units, arg_units)
 
         # >>> res
         #             Theta_0
         # cmp loc dir
         # A   0   1       1.0
 
         assert 'Theta_0' in res.columns
@@ -556,17 +546,15 @@
                     ('D', '0', '1'),
                 ),
                 names=('cmp', 'loc', 'dir'),
             ),
         )
         units = pd.Series(['ea', 'ft', 'in', 'in2'], index=marginal_params.index)
         arg_units = None
-        res = pelicun_model.convert_marginal_params(
-            marginal_params, units, arg_units
-        )
+        res = pelicun_model.convert_marginal_params(marginal_params, units, arg_units)
 
         expected_df = pd.DataFrame(
             {
                 'Family': [np.nan, 'normal', 'lognormal', 'uniform'],
                 'Theta_0': [1.0000, np.nan, 0.0254, 0.0000],
                 'Theta_1': [np.nan, 1.000000, 0.500000, 0.0064516],
                 'Theta_2': [np.nan, np.nan, np.nan, np.nan],
@@ -594,17 +582,15 @@
             columns=['Theta_0'],
             index=pd.MultiIndex.from_tuples(
                 (('A', '0', '1'),), names=('cmp', 'loc', 'dir')
             ),
         )
         units = pd.Series(['test_three'], index=marginal_params.index)
         arg_units = pd.Series(['test_two'], index=marginal_params.index)
-        res = pelicun_model.convert_marginal_params(
-            marginal_params, units, arg_units
-        )
+        res = pelicun_model.convert_marginal_params(marginal_params, units, arg_units)
 
         # >>> res
         #                              Theta_0
         # cmp loc dir
         # A   0   1    750,600|40,20
 
         # note: '40,20' = '20,10' * 2.00 (test_two)
@@ -705,17 +691,15 @@
             expected_cmp_marginal_params,
             asset_model.cmp_marginal_params,
             check_index_type=False,
             check_column_type=False,
             check_dtype=False,
         )
 
-        expected_cmp_units = pd.Series(
-            data=['ea'], index=['component_a'], name='Units'
-        )
+        expected_cmp_units = pd.Series(data=['ea'], index=['component_a'], name='Units')
 
         pd.testing.assert_series_equal(
             expected_cmp_units,
             asset_model.cmp_units,
             check_index_type=False,
         )
 
@@ -1032,15 +1016,15 @@
                     ('LS4', 'DamageStateWeights'),
                     ('LS4', 'Family'),
                     ('LS4', 'Theta_0'),
                     ('LS4', 'Theta_1'),
                 )
             ),
         )
-        assessment_instance.damage.calculate(dmg_process=dmg_process)
+        assessment_instance.damage.calculate(sample_size=4, dmg_process=dmg_process)
         assessment_instance.asset.cmp_units = pd.Series(
             ['ea'] * len(assessment_instance.damage.sample.columns),
             index=assessment_instance.damage.sample.columns,
             name='Units',
             dtype='object',
         )
         return deepcopy(assessment_instance.damage)
@@ -1070,17 +1054,15 @@
         sample_from_variable = damage_model_with_sample.save_sample(save_units=False)
         pd.testing.assert_frame_equal(
             sample_from_file,
             sample_from_variable,
             check_index_type=False,
             check_column_type=False,
         )
-        _, units_from_variable = damage_model_with_sample.save_sample(
-            save_units=True
-        )
+        _, units_from_variable = damage_model_with_sample.save_sample(save_units=True)
         assert np.all(units_from_variable.to_numpy() == 'ea')
 
     def test_load_damage_model(self, damage_model_model_loaded):
         # should no longer be None
         assert damage_model_model_loaded.damage_params is not None
 
         assert list(damage_model_model_loaded.damage_params.columns) == [
@@ -1354,30 +1336,27 @@
             sample_size, PGB
         )
 
         ds_sample = damage_model._evaluate_damage_state(
             demand_dict, EDP_req, capacity_sample, lsds_sample
         )
 
-        qnt_sample = damage_model._prepare_dmg_quantities(
-            PGB, ds_sample, dropzero=False
-        )
+        qnt_sample = damage_model._prepare_dmg_quantities(ds_sample, dropzero=False)
 
         # note: the realized number of damage states is random, limiting
         # our assertions
         assert ds_sample.shape[0] == 10
         assert qnt_sample.shape[0] == 10
         assert list(qnt_sample.index) == [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
         assert list(ds_sample.index) == [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
 
         assert list(ds_sample.columns)[0] == ('B.10.31.001', '2', '2', '0', '1')
         assert list(qnt_sample.columns)[0] == ('B.10.31.001', '2', '2', '0', '0')
 
     def test__perform_dmg_task(self, assessment_instance):
-
         damage_model = assessment_instance.damage
 
         #
         # when CMP.B reaches DS1, CMP.A should be DS4
         #
 
         ds_sample = pd.DataFrame(
@@ -1665,20 +1644,20 @@
         demand_model = damage_model._asmnt.demand
         assessment_instance = damage_model._asmnt
         asset_model = assessment_instance.asset
 
         # A damage calculation test utilizing a multilinear CDF RV for
         # the capcity.
 
-        num_realizations = 1000
+        sample_size = 1000
 
         # define the demand
         conversion_factor = assessment_instance.unit_conversion_factors['inps2']
         demand_model.sample = pd.DataFrame(
-            np.full(num_realizations, 0.50 * conversion_factor),
+            np.full(sample_size, 0.50 * conversion_factor),
             columns=(('PGV', '0', '1'),),
         )
 
         # Define the component in the asset model
         asset_model.cmp_marginal_params = pd.DataFrame(
             {
                 'Theta_0': (1.0,),
@@ -1698,30 +1677,30 @@
                 'pelicun/tests/data/model/'
                 'test_DamageModel_calculate_multilinear_CDF/'
                 'damage_model.csv'
             ]
         )
 
         # calculate damage
-        damage_model.calculate()
+        damage_model.calculate(sample_size)
 
         res = damage_model.sample.value_counts()
         assert res.to_dict() == {(1.0, 0.0): 750, (0.0, 1.0): 250}
 
 
 class TestLossModel(TestPelicunModel):
     @pytest.fixture
     def loss_model(self, assessment_instance):
         return deepcopy(model.LossModel(assessment_instance))
 
     def test_init(self, loss_model):
         assert loss_model.log_msg
         assert loss_model.log_div
 
-        assert loss_model._sample is None
+        assert loss_model.sample is None
         assert loss_model.loss_type == 'Generic'
 
     def test_load_sample_save_sample(self, loss_model):
         loss_model.loss_params = pd.DataFrame(
             (
                 (
                     "normal",
@@ -1773,15 +1752,15 @@
             ),
         )
 
         loss_model.load_sample(sample)
 
         pd.testing.assert_frame_equal(
             sample,
-            loss_model._sample,
+            loss_model.sample,
             check_index_type=False,
             check_column_type=False,
         )
 
         output = loss_model.save_sample(None)
         output.index = output.index.astype('int64')
 
@@ -1881,15 +1860,15 @@
             ),
         )
 
     def test_init(self, repair_model):
         assert repair_model.log_msg
         assert repair_model.log_div
 
-        assert repair_model._sample is None
+        assert repair_model.sample is None
         assert repair_model.loss_type == 'Repair'
 
     def test__create_DV_RVs(self, repair_model, loss_params_A):
         repair_model.loss_params = loss_params_A
 
         repair_model.loss_map = pd.DataFrame(
             ((("DMG", "some.test.component"), "some.test.component"),),
@@ -1912,26 +1891,18 @@
             'Cost-0-1-3-1-0',
             'Time-0-1-3-1-0',
         ]
         rvs = list(rv_reg.RV.values())
         for rv in rvs:
             print(rv.theta)
             assert rv.distribution == 'normal'
-        np.testing.assert_array_equal(
-            rvs[0].theta, np.array((1.00, 0.390923, np.nan))
-        )
-        np.testing.assert_array_equal(
-            rvs[1].theta, np.array((1.00, 0.464027, np.nan))
-        )
-        np.testing.assert_array_equal(
-            rvs[2].theta, np.array((1.00, 0.390923, np.nan))
-        )
-        np.testing.assert_array_equal(
-            rvs[3].theta, np.array((1.00, 0.464027, np.nan))
-        )
+        np.testing.assert_array_equal(rvs[0].theta, np.array((1.00, 0.390923, np.nan)))
+        np.testing.assert_array_equal(rvs[1].theta, np.array((1.00, 0.464027, np.nan)))
+        np.testing.assert_array_equal(rvs[2].theta, np.array((1.00, 0.390923, np.nan)))
+        np.testing.assert_array_equal(rvs[3].theta, np.array((1.00, 0.464027, np.nan)))
 
     def test__calc_median_consequence(self, repair_model, loss_params_A):
         repair_model.loss_params = loss_params_A
 
         repair_model.loss_map = pd.DataFrame(
             ((("DMG", "some.test.component"), "some.test.component"),),
             columns=("Driver", "Consequence"),
@@ -1948,50 +1919,14 @@
             ),
         )
 
         medians = repair_model._calc_median_consequence(eco_qnt)
         assert medians['Cost'].to_dict() == {(0, '1'): {0: 25704.0, 1: 22848.0}}
         assert medians['Time'].to_dict() == {(0, '1'): {0: 22.68, 1: 20.16}}
 
-    def test_aggregate_losses(self, repair_model, loss_params_A):
-        repair_model._sample = pd.DataFrame(
-            ((100.00, 1.00),),
-            columns=pd.MultiIndex.from_tuples(
-                (
-                    (
-                        "Cost",
-                        "some.test.component",
-                        "some.test.component",
-                        "1",
-                        "1",
-                        "1",
-                    ),
-                    (
-                        "Time",
-                        "some.test.component",
-                        "some.test.component",
-                        "1",
-                        "1",
-                        "1",
-                    ),
-                ),
-                names=("dv", "loss", "dmg", "ds", "loc", "dir"),
-            ),
-        )
-
-        repair_model.loss_params = loss_params_A
-
-        df_agg = repair_model.aggregate_losses()
-
-        assert df_agg.to_dict() == {
-            ('repair_cost', ''): {0: 100.0},
-            ('repair_time', 'parallel'): {0: 1.0},
-            ('repair_time', 'sequential'): {0: 1.0},
-        }
-
     def test__generate_DV_sample(self, repair_model):
         expected_sample = {
             (True, True): {
                 (
                     'Cost',
                     'some.test.component',
                     'some.test.component',
@@ -2137,15 +2072,51 @@
                         ("Quantity", "Unit"),
                     )
                 ),
             )
 
             repair_model._generate_DV_sample(dmg_quantities, 4)
 
-            assert repair_model._sample.to_dict() == expected_sample[(ecods, ecofl)]
+            assert repair_model.sample.to_dict() == expected_sample[(ecods, ecofl)]
+
+    def test_aggregate_losses(self, repair_model, loss_params_A):
+        repair_model.sample = pd.DataFrame(
+            ((100.00, 1.00),),
+            columns=pd.MultiIndex.from_tuples(
+                (
+                    (
+                        "Cost",
+                        "some.test.component",
+                        "some.test.component",
+                        "1",
+                        "1",
+                        "1",
+                    ),
+                    (
+                        "Time",
+                        "some.test.component",
+                        "some.test.component",
+                        "1",
+                        "1",
+                        "1",
+                    ),
+                ),
+                names=("dv", "loss", "dmg", "ds", "loc", "dir"),
+            ),
+        )
+
+        repair_model.loss_params = loss_params_A
+
+        df_agg = repair_model.aggregate_losses()
+
+        assert df_agg.to_dict() == {
+            ('repair_cost', ''): {0: 100.0},
+            ('repair_time', 'parallel'): {0: 1.0},
+            ('repair_time', 'sequential'): {0: 1.0},
+        }
 
 
 #  _____                 _   _
 # |  ___|   _ _ __   ___| |_(_) ___  _ __  ___
 # | |_ | | | | '_ \ / __| __| |/ _ \| '_ \/ __|
 # |  _|| |_| | | | | (__| |_| | (_) | | | \__ \
 # |_|   \__,_|_| |_|\___|\__|_|\___/|_| |_|___/
```

### Comparing `pelicun-3.3.2/pelicun/tests/test_uq.py` & `pelicun-3.3.3/pelicun/tests/test_uq.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,17 +171,15 @@
     with pytest.raises(ValueError):
         uq._get_theta(np.array((1.00,)), np.array((1.00,)), 'not_a_distribution')
 
 
 def test__get_limit_probs():
     # verify that it works for valid inputs
 
-    res = uq._get_limit_probs(
-        np.array((0.10, 0.20)), 'normal', np.array((0.15, 1.00))
-    )
+    res = uq._get_limit_probs(np.array((0.10, 0.20)), 'normal', np.array((0.15, 1.00)))
     assert np.allclose(res, np.array((0.4800611941616275, 0.5199388058383725)))
 
     res = uq._get_limit_probs(
         np.array((np.nan, 0.20)), 'normal', np.array((0.15, 1.00))
     )
     assert np.allclose(res, np.array((0.0, 0.5199388058383725)))
 
@@ -901,29 +899,25 @@
     rv = uq.LogNormalRandomVariable(
         'test_rv',
         theta=(1.0, 1.0),
         truncation_limits=np.array((0.10, np.nan)),
     )
     x = (-1.0, 0.0, 0.5, 1.0, 2.0)
     cdf = rv.cdf(x)
-    assert np.allclose(
-        cdf, (0.0, 0.0, 0.23597085, 0.49461712, 0.75326339), rtol=1e-5
-    )
+    assert np.allclose(cdf, (0.0, 0.0, 0.23597085, 0.49461712, 0.75326339), rtol=1e-5)
 
     # upper truncation
     rv = uq.LogNormalRandomVariable(
         'test_rv',
         theta=(1.0, 1.0),
         truncation_limits=np.array((np.nan, 5.00)),
     )
     x = (-1.0, 0.0, 0.5, 1.0, 2.0)
     cdf = rv.cdf(x)
-    assert np.allclose(
-        cdf, (0.00, 0.00, 0.25797755, 0.52840734, 0.79883714), rtol=1e-5
-    )
+    assert np.allclose(cdf, (0.00, 0.00, 0.25797755, 0.52840734, 0.79883714), rtol=1e-5)
 
     # no truncation
     rv = uq.LogNormalRandomVariable('test_rv', theta=(1.0, 1.0))
     x = (-1.0, 0.0, 0.5, 1.0, 2.0)
     cdf = rv.cdf(x)
     assert np.allclose(cdf, (0.0, 0.0, 0.2441086, 0.5, 0.7558914), rtol=1e-5)
 
@@ -1050,17 +1044,15 @@
     with pytest.raises(ValueError):
         rv.inverse_transform_sampling()
 
 
 def test_MultinomialRandomVariable():
     # multinomial with invalid p values provided in the theta vector
     with pytest.raises(ValueError):
-        uq.MultinomialRandomVariable(
-            'rv_invalid', np.array((0.20, 0.70, 0.10, 42.00))
-        )
+        uq.MultinomialRandomVariable('rv_invalid', np.array((0.20, 0.70, 0.10, 42.00)))
 
 
 def test_MultilinearCDFRandomVariable():
     # multilinear CDF: cases that should fail
 
     x_values = (0.00, 1.00, 2.00, 3.00, 4.00)
     y_values = (100.00, 0.20, 0.20, 0.80, 1.00)
@@ -1155,17 +1147,15 @@
     )
 
 
 def test_DeterministicRandomVariable_inverse_transform():
     rv = uq.DeterministicRandomVariable('test_rv', theta=np.array((0.00,)))
     rv.inverse_transform_sampling(4)
     inverse_transform = rv.sample
-    assert np.allclose(
-        inverse_transform, np.array((0.00, 0.00, 0.00, 0.00)), rtol=1e-5
-    )
+    assert np.allclose(inverse_transform, np.array((0.00, 0.00, 0.00, 0.00)), rtol=1e-5)
 
 
 def test_RandomVariable_Set():
     # a set of two random variables
     rv_1 = uq.NormalRandomVariable('rv1', theta=(1.0, 1.0))
     rv_2 = uq.NormalRandomVariable('rv2', theta=(1.0, 1.0))
     rv_set = uq.RandomVariableSet(  # noqa: F841
```

### Comparing `pelicun-3.3.2/pelicun/tests/util.py` & `pelicun-3.3.3/pelicun/tests/util.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.2/pelicun/tools/DL_calculation.py` & `pelicun-3.3.3/pelicun/tools/DL_calculation.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,22 +56,24 @@
 from pelicun.base import describe
 from pelicun.base import EDP_to_demand_type
 from pelicun.file_io import load_data
 from pelicun.assessment import Assessment
 
 
 # this is exceptional code
+# (so let's run pylint everywhere /except/ here.)
 # pylint: disable=consider-using-namedtuple-or-dataclass
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-statements
 # pylint: disable=too-many-nested-blocks
 # pylint: disable=too-many-branches
 
 # pd.set_option('display.max_rows', None)
 
+
 def log_msg(msg):
     formatted_msg = f'{strftime("%Y-%m-%dT%H:%M:%SZ", gmtime())} {msg}'
 
     print(formatted_msg)
 
 
 sys.path.insert(0, os.path.dirname(os.path.realpath(__file__)))
@@ -365,24 +367,23 @@
     # open the config file and parse it
     with open(config_path, 'r', encoding='utf-8') as f:
         config = json.load(f)
 
     # f"{config['commonFileDir']}/CustomDLModels/"
     custom_dl_file_path = custom_model_dir
 
-    DL_config = config.get('DL', None)
-    if not DL_config:
+    if ('DL' not in config) or (not config['DL']):
         log_msg("Damage and Loss configuration missing from config file. ")
 
         if auto_script_path is not None:
             log_msg("Trying to auto-populate")
 
             config_ap, CMP = auto_populate(config, auto_script_path)
 
-            if config_ap['DL'] is None:
+            if not config_ap['DL']:
 
                 log_msg(
                     "The prescribed auto-population script failed to identify "
                     "a valid damage and loss configuration for this asset. "
                     "Terminating analysis."
                 )
 
@@ -411,127 +412,135 @@
 
             # if detailed results are not requested, add a lean output config
             if detailed_results is False:
                 config_ap['DL'].update({'Outputs': regional_out_config})
             else:
                 config_ap['DL'].update({'Outputs': full_out_config})
                 # add output settings from regional output config
-                if 'Settings' not in config_ap['DL']['Outputs'].keys():
+                if 'Settings' not in config_ap['DL']['Outputs']:
                     config_ap['DL']['Outputs'].update({'Settings': {}})
 
                 config_ap['DL']['Outputs']['Settings'].update(
                     regional_out_config['Settings']
-                )
+                )            
 
             # save the extended config to a file
             config_ap_path = Path(config_path.stem + '_ap.json').resolve()
 
             with open(config_ap_path, 'w') as f:
                 json.dump(config_ap, f, indent=2)
 
-            DL_config = config_ap.get('DL', None)
+            config['DL'] = config_ap.get('DL', None)
 
         else:
             log_msg("Terminating analysis.")
 
             return -1
 
-    GI_config = config.get('GeneralInformation', None)
-
-    asset_config = DL_config.get('Asset', None)
-    demand_config = DL_config.get('Demands', None)
-    damage_config = DL_config.get('Damage', None)
-    loss_config = DL_config.get('Losses', None)
-    out_config = DL_config.get('Outputs', None)
+    #
+    # sample size: backwards compatibility
+    #
+    sample_size_str = (
+        # expected location
+        config.get('Options', {})
+        .get('Sampling', {})
+        .get('SampleSize', None)
+    )
+    if not sample_size_str:
+        # try previous location
+        sample_size_str = (
+            config.get('DL', {}).get('Demands', {}).get('SampleSize', None)
+        )
+    if not sample_size_str:
+        # give up
+        print('Sample size not provided in config file.')
+        return -1
+    sample_size = int(sample_size_str)
 
     # provide all outputs if the files are not specified
-    if out_config is None:
-        out_config = full_out_config
+    if ('Outputs' not in config['DL']) or (not config['DL']['Outputs']):
+        config['DL']['Outputs'] = full_out_config
 
     # provide outputs in CSV by default
-    if ('Format' in out_config.keys()) is False:
-        out_config.update({'Format': {'CSV': True, 'JSON': False}})
+    if ('Format' in config['DL']['Outputs'].keys()) is False:
+        config['DL']['Outputs'].update({'Format': {'CSV': True, 'JSON': False}})
 
     # override file format specification if the output_format is provided
     if output_format is not None:
-        out_config.update(
+        config['DL']['Outputs'].update(
             {
                 'Format': {
                     'CSV': 'csv' in output_format,
                     'JSON': 'json' in output_format,
                 }
             }
         )
 
     # add empty Settings to output config to simplify code below
-    if ('Settings' in out_config.keys()) is False:
-        out_config.update({'Settings': pbe_settings})
+    if ('Settings' in config['DL']['Outputs'].keys()) is False:
+        config['DL']['Outputs'].update({'Settings': pbe_settings})
 
-    if asset_config is None:
+    if ('Asset' not in config['DL']) or (not config['DL']['Asset']):
         log_msg("Asset configuration missing. Terminating analysis.")
         return -1
 
-    if demand_config is None:
+    if ('Demands' not in config['DL']) or (not config['DL']['Demands']):
         log_msg("Demand configuration missing. Terminating analysis.")
         return -1
 
     # get the length unit from the config file
     try:
-        length_unit = GI_config['units']['length']
+        length_unit = config['GeneralInformation']['units']['length']
     except KeyError:
         log_msg(
             "No default length unit provided in the input file. "
             "Terminating analysis. "
         )
 
         return -1
 
-    # if out_config is None:
-    #    log_msg("Output configuration missing. Terminating analysis.")
-    #    return -1
-
     # initialize the Pelicun Assessement
-    options = DL_config.get("Options", {})
+    options = config['DL'].get("Options", {})
     options.update({"LogFile": "pelicun_log.txt", "Verbose": True})
 
     # If the user did not prescribe anything for ListAllDamageStates,
-    # then use True as default for DL_calculations regardless of what 
+    # then use True as default for DL_calculations regardless of what
     # the Pelicun default is.
-    if "ListAllDamageStates" not in options.keys():
+    if "ListAllDamageStates" not in options:
         options.update({"ListAllDamageStates": True})
 
     PAL = Assessment(options)
 
     # Demand Assessment -----------------------------------------------------------
 
     # check if there is a demand file location specified in the config file
-    if demand_config.get('DemandFilePath', False):
-        demand_path = Path(demand_config['DemandFilePath']).resolve()
+    if config['DL']['Demands'].get('DemandFilePath', False):
+        demand_path = Path(config['DL']['Demands']['DemandFilePath']).resolve()
 
     else:
         # otherwise assume that there is a response.csv file next to the config file
         demand_path = config_path.parent / 'response.csv'
 
     # try to load the demands
     raw_demands = pd.read_csv(demand_path, index_col=0)
 
     # remove excessive demands that are considered collapses, if needed
-    if demand_config.get('CollapseLimits', False):
+    if config['DL']['Demands'].get('CollapseLimits', False):
         raw_demands = convert_to_MultiIndex(raw_demands, axis=1)
 
         if 'Units' in raw_demands.index:
             raw_units = raw_demands.loc['Units', :]
             raw_demands.drop('Units', axis=0, inplace=True)
 
         else:
             raw_units = None
 
         DEM_to_drop = np.full(raw_demands.shape[0], False)
 
-        for DEM_type, limit in demand_config['CollapseLimits'].items():
+        for DEM_type, limit in config['DL']['Demands']['CollapseLimits'].items():
             if raw_demands.columns.nlevels == 4:
                 DEM_to_drop += raw_demands.loc[:, idx[:, DEM_type, :, :]].max(
                     axis=1
                 ) > float(limit)
 
             else:
                 DEM_to_drop += raw_demands.loc[:, idx[DEM_type, :, :]].max(
@@ -556,42 +565,40 @@
     else:
         demands = raw_demands
 
     # load the available demand sample
     PAL.demand.load_sample(demands)
 
     # get the calibration information
-    if demand_config.get('Calibration', False):
+    if config['DL']['Demands'].get('Calibration', False):
         # then use it to calibrate the demand model
-        PAL.demand.calibrate_model(demand_config['Calibration'])
+        PAL.demand.calibrate_model(config['DL']['Demands']['Calibration'])
 
     else:
         # if no calibration is requested,
         # set all demands to use empirical distribution
         PAL.demand.calibrate_model({"ALL": {"DistributionFamily": "empirical"}})
 
     # and generate a new demand sample
-    sample_size = int(demand_config['SampleSize'])
-
     PAL.demand.generate_sample(
         {
             "SampleSize": sample_size,
-            'PreserveRawOrder': demand_config.get('CoupledDemands', False),
-            'DemandCloning': demand_config.get('DemandCloning', False)
+            'PreserveRawOrder': config['DL']['Demands'].get('CoupledDemands', False),
+            'DemandCloning': config['DL']['Demands'].get('DemandCloning', False),
         }
     )
 
     # get the generated demand sample
     demand_sample, demand_units = PAL.demand.save_sample(save_units=True)
 
     demand_sample = pd.concat([demand_sample, demand_units.to_frame().T])
 
     # get residual drift estimates, if needed
-    if demand_config.get('InferResidualDrift', False):
-        RID_config = demand_config['InferResidualDrift']
+    if config['DL']['Demands'].get('InferResidualDrift', False):
+        RID_config = config['DL']['Demands']['InferResidualDrift']
 
         if RID_config['method'] == 'FEMA P-58':
             RID_list = []
             PID = demand_sample['PID'].copy()
             PID.drop('Units', inplace=True)
             PID = PID.astype(float)
 
@@ -622,16 +629,19 @@
     # add a constant one demand
     demand_sample[('ONE', '0', '1')] = np.ones(demand_sample.shape[0])
     demand_sample.loc['Units', ('ONE', '0', '1')] = 'unitless'
 
     PAL.demand.load_sample(convert_to_SimpleIndex(demand_sample, axis=1))
 
     # save results
-    if out_config.get('Demand', None) is not None:
-        out_reqs = [out if val else "" for out, val in out_config['Demand'].items()]
+    if 'Demand' in config['DL']['Outputs']:
+        out_reqs = [
+            out if val else ""
+            for out, val in config['DL']['Outputs']['Demand'].items()
+        ]
 
         if np.any(np.isin(['Sample', 'Statistics'], out_reqs)):
             demand_sample, demand_units = PAL.demand.save_sample(save_units=True)
 
             demand_units = demand_units.to_frame().T
 
             if 'Sample' in out_reqs:
@@ -681,30 +691,30 @@
             output_files.append('EDP.csv')
         """
         # - - - - -
 
     # Asset Definition ------------------------------------------------------------
 
     # set the number of stories
-    if asset_config.get('NumberOfStories', False):
-        PAL.stories = int(asset_config['NumberOfStories'])
+    if config['DL']['Asset'].get('NumberOfStories', False):
+        PAL.stories = int(config['DL']['Asset']['NumberOfStories'])
 
     # load a component model and generate a sample
-    if asset_config.get('ComponentAssignmentFile', False):
+    if config['DL']['Asset'].get('ComponentAssignmentFile', False):
         cmp_marginals = pd.read_csv(
-            asset_config['ComponentAssignmentFile'],
+            config['DL']['Asset']['ComponentAssignmentFile'],
             index_col=0,
             encoding_errors='replace',
         )
 
         DEM_types = demand_sample.columns.unique(level=0)
 
         # add component(s) to support collapse calculation
-        if 'CollapseFragility' in damage_config.keys():
-            coll_DEM = damage_config['CollapseFragility']["DemandType"]
+        if 'CollapseFragility' in config['DL']['Damage'].keys():
+            coll_DEM = config['DL']['Damage']['CollapseFragility']["DemandType"]
             if coll_DEM.startswith('SA'):
                 # we have a global demand and evaluate collapse directly
                 pass
 
             else:
                 # we need story-specific collapse assessment
 
@@ -733,15 +743,15 @@
         # always add a component to support basic collapse calculation
         cmp_marginals.loc['collapse', 'Units'] = 'ea'
         cmp_marginals.loc['collapse', 'Location'] = 0
         cmp_marginals.loc['collapse', 'Direction'] = 1
         cmp_marginals.loc['collapse', 'Theta_0'] = 1.0
 
         # add components to support irreparable damage calculation
-        if 'IrreparableDamage' in damage_config.keys():
+        if 'IrreparableDamage' in config['DL']['Damage'].keys():
             if 'RID' in DEM_types:
                 # excessive RID is added on every floor to detect large RIDs
                 cmp_marginals.loc['excessiveRID', 'Units'] = 'ea'
 
                 locs = demand_sample['RID'].columns.unique(level=0)
                 cmp_marginals.loc['excessiveRID', 'Location'] = ','.join(locs)
 
@@ -767,35 +777,40 @@
         # load component model
         PAL.asset.load_cmp_model({'marginals': cmp_marginals})
 
         # generate component quantity sample
         PAL.asset.generate_cmp_sample()
 
     # if requested, load the quantity sample from a file
-    elif asset_config.get('ComponentSampleFile', False):
-        PAL.asset.load_cmp_sample(asset_config['ComponentSampleFile'])
+    elif config['DL']['Asset'].get('ComponentSampleFile', False):
+        PAL.asset.load_cmp_sample(config['DL']['Asset']['ComponentSampleFile'])
 
     # if requested, save results
-    if out_config.get('Asset', None) is not None:
+    if 'Asset' in config['DL']['Outputs']:
         cmp_sample, cmp_units = PAL.asset.save_cmp_sample(save_units=True)
         cmp_units = cmp_units.to_frame().T
 
         if (
-            out_config['Settings'].get('AggregateColocatedComponentResults', False)
+            config['DL']['Outputs']['Settings'].get(
+                'AggregateColocatedComponentResults', False
+            )
             is True
         ):
             cmp_units = cmp_units.groupby(level=[0, 1, 2], axis=1).first()
 
             cmp_groupby_uid = cmp_sample.groupby(level=[0, 1, 2], axis=1)
 
             cmp_sample = cmp_groupby_uid.sum().mask(
                 cmp_groupby_uid.count() == 0, np.nan
             )
 
-        out_reqs = [out if val else "" for out, val in out_config['Asset'].items()]
+        out_reqs = [
+            out if val else ""
+            for out, val in config['DL']['Outputs']['Asset'].items()
+        ]
 
         if np.any(np.isin(['Sample', 'Statistics'], out_reqs)):
             if 'Sample' in out_reqs:
                 cmp_sample_s = pd.concat([cmp_sample, cmp_units])
 
                 cmp_sample_s = convert_to_SimpleIndex(cmp_sample_s, axis=1)
                 cmp_sample_s.to_csv(
@@ -847,26 +862,31 @@
             output_files.append('AIM.csv')
         """
         # - - - - -
 
     # Damage Assessment -----------------------------------------------------------
 
     # if a damage assessment is requested
-    if damage_config is not None:
+    if 'Damage' in config['DL']:
         # load the fragility information
-        if asset_config['ComponentDatabase'] in default_DBs['fragility'].keys():
+        if (
+            config['DL']['Asset']['ComponentDatabase']
+            in default_DBs['fragility'].keys()
+        ):
             component_db = [
                 'PelicunDefault/'
-                + default_DBs['fragility'][asset_config['ComponentDatabase']],
+                + default_DBs['fragility'][
+                    config['DL']['Asset']['ComponentDatabase']
+                ],
             ]
         else:
             component_db = []
 
-        if asset_config.get('ComponentDatabasePath', False) is not False:
-            extra_comps = asset_config['ComponentDatabasePath']
+        if config['DL']['Asset'].get('ComponentDatabasePath', False) is not False:
+            extra_comps = config['DL']['Asset']['ComponentDatabasePath']
 
             if 'CustomDLDataFolder' in extra_comps:
                 extra_comps = extra_comps.replace(
                     'CustomDLDataFolder', custom_dl_file_path
                 )
 
             component_db += [
@@ -877,16 +897,16 @@
         # prepare additional fragility data
 
         # get the database header from the default P58 db
         P58_data = PAL.get_default_data('damage_DB_FEMA_P58_2nd')
 
         adf = pd.DataFrame(columns=P58_data.columns)
 
-        if 'CollapseFragility' in damage_config.keys():
-            coll_config = damage_config['CollapseFragility']
+        if 'CollapseFragility' in config['DL']['Damage'].keys():
+            coll_config = config['DL']['Damage']['CollapseFragility']
 
             if 'excessive.coll.DEM' in cmp_marginals.index:
                 # if there is story-specific evaluation
                 coll_CMP_name = 'excessive.coll.DEM'
             else:
                 # otherwise, for global collapse evaluation
                 coll_CMP_name = 'collapse'
@@ -910,17 +930,17 @@
             if coll_DEM_name is None:
                 return -1
 
             if coll_DEM_spec is None:
                 adf.loc[coll_CMP_name, ('Demand', 'Type')] = coll_DEM_name
 
             else:
-                adf.loc[
-                    coll_CMP_name, ('Demand', 'Type')
-                ] = f'{coll_DEM_name}|{coll_DEM_spec}'
+                adf.loc[coll_CMP_name, ('Demand', 'Type')] = (
+                    f'{coll_DEM_name}|{coll_DEM_spec}'
+                )
 
             coll_DEM_unit = add_units(
                 pd.DataFrame(
                     columns=[
                         f'{coll_DEM}-1-1',
                     ]
                 ),
@@ -950,35 +970,35 @@
                 adf.loc['collapse', ('Demand', 'Directional')] = 1
                 adf.loc['collapse', ('Demand', 'Offset')] = 0
                 adf.loc['collapse', ('Demand', 'Type')] = 'One'
                 adf.loc['collapse', ('Demand', 'Unit')] = 'unitless'
                 adf.loc['collapse', ('LS1', 'Theta_0')] = 1e10
                 adf.loc['collapse', 'Incomplete'] = 0
 
-        elif "Water" not in asset_config['ComponentDatabase']:
+        elif "Water" not in config['DL']['Asset']['ComponentDatabase']:
             # add a placeholder collapse fragility that will never trigger
             # collapse, but allow damage processes to work with collapse
 
             adf.loc['collapse', ('Demand', 'Directional')] = 1
             adf.loc['collapse', ('Demand', 'Offset')] = 0
             adf.loc['collapse', ('Demand', 'Type')] = 'One'
             adf.loc['collapse', ('Demand', 'Unit')] = 'unitless'
             adf.loc['collapse', ('LS1', 'Theta_0')] = 1e10
             adf.loc['collapse', 'Incomplete'] = 0
 
-        if 'IrreparableDamage' in damage_config.keys():
-            irrep_config = damage_config['IrreparableDamage']
+        if 'IrreparableDamage' in config['DL']['Damage'].keys():
+            irrep_config = config['DL']['Damage']['IrreparableDamage']
 
             # add excessive RID fragility according to settings provided in the
             # input file
             adf.loc['excessiveRID', ('Demand', 'Directional')] = 1
             adf.loc['excessiveRID', ('Demand', 'Offset')] = 0
-            adf.loc[
-                'excessiveRID', ('Demand', 'Type')
-            ] = 'Residual Interstory Drift Ratio'
+            adf.loc['excessiveRID', ('Demand', 'Type')] = (
+                'Residual Interstory Drift Ratio'
+            )
 
             adf.loc['excessiveRID', ('Demand', 'Unit')] = 'unitless'
             adf.loc['excessiveRID', ('LS1', 'Theta_0')] = irrep_config[
                 'DriftCapacityMedian'
             ]
 
             adf.loc['excessiveRID', ('LS1', 'Family')] = "lognormal"
@@ -996,32 +1016,32 @@
             adf.loc['irreparable', ('Demand', 'Type')] = 'One'
             adf.loc['irreparable', ('Demand', 'Unit')] = 'unitless'
             adf.loc['irreparable', ('LS1', 'Theta_0')] = 1e10
             adf.loc['irreparable', 'Incomplete'] = 0
 
         # TODO: we can improve this by creating a water
         # network-specific assessment class
-        if "Water" in asset_config['ComponentDatabase']:
-
+        if "Water" in config['DL']['Asset']['ComponentDatabase']:
             # add a placeholder aggregate fragility that will never trigger
             # damage, but allow damage processes to aggregate the
             # various pipeline damages
             adf.loc['aggregate', ('Demand', 'Directional')] = 1
             adf.loc['aggregate', ('Demand', 'Offset')] = 0
             adf.loc['aggregate', ('Demand', 'Type')] = 'Peak Ground Velocity'
             adf.loc['aggregate', ('Demand', 'Unit')] = 'mps'
             adf.loc['aggregate', ('LS1', 'Theta_0')] = 1e10
+            adf.loc['aggregate', ('LS2', 'Theta_0')] = 1e10
             adf.loc['aggregate', 'Incomplete'] = 0
 
         PAL.damage.load_damage_model(component_db + [adf])
 
         # load the damage process if needed
         dmg_process = None
-        if damage_config.get('DamageProcess', False) is not False:
-            dp_approach = damage_config['DamageProcess']
+        if config['DL']['Damage'].get('DamageProcess', False) is not False:
+            dp_approach = config['DL']['Damage']['DamageProcess']
 
             if dp_approach in damage_processes:
                 dmg_process = damage_processes[dp_approach]
 
                 # For Hazus Earthquake, we need to specify the component ids
                 if dp_approach == 'Hazus Earthquake':
                     cmp_sample = PAL.asset.save_cmp_sample()
@@ -1079,37 +1099,39 @@
                             new_dmg_process[new_source][ds_i] = new_target_vals
 
                     dmg_process = new_dmg_process
 
             elif dp_approach == "User Defined":
                 # load the damage process from a file
                 with open(
-                    damage_config['DamageProcessFilePath'], 'r', encoding='utf-8'
+                    config['DL']['Damage']['DamageProcessFilePath'],
+                    'r',
+                    encoding='utf-8',
                 ) as f:
                     dmg_process = json.load(f)
 
             elif dp_approach == "None":
                 # no damage process applied for the calculation
                 dmg_process = None
 
             else:
                 log_msg(
                     f"Prescribed Damage Process not recognized: " f"{dp_approach}"
                 )
 
         # calculate damages
-        PAL.damage.calculate(dmg_process=dmg_process)
+        PAL.damage.calculate(sample_size, dmg_process=dmg_process)
 
         # if requested, save results
-        if out_config.get('Damage', None) is not None:
+        if 'Damage' in config['DL']['Outputs']:
             damage_sample, damage_units = PAL.damage.save_sample(save_units=True)
             damage_units = damage_units.to_frame().T
 
             if (
-                out_config['Settings'].get(
+                config['DL']['Outputs']['Settings'].get(
                     'AggregateColocatedComponentResults', False
                 )
                 is True
             ):
                 damage_units = damage_units.groupby(
                     level=[0, 1, 2, 4], axis=1
                 ).first()
@@ -1119,15 +1141,16 @@
                 )
 
                 damage_sample = damage_groupby_uid.sum().mask(
                     damage_groupby_uid.count() == 0, np.nan
                 )
 
             out_reqs = [
-                out if val else "" for out, val in out_config['Damage'].items()
+                out if val else ""
+                for out, val in config['DL']['Outputs']['Damage'].items()
             ]
 
             if np.any(
                 np.isin(
                     ['Sample', 'Statistics', 'GroupedSample', 'GroupedStatistics'],
                     out_reqs,
                 )
@@ -1154,15 +1177,15 @@
                         output_path / "DMG_stats.csv",
                         index_label=damage_stats.columns.name,
                     )
                     output_files.append('DMG_stats.csv')
 
                 if np.any(np.isin(['GroupedSample', 'GroupedStatistics'], out_reqs)):
                     if (
-                        out_config['Settings'].get(
+                        config['DL']['Outputs']['Settings'].get(
                             'AggregateColocatedComponentResults', False
                         )
                         is True
                     ):
                         damage_groupby = damage_sample.groupby(
                             level=[0, 1, 3], axis=1
                         )
@@ -1181,15 +1204,18 @@
                         ).first()
 
                     grp_damage = damage_groupby.sum().mask(
                         damage_groupby.count() == 0, np.nan
                     )
 
                     # if requested, condense DS output
-                    if out_config['Settings'].get('CondenseDS', False) is True:
+                    if (
+                        config['DL']['Outputs']['Settings'].get('CondenseDS', False)
+                        is True
+                    ):
                         # replace non-zero values with 1
                         grp_damage = grp_damage.mask(
                             grp_damage.astype(np.float64).values > 0, 1
                         )
 
                         # get the corresponding DS for each column
                         ds_list = grp_damage.columns.get_level_values(2).astype(int)
@@ -1273,46 +1299,39 @@
                 output_files.append('DM.csv')
             """
             # - - - - -
 
     # Loss Assessment -----------------------------------------------------------
 
     # if a loss assessment is requested
-    if loss_config is not None:
-        out_config_loss = out_config.get('Loss', {})
+    if 'Losses' in config['DL']:
+        out_config_loss = config['DL']['Outputs'].get('Loss', {})
 
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         # backwards-compatibility for v3.2 and earlier | remove after v4.0
-        if loss_config.get('BldgRepair', False):
-            loss_config['Repair'] = loss_config['BldgRepair']
+        if config['DL']['Losses'].get('BldgRepair', False):
+            config['DL']['Losses']['Repair'] = config['DL']['Losses']['BldgRepair']
 
         if out_config_loss.get('BldgRepair', False):
             out_config_loss['Repair'] = out_config_loss['BldgRepair']
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         # if requested, calculate repair consequences
-        if loss_config.get('Repair', False):
-            repair_config = loss_config['Repair']
+        if config['DL']['Losses'].get('Repair', False):
+            repair_config = config['DL']['Losses']['Repair']
 
             # load the fragility information
-            if (
-                repair_config['ConsequenceDatabase']
-                in default_DBs['repair'].keys()
-            ):
+            if repair_config['ConsequenceDatabase'] in default_DBs['repair'].keys():
                 consequence_db = [
                     'PelicunDefault/'
-                    + default_DBs['repair'][
-                        repair_config['ConsequenceDatabase']
-                    ],
+                    + default_DBs['repair'][repair_config['ConsequenceDatabase']],
                 ]
 
                 conseq_df = PAL.get_default_data(
-                    default_DBs['repair'][repair_config['ConsequenceDatabase']][
-                        :-4
-                    ]
+                    default_DBs['repair'][repair_config['ConsequenceDatabase']][:-4]
                 )
             else:
                 consequence_db = []
 
                 conseq_df = pd.DataFrame()
 
             if repair_config.get('ConsequenceDatabasePath', False) is not False:
@@ -1354,15 +1373,15 @@
                         ('replacement', 'Carbon'),
                         ('replacement', 'Energy'),
                     ]
                 ),
             )
 
             # DL_method = repair_config['ConsequenceDatabase']
-            DL_method = damage_config.get('DamageProcess', 'User Defined')
+            DL_method = config['DL']['Damage'].get('DamageProcess', 'User Defined')
 
             rc = ('replacement', 'Cost')
             if 'ReplacementCost' in repair_config.keys():
                 rCost_config = repair_config['ReplacementCost']
 
                 adf.loc[rc, ('Quantity', 'Unit')] = "1 EA"
 
@@ -1424,15 +1443,15 @@
 
                 # for Hazus EQ, use 1.0 as a loss_ratio
                 elif DL_method == 'Hazus Earthquake - Buildings':
                     adf.loc[rt, ('Quantity', 'Unit')] = '1 EA'
                     adf.loc[rt, ('DV', 'Unit')] = 'day'
 
                     # load the replacement time that corresponds to total loss
-                    occ_type = asset_config['OccupancyType']
+                    occ_type = config['DL']['Asset']['OccupancyType']
                     adf.loc[rt, ('DS1', 'Theta_0')] = conseq_df.loc[
                         (f"STR.{occ_type}", 'Time'), ('DS5', 'Theta_0')
                     ]
 
                 # otherwise, use 1 (and expect to have it defined by the user)
                 else:
                     adf.loc[rt, ('Quantity', 'Unit')] = '1 EA'
@@ -1525,15 +1544,15 @@
 
                 elif DL_method in [
                     'Hazus Earthquake',
                     'Hazus Earthquake Transportation',
                 ]:
                     # with Hazus Earthquake we assume that consequence
                     # archetypes are only differentiated by occupancy type
-                    occ_type = asset_config.get('OccupancyType', None)
+                    occ_type = config['DL']['Asset'].get('OccupancyType', None)
 
                     for dmg_cmp in dmg_cmps:
                         if dmg_cmp == 'collapse':
                             continue
 
                         cmp_class = dmg_cmp.split('.')[0]
                         if occ_type is not None:
@@ -1546,20 +1565,20 @@
                             loss_models.append(loss_cmp)
 
                 loss_map = pd.DataFrame(
                     loss_models, columns=['Repair'], index=drivers
                 )
 
             elif repair_config['MapApproach'] == "User Defined":
-
                 if repair_config.get('MapFilePath', False) is not False:
                     loss_map_path = repair_config['MapFilePath']
 
                     loss_map_path = loss_map_path.replace(
-                        'CustomDLDataFolder', custom_dl_file_path)
+                        'CustomDLDataFolder', custom_dl_file_path
+                    )
 
                 else:
                     print("User defined loss map path missing. Terminating analysis")
                     return -1
 
                 loss_map = pd.read_csv(loss_map_path, index_col=0)
 
@@ -1567,17 +1586,15 @@
             if 'DMG-collapse' not in loss_map.index:
                 loss_map.loc['DMG-collapse', 'Repair'] = 'replacement'
                 loss_map.loc['DMG-irreparable', 'Repair'] = 'replacement'
 
             # assemble the list of requested decision variables
             DV_list = []
             if repair_config.get('DecisionVariables', False) is not False:
-                for DV_i, DV_status in repair_config[
-                    'DecisionVariables'
-                ].items():
+                for DV_i, DV_status in repair_config['DecisionVariables'].items():
                     if DV_status is True:
                         DV_list.append(DV_i)
 
             else:
                 DV_list = None
 
             PAL.repair.load_model(
@@ -1585,27 +1602,25 @@
                 + [
                     adf,
                 ],
                 loss_map,
                 decision_variables=DV_list,
             )
 
-            PAL.repair.calculate()
+            PAL.repair.calculate(sample_size)
 
             agg_repair = PAL.repair.aggregate_losses()
-    
+
             # if requested, save results
             if out_config_loss.get('Repair', False):
-                repair_sample, repair_units = PAL.repair.save_sample(
-                    save_units=True
-                )
+                repair_sample, repair_units = PAL.repair.save_sample(save_units=True)
                 repair_units = repair_units.to_frame().T
 
                 if (
-                    out_config['Settings'].get(
+                    config['DL']['Outputs']['Settings'].get(
                         'AggregateColocatedComponentResults', False
                     )
                     is True
                 ):
                     repair_units = repair_units.groupby(
                         level=[0, 1, 2, 3, 4, 5], axis=1
                     ).first()
@@ -1745,23 +1760,21 @@
         damage_sample_s['collapse'] = np.zeros(damage_sample_s.shape[0])
 
     if 'irreparable-1' in damage_sample_s.columns:
         damage_sample_s['irreparable'] = damage_sample_s['irreparable-1']
     else:
         damage_sample_s['irreparable'] = np.zeros(damage_sample_s.shape[0])
 
-    if loss_config is not None:
-
+    if 'Losses' in config['DL']:
         if 'agg_repair' not in locals():
             agg_repair = PAL.repair.aggregate_losses()
 
         agg_repair_s = convert_to_SimpleIndex(agg_repair, axis=1)
 
     else:
-
         agg_repair_s = pd.DataFrame()
 
     summary = pd.concat(
         [agg_repair_s, damage_sample_s[['collapse', 'irreparable']]], axis=1
     )
 
     summary_stats = describe(summary)
@@ -1771,19 +1784,22 @@
     output_files.append('DL_summary.csv')
 
     # save summary statistics
     summary_stats.to_csv(output_path / "DL_summary_stats.csv")
     output_files.append('DL_summary_stats.csv')
 
     # create json outputs if needed
-    if out_config['Format']['JSON'] is True:
+    if config['DL']['Outputs']['Format']['JSON'] is True:
         for filename in output_files:
             filename_json = filename[:-3] + 'json'
 
-            if out_config['Settings'].get('SimpleIndexInJSON', False) is True:
+            if (
+                config['DL']['Outputs']['Settings'].get('SimpleIndexInJSON', False)
+                is True
+            ):
                 df = pd.read_csv(output_path / filename, index_col=0)
             else:
                 df = convert_to_MultiIndex(
                     pd.read_csv(output_path / filename, index_col=0), axis=1
                 )
 
             if "Units" in df.index:
@@ -1807,27 +1823,26 @@
             else:
                 out_dict = convert_df_to_dict(df)
 
             with open(output_path / filename_json, 'w') as f:
                 json.dump(out_dict, f, indent=2)
 
     # remove csv outputs if they were not requested
-    if out_config['Format']['CSV'] is False:
+    if config['DL']['Outputs']['Format']['CSV'] is False:
         for filename in output_files:
             # keep the DL_summary and DL_summary_stats files
             if 'DL_summary' in filename:
                 continue
 
             os.remove(output_path / filename)
 
     return 0
 
 
 def main():
-
     args = sys.argv[1:]
 
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--filenameDL')
     parser.add_argument('-d', '--demandFile', default=None)
     parser.add_argument('-s', '--Realizations', default=None)
     parser.add_argument('--dirnameOutput', default=None)
```

### Comparing `pelicun-3.3.2/pelicun/tools/HDF_to_CSV.py` & `pelicun-3.3.3/pelicun/tools/HDF_to_CSV.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,31 +40,28 @@
 import pandas as pd
 import sys
 import argparse
 from pathlib import Path
 
 
 def convert_HDF(HDF_path):
-
     HDF_ext = HDF_path.split('.')[-1]
-    CSV_base = HDF_path[:-len(HDF_ext) - 1]
+    CSV_base = HDF_path[: -len(HDF_ext) - 1]
 
     HDF_path = Path(HDF_path).resolve()
 
     store = pd.HDFStore(HDF_path)
 
     for key in store.keys():
-
         store[key].to_csv(f'{CSV_base}_{key[1:].replace("/","_")}.csv')
 
     store.close()
 
 
 if __name__ == '__main__':
-
     args = sys.argv[1:]
 
     parser = argparse.ArgumentParser()
     parser.add_argument('HDF_path')
 
     args = parser.parse_args(args)
```

### Comparing `pelicun-3.3.2/pelicun/tools/export_DB.py` & `pelicun-3.3.3/pelicun/tools/export_DB.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,43 +55,37 @@
 
     target_dir_data = target_dir / 'data'
     target_dir_data.mkdir(exist_ok=True)
 
     DB_df = pd.read_hdf(data_path, 'data')
 
     for row_id, row in DB_df.iterrows():
-
         row_dict = convert_Series_to_dict(row)
 
-        with open(target_dir_data / f'{row_id}.json', 'w',
-                  encoding='utf-8') as f:
+        with open(target_dir_data / f'{row_id}.json', 'w', encoding='utf-8') as f:
             json.dump(row_dict, f, indent=2)
 
     # add population if it exists
 
     try:
-
         DB_df = pd.read_hdf(data_path, 'pop')
 
         pop_dict = {}
 
         for row_id, row in DB_df.iterrows():
-
             pop_dict.update({row_id: convert_Series_to_dict(row)})
 
-        with open(target_dir / 'population.json', 'w',
-                  encoding='utf-8') as f:
+        with open(target_dir / 'population.json', 'w', encoding='utf-8') as f:
             json.dump(pop_dict, f, indent=2)
 
     except (ValueError, NotImplementedError, FileNotFoundError):
         pass
 
 
 if __name__ == '__main__':
-
     args = sys.argv[1:]
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--DL_DB_path')
     parser.add_argument('--target_dir')
 
     args_namespace = parser.parse_args(args)
```

### Comparing `pelicun-3.3.2/pelicun/uq.py` & `pelicun-3.3.3/pelicun/uq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1201,15 +1201,15 @@
         value: float ndarray
             An array of floating point values in the [0, 1] domain.
 
         """
         self._uni_samples = value
 
 
-class CommonRandomVariable(BaseRandomVariable):
+class RandomVariable(BaseRandomVariable):
     """
     Random variable that needs `values` in `inverse_transform`
     """
 
     @abstractmethod
     def __init__(
         self,
@@ -1269,33 +1269,33 @@
           If there is no available uniform sample.
         """
         if self.uni_sample is None:
             raise ValueError('No available uniform sample.')
         self.sample = self.inverse_transform(self.uni_sample)
 
 
-class SampleSizeRandomVariable(BaseRandomVariable):
+class UtilityRandomVariable(BaseRandomVariable):
     """
     Random variable that needs `sample_size` in `inverse_transform`
     """
 
     @abstractmethod
     def __init__(
         self,
-        name,        
+        name,
         f_map=None,
         anchor=None,
     ):
         """
         Instantiates a normal random variable.
 
         Parameters
         ----------
         name: string
-            A unique string that identifies the random variable.        
+            A unique string that identifies the random variable.
         f_map: function, optional
             A user-defined function that is applied on the realizations before
             returning a sample.
         anchor: RandomVariable, optional
             Anchors this to another variable. If the anchor is not None, this
             variable will be perfectly correlated with its anchor. Note that
             the attributes of this variable and its anchor do not have to be
@@ -1320,15 +1320,15 @@
         """
         Creates a sample using inverse probability integral
         transformation.
         """
         self.sample = self.inverse_transform(sample_size)
 
 
-class NormalRandomVariable(CommonRandomVariable):
+class NormalRandomVariable(RandomVariable):
     """
     Normal random variable.
 
     """
 
     def __init__(
         self,
@@ -1442,15 +1442,15 @@
 
         else:
             result = norm.ppf(values, loc=mu, scale=sig)
 
         return result
 
 
-class LogNormalRandomVariable(CommonRandomVariable):
+class LogNormalRandomVariable(RandomVariable):
     """
     Lognormal random variable.
 
     """
 
     def __init__(
         self,
@@ -1558,15 +1558,15 @@
 
         else:
             result = np.exp(norm.ppf(values, loc=np.log(theta), scale=beta))
 
         return result
 
 
-class UniformRandomVariable(CommonRandomVariable):
+class UniformRandomVariable(RandomVariable):
     """
     Uniform random variable.
 
     """
 
     def __init__(
         self,
@@ -1645,15 +1645,15 @@
             a, b = self.truncation_limits
 
         result = uniform.ppf(values, loc=a, scale=(b - a))
 
         return result
 
 
-class MultilinearCDFRandomVariable(CommonRandomVariable):
+class MultilinearCDFRandomVariable(RandomVariable):
     """
     Multilinear CDF random variable. This RV is defined by specifying
     the points that define its Cumulative Density Function (CDF), and
     linear interpolation between them.
 
     """
 
@@ -1770,32 +1770,32 @@
         # note: swapping the roles of x_i and y_i for inverse
         # interpolation
         result = np.interp(values, y_i, x_i)
 
         return result
 
 
-class EmpiricalRandomVariable(CommonRandomVariable):
+class EmpiricalRandomVariable(RandomVariable):
     """
     Empirical random variable.
 
     """
 
     def __init__(
         self,
         name,
         raw_samples,
         truncation_limits=np.array((np.nan, np.nan)),
         f_map=None,
         anchor=None,
     ):
         super().__init__(
-            name=name, 
+            name=name,
             theta=raw_samples,
-            truncation_limits=truncation_limits,           
+            truncation_limits=truncation_limits,
             f_map=f_map,
             anchor=anchor,
         )
         self.distribution = 'empirical'
         if not np.all(np.isnan(truncation_limits)):
             raise NotImplementedError(
                 f'{self.distribution} RVs do not support truncation'
@@ -1825,15 +1825,15 @@
 
         """
         s_ids = (values * len(self._raw_samples)).astype(int)
         result = self._raw_samples[s_ids]
         return result
 
 
-class CoupledEmpiricalRandomVariable(SampleSizeRandomVariable):
+class CoupledEmpiricalRandomVariable(UtilityRandomVariable):
     """
     Coupled empirical random variable.
 
     """
 
     def __init__(
         self,
@@ -1902,22 +1902,20 @@
         ndarray
           A new sample array derived from repeating the original
           dataset.
 
         """
 
         raw_sample_count = len(self._raw_samples)
-        new_sample = np.tile(
-            self._raw_samples, int(sample_size / raw_sample_count) + 1
-        )
+        new_sample = np.tile(self._raw_samples, int(sample_size / raw_sample_count) + 1)
         result = new_sample[:sample_size]
         return result
 
 
-class DeterministicRandomVariable(SampleSizeRandomVariable):
+class DeterministicRandomVariable(UtilityRandomVariable):
     """
     Deterministic random variable.
 
     """
 
     def __init__(
         self,
@@ -1985,15 +1983,15 @@
 
         """
 
         result = np.full(sample_size, self.theta[0])
         return result
 
 
-class MultinomialRandomVariable(CommonRandomVariable):
+class MultinomialRandomVariable(RandomVariable):
     """
     Multinomial random variable.
 
     """
 
     def __init__(
         self,
@@ -2426,19 +2424,19 @@
         # Apply correlations for the pre-defined RV sets
         for RV_set in self.RV_set.values():
             # prepare the correlated uniform distribution for the set
             RV_set.apply_correlation()
 
         # Convert from uniform to the target distribution for every RV
         for RV in self.RV.values():
-            if RV.__class__.__mro__[1] is CommonRandomVariable:
+            if RV.__class__.__mro__[1] is RandomVariable:
                 # no sample size needed, since that information is
                 # available in the uniform sample
                 RV.inverse_transform_sampling()
-            elif RV.__class__.__mro__[1] is SampleSizeRandomVariable:
+            elif RV.__class__.__mro__[1] is UtilityRandomVariable:
                 RV.inverse_transform_sampling(sample_size)
             else:
                 raise NotImplementedError('Unknown RV parent class.')
 
 
 def rv_class_map(distribution_name):
     """
```

### Comparing `pelicun-3.3.2/pelicun.egg-info/PKG-INFO` & `pelicun-3.3.3/pelicun.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelicun
-Version: 3.3.2
+Version: 3.3.3
 Summary: Probabilistic Estimation of Losses, Injuries, and Community resilience Under Natural hazard events
 Home-page: http://nheri-simcenter.github.io/pelicun/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
@@ -24,16 +24,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<2.0,>=1.22.0
 Requires-Dist: scipy<2.0,>=1.7.0
 Requires-Dist: pandas<3.0,>=1.4.0
-Provides-Extra: testing
-Requires-Dist: pytest; extra == "testing"
+Provides-Extra: development
+Requires-Dist: flake8; extra == "development"
+Requires-Dist: pylint; extra == "development"
+Requires-Dist: black; extra == "development"
+Requires-Dist: pytest; extra == "development"
+Requires-Dist: pytest-cov; extra == "development"
+Requires-Dist: glob2; extra == "development"
+Requires-Dist: jupyter; extra == "development"
+Requires-Dist: jupytext; extra == "development"
+Requires-Dist: sphinx; extra == "development"
+Requires-Dist: sphinx-autoapi; extra == "development"
+Requires-Dist: nbsphinx; extra == "development"
+Requires-Dist: flake8-rst; extra == "development"
+Requires-Dist: flake8-rst-docstrings; extra == "development"
 
 <p align="center">
 	<img src="https://raw.githubusercontent.com/NHERI-SimCenter/pelicun/gh-pages/doc_src/common/figures/pelicun-Logo-white.png"
 		alt="pelicun" align="middle" height="200"/>
 </p>
 
 <p align="center">
@@ -102,18 +114,15 @@
 git clone https://github.com/<user>/pelicun
 cd pelicun
 # Switch to the appropriate branch, if needed.
 # git checkout <branch>
 
 # Install pelicun:
 # Note: don't forget to activate the corresponding environment.
-python -m pip install -e .
-
-# Install additional development setup dependencies
-python -m pip install -r requirements_dev.txt
+python -m pip install -e .[development]
 
 ```
 
 Contributions are managed with pull requests.
 It is required that contributed code is [PEP 8](https://peps.python.org/pep-0008/) compliant, does not introduce linter warnings and includes sufficient unit tests so as to avoid reducing the current coverage level.
 
 The following lines implement the aforementioned checks.
```

#### html2text {}

```diff
@@ -1,24 +1,32 @@
-Metadata-Version: 2.1 Name: pelicun Version: 3.3.2 Summary: Probabilistic
+Metadata-Version: 2.1 Name: pelicun Version: 3.3.3 Summary: Probabilistic
 Estimation of Losses, Injuries, and Community resilience Under Natural hazard
 events Home-page: http://nheri-simcenter.github.io/pelicun/ Author: Adam
 ZsarnÃ³czay Author-email: adamzs@stanford.edu License: BSD License Platform:
 any Classifier: Programming Language :: Python Classifier: Development Status
 :: 5 - Production/Stable Classifier: Natural Language :: English Classifier:
 Environment :: Console Classifier: Framework :: Jupyter Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
 :: English Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy<2.0,>=1.22.0 Requires-Dist:
-scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Provides-Extra: testing
-Requires-Dist: pytest; extra == "testing"
+scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Provides-Extra: development
+Requires-Dist: flake8; extra == "development" Requires-Dist: pylint; extra ==
+"development" Requires-Dist: black; extra == "development" Requires-Dist:
+pytest; extra == "development" Requires-Dist: pytest-cov; extra ==
+"development" Requires-Dist: glob2; extra == "development" Requires-Dist:
+jupyter; extra == "development" Requires-Dist: jupytext; extra == "development"
+Requires-Dist: sphinx; extra == "development" Requires-Dist: sphinx-autoapi;
+extra == "development" Requires-Dist: nbsphinx; extra == "development"
+Requires-Dist: flake8-rst; extra == "development" Requires-Dist: flake8-rst-
+docstrings; extra == "development"
                                    [pelicun]
       alt="DOI">[https://zenodo.org/badge/DOI/10.5281/zenodo.2558558.svg]
  PPrroobbaabbiilliissttiicc EEssttiimmaattiioonn ooff LLoosssseess,, IInnjjuurriieess,, aanndd CCoommmmuunniittyy rreessiilliieennccee UUnnddeerr
                              NNaattuurraall hhaazzaarrdd eevveennttss
 ![Tests](https://github.com/NHERI-SimCenter/pelicun/actions/workflows/
 tests.yml/badge.svg) [![codecov](https://codecov.io/github/NHERI-SimCenter/
 pelicun/branch/master/graph/badge.svg?token=W79M5FGOCG)](https://codecov.io/
@@ -73,30 +81,29 @@
 pelicun==2.6.0 ``` Note that 2.6.0 is the last minor version before the v3.0
 release. Other earlier versions can be found [here](https://pypi.org/project/
 pelicun/#history). ### For contributors Developers are expected to fork and
 clone this repository, and install their copy in development mode. Using a
 virtual environment is highly recommended. ```shell # Clone the repository: git
 clone https://github.com//pelicun cd pelicun # Switch to the appropriate
 branch, if needed. # git checkout # Install pelicun: # Note: don't forget to
-activate the corresponding environment. python -m pip install -e . # Install
-additional development setup dependencies python -m pip install -
-r requirements_dev.txt ``` Contributions are managed with pull requests. It is
-required that contributed code is [PEP 8](https://peps.python.org/pep-0008/
-) compliant, does not introduce linter warnings and includes sufficient unit
-tests so as to avoid reducing the current coverage level. The following lines
-implement the aforementioned checks. `flake8`, `pylint` and `pytest` can all be
-configured for use within an IDE. ```shell cd /pelicun export
-PYTHONPATH=$PYTHONPATH:$(pwd) # Linting with flake8: flake8 pelicun # Linting
-with pylint: pylint pelicun # Running the tests: python -m pytest pelicun/tests
---cov=pelicun --cov-report html # Open `htmlcov/index.html`in a browser to see
-coverage results. ``` Feel free to [open an issue](https://github.com/NHERI-
-SimCenter/pelicun/issues/new/choose) if you encounter problems setting up the
-provided development environment. ## Changelog ### Changes in v3.3 - Changes
-affecting backwards compatibility - **Remove "bldg" from repair consequence
-output filenames**: The increasing scope of Pelicun now covers simulations for
+activate the corresponding environment. python -m pip install -e .[development]
+``` Contributions are managed with pull requests. It is required that
+contributed code is [PEP 8](https://peps.python.org/pep-0008/) compliant, does
+not introduce linter warnings and includes sufficient unit tests so as to avoid
+reducing the current coverage level. The following lines implement the
+aforementioned checks. `flake8`, `pylint` and `pytest` can all be configured
+for use within an IDE. ```shell cd /pelicun export PYTHONPATH=$PYTHONPATH:$
+(pwd) # Linting with flake8: flake8 pelicun # Linting with pylint: pylint
+pelicun # Running the tests: python -m pytest pelicun/tests --cov=pelicun --
+cov-report html # Open `htmlcov/index.html`in a browser to see coverage
+results. ``` Feel free to [open an issue](https://github.com/NHERI-SimCenter/
+pelicun/issues/new/choose) if you encounter problems setting up the provided
+development environment. ## Changelog ### Changes in v3.3 - Changes affecting
+backwards compatibility - **Remove "bldg" from repair consequence output
+filenames**: The increasing scope of Pelicun now covers simulations for
 transportation and water networks. Hence, labeling repair consequence outputs
 as if they were limited to buildings no longer seems appropriate. The `bldg`
 label was dropped from the following files:
 `DV_bldg_repair_sample`,`DV_bldg_repair_stats`,`DV_bldg_repair_grp`,
 `DV_bldg_repair_grp_stats`, `DV_bldg_repair_agg`, `DV_bldg_repair_agg_stats`. -
 Deprecation warnings - **Remove `Bldg` from repair settings label in DL
 configuration file**: Following the changes above, we dropped `Bldg` from
```

### Comparing `pelicun-3.3.2/pelicun.egg-info/SOURCES.txt` & `pelicun-3.3.3/pelicun.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json
 pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv
 pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json
 pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv
 pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv
 pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json
 pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv
+pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg_template.json
 pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv
 pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json
 pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv
 pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json
 pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv
 pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json
 pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.csv
```

### Comparing `pelicun-3.3.2/setup.py` & `pelicun-3.3.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,31 @@
     platforms='any',
     install_requires=[
         'numpy>=1.22.0, <2.0',
         'scipy>=1.7.0, <2.0',
         'pandas>=1.4.0, <3.0',
         #'tables>=3.7.0',
     ],
+    extras_require={
+        'development': [
+            'flake8',
+            'pylint',
+            'black',
+            'pytest',
+            'pytest-cov',
+            'glob2',
+            'jupyter',
+            'jupytext',
+            'sphinx',
+            'sphinx-autoapi',
+            'nbsphinx',
+            'flake8-rst',
+            'flake8-rst-docstrings',
+        ],
+    },
     classifiers=[
         'Programming Language :: Python',
         'Development Status :: 5 - Production/Stable',
         'Natural Language :: English',
         'Environment :: Console',
         'Framework :: Jupyter',
         'Intended Audience :: Education',
@@ -61,16 +78,13 @@
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering',
     ],
-    extras_require={
-        'testing': ['pytest'],
-    },
     entry_points={
         'console_scripts': [
             'pelicun = pelicun.tools.DL_calculation:main',
         ]
     },
 )
```

