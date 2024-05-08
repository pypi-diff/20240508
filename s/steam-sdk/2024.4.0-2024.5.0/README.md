# Comparing `tmp/steam-sdk-2024.4.0.tar.gz` & `tmp/steam-sdk-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-sdk-2024.4.0.tar", last modified: Tue Apr 30 14:36:32 2024, max compression
+gzip compressed data, was "steam-sdk-2024.5.0.tar", last modified: Wed May  8 15:36:08 2024, max compression
```

## Comparing `steam-sdk-2024.4.0.tar` & `steam-sdk-2024.5.0.tar`

### file list

```diff
@@ -1,209 +1,211 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.730771 steam-sdk-2024.4.0/
--rw-rw-rw-   0        0        0      264 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5753 2024-04-30 14:36:32.728771 steam-sdk-2024.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-30 14:36:32.730771 steam-sdk-2024.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1668 2024-04-30 14:29:21.000000 steam-sdk-2024.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.390771 steam-sdk-2024.4.0/steam_sdk/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.411770 steam-sdk-2024.4.0/steam_sdk/analyses/
--rw-rw-rw-   0        0        0    37589 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisEvent.py
--rw-rw-rw-   0        0        0    30954 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisEventLHC.py
--rw-rw-rw-   0        0        0   133599 2024-04-30 14:35:01.000000 steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.418774 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.419771 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23388 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.436769 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16777 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2820 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6761 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95432 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2672 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2361 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.440770 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22357 2024-04-11 12:40:24.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.446769 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4450 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2844 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.449770 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29436 2024-04-11 12:41:03.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.456771 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4627 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4775 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.459771 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.480772 steam-sdk-2024.4.0/steam_sdk/builders/
--rw-rw-rw-   0        0        0    13175 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderAPDL_CT.py
--rw-rw-rw-   0        0        0     4805 2024-03-22 11:40:47.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderCosim.py
--rw-rw-rw-   0        0        0    17741 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   160440 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    53922 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12487 2024-04-11 12:01:36.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderPySIGMA.py
--rw-rw-rw-   0        0        0    56494 2024-04-30 14:26:16.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderTFM.py
--rw-rw-rw-   0        0        0    11689 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.482772 steam-sdk-2024.4.0/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.485771 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.486771 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     1426 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.494770 steam-sdk-2024.4.0/steam_sdk/cosims/
--rw-rw-rw-   0        0        0    26984 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/cosims/CoSimPyCoSim.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.567773 steam-sdk-2024.4.0/steam_sdk/data/
--rw-rw-rw-   0        0        0     1684 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataAPDLCTOptions.py
--rw-rw-rw-   0        0        0    12969 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0      414 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DataCoSim.py
--rw-rw-rw-   0        0        0     9303 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0      308 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2987 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4636 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0    86916 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0     7309 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataFiQuSOptions.py
--rw-rw-rw-   0        0        0    16769 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     9528 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataLEDETOptions.py
--rw-rw-rw-   0        0        0     5377 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5216 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelCommon.py
--rw-rw-rw-   0        0        0     6621 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    12150 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelCosim.py
--rw-rw-rw-   0        0        0     8020 2024-04-30 14:26:16.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     6491 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelParsimDakota.py
--rw-rw-rw-   0        0        0     3008 2024-04-08 08:37:58.000000 steam-sdk-2024.4.0/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0     2130 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2956 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataProteCCTOptions.py
--rw-rw-rw-   0        0        0     2595 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     1508 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPyBBQOptions.py
--rw-rw-rw-   0        0        0      766 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPyCoSim.py
--rw-rw-rw-   0        0        0     6552 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPySIGMA.py
--rw-rw-rw-   0        0        0     2228 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPySIGMAOptions.py
--rw-rw-rw-   0        0        0      236 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DataRoxieParams.py
--rw-rw-rw-   0        0        0     9824 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0    12404 2024-04-12 18:44:18.000000 steam-sdk-2024.4.0/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3263 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0     5926 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataTFM.py
--rw-rw-rw-   0        0        0    18457 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    30456 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.580771 steam-sdk-2024.4.0/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3739 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverANSYS.py
--rw-rw-rw-   0        0        0    13733 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     7448 2024-04-14 11:58:12.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     4278 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3573 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1894 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2275 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0      517 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverPySIGMA.py
--rw-rw-rw-   0        0        0     1983 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.617769 steam-sdk-2024.4.0/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      315 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0    14173 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCOSIM.py
--rw-rw-rw-   0        0        0     2290 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1024 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6302 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     2729 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     8536 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2614 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0     3760 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserFile.py
--rw-rw-rw-   0        0        0    30071 2024-04-30 14:35:01.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    18391 2024-04-30 14:35:01.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    15085 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    65009 2024-04-12 18:35:10.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4706 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6765 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     1758 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPyBBQ.py
--rw-rw-rw-   0        0        0     1663 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPyCoSim.py
--rw-rw-rw-   0        0        0     4061 2024-04-11 12:27:48.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPySIGMA.py
--rw-rw-rw-   0        0        0   155447 2024-04-15 21:11:35.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11746 2024-04-12 18:35:10.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    58167 2024-04-30 14:26:16.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     7770 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0      929 2024-03-22 11:40:47.000000 steam-sdk-2024.4.0/steam_sdk/parsers/utils_ParserCircuits.py
--rw-rw-rw-   0        0        0     9687 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/parsers/utils_ParserCosims.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.625769 steam-sdk-2024.4.0/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    66858 2024-04-15 21:11:35.000000 steam-sdk-2024.4.0/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0     4619 2024-04-14 11:38:50.000000 steam-sdk-2024.4.0/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    90102 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    48261 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.631770 steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/
--rw-rw-rw-   0        0        0     2351 2024-04-08 08:37:58.000000 steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
--rw-rw-rw-   0        0        0     2016 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/event_column_names.yaml
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.638769 steam-sdk-2024.4.0/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    29312 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0    20777 2024-04-30 14:35:01.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39519 2024-04-15 21:11:35.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0    13246 2024-03-26 07:52:01.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.640770 steam-sdk-2024.4.0/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0    11619 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.702769 steam-sdk-2024.4.0/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0      204 2024-04-15 21:11:35.000000 steam-sdk-2024.4.0/steam_sdk/utils/MatrixOperations.py
--rw-rw-rw-   0        0        0    15002 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     3201 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2770 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0     5730 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/ParserRoxieHelpers.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     5806 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/utils/attribute_model.py
--rw-rw-rw-   0        0        0      686 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0    12832 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/compare_simulations.py
--rw-rw-rw-   0        0        0     3837 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0     1650 2024-04-12 18:35:10.000000 steam-sdk-2024.4.0/steam_sdk/utils/correct_RRR_NIST.py
--rw-rw-rw-   0        0        0      227 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/delete_if_existing.py
--rw-rw-rw-   0        0        0     1204 2024-03-22 11:42:52.000000 steam-sdk-2024.4.0/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      691 2024-04-11 06:51:22.000000 steam-sdk-2024.4.0/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     3555 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0     1596 2024-04-13 18:58:31.000000 steam-sdk-2024.4.0/steam_sdk/utils/read_settings_file.py
--rw-rw-rw-   0        0        0     3365 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/reformat_figure.py
--rw-rw-rw-   0        0        0      388 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.704770 steam-sdk-2024.4.0/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    39140 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.709769 steam-sdk-2024.4.0/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.717770 steam-sdk-2024.4.0/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.718770 steam-sdk-2024.4.0/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.719770 steam-sdk-2024.4.0/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1830 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.720770 steam-sdk-2024.4.0/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     5753 2024-04-30 14:36:27.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7626 2024-04-30 14:36:28.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 14:36:27.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1745 2024-04-30 14:36:27.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-30 14:36:27.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.787967 steam-sdk-2024.5.0/
+-rw-rw-rw-   0        0        0      264 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5753 2024-05-08 15:36:08.786967 steam-sdk-2024.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:36:08.788967 steam-sdk-2024.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1668 2024-05-08 15:32:43.000000 steam-sdk-2024.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.311969 steam-sdk-2024.5.0/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.339968 steam-sdk-2024.5.0/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0    37589 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/analyses/AnalysisEvent.py
+-rw-rw-rw-   0        0        0    30954 2024-04-30 05:16:26.000000 steam-sdk-2024.5.0/steam_sdk/analyses/AnalysisEventLHC.py
+-rw-rw-rw-   0        0        0   134527 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.347968 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.350968 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23388 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.393968 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16777 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2820 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6761 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95432 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2672 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2361 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.397968 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22357 2024-04-11 12:40:24.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.404967 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4450 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2844 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.408967 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29436 2024-04-11 12:41:03.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.428968 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4627 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4775 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.432968 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.458967 steam-sdk-2024.5.0/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    13175 2024-03-21 12:26:24.000000 steam-sdk-2024.5.0/steam_sdk/builders/BuilderAPDL_CT.py
+-rw-rw-rw-   0        0        0     4805 2024-03-22 11:40:47.000000 steam-sdk-2024.5.0/steam_sdk/builders/BuilderCosim.py
+-rw-rw-rw-   0        0        0    17741 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   160440 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    53471 2024-05-08 10:58:22.000000 steam-sdk-2024.5.0/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12487 2024-04-11 12:01:36.000000 steam-sdk-2024.5.0/steam_sdk/builders/BuilderPySIGMA.py
+-rw-rw-rw-   0        0        0    57747 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/builders/BuilderTFM.py
+-rw-rw-rw-   0        0        0    11689 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.459968 steam-sdk-2024.5.0/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.461969 steam-sdk-2024.5.0/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.461969 steam-sdk-2024.5.0/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     1426 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.463968 steam-sdk-2024.5.0/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0    26984 2024-04-30 05:16:26.000000 steam-sdk-2024.5.0/steam_sdk/cosims/CoSimPyCoSim.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.577968 steam-sdk-2024.5.0/steam_sdk/data/
+-rw-rw-rw-   0        0        0     1684 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataAPDLCTOptions.py
+-rw-rw-rw-   0        0        0    13001 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0      414 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/data/DataCoSim.py
+-rw-rw-rw-   0        0        0     9303 2024-04-05 07:58:47.000000 steam-sdk-2024.5.0/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0      308 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2987 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4636 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    87445 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0     7309 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataFiQuSOptions.py
+-rw-rw-rw-   0        0        0    16769 2024-04-05 07:58:47.000000 steam-sdk-2024.5.0/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     9528 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataLEDETOptions.py
+-rw-rw-rw-   0        0        0     5377 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5216 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataModelCommon.py
+-rw-rw-rw-   0        0        0     6621 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    12150 2024-04-30 05:16:26.000000 steam-sdk-2024.5.0/steam_sdk/data/DataModelCosim.py
+-rw-rw-rw-   0        0        0     8020 2024-04-30 14:26:16.000000 steam-sdk-2024.5.0/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     6491 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/data/DataModelParsimDakota.py
+-rw-rw-rw-   0        0        0     3008 2024-04-08 08:37:58.000000 steam-sdk-2024.5.0/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0      625 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/data/DataPlot.py
+-rw-rw-rw-   0        0        0     2130 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2956 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataProteCCTOptions.py
+-rw-rw-rw-   0        0        0     2595 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     1508 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataPyBBQOptions.py
+-rw-rw-rw-   0        0        0      766 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/data/DataPyCoSim.py
+-rw-rw-rw-   0        0        0     6552 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataPySIGMA.py
+-rw-rw-rw-   0        0        0     2228 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataPySIGMAOptions.py
+-rw-rw-rw-   0        0        0      236 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/data/DataRoxieParams.py
+-rw-rw-rw-   0        0        0     9824 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0    12733 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3263 2024-03-19 10:04:08.000000 steam-sdk-2024.5.0/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0     6024 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/data/DataTFM.py
+-rw-rw-rw-   0        0        0    18457 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    30456 2024-04-05 07:58:47.000000 steam-sdk-2024.5.0/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:07.693969 steam-sdk-2024.5.0/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3739 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverANSYS.py
+-rw-rw-rw-   0        0        0    13733 2024-04-30 05:16:26.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     7448 2024-04-14 11:58:12.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     4278 2024-04-30 05:16:26.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3573 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1894 2024-03-21 12:26:24.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2275 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0      517 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverPySIGMA.py
+-rw-rw-rw-   0        0        0     1983 2024-03-21 12:26:24.000000 steam-sdk-2024.5.0/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.028966 steam-sdk-2024.5.0/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      315 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0    14173 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserCOSIM.py
+-rw-rw-rw-   0        0        0     2290 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1024 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6302 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     2729 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     8536 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2614 2024-03-21 12:26:24.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0     3760 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserFile.py
+-rw-rw-rw-   0        0        0    30071 2024-04-30 14:35:01.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    18391 2024-04-30 14:35:01.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    15085 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    65009 2024-04-12 18:35:10.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4706 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6765 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     1758 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserPyBBQ.py
+-rw-rw-rw-   0        0        0     1663 2024-04-22 06:54:43.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserPyCoSim.py
+-rw-rw-rw-   0        0        0     4061 2024-04-11 12:27:48.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserPySIGMA.py
+-rw-rw-rw-   0        0        0   155447 2024-04-15 21:11:35.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0    11746 2024-04-12 18:35:10.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    58167 2024-04-30 14:26:16.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     7770 2024-04-05 07:58:47.000000 steam-sdk-2024.5.0/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0      929 2024-03-22 11:40:47.000000 steam-sdk-2024.5.0/steam_sdk/parsers/utils_ParserCircuits.py
+-rw-rw-rw-   0        0        0     9687 2024-04-30 05:16:26.000000 steam-sdk-2024.5.0/steam_sdk/parsers/utils_ParserCosims.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.644967 steam-sdk-2024.5.0/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    66858 2024-04-15 21:11:35.000000 steam-sdk-2024.5.0/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0     4619 2024-04-14 11:38:50.000000 steam-sdk-2024.5.0/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    90102 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    48261 2024-03-21 12:26:24.000000 steam-sdk-2024.5.0/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.646967 steam-sdk-2024.5.0/steam_sdk/parsims/translation_dicts/
+-rw-rw-rw-   0        0        0     2351 2024-04-08 08:37:58.000000 steam-sdk-2024.5.0/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+-rw-rw-rw-   0        0        0     2016 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/parsims/translation_dicts/event_column_names.yaml
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.670968 steam-sdk-2024.5.0/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0    29312 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0     8480 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/plotters/PlotterGriddedData.py
+-rw-rw-rw-   0        0        0    20627 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39519 2024-04-15 21:11:35.000000 steam-sdk-2024.5.0/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0    13246 2024-03-26 07:52:01.000000 steam-sdk-2024.5.0/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.672967 steam-sdk-2024.5.0/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0    15676 2024-05-08 10:41:57.000000 steam-sdk-2024.5.0/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.751968 steam-sdk-2024.5.0/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0      204 2024-04-15 21:11:35.000000 steam-sdk-2024.5.0/steam_sdk/utils/MatrixOperations.py
+-rw-rw-rw-   0        0        0    15002 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     3201 2024-04-05 07:58:47.000000 steam-sdk-2024.5.0/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2770 2024-04-05 07:58:47.000000 steam-sdk-2024.5.0/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0     5730 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/ParserRoxieHelpers.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     5806 2024-04-05 07:58:47.000000 steam-sdk-2024.5.0/steam_sdk/utils/attribute_model.py
+-rw-rw-rw-   0        0        0      686 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0    12832 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/compare_simulations.py
+-rw-rw-rw-   0        0        0     3837 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0     1650 2024-04-12 18:35:10.000000 steam-sdk-2024.5.0/steam_sdk/utils/correct_RRR_NIST.py
+-rw-rw-rw-   0        0        0      227 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/delete_if_existing.py
+-rw-rw-rw-   0        0        0     1204 2024-03-22 11:42:52.000000 steam-sdk-2024.5.0/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      691 2024-04-11 06:51:22.000000 steam-sdk-2024.5.0/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     3555 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0     1596 2024-04-13 18:58:31.000000 steam-sdk-2024.5.0/steam_sdk/utils/read_settings_file.py
+-rw-rw-rw-   0        0        0     3365 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/reformat_figure.py
+-rw-rw-rw-   0        0        0      388 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.761969 steam-sdk-2024.5.0/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    39140 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.764968 steam-sdk-2024.5.0/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.767968 steam-sdk-2024.5.0/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.768967 steam-sdk-2024.5.0/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.770967 steam-sdk-2024.5.0/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1830 2024-03-19 09:48:27.000000 steam-sdk-2024.5.0/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:36:08.772967 steam-sdk-2024.5.0/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     5753 2024-05-08 15:36:03.000000 steam-sdk-2024.5.0/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7694 2024-05-08 15:36:03.000000 steam-sdk-2024.5.0/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:36:03.000000 steam-sdk-2024.5.0/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1745 2024-05-08 15:36:03.000000 steam-sdk-2024.5.0/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 15:36:03.000000 steam-sdk-2024.5.0/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2024.4.0/PKG-INFO` & `steam-sdk-2024.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: STEAM,API,SDK,CERN
+Keywords: STEAM,CERN,API,SDK
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
```

### Comparing `steam-sdk-2024.4.0/setup.py` & `steam-sdk-2024.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 build_require = ["setuptools==69.2.0"]
 
 all_requirements = required + docs_require + tests_require + build_require
 
 setup(
     name="steam-sdk",
-    version="2024.4.0",
+    version="2024.5.0",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={"STEAM", "API", "SDK", "CERN"},
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisEvent.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/AnalysisEvent.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisEventLHC.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/AnalysisEventLHC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from steam_sdk.parsers.ParserPSPICE import writeStimuliFromInterpolation
 from steam_sdk.parsers.ParserXYCE import translate_stimulus, get_name_stimulus_folder
 from steam_sdk.parsers.ParserYAML import yaml_to_data, dict_to_yaml
 from steam_sdk.parsims.ParsimConductor import ParsimConductor
 from steam_sdk.parsims.ParsimEventCircuit import ParsimEventCircuit
 from steam_sdk.parsims.ParsimEventMagnet import ParsimEventMagnet
 from steam_sdk.plotters.PlotterMap2d import PlotterMap2d
-# from steam_sdk.plotters.PlotterFiQuSMultipole import PlotterFiQuSMultipole
+from steam_sdk.plotters.PlotterGriddedData import PlotterGriddedData
 from steam_sdk.postprocs.PostprocsMetrics import PostprocsMetrics
 from steam_sdk.utils import parse_str_to_list
 from steam_sdk.utils.attribute_model import set_attribute_model, get_attribute_model
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.parse_str_to_list import parse_str_to_list
 from steam_sdk.utils.read_settings_file import read_settings_file
 from steam_sdk.utils.rgetattr import rgetattr
@@ -80,15 +80,15 @@
 
         self.list_sims = []  # this list will be populated with integers indicating simulations to run
         self.list_viewers = {}  # this dictionary will be populated with Viewer objects and their names
         self.list_metrics = {}  # this dictionary will be populated with calculated metrics
         self.verbose = verbose
         self.summary = None  # float representing the overall outcome of a simulation for parsims
         self.file_name_analysis = file_name_analysis
-        self.simulation_numbers_source_tools = {}
+        self.simulation_numbers_source_tools_and_models = {}
         if file_name_analysis:
             self.path_analysis_file = str(Path(self.file_name_analysis).resolve())  # Find folder where the input file is located, which will be used as the "anchor" for all input files
         if isinstance(file_name_analysis, str) or isinstance(file_name_analysis, PurePath):
             self.data_analysis: DataAnalysis = yaml_to_data(file_name_analysis, DataAnalysis)  # Load yaml keys into DataAnalysis dataclass
             # Read analysis settings
             self._resolve_settings()
             # Read working folders and set them up
@@ -345,15 +345,15 @@
             if step.variable_to_change.startswith('Sources.'):
                 BM.set_input_paths()
 
             # Build simulation file
             if len_simulation_numbers > 0:
                 # Set paths of input files
                 BM.set_input_paths()
-                self.simulation_numbers_source_tools[step.simulation_numbers[v]] = step.software
+                self.simulation_numbers_source_tools_and_models[step.simulation_numbers[v]] = {'tool': step.software, 'model_name': step.model_name}
                 BM = self.setup_sim(BM=BM, step=step, sim_number=step.simulation_numbers[v], verbose=step.verbose)
 
     def step_modify_model_multiple_variables(self, step, verbose: bool = None):
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
         if verbose:
             print('Modifying model object named {}'.format(str(step.model_name)))
 
@@ -453,64 +453,73 @@
             path_result_txt_By = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_nbr}", "output", "mf.By.txt")
             if not os.path.exists(path_result_txt_Bx):
                 raise Warning(f"No Bx file is found: {path_result_txt_Bx}, please check that simulation ran successfully.")
             elif not os.path.exists(path_result_txt_By):
                 raise Warning(f"No By file is found: {path_result_txt_By}, please check that simulation ran successfully.")
 
         def create_map2d_files():
-            if self.simulation_numbers_source_tools[source_sim_nbr].lower() == 'sigma':
+            if self.simulation_numbers_source_tools_and_models[source_sim_nbr]['tool'].lower() == 'sigma':
                 check_if_SIGMA_files_exist(sim_nbr=source_sim_nbr)
                 parser_obj.create_map2d_file_from_SIGMA(
                     results_path=Path(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{source_sim_nbr}", "output")),
                     new_file_name=new_file_names[results_name], check_coordinates=True)
-            elif self.simulation_numbers_source_tools[source_sim_nbr].lower() == 'fiqus':
+            elif self.simulation_numbers_source_tools_and_models[source_sim_nbr]['tool'].lower() == 'fiqus':
                 parser_obj.create_map2d_file_from_FiQuS(
                     results_path=Path(os.path.join(get_solution_folder_path_FiQuS(sim_nbr=source_sim_nbr), step.simulation_name + ".map2d")),
                     new_file_name=new_file_names[results_name])
             else:
                 raise ValueError("Source tool not yet supported for post-process comparison.")
 
         if isinstance(step.simulation_numbers, int) and step.physical_quantity != 'magnetic_flux_density':
             raise ValueError("Comparison with ROXIE is only supported for the magnetic flux density.")
 
         elif isinstance(step.simulation_numbers, int) and step.physical_quantity == 'magnetic_flux_density':
             source_sim_nbr = step.simulation_numbers
-            results_name = self.simulation_numbers_source_tools[source_sim_nbr] + '_' + str(source_sim_nbr)
-            new_file_names[results_name] = results_name + '.map2d'
+            results_name = f"{self.simulation_numbers_source_tools_and_models[source_sim_nbr]['tool']}_{source_sim_nbr}"
+            new_file_names[results_name] = f"{results_name}_b.map2d"
             create_map2d_files()
 
             # Copy ROXIE reference file
             shutil.copy(ref_map2d, step.path_to_saved_files)
 
             PlotterMap2d(parsed_results_path=Path(step.path_to_saved_files)).generate_report_from_map2d(
-                comparison_name=step.simulation_name, file_names=new_file_names, plot_type="coil")
+                comparison_name=step.simulation_name, files_names=new_file_names, plot_type="coil")
 
         elif isinstance(step.simulation_numbers, tuple) and step.physical_quantity == 'magnetic_flux_density':
             for source_sim_nbr in step.simulation_numbers:
-                results_name = self.simulation_numbers_source_tools[source_sim_nbr] + '_' + str(source_sim_nbr)
-                new_file_names[results_name] = results_name + '.map2d'
+                results_name = f"{self.simulation_numbers_source_tools_and_models[source_sim_nbr]['tool']}_{source_sim_nbr}"
+                new_file_names[results_name] = f"{results_name}_b.map2d"
                 create_map2d_files()
             PlotterMap2d(parsed_results_path=Path(step.path_to_saved_files)).generate_report_from_map2d(
-                comparison_name=step.simulation_name, file_names=new_file_names, plot_type="coil")
+                comparison_name=step.simulation_name, files_names=new_file_names, plot_type="coil")
 
         elif isinstance(step.simulation_numbers, tuple) and step.physical_quantity == 'temperature':
-            pass
-            # fiqus_solution_folders = {}
-            # for source_sim_nbr in step.simulation_numbers:
-            #     if self.simulation_numbers_source_tools[source_sim_nbr].lower() == 'fiqus':
-            #         results_name = self.simulation_numbers_source_tools[source_sim_nbr] + '_' + str(source_sim_nbr)
-            #         results_paths[results_name] = os.path.join(get_solution_folder_path_FiQuS(sim_nbr=source_sim_nbr))
-            #         fiqus_solution_folders.update({str(source_sim_nbr): results_paths[results_name]})
-            #     else:
-            #         raise ValueError("Source tool not yet supported for post-process comparison.")
-            #
-            # if all([self.simulation_numbers_source_tools[source_sim_nbr].lower() == 'fiqus' for source_sim_nbr in step.simulation_numbers]):
-            #     plot_object = PlotterFiQuSMultipole(solution_folders_paths=fiqus_solution_folders,
-            #                                         physical_quantity_to_initialize_per_solution={sim_nbr: step.physical_quantity for sim_nbr in fiqus_solution_folders.keys()})
-            #     plot_object.plot_time_figure(solution='1', physical_quantity=step.physical_quantity, half_turns=[229, 230, 231])
+            data_frames = ()
+            plotter_obj = PlotterGriddedData(
+                parsed_results_path=Path(step.path_to_saved_files), simulation_name=step.simulation_name,
+                coil_data=self.list_models[self.simulation_numbers_source_tools_and_models[step.simulation_numbers[0]]['model_name']].roxie_data.coil,
+                ffmpeg_exe_path=self.settings.ffmpeg_path)
+            for source_sim_nbr in step.simulation_numbers:
+                results_name = f"{self.simulation_numbers_source_tools_and_models[source_sim_nbr]['tool']}_{source_sim_nbr}"
+                new_file_names[results_name] = f"{results_name}_T_time.csv"
+                if self.simulation_numbers_source_tools_and_models[source_sim_nbr]['tool'].lower() == 'fiqus':
+                    # add parser step if in the future the standard transient temperature file differs from half_turn_temperatures_over_time.csv
+                    shutil.copy(os.path.join(get_solution_folder_path_FiQuS(sim_nbr=source_sim_nbr), 'half_turn_temperatures_over_time.csv'),
+                                os.path.join(step.path_to_saved_files, new_file_names[results_name]))
+                else:
+                    raise ValueError(f"Source tool {self.simulation_numbers_source_tools_and_models[source_sim_nbr]['tool']} not yet supported for {step.physical_quantity}.")
+
+                plotter_obj.plot_conductors_temperatures_over_time(file_name=new_file_names[results_name])
+                data_frames += (pd.read_csv(os.path.join(step.path_to_saved_files, new_file_names[results_name])),)
+
+            data_frame_compare = data_frames[0] - data_frames[1]
+            data_frame_compare['Time'] = data_frames[0]['Time']
+            file_name = f"compare_{step.simulation_numbers[0]}_to_{step.simulation_numbers[1]}_T_time.csv"
+            data_frame_compare.to_csv(os.path.join(step.path_to_saved_files, file_name), index=False, float_format='%.4f')
+            plotter_obj.plot_conductors_temperatures_over_time(file_name=file_name, data_type='absolute_error')
 
     # def step_setup_folder(self, step, verbose: bool = None):
     #     """
     #     Set up simulation working folder.
     #     The function applies a different logic for each simulation software.
     #     """
     #     verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2024.5.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/BuilderAPDL_CT.py` & `steam-sdk-2024.5.0/steam_sdk/builders/BuilderAPDL_CT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/BuilderCosim.py` & `steam-sdk-2024.5.0/steam_sdk/builders/BuilderCosim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2024.5.0/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2024.5.0/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2024.5.0/steam_sdk/builders/BuilderModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import datetime
 import os
 import shutil
 from pathlib import Path
 from typing import Union
 
 import numpy as np
@@ -343,28 +344,30 @@
                 for _ in range(2):  # for 'go' and 'return' part of fqpl
                     max_turn += 1   # increment by one, this matches fiqus postprocessing
                     electrical_order.append(max_turn)
 
             el_order_half_turns = electrical_order
         elif self.model_data.GeneralParameters.magnet_type in ['CWS']:
             el_order_half_turns = self.model_data.Options_FiQuS.cws.postproc.field_map.winding_order
+        # elif self.model_data.GeneralParameters.magnet_type in ['Pancake3D']:  # TODO
+        # elif self.model_data.GeneralParameters.magnet_type in ['Racetrack']:  # TODO
+
         # Assign values to the attribute in the model_data dataclass
         self.el_order_half_turns = el_order_half_turns  #TODO assign it to a better structure
 
         if verbose:
             print('Setting electrical order was successful.')
 
         if flag_plot:
             PM = PlotterModel(self.roxie_data)
             if self.model_data.GeneralParameters.magnet_type not in ['CCT_straight', 'CWS']:
                 PM.plot_electrical_order(el_order_half_turns, self.model_data.CoilWindings.electrical_pairs.group_together, strandToGroup, self.roxie_params.x_strands, self.roxie_params.y_strands, strandToHalfTurn, self.model_data)
         return np.array(el_order_half_turns)
 
-    def buildAPDL_CT(self, sim_name: str, sim_number: Union[
-        int, str], output_path: str, flag_plot_all: bool = False, verbose: bool = None):
+    def buildAPDL_CT(self, sim_name: str, sim_number: Union[int, str], output_path: str, flag_plot_all: bool = False, verbose: bool = None):
         '''
             Write input file for an APDL model of a cos-theta magnet (LBNL model)
             :param sim_name: Simulation name that will be used to write the output file
             :param sim_number: Simulation number or string that will be used to write the output file
             :param output_path: Output folder
             :param flag_plot_all: Display figures
             :param verbose: If True, display logging information
@@ -730,66 +733,64 @@
         mps.build(input_yaml_file_path=input_yaml_file_path, input_coordinates_path=coordinate_file_path, results_folder_name='output', settings=self.settings_dict)  # TODO DISCUSS
 
         if flag_plot_all:
             PlotterRoxie.plot_all(self.roxie_data)
             PM = PlotterModel(self.roxie_data)
             PM.plot_all(self.model_data)
 
-    def buildTFM(self, output_path: str, T: float, flag_PC:bool = False, flag_IFCC:bool = False, flag_ISCC:bool = False,
-                                flag_Wedges:bool = False, flag_ColdBore:bool = False, flag_EC:bool = False, flag_Roxie:bool = False,
-                                flag_BS: bool = False, flag_Mutual: bool = False, Field_interp_value: float = None):
+    def buildTFM(self, output_path: str, TFM_inputs = None, Magnet_data = None):
         """
             Building a TFM model
         """
 
         magnet_name = self.model_data.GeneralParameters.magnet_name
         builder_ledet = BuilderLEDET(path_input_file=self.path_input_file, input_model_data=self.model_data,
                                      input_map2d=self.path_map2d, flag_build=True, input_roxie_data=self.roxie_data,
                                      smic_write_path='skip')
-        self.builderTFM = BuilderTFM(magnet_name=magnet_name, builder_LEDET=builder_ledet, T=T, output_path=output_path,
-                                    flag_PC=flag_PC, flag_IFCC=flag_IFCC, flag_ISCC=flag_ISCC,
-                                    flag_Wedges=flag_Wedges, flag_ColdBore=flag_ColdBore, flag_EC=flag_EC, flag_Roxie=flag_Roxie,
-                                    flag_BS=flag_BS, Field_interp_value=Field_interp_value, flag_Mutual=flag_Mutual)
+        self.builderTFM = BuilderTFM(magnet_name=magnet_name, builder_LEDET=builder_ledet, output_path=output_path,
+                                    TFM_inputs=TFM_inputs, Magnet_data=Magnet_data)
 
     def buildXYCE(self, sim_name: str, sim_number: Union[int, str], output_path: str, verbose: bool = None):
         """
             Build a XYCE circuit netlist model
             :param sim_name: Simulation name that will be used to write the output file
             :param sim_number: Simulation number or string that will be used to write the output file
             :param output_path: Output folder
             :param verbose: If True, display logging information
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
         sim_suffix = f'_{sim_number}' if isinstance(sim_number, int) else sim_number
         make_folder_if_not_existing(output_path, verbose=verbose)
 
+
         if self.circuit_data.TFM != None:
             TFM = self.circuit_data.TFM
             # Save each element inside TFM which is not Magnet (flags, T, M_IF_PC) inside the GlobalParameters class of circuit_data
             # format: 'flag_PC' = value
             for key, value in TFM.__dict__.items():
                 if key != 'Magnets':
-                    self.circuit_data.GlobalParameters.global_parameters[key] = value
+                    if value is not None:
+                        self.circuit_data.GlobalParameters.global_parameters[key] = value
                     if key == 'T':
                         if value is not None:
                             T = value
                         else:
                             T = 1.9
+            TFM_general = copy.deepcopy(TFM)
+            del TFM_general.Magnets
 
             Magnets = self.circuit_data.TFM.Magnets
             for key, Magnet in Magnets.items():
                 # For each magnet element, calls TFM to build the model
                 file_model_data_TFM = os.path.join(self.settings_dict.local_library_path,  'magnets', Magnet.name, 'input', f'modelData_{Magnet.name}.yaml')
                 bM_TFM = BuilderModel(file_model_data=file_model_data_TFM)
                 output_path_TFM = os.path.join(output_path, 'TFM_' + key)
                 if Magnet.Field_interp_value is None:
                     Magnet.Field_interp_value = T
-                bM_TFM.buildTFM(output_path=output_path_TFM, T=T, flag_PC=TFM.flag_PC, flag_IFCC=TFM.flag_IFCC, flag_ISCC=TFM.flag_ISCC,
-                                flag_Wedges=TFM.flag_Wedges, flag_ColdBore=TFM.flag_ColdBore, flag_EC=TFM.flag_EC, flag_Roxie=TFM.flag_Roxie,
-                                flag_BS = TFM.flag_BS,  Field_interp_value=Magnet.Field_interp_value, flag_Mutual = TFM.flag_Mutual)
+                bM_TFM.buildTFM(output_path=output_path_TFM, TFM_inputs=TFM_general, Magnet_data=Magnet)
                 # Save the library in which the magnet models have been created
                 if output_path_TFM not in self.circuit_data.Libraries.component_libraries:
                     self.circuit_data.Libraries.component_libraries.append(output_path_TFM)
                 if output_path_TFM not in self.circuit_data.GeneralParameters.additional_files:
                     self.circuit_data.GeneralParameters.additional_files.append(output_path_TFM)
                 # Add the corresponding Lmag and C_ground of each magnet to the global parameters in the format 'Lmag_x_Magnet_1' = value
                 self.circuit_data.GlobalParameters.global_parameters[f'L_mag_{key}'] = Magnet.L_mag
@@ -799,15 +800,16 @@
                 # Add for each magnet the corresponding Lmag and C_ground to the netlist parameters in the format 'Lmag' = 'Lmag_x_Magnet_1'
                 self.circuit_data.Netlist[key].parameters['L_mag']= f'L_mag_{key}'
                 self.circuit_data.Netlist[key].parameters['C_ground'] = f'C_ground_{key}'
                 self.circuit_data.Netlist[key].parameters['Field_interp_value'] = f'Field_interp_value_{key}'
                 for flag in TFM.__dict__.keys():
                     if flag != 'Magnets':
                         # Add for each magnet the corresponding flags to the netlist parameters in the format  'flag_PC' = 'flag_PC'
-                        self.circuit_data.Netlist[key].parameters[flag] = flag
+                        if flag != 'M_CB_Wedges' or (flag == 'M_CB_Wedges' and TFM.M_CB_Wedges):
+                            self.circuit_data.Netlist[key].parameters[flag] = flag
 
         # Write output .cir file
         parser_xyce = ParserXYCE(circuit_data=self.circuit_data, path_input=self.path_input_file, output_path=output_path)
         path_file_name = os.path.join(output_path, f'{sim_name}{sim_suffix}.cir')  # full path of the XYCE netlist to write
         parser_xyce.write2XYCE(path_file_name, flag_resolve_library_paths=True, flag_copy_additional_files=True, verbose=verbose)
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2024.5.0/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2024.5.0/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/BuilderPySIGMA.py` & `steam-sdk-2024.5.0/steam_sdk/builders/BuilderPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/BuilderTFM.py` & `steam-sdk-2024.5.0/steam_sdk/builders/BuilderTFM.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dataclasses import asdict
 from scipy.interpolate import RegularGridInterpolator
 from scipy.signal import find_peaks
 import steammaterials
 from steam_sdk.data.DataTFM import General
 from steam_sdk.data.DataTFM import HalfTurns
 from steam_sdk.data.DataTFM import Strands
-from steam_sdk.data.DataTFM import PersistentCurrent
+from steam_sdk.data.DataTFM import PC
 from steam_sdk.data.DataTFM import Options
 from steam_sdk.data.DataTFM import IFCC
 from steam_sdk.data.DataTFM import ISCC
 from steam_sdk.data.DataTFM import EC_CopperSheath
 from steam_sdk.data.DataTFM import Wedges
 from steam_sdk.data.DataTFM import ColdBore
 from steammaterials.STEAM_materials import STEAM_materials
@@ -26,18 +26,15 @@
 
 class BuilderTFM:
     """
            Class to generate TFM models
     """
 
     def __init__(self, magnet_name: str = None, builder_LEDET= None, flag_build: bool = True,
-                  T: float = 1.9, Field_interp_value: float = None, output_path: str = None,
-                 path_input_file: str = None, flag_Roxie: bool = False, flag_BS: bool = False,
-                 flag_PC: bool = False, flag_IFCC: bool = False, flag_ISCC: bool = False, flag_Wedges: bool = False,
-                 flag_ColdBore: bool = False, flag_EC: bool = False, flag_Mutual: bool = False):
+                  output_path: str = None, path_input_file: str = None, TFM_inputs=None, Magnet_data=None ):
         """
              Object is initialized by defining TFM variable structure and default parameter descriptions, starting from
              the magnet_name and the builder_LEDET model. The class can also calculate various passive effects, depending on the flag values.
 
             :param magnet_name: name of the analyzed magnet
             :param builder_LEDET: builderLEDET object corresponding to that magnet
             :param flag_build: defines whether the model has to be build
@@ -58,63 +55,68 @@
         # TODO lib_path
         # TODO hard coded path to steam models
         # Data structures
         self.General = General()
         self.HalfTurns = HalfTurns()
         self.Strands = Strands()
         self.Options = Options()
-        self.PersistentCurrent = PersistentCurrent()
+        self.PC = PC()
         self.IFCC = IFCC()
         self.ISCC = ISCC()
         self.EC_CopperSheath = EC_CopperSheath()
         self.Wedges = Wedges()
         self.ColdBore = ColdBore()
-        self.magnet_name = magnet_name
+        self.magnet_name = Magnet_data.name
         self.path_input_file = path_input_file
 
         if flag_build:
             if not builder_LEDET or not self.magnet_name:
                  raise Exception('Cannot build model without providing BuilderLEDET object with Inputs dataclass and magnet_name')
 
             # Translate the Inputs dataclass of BuilderLEDET in a dictionary
             LedetInputs = asdict(builder_LEDET.Inputs)
             self.LedetInputs = LedetInputs
             self.LedetAuxiliary = builder_LEDET.Auxiliary
             self.LedetOptions = builder_LEDET.Options
-            self.T = T
-            self.flag_Roxie = flag_Roxie
-            self.Field_interp_value = Field_interp_value
+            self.TFM_inputs = TFM_inputs
+            self.Magnet_data = Magnet_data
+
+            self.M_CB_Wedges = TFM_inputs.M_CB_Wedges
+            self.T = TFM_inputs.T
+            self.Field_interp_value = Magnet_data.Field_interp_value
 
             # TODO: HardCoded values
             self.General.I_magnet = 1
             self.General.lib_path = f"D:\\Code_new\\steam_analyses\\mbrd_tfm\\local_library\\lib\\{magnet_name}_TFM_General.lib"
             # self.General.path_input_file = f"D:\\Code_new\\\steam_analyses\\mbrd_tfm\\local_library\\magnets\\{magnet_name}\\input"
             self.General.path_input_file = f"D:\\Code_new\\\steam_sdk\\tests\\builders\\model_library\\magnets\\{magnet_name}\\input"
             self.Wedges.RRR_wedges = np.array([50])
 
             self.conductor_to_group = np.array(builder_LEDET.model_data.CoilWindings.conductor_to_group)
 
             self.translateModelDataToTFMGeneral()
             self.translateModelDataToTFMHalfTurns()
             self.translateModelDataToTFMStrands()
-            self.setOptions(flag_PC=flag_PC, flag_IFCC=flag_IFCC, flag_ISCC=flag_ISCC, flag_Wedges=flag_Wedges,
-                            flag_ColdBore=flag_ColdBore, flag_EC=flag_EC, flag_BS=flag_BS)
-            self.flag_Mutual = flag_Mutual
+            self.setOptions()
             self.change_coupling_parameter(output_path=output_path)
 
     def translateModelDataToTFMGeneral(self):
         """
             This function saves the appropriate BuilderLEDET Inputs dataclass values for the General dataclass attributes.
         """
         self.setAttribute(self.General, 'magnet_name', self.magnet_name)
         self.setAttribute(self.General, 'magnet_length', self.LedetInputs['l_magnet'])
         nT = self.LedetInputs['nT']
         self.setAttribute(self.General, 'num_HalfTurns', np.sum(nT))
         bins = max(self.conductor_to_group)
         self.setAttribute(self.General, 'bins', bins)
+        L_mag = self.Magnet_data.L_mag
+        self.setAttribute(self.General, 'L_mag', L_mag)
+        C_ground = self.Magnet_data.C_ground
+        self.setAttribute(self.General, 'C_ground', C_ground)
 
 
     def translateModelDataToTFMHalfTurns(self):
         """
              This function saves the appropriate BuilderLEDET Inputs dataclass values for the HalfTurns dataclass attributes.
              The saved data are arrays with len equal to the total number of HalfTurns
          """
@@ -173,45 +175,42 @@
             :param flag_ColdBore: if True includes the Cold Bore effect
             :param flag_EC: if True includes the Eddy Currents effect in the Copper Sheath
         """
         if self.T < min(self.LedetInputs['Tc0_NbTi_ht_inGroup']):
             flag_SC = True
         else:
             flag_SC = False
-
         self.setAttribute(self.Options, 'flag_SC', flag_SC)
-        self.setAttribute(self.Options, 'flag_PC', flag_PC)
-        self.setAttribute(self.Options, 'flag_IFCC', flag_IFCC)
-        self.setAttribute(self.Options, 'flag_ISCC', flag_ISCC)
-        self.setAttribute(self.Options, 'flag_Wedges', flag_Wedges)
-        self.setAttribute(self.Options, 'flag_ColdBore', flag_ColdBore)
-        self.setAttribute(self.Options, 'flag_EC', flag_EC)
-        self.setAttribute(self.Options, 'flag_BS', flag_BS)
+
+        for keyTFMData, value in self.TFM_inputs.__dict__.items():
+            if keyTFMData.startswith('flag'):
+                self.setAttribute(self.Options, keyTFMData, value)
+
 
     def calculate_field_contributions(self):
         '''
         Calculates the field in each filament of the MB magnet - ROXIE Edition
         This function returns the calculated field contributions from ROXIE for the magnet
         '''
         ## Field in all filaments when fully powering the magnet
 
-        if self.flag_Roxie:
+        if self.Options.flag_Roxie:
             f_mag, f_mag_X_all, f_mag_Y_all = self.retrieve_field_contributions_Roxie()
         else:
             f_mag, f_mag_X_all, f_mag_Y_all = self.retrieve_field_contributions_COMSOL(value=self.Field_interp_value, flag_BS=self.Options.flag_BS)
 
         self.setAttribute(self.Strands, 'f_mag_X', f_mag_X_all)
         self.setAttribute(self.Strands, 'f_mag_Y', f_mag_Y_all)
         self.setAttribute(self.Strands, 'f_mag', f_mag)
 
 
-    def calculate_persistentCurrents(self, frequency: np.ndarray, T: float, fMag: np.ndarray):
+    def calculate_PC(self, frequency: np.ndarray, T: float, fMag: np.ndarray):
         '''
         Function that calculates the equivalent circuit parameter for the persistent currents and save them to the
-        PersistentCurrent dataclass
+        PC dataclass
 
         :param frequency: Frequency vector
         :param T: temperature vector, to be used in the interaction with Eddy-currents
         :param flag_Roxie: if True it uses f_mag calculated from Roxie, else it uses the f_mag provided as parameter
         :param f_mag: field-factor for each strand
         '''
 
@@ -252,18 +251,18 @@
         L_pc = np.squeeze(L_pc[:, idx_valid])
         STC_pc = np.squeeze(STC_pc[:, idx_valid])
         M_temp = np.squeeze(M_temp[:, idx_valid])
 
         L_bin, R_bin, M_bin = bin_components(frequency=frequency, L=L_pc, R=STC_pc, M=M_temp, bins=bins, sort_on="R")
 
 
-        self.setAttribute(self.PersistentCurrent, 'M', M_bin)
-        self.setAttribute(self.PersistentCurrent, 'I', I_Pc)
-        self.setAttribute(self.PersistentCurrent, 'L', L_bin)
-        self.setAttribute(self.PersistentCurrent, 'M_IF_PC', M_if_Pc)
+        self.setAttribute(self.PC, 'M', M_bin)
+        self.setAttribute(self.PC, 'I', I_Pc)
+        self.setAttribute(self.PC, 'L', L_bin)
+        self.setAttribute(self.PC, 'M_IF_PC', M_if_Pc)
 
 
     def calculate_IFCC(self, frequency: np.ndarray, T: float, fMag: np.ndarray) -> np.ndarray:
         '''
         Calculates the equivalent IFCC coupling loops for a given temperature and field
 
         :param frequency: Frequency vector
@@ -607,15 +606,15 @@
         It takes the Temperature. It then calculates the resistivity and
         interpolates the current and power from pre-simulated values.
         '''
 
         rho_CB = self.rhoSS_nist(T=T)
         P_tot, I_tot, tau_CB, frequency = self.interpolate(rho=rho_CB, case='ColdBore')
         w = 2 * np.pi * frequency
-        P_tot = P_tot * self.General.magnet_length * 2
+        P_tot = P_tot * self.General.magnet_length #* 2
 
         # Calculating the coupled loop equivalent parameter
         R_CB= P_tot / I_tot ** 2
         L_CB = tau_CB * R_CB[0]
         M_CB = (1j * w * L_CB * I_tot + I_tot * R_CB) / (1j * w * 1)
 
         M_CB = np.sqrt(np.real(M_CB) ** 2 + np.imag(M_CB) ** 2)
@@ -727,16 +726,16 @@
             # Persistent currents and magnetization
             if self.Options.flag_PC:
                 if not self.Options.flag_ISCC:
                     f_mag_PC = self.Strands.f_mag
                 else:
                     f_mag_PC = np.maximum(self.Strands.f_mag - np.sqrt(f_mag_X_ISCC_return ** 2 + f_mag_Y_ISCC_return ** 2), 1e-12)
                 self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original)
-                self.calculate_persistentCurrents(frequency=frequency, T=T, fMag=f_mag_PC)
-                self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'PC', frequency, self.PersistentCurrent.L, np.array([]), self.PersistentCurrent.M, bins=bins,
+                self.calculate_PC(frequency=frequency, T=T, fMag=f_mag_PC)
+                self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'PC', frequency, self.PC.L, np.array([]), self.PC.M, bins=bins,
                                                  force_new_name=self.General.new_lib_path)
 
             # Inter-Filament Coupling Currents
             if self.Options.flag_IFCC:  #Change rho_eff to 0.3
                 if not self.Options.flag_ISCC:
                     f_mag_IFCC = self.Strands.f_mag
                 else:
@@ -763,23 +762,28 @@
 
             if self.Options.flag_ColdBore:
                 self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original)
                 self.calculate_ColdBore(T=T)
                 self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'ColdBore', frequency, self.ColdBore.L, self.ColdBore.R, self.ColdBore.M, bins=bins,
                                                               force_new_name=self.General.new_lib_path)
 
-            if self.flag_Mutual:
-                self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original)
-                M_Wedges_ColdBore = [self.calculate_MutualCoupling_ColdBore_Wedges()[0] * 10] * 63 + [0] * 58
-                self.General.lib_path = change_library_MutualCoupling(self.General.lib_path, 'M_Wedges_ColdBore',
-                                                                      frequency, M_Wedges_ColdBore)
+            if self.M_CB_Wedges is not None:
+                self.General.lib_path = change_library_MutualCoupling(self.General.lib_path, 'M_Wedges_ColdBore',[1, 1e5], [self.M_CB_Wedges,self.M_CB_Wedges])
+                # self.General.lib_path = change_library_MutualCoupling(self.General.lib_path, 'M_Wedges_ColdBore',
+                #                                                       frequency, M_Wedges_ColdBore)
+
+
+            attributes = [value for attr, value in vars(self.Options).items() if (attr != 'flag_SC' and attr != 'flag_Roxie' and attr != 'flag_BS')]
+
+            # Check if all the flags of the effects in the Option class are True, in that case it means that the inductance matrix needs to be checked
+            if all(value for value in attributes):
+                self.check_inductance_matrix()
 
             # Check if all the flags of the effects in the Option class are False, in that case it means that no lib file has been generated yet,
             # but since the Output path is not None we still need to generate it
-            attributes = [value for attr, value in vars(self.Options).items() if attr != 'flag_SC']
             if all(not value for value in attributes):
                 # The value to be sent to change_library_EqLoop needs to have the as .shape[1] the number of bins
                 value = np.zeros((1, self.General.bins))
                 self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'ABC', value, value, value, value, bins=bins, force_new_name=self.General.new_lib_path)
 
 
     def retrieve_field_contributions_COMSOL(self, value: float = None,  flag_BS: bool = False) -> np.ndarray:
@@ -895,14 +899,45 @@
         f_mag = np.repeat(f_mag[:, np.newaxis], len(frequency), axis=1).T
 
 
         self.frequency = frequency
 
         return f_mag, f_mag_X_all, f_mag_Y_all
 
+    def check_inductance_matrix(self):
+
+        frequency = self.frequency
+        Effects = ['Magnet', 'PC', 'ISCC', 'IFCC', 'EC_CopperSheath', 'ColdBore', 'Wedges']
+        L_matrix_list = []
+
+        for i in range(len(frequency)):
+            L_matrix = np.zeros((len(Effects), len(Effects)))
+            for j in range(len(Effects)):
+                if Effects[j] == 'Magnet':
+                    L_matrix[0, 0] = self.General.L_mag
+                else:
+                    if Effects[j] != 'ColdBore' and Effects[j] != 'Wedges':
+                        L_matrix[0, j] = self.__dict__[Effects[j]].M[i, :]
+                        L_matrix[j, 0] = self.__dict__[Effects[j]].M[i, :]
+                        L_matrix[j, j] = self.__dict__[Effects[j]].L[i, :]
+                    else:
+                        L_matrix[0, j] = self.__dict__[Effects[j]].M[i]
+                        L_matrix[j, 0] = self.__dict__[Effects[j]].M[i]
+                        L_matrix[j, j] = self.__dict__[Effects[j]].L[i]
+            L_matrix_list.append(L_matrix)
+
+        for i in range(len(L_matrix_list)):
+            if not is_positive_definite(L_matrix_list[i]):
+                raise Exception(f'Matrix not positive definite for frequency {frequency[i]}')
+            # else:
+            #     print(f'Matrix positive definite for frequency {frequency[i]}')
+
+
+
+
     def rhoCu_nist(self, T: float, RRR: np.ndarray, B: np.ndarray) -> np.ndarray:
         '''
         Helper function to calculate resistivity of copper. Taken from steam-materials library
 
         :param T: Temperature
         :return: array of resistivities
         '''
@@ -1204,7 +1239,16 @@
             else:
                 break
         tau_index = int((np.min(list_index) + np.max(list_index)) / 2)
 
     return tau_index
 
 
+def is_positive_definite(matrix):
+    try:
+        # Attempt Cholesky decomposition
+        np.linalg.cholesky(matrix)
+        return True
+    except np.linalg.LinAlgError:
+        return False
+
+
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2024.5.0/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/Solenoids.py` & `steam-sdk-2024.5.0/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2024.5.0/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2024.5.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/cosims/CoSimPyCoSim.py` & `steam-sdk-2024.5.0/steam_sdk/cosims/CoSimPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataAPDLCTOptions.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataAPDLCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 class PostProcessCompare(BaseModel):
     """
         Level 2: Analysis step to run a simulation file
     """
     type: Literal['PostProcessCompare']
     physical_quantity: Optional[str] = None
     simulation_numbers: Optional[
-        Union[Tuple[int, int], int]] = None  # if only an int is provided, the other results are taken from ROXIE
+        Union[Tuple[int, int], int]] = None  # second is considered reference. If only an int is provided, the other results are taken from ROXIE
     simulation_name: Optional[str] = None
     path_to_saved_files: Optional[str] = None
 
 
 class RunCustomPyFunction(BaseModel):
     """
         Level 2: Analysis step to run a custom Python function
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataConductor.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataFiQuS.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,14 +467,15 @@
 class MultipoleSolveTimeParametersAdaptive(BaseModel):
     """
         Level 6: Class for FiQuS Multipole
     """
     initial_time_step: Optional[float] = None
     min_time_step: Optional[float] = None
     max_time_step: Optional[float] = None
+    breakpoints: Optional[List[float]] = []
     integration_method: Optional[str] = None
     rel_tol_time: Optional[float] = None
     abs_tol_time: Optional[float] = None
     norm_type: Optional[str] = None
 
 
 class MultipoleSolveTimeParametersFixed(BaseModel):
@@ -523,16 +524,16 @@
     adaptive: MultipoleSolveTimeParametersAdaptive = MultipoleSolveTimeParametersAdaptive()
 
 
 class MultipoleSolveQuenchInitiation(BaseModel):
     """
         Level 5: Class for FiQuS Multipole
     """
-    turns: List[int] = []
-    temperatures: List[float] = []
+    turns: Optional[List[int]] = None
+    t_trigger: Optional[List[float]] = None
 
 
 class MultipoleSolveBoundaryConditionsElectromagnetics(BaseModel):
     """
         Level 4: Class for FiQuS Multipole
     """
     currents: List[float] = []
@@ -588,14 +589,23 @@
     """
         Level 4: Class for FiQuS Multipole
     """
     coil_and_wedges: int = 1
     insulation: int = 1
 
 
+class MultipoleSolveGaussianPoints(BaseModel):
+    """
+    Level 4: Class for FiQuS Multipole
+    """
+
+    conducting_elements: int = 4
+    insulation: int = 3
+
+
 class MultipoleSolveThinShellApproximationParameters(BaseModel):
     """
         Level 4: Class for FiQuS Multipole
     """
     integration_points: Optional[int] = None  # needs to be reasonably large to properly integrate non-linearity (>= 2)
     global_size: Optional[float] = None
     minimum_discretizations: int = 1
@@ -649,14 +659,15 @@
 
 
 class MultipoleSolveThermal(BaseModel):
     """
         Level 3: Class for FiQuS Multipole
     """
     solved: Optional[str] = None
+    gaussian_points: MultipoleSolveGaussianPoints = MultipoleSolveGaussianPoints()
     TSA: MultipoleSolveThinShellApproximationParameters = MultipoleSolveThinShellApproximationParameters()
     basis_order: MultipoleSolveBasisOrder = MultipoleSolveBasisOrder()
     isothermal_conductors: bool = False
     isothermal_wedges: bool = False
     initial_temperature: Optional[float] = None
     enforce_initial_temperature_as_minimum: bool = False
     He_cooling: MultipoleSolveHeCooling = MultipoleSolveHeCooling()
@@ -726,16 +737,19 @@
     pro_template: Optional[str] = None  # file name of .pro template file
 
 
 class MultipolePostProc(BaseModel):
     """
         Level 2: Class for FiQuS Multipole
     """
-    output_time_steps: Optional[Union[int, List[float]]] = None
-    compare_to_ROXIE: Optional[str] = None
+    output_time_steps_pos: Optional[Union[bool, int]] = None
+    output_time_steps_txt: Optional[Union[bool, int]] = None
+    save_pos_at_the_end: bool = True
+    compare_to_ROXIE: Optional[str] = None  # EM-specific key
+    take_average_conductor_temperature: Optional[bool] = None  # TH-specific key
     plot_all: Optional[str] = None
     variables: Optional[List[str]] = None  # Name of variables to post-process, like "b" for magnetic flux density
     volumes: Optional[List[str]] = None  # Name of domains to post-process, like "powered"
     file_exts: Optional[List[str]] = None  # Name of file extensions to output to, like "pos"
     additional_outputs: Optional[List[str]] = None  # Name of software specific input files to prepare, like "LEDET3D"
 
 
@@ -1671,15 +1685,15 @@
         title="Quantity",
         description="Name of the quantity to be saved.",
     )
 
 
 class Pancake3DSolveSaveQuantity(Pancake3DSolveQuantityBase):
     # Optionals:
-    timesToBeSaved: list[float] = Field(
+    timesToBeSaved: Optional[list[float]] = Field(
         default=[],
         title="Times to be Saved",
         description=(
             "List of times that wanted to be saved. If not given, all the time steps"
             " will be saved."
         ),
     )
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataFiQuSOptions.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataFiQuSOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataLEDET.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataLEDETOptions.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataLEDETOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataModelCircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,23 +55,23 @@
     name: Optional[str] = None
     L_mag: Optional[float] = None
     C_ground: Optional[float] =None
     Field_interp_value: Optional[float] = None
 
 class TFMClass(BaseModel):
     flag_PC: Optional[bool] = False
-    flag_IFCC: Optional[bool] = False
     flag_ISCC: Optional[bool] = False
+    flag_IFCC: Optional[bool] = False
+    flag_EC: Optional[bool] = False
     flag_Wedges: Optional[bool] = False
     flag_ColdBore: Optional[bool] = False
-    flag_EC: Optional[bool] = False
     flag_BS: Optional[bool] = False
     flag_Roxie: Optional[bool] = False
-    flag_Mutual: Optional[bool] = False
     M_IF_PC: Optional[float] = None
+    M_CB_Wedges: Optional[float] = None
     T: Optional[float] = None
     Magnets: Dict[str, Magnet] = {}
 
 
 ############################
 # Global parameters
 class Global_Parameters(BaseModel):
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataModelCommon.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataModelCommon.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataModelCosim.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataModelCosim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataModelParsimDakota.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataModelParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataProteCCTOptions.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataProteCCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataPyBBQOptions.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataPyBBQOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataPyCoSim.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataPySIGMA.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataPySIGMAOptions.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataPySIGMAOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataSettings.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,21 @@
                                       title="COSIM executable path",
                                       description="Absolute path to COSIM.exe. Only version 0.5 is supported.",
                                       examples=[r"C:\STEAM\steam-cosim_v0.5.exe"])
     Dakota_path: Optional[str] = Field(default=None,
                                        title="DAKOTA executable path",
                                        description="Full path to dakota.exe. Only version 6.16.0 has been tested to work correctly.",
                                        examples=[r"C:\Program Files\dakota-6.16.0-public-windows.Windows.x64-cli\bin\dakota.exe"])
+    ffmpeg_path: Optional[str] = Field(default=None,
+                                       title="ffmpeg executable path",
+                                       description="Absolute path to ffmpeg.exe.",
+                                       examples=[r"C:\Program Files\ffmpeg-master-latest-win64-gpl\bin\ffmpeg.exe"])
     FiQuS_path: Optional[str] = Field(default=None,
                                       title="FiQuS folder path",
-                                      description="Absolute path to FiQuS folder containing it source code",
+                                      description="Absolute path to FiQuS folder containing its source code",
                                       examples=[r"C:\STEAM\steam-fiqus", r"C:\STEAM\steam-fiqus-dev"])
     GetDP_path: Optional[str] = Field(default=None,
                                       title="GetDP executable path",
                                       description="Absolute path to getdp.exe. Either official GetDP and CERNGetDP can be used, depending on the model requirements",
                                       examples=[r"C:\STEAM\cerngetdp_2024.1.0\getdp_2024.1.0.exe", r"C:\getdp-3.5.0-Windows64\getdp.exe"])
     LEDET_path: Optional[str] = Field(default=None,
                                       title="LEDET executable path",
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataSignal.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DataTFM.py` & `steam-sdk-2024.5.0/steam_sdk/data/DataTFM.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     magnet_length: Optional[float] = None
     num_HalfTurns: Optional[int] = None
     I_magnet: Optional[float] = None
     bins: Optional[int] = None
     path_input_file: Optional[str] = None
     lib_path: Optional[str] = None
     new_lib_path: Optional[str] = None
+    L_mag: Optional[float] = None
+    C_ground: Optional[float] = None
 
 
 @dataclass
 class HalfTurns:
     HalfTurns_to_coil_sections: np.ndarray = field(default_factory=lambda: np.array([]))
     HalfTurns_to_group: np.ndarray = field(default_factory=lambda: np.array([]))
     HalfTurns_to_conductor: np.ndarray = field(default_factory=lambda: np.array([]))
@@ -62,17 +64,18 @@
     flag_PC: Optional[bool] = False
     flag_IFCC: Optional[bool] = False
     flag_ISCC: Optional[bool] = False
     flag_Wedges: Optional[bool] = False
     flag_ColdBore: Optional[bool] = False
     flag_EC: Optional[bool] = False
     flag_BS: Optional[bool] = False
+    flag_Roxie: Optional[bool] = False
 
 @dataclass
-class PersistentCurrent:  # DataClass for persistent current
+class PC:  # DataClass for persistent current
     L: np.ndarray = field(default_factory=lambda: np.array([]))  # Inductance for PC modelisation
     I: np.ndarray = field(default_factory=lambda: np.array([]))  # Current generator for PC modelisation
     M: np.ndarray = field(default_factory=lambda: np.array([]))  # Coupling factor for PC modelisation
     M_IF_PC: np.ndarray = field(default_factory=lambda: np.array([]))  # Coupling factor between PC currents and interfilament currents
 
 @dataclass
 class IFCC:
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2024.5.0/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2024.5.0/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2024.5.0/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2024.5.0/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2024.5.0/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverANSYS.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverANSYS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverPySIGMA.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2024.5.0/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserCOSIM.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserCOSIM.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserFile.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserFile.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPyBBQ.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPyCoSim.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPySIGMA.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/utils_ParserCircuits.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/utils_ParserCircuits.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsers/utils_ParserCosims.py` & `steam-sdk-2024.5.0/steam_sdk/parsers/utils_ParserCosims.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2024.5.0/steam_sdk/parsims/ParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2024.5.0/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2024.5.0/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2024.5.0/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml` & `steam-sdk-2024.5.0/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/event_column_names.yaml` & `steam-sdk-2024.5.0/steam_sdk/parsims/translation_dicts/event_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2024.5.0/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2024.5.0/steam_sdk/plotters/PlotterMap2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,22 +307,22 @@
         df["abs_err_x"] = abs(df["Bx1"] - df["Bx2"])
         df["abs_err_y"] = abs(df["By1"] - df["By2"])
         df["Bmod1"] = np.sqrt(df["Bx1"] ** 2 + df["By1"] ** 2)
         df["Bmod2"] = np.sqrt(df["Bx2"] ** 2 + df["By2"] ** 2)
         df["Bmod_error"] = abs(df["Bmod1"] - df["Bmod2"])
         return df
 
-    def generate_report_from_map2d(self, comparison_name: str, file_names: dict, plot_type: str, save: bool = True):
+    def generate_report_from_map2d(self, comparison_name: str, files_names: dict, plot_type: str, save: bool = True):
         """
         Generate plots for comparing two map2d files. Method generates the following plots:
         Bmod fields, Bmod error, relative error Bx/By, Bx/By field, Bx/By error, absolut difference Bx/By
         :return:
         """
-        sources = list(file_names.keys())
-        paths = [os.path.join(self.parsed_results_path, name) for name in file_names.values()]
+        sources = list(files_names.keys())
+        paths = [os.path.join(self.parsed_results_path, name) for name in files_names.values()]
         df = self.get_df_map2d(paths)
         fig1, ax1 = plt.subplots(2, 2, figsize=(12, 12))
         fig2, ax2 = plt.subplots(1, 2, figsize=(12, 12))
         fig3, ax3 = plt.subplots(3, 2, figsize=(12, 12))
         fig4, ax4 = plt.subplots(2, 2, figsize=(12, 12))
         fig5, ax5 = plt.subplots(2, 2, figsize=(12, 12))
         self.plot_Bmod(df, sources[0], sources[1], fig1, ax1, plot_type)
@@ -357,24 +357,19 @@
                      'B_mod_diff_std': df["Bmod_error"].std(),
                      'B_x_diff_max': abs(df["diff_x"]).max(), 'B_x_diff_mean': abs(df["diff_x"]).mean(),
                      'B_x_diff_std': abs(df["diff_x"]).std(),
                      'B_y_diff_max': abs(df["diff_y"]).max(), 'B_y_diff_mean': abs(df["diff_y"]).mean(),
                      'B_y_diff_std': abs(df["diff_y"]).std()}
 
         if save:
-            fig1.savefig(
-                os.path.join(self.parsed_results_path, f"{comparison_name}_plot_Bmod_{sources[0]}_{sources[1]}.png"))
-            fig2.savefig(os.path.join(self.parsed_results_path,
-                                      f"{comparison_name}_plot_B_mod_error_{sources[0]}_{sources[1]}.png"))
-            fig3.savefig(
-                os.path.join(self.parsed_results_path, f"{comparison_name}_plot_Bx_By_{sources[0]}_{sources[1]}.png"))
-            fig4.savefig(os.path.join(self.parsed_results_path,
-                                      f"{comparison_name}_plot_relative_error_x_y_{sources[0]}_{sources[1]}.png"))
-            fig5.savefig(os.path.join(self.parsed_results_path,
-                                      f"{comparison_name}_plot_difference_Bx_By_{sources[0]}_{sources[1]}.png"))
+            fig1.savefig(os.path.join(self.parsed_results_path, f"{comparison_name}_plot_Bmod_{sources[0]}_{sources[1]}.png"))
+            fig2.savefig(os.path.join(self.parsed_results_path, f"{comparison_name}_plot_B_mod_error_{sources[0]}_{sources[1]}.png"))
+            fig3.savefig(os.path.join(self.parsed_results_path, f"{comparison_name}_plot_Bx_By_{sources[0]}_{sources[1]}.png"))
+            fig4.savefig(os.path.join(self.parsed_results_path, f"{comparison_name}_plot_relative_error_x_y_{sources[0]}_{sources[1]}.png"))
+            fig5.savefig(os.path.join(self.parsed_results_path, f"{comparison_name}_plot_difference_Bx_By_{sources[0]}_{sources[1]}.png"))
 
         # displayWaitAndClose(waitTimeBeforeMessage=.1, waitTimeAfterMessage=0.5)
         plt.close('all')
         return to_export
 
     def plot_roxie_coil(self, roxie_data):
         xPos = []
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2024.5.0/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2024.5.0/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2024.5.0/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2024.5.0/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
     def run_metrics(self):
         """
             Function to initiate interpolation, start the different metrics and append the result to the output
         """
         # variables which need to be interpolated
         list_metrics_that_need_interpolation = ['maximum_abs_error', 'RMSE', 'RELATIVE_RMSE', 'RMSE_ratio',
-                                                'RELATIVE_RMSE_AFTER_t_PC_off', 'MARE','MARE_1S']
+                                                'RELATIVE_RMSE_AFTER_t_PC_off','_RELATIVE_RMSE_IN_INTERVAL_0_100',
+                                                'MARE','MARE_1S', 'MARE_AFTER_t_PC_off']
          # For metrics that need interpolation of both simulation data and reference data:
         if any(n in self.metrics_to_do for n in set(list_metrics_that_need_interpolation)):
 
             # Clean arrays
             var_to_interpolate_cleaned, time_vector_cleaned = self.clean_array_touple(
                 self.var_to_interpolate,
                 self.time_vector)
@@ -77,18 +78,22 @@
                 result = self._maximum_abs_error(var_of_interest,var_ref )
             elif metric == 'RMSE':
                 result = self._RMSE(var_of_interest, var_ref)
             elif metric == 'RELATIVE_RMSE':
                 result = self._RELATIVE_RMSE(var_of_interest, var_ref)
             elif metric == 'RELATIVE_RMSE_AFTER_t_PC_off':
                 result = self._RELATIVE_RMSE_AFTER_t_PC_off(var_of_interest, var_ref,time_stamps_overlap)
+            elif metric == '_RELATIVE_RMSE_IN_INTERVAL_0_100':
+                result = self._RELATIVE_RMSE_IN_INTERVAL_0_100(var_of_interest, var_ref,time_stamps_overlap)
             elif metric == 'RMSE_ratio':
                 result = self._RMSE_ratio(var_of_interest, var_ref)
             elif metric == 'MARE':
                 result = self._MARE(var_of_interest, var_ref) # Calculate Mean Absolute Relative Error (MARE)
+            elif metric == 'MARE_AFTER_t_PC_off':
+                result = self._MARE_AFTER_t_PC_off(var_of_interest, var_ref,time_stamps_overlap)
             elif metric == 'MARE_1S':
                 result = self._MARE_1S(var_of_interest,var_ref,time_stamps_overlap)
             elif metric == 'quench_load_error':
                 result = self._quench_load_error(time_vector, var_of_interest, time_vector_ref, var_ref)
             elif metric == 'quench_load':
                 result = self._quench_load(time_vector, var_of_interest)
             elif metric == 'max':
@@ -123,25 +128,41 @@
             function to calculate the RMSE between simulation and measurement
         """
 
         return float(np.sqrt(((y - y_ref) ** 2).mean()) )# np.sqrt(mean_squared_error(y, y_ref))
 
     @staticmethod
     def _RELATIVE_RMSE(y, y_ref)-> float:
-
         """
             function to calculate the RMSE between simulation and measurement, but normalized to the maximum reference value
         """
         avoid_zero_division = 1e-10
         max_abs_y_ref = np.max(np.abs(y_ref)) + avoid_zero_division
         RELATIVE_RMSE = np.sqrt(((y - y_ref) ** 2).mean())/max_abs_y_ref
 
         return float(RELATIVE_RMSE) # np.sqrt(mean_squared_error(y, y_ref))
 
-    def _RELATIVE_RMSE_AFTER_t_PC_off(self, y, y_ref,time_stamps_overlap)-> float:
+    @staticmethod
+    def _RELATIVE_RMSE_AFTER_t_PC_off(y, y_ref,time_stamps_overlap)-> float:
+        """
+        Calculate the relative RMSE after t_PC_off.
+
+        Parameters:
+        - y: Array-like, observed values.
+        - y_ref: Array-like, reference values.
+        - time_stamps_overlap: Array-like, time stamps corresponding to the overlap between y and y_ref.
+
+        Returns:
+        - float: Relative RMSE calculated after t_PC_off.
+
+        This function calculates the relative Root Mean Square Error (RMSE) between observed values (y)
+        and reference values (y_ref) after the t_PC_off time point. It considers only the data points
+        occurring after t_PC_off for the calculation.
+        RMSE is set into relation to the maximum value of the reference dataset.
+        """
         y_after_t_PC_off = []
         y_ref_after_t_PC_off = []
 
         for index, timestamp in enumerate(time_stamps_overlap):
             if (0 <= timestamp):
                 y_after_t_PC_off.append(y[index])
                 y_ref_after_t_PC_off.append(y_ref[index])
@@ -149,14 +170,81 @@
         y_after_t_PC_off = np.array(y_after_t_PC_off)
         y_ref_after_t_PC_off = np.array(y_ref_after_t_PC_off)
 
         avoid_zero_division = 1e-10
         max_abs_y_ref_after_t_PC_off = np.max(np.abs(y_ref_after_t_PC_off)) + avoid_zero_division
         RELATIVE_RMSE_AFTER_t_PC_off = np.sqrt(((y_after_t_PC_off - y_ref_after_t_PC_off) ** 2).mean()) / max_abs_y_ref_after_t_PC_off
 
+        return float(RELATIVE_RMSE_AFTER_t_PC_off)
+
+    @staticmethod
+    def _MARE_AFTER_t_PC_off(y, y_ref, time_stamps_overlap) -> float:
+        """
+        Calculate the Mean Average Relative Error after t_PC_off.
+
+        Parameters:
+        - y: Array-like, observed values.
+        - y_ref: Array-like, reference values.
+        - time_stamps_overlap: Array-like, time stamps corresponding to the overlap between y and y_ref.
+
+        Returns:
+        - float: MARE calculated after t_PC_off.
+
+        This function calculates the MARE between observed values (y)
+        and reference values (y_ref) after the t_PC_off time point. It considers only the data points
+        occurring after t_PC_off for the calculation.
+        """
+        y_after_t_PC_off = []
+        y_ref_after_t_PC_off = []
+
+        for index, timestamp in enumerate(time_stamps_overlap):
+            if (0 <= timestamp):
+                y_after_t_PC_off.append(y[index])
+                y_ref_after_t_PC_off.append(y_ref[index])
+
+        y_after_t_PC_off = np.array(y_after_t_PC_off)
+        y_ref_after_t_PC_off = np.array(y_ref_after_t_PC_off)
+
+        avoid_zero_division = 1e-10
+        MARE = np.abs((y_after_t_PC_off - y_ref_after_t_PC_off)/(y_ref_after_t_PC_off+avoid_zero_division)).mean()
+        return float(MARE)
+
+    @staticmethod
+    def _RELATIVE_RMSE_IN_INTERVAL_0_100(y, y_ref,time_stamps_overlap)-> float:
+        """
+        Calculate the relative RMSE in a time interval from 0 to 100 seconds after t_PC_off.
+
+        Parameters:
+        - y: Array-like, observed values.
+        - y_ref: Array-like, reference values.
+        - time_stamps_overlap: Array-like, time stamps corresponding to the overlap between y and y_ref.
+
+        Returns:
+        - float: Relative RMSE calculated within the specified time interval.
+
+        This function calculates the relative Root Mean Square Error (RMSE) between observed values (y)
+        and reference values (y_ref) within a specified time interval [0, 100] seconds after t_PC_off.
+        It considers only the data points within this time interval for the calculation.
+        RMSE is set into relation to the maximum value of the reference dataset.
+        """
+        y_intervall = []
+        y_ref_intervall = []
+
+        for index, timestamp in enumerate(time_stamps_overlap):
+            if (0 <= timestamp and timestamp <=100) :
+                y_intervall.append(y[index])
+                y_ref_intervall.append(y_ref[index])
+
+        y_intervall = np.array(y_intervall)
+        y_ref_intervall = np.array(y_ref_intervall)
+
+        avoid_zero_division = 1e-10
+        max_abs_y_ref_intervall = np.max(np.abs(y_ref_intervall)) + avoid_zero_division
+        RELATIVE_RMSE_AFTER_t_PC_off = np.sqrt(((y_intervall - y_ref_intervall) ** 2).mean()) / max_abs_y_ref_intervall
+
         return float(RELATIVE_RMSE_AFTER_t_PC_off)  # np.sqrt(mean_squared_error(y, y_ref))
 
     @staticmethod
     def _MARE(y,y_ref) -> float:
         "Calculate Mean Absolute Relative Error (MARE)"
         avoid_zero_division = 1e-10
         MARE = np.abs((y - y_ref)/(y_ref+avoid_zero_division)).mean()
```

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2024.5.0/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2024.5.0/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2024.5.0/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2024.5.0/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/ParserRoxieHelpers.py` & `steam-sdk-2024.5.0/steam_sdk/utils/ParserRoxieHelpers.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/attribute_model.py` & `steam-sdk-2024.5.0/steam_sdk/utils/attribute_model.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2024.5.0/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/compare_simulations.py` & `steam-sdk-2024.5.0/steam_sdk/utils/compare_simulations.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2024.5.0/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/correct_RRR_NIST.py` & `steam-sdk-2024.5.0/steam_sdk/utils/correct_RRR_NIST.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2024.5.0/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/make_folder_if_not_existing.py` & `steam-sdk-2024.5.0/steam_sdk/utils/make_folder_if_not_existing.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/misc.py` & `steam-sdk-2024.5.0/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2024.5.0/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/read_settings_file.py` & `steam-sdk-2024.5.0/steam_sdk/utils/read_settings_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/reformat_figure.py` & `steam-sdk-2024.5.0/steam_sdk/utils/reformat_figure.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/tic_toc.py` & `steam-sdk-2024.5.0/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/utils/utils_PC.py` & `steam-sdk-2024.5.0/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/viewers/Viewer.py` & `steam-sdk-2024.5.0/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2024.5.0/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.4.0/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2024.5.0/steam_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: STEAM,API,SDK,CERN
+Keywords: STEAM,CERN,API,SDK
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
```

### Comparing `steam-sdk-2024.4.0/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2024.5.0/steam_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 steam_sdk/data/DataModelCircuit.py
 steam_sdk/data/DataModelCommon.py
 steam_sdk/data/DataModelConductor.py
 steam_sdk/data/DataModelCosim.py
 steam_sdk/data/DataModelMagnet.py
 steam_sdk/data/DataModelParsimDakota.py
 steam_sdk/data/DataParsimConductor.py
+steam_sdk/data/DataPlot.py
 steam_sdk/data/DataProteCCT.py
 steam_sdk/data/DataProteCCTOptions.py
 steam_sdk/data/DataPyBBQ.py
 steam_sdk/data/DataPyBBQOptions.py
 steam_sdk/data/DataPyCoSim.py
 steam_sdk/data/DataPySIGMA.py
 steam_sdk/data/DataPySIGMAOptions.py
@@ -130,14 +131,15 @@
 steam_sdk/parsims/ParsimDakota.py
 steam_sdk/parsims/ParsimEventCircuit.py
 steam_sdk/parsims/ParsimEventMagnet.py
 steam_sdk/parsims/__init__.py
 steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
 steam_sdk/parsims/translation_dicts/event_column_names.yaml
 steam_sdk/plotters/PlotterAnalysis.py
+steam_sdk/plotters/PlotterGriddedData.py
 steam_sdk/plotters/PlotterMap2d.py
 steam_sdk/plotters/PlotterModel.py
 steam_sdk/plotters/PlotterParametric.py
 steam_sdk/plotters/PlotterRoxie.py
 steam_sdk/plotters/__init__.py
 steam_sdk/postprocs/PostprocsMetrics.py
 steam_sdk/postprocs/__init__.py
```

### Comparing `steam-sdk-2024.4.0/steam_sdk.egg-info/requires.txt` & `steam-sdk-2024.5.0/steam_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

